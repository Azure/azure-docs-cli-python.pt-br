---
title: Notas de versão da CLI do Azure
description: Saiba mais sobre as últimas atualizações da CLI do Azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/26/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 75a3a3ee800edc20bd1c8ed7ab1ff542f5935c6c
ms.sourcegitcommit: 443e14098d6643cdb2e178847d1c79b1b95146ce
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/26/2019
ms.locfileid: "74543461"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="48988-103">Notas de versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="48988-103">Azure CLI release notes</span></span>

## <a name="november-26-2019"></a><span data-ttu-id="48988-104">26 de novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="48988-104">November 26, 2019</span></span>

<span data-ttu-id="48988-105">Versão 2.0.77</span><span class="sxs-lookup"><span data-stu-id="48988-105">Version 2.0.77</span></span>

### <a name="acr"></a><span data-ttu-id="48988-106">ACR</span><span class="sxs-lookup"><span data-stu-id="48988-106">ACR</span></span>

* <span data-ttu-id="48988-107">Parâmetro `--branch` preterido de acr task create/update</span><span class="sxs-lookup"><span data-stu-id="48988-107">Deprecated paramater `--branch` from acr task create/update</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="48988-108">Red Hat OpenShift no Azure</span><span class="sxs-lookup"><span data-stu-id="48988-108">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="48988-109">Sinalizador `--workspace-resource-id` adicionado para permitir a criação do cluster do Red Hat OpenShift no Azure com monitoramento</span><span class="sxs-lookup"><span data-stu-id="48988-109">Added `--workspace-resource-id` flag to allow creation of Azure Red Hat Openshift cluster with monitoring</span></span>
* <span data-ttu-id="48988-110">`monitor_profile` adicionado para criar o cluster do Red Hat OpenShift no Azure com monitoramento</span><span class="sxs-lookup"><span data-stu-id="48988-110">Added `monitor_profile` to create Azure Red Hat OpenShift cluster with monitoring</span></span>

### <a name="aks"></a><span data-ttu-id="48988-111">AKS</span><span class="sxs-lookup"><span data-stu-id="48988-111">AKS</span></span>

* <span data-ttu-id="48988-112">Operação de rotação de certificado de cluster de suporte adicionada usando "az aks rotate-certs".</span><span class="sxs-lookup"><span data-stu-id="48988-112">Added support cluster certificate rotation operation using "az aks rotate-certs".</span></span>

### <a name="appconfig"></a><span data-ttu-id="48988-113">AppConfig</span><span class="sxs-lookup"><span data-stu-id="48988-113">AppConfig</span></span>

* <span data-ttu-id="48988-114">Suporte adicionado para usar ":" para o separador `as az appconfig kv import`</span><span class="sxs-lookup"><span data-stu-id="48988-114">Added support for using ":" for `as az appconfig kv import` separator</span></span>
* <span data-ttu-id="48988-115">Problema corrigido para listar valores de chave com vários rótulos incluindo o rótulo nulo.</span><span class="sxs-lookup"><span data-stu-id="48988-115">Fixed issue for listing key values with multiple labels including null label.</span></span> 
* <span data-ttu-id="48988-116">SDK do plano de gerenciamento atualizado, azure-mgmt-appconfiguration, para a versão 0.3.0.</span><span class="sxs-lookup"><span data-stu-id="48988-116">Updated management plane sdk, azure-mgmt-appconfiguration, to version 0.3.0.</span></span> 

### <a name="appservice"></a><span data-ttu-id="48988-117">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-117">AppService</span></span>

* <span data-ttu-id="48988-118">Problema corrigido nº 11100: AttributeError para az webapp up ao criar o plano de serviço</span><span class="sxs-lookup"><span data-stu-id="48988-118">Fixed issue #11100: AttributeError for az webapp up when create service plan</span></span>
* <span data-ttu-id="48988-119">az webapp up: Forçar a criação ou a implantação em um site para linguagens com suporte, nenhum padrão usado.</span><span class="sxs-lookup"><span data-stu-id="48988-119">az webapp up: Forcing the creation or deployment to a site for supported languages, no defaults used.</span></span>
* <span data-ttu-id="48988-120">Suporte adicionado para o Ambiente do Serviço de Aplicativo: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span><span class="sxs-lookup"><span data-stu-id="48988-120">Added support for App Service Environment: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span></span>

### <a name="backup"></a><span data-ttu-id="48988-121">Backup</span><span class="sxs-lookup"><span data-stu-id="48988-121">Backup</span></span>

* <span data-ttu-id="48988-122">Problema corrigido em list-associated-items da política de backup az.</span><span class="sxs-lookup"><span data-stu-id="48988-122">Fixed issue in az backup policy list-associated-items.</span></span> <span data-ttu-id="48988-123">Parâmetro BackupManagementType opcional adicionado.</span><span class="sxs-lookup"><span data-stu-id="48988-123">Added optional BackupManagementType parameter.</span></span>

### <a name="compute"></a><span data-ttu-id="48988-124">Computação</span><span class="sxs-lookup"><span data-stu-id="48988-124">Compute</span></span>

* <span data-ttu-id="48988-125">Versão de API de computação, discos e instantâneos atualizados para 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="48988-125">Upgraded API version of compute, disks, snapshots to 2019-07-01</span></span>
* <span data-ttu-id="48988-126">vmss create: melhoria para --orchestration-mode</span><span class="sxs-lookup"><span data-stu-id="48988-126">vmss create: Improvement for --orchestration-mode</span></span>
* <span data-ttu-id="48988-127">sig image-definition create: --os-state adicionado para permitir a especificação se as máquinas virtuais criadas nessa imagem são 'Generalizadas' ou 'Especializadas'</span><span class="sxs-lookup"><span data-stu-id="48988-127">sig image-definition create: Added --os-state to allow specifying whether the virtual machines created under this image are 'Generalized' or 'Specialized'</span></span>
* <span data-ttu-id="48988-128">sig image-definition create: --hyper-v-generation adicionado para permitir a especificação da geração do hipervisor</span><span class="sxs-lookup"><span data-stu-id="48988-128">sig image-definition create: Added --hyper-v-generation to allow specifying the hypervisor generation</span></span>
* <span data-ttu-id="48988-129">sig image-version create: --os-snapshot e --data-snapshots de suporte adicionados</span><span class="sxs-lookup"><span data-stu-id="48988-129">sig image-version create: Added support --os-snapshot and --data-snapshots</span></span>
* <span data-ttu-id="48988-130">image create: --data-disk-caching adicionado para permitir a especificação da configuração de cache de discos de dados</span><span class="sxs-lookup"><span data-stu-id="48988-130">image create: Added --data-disk-caching to allow specifying caching setting of data disks</span></span>
* <span data-ttu-id="48988-131">SDK de computação do Python atualizado para 10.0.0</span><span class="sxs-lookup"><span data-stu-id="48988-131">Upgraded Python Compute SDK to 10.0.0</span></span>
* <span data-ttu-id="48988-132">vm/vmss create: 'Spot' adicionado à propriedade de enumeração 'Priority'</span><span class="sxs-lookup"><span data-stu-id="48988-132">vm/vmss create: Added 'Spot' to 'Priority' enum property</span></span>
* <span data-ttu-id="48988-133">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro '--max-billing' renomeado para '--max-price', para a VM e o VMSS, a fim de que seja consistente com os cmdlets do Swagger e do PowerShell</span><span class="sxs-lookup"><span data-stu-id="48988-133">[Breaking change] Renamed '--max-billing' parameter to '--max-price', for both VM and VMSS, to be consistent with Swagger and Powershell cmdlets</span></span>
* <span data-ttu-id="48988-134">vm monitor log show: suporte adicionado para consultar o log pelo workspace do Log Analytics vinculado.</span><span class="sxs-lookup"><span data-stu-id="48988-134">vm monitor log show: Added support for querying log over linked log analytics workspace.</span></span>

### <a name="iot"></a><span data-ttu-id="48988-135">IOT</span><span class="sxs-lookup"><span data-stu-id="48988-135">IOT</span></span>

* <span data-ttu-id="48988-136">Correção nº 2531: argumentos de conveniência adicionados para a atualização do hub.</span><span class="sxs-lookup"><span data-stu-id="48988-136">Fix #2531: Added convenience arguments for hub update.</span></span>
* <span data-ttu-id="48988-137">Correção nº 8323: parâmetros ausentes adicionados para criar o ponto de extremidade personalizado de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="48988-137">Fix #8323: Added missing parameters to create storage custom endpoint.</span></span>
* <span data-ttu-id="48988-138">Corrigir bug de regressão: as alterações que substituem o ponto de extremidade de armazenamento padrão foram revertidas.</span><span class="sxs-lookup"><span data-stu-id="48988-138">Fix regression bug: Reverted the changes which overrides the default storage endpoint.</span></span>

### <a name="key-vault"></a><span data-ttu-id="48988-139">Key Vault</span><span class="sxs-lookup"><span data-stu-id="48988-139">Key Vault</span></span>

* <span data-ttu-id="48988-140">Correção nº 11121: ao usar `az keyvault certificate list`, passar `--include-pending` agora não exige um valor de `true` ou `false`</span><span class="sxs-lookup"><span data-stu-id="48988-140">Fixed #11121: When using `az keyvault certificate list`, passing `--include-pending` now doesn't require a value of `true` or `false`</span></span>

### <a name="netappfiles"></a><span data-ttu-id="48988-141">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="48988-141">NetAppFiles</span></span>

* <span data-ttu-id="48988-142">azure-mgmt-netapp atualizado para 0.7.0 que inclui algumas propriedades de volume adicionais associadas a operações de replicação futuras</span><span class="sxs-lookup"><span data-stu-id="48988-142">Upgraded azure-mgmt-netapp to 0.7.0 which includes some additional volume properties associated with upcoming replication operations</span></span>

### <a name="network"></a><span data-ttu-id="48988-143">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-143">Network</span></span>

* <span data-ttu-id="48988-144">application-gateway waf-config: preterido</span><span class="sxs-lookup"><span data-stu-id="48988-144">application-gateway waf-config: deprecated</span></span>
* <span data-ttu-id="48988-145">application-gateway waf-policy: subgrupo managed-rules adicionado para gerenciar os conjuntos de regras e regras de exclusão gerenciados</span><span class="sxs-lookup"><span data-stu-id="48988-145">application-gateway waf-policy: Added subgroup managed-rules to manage managed rule sets and exclusion rules</span></span>
* <span data-ttu-id="48988-146">application-gateway waf-policy: subgrupo policy-setting adicionado para gerenciar a configuração global de um waf-policy</span><span class="sxs-lookup"><span data-stu-id="48988-146">application-gateway waf-policy: Added subgroup policy-setting to manage global configuration of a waf-policy</span></span>
* <span data-ttu-id="48988-147">[ALTERAÇÃO SIGNIFICATIVA] application-gateway waf-policy: subgrupo rule renomeado para custom-rule</span><span class="sxs-lookup"><span data-stu-id="48988-147">[BREAKING CHANGE] application-gateway waf-policy: Renamed subgroup rule to custom-rule</span></span>
* <span data-ttu-id="48988-148">application-gateway http-listener: --firewall-policy adicionado durante a criação</span><span class="sxs-lookup"><span data-stu-id="48988-148">application-gateway http-listener: Added --firewall-policy when create</span></span>
* <span data-ttu-id="48988-149">application-gateway url-path-map rule: --firewall-policy adicionado durante a criação</span><span class="sxs-lookup"><span data-stu-id="48988-149">application-gateway url-path-map rule: Added --firewall-policy when create</span></span>

### <a name="packaging"></a><span data-ttu-id="48988-150">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="48988-150">Packaging</span></span>

* <span data-ttu-id="48988-151">Wrapper az reescrito no Python</span><span class="sxs-lookup"><span data-stu-id="48988-151">Rewrote the az wrapper in Python</span></span>
* <span data-ttu-id="48988-152">Suporte adicionado para Python 3.8</span><span class="sxs-lookup"><span data-stu-id="48988-152">Added support for Python 3.8</span></span>
* <span data-ttu-id="48988-153">Alterado para Python 3 para o pacote RPM</span><span class="sxs-lookup"><span data-stu-id="48988-153">Changed to Python 3 for RPM package</span></span>

### <a name="profile"></a><span data-ttu-id="48988-154">Perfil</span><span class="sxs-lookup"><span data-stu-id="48988-154">Profile</span></span>

* <span data-ttu-id="48988-155">Erro aperfeiçoado ao executar `az login -u {} -p {}` com a conta Microsoft</span><span class="sxs-lookup"><span data-stu-id="48988-155">Polished error when running `az login -u {} -p {}` with Microsoft account</span></span>
* <span data-ttu-id="48988-156">`SSLError` aperfeiçoado ao executar `az login` atrás de um proxy com o certificado raiz autoassinado</span><span class="sxs-lookup"><span data-stu-id="48988-156">Polished `SSLError` when running `az login` behind a proxy with self-signed root certificate</span></span>
* <span data-ttu-id="48988-157">Correção nº 10578: `az login` trava quando mais de uma instância é iniciada ao mesmo tempo no Windows ou WSL</span><span class="sxs-lookup"><span data-stu-id="48988-157">Fixed #10578: `az login` hangs when more than one instances are launched at the same time on Windows or WSL</span></span>
* <span data-ttu-id="48988-158">Correção nº 11059: `az login --allow-no-subscriptions` falhará se houver assinaturas no locatário</span><span class="sxs-lookup"><span data-stu-id="48988-158">Fixed #11059: `az login --allow-no-subscriptions` fails if there are subscriptions in the tenant</span></span>
* <span data-ttu-id="48988-159">Correção nº 11238: após renomear uma assinatura, fazer logon com a MSI fará a mesma assinatura aparecer duas vezes</span><span class="sxs-lookup"><span data-stu-id="48988-159">Fixed #11238: After renaming a subscription, logging in with MSI will result in the same subscription appearing twice</span></span>

### <a name="rbac"></a><span data-ttu-id="48988-160">RBAC</span><span class="sxs-lookup"><span data-stu-id="48988-160">RBAC</span></span>

* <span data-ttu-id="48988-161">Correção nº 10996: erro aperfeiçoado para `--force-change-password-next-login` em `az ad user update` quando `--password` não for especificado</span><span class="sxs-lookup"><span data-stu-id="48988-161">Fixed #10996: Polish error for `--force-change-password-next-login` in `az ad user update` when `--password` is not specified</span></span>

### <a name="redis"></a><span data-ttu-id="48988-162">Redis</span><span class="sxs-lookup"><span data-stu-id="48988-162">Redis</span></span>

* <span data-ttu-id="48988-163">Correção nº 2902: evite definir configurações de memória ao atualizar o cache do SKU básico</span><span class="sxs-lookup"><span data-stu-id="48988-163">Fixed #2902: Avoid setting memory configs while updating Basic SKU cache</span></span>

### <a name="reservations"></a><span data-ttu-id="48988-164">Reservas</span><span class="sxs-lookup"><span data-stu-id="48988-164">Reservations</span></span>

* <span data-ttu-id="48988-165">Versão do SDK atualizada para 0.6.0</span><span class="sxs-lookup"><span data-stu-id="48988-165">Upgraded SDK Version to 0.6.0</span></span>
* <span data-ttu-id="48988-166">Informações de detalhes do plano de cobrança atualizadas após chamar Get-Gatalogs</span><span class="sxs-lookup"><span data-stu-id="48988-166">Added billingplan details info after calling Get-Gatalogs</span></span>
* <span data-ttu-id="48988-167">Novo comando `az reservations reservation-order calculate` adicionado para calcular o preço de uma reserva</span><span class="sxs-lookup"><span data-stu-id="48988-167">Added new command `az reservations reservation-order calculate` to calculate the price for a reservation</span></span>
* <span data-ttu-id="48988-168">Novo comando `az reservations reservation-order purchase` adicionado para comprar uma nova reserva</span><span class="sxs-lookup"><span data-stu-id="48988-168">Added new command `az reservations reservation-order purchase` to purchase a new reservation</span></span>

### <a name="rest"></a><span data-ttu-id="48988-169">Rest</span><span class="sxs-lookup"><span data-stu-id="48988-169">Rest</span></span>
* <span data-ttu-id="48988-170">`az rest` alterado para GA</span><span class="sxs-lookup"><span data-stu-id="48988-170">Changed `az rest` to GA</span></span>

### <a name="sql"></a><span data-ttu-id="48988-171">SQL</span><span class="sxs-lookup"><span data-stu-id="48988-171">SQL</span></span>

* <span data-ttu-id="48988-172">azure-mgmt-sql atualizado para 0.15.0.</span><span class="sxs-lookup"><span data-stu-id="48988-172">Updated azure-mgmt-sql to version 0.15.0.</span></span>

### <a name="storage"></a><span data-ttu-id="48988-173">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48988-173">Storage</span></span>

* <span data-ttu-id="48988-174">storage account create: --enable-hierarchical-namespace adicionado para dar suporte à semântica do sistema de arquivos no serviço Blob.</span><span class="sxs-lookup"><span data-stu-id="48988-174">storage account create: Added --enable-hierarchical-namespace to support filesystem semantics in blob service.</span></span>
* <span data-ttu-id="48988-175">Exceção não relacionada removida da mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="48988-175">Removed unrelated exception from error message</span></span>
* <span data-ttu-id="48988-176">Problemas corrigidos com a mensagem de erro incorreta "Você não tem as permissões necessárias para executar essa operação."</span><span class="sxs-lookup"><span data-stu-id="48988-176">Fixed issues with incorrect error message "You do not have the required permissions needed to perform this operation."</span></span> <span data-ttu-id="48988-177">quando bloqueado pelas regras de rede ou AuthenticationFailed.</span><span class="sxs-lookup"><span data-stu-id="48988-177">when blocked by network rules or AuthenticationFailed.</span></span>

## <a name="november-4-2019"></a><span data-ttu-id="48988-178">4 de novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="48988-178">November 4, 2019</span></span>

<span data-ttu-id="48988-179">Versão 2.0.76</span><span class="sxs-lookup"><span data-stu-id="48988-179">Version 2.0.76</span></span>

### <a name="acr"></a><span data-ttu-id="48988-180">ACR</span><span class="sxs-lookup"><span data-stu-id="48988-180">ACR</span></span>

* <span data-ttu-id="48988-181">O parâmetro de versão prévia `--pack-image-tag` foi adicionado ao comando `az acr pack build`.</span><span class="sxs-lookup"><span data-stu-id="48988-181">Added a preview parameter `--pack-image-tag` to command `az acr pack build`.</span></span>
* <span data-ttu-id="48988-182">Suporte adicionado para habilitar a auditoria na criação de um registro</span><span class="sxs-lookup"><span data-stu-id="48988-182">Added support for enabling auditing on creating a registry</span></span>
* <span data-ttu-id="48988-183">Suporte adicionado para o RBAC com escopo de repositório</span><span class="sxs-lookup"><span data-stu-id="48988-183">Added support for Repository-scoped RBAC</span></span>

### <a name="aks"></a><span data-ttu-id="48988-184">AKS</span><span class="sxs-lookup"><span data-stu-id="48988-184">AKS</span></span>

* <span data-ttu-id="48988-185">`--enable-cluster-autoscaler`, `--min-count` e `--max-count` foram adicionados ao comando `az aks create`, que habilita o dimensionamento automático do cluster para o pool de nós.</span><span class="sxs-lookup"><span data-stu-id="48988-185">Added `--enable-cluster-autoscaler`, `--min-count` and `--max-count` to the `az aks create` command, which enables cluster autoscaler for the node pool.</span></span>
* <span data-ttu-id="48988-186">Foram adicionados os sinalizadores acima, bem como `--update-cluster-autoscaler` e `--disable-cluster-autoscaler` ao comando `az aks update`, permitindo atualizações do cluster de dimensionamento automático.</span><span class="sxs-lookup"><span data-stu-id="48988-186">Added the above flags as well as `--update-cluster-autoscaler` and `--disable-cluster-autoscaler` to the `az aks update` command, allowing updates to cluster autoscaler.</span></span>

### <a name="appconfig"></a><span data-ttu-id="48988-187">AppConfig</span><span class="sxs-lookup"><span data-stu-id="48988-187">AppConfig</span></span>

* <span data-ttu-id="48988-188">O grupo de comandos do recurso AppConfig foi adicionado para gerenciar os sinalizadores de recurso armazenados em uma Configuração de Aplicativos.</span><span class="sxs-lookup"><span data-stu-id="48988-188">Added appconfig feature command group to manage feature flags stored in an App Configuration.</span></span>
* <span data-ttu-id="48988-189">Foi corrigido um bug secundário do comando de exportação para arquivo appconfig kv.</span><span class="sxs-lookup"><span data-stu-id="48988-189">Fixed minor bug for appconfig kv export to file command.</span></span> <span data-ttu-id="48988-190">Foi interrompida a leitura de conteúdo do arquivo de destino durante a exportação.</span><span class="sxs-lookup"><span data-stu-id="48988-190">Stop reading dest file contents during export.</span></span>

### <a name="appservice"></a><span data-ttu-id="48988-191">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-191">AppService</span></span>

* <span data-ttu-id="48988-192">`az appservice plan create`: Foi adicionado o suporte para definir 'persitecalling' no comando appservice plan create.</span><span class="sxs-lookup"><span data-stu-id="48988-192">`az appservice plan create`: Added support to set 'persitescaling' on appservice plan create.</span></span>
* <span data-ttu-id="48988-193">Foi corrigido um problema em que a operação webapp config ssl bind estava removendo as marcas existentes do recurso</span><span class="sxs-lookup"><span data-stu-id="48988-193">Fixed an issue where webapp config ssl bind operation was removing existing tags from the resource</span></span>
* <span data-ttu-id="48988-194">Foi adicionado o sinalizador `--build-remote` para `az functionapp deployment source config-zip` para dar suporte à ação de build remoto durante a implantação do aplicativo de funções.</span><span class="sxs-lookup"><span data-stu-id="48988-194">Added `--build-remote` flag for `az functionapp deployment source config-zip` to support remote build action during function app deployment.</span></span>
* <span data-ttu-id="48988-195">Foi alterada a versão do nó padrão em aplicativos de funções para ~10 para Windows</span><span class="sxs-lookup"><span data-stu-id="48988-195">Changed default node version on function apps to ~10 for Windows</span></span>
* <span data-ttu-id="48988-196">A propriedade `--runtime-version` foi adicionada a `az functionapp create`</span><span class="sxs-lookup"><span data-stu-id="48988-196">Added `--runtime-version` property to `az functionapp create`</span></span>

### <a name="arm"></a><span data-ttu-id="48988-197">ARM</span><span class="sxs-lookup"><span data-stu-id="48988-197">ARM</span></span>

* <span data-ttu-id="48988-198">`az deployment/group deployment validate`: Foi adicionado o parâmetro `--handle-extended-json-format` para dar suporte a várias linhas e comentários no modelo JSON durante a implantação.</span><span class="sxs-lookup"><span data-stu-id="48988-198">`az deployment/group deployment validate`: Added `--handle-extended-json-format` parameter to support multiline and comments in json template when deployment.</span></span>
* <span data-ttu-id="48988-199">O azure-mgmt-resource passou a usar a 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="48988-199">Bumped azure-mgmt-resource to 2019-07-01</span></span>

### <a name="backup"></a><span data-ttu-id="48988-200">Backup</span><span class="sxs-lookup"><span data-stu-id="48988-200">Backup</span></span>

* <span data-ttu-id="48988-201">Foi adicionado o suporte de backup aos Arquivos do Azure</span><span class="sxs-lookup"><span data-stu-id="48988-201">Added AzureFiles backup support</span></span>

### <a name="compute"></a><span data-ttu-id="48988-202">Computação</span><span class="sxs-lookup"><span data-stu-id="48988-202">Compute</span></span>

* <span data-ttu-id="48988-203">`az vm create`: foi adicionado um aviso ao especificar a rede acelerada e um adaptador de rede existente juntos.</span><span class="sxs-lookup"><span data-stu-id="48988-203">`az vm create`: Added warning when specifying accelerated networking and an existing NIC together.</span></span>
* <span data-ttu-id="48988-204">`az vm create`: foi adicionado `--vmss` para especificar um conjunto de dimensionamento de máquinas virtuais existente ao qual a máquina virtual deve ser atribuída.</span><span class="sxs-lookup"><span data-stu-id="48988-204">`az vm create`: Added `--vmss` to specify an existing virtual machine scale set that the virtual machine should be assigned to.</span></span>
* <span data-ttu-id="48988-205">`az vm/vmss create`: foi adicionada uma cópia local do arquivo de alias de imagem para que ele possa ser acessado em um ambiente de rede restrita.</span><span class="sxs-lookup"><span data-stu-id="48988-205">`az vm/vmss create`: Added a local copy of image alias file so that it can be accessed in a restricted network environment.</span></span>
* <span data-ttu-id="48988-206">`az vmss create`: foi adicionado `--orchestration-mode` para especificar como as máquinas virtuais são gerenciadas pelo conjunto de dimensionamento.</span><span class="sxs-lookup"><span data-stu-id="48988-206">`az vmss create`: Added `--orchestration-mode` to specify how virtual machines are managed by the scale set.</span></span>
* <span data-ttu-id="48988-207">`az vm/vmss update`: foi adicionado `--ultra-ssd-enabled` para permitir a atualização da configuração de SSD Ultra.</span><span class="sxs-lookup"><span data-stu-id="48988-207">`az vm/vmss update`: Added `--ultra-ssd-enabled` to allow updating ultra SSD setting.</span></span>
* <span data-ttu-id="48988-208">[ALTERAÇÃO DA FALHA] `az vm extension set`: foi corrigido o bug em que os usuários não podiam definir uma extensão em uma VM com `--ids`.</span><span class="sxs-lookup"><span data-stu-id="48988-208">[BREAKING CHANGE] `az vm extension set`: Fixed bug where users could not set an extension on a VM with `--ids`.</span></span>
* <span data-ttu-id="48988-209">Foram adicionados os novos comandos `az vm image terms accept/cancel/show` para gerenciar os termos de imagem do Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="48988-209">Added new commands `az vm image terms accept/cancel/show` to manage Azure Marketplace image terms.</span></span>
* <span data-ttu-id="48988-210">O VMAccessForLinux foi atualizado para a versão 1.5</span><span class="sxs-lookup"><span data-stu-id="48988-210">Updated VMAccessForLinux to version 1.5</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="48988-211">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="48988-211">CosmosDB</span></span>

* <span data-ttu-id="48988-212">[ALTERAÇÃO DA FALHA] `az sql container create`: `--partition-key-path` foi alterado para parâmetro obrigatório</span><span class="sxs-lookup"><span data-stu-id="48988-212">[BREAKING CHANGE] `az sql container create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="48988-213">[ALTERAÇÃO DA FALHA] `az gremlin graph create`: `--partition-key-path` foi alterado para parâmetro obrigatório</span><span class="sxs-lookup"><span data-stu-id="48988-213">[BREAKING CHANGE] `az gremlin graph create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="48988-214">`az sql container create`: Adição de `--unique-key-policy` e `--conflict-resolution-policy`</span><span class="sxs-lookup"><span data-stu-id="48988-214">`az sql container create`: Added `--unique-key-policy` and `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="48988-215">`az sql container create/update`: o esquema padrão `--idx` foi atualizado</span><span class="sxs-lookup"><span data-stu-id="48988-215">`az sql container create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="48988-216">`gremlin graph create`: Adicionado `--conflict-resolution-policy`</span><span class="sxs-lookup"><span data-stu-id="48988-216">`gremlin graph create`: Added `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="48988-217">`gremlin graph create/update`: o esquema padrão `--idx` foi atualizado</span><span class="sxs-lookup"><span data-stu-id="48988-217">`gremlin graph create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="48988-218">Erro de digitação corrigido na mensagem de ajuda</span><span class="sxs-lookup"><span data-stu-id="48988-218">Fixed typo in help message</span></span>
* <span data-ttu-id="48988-219">banco de dados: foram adicionadas informações sobre preteridos</span><span class="sxs-lookup"><span data-stu-id="48988-219">database: Added deprecation infomation</span></span>
* <span data-ttu-id="48988-220">coleção: foram adicionadas informações sobre preteridos</span><span class="sxs-lookup"><span data-stu-id="48988-220">collection: Added deprecation infomation</span></span>

### <a name="iot"></a><span data-ttu-id="48988-221">IoT</span><span class="sxs-lookup"><span data-stu-id="48988-221">IoT</span></span>

* <span data-ttu-id="48988-222">Um novo tipo de fonte de roteamento foi adicionado: DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="48988-222">Added new routing source type: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="48988-223">Foi corrigido o erro de recursos ausentes no `az iot hub create`</span><span class="sxs-lookup"><span data-stu-id="48988-223">Fixed missing features in `az iot hub create`</span></span>

### <a name="key-vault"></a><span data-ttu-id="48988-224">Key Vault</span><span class="sxs-lookup"><span data-stu-id="48988-224">Key Vault</span></span>

* <span data-ttu-id="48988-225">Foi corrigido um erro inesperado quando o arquivo de certificado não existe</span><span class="sxs-lookup"><span data-stu-id="48988-225">Fixed an unexpected error when certificate file does not exist</span></span>
* <span data-ttu-id="48988-226">Foi corrigido o problema em que o `az keyvault recover/purge` não funcionava</span><span class="sxs-lookup"><span data-stu-id="48988-226">Fixed `az keyvault recover/purge` not working</span></span>

### <a name="netappfiles"></a><span data-ttu-id="48988-227">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="48988-227">NetAppFiles</span></span>

* <span data-ttu-id="48988-228">O azure-mgmt-netapp foi atualizado para 0.6.0 para usar a versão da API 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="48988-228">Upgraded azure-mgmt-netapp to 0.6.0 to use API version 2019-07-01.</span></span> <span data-ttu-id="48988-229">Essa nova versão da API inclui:</span><span class="sxs-lookup"><span data-stu-id="48988-229">This new API version includes:</span></span>

    - <span data-ttu-id="48988-230">A criação de volume `--protocol-types` agora aceita "NFSv4.1" não "NFSv4"</span><span class="sxs-lookup"><span data-stu-id="48988-230">Volume creation `--protocol-types` accepts now "NFSv4.1" not "NFSv4"</span></span>
    - <span data-ttu-id="48988-231">A propriedade da política de exportação de volume agora é chamada 'nfsv41' não 'nfsv4'</span><span class="sxs-lookup"><span data-stu-id="48988-231">Volume export policy property now named 'nfsv41' not 'nfsv4'</span></span>
    - <span data-ttu-id="48988-232">O volume `--creation-token` foi renomeado para `--file-path`</span><span class="sxs-lookup"><span data-stu-id="48988-232">Volume `--creation-token` renamed to `--file-path`</span></span>
    - <span data-ttu-id="48988-233">A data de criação do instantâneo agora é chamada apenas de 'criação'</span><span class="sxs-lookup"><span data-stu-id="48988-233">Snapshot creation date now named just 'created'</span></span>

### <a name="network"></a><span data-ttu-id="48988-234">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-234">Network</span></span>

* <span data-ttu-id="48988-235">`az network private-dns link vnet create/update`: suporte à vinculação de rede virtual entre locatários.</span><span class="sxs-lookup"><span data-stu-id="48988-235">`az network private-dns link vnet create/update`: Support cross-tenant virtual network linking.</span></span>
* <span data-ttu-id="48988-236">[ALTERAÇÃO DA FALHA] `az network vnet subnet list`: `--resource-group` e `--vnet-name` foram alterados para serem obrigatórios agora.</span><span class="sxs-lookup"><span data-stu-id="48988-236">[BREAKING CHANGE] `az network vnet subnet list`: Changed `--resource-group` and `--vnet-name` to be required now.</span></span>
* <span data-ttu-id="48988-237">`az network public-ip prefix create`: Suporte adicionado para especificar a versão do endereço IP (IPv4, IPv6) durante a criação</span><span class="sxs-lookup"><span data-stu-id="48988-237">`az network public-ip prefix create`: Added support to specify IP address version (IPv4, IPv6) when creation</span></span>
* <span data-ttu-id="48988-238">O azure-mgmt-network foi atualizado para 7.0.0 e a api-version para 2019-09-01</span><span class="sxs-lookup"><span data-stu-id="48988-238">Bumped azure-mgmt-network to 7.0.0 and api-version to 2019-09-01</span></span>
* <span data-ttu-id="48988-239">`az network vrouter`: Suporte adicionado para o novo roteador virtual de serviço e o emparelhamento do roteador virtual</span><span class="sxs-lookup"><span data-stu-id="48988-239">`az network vrouter`: Added support for new service virtual router and virtual router peering</span></span>
* <span data-ttu-id="48988-240">`az network express-route gateway connection`: Adicionado o suporte para `--internet-security`</span><span class="sxs-lookup"><span data-stu-id="48988-240">`az network express-route gateway connection`: Added support for `--internet-security`</span></span>

### <a name="profile"></a><span data-ttu-id="48988-241">Perfil</span><span class="sxs-lookup"><span data-stu-id="48988-241">Profile</span></span>

* <span data-ttu-id="48988-242">Foi corrigido o problema em que o `az account get-access-token --resource-type ms-graph` não funcionava</span><span class="sxs-lookup"><span data-stu-id="48988-242">Fixed `az account get-access-token --resource-type ms-graph` not working</span></span>
* <span data-ttu-id="48988-243">O aviso foi removido de `az login`</span><span class="sxs-lookup"><span data-stu-id="48988-243">Removed warning from `az login`</span></span>

### <a name="rbac"></a><span data-ttu-id="48988-244">RBAC</span><span class="sxs-lookup"><span data-stu-id="48988-244">RBAC</span></span>

* <span data-ttu-id="48988-245">Foi corrigido o problema em que o `az ad app update --id {} --display-name {}` não funcionava</span><span class="sxs-lookup"><span data-stu-id="48988-245">Fixed `az ad app update --id {} --display-name {}` doesn't work</span></span>

### <a name="servicefabric"></a><span data-ttu-id="48988-246">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="48988-246">ServiceFabric</span></span>

* <span data-ttu-id="48988-247">`az sf cluster create`: foi corrigido um problema que ocorria ao modificar o VMSS de computação do template.json do Linux e do Windows, do Service Fabric, de discos Standard para discos gerenciados</span><span class="sxs-lookup"><span data-stu-id="48988-247">`az sf cluster create`: Fixed an issue by modifying service fabric linux and windows template.json compute vmss from standard to managed disks</span></span>

### <a name="sql"></a><span data-ttu-id="48988-248">SQL</span><span class="sxs-lookup"><span data-stu-id="48988-248">SQL</span></span>

* <span data-ttu-id="48988-249">Os parâmetros `--compute-model`, `--auto-pause-delay` e `--min-capacity` foram adicionados para dar suporte a operações CRUD para a nova oferta de Banco de Dados SQL: Modelo de computação sem servidor.</span><span class="sxs-lookup"><span data-stu-id="48988-249">Added `--compute-model`, `--auto-pause-delay`, and `--min-capacity` parameters to support CRUD operations for new SQL Database offering: Serverless compute model.</span></span>

### <a name="storage"></a><span data-ttu-id="48988-250">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48988-250">Storage</span></span>

* <span data-ttu-id="48988-251">`az storage account create/update`: Foram adicionados o parâmetro --enable-files-adds e o grupo Argumentos de Propriedades do Azure Active Directory para dar suporte à Autenticação do Serviço de Domínio do Active Directory do Arquivos do Azure</span><span class="sxs-lookup"><span data-stu-id="48988-251">`az storage account create/update`: Added --enable-files-adds parameter and Azure Active Directory Properties Argument group to support Azure Files Active Directory Domain Service Authentication</span></span>
* <span data-ttu-id="48988-252">O `az storage account keys list/renew` foi expandido para dar suporte à listagem ou à regeneração de chaves Kerberos da conta de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="48988-252">Expanded `az storage account keys list/renew` to support listing or regenerating Kerberos keys of storage account.</span></span>

## <a name="october-15-2019"></a><span data-ttu-id="48988-253">15 de outubro de 2019</span><span class="sxs-lookup"><span data-stu-id="48988-253">October 15, 2019</span></span>

<span data-ttu-id="48988-254">Versão 2.0.75</span><span class="sxs-lookup"><span data-stu-id="48988-254">Version 2.0.75</span></span>

### <a name="aks"></a><span data-ttu-id="48988-255">AKS</span><span class="sxs-lookup"><span data-stu-id="48988-255">AKS</span></span>

* <span data-ttu-id="48988-256">Alteração do valor padrão `--load-balancer-sku` para `standard` se for compatível com a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="48988-256">Changed `--load-balancer-sku` default value to `standard` if supported by the kubernetes version</span></span>
* <span data-ttu-id="48988-257">Alteração do valor padrão `--vm-set-type` para `virtualmachinescalesets` se for compatível com a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="48988-257">Changed `--vm-set-type` default value to `virtualmachinescalesets` if supported by the kubernetes version</span></span>

### <a name="ams"></a><span data-ttu-id="48988-258">AMS</span><span class="sxs-lookup"><span data-stu-id="48988-258">AMS</span></span>

* <span data-ttu-id="48988-259">[ALTERAÇÃO SIGNIFICATIVA] Alteração do nome de `job start` para `job create`</span><span class="sxs-lookup"><span data-stu-id="48988-259">[BREAKING CHANGE] Changed the name of `job start` to `job create`</span></span>
* <span data-ttu-id="48988-260">[ALTERAÇÃO SIGNIFICATIVA] Alteração do parâmetro `--ask` de `content-key-policy create` para usar uma cadeia de 32 caracteres hexadecimais em vez do UTF8</span><span class="sxs-lookup"><span data-stu-id="48988-260">[BREAKING CHANGE] Changed the `--ask` parameter of `content-key-policy create` to use a 32-character hex string instead of UTF8</span></span>

### <a name="appservice"></a><span data-ttu-id="48988-261">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-261">AppService</span></span>

* <span data-ttu-id="48988-262">Adição dos comandos `webapp config access-restriction show|set|add|remove`</span><span class="sxs-lookup"><span data-stu-id="48988-262">Added commands `webapp config access-restriction show|set|add|remove`</span></span>
* <span data-ttu-id="48988-263">Adição de um melhor tratamento de erro a `webapp up`</span><span class="sxs-lookup"><span data-stu-id="48988-263">Added better error handling to `webapp up`</span></span>
* <span data-ttu-id="48988-264">Adição de suporte do SKU `Isolated` para `appservice plan update`</span><span class="sxs-lookup"><span data-stu-id="48988-264">Added support for `Isolated` SKU to `appservice plan update`</span></span>

### <a name="arm"></a><span data-ttu-id="48988-265">ARM</span><span class="sxs-lookup"><span data-stu-id="48988-265">ARM</span></span>

* <span data-ttu-id="48988-266">Adição do parâmetro `--handle-extended-json-format` `deployment create` para dar suporte a várias linhas e a comentários no modelo json</span><span class="sxs-lookup"><span data-stu-id="48988-266">Added `--handle-extended-json-format` parameter `deployment create` to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="48988-267">Computação</span><span class="sxs-lookup"><span data-stu-id="48988-267">Compute</span></span>

* <span data-ttu-id="48988-268">Parâmetro `--enable-agent` adicionado a `vm create`</span><span class="sxs-lookup"><span data-stu-id="48988-268">Added `--enable-agent` parameter to `vm create`</span></span>
* <span data-ttu-id="48988-269">Alteração de `vm create` para usar um SKU de IP público padrão automaticamente ao usar zonas</span><span class="sxs-lookup"><span data-stu-id="48988-269">Changed `vm create` to use standard public IP SKU automatically when using zones</span></span>
* <span data-ttu-id="48988-270">Alteração de `vm create` para criar automaticamente um nome de computador válido para uma VM, caso nenhum tenha sido fornecido</span><span class="sxs-lookup"><span data-stu-id="48988-270">Changed `vm create` to automatically create a valid computer name for a VM if none is provided</span></span>
* <span data-ttu-id="48988-271">Adição do parâmetro `--computer-name-prefix` a `vmss create` para dar suporte ao prefixo de nome de computador personalizado de máquinas virtuais no VMSS</span><span class="sxs-lookup"><span data-stu-id="48988-271">Added `--computer-name-prefix` parameter to `vmss create` to support custom computer name prefix of virtual machines in the VMSS</span></span>
* <span data-ttu-id="48988-272">Adicione o parâmetro `--workspace` a `vm create` para habilitar o workspace de análise de logs automaticamente</span><span class="sxs-lookup"><span data-stu-id="48988-272">Add `--workspace` parameter to `vm create` to enable log analytics workspace automatically</span></span>
* <span data-ttu-id="48988-273">Versão de API de galerias atualizadas para 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="48988-273">Updated galleries API version to 2019-07-01</span></span>

### <a name="core"></a><span data-ttu-id="48988-274">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48988-274">Core</span></span>

* <span data-ttu-id="48988-275">Adição da verificação de sintaxe para o parâmetro `--set` no comando de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="48988-275">Added syntax check for `--set` parameter in generic update command</span></span>

### <a name="iot"></a><span data-ttu-id="48988-276">IoT</span><span class="sxs-lookup"><span data-stu-id="48988-276">IoT</span></span>

* <span data-ttu-id="48988-277">Correção de um problema em que o `iot hub show` retornaria incorretamente um erro com "recurso não encontrado"</span><span class="sxs-lookup"><span data-stu-id="48988-277">Fixed an issue where `iot hub show` would incorrectly error with "resource not found"</span></span>

### <a name="monitor"></a><span data-ttu-id="48988-278">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="48988-278">Monitor</span></span>

* <span data-ttu-id="48988-279">Adição de suporte para CRUD a `monitor log-analytics workspace`</span><span class="sxs-lookup"><span data-stu-id="48988-279">Added support for CRUD to `monitor log-analytics workspace`</span></span>

### <a name="network"></a><span data-ttu-id="48988-280">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-280">Network</span></span>

* <span data-ttu-id="48988-281">Adição de suporte para vinculação virtual entre locatários para `network private-dns link vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48988-281">Added support for cross-tenant virtual linking to `network private-dns link vnet [create|update]`</span></span>
* <span data-ttu-id="48988-282">[ALTERAÇÃO SIGNIFICATIVA] Alteração de `network vnet subnet list` para exigir os parâmetros `--resource-group` e `--vnet-name`</span><span class="sxs-lookup"><span data-stu-id="48988-282">[BREAKING CHANGE] Changed `network vnet subnet list` to require `--resource-group` and `--vnet-name` parameters</span></span>

### <a name="sql"></a><span data-ttu-id="48988-283">SQL</span><span class="sxs-lookup"><span data-stu-id="48988-283">SQL</span></span>

* <span data-ttu-id="48988-284">Adição de comandos a `sql mi ad-admin` que dão suporte à configuração de um administrador do AAD em instâncias gerenciadas</span><span class="sxs-lookup"><span data-stu-id="48988-284">Added commands to `sql mi ad-admin` that support setting an AAD administrator on managed instances</span></span>

### <a name="storage"></a><span data-ttu-id="48988-285">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48988-285">Storage</span></span>

* <span data-ttu-id="48988-286">Adição do parâmetro `--preserve-s2s-access-tier` `storage copy` para preservar a camada de acesso durante a cópia do serviço para serviço</span><span class="sxs-lookup"><span data-stu-id="48988-286">Added `--preserve-s2s-access-tier` parameter `storage copy` to preserve access tier during service to service copy</span></span>
* <span data-ttu-id="48988-287">Adição do parâmetro `--enable-large-file-share` a `storage account [create|update]` para dar suporte a compartilhamentos de arquivos grandes para a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="48988-287">Added `--enable-large-file-share` parameter to `storage account [create|update]` to support large file shares for storage account</span></span>

## <a name="september-24-2019"></a><span data-ttu-id="48988-288">24 de setembro de 2019</span><span class="sxs-lookup"><span data-stu-id="48988-288">September 24, 2019</span></span>

<span data-ttu-id="48988-289">Versão 2.0.74</span><span class="sxs-lookup"><span data-stu-id="48988-289">Version 2.0.74</span></span>

### <a name="acr"></a><span data-ttu-id="48988-290">ACR</span><span class="sxs-lookup"><span data-stu-id="48988-290">ACR</span></span>

* <span data-ttu-id="48988-291">Inclusão de um parâmetro `--type` obrigatório em `acr config retention update`</span><span class="sxs-lookup"><span data-stu-id="48988-291">Added a required `--type` parameter to `acr config retention update`</span></span>
* <span data-ttu-id="48988-292">[ALTERAÇÃO DE FALHA] O parâmetro renomeado `--name -n` foi alterado para `--registry -r ` para o grupo de comando `acr config`</span><span class="sxs-lookup"><span data-stu-id="48988-292">[BREAKING CHNAGE] Renamed parameter `--name -n` changed to `--registry -r ` for `acr config` command group</span></span>

### <a name="aks"></a><span data-ttu-id="48988-293">AKS</span><span class="sxs-lookup"><span data-stu-id="48988-293">AKS</span></span>

* <span data-ttu-id="48988-294">Inclusão do parâmetro `--load-balancer-sku` no comando `aks create`, o que permite criar um cluster do AKS com SLB</span><span class="sxs-lookup"><span data-stu-id="48988-294">Added `--load-balancer-sku` parameter to `aks create` command, which allows for creating AKS cluster with SLB</span></span>
* <span data-ttu-id="48988-295">Inclusão dos parâmetros `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` e `--load-balancer-outbound-ip-prefixes` nos comandos `aks [create|update]`, o que permite atualizar o perfil do balanceador de carga de um cluster do AKS com SLB</span><span class="sxs-lookup"><span data-stu-id="48988-295">Added `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` and `--load-balancer-outbound-ip-prefixes` parameters to `aks [create|update]` commands, which allow for updating load balancer profile of an AKS cluster with SLB</span></span>
* <span data-ttu-id="48988-296">Inclusão do parâmetro `--vm-set-type` no comando `aks create`, o que permite especificar os tipos de VM de um cluster do AKS (vmas ou vmss)</span><span class="sxs-lookup"><span data-stu-id="48988-296">Added `--vm-set-type` parameter to `aks create` command, which allows to specify vm types of an AKS Cluster (vmas or vmss)</span></span>

### <a name="arm"></a><span data-ttu-id="48988-297">ARM</span><span class="sxs-lookup"><span data-stu-id="48988-297">ARM</span></span>

* <span data-ttu-id="48988-298">Inclusão do parâmetro `--handle-extended-json-format` no comando `group deployment create` para compatibilidade com várias linhas e comentários no modelo JSON</span><span class="sxs-lookup"><span data-stu-id="48988-298">Added `--handle-extended-json-format` parameter to `group deployment create` command to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="48988-299">Computação</span><span class="sxs-lookup"><span data-stu-id="48988-299">Compute</span></span>

* <span data-ttu-id="48988-300">Inclusão do parâmetro `--terminate-notification-time` nos comandos `vmss [create|update]` para compatibilidade com a capacidade de configurar o encerramento de eventos agendados</span><span class="sxs-lookup"><span data-stu-id="48988-300">Added `--terminate-notification-time` parameter to `vmss [create|update]` commands to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="48988-301">Inclusão do parâmetro `--enable-terminate-notification` no comando `vmss update` para compatibilidade com a capacidade de configurar o encerramento de eventos agendados</span><span class="sxs-lookup"><span data-stu-id="48988-301">Added `--enable-terminate-notification` parameter to `vmss update` command to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="48988-302">Inclusão dos parâmetros `--priority,`, `--eviction-policy,` e `--max-billing` nos comandos `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="48988-302">Added `--priority,` `--eviction-policy,` `--max-billing` parameters to `[vm|vmss] create` commands</span></span>
* <span data-ttu-id="48988-303">Alteração de `disk create` para permitir a especificação do tamanho exato do carregamento de disco</span><span class="sxs-lookup"><span data-stu-id="48988-303">Changed `disk create` to allow specifying the exact size of the disk upload</span></span>
* <span data-ttu-id="48988-304">Inclusão de compatibilidade com instantâneos incrementais para discos gerenciados para `snapshot create`</span><span class="sxs-lookup"><span data-stu-id="48988-304">Added support for incremental snapshots for managed disks to `snapshot create`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="48988-305">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="48988-305">Cosmos DB</span></span>

* <span data-ttu-id="48988-306">Inclusão do parâmetro `--type <key-type>` no comando `cosmosdb keys list` para mostrar a chave, as chaves somente leitura ou cadeias de conexão</span><span class="sxs-lookup"><span data-stu-id="48988-306">Added `--type <key-type>` parameter to `cosmosdb keys list` command to show key, read only keys or connection strings</span></span>
* <span data-ttu-id="48988-307">Adicionado o comando `cosmosdb keys regenerate`</span><span class="sxs-lookup"><span data-stu-id="48988-307">Added `cosmosdb keys regenerate` command</span></span>
* <span data-ttu-id="48988-308">[PRETERIDO] Comandos `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` e `cosmosdb list-read-only-keys` preteridos</span><span class="sxs-lookup"><span data-stu-id="48988-308">[DEPRECATED] Deprecated `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` and `cosmosdb list-read-only-keys` commands</span></span>

### <a name="eventgrid"></a><span data-ttu-id="48988-309">EventGrid</span><span class="sxs-lookup"><span data-stu-id="48988-309">EventGrid</span></span>

* <span data-ttu-id="48988-310">Correção do texto de ajuda do ponto de extremidade para fazer referência ao parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="48988-310">Fixed the endpoint help text to refer to the right parameter</span></span>

### <a name="key-vault"></a><span data-ttu-id="48988-311">Key Vault</span><span class="sxs-lookup"><span data-stu-id="48988-311">Key Vault</span></span>

* <span data-ttu-id="48988-312">Correção do problema em que fazer logon com um locatário (`login -t`) poderia causar uma falha no `keyvault create`</span><span class="sxs-lookup"><span data-stu-id="48988-312">Fixed issue where logging in with a tenant (`login -t`) could cause `keyvault create` to fail</span></span>

### <a name="monitor"></a><span data-ttu-id="48988-313">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="48988-313">Monitor</span></span>

* <span data-ttu-id="48988-314">Correção do problema em que o caractere `:` não era permitido no argumento `--condition` para `monitor metrics alert create`</span><span class="sxs-lookup"><span data-stu-id="48988-314">Fixed issue where `:` character was not allowed in `--condition` argument to `monitor metrics alert create`</span></span>

### <a name="policy"></a><span data-ttu-id="48988-315">Política</span><span class="sxs-lookup"><span data-stu-id="48988-315">Policy</span></span>

* <span data-ttu-id="48988-316">Inclusão de compatibilidade com a API de Política, versão de 01/06/2019</span><span class="sxs-lookup"><span data-stu-id="48988-316">Added support for Policy API version 2019-06-01</span></span>
* <span data-ttu-id="48988-317">Inclusão do parâmetro `--enforcement-mode` no comando `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="48988-317">Added `--enforcement-mode` parameter to `policy assignment create` command</span></span>

### <a name="storage"></a><span data-ttu-id="48988-318">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48988-318">Storage</span></span>

* <span data-ttu-id="48988-319">Inclusão do parâmetro `--blob-type` no comando `az storage copy`</span><span class="sxs-lookup"><span data-stu-id="48988-319">Added `--blob-type` parameter to `az storage copy` command</span></span>

## <a name="september-10-2019"></a><span data-ttu-id="48988-320">10 de setembro de 2019</span><span class="sxs-lookup"><span data-stu-id="48988-320">September 10, 2019</span></span>

### <a name="acr"></a><span data-ttu-id="48988-321">ACR</span><span class="sxs-lookup"><span data-stu-id="48988-321">ACR</span></span>

* <span data-ttu-id="48988-322">Adição do grupo de comandos `acr config retention` para configurar a política de retenção</span><span class="sxs-lookup"><span data-stu-id="48988-322">Added command group `acr config retention` to configure retention policy</span></span>

### <a name="aks"></a><span data-ttu-id="48988-323">AKS</span><span class="sxs-lookup"><span data-stu-id="48988-323">AKS</span></span>

* <span data-ttu-id="48988-324">Adição de suporte para integração do ACR com os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="48988-324">Added support for ACR integration with the following commands:</span></span>
  * <span data-ttu-id="48988-325">Adição do parâmetro `--attach-acr` a `aks [create|update]` para anexar um ACR a um cluster do AKS</span><span class="sxs-lookup"><span data-stu-id="48988-325">Added `--attach-acr` parameter to `aks [create|update]` to attach an ACR to an AKS cluster</span></span>
  * <span data-ttu-id="48988-326">Adição do parâmetro `--detach-acr` a `aks update` para desanexar o ACR de um cluster do AKS</span><span class="sxs-lookup"><span data-stu-id="48988-326">Added `--detach-acr` parameter to `aks update` to detach the ACR from an AKS cluster</span></span>

### <a name="arm"></a><span data-ttu-id="48988-327">ARM</span><span class="sxs-lookup"><span data-stu-id="48988-327">ARM</span></span>

* <span data-ttu-id="48988-328">Atualização para uso da versão de API 2019-05-10</span><span class="sxs-lookup"><span data-stu-id="48988-328">Updated to use API version 2019-05-10</span></span>

### <a name="batch"></a><span data-ttu-id="48988-329">Lote</span><span class="sxs-lookup"><span data-stu-id="48988-329">Batch</span></span>

* <span data-ttu-id="48988-330">Adição de novas definições de configuração JSON de `--json-file` para `batch pool create`:</span><span class="sxs-lookup"><span data-stu-id="48988-330">Added new JSON configuration settings to `--json-file` for `batch pool create`:</span></span>
  * <span data-ttu-id="48988-331">Adição de `MountConfigurations` para montagens do sistema de arquivos (confira https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body para obter detalhes)</span><span class="sxs-lookup"><span data-stu-id="48988-331">Added `MountConfigurations` for file system mounts (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
  * <span data-ttu-id="48988-332">Adição da propriedade opcional `publicIPs` a `NetworkConfiguration` para IPs públicos em pools (confira https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body para obter detalhes)</span><span class="sxs-lookup"><span data-stu-id="48988-332">Added optional property `publicIPs` on `NetworkConfiguration` for public IPs on pools (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
* <span data-ttu-id="48988-333">Adição de suporte para galerias de imagens compartilhadas a `--image`</span><span class="sxs-lookup"><span data-stu-id="48988-333">Added support for shared image galleries to `--image`</span></span>
* <span data-ttu-id="48988-334">[ALTERAÇÃO SIGNIFICATIVA] Alteração do valor padrão de `--start-task-wait-for-success` em `batch pool create` para `true`</span><span class="sxs-lookup"><span data-stu-id="48988-334">[BREAKING CHANGE] Changed default value of `--start-task-wait-for-success` on `batch pool create` to be `true`</span></span>
* <span data-ttu-id="48988-335">[ALTERAÇÃO SIGNIFICATIVA] Alteração do valor padrão de `Scope` em `AutoUserSpecification` para sempre ser Pool (anteriormente, `Task` em nós do Windows e `Pool` em nós do Linux)</span><span class="sxs-lookup"><span data-stu-id="48988-335">[BREAKING CHANGE] Changed default value for `Scope` on `AutoUserSpecification` to always be Pool (was `Task` on Windows nodes, `Pool` on Linux nodes)</span></span>
  * <span data-ttu-id="48988-336">Esse argumento só pode ser definido em uma configuração JSON com `--json-file`</span><span class="sxs-lookup"><span data-stu-id="48988-336">This argument can only be set from a JSON configuration with `--json-file`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="48988-337">HDInsight</span><span class="sxs-lookup"><span data-stu-id="48988-337">HDInsight</span></span>

* <span data-ttu-id="48988-338">Versão de GA</span><span class="sxs-lookup"><span data-stu-id="48988-338">GA release</span></span>
* <span data-ttu-id="48988-339">[ALTERAÇÃO SIGNIFICATIVA] Alteração do parâmetro `--workernode-count/-c` de `az hdinsight resize` para ser obrigatório.</span><span class="sxs-lookup"><span data-stu-id="48988-339">[BREAKING CHANGE] Changed parameter `--workernode-count/-c` of `az hdinsight resize` to be required.</span></span>

### <a name="key-vault"></a><span data-ttu-id="48988-340">Key Vault</span><span class="sxs-lookup"><span data-stu-id="48988-340">Key Vault</span></span>

* <span data-ttu-id="48988-341">Correção do problema em que as sub-redes não podiam ser excluídas das regras da rede</span><span class="sxs-lookup"><span data-stu-id="48988-341">Fixed issue where subnets couldn't be deleted from network rules</span></span>
* <span data-ttu-id="48988-342">Correção do problema em que sub-redes e endereços IP duplicados podiam ser adicionados às regras da rede</span><span class="sxs-lookup"><span data-stu-id="48988-342">Fixed issue where duplicated subnets and IP addresses could be added to network rules</span></span>

### <a name="network"></a><span data-ttu-id="48988-343">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-343">Network</span></span>

* <span data-ttu-id="48988-344">Adição do parâmetro `--interval` a `network watcher flow-log` para definir o valor do intervalo de análise de tráfego</span><span class="sxs-lookup"><span data-stu-id="48988-344">Added `--interval` parameter to `network watcher flow-log` to set traffic analysis interval value</span></span>
* <span data-ttu-id="48988-345">Adição de `network application-gateway identity` para gerenciar a identidade do gateway</span><span class="sxs-lookup"><span data-stu-id="48988-345">Added `network application-gateway identity` to manage gateway identity</span></span>
* <span data-ttu-id="48988-346">Adição de suporte para definir a ID do Key Vault como `network application-gateway ssl-cert`</span><span class="sxs-lookup"><span data-stu-id="48988-346">Added support for setting Key Vault ID to `network application-gateway ssl-cert`</span></span>
* <span data-ttu-id="48988-347">Adicionado `network express-route peering peer-connection [show|list]`</span><span class="sxs-lookup"><span data-stu-id="48988-347">Added `network express-route peering peer-connection [show|list]`</span></span>

### <a name="policy"></a><span data-ttu-id="48988-348">Política</span><span class="sxs-lookup"><span data-stu-id="48988-348">Policy</span></span>

* <span data-ttu-id="48988-349">Atualização para uso da versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="48988-349">Updated to use API version 2019-01-01</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="48988-350">27 de agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="48988-350">August 27, 2019</span></span>

<span data-ttu-id="48988-351">Versão 2.0.72</span><span class="sxs-lookup"><span data-stu-id="48988-351">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="48988-352">ACR</span><span class="sxs-lookup"><span data-stu-id="48988-352">ACR</span></span>

* <span data-ttu-id="48988-353">[ALTERAÇÃO SIGNIFICATIVA] Remoção da compatibilidade com o SKU `classic`</span><span class="sxs-lookup"><span data-stu-id="48988-353">[BREAKING CHANGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="48988-354">Gerenciamento de API</span><span class="sxs-lookup"><span data-stu-id="48988-354">API Management</span></span>

* <span data-ttu-id="48988-355">[VERSÃO PRÉVIA] Adição do grupo de comandos `apim`</span><span class="sxs-lookup"><span data-stu-id="48988-355">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="48988-356">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-356">AppService</span></span>

* <span data-ttu-id="48988-357">Correção do problema com o comando `webapp webjob continuous start` ao especificar um slot</span><span class="sxs-lookup"><span data-stu-id="48988-357">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="48988-358">Alteração de `webapp up` para detectar a pasta `env` e removê-la do arquivo usado para implantação</span><span class="sxs-lookup"><span data-stu-id="48988-358">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="48988-359">Keyvault</span><span class="sxs-lookup"><span data-stu-id="48988-359">Keyvault</span></span>

* <span data-ttu-id="48988-360">Correção de um bug no `keyvault secret set` que ignorava o argumento `--expires`</span><span class="sxs-lookup"><span data-stu-id="48988-360">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="48988-361">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-361">Network</span></span>

* <span data-ttu-id="48988-362">Adição de suporte para endereços IPv6 a argumentos `--private-ip-address-version`</span><span class="sxs-lookup"><span data-stu-id="48988-362">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="48988-363">Adição de novos comandos `network private-endpoint [create|update|list-types]` para o gerenciamento de ponto de extremidade privado</span><span class="sxs-lookup"><span data-stu-id="48988-363">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="48988-364">Adição do grupo de comandos `network private-link-service`</span><span class="sxs-lookup"><span data-stu-id="48988-364">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="48988-365">Adicionados os argumentos `--private-endpoint-network-policies` e `--private-link-service-network-policies` para `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="48988-365">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="48988-366">RBAC</span><span class="sxs-lookup"><span data-stu-id="48988-366">RBAC</span></span>

* <span data-ttu-id="48988-367">Correção de um problema com `ad app update --homepage` em que a página inicial não era atualizada</span><span class="sxs-lookup"><span data-stu-id="48988-367">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="48988-368">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="48988-368">ServiceFabric</span></span>

* <span data-ttu-id="48988-369">Adição de suporte para nomes de Key Vault grafados com maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="48988-369">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="48988-370">Correção de um problema ao usar certificados no Key Vault</span><span class="sxs-lookup"><span data-stu-id="48988-370">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="48988-371">Correção de um problema com o uso de arquivos de certificado PFX</span><span class="sxs-lookup"><span data-stu-id="48988-371">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="48988-372">Correção de um problema com `sf cluster certificate add` quando o grupo de recursos do Key Vault não era especificado</span><span class="sxs-lookup"><span data-stu-id="48988-372">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="48988-373">Correção de um problema em que `sf cluster set` não funcionava</span><span class="sxs-lookup"><span data-stu-id="48988-373">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="48988-374">SignalR</span><span class="sxs-lookup"><span data-stu-id="48988-374">SignalR</span></span>

* <span data-ttu-id="48988-375">Novos comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="48988-375">Added new commands:</span></span>
  * <span data-ttu-id="48988-376">`signalr cors`: gerenciar CORS do SignalR</span><span class="sxs-lookup"><span data-stu-id="48988-376">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="48988-377">`signalr restart`: reiniciar um serviço do SignalR</span><span class="sxs-lookup"><span data-stu-id="48988-377">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="48988-378">`signalr update`: atualizar um serviço do SignalR</span><span class="sxs-lookup"><span data-stu-id="48988-378">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="48988-379">Adicionado o argumento `--service-mode` para `signalr create`</span><span class="sxs-lookup"><span data-stu-id="48988-379">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="48988-380">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48988-380">Storage</span></span>

* <span data-ttu-id="48988-381">Adicionado o comando `storage account revoke-delegation-keys`</span><span class="sxs-lookup"><span data-stu-id="48988-381">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="48988-382">13 de agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="48988-382">August 13, 2019</span></span>

<span data-ttu-id="48988-383">Versão 2.0.71</span><span class="sxs-lookup"><span data-stu-id="48988-383">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="48988-384">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-384">AppService</span></span>

* <span data-ttu-id="48988-385">Um problema de falha de slots com os comandos `webapp webjob continuous` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="48988-385">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="48988-386">BotService</span><span class="sxs-lookup"><span data-stu-id="48988-386">BotService</span></span>

* <span data-ttu-id="48988-387">[ALTERAÇÃO SIGNIFICATIVA] O suporte para a criação de bots SDK v3 foi removido</span><span class="sxs-lookup"><span data-stu-id="48988-387">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="48988-388">CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="48988-388">CognitiveServices</span></span>

* <span data-ttu-id="48988-389">Adicionados os comandos `cognitiveservices account network-rule`</span><span class="sxs-lookup"><span data-stu-id="48988-389">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="48988-390">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="48988-390">Cosmos DB</span></span>

* <span data-ttu-id="48988-391">Removido o aviso ao atualizar vários locais de gravação</span><span class="sxs-lookup"><span data-stu-id="48988-391">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="48988-392">Foram adicionados os comandos CRUD para o CosmosDB SQL, MongoDB, Cassandra, Gremlin e Recursos de tabela e taxa de transferência do recurso</span><span class="sxs-lookup"><span data-stu-id="48988-392">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="48988-393">HDInsight</span><span class="sxs-lookup"><span data-stu-id="48988-393">HDInsight</span></span>

<span data-ttu-id="48988-394">Esta versão contém um grande número de alterações da falha.</span><span class="sxs-lookup"><span data-stu-id="48988-394">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="48988-395">[ALTERAÇÃO SIGNIFICATIVA] Parâmetros renomeados para `hdinsight create`:</span><span class="sxs-lookup"><span data-stu-id="48988-395">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="48988-396">`--storage-default-container` renomeado para `--storage-container`</span><span class="sxs-lookup"><span data-stu-id="48988-396">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="48988-397">`--storage-default-filesystem` renomeado para `--storage-filesystem`</span><span class="sxs-lookup"><span data-stu-id="48988-397">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="48988-398">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--name` de `application create` foi alterado para representar o nome do aplicativo em vez do nome do cluster</span><span class="sxs-lookup"><span data-stu-id="48988-398">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="48988-399">O argumento `--cluster-name` foi adicionado a `application create` para substituir a funcionalidade `--name` antiga</span><span class="sxs-lookup"><span data-stu-id="48988-399">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="48988-400">[ALTERAÇÃO SIGNIFICATIVA] Parâmetros renomeados para `application create`:</span><span class="sxs-lookup"><span data-stu-id="48988-400">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="48988-401">`--application-type` renomeado para `--type`</span><span class="sxs-lookup"><span data-stu-id="48988-401">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="48988-402">`--marketplace-identifier` renomeado para `--marketplace-id`</span><span class="sxs-lookup"><span data-stu-id="48988-402">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="48988-403">`--https-endpoint-access-mode` renomeado para `--access-mode`</span><span class="sxs-lookup"><span data-stu-id="48988-403">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="48988-404">Renomeado de `--https-endpoint-destination-port` para `--destination-port`</span><span class="sxs-lookup"><span data-stu-id="48988-404">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="48988-405">[ALTERAÇÃO SIGNIFICATIVA] Parâmetros removidos para `application create`:</span><span class="sxs-lookup"><span data-stu-id="48988-405">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="48988-406">[ALTERAÇÃO DA FALHA] Renomeado de `--target-instance-count` para `--workernode-count` para `hdinsight resize`</span><span class="sxs-lookup"><span data-stu-id="48988-406">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="48988-407">[ALTERAÇÃO SIGNIFICATIVA] Todos os comandos no grupo `hdinsight script-action` foram alterados para usar o parâmetro `--name` como o nome da ação de script.</span><span class="sxs-lookup"><span data-stu-id="48988-407">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="48988-408">O argumento `--cluster-name` foi adicionado a todos os comandos `hdinsight script-action` para substituir a funcionalidade `--name` antiga</span><span class="sxs-lookup"><span data-stu-id="48988-408">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="48988-409">[ALTERAÇÃO SIGNIFICATIVA] Renomeado de `--script-execution-id` para `--execution-id` para todos os comandos `hdinsight script-action`</span><span class="sxs-lookup"><span data-stu-id="48988-409">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="48988-410">[ALTERAÇÃO SIGNIFICATIVA] `hdinsight script-action show` renomeado para `hdinsight script-action show-execution-details`</span><span class="sxs-lookup"><span data-stu-id="48988-410">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="48988-411">[ALTERAÇÃO DA FALHA] Os parâmetros foram alterados para `hdinsight script-action execute --roles` para serem separados por espaços em vez de separados por vírgula</span><span class="sxs-lookup"><span data-stu-id="48988-411">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="48988-412">[ALTERAÇÃO SIGNIFICATIVA] O parâmetro `--persisted` de `hdinsight script-action list` foi removido</span><span class="sxs-lookup"><span data-stu-id="48988-412">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="48988-413">O parâmetro `hdinsight create --cluster-configurations` foi alterado para aceitar um caminho para um arquivo JSON local ou uma cadeia de caracteres JSON</span><span class="sxs-lookup"><span data-stu-id="48988-413">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="48988-414">Adicionado o comando `hdinsight script-action list-execution-history`</span><span class="sxs-lookup"><span data-stu-id="48988-414">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="48988-415">Alterado `hdinsight monitor enable --workspace` para aceitar uma ID do workspace ou nome do workspace do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="48988-415">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="48988-416">O argumento `hdinsight monitor enable --primary-key`, que será necessário caso uma ID do workspace seja fornecida como o parâmetro, foi adicionado</span><span class="sxs-lookup"><span data-stu-id="48988-416">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="48988-417">Foram adicionados mais exemplos e atualização das descrições das mensagens de erro</span><span class="sxs-lookup"><span data-stu-id="48988-417">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="48988-418">Interativo</span><span class="sxs-lookup"><span data-stu-id="48988-418">Interactive</span></span>

* <span data-ttu-id="48988-419">Um erro no carregamento foi corrigido</span><span class="sxs-lookup"><span data-stu-id="48988-419">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="48988-420">kubernetes</span><span class="sxs-lookup"><span data-stu-id="48988-420">Kubernetes</span></span>

* <span data-ttu-id="48988-421">Alterado para usar `https` se a porta do contêiner do painel estiver usando `https`</span><span class="sxs-lookup"><span data-stu-id="48988-421">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="48988-422">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-422">Network</span></span>

* <span data-ttu-id="48988-423">O argumento `--yes` foi adicionado a `network dns record-set cname delete`</span><span class="sxs-lookup"><span data-stu-id="48988-423">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="48988-424">Perfil</span><span class="sxs-lookup"><span data-stu-id="48988-424">Profile</span></span>

* <span data-ttu-id="48988-425">O argumento `--resource-type` foi adicionado a `account get-access-token` para obter tokens de acesso de recurso</span><span class="sxs-lookup"><span data-stu-id="48988-425">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="48988-426">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="48988-426">ServiceFabric</span></span>

* <span data-ttu-id="48988-427">Todas as versões de sistema operacional com suporte para criação do cluster sf foram adicionadas</span><span class="sxs-lookup"><span data-stu-id="48988-427">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="48988-428">Foi corrigido o bug de validação do certificado primário</span><span class="sxs-lookup"><span data-stu-id="48988-428">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="48988-429">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48988-429">Storage</span></span>

* <span data-ttu-id="48988-430">Adicionado o comando `storage copy`</span><span class="sxs-lookup"><span data-stu-id="48988-430">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="48988-431">30 de julho de 2019</span><span class="sxs-lookup"><span data-stu-id="48988-431">July 30, 2019</span></span>

<span data-ttu-id="48988-432">Versão 2.0.70</span><span class="sxs-lookup"><span data-stu-id="48988-432">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="48988-433">ACR</span><span class="sxs-lookup"><span data-stu-id="48988-433">ACR</span></span>

* <span data-ttu-id="48988-434">Corrigido o problema #9952 (uma regressão no comando `acr pack build`)</span><span class="sxs-lookup"><span data-stu-id="48988-434">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="48988-435">Removido o nome da imagem do construtor padrão em `acr pack build`</span><span class="sxs-lookup"><span data-stu-id="48988-435">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="48988-436">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-436">Appservice</span></span>

* <span data-ttu-id="48988-437">Alterado `webapp config ssl` para mostrar uma mensagem se um recurso não for encontrado</span><span class="sxs-lookup"><span data-stu-id="48988-437">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="48988-438">Corrigido o problema em que `functionapp create` não aceita o tipo de conta de armazenamento `Standard_RAGRS`</span><span class="sxs-lookup"><span data-stu-id="48988-438">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="48988-439">Corrigido um problema em que `webapp up` falharia se fosse executado usando versões mais antigas do Python</span><span class="sxs-lookup"><span data-stu-id="48988-439">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="48988-440">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-440">Network</span></span>

* <span data-ttu-id="48988-441">Removido parâmetro inválido `--ids` de `network nic ip-config add` (corrige o #9861)</span><span class="sxs-lookup"><span data-stu-id="48988-441">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="48988-442">Corrige o #9604.</span><span class="sxs-lookup"><span data-stu-id="48988-442">Fixes #9604.</span></span> <span data-ttu-id="48988-443">Adicionado o parâmetro `--root-certs` ao `network application-gateway http-settings [create|update]` para dar suporte a certificados raiz confiáveis associados ao usuário.</span><span class="sxs-lookup"><span data-stu-id="48988-443">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="48988-444">Fixado argumento `--subscription` para `network dns record-set ns create` (#9965)</span><span class="sxs-lookup"><span data-stu-id="48988-444">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="48988-445">RBAC</span><span class="sxs-lookup"><span data-stu-id="48988-445">RBAC</span></span>

* <span data-ttu-id="48988-446">Adicionado o comando `user update`</span><span class="sxs-lookup"><span data-stu-id="48988-446">Added `user update` command</span></span>
* <span data-ttu-id="48988-447">[PRETERIDO] Preterido `--upn-or-object-id` de comandos relacionados ao usuário</span><span class="sxs-lookup"><span data-stu-id="48988-447">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="48988-448">Usar argumento de substituição `--id`</span><span class="sxs-lookup"><span data-stu-id="48988-448">Use replacement argument `--id`</span></span>
* <span data-ttu-id="48988-449">Adicionado argumento `--id` para comandos relacionados ao usuário</span><span class="sxs-lookup"><span data-stu-id="48988-449">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="48988-450">SQL</span><span class="sxs-lookup"><span data-stu-id="48988-450">SQL</span></span>

* <span data-ttu-id="48988-451">Adicionados comandos de gerenciamento para chaves de instância gerenciada e protetor de TDE</span><span class="sxs-lookup"><span data-stu-id="48988-451">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="48988-452">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48988-452">Storage</span></span>

* <span data-ttu-id="48988-453">Adicionado o comando `storage remove`</span><span class="sxs-lookup"><span data-stu-id="48988-453">Added `storage remove` command</span></span>
* <span data-ttu-id="48988-454">Corrigido um problema com `storage blob update`</span><span class="sxs-lookup"><span data-stu-id="48988-454">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="48988-455">VM</span><span class="sxs-lookup"><span data-stu-id="48988-455">VM</span></span>

* <span data-ttu-id="48988-456">Alterado `list-skus` para usar versão de API mais recente a fim de externar detalhes de zona</span><span class="sxs-lookup"><span data-stu-id="48988-456">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="48988-457">Alterado o padrão de `--single-placement-group` para `false` para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="48988-457">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="48988-458">Adicionada a capacidade de selecionar SKUs de armazenamento ZRS para `[snapshot|disk] create`</span><span class="sxs-lookup"><span data-stu-id="48988-458">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="48988-459">Adicionado novo grupo de comandos `vm host` para dar suporte a hosts dedicados</span><span class="sxs-lookup"><span data-stu-id="48988-459">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="48988-460">Adicionados parâmetros `--host` e `--host-group` em `vm create` para definir o host dedicado da VM</span><span class="sxs-lookup"><span data-stu-id="48988-460">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="48988-461">16 de julho de 2019</span><span class="sxs-lookup"><span data-stu-id="48988-461">July 16, 2019</span></span>

<span data-ttu-id="48988-462">Versão 2.0.69</span><span class="sxs-lookup"><span data-stu-id="48988-462">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="48988-463">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-463">Appservice</span></span>

* <span data-ttu-id="48988-464">Os comandos `webapp identity` foram alterados para retornar uma mensagem de erro apropriada se o nome do aplicativo ou ResourceGroupName for inválido</span><span class="sxs-lookup"><span data-stu-id="48988-464">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="48988-465">`webapp list` corrigido para retornar o valor correto para numberOfSites se nenhum ResourceGroup foi fornecido</span><span class="sxs-lookup"><span data-stu-id="48988-465">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="48988-466">Corrigidos os efeitos colaterais de `appservice plan create` e `webapp create`</span><span class="sxs-lookup"><span data-stu-id="48988-466">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="48988-467">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48988-467">Core</span></span>

* <span data-ttu-id="48988-468">Corrigido um problema em que `--subscription` aparecia apesar de não ser aplicável</span><span class="sxs-lookup"><span data-stu-id="48988-468">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="48988-469">Lote</span><span class="sxs-lookup"><span data-stu-id="48988-469">Batch</span></span>

* <span data-ttu-id="48988-470">[ALTERAÇÃO SIGNIFICATIVA] `batch pool node-agent-skus list` foi substituído por `batch pool supported-images list`</span><span class="sxs-lookup"><span data-stu-id="48988-470">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="48988-471">Adicionado suporte para regras de segurança bloqueando o acesso de rede a um pool com base na porta de origem do tráfego ao usar a opção `--json-file` de `batch pool create network`</span><span class="sxs-lookup"><span data-stu-id="48988-471">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="48988-472">Suporte adicionado para executar a tarefa no diretório de trabalho de contêiner ou no diretório de trabalho de tarefa em lotes ao usar a opção `--json-file` de `batch task create`</span><span class="sxs-lookup"><span data-stu-id="48988-472">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="48988-473">Corrigido o erro na opção `--application-package-references` de `batch pool create` em que ela funcionaria apenas com padrões</span><span class="sxs-lookup"><span data-stu-id="48988-473">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="48988-474">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="48988-474">Eventhubs</span></span>

* <span data-ttu-id="48988-475">Adicionada validação para o parâmetro `--rights` dos comandos `authorizationrule`</span><span class="sxs-lookup"><span data-stu-id="48988-475">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="48988-476">RDBMS</span><span class="sxs-lookup"><span data-stu-id="48988-476">RDBMS</span></span>

* <span data-ttu-id="48988-477">Adicionado um parâmetro opcional para especificar a réplica de SKU para criar o comando de réplica</span><span class="sxs-lookup"><span data-stu-id="48988-477">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="48988-478">Corrigido o problema com a falha no teste de CI com a criação de réplica de MySQL</span><span class="sxs-lookup"><span data-stu-id="48988-478">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="48988-479">Retransmissão</span><span class="sxs-lookup"><span data-stu-id="48988-479">Relay</span></span>

* <span data-ttu-id="48988-480">Corrigido o problema com a conexão híbrida quando a autorização do cliente desabilitava [#8775](https://github.com/azure/azure-cli/issues/8775)</span><span class="sxs-lookup"><span data-stu-id="48988-480">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="48988-481">Parâmetro `--requires-transport-security` adicionado a `relay wcfrelay create`</span><span class="sxs-lookup"><span data-stu-id="48988-481">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="48988-482">Barramento de serviço</span><span class="sxs-lookup"><span data-stu-id="48988-482">Servicebus</span></span>

* <span data-ttu-id="48988-483">Adicionada validação para o parâmetro `--rights` dos comandos `authorizationrule`</span><span class="sxs-lookup"><span data-stu-id="48988-483">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="48988-484">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48988-484">Storage</span></span>

* <span data-ttu-id="48988-485">Habilitar AADDS de arquivos para atualização da conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="48988-485">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="48988-486">Problema corrigido `storage blob service-properties update --set`</span><span class="sxs-lookup"><span data-stu-id="48988-486">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="48988-487">2 de julho de 2019</span><span class="sxs-lookup"><span data-stu-id="48988-487">July 2, 2019</span></span>

<span data-ttu-id="48988-488">Versão 2.0.68</span><span class="sxs-lookup"><span data-stu-id="48988-488">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="48988-489">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48988-489">Core</span></span>

* <span data-ttu-id="48988-490">Agora, os módulos de comando são consolidados em um único Python distribuível.</span><span class="sxs-lookup"><span data-stu-id="48988-490">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="48988-491">Isso substitui o uso direto de muitos pacotes `azure-cli-` no PyPI.</span><span class="sxs-lookup"><span data-stu-id="48988-491">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="48988-492">Assim, o tamanho da instalação será reduzido e apenas os usuários que tiverem instalado diretamente por meio do `pip` serão afetados.</span><span class="sxs-lookup"><span data-stu-id="48988-492">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="48988-493">ACR</span><span class="sxs-lookup"><span data-stu-id="48988-493">ACR</span></span>

* <span data-ttu-id="48988-494">Foi adicionado o suporte para gatilhos de temporizador para tarefa</span><span class="sxs-lookup"><span data-stu-id="48988-494">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="48988-495">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-495">Appservice</span></span>

* <span data-ttu-id="48988-496">O `functionapp create` foi alterado para habilitar o Application Insights por padrão</span><span class="sxs-lookup"><span data-stu-id="48988-496">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="48988-497">[ALTERAÇÃO SIGNIFICATIVA] Foi removido o comando `functionapp devops-build` preterido.</span><span class="sxs-lookup"><span data-stu-id="48988-497">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="48988-498">Agora, use o novo comando `az functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="48988-498">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="48988-499">Foi adicionado o suporte ao plano de aplicativo de funções Consumo em Linux ao `functionapp deployment config-zip`</span><span class="sxs-lookup"><span data-stu-id="48988-499">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="48988-500">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="48988-500">Cosmos DB</span></span>

* <span data-ttu-id="48988-501">Foi adicionado o suporte para desabilitar a TTL</span><span class="sxs-lookup"><span data-stu-id="48988-501">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="48988-502">DLS</span><span class="sxs-lookup"><span data-stu-id="48988-502">DLS</span></span>

* <span data-ttu-id="48988-503">Versão atualizada do ADLS (0.0.45)</span><span class="sxs-lookup"><span data-stu-id="48988-503">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="48988-504">Comentários</span><span class="sxs-lookup"><span data-stu-id="48988-504">Feedback</span></span>

* <span data-ttu-id="48988-505">Ao relatar um comando de extensão com falha, agora, o `az feedback` tenta abrir o navegador na URL do projeto/repositório da extensão por meio do índice</span><span class="sxs-lookup"><span data-stu-id="48988-505">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="48988-506">HDInsight</span><span class="sxs-lookup"><span data-stu-id="48988-506">HDInsight</span></span>

* <span data-ttu-id="48988-507">[ALTERAÇÃO SIGNIFICATIVA] O nome do grupo de comandos `oms` foi alterado para `monitor`</span><span class="sxs-lookup"><span data-stu-id="48988-507">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="48988-508">[ALTERAÇÃO SIGNIFICATIVA] `--http-password/-p` tornou-se um parâmetro obrigatório</span><span class="sxs-lookup"><span data-stu-id="48988-508">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="48988-509">Foram adicionados preenchedores para o preenchedor dos parâmetros `--cluster-admin-account` e `cluster-users-group-dns`</span><span class="sxs-lookup"><span data-stu-id="48988-509">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="48988-510">O parâmetro `cluster-users-group-dns` foi alterado para ser obrigatório quando `—esp` estiver presente</span><span class="sxs-lookup"><span data-stu-id="48988-510">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="48988-511">Foi adicionado um tempo limite para todos os preenchedores automáticos de argumento existentes</span><span class="sxs-lookup"><span data-stu-id="48988-511">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="48988-512">Foi adicionado um tempo limite para transformar o nome do recurso na ID de recurso</span><span class="sxs-lookup"><span data-stu-id="48988-512">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="48988-513">Os preenchedores automáticos foram alterados para selecionar recursos de qualquer grupo de recursos.</span><span class="sxs-lookup"><span data-stu-id="48988-513">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="48988-514">Pode ser um grupo de recursos diferente daquele especificado com `-g`</span><span class="sxs-lookup"><span data-stu-id="48988-514">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="48988-515">Foi adicionado o suporte para os parâmetros `--sub-domain-suffix` e `--disable_gateway_auth` no comando `hdinsight application create`</span><span class="sxs-lookup"><span data-stu-id="48988-515">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="48988-516">Serviços gerenciados</span><span class="sxs-lookup"><span data-stu-id="48988-516">Managed Services</span></span>

* <span data-ttu-id="48988-517">Introdução ao módulo de comando de serviço gerenciado em versão prévia</span><span class="sxs-lookup"><span data-stu-id="48988-517">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="48988-518">Perfil</span><span class="sxs-lookup"><span data-stu-id="48988-518">Profile</span></span>
* <span data-ttu-id="48988-519">Suprimir o argumento `--subscription` para o comando de logoff</span><span class="sxs-lookup"><span data-stu-id="48988-519">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="48988-520">RBAC</span><span class="sxs-lookup"><span data-stu-id="48988-520">RBAC</span></span>

* <span data-ttu-id="48988-521">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--password` foi removido de `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="48988-521">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="48988-522">Foi adicionado o parâmetro `--assignee-principal-type` ao comando `create` para evitar falhas intermitentes causadas pela latência de replicação do servidor do AAD Graph</span><span class="sxs-lookup"><span data-stu-id="48988-522">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="48988-523">Foi corrigida uma falha em `ad signed-in-user` ao listar objetos de propriedade</span><span class="sxs-lookup"><span data-stu-id="48988-523">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="48988-524">Foi corrigido um problema em que o `ad sp` não localizava o aplicativo certo de uma entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="48988-524">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="48988-525">RDBMS</span><span class="sxs-lookup"><span data-stu-id="48988-525">RDBMS</span></span>

* <span data-ttu-id="48988-526">Foi adicionado o suporte à replicação para o MariaDB</span><span class="sxs-lookup"><span data-stu-id="48988-526">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="48988-527">SQL</span><span class="sxs-lookup"><span data-stu-id="48988-527">SQL</span></span>

* <span data-ttu-id="48988-528">Valores permitidos documentados para `sql db create --sample-name`</span><span class="sxs-lookup"><span data-stu-id="48988-528">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="48988-529">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48988-529">Storage</span></span>

* <span data-ttu-id="48988-530">Foi adicionado o suporte ao token SAS de delegação de usuário com `--as-user` para `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="48988-530">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="48988-531">Foi adicionado o suporte ao token SAS de delegação de usuário com `--as-user` para `storage container generate-sas`</span><span class="sxs-lookup"><span data-stu-id="48988-531">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="48988-532">VM</span><span class="sxs-lookup"><span data-stu-id="48988-532">VM</span></span>

* <span data-ttu-id="48988-533">Foi corrigido o bug em que o `vmss create` retornava uma mensagem de erro quando era executado com `--no-wait`</span><span class="sxs-lookup"><span data-stu-id="48988-533">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="48988-534">Foi removida a validação do lado do cliente de `vmss create --single-placement-group`.</span><span class="sxs-lookup"><span data-stu-id="48988-534">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="48988-535">Não falha quando `--single-placement-group` é definido como `true` e `--instance-count` é maior que 100 ou quando são especificadas zonas de disponibilidade, mas deixa essa validação para o serviço de computação</span><span class="sxs-lookup"><span data-stu-id="48988-535">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="48988-536">Foi corrigido o bug em que o `[vm|vmss] extension image list` falhava quando era usado com `--latest`</span><span class="sxs-lookup"><span data-stu-id="48988-536">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="48988-537">18 de junho de 2019</span><span class="sxs-lookup"><span data-stu-id="48988-537">June 18, 2019</span></span>

<span data-ttu-id="48988-538">Versão 2.0.67</span><span class="sxs-lookup"><span data-stu-id="48988-538">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="48988-539">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48988-539">Core</span></span>

<span data-ttu-id="48988-540">Esta versão apresenta uma nova marca [Versão prévia] para comunicar com mais clareza aos clientes quando um comando, um grupo de comandos ou um argumento está no status de versão prévia.</span><span class="sxs-lookup"><span data-stu-id="48988-540">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="48988-541">Anteriormente, essa informação era transmitida no texto de ajuda ou, implicitamente, pelo número da versão do módulo de comando.</span><span class="sxs-lookup"><span data-stu-id="48988-541">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="48988-542">A CLI removerá os números de versão dos pacotes individuais no futuro.</span><span class="sxs-lookup"><span data-stu-id="48988-542">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="48988-543">Se um comando estiver em versão prévia, todos os seus argumentos também estarão.</span><span class="sxs-lookup"><span data-stu-id="48988-543">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="48988-544">Se um grupo de comandos for rotulado com o status de versão prévia, então todos os seus comandos e argumentos também serão considerados em versão prévia.</span><span class="sxs-lookup"><span data-stu-id="48988-544">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="48988-545">Como resultado dessa alteração, diversos grupos de comandos podem parecer surgir "de repente" com o status de versão prévia com esta liberação.</span><span class="sxs-lookup"><span data-stu-id="48988-545">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="48988-546">O que realmente aconteceu é que a maioria dos pacotes já estava com status de versão prévia, mas estão sendo consideradas GA com esta liberação</span><span class="sxs-lookup"><span data-stu-id="48988-546">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="48988-547">ACR</span><span class="sxs-lookup"><span data-stu-id="48988-547">ACR</span></span>
* <span data-ttu-id="48988-548">Adicionado o comando 'acr check-health'</span><span class="sxs-lookup"><span data-stu-id="48988-548">Added 'acr check-health' command</span></span>
* <span data-ttu-id="48988-549">Melhorado o tratamento de erro para tokens do AAD e para recuperar comandos externos</span><span class="sxs-lookup"><span data-stu-id="48988-549">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="48988-550">ACS</span><span class="sxs-lookup"><span data-stu-id="48988-550">ACS</span></span>
* <span data-ttu-id="48988-551">Comandos preteridos do ACS agora ficam ocultos da exibição da ajuda</span><span class="sxs-lookup"><span data-stu-id="48988-551">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="48988-552">AMS</span><span class="sxs-lookup"><span data-stu-id="48988-552">AMS</span></span>
* <span data-ttu-id="48988-553">[ALTERAÇÃO SIGNIFICATIVA] Alterada para retornar cadeias de caracteres de tempo da ISO 8601 para archive-window-length e key-frame-interval-duration</span><span class="sxs-lookup"><span data-stu-id="48988-553">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="48988-554">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-554">AppService</span></span>
* <span data-ttu-id="48988-555">Adicionado roteamento com base no local para `webapp deleted list` e `webapp deleted restore`</span><span class="sxs-lookup"><span data-stu-id="48988-555">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="48988-556">Corrigido problema em que a URL de destino registrada do webapp ("Não é possível iniciar o aplicativo em...") não era clicável no Azure Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="48988-556">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="48988-557">Corrigido um problema em que a criação de aplicativos com algumas SKUs falhava com um erro de AlwaysOn</span><span class="sxs-lookup"><span data-stu-id="48988-557">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="48988-558">Adicionada a pré-validação para o `[appservice|webapp] create`</span><span class="sxs-lookup"><span data-stu-id="48988-558">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="48988-559">Corrigido o `[webapp|functionapp] traffic-routing` para usar o actionHostName correto</span><span class="sxs-lookup"><span data-stu-id="48988-559">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="48988-560">Adicionado o suporte de slot para comandos `functionapp`</span><span class="sxs-lookup"><span data-stu-id="48988-560">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="48988-561">Lote</span><span class="sxs-lookup"><span data-stu-id="48988-561">Batch</span></span>
* <span data-ttu-id="48988-562">Corrigida a regressão de autenticação do AAD causada pela geração de relatórios de erros superagressiva para autenticação de chave compartilhada</span><span class="sxs-lookup"><span data-stu-id="48988-562">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="48988-563">BatchAI</span><span class="sxs-lookup"><span data-stu-id="48988-563">BatchAI</span></span>
* <span data-ttu-id="48988-564">Agora os comandos do BatchAI estão preteridos e ocultos</span><span class="sxs-lookup"><span data-stu-id="48988-564">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="48988-565">BotService</span><span class="sxs-lookup"><span data-stu-id="48988-565">BotService</span></span>
* <span data-ttu-id="48988-566">Adição das mensagens de aviso "suporte descontinuado"/"modo de manutenção" para os comandos compatíveis com a v3 do SDK</span><span class="sxs-lookup"><span data-stu-id="48988-566">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="48988-567">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="48988-567">CosmosDB</span></span>
* <span data-ttu-id="48988-568">[PRETERIDO] Preterido o comando `cosmosdb list-keys`</span><span class="sxs-lookup"><span data-stu-id="48988-568">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="48988-569">Adicionado o comando `cosmosdb keys list` – substitui o `cosmosdb list-keys`</span><span class="sxs-lookup"><span data-stu-id="48988-569">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="48988-570">`cosmsodb create/update`: Adicionado novo formato para --location a fim de permitir a configuração da propriedade "isZoneRedundant".</span><span class="sxs-lookup"><span data-stu-id="48988-570">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="48988-571">Formato antigo preterido</span><span class="sxs-lookup"><span data-stu-id="48988-571">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="48988-572">EventGrid</span><span class="sxs-lookup"><span data-stu-id="48988-572">EventGrid</span></span>
* <span data-ttu-id="48988-573">Adicionados comandos do `eventgrid domain` para operações de CRUD no domínio</span><span class="sxs-lookup"><span data-stu-id="48988-573">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="48988-574">Adicionados comandos do `eventgrid domain topic` para operações de CRUD nos tópicos do domínio</span><span class="sxs-lookup"><span data-stu-id="48988-574">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="48988-575">Adicionado argumento do `--odata-query` ao `eventgrid [topic|event-subscription] list` para filtrar os resultados usando a sintaxe do OData</span><span class="sxs-lookup"><span data-stu-id="48988-575">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="48988-576">`event-subscription create/update`: Adicionado o servicebusqueue como novos valores para o parâmetro `--endpoint-type`</span><span class="sxs-lookup"><span data-stu-id="48988-576">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="48988-577">[ALTERAÇÃO SIGNIFICATIVA] Removido o suporte para `--included-event-types All` com `eventgrid event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48988-577">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="48988-578">HDInsight</span><span class="sxs-lookup"><span data-stu-id="48988-578">HDInsight</span></span>
* <span data-ttu-id="48988-579">Adicionado suporte para o parâmetro `--ssh-public-key` no comando `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="48988-579">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="48988-580">IoT</span><span class="sxs-lookup"><span data-stu-id="48988-580">IoT</span></span>
* <span data-ttu-id="48988-581">Adicionado suporte para regenerar as chaves da política de autorização</span><span class="sxs-lookup"><span data-stu-id="48988-581">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="48988-582">Adicionados SDK e suporte para o serviço de provisionamento de repositórios do DigitalTwin</span><span class="sxs-lookup"><span data-stu-id="48988-582">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="48988-583">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-583">Network</span></span>
* <span data-ttu-id="48988-584">Adicionado suporte de zona para o Gateway da NAT</span><span class="sxs-lookup"><span data-stu-id="48988-584">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="48988-585">Adicionado o comando `network list-service-tags`</span><span class="sxs-lookup"><span data-stu-id="48988-585">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="48988-586">Corrigido o problema com o `dns zone import` em que os usuários não conseguiam importar registros do curinga A</span><span class="sxs-lookup"><span data-stu-id="48988-586">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="48988-587">Corrigido o problema com o `watcher flow-log configure` em que o registro de fluxo não podia ser habilitado em determinadas regiões</span><span class="sxs-lookup"><span data-stu-id="48988-587">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="48988-588">Recurso</span><span class="sxs-lookup"><span data-stu-id="48988-588">Resource</span></span>
* <span data-ttu-id="48988-589">Adicionado o comando do `az rest` para fazer chamadas REST</span><span class="sxs-lookup"><span data-stu-id="48988-589">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="48988-590">Corrigido o erro ao usar o `policy assignment list` com um grupo de recursos ou o nível de assinatura `--scope`</span><span class="sxs-lookup"><span data-stu-id="48988-590">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="48988-591">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="48988-591">ServiceBus</span></span>
* <span data-ttu-id="48988-592">Corrigido o problema com o `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span><span class="sxs-lookup"><span data-stu-id="48988-592">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="48988-593">SQL</span><span class="sxs-lookup"><span data-stu-id="48988-593">SQL</span></span>
* <span data-ttu-id="48988-594">Alterado o `--location` para ser opcional para `sql [server|mi] create` – usa o local do grupo de recursos se não especificado</span><span class="sxs-lookup"><span data-stu-id="48988-594">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="48988-595">Corrigido o erro "objeto 'NoneType' não é iterável" para `sql db list-editions --available`</span><span class="sxs-lookup"><span data-stu-id="48988-595">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="48988-596">SQLVm</span><span class="sxs-lookup"><span data-stu-id="48988-596">SQLVm</span></span>
* <span data-ttu-id="48988-597">[ALTERAÇÃO DA FALHA] Alterado `sql vm create` para exigir o parâmetro `--license-type`</span><span class="sxs-lookup"><span data-stu-id="48988-597">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="48988-598">Alterado para permitir a configuração da SKU da imagem do SQL ao criar ou atualizar uma VM do SQL</span><span class="sxs-lookup"><span data-stu-id="48988-598">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="48988-599">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48988-599">Storage</span></span>
* <span data-ttu-id="48988-600">Corrigido o problema com a chave de conta ignorada para `storage container generate-sas`</span><span class="sxs-lookup"><span data-stu-id="48988-600">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="48988-601">Corrigido o problema com o `storage blob sync` no Linux</span><span class="sxs-lookup"><span data-stu-id="48988-601">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="48988-602">VM</span><span class="sxs-lookup"><span data-stu-id="48988-602">VM</span></span>
* <span data-ttu-id="48988-603">[VERSÃO PRÉVIA] Adicionados os comandos `vm image template` para criar imagens de VM</span><span class="sxs-lookup"><span data-stu-id="48988-603">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="48988-604">4 de junho de 2019</span><span class="sxs-lookup"><span data-stu-id="48988-604">June 4, 2019</span></span>

<span data-ttu-id="48988-605">Versão 2.0.66</span><span class="sxs-lookup"><span data-stu-id="48988-605">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="48988-606">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48988-606">Core</span></span>
* <span data-ttu-id="48988-607">Foi corrigido o bug em que os comandos falhavam quando `--output yaml` era usado com `--query`</span><span class="sxs-lookup"><span data-stu-id="48988-607">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="48988-608">ACR</span><span class="sxs-lookup"><span data-stu-id="48988-608">ACR</span></span>
* <span data-ttu-id="48988-609">Foi adicionado o grupo de comando 'pack acr' para a criação de Tarefas de build rápida usando Buildpacks.</span><span class="sxs-lookup"><span data-stu-id="48988-609">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="48988-610">ACS</span><span class="sxs-lookup"><span data-stu-id="48988-610">ACS</span></span>
* <span data-ttu-id="48988-611">Permitir a opção de habilitar/desabilitar o complemento kube-dashboard do AKS</span><span class="sxs-lookup"><span data-stu-id="48988-611">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="48988-612">Imprimir uma mensagem amigável quando a assinatura não estiver na lista de permissões para usar o Red Hat OpenShift no Azure</span><span class="sxs-lookup"><span data-stu-id="48988-612">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="48988-613">Lote</span><span class="sxs-lookup"><span data-stu-id="48988-613">Batch</span></span>
* <span data-ttu-id="48988-614">Melhoria no tratamento de erro quando você não está conectado a uma conta \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span><span class="sxs-lookup"><span data-stu-id="48988-614">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="48988-615">IoT</span><span class="sxs-lookup"><span data-stu-id="48988-615">IoT</span></span>
* <span data-ttu-id="48988-616">Foi adicionado o suporte para failover manual</span><span class="sxs-lookup"><span data-stu-id="48988-616">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="48988-617">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-617">Network</span></span>
* <span data-ttu-id="48988-618">Foram adicionados os comandos `network application-gateway waf-policy` para oferecer suporte às regras de WAF personalizadas.</span><span class="sxs-lookup"><span data-stu-id="48988-618">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="48988-619">Adicionados os argumentos `--waf-policy` e `--max-capacity` para `network application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48988-619">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="48988-620">Recurso</span><span class="sxs-lookup"><span data-stu-id="48988-620">Resource</span></span>
* <span data-ttu-id="48988-621">Melhoria da mensagem de erro do `deployment create` quando não há nenhum TTY disponível</span><span class="sxs-lookup"><span data-stu-id="48988-621">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="48988-622">Função</span><span class="sxs-lookup"><span data-stu-id="48988-622">Role</span></span>
* <span data-ttu-id="48988-623">O texto da Ajuda foi atualizado.</span><span class="sxs-lookup"><span data-stu-id="48988-623">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="48988-624">Computação</span><span class="sxs-lookup"><span data-stu-id="48988-624">Compute</span></span>
* <span data-ttu-id="48988-625">Foi adicionado o suporte para `vm create` para as VMs de uma imagem gerenciada com LUNs de disco de dados que não começam em 0 ou que ignoram números</span><span class="sxs-lookup"><span data-stu-id="48988-625">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="48988-626">21 de maio de 2019</span><span class="sxs-lookup"><span data-stu-id="48988-626">May 21, 2019</span></span>

<span data-ttu-id="48988-627">Versão 2.0.65</span><span class="sxs-lookup"><span data-stu-id="48988-627">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="48988-628">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48988-628">Core</span></span>
* <span data-ttu-id="48988-629">Foram adicionados comentários melhores para erros de autenticação</span><span class="sxs-lookup"><span data-stu-id="48988-629">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="48988-630">Corrigido um problema em que a CLI carregava extensões que não eram compatíveis com a versão do núcleo</span><span class="sxs-lookup"><span data-stu-id="48988-630">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="48988-631">Corrigido um problema com a inicialização quando `clouds.config` está corrompido</span><span class="sxs-lookup"><span data-stu-id="48988-631">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="48988-632">ACR</span><span class="sxs-lookup"><span data-stu-id="48988-632">ACR</span></span>
* <span data-ttu-id="48988-633">Foi adicionado suporte das Identidades Gerenciadas para Tarefas</span><span class="sxs-lookup"><span data-stu-id="48988-633">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="48988-634">ACS</span><span class="sxs-lookup"><span data-stu-id="48988-634">ACS</span></span>
* <span data-ttu-id="48988-635">Corrigido o comando `openshift create` quando usado com o cliente AAD do consumidor</span><span class="sxs-lookup"><span data-stu-id="48988-635">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="48988-636">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-636">AppService</span></span>
* <span data-ttu-id="48988-637">[PRETERIDO] Preterido o comando `functionapp devops-build` – Será removido na próxima versão</span><span class="sxs-lookup"><span data-stu-id="48988-637">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="48988-638">`functionapp devops-pipeline` foi alterado para buscar o log de build do Azure DevOps no modo detalhado</span><span class="sxs-lookup"><span data-stu-id="48988-638">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="48988-639">[ALTERAÇÃO SIGNIFICATIVA] O sinalizador `--use_local_settings` foi removido do comando `functionapp devops-pipeline` – não estava operacional</span><span class="sxs-lookup"><span data-stu-id="48988-639">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="48988-640">`webapp up` foi alterado para retornar uma saída JSON se `--logs` não for usado</span><span class="sxs-lookup"><span data-stu-id="48988-640">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="48988-641">Foi adicionado suporte para escrever recursos padrão para a configuração local de `webapp up`</span><span class="sxs-lookup"><span data-stu-id="48988-641">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="48988-642">Foi adicionado suporte para `webapp up` reimplantar um aplicativo sem usar o argumento `--location`</span><span class="sxs-lookup"><span data-stu-id="48988-642">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="48988-643">Corrigido um problema em que o valor do SKU gratuito não funcionava na criação do ASP do SKU gratuito do Linux</span><span class="sxs-lookup"><span data-stu-id="48988-643">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="48988-644">BotService</span><span class="sxs-lookup"><span data-stu-id="48988-644">BotService</span></span>
* <span data-ttu-id="48988-645">Alterado para permitir todas as capitalizações para parâmetros `--lang` em todos os comandos</span><span class="sxs-lookup"><span data-stu-id="48988-645">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="48988-646">Descrição atualizada do módulo de comando</span><span class="sxs-lookup"><span data-stu-id="48988-646">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="48988-647">Consumo</span><span class="sxs-lookup"><span data-stu-id="48988-647">Consumption</span></span>
* <span data-ttu-id="48988-648">O parâmetro obrigatório ausente foi adicionado para executar `consumption usage list --billing-period-name`</span><span class="sxs-lookup"><span data-stu-id="48988-648">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="48988-649">IoT</span><span class="sxs-lookup"><span data-stu-id="48988-649">IoT</span></span>
* <span data-ttu-id="48988-650">Suporte adicionado para listar todas as chaves</span><span class="sxs-lookup"><span data-stu-id="48988-650">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="48988-651">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-651">Network</span></span>
* [ALTERAÇÃO SIGNIFICATIVA]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="48988-653">O argumento `--nat-gateway` foi adicionado a `network vnet subnet [create|update]` para anexar a um gateway NAT</span><span class="sxs-lookup"><span data-stu-id="48988-653">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="48988-654">Corrigido o problema de `dns zone import`, em que os nomes de registro não correspondiam ao tipo de registro</span><span class="sxs-lookup"><span data-stu-id="48988-654">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="48988-655">RDBMS</span><span class="sxs-lookup"><span data-stu-id="48988-655">RDBMS</span></span>
* <span data-ttu-id="48988-656">Suporte a postgres e mysql adicionado para replicação geográfica</span><span class="sxs-lookup"><span data-stu-id="48988-656">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="48988-657">RBAC</span><span class="sxs-lookup"><span data-stu-id="48988-657">RBAC</span></span>
* <span data-ttu-id="48988-658">Adição de suporte do escopo de grupo de gerenciamento a `role assignment`</span><span class="sxs-lookup"><span data-stu-id="48988-658">Added support for management group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="48988-659">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48988-659">Storage</span></span>
* <span data-ttu-id="48988-660">`storage blob sync`: adicionar um comando de sincronização ao armazenamento de blobs</span><span class="sxs-lookup"><span data-stu-id="48988-660">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="48988-661">Computação</span><span class="sxs-lookup"><span data-stu-id="48988-661">Compute</span></span>
* <span data-ttu-id="48988-662">`--computer-name` foi adicionado a `vm create` para configurar o nome do computador da VM</span><span class="sxs-lookup"><span data-stu-id="48988-662">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="48988-663">`--ssh-key-value` foi renomeado para `--ssh-key-values` para `[vm|vmss] create` – Agora, pode aceitar vários valores de chave pública ou caminhos ssh</span><span class="sxs-lookup"><span data-stu-id="48988-663">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="48988-664">__Observação__: Isso **não** é uma alteração da falha – `--ssh-key-value` será analisado corretamente, pois corresponde somente a `--ssh-key-values`</span><span class="sxs-lookup"><span data-stu-id="48988-664">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="48988-665">O argumento `--type` de `ppg create` foi alterado para ser opcional</span><span class="sxs-lookup"><span data-stu-id="48988-665">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="48988-666">6 de maio de 2019</span><span class="sxs-lookup"><span data-stu-id="48988-666">May 6, 2019</span></span>

<span data-ttu-id="48988-667">Versão 2.0.64</span><span class="sxs-lookup"><span data-stu-id="48988-667">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="48988-668">ACS</span><span class="sxs-lookup"><span data-stu-id="48988-668">ACS</span></span>
* <span data-ttu-id="48988-669">[ALTERAÇÃO SIGNIFICATIVA] O sinalizador `--fqdn` foi removido dos comandos `openshift`</span><span class="sxs-lookup"><span data-stu-id="48988-669">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="48988-670">Alterado para usar a versão da API do Red Hat OpenShift no Azure em disponibilidade geral</span><span class="sxs-lookup"><span data-stu-id="48988-670">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="48988-671">O sinalizador `customer-admin-group-id` foi adicionado a `openshift create`</span><span class="sxs-lookup"><span data-stu-id="48988-671">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="48988-672">[GA] `(PREVIEW)` foi removido da opção `aks create` `--network-policy`</span><span class="sxs-lookup"><span data-stu-id="48988-672">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="48988-673">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-673">Appservice</span></span>
* <span data-ttu-id="48988-674">[PRETERIDO] O comando `functionapp devops-build` foi preterido</span><span class="sxs-lookup"><span data-stu-id="48988-674">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="48988-675">Renomeado para `functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="48988-675">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="48988-676">Corrigido ao obter o nome de usuário correto para cloudshell que estava causando a falha em `webapp up`</span><span class="sxs-lookup"><span data-stu-id="48988-676">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="48988-677">Documentação `appservice plan --sku` atualizada para refletir o appserviceplans com suporte</span><span class="sxs-lookup"><span data-stu-id="48988-677">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="48988-678">Adicionado argumentos opcionais para o grupo de recursos e plano a `webapp up`</span><span class="sxs-lookup"><span data-stu-id="48988-678">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="48988-679">Adicionado suporte a `webapp ssh` para respeitar a variável de ambiente `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="48988-679">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="48988-680">Adicionado suporte `appserviceplan create` para a SKU gratuita do Linux</span><span class="sxs-lookup"><span data-stu-id="48988-680">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="48988-681">Alterado `webapp up` para ter uma suspensão de 30 segundos depois de definir appsetting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` para lidar com a inicialização a frio kudu</span><span class="sxs-lookup"><span data-stu-id="48988-681">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="48988-682">Adicionado suporte para runtime `powershell` a `functionapp create` no Windows</span><span class="sxs-lookup"><span data-stu-id="48988-682">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="48988-683">Adicionado o comando `create-remote-connection`</span><span class="sxs-lookup"><span data-stu-id="48988-683">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="48988-684">Lote</span><span class="sxs-lookup"><span data-stu-id="48988-684">Batch</span></span>
* <span data-ttu-id="48988-685">Corrigido o bug no validador para as opções `--application-package-references`</span><span class="sxs-lookup"><span data-stu-id="48988-685">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="48988-686">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="48988-686">Botservice</span></span>
* <span data-ttu-id="48988-687">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v4 -k webapp` foi alterado para criar um Bot de Aplicativo Web vazio por padrão (ou seja, nenhum bot será implantado no Serviço de Aplicativo)</span><span class="sxs-lookup"><span data-stu-id="48988-687">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="48988-688">O sinalizador `--echo` foi adicionado ao `bot create` para usar o comportamento antigo com `-v v4`</span><span class="sxs-lookup"><span data-stu-id="48988-688">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="48988-689">[ALTERAÇÃO SIGNIFICATIVA] O valor padrão de `--version` foi alterado para `v4`</span><span class="sxs-lookup"><span data-stu-id="48988-689">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="48988-690">__OBSERVAÇÃO:__ `bot prepare-publish` ainda usa o padrão antigo</span><span class="sxs-lookup"><span data-stu-id="48988-690">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="48988-691">[ALTERAÇÃO SIGNIFICATIVA] `--lang` foi alterado para não definir mais `Csharp` como padrão.</span><span class="sxs-lookup"><span data-stu-id="48988-691">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="48988-692">Se o comando exigir `--lang` e ele não for fornecido, o comando será um erro</span><span class="sxs-lookup"><span data-stu-id="48988-692">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="48988-693">[ALTERAÇÃO SIGNIFICATIVA] Os argumentos `--appid` e `--password` foram alterados para `bot create` ser obrigatório e agora podem ser criados por meio de `ad app create`</span><span class="sxs-lookup"><span data-stu-id="48988-693">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="48988-694">Foi adicionada validação a `--appid` e `--password`</span><span class="sxs-lookup"><span data-stu-id="48988-694">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="48988-695">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v4` foi alterado para não criar ou usar uma Conta de Armazenamento ou o Application Insights</span><span class="sxs-lookup"><span data-stu-id="48988-695">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="48988-696">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v3` foi alterado para exigir uma região em que o Application Insights está disponível</span><span class="sxs-lookup"><span data-stu-id="48988-696">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="48988-697">[ALTERAÇÃO SIGNIFICATIVA] O `bot update` foi alterado para afetar somente as propriedades específicas de um bot</span><span class="sxs-lookup"><span data-stu-id="48988-697">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="48988-698">[ALTERAÇÃO SIGNIFICATIVA] Os sinalizadores `--lang` foram alterados para aceitar `Javascript` em vez de `Node`</span><span class="sxs-lookup"><span data-stu-id="48988-698">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="48988-699">[ALTERAÇÃO SIGNIFICATIVA] O `Node` foi removido como um valor `--lang` permitido</span><span class="sxs-lookup"><span data-stu-id="48988-699">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="48988-700">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v4 -k webapp` foi alterado para não definir mais `SCM_DO_BUILD_DURING_DEPLOYMENT` como verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="48988-700">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="48988-701">Todas as implantações por meio do Kudu atuarão de acordo com o comportamento padrão</span><span class="sxs-lookup"><span data-stu-id="48988-701">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="48988-702">O `bot download` foi alterado para os bots sem arquivos `.bot` para criar o arquivo de configuração específico a um idioma com os valores das Configurações de Aplicativo do bot</span><span class="sxs-lookup"><span data-stu-id="48988-702">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="48988-703">Adicionado o suporte `Typescript` para `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="48988-703">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="48988-704">Uma mensagem de aviso foi adicionada a `bot prepare-deploy` para os bots `Javascript` e `Typescript` para quando `--code-dir` não contiver `package.json`</span><span class="sxs-lookup"><span data-stu-id="48988-704">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="48988-705">O `bot prepare-deploy` foi alterado para retornar `true`, se bem-sucedido</span><span class="sxs-lookup"><span data-stu-id="48988-705">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="48988-706">O log detalhado foi adicionado a `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="48988-706">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="48988-707">Mais regiões disponíveis do Application Insights foram adicionadas ao `az bot create -v v3`</span><span class="sxs-lookup"><span data-stu-id="48988-707">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="48988-708">Configurar</span><span class="sxs-lookup"><span data-stu-id="48988-708">Configure</span></span>
* <span data-ttu-id="48988-709">Adicionado suporte para configurações de valor padrão do argumento baseado em pasta</span><span class="sxs-lookup"><span data-stu-id="48988-709">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="48988-710">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="48988-710">Eventhubs</span></span>
* <span data-ttu-id="48988-711">Adicionados os comandos `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="48988-711">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="48988-712">O argumento `--default-action` foi adicionado às regras de rede de `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48988-712">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="48988-713">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-713">Network</span></span>
* <span data-ttu-id="48988-714">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--cache` foi substituído por `--defer` para `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48988-714">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="48988-715">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="48988-715">Policy Insights</span></span>
* <span data-ttu-id="48988-716">Suporte adicionado a `--expand PolicyEvaluationDetails` para detalhes de avaliação de política de consulta no recurso</span><span class="sxs-lookup"><span data-stu-id="48988-716">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="48988-717">Função</span><span class="sxs-lookup"><span data-stu-id="48988-717">Role</span></span>
* <span data-ttu-id="48988-718">[PRETERIDO] Alterado argumento ocultar '--password' `create-for-rbac` - suporte será removido em maio de 2019</span><span class="sxs-lookup"><span data-stu-id="48988-718">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="48988-719">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="48988-719">Service Bus</span></span>
* <span data-ttu-id="48988-720">Adicionados os comandos `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="48988-720">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="48988-721">O argumento `--default-action` foi adicionado às regras de rede de `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48988-721">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="48988-722">`topic [create|update]` foi fixado para permitir suporte a `--max-size` para valores de 10, 20, 40 e 80 GB com a SKU Premium</span><span class="sxs-lookup"><span data-stu-id="48988-722">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="48988-723">SQL</span><span class="sxs-lookup"><span data-stu-id="48988-723">SQL</span></span>
* <span data-ttu-id="48988-724">Adicionados os comandos `sql virtual-cluster [list|show|delete]`</span><span class="sxs-lookup"><span data-stu-id="48988-724">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="48988-725">VM</span><span class="sxs-lookup"><span data-stu-id="48988-725">VM</span></span>
* <span data-ttu-id="48988-726">O `--protect-from-scale-in` e o `--protect-from-scale-set-actions` foram adicionados a `vmss update` para habilitar atualizações à política de proteção das instâncias de VM VMSS</span><span class="sxs-lookup"><span data-stu-id="48988-726">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="48988-727">Adicionado a `--instance-id` e `vmss update` para habilitar atualização genérica das instâncias de VM VMSS</span><span class="sxs-lookup"><span data-stu-id="48988-727">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="48988-728">`--instance-id` foi adicionado a `vmss wait`</span><span class="sxs-lookup"><span data-stu-id="48988-728">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="48988-729">Adição do novo grupo de comandos `ppg` para gerenciar Grupos de Posicionamento de Proximidade</span><span class="sxs-lookup"><span data-stu-id="48988-729">Added new `ppg` command group for managing Proximity Placement Groups</span></span>
* <span data-ttu-id="48988-730">Adicionado a `--ppg`, `[vm|vmss] create` e `vm availability-set create` para gerenciar PPGs</span><span class="sxs-lookup"><span data-stu-id="48988-730">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="48988-731">Parâmetro `--hyper-v-generation` adicionado a `image create`</span><span class="sxs-lookup"><span data-stu-id="48988-731">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="48988-732">23 de abril de 2019</span><span class="sxs-lookup"><span data-stu-id="48988-732">April 23, 2019</span></span>

<span data-ttu-id="48988-733">Versão 2.0.63</span><span class="sxs-lookup"><span data-stu-id="48988-733">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="48988-734">ACS</span><span class="sxs-lookup"><span data-stu-id="48988-734">ACS</span></span>
* <span data-ttu-id="48988-735">Alterado `aks get-credentials` para solicitar substituição dos valores duplicados</span><span class="sxs-lookup"><span data-stu-id="48988-735">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="48988-736">Removido `(PREVIEW)` dos comandos de espaços de desenvolvimento "aks use-dev-espaces" e "aks remove-dev-espaces"</span><span class="sxs-lookup"><span data-stu-id="48988-736">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="48988-737">AMS</span><span class="sxs-lookup"><span data-stu-id="48988-737">AMS</span></span>
* <span data-ttu-id="48988-738">Corrigido o bug com a atualização de filtros de conta e de ativo</span><span class="sxs-lookup"><span data-stu-id="48988-738">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="48988-739">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-739">AppService</span></span>
* <span data-ttu-id="48988-740">Adicionado suporte para o ASE e o tempo limite para `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="48988-740">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="48988-741">Adicionado suporte para o estabelecimento de CI CD em um pipeline do Azure DevOps de um repositório do Github para aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="48988-741">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="48988-742">Adicionado argumento `--github-pat` a `functionapp devops-build create` para aceitar o token de acesso pessoal do Github</span><span class="sxs-lookup"><span data-stu-id="48988-742">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="48988-743">Adicionado argumento `--github-repository` a `functionapp devops-build create` para aceitar o repositório Github que contém um código-fonte functionapp</span><span class="sxs-lookup"><span data-stu-id="48988-743">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="48988-744">Problema corrigido em que `az webapp up --logs` estava falhando com um erro e atualização da versão .NETCORE padrão para 2.1</span><span class="sxs-lookup"><span data-stu-id="48988-744">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="48988-745">Configurações de functionapp desnecessárias removidas durante a criação de um aplicativo de funções com plano de consumo</span><span class="sxs-lookup"><span data-stu-id="48988-745">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="48988-746">Alterado `webapp up` para que a cadeia de caracteres padrão asp agora acrescente o número no final para criar um novo ASP com base nas opções de SKU</span><span class="sxs-lookup"><span data-stu-id="48988-746">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="48988-747">Adicionado `-b` como uma opção a `webapp up` para iniciar o aplicativo no navegador</span><span class="sxs-lookup"><span data-stu-id="48988-747">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="48988-748">Alterado `webapp deployment source config zip` para lidar com a variável de ambiente `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="48988-748">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="48988-749">Gerenciador de Implantação</span><span class="sxs-lookup"><span data-stu-id="48988-749">Deployment Manager</span></span>
* <span data-ttu-id="48988-750">[VERSÃO PRÉVIA] Criar e gerenciar artefatos que dão suporte a distribuições</span><span class="sxs-lookup"><span data-stu-id="48988-750">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="48988-751">Laboratório</span><span class="sxs-lookup"><span data-stu-id="48988-751">Lab</span></span>
* <span data-ttu-id="48988-752">Corrigido o bug que causa uma saída inicial</span><span class="sxs-lookup"><span data-stu-id="48988-752">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="48988-753">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-753">Network</span></span>
* <span data-ttu-id="48988-754">Adicionada delegação de servidor de nome automática a `dns zone create` no pai durante a criação da zona filho</span><span class="sxs-lookup"><span data-stu-id="48988-754">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="48988-755">Recurso</span><span class="sxs-lookup"><span data-stu-id="48988-755">Resource</span></span>
* <span data-ttu-id="48988-756">[PRETERIDO] Argumentos `--link-id`, `--target-id` e `--filter-string` preteridos de `resource link`</span><span class="sxs-lookup"><span data-stu-id="48988-756">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="48988-757">Use os argumentos `--link`, `--target` e `--filter`</span><span class="sxs-lookup"><span data-stu-id="48988-757">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="48988-758">Corrigido o problema em que os comandos `resource link [create|update]` não funcionavam</span><span class="sxs-lookup"><span data-stu-id="48988-758">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="48988-759">Corrigido um problema em que a exclusão usando uma ID de recurso poderia causar falha no erro</span><span class="sxs-lookup"><span data-stu-id="48988-759">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="48988-760">SQL</span><span class="sxs-lookup"><span data-stu-id="48988-760">SQL</span></span>
* <span data-ttu-id="48988-761">Adicionado suporte para fuso horário personalizado nas instâncias gerenciadas</span><span class="sxs-lookup"><span data-stu-id="48988-761">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="48988-762">Alterado para permitir que o nome do pool Elástico seja usado com `sql db update`</span><span class="sxs-lookup"><span data-stu-id="48988-762">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="48988-763">Adicionado o suporte `--no-wait` para `sql server [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48988-763">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="48988-764">Adicionado o comando `sql server wait`</span><span class="sxs-lookup"><span data-stu-id="48988-764">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="48988-765">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48988-765">Storage</span></span>
* <span data-ttu-id="48988-766">Corrigido o problema com tokens SAS com codificação dupla em `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="48988-766">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="48988-767">VM</span><span class="sxs-lookup"><span data-stu-id="48988-767">VM</span></span>
* <span data-ttu-id="48988-768">Adicionado sinalizador `--skip-shutdown` a `vm|vmss stop` para desligar as VMs sem o desligamento</span><span class="sxs-lookup"><span data-stu-id="48988-768">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="48988-769">Adicionado argumento `--storage-account-type` a `sig image-version create` para definir o tipo de conta do perfil de publicação</span><span class="sxs-lookup"><span data-stu-id="48988-769">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="48988-770">Adicionado argumento `--target-regions` a `sig image-version create` para permitir definir os tipos de conta de armazenamento específico da região</span><span class="sxs-lookup"><span data-stu-id="48988-770">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="48988-771">9 de abril de 2019</span><span class="sxs-lookup"><span data-stu-id="48988-771">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="48988-772">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48988-772">Core</span></span>
* <span data-ttu-id="48988-773">Correção do problema em que algumas extensões mostraram uma versão do `Unknown` e não podiam ser atualizadas</span><span class="sxs-lookup"><span data-stu-id="48988-773">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="48988-774">ACR</span><span class="sxs-lookup"><span data-stu-id="48988-774">ACR</span></span>
* <span data-ttu-id="48988-775">Adição de suporte para execução de uma imagem sem contexto</span><span class="sxs-lookup"><span data-stu-id="48988-775">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="48988-776">AMS</span><span class="sxs-lookup"><span data-stu-id="48988-776">AMS</span></span>
* [PRETERIDO]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [ALTERAÇÃO SIGNIFICATIVA]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="48988-779">Adição de suporte para novos parâmetros de criptografia em `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="48988-779">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="48988-780">Adição de novo parâmetro `--filters` a `ams streaming-locator create`</span><span class="sxs-lookup"><span data-stu-id="48988-780">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="48988-781">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-781">AppService</span></span>
* <span data-ttu-id="48988-782">Adicionado o suporte `--logs` para `webapp up`</span><span class="sxs-lookup"><span data-stu-id="48988-782">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="48988-783">Correção de problemas do comando `functionapp devops-build create` de geração de `azure-pipelines.yml`</span><span class="sxs-lookup"><span data-stu-id="48988-783">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="48988-784">Melhoria do tratamento de erros e indicadores `unctionapp devops-build create`</span><span class="sxs-lookup"><span data-stu-id="48988-784">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="48988-785">[ALTERAÇÃO SIGNIFICATIVA] Remoção do sinalizador `--local-git` para o comando `devops-build`; a detecção de git local e a manipulação são obrigatórias para a criação de pipelines do Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="48988-785">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="48988-786">Adição de suporte para a criação de planos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="48988-786">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="48988-787">Adição da capacidade de trocar um plano sob um aplicativo de funções usando `functionapp update --plan`</span><span class="sxs-lookup"><span data-stu-id="48988-787">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="48988-788">Adição de suporte para configurações de expansão de plano Premium do Azure Functions</span><span class="sxs-lookup"><span data-stu-id="48988-788">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="48988-789">CDN</span><span class="sxs-lookup"><span data-stu-id="48988-789">CDN</span></span>
* <span data-ttu-id="48988-790">Adição de suporte para `Microsoft_Standard` e `Standard_ChinaCdn`</span><span class="sxs-lookup"><span data-stu-id="48988-790">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="48988-791">Comentários</span><span class="sxs-lookup"><span data-stu-id="48988-791">Feedback</span></span>
* <span data-ttu-id="48988-792">Alteração de `feedback` para mostrar metadados em comandos executados recentemente</span><span class="sxs-lookup"><span data-stu-id="48988-792">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="48988-793">Alteração de `feedback` para solicitar o auxílio do usuário no processo de criação de problema abrindo um navegador e usando um modelo de problema</span><span class="sxs-lookup"><span data-stu-id="48988-793">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="48988-794">Alteração do `feedback` para imprimir o corpo do problema ao executar com '--verbose'</span><span class="sxs-lookup"><span data-stu-id="48988-794">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="48988-795">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="48988-795">Monitor</span></span>
* <span data-ttu-id="48988-796">Correção de um problema em que “count” não era um valor permitido com `metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48988-796">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="48988-797">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-797">Network</span></span>
* <span data-ttu-id="48988-798">Correção do formato de tabela que não estava sendo exibido com `vnet-gateway list-bgp-peer-status`</span><span class="sxs-lookup"><span data-stu-id="48988-798">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="48988-799">Adição dos comandos `list-request-headers` e `list-response-headers` para `application-gateway rewrite-rule`</span><span class="sxs-lookup"><span data-stu-id="48988-799">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="48988-800">Adição do comando `list-server-variables` para `application-gateway rewrite-rule condition`</span><span class="sxs-lookup"><span data-stu-id="48988-800">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="48988-801">Correção de um problema em que a atualização do estado do link em uma porta express-route geraria uma exceção de atributo desconhecido `express-route port update`</span><span class="sxs-lookup"><span data-stu-id="48988-801">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="48988-802">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="48988-802">PrivateDNS</span></span>
* <span data-ttu-id="48988-803">Adição de `network private-dns` para zonas de DNS privado</span><span class="sxs-lookup"><span data-stu-id="48988-803">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="48988-804">Recurso</span><span class="sxs-lookup"><span data-stu-id="48988-804">Resource</span></span>
* <span data-ttu-id="48988-805">Correção do problema com `deployment create` e `group deployment create`, em que um arquivo de parâmetros com um conjunto vazio de parâmetros não funcionaria</span><span class="sxs-lookup"><span data-stu-id="48988-805">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="48988-806">Função</span><span class="sxs-lookup"><span data-stu-id="48988-806">Role</span></span>
* <span data-ttu-id="48988-807">Correção de `create-for-rbac` para lidar corretamente com `--years`</span><span class="sxs-lookup"><span data-stu-id="48988-807">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="48988-808">[ALTERAÇÃO SIGNIFICATIVA] Alteração de `role assignment delete` para solicitar ao excluir todas as atribuições na assinatura incondicionalmente</span><span class="sxs-lookup"><span data-stu-id="48988-808">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="48988-809">SQL</span><span class="sxs-lookup"><span data-stu-id="48988-809">SQL</span></span>
* <span data-ttu-id="48988-810">Atualização de `sql mi [create|update]` com as propriedades proxyOverride e publicDataEndpointEnabled</span><span class="sxs-lookup"><span data-stu-id="48988-810">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="48988-811">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48988-811">Storage</span></span>
* <span data-ttu-id="48988-812">[ALTERAÇÃO SIGNIFICATIVA] Remoção do resultado de `storage blob delete`</span><span class="sxs-lookup"><span data-stu-id="48988-812">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="48988-813">Adição de `--full-uri` a `storage blob generate-sas` para criar o URI completo para o blob com SAS</span><span class="sxs-lookup"><span data-stu-id="48988-813">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="48988-814">Adição de `--file-snapshot` a `storage file copy start` para copiar arquivo do instantâneo</span><span class="sxs-lookup"><span data-stu-id="48988-814">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="48988-815">Alteração de `storage blob copy cancel` para mostrar apenas o erro em vez da exceção para NoPendingCopyOperation</span><span class="sxs-lookup"><span data-stu-id="48988-815">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="48988-816">26 de março de 2019</span><span class="sxs-lookup"><span data-stu-id="48988-816">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="48988-817">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48988-817">Core</span></span>
* <span data-ttu-id="48988-818">Correção de problemas com incompatibilidade da extensão de desenvolvimento</span><span class="sxs-lookup"><span data-stu-id="48988-818">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="48988-819">Agora o tratamento de erros encaminha os clientes para a página de problemas</span><span class="sxs-lookup"><span data-stu-id="48988-819">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="48988-820">Nuvem</span><span class="sxs-lookup"><span data-stu-id="48988-820">Cloud</span></span>
* <span data-ttu-id="48988-821">Erro de “assinatura não encontrada” corrigido em `cloud set`</span><span class="sxs-lookup"><span data-stu-id="48988-821">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="48988-822">ACR</span><span class="sxs-lookup"><span data-stu-id="48988-822">ACR</span></span>
* <span data-ttu-id="48988-823">Corrigidas fontes redundantes na importação de imagem.</span><span class="sxs-lookup"><span data-stu-id="48988-823">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="48988-824">`--auth-mode` adicionado aos comandos `acr build`, `acr run`, `acr task create` e `acr task update`</span><span class="sxs-lookup"><span data-stu-id="48988-824">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="48988-825">Grupo de comandos “acr task credential” adicionado para gerenciar as credenciais de uma Tarefa</span><span class="sxs-lookup"><span data-stu-id="48988-825">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="48988-826">“--no-wait” adicionado ao comando `acr build`</span><span class="sxs-lookup"><span data-stu-id="48988-826">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="48988-827">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-827">AppService</span></span>
* <span data-ttu-id="48988-828">Bug corrigido onde `webapp up` não estava lidando corretamente com a execução do diretório vazio ou do cenário de código desconhecido</span><span class="sxs-lookup"><span data-stu-id="48988-828">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="48988-829">Bug corrigido onde os slots não funcionavam para `[webapp|functionapp] config ssl bind`</span><span class="sxs-lookup"><span data-stu-id="48988-829">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="48988-830">Serviço de BOT</span><span class="sxs-lookup"><span data-stu-id="48988-830">BOT Service</span></span>
* <span data-ttu-id="48988-831">`bot prepare-deploy` adicionado para se preparar para a implantação de bots via `webapp`</span><span class="sxs-lookup"><span data-stu-id="48988-831">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="48988-832">`bot create --kind registration` alterado para mostrar a senha se ela não for fornecida</span><span class="sxs-lookup"><span data-stu-id="48988-832">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="48988-833">[ALTERAÇÃO SIGNIFICATIVA] `--endpoint` alterado em `bot create --kind registration` como padrão para uma cadeia de caracteres vazia, em vez de ser requerido</span><span class="sxs-lookup"><span data-stu-id="48988-833">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="48988-834">Adicionado `SCM_DO_BUILD_DURING_DEPLOYMENT` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.</span><span class="sxs-lookup"><span data-stu-id="48988-834">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="48988-835">CDN</span><span class="sxs-lookup"><span data-stu-id="48988-835">CDN</span></span>
* <span data-ttu-id="48988-836">Adicionado o suporte ao `--no-wait` para `cdn endpoint [create|update|start|stop|delete|load|purge]`</span><span class="sxs-lookup"><span data-stu-id="48988-836">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* [ALTERAÇÃO SIGNIFICATIVA]: `cdn endpoint create` alterado para o comportamento de cache da cadeia de consulta padrão.
[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour. <span data-ttu-id="48988-838">Não há mais padrão para "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="48988-838">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="48988-839">Agora, ele é definido pelo serviço</span><span class="sxs-lookup"><span data-stu-id="48988-839">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="48988-840">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="48988-840">Cosmosdb</span></span>
* <span data-ttu-id="48988-841">Suporte adicionado para `--enable-multiple-write-locations` na atualização da conta</span><span class="sxs-lookup"><span data-stu-id="48988-841">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="48988-842">O subgrupo `network-rule` foi adicionado com os comandos `add`, `remove` e `list` para gerenciar as regras de VNET de uma conta do Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="48988-842">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="48988-843">Interativo</span><span class="sxs-lookup"><span data-stu-id="48988-843">Interactive</span></span>
* <span data-ttu-id="48988-844">Incompatibilidade corrigida com a extensão Interativa instalada por meio do azdev</span><span class="sxs-lookup"><span data-stu-id="48988-844">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="48988-845">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="48988-845">Monitor</span></span>
* <span data-ttu-id="48988-846">Alterado para permitir o valor de dimensão `*` para `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48988-846">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="48988-847">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-847">Network</span></span>
* <span data-ttu-id="48988-848">Grupo de comandos `rewrite-rule` adicionado em `application-gateway`</span><span class="sxs-lookup"><span data-stu-id="48988-848">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="48988-849">Perfil</span><span class="sxs-lookup"><span data-stu-id="48988-849">Profile</span></span>
* <span data-ttu-id="48988-850">Suporte de conta no nível do locatário para a identidade de serviço gerenciado adicionado em `login`</span><span class="sxs-lookup"><span data-stu-id="48988-850">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="48988-851">Postgres</span><span class="sxs-lookup"><span data-stu-id="48988-851">Postgres</span></span> 
* <span data-ttu-id="48988-852">Adicionados os comandos postgresql `replica` e `restart server`</span><span class="sxs-lookup"><span data-stu-id="48988-852">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="48988-853">Alterado para obter o local padrão do grupo de recursos quando não fornecido para criar servidores e adicionar validação para os dias de retenção</span><span class="sxs-lookup"><span data-stu-id="48988-853">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="48988-854">Recurso</span><span class="sxs-lookup"><span data-stu-id="48988-854">Resource</span></span>
* <span data-ttu-id="48988-855">Saída da tabela aperfeiçoada para `deployment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="48988-855">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="48988-856">Corrigido o problema com `deployment [create|validate]` onde o tipo secureObject não era reconhecido</span><span class="sxs-lookup"><span data-stu-id="48988-856">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="48988-857">Grafo</span><span class="sxs-lookup"><span data-stu-id="48988-857">Graph</span></span>
* <span data-ttu-id="48988-858">Adicionado o suporte ao `--end-date` para `ad [app|sp] credential reset`</span><span class="sxs-lookup"><span data-stu-id="48988-858">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="48988-859">Suporte adicionado para acrescentar permissões com `ad app permission add`</span><span class="sxs-lookup"><span data-stu-id="48988-859">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="48988-860">Bug corrigido com `ad app permission list` quando não havia nenhuma permissão</span><span class="sxs-lookup"><span data-stu-id="48988-860">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="48988-861">`ad sp delete` alterado para ignorar a exclusão da atribuição de função se a conta atual não tem nenhuma assinatura</span><span class="sxs-lookup"><span data-stu-id="48988-861">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="48988-862">`ad app create` alterado para `--identifier-uris` passar para lista vazia como padrão se não fornecido</span><span class="sxs-lookup"><span data-stu-id="48988-862">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="48988-863">storage</span><span class="sxs-lookup"><span data-stu-id="48988-863">storage</span></span>
* <span data-ttu-id="48988-864">`--snapshot` adicionado a `storage file download-batch` para baixar de um instantâneo de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="48988-864">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="48988-865">Barra de progresso `storage blob [download-batch|upload-batch]` alterada para ser menos detalhada e indicar o blob atual</span><span class="sxs-lookup"><span data-stu-id="48988-865">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="48988-866">Problema corrigido com `storage account update` ao atualizar os parâmetros de criptografia</span><span class="sxs-lookup"><span data-stu-id="48988-866">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="48988-867">Problema corrigido onde `storage blob show` falharia ao usar o oauth (`--auth-mode=login`)</span><span class="sxs-lookup"><span data-stu-id="48988-867">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="48988-868">VM</span><span class="sxs-lookup"><span data-stu-id="48988-868">VM</span></span>
* <span data-ttu-id="48988-869">Adicionado o comando `image update`</span><span class="sxs-lookup"><span data-stu-id="48988-869">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="48988-870">12 de março de 2019</span><span class="sxs-lookup"><span data-stu-id="48988-870">March 12, 2019</span></span>

<span data-ttu-id="48988-871">Versão 2.0.60</span><span class="sxs-lookup"><span data-stu-id="48988-871">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="48988-872">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48988-872">Core</span></span>

* <span data-ttu-id="48988-873">Foi corrigido um erro incorreto no `cloud set` sobre assinatura não encontrada.</span><span class="sxs-lookup"><span data-stu-id="48988-873">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="48988-874">ACR</span><span class="sxs-lookup"><span data-stu-id="48988-874">ACR</span></span>

* <span data-ttu-id="48988-875">Corrigidas fontes redundantes na importação de imagem.</span><span class="sxs-lookup"><span data-stu-id="48988-875">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="48988-876">ACS</span><span class="sxs-lookup"><span data-stu-id="48988-876">ACS</span></span>

* <span data-ttu-id="48988-877">Alteração para ignorar o parâmetro `--listen-address` para `aks browse` se ele não for compatível com kubectl</span><span class="sxs-lookup"><span data-stu-id="48988-877">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="48988-878">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-878">AppService</span></span>

* <span data-ttu-id="48988-879">Adicionado `[webapp|functionapp] deployment list-publishing-credentials` para obter a URL de publicação do Kudu e suas credenciais.</span><span class="sxs-lookup"><span data-stu-id="48988-879">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="48988-880">Removida a instrução de impressão errônea de `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="48988-880">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="48988-881">Corrigido `functionapp` para definir a imagem correta do runtime nos planos do Serviço de Aplicativo no Linux.</span><span class="sxs-lookup"><span data-stu-id="48988-881">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="48988-882">Removida a marca de versão prévia do `webapp up` e adicionadas melhorias ao comando.</span><span class="sxs-lookup"><span data-stu-id="48988-882">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="48988-883">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="48988-883">Botservice</span></span>

* <span data-ttu-id="48988-884">Adicionado `SCM_DO_BUILD_DURING_DEPLOYMENT` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.</span><span class="sxs-lookup"><span data-stu-id="48988-884">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="48988-885">Adicionados `Microsoft-BotFramework-AppId` e `Microsoft-BotFramework-AppPassword` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.</span><span class="sxs-lookup"><span data-stu-id="48988-885">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="48988-886">Removidas as aspas simples da saída de comando `bot publish`, no final de `bot create`.</span><span class="sxs-lookup"><span data-stu-id="48988-886">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="48988-887">Alterado `bot publish` para que seja assíncrono.</span><span class="sxs-lookup"><span data-stu-id="48988-887">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="48988-888">Contêiner</span><span class="sxs-lookup"><span data-stu-id="48988-888">Container</span></span>

* <span data-ttu-id="48988-889">Adicionado o argumento `--no-wait` para `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="48988-889">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="48988-890">EventHub</span><span class="sxs-lookup"><span data-stu-id="48988-890">EventHub</span></span>

* <span data-ttu-id="48988-891">Adicionado o sinalizador `--skip-empty-archives` a `eventhub create|update` para dar suporte a arquivos vazios na captura.</span><span class="sxs-lookup"><span data-stu-id="48988-891">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="48988-892">Localizar</span><span class="sxs-lookup"><span data-stu-id="48988-892">Find</span></span>

* <span data-ttu-id="48988-893">Atualização de funcionalidade principal</span><span class="sxs-lookup"><span data-stu-id="48988-893">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="48988-894">HDInsight</span><span class="sxs-lookup"><span data-stu-id="48988-894">HDInsight</span></span>

* <span data-ttu-id="48988-895">Adicionado o parâmetro `--storage-account-managed-identity` a `hdinsight create` para oferecer suporte ao MSI do ADLS Gen2.</span><span class="sxs-lookup"><span data-stu-id="48988-895">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="48988-896">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-896">Network</span></span>

* <span data-ttu-id="48988-897">Corrigido o problema com `vpn-connection update`, onde a atualização de uma conexão VPN entre gateways em assinaturas diferentes falharia.</span><span class="sxs-lookup"><span data-stu-id="48988-897">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="48988-898">Rdbms</span><span class="sxs-lookup"><span data-stu-id="48988-898">Rdbms</span></span>

* <span data-ttu-id="48988-899">Correções secundárias para obter a localização padrão do grupo de recursos, quando não fornecida, para criar servidores e adicionar validação nos dias de retenção.</span><span class="sxs-lookup"><span data-stu-id="48988-899">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="48988-900">Função</span><span class="sxs-lookup"><span data-stu-id="48988-900">Role</span></span>

* <span data-ttu-id="48988-901">Corrigido `role definition update` para usar ID a fim de resolver a definição corretamente.</span><span class="sxs-lookup"><span data-stu-id="48988-901">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="48988-902">Alterado `ad app credential reset` para remover a suposição de que a entidade de serviço do aplicativo já existe.</span><span class="sxs-lookup"><span data-stu-id="48988-902">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="48988-903">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="48988-903">Service Fabric</span></span>

* <span data-ttu-id="48988-904">Corrigido o problema com o fato de `sf cluster list` não ser iterável.</span><span class="sxs-lookup"><span data-stu-id="48988-904">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="48988-905">26 de fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="48988-905">February 26, 2019</span></span>

<span data-ttu-id="48988-906">Versão 2.0.59</span><span class="sxs-lookup"><span data-stu-id="48988-906">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="48988-907">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48988-907">Core</span></span>

* <span data-ttu-id="48988-908">Corrigido o problema onde algumas instâncias usando `--subscription NAME` produziriam uma exceção</span><span class="sxs-lookup"><span data-stu-id="48988-908">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="48988-909">ACR</span><span class="sxs-lookup"><span data-stu-id="48988-909">ACR</span></span>

* <span data-ttu-id="48988-910">Parâmetro `--target` adicionado para os comandos `acr build`, `acr task create` e `acr task update`</span><span class="sxs-lookup"><span data-stu-id="48988-910">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="48988-911">Melhor tratamento de erros para os comandos de execução quando não conectado ao Azure</span><span class="sxs-lookup"><span data-stu-id="48988-911">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="48988-912">ACS</span><span class="sxs-lookup"><span data-stu-id="48988-912">ACS</span></span>

* <span data-ttu-id="48988-913">Opção `--listen-address` adicionada a `aks port-forward`</span><span class="sxs-lookup"><span data-stu-id="48988-913">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="48988-914">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-914">AppService</span></span>

* <span data-ttu-id="48988-915">Adicionado o comando `functionapp devops-build`</span><span class="sxs-lookup"><span data-stu-id="48988-915">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="48988-916">Lote</span><span class="sxs-lookup"><span data-stu-id="48988-916">Batch</span></span>
* <span data-ttu-id="48988-917">[ALTERAÇÃO SIGNIFICATIVA] Comando `batch pool upgrade os` removido</span><span class="sxs-lookup"><span data-stu-id="48988-917">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="48988-918">[ALTERAÇÃO SIGNIFICATIVA] Propriedade `Pacakges` removida das respostas `Application`</span><span class="sxs-lookup"><span data-stu-id="48988-918">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="48988-919">Comando `batch application package list` adicionado para listar os pacotes de um aplicativo</span><span class="sxs-lookup"><span data-stu-id="48988-919">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="48988-920">[ALTERAÇÃO SIGNIFICATIVA] `--application-id` alterado para `--application-name` em todos os comandos `batch application`,</span><span class="sxs-lookup"><span data-stu-id="48988-920">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="48988-921">O argumento `--json-file` foi adicionado aos comandos para a solicitação de resposta da API bruta</span><span class="sxs-lookup"><span data-stu-id="48988-921">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="48988-922">Validação atualizada para incluir automaticamente `https://` em todos os pontos de extremidade, se ausente</span><span class="sxs-lookup"><span data-stu-id="48988-922">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="48988-923">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="48988-923">CosmosDB</span></span>

* <span data-ttu-id="48988-924">O subgrupo `network-rule` foi adicionado com os comandos `add`, `remove` e `list` para gerenciar as regras de VNET de uma conta do Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="48988-924">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="48988-925">Kusto</span><span class="sxs-lookup"><span data-stu-id="48988-925">Kusto</span></span>

* <span data-ttu-id="48988-926">[ALTERAÇÃO SIGNIFICATIVA] Os tipos `hot_cache_period` e `soft_delete_period` foram alterados do banco de dados para o formato de duração ISO8601</span><span class="sxs-lookup"><span data-stu-id="48988-926">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="48988-927">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-927">Network</span></span>

* <span data-ttu-id="48988-928">Adicionado o argumento `--express-route-gateway-bypass` para `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48988-928">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="48988-929">Foram adicionados os grupos de comando a partir das extensões `express-route`</span><span class="sxs-lookup"><span data-stu-id="48988-929">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="48988-930">Os grupos de comando `express-route gateway` e `express-route port` foram adicionados</span><span class="sxs-lookup"><span data-stu-id="48988-930">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="48988-931">Adicionado o argumento `--legacy-mode` para `express-route peering [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48988-931">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="48988-932">Os argumentos `--allow-classic-operations` e `--express-route-port` foram adicionados a `express-route [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48988-932">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="48988-933">Adicionado o argumento `--gateway-default-site` para `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48988-933">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="48988-934">Os comandos `ipsec-policy` foram adicionados a `vnet-gateway`</span><span class="sxs-lookup"><span data-stu-id="48988-934">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="48988-935">Recurso</span><span class="sxs-lookup"><span data-stu-id="48988-935">Resource</span></span>

* <span data-ttu-id="48988-936">Foi corrigido o problema com `deployment create` em que o campo do tipo diferencia letras maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="48988-936">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="48988-937">Foi adicionado o suporte para arquivo de parâmetros de URI a `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="48988-937">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="48988-938">Foi adicionado o suporte para parâmetros de URI e definições a `policy set-definition update`</span><span class="sxs-lookup"><span data-stu-id="48988-938">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="48988-939">Foi corrigido o tratamento de parâmetros e regras para `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="48988-939">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="48988-940">Foi corrigido o problema com `resource show/update/delete/tag/invoke-action` em que as IDs de assinatura cruzada não respeitaram corretamente a ID da assinatura</span><span class="sxs-lookup"><span data-stu-id="48988-940">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="48988-941">Função</span><span class="sxs-lookup"><span data-stu-id="48988-941">Role</span></span>

* <span data-ttu-id="48988-942">Foi adicionado o suporte para as funções do aplicativo a `ad app [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48988-942">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="48988-943">VM</span><span class="sxs-lookup"><span data-stu-id="48988-943">VM</span></span>

* <span data-ttu-id="48988-944">Foi corrigido o problema com `vm create where ` – a rede acelerada não foi habilitada por padrão no Ubuntu 18.0</span><span class="sxs-lookup"><span data-stu-id="48988-944">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="48988-945">12 de fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="48988-945">February 12, 2019</span></span>

<span data-ttu-id="48988-946">Versão 2.0.58</span><span class="sxs-lookup"><span data-stu-id="48988-946">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="48988-947">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48988-947">Core</span></span>

* <span data-ttu-id="48988-948">`az --version` agora exibe uma notificação se você tiver pacotes para atualização</span><span class="sxs-lookup"><span data-stu-id="48988-948">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="48988-949">A regressão em que `--ids` não pode ser usado com a saída JSON foi corrigida</span><span class="sxs-lookup"><span data-stu-id="48988-949">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="48988-950">ACR</span><span class="sxs-lookup"><span data-stu-id="48988-950">ACR</span></span>
* <span data-ttu-id="48988-951">[ALTERAÇÃO SIGNIFICATIVA] O grupo de comandos `acr build-task` foi removido</span><span class="sxs-lookup"><span data-stu-id="48988-951">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="48988-952">[ALTERAÇÃO SIGNIFICATIVA] As opções `--tag` e `--manifest` de `acr repository delete` foram removidas</span><span class="sxs-lookup"><span data-stu-id="48988-952">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="48988-953">ACS</span><span class="sxs-lookup"><span data-stu-id="48988-953">ACS</span></span>
* <span data-ttu-id="48988-954">Suporte adicionado a `aks [enable-addons|disable-addons]` para nomes que não diferenciam maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="48988-954">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="48988-955">Suporte adicionado para a operação de atualização do Azure Active Directory usando `aks update-credentials --reset-aad`</span><span class="sxs-lookup"><span data-stu-id="48988-955">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="48988-956">Um esclarecimento informando que `--output` é ignorado para `aks get-credentials` foi adicionado</span><span class="sxs-lookup"><span data-stu-id="48988-956">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="48988-957">AMS</span><span class="sxs-lookup"><span data-stu-id="48988-957">AMS</span></span>
* <span data-ttu-id="48988-958">Adicionados os comandos `ams streaming-endpoint [start | stop | create | update] wait`</span><span class="sxs-lookup"><span data-stu-id="48988-958">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="48988-959">Adicionados os comandos `ams live-event [create | start | stop | reset] wait`</span><span class="sxs-lookup"><span data-stu-id="48988-959">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="48988-960">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-960">Appservice</span></span>
* <span data-ttu-id="48988-961">Foi adicionada a capacidade de criar e configurar funções usando contêineres de ACR</span><span class="sxs-lookup"><span data-stu-id="48988-961">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="48988-962">Suporte adicionado para a atualização das configurações de aplicativos Web por meio de JSON</span><span class="sxs-lookup"><span data-stu-id="48988-962">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="48988-963">A ajuda foi aprimorada para `appservice-plan-update`</span><span class="sxs-lookup"><span data-stu-id="48988-963">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="48988-964">Suporte adicionado para o App Insights para auxiliar na criação de aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="48988-964">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="48988-965">Os problemas com o SSH do aplicativo Web foram corrigidos</span><span class="sxs-lookup"><span data-stu-id="48988-965">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="48988-966">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="48988-966">Botservice</span></span>
* <span data-ttu-id="48988-967">A experiência do usuário para `bot publish` foi aprimorada</span><span class="sxs-lookup"><span data-stu-id="48988-967">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="48988-968">Foram adicionados avisos de tempos limite ao executar `npm install` durante `az bot publish`</span><span class="sxs-lookup"><span data-stu-id="48988-968">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="48988-969">O caractere inválido `.` de `--name` em `az bot create` foi removido</span><span class="sxs-lookup"><span data-stu-id="48988-969">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="48988-970">Alteração para interromper a geração aleatória de nomes de recursos durante a criação do Armazenamento do Azure, Plano do Serviço de Aplicativo, Aplicativo Web/de funções e Application Insights</span><span class="sxs-lookup"><span data-stu-id="48988-970">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="48988-971">[PRETERIDO] O argumento `--proj-name` foi preterido em favor de `--proj-file-path`</span><span class="sxs-lookup"><span data-stu-id="48988-971">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="48988-972">`az bot publish` foi alterado para remover arquivos de implantação do Node.js do IIS buscados, caso eles já não existissem</span><span class="sxs-lookup"><span data-stu-id="48988-972">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="48988-973">Foi adicionado o argumento `--keep-node-modules` para `az bot publish` para não excluir a pasta `node_modules` no Serviço de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="48988-973">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="48988-974">O par chave-valor `"publishCommand"` foi adicionado à saída de `az bot create` durante a criação de uma função do Azure ou bot de aplicativo Web</span><span class="sxs-lookup"><span data-stu-id="48988-974">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="48988-975">O valor de `"publishCommand"` é um comando `az bot publish` que é automaticamente preenchido com os parâmetros necessários para publicar o bot recém-criado</span><span class="sxs-lookup"><span data-stu-id="48988-975">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="48988-976">O `"WEBSITE_NODE_DEFAULT_VERSION"` foi atualizado no modelo do ARM para que os bots de SDK v4 usem 10.14.1 em vez de 8.9.4</span><span class="sxs-lookup"><span data-stu-id="48988-976">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="48988-977">Key Vault</span><span class="sxs-lookup"><span data-stu-id="48988-977">Key Vault</span></span>
* <span data-ttu-id="48988-978">Foi corrigido o problema com `keyvault secret backup`, em que alguns usuários recebiam um erro `unexpected_keyword` ao usar `--id`</span><span class="sxs-lookup"><span data-stu-id="48988-978">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="48988-979">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="48988-979">Monitor</span></span>
* <span data-ttu-id="48988-980">`monitor metrics alert [create|update]` foi alterado para permitir o valor dimensional `*`</span><span class="sxs-lookup"><span data-stu-id="48988-980">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="48988-981">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-981">Network</span></span>
* <span data-ttu-id="48988-982">`dns zone export` foi alterado para garantir que CNAMEs exportados fossem FQDNs</span><span class="sxs-lookup"><span data-stu-id="48988-982">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="48988-983">O parâmetro `--gateway-name` foi adicionado a `nic ip-config address-pool [add|remove]` para dar suporte a pools de endereços de back-end de gateway de aplicativo</span><span class="sxs-lookup"><span data-stu-id="48988-983">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="48988-984">Os argumentos `--traffic-analytics` e `--workspace` foram adicionados a `network watcher flow-log configure` para dar suporte à análise de tráfego por meio de um espaço de trabalho do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="48988-984">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="48988-985">`--idle-timeout` e `--floating-ip` foram adicionados a `lb inbound-nat-pool [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48988-985">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="48988-986">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="48988-986">Policy Insights</span></span>
* <span data-ttu-id="48988-987">Os comandos `policy remediation` foram adicionados para dar suporte a recursos de correção de política de recursos</span><span class="sxs-lookup"><span data-stu-id="48988-987">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="48988-988">RDBMS</span><span class="sxs-lookup"><span data-stu-id="48988-988">RDBMS</span></span>
* <span data-ttu-id="48988-989">A mensagem e os parâmetros de comando de ajuda foram aprimorados</span><span class="sxs-lookup"><span data-stu-id="48988-989">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="48988-990">Redis</span><span class="sxs-lookup"><span data-stu-id="48988-990">Redis</span></span>
* <span data-ttu-id="48988-991">Foram adicionados comandos para gerenciar regras de firewall (criar, atualizar, excluir, mostrar, listar)</span><span class="sxs-lookup"><span data-stu-id="48988-991">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="48988-992">Foram adicionados comandos para gerenciar links do servidor (criar, excluir, mostrar, listar)</span><span class="sxs-lookup"><span data-stu-id="48988-992">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="48988-993">Foram adicionados comandos para gerenciar o agendamento de patches (criar, atualizar, excluir, mostrar)</span><span class="sxs-lookup"><span data-stu-id="48988-993">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="48988-994">Suporte adicionado para Zonas de Disponibilidade e versão mínima de TLS para criar Redis</span><span class="sxs-lookup"><span data-stu-id="48988-994">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="48988-995">[ALTERAÇÃO SIGNIFICATIVA] Os comandos `redis update-settings` e `redis list-all` foram removidos</span><span class="sxs-lookup"><span data-stu-id="48988-995">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="48988-996">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro para `redis create`: “configurações de locatário” não é aceito no formato chave[=valor]</span><span class="sxs-lookup"><span data-stu-id="48988-996">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="48988-997">[PRETERIDO] Uma mensagem de aviso foi adicionada para preterir o comando `redis import-method`</span><span class="sxs-lookup"><span data-stu-id="48988-997">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="48988-998">Função</span><span class="sxs-lookup"><span data-stu-id="48988-998">Role</span></span>
* <span data-ttu-id="48988-999">[ALTERAÇÃO SIGNIFICATIVA] O comando `az identity` foi movido dos comandos `vm` para esta localização</span><span class="sxs-lookup"><span data-stu-id="48988-999">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="48988-1000">SQL VM</span><span class="sxs-lookup"><span data-stu-id="48988-1000">SQL VM</span></span>
* <span data-ttu-id="48988-1001">[PRETERIDO] O argumento `--boostrap-acc-pwd` foi preterido devido a um erro de digitação</span><span class="sxs-lookup"><span data-stu-id="48988-1001">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="48988-1002">VM</span><span class="sxs-lookup"><span data-stu-id="48988-1002">VM</span></span>
* <span data-ttu-id="48988-1003">`vm list-skus` foi alterado para permitir o uso de `--all` no lugar de `--all true`</span><span class="sxs-lookup"><span data-stu-id="48988-1003">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="48988-1004">Adicionado `vmss run-command [invoke | list | show]`</span><span class="sxs-lookup"><span data-stu-id="48988-1004">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="48988-1005">Foi corrigido o bug em que `vmss encryption enable` falhava se fosse executado anteriormente</span><span class="sxs-lookup"><span data-stu-id="48988-1005">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="48988-1006">[ALTERAÇÃO SIGNIFICATIVA] O comando `az identity` foi movido para os comandos `role`</span><span class="sxs-lookup"><span data-stu-id="48988-1006">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="48988-1007">31 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="48988-1007">January 31, 2019</span></span>

<span data-ttu-id="48988-1008">Versão 2.0.57</span><span class="sxs-lookup"><span data-stu-id="48988-1008">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="48988-1009">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48988-1009">Core</span></span>

* <span data-ttu-id="48988-1010">Hotfix para o [problema 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="48988-1010">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="48988-1011">28 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="48988-1011">January 28, 2019</span></span>

<span data-ttu-id="48988-1012">Versão 2.0.56</span><span class="sxs-lookup"><span data-stu-id="48988-1012">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="48988-1013">ACR</span><span class="sxs-lookup"><span data-stu-id="48988-1013">ACR</span></span>
* <span data-ttu-id="48988-1014">Suporte adicionado para regras de rede virtual/IP</span><span class="sxs-lookup"><span data-stu-id="48988-1014">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="48988-1015">ACS</span><span class="sxs-lookup"><span data-stu-id="48988-1015">ACS</span></span>
* <span data-ttu-id="48988-1016">Adicionada visualização dos nós virtuais</span><span class="sxs-lookup"><span data-stu-id="48988-1016">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="48988-1017">Comandos do OpenShift gerenciado foram adicionados</span><span class="sxs-lookup"><span data-stu-id="48988-1017">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="48988-1018">Suporte adicionado para operações de atualização da entidade de serviço com `aks update-credentials -reset-service-principal`</span><span class="sxs-lookup"><span data-stu-id="48988-1018">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="48988-1019">AMS</span><span class="sxs-lookup"><span data-stu-id="48988-1019">AMS</span></span>
* <span data-ttu-id="48988-1020">[ALTERAÇÃO SIGNIFICATIVA] `ams asset get-streaming-locators` renomeado para `ams asset list-streaming-locators`</span><span class="sxs-lookup"><span data-stu-id="48988-1020">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="48988-1021">[ALTERAÇÃO SIGNIFICATIVA] `ams streaming-locator get-content-keys` renomeado para `ams streaming-locator list-content-keys`</span><span class="sxs-lookup"><span data-stu-id="48988-1021">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="48988-1022">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-1022">Appservice</span></span>
* <span data-ttu-id="48988-1023">Suporte adicionado para o App Insights no `functionapp create`</span><span class="sxs-lookup"><span data-stu-id="48988-1023">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="48988-1024">Suporte adicionado para a criação do plano de serviço de aplicativo (incluindo Elástico Premium) para Aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="48988-1024">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="48988-1025">Foram corrigidos os problemas com de configuração de aplicativo com os planos Elástico Premium</span><span class="sxs-lookup"><span data-stu-id="48988-1025">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="48988-1026">Contêiner</span><span class="sxs-lookup"><span data-stu-id="48988-1026">Container</span></span>
* <span data-ttu-id="48988-1027">Adicionado o comando `container start`</span><span class="sxs-lookup"><span data-stu-id="48988-1027">Added `container start` command</span></span>
* <span data-ttu-id="48988-1028">Alteração para permitir o uso de valores decimais para CPU durante a criação do contêiner</span><span class="sxs-lookup"><span data-stu-id="48988-1028">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="48988-1029">EventGrid</span><span class="sxs-lookup"><span data-stu-id="48988-1029">EventGrid</span></span>
* <span data-ttu-id="48988-1030">Parâmetro `--deadletter-endpoint` adicionado a `event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48988-1030">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="48988-1031">Storagequeue e hybridconnection foram adicionados como novos valores para 'event-subscription [create|update] --endpoint-type\`</span><span class="sxs-lookup"><span data-stu-id="48988-1031">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="48988-1032">Os parâmetros `--max-delivery-attempts` e `--event-ttl` foram adicionados a `event-subscription create` para especificar a política de repetição para eventos</span><span class="sxs-lookup"><span data-stu-id="48988-1032">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="48988-1033">Uma mensagem de aviso foi adicionada a `event-subscription [create|update]` quando o webhook como destino for usado para uma assinatura de evento</span><span class="sxs-lookup"><span data-stu-id="48988-1033">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="48988-1034">O parâmetro source-resource-id foi adicionado para todos os comandos relacionados a eventos e marcar todos os outros parâmetros relacionados ao recurso de origem como preteridos</span><span class="sxs-lookup"><span data-stu-id="48988-1034">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="48988-1035">HDInsight</span><span class="sxs-lookup"><span data-stu-id="48988-1035">HDInsight</span></span>
* <span data-ttu-id="48988-1036">[ALTERAÇÃO SIGNIFICATIVA] Os parâmetros `--virtual-network` e `--subnet-name` de `hdinsight [application] create` foram removidos</span><span class="sxs-lookup"><span data-stu-id="48988-1036">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="48988-1037">[ALTERAÇÃO SIGNIFICATIVA] `hdinsight create --storage-account` foi alterado para aceitar o nome ou ID da conta de armazenamento, em vez de pontos de extremidade de blob</span><span class="sxs-lookup"><span data-stu-id="48988-1037">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="48988-1038">Parâmetros `--vnet-name` e `--subnet-name` adicionados a `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="48988-1038">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="48988-1039">Suporte adicionado para a criptografia de disco e Enterprise Security Package ao `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="48988-1039">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="48988-1040">Adicionado o comando `hdinsight rotate-disk-encryption-key`</span><span class="sxs-lookup"><span data-stu-id="48988-1040">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="48988-1041">Adicionado o comando `hdinsight update`</span><span class="sxs-lookup"><span data-stu-id="48988-1041">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="48988-1042">IoT</span><span class="sxs-lookup"><span data-stu-id="48988-1042">IoT</span></span>
* <span data-ttu-id="48988-1043">O formato de codificação foi adicionado ao comando routing-endpoint</span><span class="sxs-lookup"><span data-stu-id="48988-1043">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="48988-1044">Kusto</span><span class="sxs-lookup"><span data-stu-id="48988-1044">Kusto</span></span>
* <span data-ttu-id="48988-1045">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="48988-1045">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="48988-1046">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="48988-1046">Monitor</span></span>
* <span data-ttu-id="48988-1047">A comparação de ID foi alterada para diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="48988-1047">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="48988-1048">Perfil</span><span class="sxs-lookup"><span data-stu-id="48988-1048">Profile</span></span>
* <span data-ttu-id="48988-1049">A conta de nível de locatário foi habilitada para a identidade de serviço gerenciada de `login`</span><span class="sxs-lookup"><span data-stu-id="48988-1049">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="48988-1050">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-1050">Network</span></span>
* <span data-ttu-id="48988-1051">Foi corrigido o problema com `express-route update`: em que o argumento `--bandwidth` era ignorado</span><span class="sxs-lookup"><span data-stu-id="48988-1051">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="48988-1052">Foi corrigido o problema com `ddos-protection update` em que definir a compreensão levava ao rastreamento de pilha</span><span class="sxs-lookup"><span data-stu-id="48988-1052">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="48988-1053">Recurso</span><span class="sxs-lookup"><span data-stu-id="48988-1053">Resource</span></span>
* <span data-ttu-id="48988-1054">Suporte adicionado para o arquivo de parâmetros de URI à `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="48988-1054">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="48988-1055">Suporte adicionado para a identidade gerenciada à `policy assignment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="48988-1055">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="48988-1056">Máquina virtual SQL</span><span class="sxs-lookup"><span data-stu-id="48988-1056">SQL Virtual Machine</span></span>
* <span data-ttu-id="48988-1057">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="48988-1057">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="48988-1058">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48988-1058">Storage</span></span>
* <span data-ttu-id="48988-1059">Alteração na correção para atualizar apenas as propriedades que são alteradas no mesmo objeto</span><span class="sxs-lookup"><span data-stu-id="48988-1059">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="48988-1060">#8021 foi corrigido, dados binários são codificados em base 64 quando retornados</span><span class="sxs-lookup"><span data-stu-id="48988-1060">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="48988-1061">VM</span><span class="sxs-lookup"><span data-stu-id="48988-1061">VM</span></span>
* <span data-ttu-id="48988-1062">Alteração de `vm encryption enable` para validar o cofre de chaves de criptografia de disco e se esse cofre de chaves de criptografia de chave existe</span><span class="sxs-lookup"><span data-stu-id="48988-1062">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="48988-1063">O sinalizador `--force` foi adicionado a `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="48988-1063">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="48988-1064">15 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="48988-1064">January 15, 2019</span></span>

<span data-ttu-id="48988-1065">Versão 2.0.55</span><span class="sxs-lookup"><span data-stu-id="48988-1065">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="48988-1066">ACR</span><span class="sxs-lookup"><span data-stu-id="48988-1066">ACR</span></span>
* <span data-ttu-id="48988-1067">Alteração para permitir forçar o envio por push de um gráfico Helm que não existe</span><span class="sxs-lookup"><span data-stu-id="48988-1067">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="48988-1068">Alteração para permitir operações de runtime sem solicitações ARM</span><span class="sxs-lookup"><span data-stu-id="48988-1068">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="48988-1069">[PRETERIDO] O parâmetro `--resource-group` foi preterido nos comandos:</span><span class="sxs-lookup"><span data-stu-id="48988-1069">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="48988-1070">ACS</span><span class="sxs-lookup"><span data-stu-id="48988-1070">ACS</span></span>
* <span data-ttu-id="48988-1071">Suporte adicionado para novas regiões ACI</span><span class="sxs-lookup"><span data-stu-id="48988-1071">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="48988-1072">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-1072">Appservice</span></span>
* <span data-ttu-id="48988-1073">Foi corrigido o problema com o carregamento de certificados para aplicativos que são hospedados em um ASE, em que o RG do ASE e o RG do aplicativo são diferentes</span><span class="sxs-lookup"><span data-stu-id="48988-1073">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="48988-1074">Alteração de `webapp up` para usar a SKU P1V1 como padrão para Linux</span><span class="sxs-lookup"><span data-stu-id="48988-1074">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="48988-1075">`[webapp|functionapp] deployment source config-zip` foi corrigido para mostrar a mensagem de erro adequada quando uma implantação falhar</span><span class="sxs-lookup"><span data-stu-id="48988-1075">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="48988-1076">Adicionado o comando `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="48988-1076">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="48988-1077">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="48988-1077">Botservice</span></span>
* <span data-ttu-id="48988-1078">Atualizações de status de implantação foram adicionadas a `bot create`</span><span class="sxs-lookup"><span data-stu-id="48988-1078">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="48988-1079">Configurar</span><span class="sxs-lookup"><span data-stu-id="48988-1079">Configure</span></span>
* <span data-ttu-id="48988-1080">`none` foi adicionado como um formato de saída configurável</span><span class="sxs-lookup"><span data-stu-id="48988-1080">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="48988-1081">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="48988-1081">CosmosDB</span></span>
* <span data-ttu-id="48988-1082">Suporte adicionado para criar o banco de dados com taxa de transferência compartilhada</span><span class="sxs-lookup"><span data-stu-id="48988-1082">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="48988-1083">HDInsight</span><span class="sxs-lookup"><span data-stu-id="48988-1083">HDInsight</span></span>
* <span data-ttu-id="48988-1084">Foram adicionados comandos para o gerenciamento de aplicativos</span><span class="sxs-lookup"><span data-stu-id="48988-1084">Added commands for managing applications</span></span>
* <span data-ttu-id="48988-1085">Foram adicionados comandos para o gerenciamento de ações de script</span><span class="sxs-lookup"><span data-stu-id="48988-1085">Added commands for managing script actions</span></span>
* <span data-ttu-id="48988-1086">Foram adicionados comandos para o gerenciamento do Operations Management Suite (OMS)</span><span class="sxs-lookup"><span data-stu-id="48988-1086">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="48988-1087">Suporte adicionado para listar a utilização regional ao `hdinsight list-usage`</span><span class="sxs-lookup"><span data-stu-id="48988-1087">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="48988-1088">[ALTERAÇÃO SIGNIFICATIVA] O tipo de cluster padrão de `hdinsight create` foi removido</span><span class="sxs-lookup"><span data-stu-id="48988-1088">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="48988-1089">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-1089">Network</span></span>
* <span data-ttu-id="48988-1090">Adicionados os argumentos `--custom-headers` e `--status-code-ranges` para `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48988-1090">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="48988-1091">Novos tipos de roteamento foram adicionados: Subrede e múltiplos valores</span><span class="sxs-lookup"><span data-stu-id="48988-1091">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="48988-1092">Adicionados os argumentos `--custom-headers` e `--subnets` para `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48988-1092">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="48988-1093">Foi corrigido o problema no qual fornecer `--vnets ""` a `ddos-protection update` causava um erro</span><span class="sxs-lookup"><span data-stu-id="48988-1093">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="48988-1094">Função</span><span class="sxs-lookup"><span data-stu-id="48988-1094">Role</span></span>
* <span data-ttu-id="48988-1095">[PRETERIDO] O argumento `--password` foi preterido para `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="48988-1095">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="48988-1096">Como alternativa, use senhas seguras geradas pela CLI</span><span class="sxs-lookup"><span data-stu-id="48988-1096">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="48988-1097">Segurança</span><span class="sxs-lookup"><span data-stu-id="48988-1097">Security</span></span>
* <span data-ttu-id="48988-1098">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="48988-1098">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="48988-1099">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48988-1099">Storage</span></span>
* <span data-ttu-id="48988-1100">[ALTERAÇÃO SIGNIFICATIVA] O número padrão de resultados de `storage [blob|file|container|share] list` foi alterado para 5.000.</span><span class="sxs-lookup"><span data-stu-id="48988-1100">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="48988-1101">Use `--num-results *` para o comportamento original de retornar todos os resultados</span><span class="sxs-lookup"><span data-stu-id="48988-1101">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="48988-1102">Parâmetro `--marker` adicionado a `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="48988-1102">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="48988-1103">Um marcador de log foi adicionado para a próxima página ao STDERR de `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="48988-1103">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="48988-1104">O comando `storage blob service-properties update` foi adicionado com suporte para sites estáticos</span><span class="sxs-lookup"><span data-stu-id="48988-1104">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="48988-1105">VM</span><span class="sxs-lookup"><span data-stu-id="48988-1105">VM</span></span>
* <span data-ttu-id="48988-1106">`vm [disk|unmanaged-disk]` e `vmss disk` foram alterados para que tenham parâmetros mais consistentes</span><span class="sxs-lookup"><span data-stu-id="48988-1106">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="48988-1107">Suporte adicionado para referência cruzada de imagem de locatário a `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="48988-1107">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="48988-1108">O bug de configuração padrão foi corrigido em `vm diagnostics get-default-config --windows-os`</span><span class="sxs-lookup"><span data-stu-id="48988-1108">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="48988-1109">O argumento `--provision-after-extensions` foi adicionado a `vmss extension set` para definir quais extensões deverão ser provisionadas antes da extensão ser definida</span><span class="sxs-lookup"><span data-stu-id="48988-1109">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="48988-1110">O argumento `--replica-count` foi adicionado a `sig image-version update` para definir a contagem de replicação padrão</span><span class="sxs-lookup"><span data-stu-id="48988-1110">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="48988-1111">Foi corrigido o bug com `image create --source` em que o disco do sistema operacional de origem era confundido com uma VM do mesmo nome, mesmo se a ID de recurso completa fosse fornecida</span><span class="sxs-lookup"><span data-stu-id="48988-1111">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="48988-1112">20 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="48988-1112">December 20, 2018</span></span>

<span data-ttu-id="48988-1113">Versão 2.0.54</span><span class="sxs-lookup"><span data-stu-id="48988-1113">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="48988-1114">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-1114">Appservice</span></span>
* <span data-ttu-id="48988-1115">Corrigido o problema que causava falha na reimplantação do `webapp up`</span><span class="sxs-lookup"><span data-stu-id="48988-1115">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="48988-1116">Adicionado suporte para listar e restaurar instantâneos de aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="48988-1116">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="48988-1117">Adicionado suporte para o sinalizador `--runtime` para aplicativos de funções do Windows</span><span class="sxs-lookup"><span data-stu-id="48988-1117">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="48988-1118">IoT Central</span><span class="sxs-lookup"><span data-stu-id="48988-1118">IoTCentral</span></span>
* <span data-ttu-id="48988-1119">Corrigida a chamada à API do comando de atualização</span><span class="sxs-lookup"><span data-stu-id="48988-1119">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="48988-1120">Função</span><span class="sxs-lookup"><span data-stu-id="48988-1120">Role</span></span>
* <span data-ttu-id="48988-1121">[ALTERAÇÃO SIGNIFICATIVA] `ad [app|sp] list` alterado para listar somente os 100 primeiros objetos por padrão</span><span class="sxs-lookup"><span data-stu-id="48988-1121">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="48988-1122">SQL</span><span class="sxs-lookup"><span data-stu-id="48988-1122">SQL</span></span>
* <span data-ttu-id="48988-1123">Adicionado suporte para ordenação personalizada nas instâncias gerenciadas</span><span class="sxs-lookup"><span data-stu-id="48988-1123">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="48988-1124">VM</span><span class="sxs-lookup"><span data-stu-id="48988-1124">VM</span></span>
* <span data-ttu-id="48988-1125">Parâmetro `---os-type` adicionado a `disk create`</span><span class="sxs-lookup"><span data-stu-id="48988-1125">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="48988-1126">18 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="48988-1126">December 18, 2018</span></span>

<span data-ttu-id="48988-1127">Versão 2.0.53</span><span class="sxs-lookup"><span data-stu-id="48988-1127">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="48988-1128">ACR</span><span class="sxs-lookup"><span data-stu-id="48988-1128">ACR</span></span>
* <span data-ttu-id="48988-1129">Adicionado suporte para importação de imagem de Registros de Contêiner externos</span><span class="sxs-lookup"><span data-stu-id="48988-1129">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="48988-1130">Simplificado o layout da tabela para a lista de tarefas</span><span class="sxs-lookup"><span data-stu-id="48988-1130">Condensed the table layout for task list</span></span>
* <span data-ttu-id="48988-1131">Adicionado suporte para URLs do Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="48988-1131">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="48988-1132">ACS</span><span class="sxs-lookup"><span data-stu-id="48988-1132">ACS</span></span>
* <span data-ttu-id="48988-1133">Adicionada visualização dos nós virtuais</span><span class="sxs-lookup"><span data-stu-id="48988-1133">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="48988-1134">Removido “(VISUALIZAÇÃO)” de argumentos do AAD para `aks create`</span><span class="sxs-lookup"><span data-stu-id="48988-1134">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="48988-1135">[PRETERIDO] Comandos `az acs` preteridos.</span><span class="sxs-lookup"><span data-stu-id="48988-1135">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="48988-1136">O serviço ACS será desativado em 31 de janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="48988-1136">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="48988-1137">Adicionado suporte da Política de Rede durante a criação de novos clusters AKS</span><span class="sxs-lookup"><span data-stu-id="48988-1137">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="48988-1138">Removido o requisito do argumento `--nodepool-name` para `aks scale` se houver apenas um pool de nós</span><span class="sxs-lookup"><span data-stu-id="48988-1138">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="48988-1139">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-1139">Appservice</span></span>
* <span data-ttu-id="48988-1140">Corrigido o problema em que `webapp config container` não honra o parâmetro `--slot`</span><span class="sxs-lookup"><span data-stu-id="48988-1140">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="48988-1141">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="48988-1141">Botservice</span></span>
* <span data-ttu-id="48988-1142">Suporte adicionado para análise do arquivo `.bot` ao chamar `bot show`</span><span class="sxs-lookup"><span data-stu-id="48988-1142">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="48988-1143">Corrigido o bug de provisionamento do AppInsights</span><span class="sxs-lookup"><span data-stu-id="48988-1143">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="48988-1144">Corrigido o bug de espaço em branco ao lidar com caminhos de arquivo</span><span class="sxs-lookup"><span data-stu-id="48988-1144">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="48988-1145">Reduzidas as chamadas de rede do Kudu</span><span class="sxs-lookup"><span data-stu-id="48988-1145">Reduced Kudu network calls</span></span>
* <span data-ttu-id="48988-1146">Melhorias de UX para comandos gerais</span><span class="sxs-lookup"><span data-stu-id="48988-1146">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="48988-1147">Consumo</span><span class="sxs-lookup"><span data-stu-id="48988-1147">Consumption</span></span>
* <span data-ttu-id="48988-1148">Corrigidos os bugs da API de orçamento ao mostrar notificações</span><span class="sxs-lookup"><span data-stu-id="48988-1148">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="48988-1149">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="48988-1149">CosmosDB</span></span>
* <span data-ttu-id="48988-1150">Suporte adicionado para atualizar a conta de vários mestres para mestre único</span><span class="sxs-lookup"><span data-stu-id="48988-1150">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="48988-1151">Mapas</span><span class="sxs-lookup"><span data-stu-id="48988-1151">Maps</span></span>
* <span data-ttu-id="48988-1152">Adicionado suporte ao SKU S1 para `maps account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48988-1152">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="48988-1153">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-1153">Network</span></span>
* <span data-ttu-id="48988-1154">Adicionado suporte para `--format` e `--log-version` para `watcher flow-log configure`</span><span class="sxs-lookup"><span data-stu-id="48988-1154">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="48988-1155">Corrigido o problema com `dns zone update` em que usar "" para limpar a resolução e o registro de redes virtuais não funcionava</span><span class="sxs-lookup"><span data-stu-id="48988-1155">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="48988-1156">Recurso</span><span class="sxs-lookup"><span data-stu-id="48988-1156">Resource</span></span>
* <span data-ttu-id="48988-1157">Corrigido o tratamento do parâmetro de escopo para grupos de gerenciamento do `policy assignment [create|list|delete|show|update]`</span><span class="sxs-lookup"><span data-stu-id="48988-1157">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="48988-1158">Adicionado o novo comando `resource wait`</span><span class="sxs-lookup"><span data-stu-id="48988-1158">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="48988-1159">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48988-1159">Storage</span></span>
*  <span data-ttu-id="48988-1160">Adicionada a capacidade de atualizar a versão do esquema de log para serviços de armazenamento no `storage logging update`</span><span class="sxs-lookup"><span data-stu-id="48988-1160">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="48988-1161">VM</span><span class="sxs-lookup"><span data-stu-id="48988-1161">VM</span></span>
* <span data-ttu-id="48988-1162">Corrigida a falha em `vm identity remove` quando a VM especificada não tem nenhuma identidade de serviço gerenciado atribuída</span><span class="sxs-lookup"><span data-stu-id="48988-1162">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="48988-1163">4 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="48988-1163">December 4, 2018</span></span>

<span data-ttu-id="48988-1164">Versão 2.0.52</span><span class="sxs-lookup"><span data-stu-id="48988-1164">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="48988-1165">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48988-1165">Core</span></span>
* <span data-ttu-id="48988-1166">Adicionado suporte para provisionamento de recursos de locatários cruzados para a entidade de serviço de multilocatários</span><span class="sxs-lookup"><span data-stu-id="48988-1166">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="48988-1167">Corrigido o bug onde as ids enviadas por pipe de um comando com a saída tsv eram analisados incorretamente</span><span class="sxs-lookup"><span data-stu-id="48988-1167">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="48988-1168">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-1168">Appservice</span></span>
* <span data-ttu-id="48988-1169">[VERSÃO PRÉVIA] Adicionado o comando `webapp up` que ajuda a criar e implantar conteúdo em aplicativo</span><span class="sxs-lookup"><span data-stu-id="48988-1169">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="48988-1170">Corrigido um bug no aplicativo com base em contêiner do Windows devido à alteração de back-end</span><span class="sxs-lookup"><span data-stu-id="48988-1170">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="48988-1171">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-1171">Network</span></span>
* <span data-ttu-id="48988-1172">Adicionado o argumento `--exclusion` a `application-gateway waf-config set` para dar suporte a exclusões de WAF</span><span class="sxs-lookup"><span data-stu-id="48988-1172">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="48988-1173">Função</span><span class="sxs-lookup"><span data-stu-id="48988-1173">Role</span></span>
* <span data-ttu-id="48988-1174">Adicionado suporte para identificadores personalizados para a credencial de senha</span><span class="sxs-lookup"><span data-stu-id="48988-1174">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="48988-1175">VM</span><span class="sxs-lookup"><span data-stu-id="48988-1175">VM</span></span>
* <span data-ttu-id="48988-1176">[PRETERIDO] Parâmetro `vm extension [show|wait] --expand` preterido</span><span class="sxs-lookup"><span data-stu-id="48988-1176">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="48988-1177">Adicionado parâmetro `--force` a `vm restart` para reimplantar as VMs sem resposta</span><span class="sxs-lookup"><span data-stu-id="48988-1177">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="48988-1178">Alterado `[vm|vmss] create --authentication-type` para aceitar "todos" para criar uma VM com senha e autenticação SSH</span><span class="sxs-lookup"><span data-stu-id="48988-1178">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="48988-1179">Adicionado parâmetro `image create --os-disk-caching` para definir o cache de disco do sistema operacional para uma imagem</span><span class="sxs-lookup"><span data-stu-id="48988-1179">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="48988-1180">20 de novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="48988-1180">November 20, 2018</span></span>

<span data-ttu-id="48988-1181">Versão 2.0.51</span><span class="sxs-lookup"><span data-stu-id="48988-1181">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="48988-1182">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48988-1182">Core</span></span>
* <span data-ttu-id="48988-1183">Logon do MSI alterado para não reutilizar o nome da assinatura na identidade</span><span class="sxs-lookup"><span data-stu-id="48988-1183">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="48988-1184">ACR</span><span class="sxs-lookup"><span data-stu-id="48988-1184">ACR</span></span>
* <span data-ttu-id="48988-1185">Token de contexto adicionado à etapa da tarefa</span><span class="sxs-lookup"><span data-stu-id="48988-1185">Added context token to task step</span></span>
* <span data-ttu-id="48988-1186">Suporte adicionado para definir segredos na execução do acr para espelhar a tarefa do acr</span><span class="sxs-lookup"><span data-stu-id="48988-1186">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="48988-1187">Suporte aprimorado para `--top` e `--orderby` para os comandos `show-tags` e `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="48988-1187">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="48988-1188">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-1188">Appservice</span></span>
* <span data-ttu-id="48988-1189">Tempo limite padrão para a implantação do zip alterado para sondar o status aumentado para 5 minutos, também adicionando uma propriedade de tempo limite para personalizar esse valor</span><span class="sxs-lookup"><span data-stu-id="48988-1189">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="48988-1190">Padrão `node_version` atualizado.</span><span class="sxs-lookup"><span data-stu-id="48988-1190">Updated the default `node_version`.</span></span> <span data-ttu-id="48988-1191">Redefinir a ação de troca de slots durante uma troca de duas fases preserva todas as configurações do aplicativo e cadeias de conexão</span><span class="sxs-lookup"><span data-stu-id="48988-1191">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="48988-1192">Verificação da SKU no lado do cliente removida para o Linux criar o plano do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="48988-1192">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="48988-1193">Erro corrigido ao tentar obter o status de implantação do zip</span><span class="sxs-lookup"><span data-stu-id="48988-1193">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="48988-1194">Iot Central</span><span class="sxs-lookup"><span data-stu-id="48988-1194">IotCentral</span></span>
* <span data-ttu-id="48988-1195">Verificação de disponibilidade do subdomínio adicionada ao criar um aplicativo do IoT Central</span><span class="sxs-lookup"><span data-stu-id="48988-1195">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="48988-1196">KeyVault</span><span class="sxs-lookup"><span data-stu-id="48988-1196">KeyVault</span></span>
* <span data-ttu-id="48988-1197">Bug corrigido em que os erros podem ter sido ignorados</span><span class="sxs-lookup"><span data-stu-id="48988-1197">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="48988-1198">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-1198">Network</span></span>
* <span data-ttu-id="48988-1199">Subcomandos `root-cert` adicionados a `application-gateway` para lidar com os certificados de raiz confiável</span><span class="sxs-lookup"><span data-stu-id="48988-1199">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="48988-1200">Opções `--min-capacity` e `--custom-error-pages` adicionadas a `application-gateway [create|update]`:</span><span class="sxs-lookup"><span data-stu-id="48988-1200">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="48988-1201">`--zones` adicionado para suporte da zona de disponibilidade a `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="48988-1201">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="48988-1202">Argumentos `--file-upload-limit`, `--max-request-body-size` e `--request-body-check` a `application-gateway waf-config set` adicionados</span><span class="sxs-lookup"><span data-stu-id="48988-1202">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="48988-1203">Rdbms</span><span class="sxs-lookup"><span data-stu-id="48988-1203">Rdbms</span></span>
* <span data-ttu-id="48988-1204">Comandos vnet do mariadb adicionados</span><span class="sxs-lookup"><span data-stu-id="48988-1204">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="48988-1205">Rbac</span><span class="sxs-lookup"><span data-stu-id="48988-1205">Rbac</span></span>
* <span data-ttu-id="48988-1206">Um problema corrigido ao tentar atualizar credenciais inalteradas em `ad app update`</span><span class="sxs-lookup"><span data-stu-id="48988-1206">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="48988-1207">Avisos de saída adicionados para comunicar alterações de falha em um futuro próximo para `ad [app|sp] list`</span><span class="sxs-lookup"><span data-stu-id="48988-1207">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="48988-1208">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48988-1208">Storage</span></span>
* <span data-ttu-id="48988-1209">Melhor manipulação de casos incomuns para os comandos da cópia de armazenamento</span><span class="sxs-lookup"><span data-stu-id="48988-1209">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="48988-1210">Corrigido o problema em que `storage blob copy start-batch` não usava credenciais de logon quando as contas de origem e destino eram iguais</span><span class="sxs-lookup"><span data-stu-id="48988-1210">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="48988-1211">Bug corrigido com `storage [blob|file] url` em que `sas_token` não foi incorporado na URL</span><span class="sxs-lookup"><span data-stu-id="48988-1211">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="48988-1212">Aviso de alteração da falha adicionado a `[blob|container] list`: produzirá apenas os primeiros 5.000 resultados por padrão</span><span class="sxs-lookup"><span data-stu-id="48988-1212">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="48988-1213">VM</span><span class="sxs-lookup"><span data-stu-id="48988-1213">VM</span></span>
* <span data-ttu-id="48988-1214">Suporte adicionado a `[vm|vmss] create --storage-sku` para especificar a SKU da conta de armazenamento para o SO gerenciado e os discos de dados separadamente</span><span class="sxs-lookup"><span data-stu-id="48988-1214">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="48988-1215">Parâmetros do nome da versão alterados de `sig image-version` para `--image-version -e`</span><span class="sxs-lookup"><span data-stu-id="48988-1215">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="48988-1216">Argumento `sig image-version` preterido `--image-version-name`, substituído por `--image-version`</span><span class="sxs-lookup"><span data-stu-id="48988-1216">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="48988-1217">Suporte adicionado para usar o disco local do SO a `[vm|vmss] create --ephemeral-os-disk`</span><span class="sxs-lookup"><span data-stu-id="48988-1217">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="48988-1218">Adicionado o suporte ao `--no-wait` para `snapshot create/update`</span><span class="sxs-lookup"><span data-stu-id="48988-1218">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="48988-1219">Adicionado o comando `snapshot wait`</span><span class="sxs-lookup"><span data-stu-id="48988-1219">Added `snapshot wait` command</span></span>
* <span data-ttu-id="48988-1220">Suporte adicionado para usar o nome da instância com `[vm|vmss] extension set --extension-instance-name`</span><span class="sxs-lookup"><span data-stu-id="48988-1220">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="48988-1221">6 de novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="48988-1221">November 6, 2018</span></span>

<span data-ttu-id="48988-1222">Versão 2.0.50</span><span class="sxs-lookup"><span data-stu-id="48988-1222">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="48988-1223">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48988-1223">Core</span></span>
* <span data-ttu-id="48988-1224">Foi adicionado suporte para o serviço principal sn + autenticação do emissor</span><span class="sxs-lookup"><span data-stu-id="48988-1224">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="48988-1225">ACR</span><span class="sxs-lookup"><span data-stu-id="48988-1225">ACR</span></span>
* <span data-ttu-id="48988-1226">Foi adicionado suporte para eventos de git de solicitação de pull e de confirmação para o gatilho de origem da tarefa</span><span class="sxs-lookup"><span data-stu-id="48988-1226">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="48988-1227">Alterado para usar o padrão do Dockerfile se ele não for especificado no comando de compilação</span><span class="sxs-lookup"><span data-stu-id="48988-1227">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="48988-1228">ACS</span><span class="sxs-lookup"><span data-stu-id="48988-1228">ACS</span></span>
* <span data-ttu-id="48988-1229">[ALTERAÇÃO SIGNIFICATIVA] `enable_cloud_console_aks_browse` foi removido para habilitar 'az aks browse' por padrão</span><span class="sxs-lookup"><span data-stu-id="48988-1229">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="48988-1230">Supervisor</span><span class="sxs-lookup"><span data-stu-id="48988-1230">Advisor</span></span>
* <span data-ttu-id="48988-1231">Versão de GA</span><span class="sxs-lookup"><span data-stu-id="48988-1231">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="48988-1232">AMS</span><span class="sxs-lookup"><span data-stu-id="48988-1232">AMS</span></span>
* <span data-ttu-id="48988-1233">Novos grupos de comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="48988-1233">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="48988-1234">Novos comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="48988-1234">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="48988-1235">Adicionados parâmetros de criptografia com suporte para `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="48988-1235">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="48988-1236">O suporte adicionado para `ams transform output remove` agora pode ser executado passando o índice de saída a ser removido</span><span class="sxs-lookup"><span data-stu-id="48988-1236">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="48988-1237">Adicionados os argumentos `--correlation-data` e `--label` ao grupo de comandos `ams job`</span><span class="sxs-lookup"><span data-stu-id="48988-1237">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="48988-1238">Adicionados os argumentos `--storage-account` e `--container` ao grupo de comandos `ams asset`</span><span class="sxs-lookup"><span data-stu-id="48988-1238">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="48988-1239">Foram adicionados valores padrões para o horário de expiração (agora +23h) e permissões (Leitura) no comando `ams asset get-sas-url`</span><span class="sxs-lookup"><span data-stu-id="48988-1239">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="48988-1240">[ALTERAÇÃO SIGNIFICATIVA] O comando `ams streaming locator` foi substituído por `ams streaming-locator`</span><span class="sxs-lookup"><span data-stu-id="48988-1240">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="48988-1241">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--content-keys` de `ams streaming locator` foi atualizado</span><span class="sxs-lookup"><span data-stu-id="48988-1241">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="48988-1242">[ALTERAÇÃO SIGNIFICATIVA] `--content-policy-name` foi renomeado como `--content-key-policy-name` no comando `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="48988-1242">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="48988-1243">[ALTERAÇÃO SIGNIFICATIVA] O comando `ams streaming policy` foi substituído por `ams streaming-policy`</span><span class="sxs-lookup"><span data-stu-id="48988-1243">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="48988-1244">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--preset-names` foi substituído por `--preset` no grupo de comandos `ams transform`.</span><span class="sxs-lookup"><span data-stu-id="48988-1244">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="48988-1245">Agora, você só pode definir uma saída/predefinição de cada vez (para adicionar mais, é preciso executar `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="48988-1245">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="48988-1246">Além disso, você pode definir StandardEncoderPreset personalizado passando o caminho para seu JSON personalizado</span><span class="sxs-lookup"><span data-stu-id="48988-1246">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="48988-1247">[ALTERAÇÃO SIGNIFICATIVA] `--output-asset-names ` foi renomeado como `--output-assets` no comando `ams job start`.</span><span class="sxs-lookup"><span data-stu-id="48988-1247">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="48988-1248">Agora, ele aceita uma lista separada por espaços dos ativos no formato 'assetName=label'.</span><span class="sxs-lookup"><span data-stu-id="48988-1248">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="48988-1249">Um ativo sem rótulo pode ser enviado assim: 'assetName='</span><span class="sxs-lookup"><span data-stu-id="48988-1249">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="48988-1250">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-1250">AppService</span></span>
* <span data-ttu-id="48988-1251">Um bug no `az webapp config backup update` que impede a configuração de um agendamento de backup foi corrigido, caso ele ainda não tenha sido definido</span><span class="sxs-lookup"><span data-stu-id="48988-1251">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="48988-1252">Configurar</span><span class="sxs-lookup"><span data-stu-id="48988-1252">Configure</span></span>
* <span data-ttu-id="48988-1253">O YAML foi adicionado às opções de formato de saída</span><span class="sxs-lookup"><span data-stu-id="48988-1253">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="48988-1254">Contêiner</span><span class="sxs-lookup"><span data-stu-id="48988-1254">Container</span></span>
* <span data-ttu-id="48988-1255">Alterado para mostrar a identidade ao exportar um grupo de contêineres para yaml</span><span class="sxs-lookup"><span data-stu-id="48988-1255">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="48988-1256">EventHub</span><span class="sxs-lookup"><span data-stu-id="48988-1256">EventHub</span></span>
* <span data-ttu-id="48988-1257">O sinalizador `--enable-kafka` foi adicionado para dar suporte ao Kafka no `eventhub namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48988-1257">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="48988-1258">Interativo</span><span class="sxs-lookup"><span data-stu-id="48988-1258">Interactive</span></span>
* <span data-ttu-id="48988-1259">O interativo agora instala a extensão `interactive` que permite atualizações e suporte mais rápidos</span><span class="sxs-lookup"><span data-stu-id="48988-1259">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="48988-1260">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="48988-1260">Monitor</span></span>
* <span data-ttu-id="48988-1261">Foi adicionado suporte para nomes de métricas, que incluem os caracteres barra (/) e ponto (.) para `--condition` em `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48988-1261">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="48988-1262">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-1262">Network</span></span>
* <span data-ttu-id="48988-1263">Os nomes de comandos `network interface-endpoint` foram preteridos em benefício de `network private-endpoint`</span><span class="sxs-lookup"><span data-stu-id="48988-1263">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="48988-1264">Foi corrigido um problema onde um argumento `--peer-circuit` em `express-route peering connection create` não aceitaria uma ID</span><span class="sxs-lookup"><span data-stu-id="48988-1264">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="48988-1265">Foi corrigido um problema onde `--ip-tags` não funcionava corretamente com `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="48988-1265">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="48988-1266">Perfil</span><span class="sxs-lookup"><span data-stu-id="48988-1266">Profile</span></span>
* <span data-ttu-id="48988-1267">`--use-cert-sn-issuer` foi adicionado a `az login` para logon da entidade de serviço com rolagens automáticas de certificado</span><span class="sxs-lookup"><span data-stu-id="48988-1267">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="48988-1268">RDBMS</span><span class="sxs-lookup"><span data-stu-id="48988-1268">RDBMS</span></span>
* <span data-ttu-id="48988-1269">Adicionados comandos da réplica mysql</span><span class="sxs-lookup"><span data-stu-id="48988-1269">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="48988-1270">Recurso</span><span class="sxs-lookup"><span data-stu-id="48988-1270">Resource</span></span>
* <span data-ttu-id="48988-1271">Adicionado suporte para grupos de gerenciamento e assinaturas aos comandos `policy definition|set-definition`</span><span class="sxs-lookup"><span data-stu-id="48988-1271">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="48988-1272">Função</span><span class="sxs-lookup"><span data-stu-id="48988-1272">Role</span></span>
* <span data-ttu-id="48988-1273">Adicionado suporte para gerenciamento de permissões de API, usuário conectado e gerenciamento de senhas dos aplicativos e certificados de credenciais</span><span class="sxs-lookup"><span data-stu-id="48988-1273">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="48988-1274">`ad sp create-for-rbac` foi alterado para esclarecer a confusão entre o displayName e o nome da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="48988-1274">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="48988-1275">Suporte adicionado para conceder permissões a aplicativos do AAD</span><span class="sxs-lookup"><span data-stu-id="48988-1275">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="48988-1276">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48988-1276">Storage</span></span>
* <span data-ttu-id="48988-1277">Suporte adicionado para se conectar aos serviços de armazenamento somente com SAS e pontos de extremidade (sem um nome de conta ou uma chave), conforme descrito em `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span><span class="sxs-lookup"><span data-stu-id="48988-1277">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="48988-1278">VM</span><span class="sxs-lookup"><span data-stu-id="48988-1278">VM</span></span>
* <span data-ttu-id="48988-1279">O argumento `storage-sku` foi adicionado a `image create` para definir o tipo de conta de armazenamento padrão da imagem</span><span class="sxs-lookup"><span data-stu-id="48988-1279">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="48988-1280">O bug com `vm resize` onde a opção `--no-wait` faz com que o comando falhasse foi corrigido</span><span class="sxs-lookup"><span data-stu-id="48988-1280">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="48988-1281">O formato de saída da tabela `vm encryption show` para mostrar o status foi alterado</span><span class="sxs-lookup"><span data-stu-id="48988-1281">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="48988-1282">`vm secret format` foi alterado para exigir a saída json/jsonc.</span><span class="sxs-lookup"><span data-stu-id="48988-1282">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="48988-1283">Avisa o usuário e assume como padrão a saída json se um formato de saída indesejado for escolhido</span><span class="sxs-lookup"><span data-stu-id="48988-1283">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="48988-1284">Validação de argumento aprimorado para `vm create --image`</span><span class="sxs-lookup"><span data-stu-id="48988-1284">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="48988-1285">23 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="48988-1285">October 23, 2018</span></span>

<span data-ttu-id="48988-1286">Versão 2.0.49</span><span class="sxs-lookup"><span data-stu-id="48988-1286">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="48988-1287">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48988-1287">Core</span></span>
* <span data-ttu-id="48988-1288">Corrigido o problema com `--ids` onde `--subscription` teria precedência sobre a assinatura em `--ids`</span><span class="sxs-lookup"><span data-stu-id="48988-1288">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="48988-1289">Adicionados avisos explícitos quando parâmetros seriam ignorados pelo uso de `--ids`</span><span class="sxs-lookup"><span data-stu-id="48988-1289">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="48988-1290">ACR</span><span class="sxs-lookup"><span data-stu-id="48988-1290">ACR</span></span>
* <span data-ttu-id="48988-1291">Corrigido um problema de codificação de ACR Build no Python2</span><span class="sxs-lookup"><span data-stu-id="48988-1291">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="48988-1292">CDN</span><span class="sxs-lookup"><span data-stu-id="48988-1292">CDN</span></span>
* <span data-ttu-id="48988-1293">[ALTERAÇÃO SIGNIFICATIVA] Alterado o comportamento de armazenamento em cache da cadeia de caracteres de consulta padrão de `cdn endpoint create` para não assumir o padrão "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="48988-1293">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="48988-1294">Agora, ele é definido pelo serviço</span><span class="sxs-lookup"><span data-stu-id="48988-1294">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="48988-1295">Contêiner</span><span class="sxs-lookup"><span data-stu-id="48988-1295">Container</span></span>
* <span data-ttu-id="48988-1296">Adicionado `Private` como um tipo válido para passar para '--ip-address'</span><span class="sxs-lookup"><span data-stu-id="48988-1296">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="48988-1297">Alterado para permitir o uso somente de ID de sub-rede para configurar uma rede virtual para o grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="48988-1297">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="48988-1298">Alterado para permitir o uso de nome de rede virtual ou ID de recurso para habilitar o uso de redes virtuais de diferentes grupos de recursos</span><span class="sxs-lookup"><span data-stu-id="48988-1298">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="48988-1299">Adicionado `--assign-identity` para adicionar uma identidade MSI a um grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="48988-1299">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="48988-1300">Adicionado `--scope` para criar uma atribuição de função para a identidade MSI atribuída pelo sistema</span><span class="sxs-lookup"><span data-stu-id="48988-1300">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="48988-1301">Adicionado um aviso ao criar um grupo de contêineres com uma imagem sem um processo de execução longa</span><span class="sxs-lookup"><span data-stu-id="48988-1301">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="48988-1302">Corrigidos os problemas de saída da tabela para comandos `list` e `show`</span><span class="sxs-lookup"><span data-stu-id="48988-1302">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="48988-1303">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="48988-1303">CosmosDB</span></span>
* <span data-ttu-id="48988-1304">Adicionado o suporte `--enable-multiple-write-locations` para `cosmosdb create`</span><span class="sxs-lookup"><span data-stu-id="48988-1304">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="48988-1305">Interativo</span><span class="sxs-lookup"><span data-stu-id="48988-1305">Interactive</span></span>
* <span data-ttu-id="48988-1306">Alterado para garantir que o parâmetro de assinatura global seja exibido nos parâmetros</span><span class="sxs-lookup"><span data-stu-id="48988-1306">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="48988-1307">Central da IoT</span><span class="sxs-lookup"><span data-stu-id="48988-1307">IoT Central</span></span>
* <span data-ttu-id="48988-1308">Adicionadas opções de nome de exibição e modelo para criação de aplicativos de IoT Central</span><span class="sxs-lookup"><span data-stu-id="48988-1308">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="48988-1309">[ALTERAÇÃO SIGNIFICATIVA] Removido o suporte para a SKU F1; Use a SKU S1</span><span class="sxs-lookup"><span data-stu-id="48988-1309">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="48988-1310">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="48988-1310">Monitor</span></span>
* <span data-ttu-id="48988-1311">Alterações para `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="48988-1311">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="48988-1312">Adicionado suporte para listar todos os eventos no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="48988-1312">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="48988-1313">Adicionado o parâmetro `--offset` para criar consultas de tempo mais facilmente</span><span class="sxs-lookup"><span data-stu-id="48988-1313">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="48988-1314">Melhorada a validação para `--start-time` e `--end-time` para usar um intervalo mais amplo de formatos ISO8601 e formatos de data/hora mais amigáveis ao usuário</span><span class="sxs-lookup"><span data-stu-id="48988-1314">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="48988-1315">Adicionado `--namespace` como alias para a opção preterida `--resource-provider`</span><span class="sxs-lookup"><span data-stu-id="48988-1315">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="48988-1316">Preterido `--filters` porque não há valores diferentes daqueles com opções fortemente tipadas compatíveis com o serviço</span><span class="sxs-lookup"><span data-stu-id="48988-1316">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="48988-1317">Alterações para `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="48988-1317">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="48988-1318">Adicionado o parâmetro `--offset` para criar consultas de tempo mais facilmente</span><span class="sxs-lookup"><span data-stu-id="48988-1318">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="48988-1319">Melhorada a validação para `--start-time` e `--end-time` para usar um intervalo mais amplo de formatos ISO8601 e formatos de data/hora mais amigáveis ao usuário</span><span class="sxs-lookup"><span data-stu-id="48988-1319">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="48988-1320">Melhorada a validação para os argumentos `--event-hub` e `--event-hub-rule` para `monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="48988-1320">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="48988-1321">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-1321">Network</span></span>
* <span data-ttu-id="48988-1322">Adicionados os argumentos `--app-gateway-address-pools` e `--gateway-name` para `nic create`, para dar suporte à adição de pools de endereços de back-end do gateway de aplicativo a um NIC</span><span class="sxs-lookup"><span data-stu-id="48988-1322">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="48988-1323">Adicionados os argumentos `--app-gateway-address-pools` e `--gateway-name` para `nic ip-config create/update`, para dar suporte à adição de pools de endereços de back-end do gateway de aplicativo a um NIC</span><span class="sxs-lookup"><span data-stu-id="48988-1323">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="48988-1324">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="48988-1324">ServiceBus</span></span>
* <span data-ttu-id="48988-1325">Adicionado `migration_state` somente leitura para MigrationConfigProperties para mostrar o atual estado de migração de namespace Standard para Premium do Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="48988-1325">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="48988-1326">SQL</span><span class="sxs-lookup"><span data-stu-id="48988-1326">SQL</span></span>
* <span data-ttu-id="48988-1327">Corrigidos `sql failover-group create` e `sql failover-group update` para trabalhar com a política de failover Manual</span><span class="sxs-lookup"><span data-stu-id="48988-1327">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="48988-1328">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48988-1328">Storage</span></span>
* <span data-ttu-id="48988-1329">Corrigida a formatação de saída `az storage cors list`, todos os itens mostram a chave correta de "Serviço"</span><span class="sxs-lookup"><span data-stu-id="48988-1329">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="48988-1330">Adicionado o parâmetro `--bypass-immutability-policy` para a exclusão de contêiner bloqueado pela política de imutabilidade</span><span class="sxs-lookup"><span data-stu-id="48988-1330">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="48988-1331">VM</span><span class="sxs-lookup"><span data-stu-id="48988-1331">VM</span></span>
* <span data-ttu-id="48988-1332">Aplicado o modo `None` de armazenamento em cache de disco para as séries Lv/Lv2 de computadores no `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="48988-1332">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="48988-1333">Atualizada a lista de tamanhos com suporte compatíveis com a aceleração de rede para `vm create`</span><span class="sxs-lookup"><span data-stu-id="48988-1333">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="48988-1334">Adicionado argumentos fortemente tipados para configurações de iops e mbps de ultra ssd para `disk create`</span><span class="sxs-lookup"><span data-stu-id="48988-1334">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="48988-1335">16 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="48988-1335">October 16, 2018</span></span>

<span data-ttu-id="48988-1336">Versão 2.0.48</span><span class="sxs-lookup"><span data-stu-id="48988-1336">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="48988-1337">VM</span><span class="sxs-lookup"><span data-stu-id="48988-1337">VM</span></span>
* <span data-ttu-id="48988-1338">Corrigido o problema do SDK que causava falha durante a instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="48988-1338">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="48988-1339">9 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="48988-1339">October 9, 2018</span></span>

<span data-ttu-id="48988-1340">Versão 2.0.47</span><span class="sxs-lookup"><span data-stu-id="48988-1340">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="48988-1341">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48988-1341">Core</span></span>
* <span data-ttu-id="48988-1342">Melhoria do tratamento de erro para os erros de "Solicitação Incorreta"</span><span class="sxs-lookup"><span data-stu-id="48988-1342">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="48988-1343">ACR</span><span class="sxs-lookup"><span data-stu-id="48988-1343">ACR</span></span>
* <span data-ttu-id="48988-1344">Suporte adicionado para o formato de tabela semelhante como cliente do helm</span><span class="sxs-lookup"><span data-stu-id="48988-1344">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="48988-1345">ACS</span><span class="sxs-lookup"><span data-stu-id="48988-1345">ACS</span></span>
* <span data-ttu-id="48988-1346">`aks [create|scale] --nodepool-name` adicionado para configurar o nome nodepool, truncado com 12 caracteres, padrão – nodepool1</span><span class="sxs-lookup"><span data-stu-id="48988-1346">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="48988-1347">Corrigido para voltar para “scp” quando Parimiko falha</span><span class="sxs-lookup"><span data-stu-id="48988-1347">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="48988-1348">`aks create` alterado para não precisar mais de `--aad-tenant-id`</span><span class="sxs-lookup"><span data-stu-id="48988-1348">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="48988-1349">Melhoria da mesclagem das credenciais do Kubernetes quando houver entradas duplicadas</span><span class="sxs-lookup"><span data-stu-id="48988-1349">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="48988-1350">Contêiner</span><span class="sxs-lookup"><span data-stu-id="48988-1350">Container</span></span>
* <span data-ttu-id="48988-1351">`functionapp create` alterado para dar suporte à criação de um tipo de plano de consumo do Linux com um runtime específico</span><span class="sxs-lookup"><span data-stu-id="48988-1351">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="48988-1352">[VERSÃO PRÉVIA] Suporte adicionado para hospedar aplicativos Web nos contêineres do Windows</span><span class="sxs-lookup"><span data-stu-id="48988-1352">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="48988-1353">Hub de evento</span><span class="sxs-lookup"><span data-stu-id="48988-1353">Event Hub</span></span>
* <span data-ttu-id="48988-1354">Corrigido o comando `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="48988-1354">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="48988-1355">[ALTERAÇÃO SIGNIFICATIVA] `list` comandos alterados para lidar com os erros de recurso(s) NotFound(404) do modo típico, em vez de mostrar uma lista vazia</span><span class="sxs-lookup"><span data-stu-id="48988-1355">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="48988-1356">Extensões</span><span class="sxs-lookup"><span data-stu-id="48988-1356">Extensions</span></span>
* <span data-ttu-id="48988-1357">Corrigido o problema ao tentar adicionar uma extensão já instalada</span><span class="sxs-lookup"><span data-stu-id="48988-1357">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="48988-1358">HDInsight</span><span class="sxs-lookup"><span data-stu-id="48988-1358">HDInsight</span></span>
* <span data-ttu-id="48988-1359">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="48988-1359">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="48988-1360">IoT</span><span class="sxs-lookup"><span data-stu-id="48988-1360">IoT</span></span>
* <span data-ttu-id="48988-1361">Comando de instalação da extensão adicionado à faixa inicial</span><span class="sxs-lookup"><span data-stu-id="48988-1361">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="48988-1362">KeyVault</span><span class="sxs-lookup"><span data-stu-id="48988-1362">KeyVault</span></span>
* <span data-ttu-id="48988-1363">Alterado para restringir os comandos de armazenamento do keyvault ao perfil da API mais recente</span><span class="sxs-lookup"><span data-stu-id="48988-1363">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="48988-1364">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-1364">Network</span></span>
* <span data-ttu-id="48988-1365">Corrigido `network dns zone create`: O comando terá êxito mesmo se o usuário tiver configurado um local padrão.</span><span class="sxs-lookup"><span data-stu-id="48988-1365">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="48988-1366">Veja o n° 6052</span><span class="sxs-lookup"><span data-stu-id="48988-1366">See #6052</span></span>
* <span data-ttu-id="48988-1367">Preterido `--remote-vnet-id` para `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="48988-1367">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="48988-1368">`--remote-vnet` a `network vnet peering create` adicionados, que aceita um nome ou uma ID</span><span class="sxs-lookup"><span data-stu-id="48988-1368">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="48988-1369">Suporte adicionado para vários prefixos de sub-rede a `network vnet create` com `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="48988-1369">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="48988-1370">Suporte adicionado para vários prefixos de sub-rede a `network vnet subnet [create|update]` com `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="48988-1370">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="48988-1371">Corrigido o problema com `network application-gateway create` que impedia a criação de gateways com a SKU `WAF_v2` ou `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="48988-1371">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="48988-1372">Argumento de conveniência `--service-endpoint-policy` adicionado a `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="48988-1372">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="48988-1373">Função</span><span class="sxs-lookup"><span data-stu-id="48988-1373">Role</span></span>
* <span data-ttu-id="48988-1374">Suporte adicionado para listar os proprietários de aplicativo do Azure AD para `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="48988-1374">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="48988-1375">Suporte adicionado para listar os proprietários da entidade de serviço do Azure AD para `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="48988-1375">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="48988-1376">Alterado para garantir que os comandos para criar e atualizar a definição da função aceitem várias configurações de permissão</span><span class="sxs-lookup"><span data-stu-id="48988-1376">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="48988-1377">`ad sp create-for-rbac` alterado para garantir que a URI da home page sempre seja "https"</span><span class="sxs-lookup"><span data-stu-id="48988-1377">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="48988-1378">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="48988-1378">Service Bus</span></span>
* <span data-ttu-id="48988-1379">[ALTERAÇÃO SIGNIFICATIVA] `list` comandos alterados para lidar com os erros de recurso(s) NotFound(404) do modo típico, em vez de mostrar uma lista vazia</span><span class="sxs-lookup"><span data-stu-id="48988-1379">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="48988-1380">VM</span><span class="sxs-lookup"><span data-stu-id="48988-1380">VM</span></span>
* <span data-ttu-id="48988-1381">Corrigido o campo `accessSas` vazio em `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="48988-1381">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="48988-1382">`vmss create` alterado para reservar um intervalo de portas de front-end grande o suficiente para lidar com excesso de provisionamento</span><span class="sxs-lookup"><span data-stu-id="48988-1382">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="48988-1383">Corrigidos os comandos de atualização para `sig`</span><span class="sxs-lookup"><span data-stu-id="48988-1383">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="48988-1384">Suporte `--no-wait` adicionado para gerenciar as versões da imagem em `sig`</span><span class="sxs-lookup"><span data-stu-id="48988-1384">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="48988-1385">`vm list-ip-addresses` alterado para mostrar a zona de disponibilidade dos endereços IP públicos</span><span class="sxs-lookup"><span data-stu-id="48988-1385">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="48988-1386">`[vm|vmss] disk attach` alterado para definir o LUN padrão do disco para o primeiro ponto disponível</span><span class="sxs-lookup"><span data-stu-id="48988-1386">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="48988-1387">21 de setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="48988-1387">September 21, 2018</span></span>

<span data-ttu-id="48988-1388">Versão 2.0.46</span><span class="sxs-lookup"><span data-stu-id="48988-1388">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="48988-1389">ACR</span><span class="sxs-lookup"><span data-stu-id="48988-1389">ACR</span></span>
* <span data-ttu-id="48988-1390">Adicionados comandos de tarefa de ACR</span><span class="sxs-lookup"><span data-stu-id="48988-1390">Added ACR Task commands</span></span>
* <span data-ttu-id="48988-1391">Adicionado o comando de execução rápido</span><span class="sxs-lookup"><span data-stu-id="48988-1391">Added quick run command</span></span>
* <span data-ttu-id="48988-1392">Grupo de comandos `build-task` preteridos</span><span class="sxs-lookup"><span data-stu-id="48988-1392">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="48988-1393">Adicionado o grupo de comando `helm` para dar suporte ao gerenciamento de gráficos Helm com o ACR</span><span class="sxs-lookup"><span data-stu-id="48988-1393">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="48988-1394">Suporte adicionado para criação idempotente para registro gerenciado</span><span class="sxs-lookup"><span data-stu-id="48988-1394">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="48988-1395">Adicionado um sinalizador de formato no para exibir logs de build</span><span class="sxs-lookup"><span data-stu-id="48988-1395">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="48988-1396">ACS</span><span class="sxs-lookup"><span data-stu-id="48988-1396">ACS</span></span>
* <span data-ttu-id="48988-1397">Alterado o comando `install-connector` para definir o FQDN mestre do AKS</span><span class="sxs-lookup"><span data-stu-id="48988-1397">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="48988-1398">Corrigida a criação de atribuição de função para vnet-subnet-id ao não especificar a entidade de serviço e skip-role-assignment</span><span class="sxs-lookup"><span data-stu-id="48988-1398">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="48988-1399">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-1399">AppService</span></span>

* <span data-ttu-id="48988-1400">Adicionado suporte para o gerenciamento de operações de WebJobs (contínuos e disparados)</span><span class="sxs-lookup"><span data-stu-id="48988-1400">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="48988-1401">Suporte de az webapp config set para a propriedade --fts-state property. Adicionado suporte também para az functionapp config set & show</span><span class="sxs-lookup"><span data-stu-id="48988-1401">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="48988-1402">Adicionado suporte para trazer seu próprio armazenamento para aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="48988-1402">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="48988-1403">Adicionado suporte para a listar e restaurar aplicativos Web excluídos</span><span class="sxs-lookup"><span data-stu-id="48988-1403">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="48988-1404">Lote</span><span class="sxs-lookup"><span data-stu-id="48988-1404">Batch</span></span>
* <span data-ttu-id="48988-1405">Alterada a inclusão de tarefas por meio de `--json-file` para dar suporte à sintaxe AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="48988-1405">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="48988-1406">Atualizada a documentação de formatos `--json-file` aceitos</span><span class="sxs-lookup"><span data-stu-id="48988-1406">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="48988-1407">`--max-tasks-per-node-option` foi adicionado a `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="48988-1407">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="48988-1408">Alterado o comportamento de `batch account` para mostrar as contas atualmente conectadas se nenhuma opção foi especificada</span><span class="sxs-lookup"><span data-stu-id="48988-1408">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="48988-1409">Lote AI</span><span class="sxs-lookup"><span data-stu-id="48988-1409">Batch AI</span></span> 
* <span data-ttu-id="48988-1410">Corrigida a falha na criação de conta de armazenamento automática no comando `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="48988-1410">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="48988-1411">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="48988-1411">Cognitive Services</span></span>
* <span data-ttu-id="48988-1412">Adicionado o complemento para os argumentos `--sku`, `--kind`, `--location`</span><span class="sxs-lookup"><span data-stu-id="48988-1412">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="48988-1413">Adicionado o comando `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="48988-1413">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="48988-1414">Adicionado o comando `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="48988-1414">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="48988-1415">Adicionado o comando `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="48988-1415">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="48988-1416">Preterido `cognitiveservices list`</span><span class="sxs-lookup"><span data-stu-id="48988-1416">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="48988-1417">Alterado `--name` para que seja opcional para `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="48988-1417">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="48988-1418">Contêiner</span><span class="sxs-lookup"><span data-stu-id="48988-1418">Container</span></span>
* <span data-ttu-id="48988-1419">Adicionada a capacidade de reiniciar e parar um grupo de contêineres em execução</span><span class="sxs-lookup"><span data-stu-id="48988-1419">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="48988-1420">Adicionado `--network-profile` para passar em um perfil de rede</span><span class="sxs-lookup"><span data-stu-id="48988-1420">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="48988-1421">Adicionado `--subnet`, `--vnet_name`, para permitir a criação de grupos de contêineres em uma rede virtual</span><span class="sxs-lookup"><span data-stu-id="48988-1421">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="48988-1422">Alterada a saída da tabela para mostrar o status do grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="48988-1422">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="48988-1423">DataLake</span><span class="sxs-lookup"><span data-stu-id="48988-1423">Datalake</span></span>
* <span data-ttu-id="48988-1424">Comandos adicionados para regras da rede virtual</span><span class="sxs-lookup"><span data-stu-id="48988-1424">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="48988-1425">Shell interativo</span><span class="sxs-lookup"><span data-stu-id="48988-1425">Interactive Shell</span></span>
* <span data-ttu-id="48988-1426">Corrigido o erro no Windows em que comandos não são executados corretamente</span><span class="sxs-lookup"><span data-stu-id="48988-1426">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="48988-1427">Corrigido o problema para carregar o comando no modo interativo que era causado por objetos preteridos</span><span class="sxs-lookup"><span data-stu-id="48988-1427">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="48988-1428">IoT</span><span class="sxs-lookup"><span data-stu-id="48988-1428">IoT</span></span>
* <span data-ttu-id="48988-1429">Adicionado suporte para roteamento de Hubs de IoT</span><span class="sxs-lookup"><span data-stu-id="48988-1429">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="48988-1430">Key Vault</span><span class="sxs-lookup"><span data-stu-id="48988-1430">Key Vault</span></span>
* <span data-ttu-id="48988-1431">Corrigida a importação de chave do Key Vault para chaves RSA</span><span class="sxs-lookup"><span data-stu-id="48988-1431">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="48988-1432">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-1432">Network</span></span>
* <span data-ttu-id="48988-1433">Adicionados os comandos `network public-ip prefix` para dar suporte a recursos de prefixos de IP público</span><span class="sxs-lookup"><span data-stu-id="48988-1433">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="48988-1434">Adicionados os comandos `network service-endpoint` para dar suporte a recursos de política de ponto de extremidade de serviço</span><span class="sxs-lookup"><span data-stu-id="48988-1434">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="48988-1435">Adicionados os comandos `network lb outbound-rule` para dar suporte à criação de regras de saída do Standard Load Balancer</span><span class="sxs-lookup"><span data-stu-id="48988-1435">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="48988-1436">Adicionado `--public-ip-prefix` a `network lb frontend-ip create/update` para dar suporte a configurações de IP de front-end usando prefixos de IP público</span><span class="sxs-lookup"><span data-stu-id="48988-1436">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="48988-1437">Adicionado `--enable-tcp-reset` a `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="48988-1437">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="48988-1438">Adicionado `--disable-outbound-snat` a `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="48988-1438">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="48988-1439">Permitido o uso de `network watcher flow-log show/configure` com NSGs clássicos</span><span class="sxs-lookup"><span data-stu-id="48988-1439">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="48988-1440">Adição do comando `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="48988-1440">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="48988-1441">Corrigido o comando `network watcher test-connectivity` e adicionadas as propriedades `--method`, `--valid-status-codes` e `--headers`</span><span class="sxs-lookup"><span data-stu-id="48988-1441">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="48988-1442">`network express-route create/update`: Adicionado o sinalizador `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="48988-1442">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="48988-1443">`network vnet subnet create/update`: Adicionado suporte para `--delegation`</span><span class="sxs-lookup"><span data-stu-id="48988-1443">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="48988-1444">Adicionado o comando `network vnet subnet list-available-delegations`</span><span class="sxs-lookup"><span data-stu-id="48988-1444">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="48988-1445">`network traffic-manager profile create/update`: Adicionado suporte para `--interval`, `--timeout` e `--max-failures` para as opções preteridas de configuração do monitor `--monitor-path`, `--monitor-port` e `--monitor-protocol`, que foram substituídas por `--path`, `--port` e `--protocol`</span><span class="sxs-lookup"><span data-stu-id="48988-1445">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="48988-1446">`network lb frontend-ip create/update`: Corrigida a lógica para configurar o método de alocação de IP privado. Se um endereço IP privado for fornecido, a alocação será estática. Se nenhum endereço IP privado for fornecido ou uma cadeia de caracteres vazia for fornecida para o endereço IP privado, a alocação será dinâmica.</span><span class="sxs-lookup"><span data-stu-id="48988-1446">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="48988-1447">`dns record-set * create/update`: Adicionado suporte para `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="48988-1447">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="48988-1448">Adicionados comandos `network interface-endpoint` para consultar objetos do ponto de extremidade da interface</span><span class="sxs-lookup"><span data-stu-id="48988-1448">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="48988-1449">Adicionado `network profile show/list/delete` para gerenciamento parcial dos perfis de rede</span><span class="sxs-lookup"><span data-stu-id="48988-1449">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="48988-1450">Adicionados comandos `network express-route peering connection` para gerenciar conexões de emparelhamento entre as ExpressRoutes</span><span class="sxs-lookup"><span data-stu-id="48988-1450">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="48988-1451">RDBMS</span><span class="sxs-lookup"><span data-stu-id="48988-1451">RDBMS</span></span>
* <span data-ttu-id="48988-1452">Adicionado suporte para o serviço MariaDB</span><span class="sxs-lookup"><span data-stu-id="48988-1452">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="48988-1453">Reserva</span><span class="sxs-lookup"><span data-stu-id="48988-1453">Reservation</span></span>
* <span data-ttu-id="48988-1454">Adicionado CosmosDB no tipo enumerado de recurso reservado</span><span class="sxs-lookup"><span data-stu-id="48988-1454">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="48988-1455">Adicionada a propriedade nome no modelo do Patch</span><span class="sxs-lookup"><span data-stu-id="48988-1455">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="48988-1456">Gerenciar aplicativo</span><span class="sxs-lookup"><span data-stu-id="48988-1456">Manage App</span></span>
* <span data-ttu-id="48988-1457">Corrigido o bug em `managedapp create --kind MarketPlace` que resultava em falha durante a criação da instância de um aplicativo gerenciado do Marketplace</span><span class="sxs-lookup"><span data-stu-id="48988-1457">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="48988-1458">Alterados os comandos `feature` para serem restritos somente aos perfis com suporte</span><span class="sxs-lookup"><span data-stu-id="48988-1458">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="48988-1459">Função</span><span class="sxs-lookup"><span data-stu-id="48988-1459">Role</span></span>
* <span data-ttu-id="48988-1460">Adicionado suporte para listar membros de grupo de usuários</span><span class="sxs-lookup"><span data-stu-id="48988-1460">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="48988-1461">SignalR</span><span class="sxs-lookup"><span data-stu-id="48988-1461">SignalR</span></span>
* <span data-ttu-id="48988-1462">Primeira versão</span><span class="sxs-lookup"><span data-stu-id="48988-1462">First release</span></span>

### <a name="storage"></a><span data-ttu-id="48988-1463">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48988-1463">Storage</span></span>
* <span data-ttu-id="48988-1464">Adicionado o parâmetro `--auth-mode login` para usar as credenciais de login do usuário para autorização de filas e blobs</span><span class="sxs-lookup"><span data-stu-id="48988-1464">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="48988-1465">Adicionado `storage container immutability-policy/legal-hold` para gerenciar o armazenamento imutável</span><span class="sxs-lookup"><span data-stu-id="48988-1465">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="48988-1466">VM</span><span class="sxs-lookup"><span data-stu-id="48988-1466">VM</span></span>
* <span data-ttu-id="48988-1467">Corrigido o problema em que `vm create --generate-ssh-keys` sobrescreve o arquivo de chave privada se o arquivo de chave pública estiver ausente (#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="48988-1467">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="48988-1468">Adicionado suporte para galeria de imagem compartilhada através de `az sig`</span><span class="sxs-lookup"><span data-stu-id="48988-1468">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="48988-1469">28 de Agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="48988-1469">August 28, 2018</span></span>

<span data-ttu-id="48988-1470">Versão 2.0.45</span><span class="sxs-lookup"><span data-stu-id="48988-1470">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="48988-1471">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48988-1471">Core</span></span>

* <span data-ttu-id="48988-1472">Corrigido o problema de carregamento de arquivo de configuração vazio</span><span class="sxs-lookup"><span data-stu-id="48988-1472">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="48988-1473">Adicionado suporte para o perfil `2018-03-01-hybrid` para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="48988-1473">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="48988-1474">ACR</span><span class="sxs-lookup"><span data-stu-id="48988-1474">ACR</span></span>

* <span data-ttu-id="48988-1475">Adicionada uma solução alternativa para operações de runtime sem solicitações ARM</span><span class="sxs-lookup"><span data-stu-id="48988-1475">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="48988-1476">Alterado para excluir arquivos de controle de versão (por exemplo, .git, .gitignore) de tar carregados por padrão no comando `build`</span><span class="sxs-lookup"><span data-stu-id="48988-1476">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="48988-1477">ACS</span><span class="sxs-lookup"><span data-stu-id="48988-1477">ACS</span></span>

* <span data-ttu-id="48988-1478">Alterado `aks create` para os padrões para VMs `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="48988-1478">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="48988-1479">Alterado `aks get-credentials` para agora chamar novas APIs para obter credenciais de cluster</span><span class="sxs-lookup"><span data-stu-id="48988-1479">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="48988-1480">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-1480">AppService</span></span>

* <span data-ttu-id="48988-1481">Adicionado suporte para CORS no functionapp e webapp</span><span class="sxs-lookup"><span data-stu-id="48988-1481">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="48988-1482">Adicionado suporte a marcas ARM ao criar comandos</span><span class="sxs-lookup"><span data-stu-id="48988-1482">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="48988-1483">Alterado `[webapp|functionapp] identity show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="48988-1483">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="48988-1484">Backup</span><span class="sxs-lookup"><span data-stu-id="48988-1484">Backup</span></span>

* <span data-ttu-id="48988-1485">Alterado `backup vault backup-properties show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="48988-1485">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="48988-1486">Serviço de Bot</span><span class="sxs-lookup"><span data-stu-id="48988-1486">Bot Service</span></span>

* <span data-ttu-id="48988-1487">Versão da CLI do serviço de Bot inicial</span><span class="sxs-lookup"><span data-stu-id="48988-1487">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="48988-1488">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="48988-1488">Cognitive Services</span></span>

* <span data-ttu-id="48988-1489">Adicionado novo parâmetro `--api-properties,` que é necessário para a criação de alguns dos serviços</span><span class="sxs-lookup"><span data-stu-id="48988-1489">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="48988-1490">IoT</span><span class="sxs-lookup"><span data-stu-id="48988-1490">IoT</span></span>

* <span data-ttu-id="48988-1491">Corrigido o problema com a associação de hubs vinculados</span><span class="sxs-lookup"><span data-stu-id="48988-1491">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="48988-1492">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="48988-1492">Monitor</span></span>

* <span data-ttu-id="48988-1493">Adicionados comandos `monitor metrics alert` para alertas de métrica quase em tempo real</span><span class="sxs-lookup"><span data-stu-id="48988-1493">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="48988-1494">Comandos `monitor alert` preteridos</span><span class="sxs-lookup"><span data-stu-id="48988-1494">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="48988-1495">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-1495">Network</span></span>

* <span data-ttu-id="48988-1496">Alterado `network application-gateway ssl-policy predefined show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="48988-1496">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="48988-1497">Recurso</span><span class="sxs-lookup"><span data-stu-id="48988-1497">Resource</span></span>

* <span data-ttu-id="48988-1498">Alterado `provider operation show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="48988-1498">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="48988-1499">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48988-1499">Storage</span></span>

* <span data-ttu-id="48988-1500">Alterado `storage share policy show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="48988-1500">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="48988-1501">VM</span><span class="sxs-lookup"><span data-stu-id="48988-1501">VM</span></span>

* <span data-ttu-id="48988-1502">Alterado `vm/vmss identity show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="48988-1502">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="48988-1503">Preterido `--storage-caching` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="48988-1503">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="48988-1504">14 de agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="48988-1504">Auguest 14, 2018</span></span>

<span data-ttu-id="48988-1505">Versão 2.0.44</span><span class="sxs-lookup"><span data-stu-id="48988-1505">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="48988-1506">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48988-1506">Core</span></span>

* <span data-ttu-id="48988-1507">Corrigida a exibição numérica na saída `table`</span><span class="sxs-lookup"><span data-stu-id="48988-1507">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="48988-1508">Adicionado o formato de saída YAML</span><span class="sxs-lookup"><span data-stu-id="48988-1508">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="48988-1509">Telemetria</span><span class="sxs-lookup"><span data-stu-id="48988-1509">Telemetry</span></span>

* <span data-ttu-id="48988-1510">Melhorias nos relatórios de telemetria</span><span class="sxs-lookup"><span data-stu-id="48988-1510">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="48988-1511">ACR</span><span class="sxs-lookup"><span data-stu-id="48988-1511">ACR</span></span>

* <span data-ttu-id="48988-1512">Adicionados os comandos `content-trust policy`</span><span class="sxs-lookup"><span data-stu-id="48988-1512">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="48988-1513">Corrigido o problema onde `.dockerignore` não foi tratado adequadamente</span><span class="sxs-lookup"><span data-stu-id="48988-1513">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="48988-1514">ACS</span><span class="sxs-lookup"><span data-stu-id="48988-1514">ACS</span></span>

* <span data-ttu-id="48988-1515">Alterado `az acs/aks install-cli` para instalar em `%USERPROFILE%\.azure-kubectl` no Windows</span><span class="sxs-lookup"><span data-stu-id="48988-1515">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="48988-1516">Alterado `az aks install-connector` para detectar se o cluster tem RBAC e configurar o conector ACI adequadamente</span><span class="sxs-lookup"><span data-stu-id="48988-1516">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="48988-1517">Alterado para atribuição de função à sub-rede quando ela é fornecida</span><span class="sxs-lookup"><span data-stu-id="48988-1517">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="48988-1518">Adicionada uma nova opção para “ignorar a atribuição de função” à sub-rede quando ela é fornecida</span><span class="sxs-lookup"><span data-stu-id="48988-1518">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="48988-1519">Alterado para ignorar a atribuição de função à sub-rede quando a atribuição já existe</span><span class="sxs-lookup"><span data-stu-id="48988-1519">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="48988-1520">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-1520">AppService</span></span>

* <span data-ttu-id="48988-1521">Corrigido um bug que impede a criação de um aplicativo de funções usando contas de armazenamento em grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="48988-1521">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="48988-1522">Corrigida uma falha na implantação de zip</span><span class="sxs-lookup"><span data-stu-id="48988-1522">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="48988-1523">BatchAI</span><span class="sxs-lookup"><span data-stu-id="48988-1523">BatchAI</span></span>

* <span data-ttu-id="48988-1524">Alterada a saída do agente para criação de conta de armazenamento automática para especificar “*grupo* de recurso”.</span><span class="sxs-lookup"><span data-stu-id="48988-1524">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="48988-1525">Contêiner</span><span class="sxs-lookup"><span data-stu-id="48988-1525">Container</span></span>

* <span data-ttu-id="48988-1526">Adicionado `--secure-environment-variables` para passar as variáveis de ambiente seguras para um contêiner</span><span class="sxs-lookup"><span data-stu-id="48988-1526">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="48988-1527">IoT</span><span class="sxs-lookup"><span data-stu-id="48988-1527">IoT</span></span>

* <span data-ttu-id="48988-1528">[ALTERAÇÃO SIGNIFICATIVA] Removidos os comandos preteridos que foram movidos para a extensão iot</span><span class="sxs-lookup"><span data-stu-id="48988-1528">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="48988-1529">Atualizados os elementos para não presumirem o domínio `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="48988-1529">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="48988-1530">Central de IoT</span><span class="sxs-lookup"><span data-stu-id="48988-1530">Iot Central</span></span>

* <span data-ttu-id="48988-1531">Versão inicial do módulo do IoT Central</span><span class="sxs-lookup"><span data-stu-id="48988-1531">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="48988-1532">KeyVault</span><span class="sxs-lookup"><span data-stu-id="48988-1532">KeyVault</span></span>


* <span data-ttu-id="48988-1533">Comandos adicionados para gerenciar contas de armazenamento e as definições de sas</span><span class="sxs-lookup"><span data-stu-id="48988-1533">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="48988-1534">Comandos adicionados para regras de rede</span><span class="sxs-lookup"><span data-stu-id="48988-1534">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="48988-1535">Adicionado o parâmetro `--id` para operações de certificado, chave e segredo</span><span class="sxs-lookup"><span data-stu-id="48988-1535">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="48988-1536">Adicionado suporte para a versão de várias APIs de gerenciamento KV</span><span class="sxs-lookup"><span data-stu-id="48988-1536">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="48988-1537">Adicionado suporte para a versão de várias APIs do plano de dados KV</span><span class="sxs-lookup"><span data-stu-id="48988-1537">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="48988-1538">Retransmissão</span><span class="sxs-lookup"><span data-stu-id="48988-1538">Relay</span></span>

* <span data-ttu-id="48988-1539">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="48988-1539">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="48988-1540">Sql</span><span class="sxs-lookup"><span data-stu-id="48988-1540">Sql</span></span>

* <span data-ttu-id="48988-1541">Adicionados os comandos `sql failover-group`</span><span class="sxs-lookup"><span data-stu-id="48988-1541">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="48988-1542">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48988-1542">Storage</span></span>

* <span data-ttu-id="48988-1543">[ALTERAÇÃO SIGNIFICATIVA] Alterado `storage account show-usage` para exigir o parâmetro `--location` e listará por região</span><span class="sxs-lookup"><span data-stu-id="48988-1543">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="48988-1544">Alterado o parâmetro `--resource-group` para ser opcional para comandos `storage account`</span><span class="sxs-lookup"><span data-stu-id="48988-1544">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="48988-1545">Removidos os avisos de “Falha na pré-condição” para as falhas individuais em comandos em lote para uma única mensagem agregada</span><span class="sxs-lookup"><span data-stu-id="48988-1545">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="48988-1546">Alterados os comandos `[blob|file] delete-batch` para não exibir mais matriz de nulos</span><span class="sxs-lookup"><span data-stu-id="48988-1546">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="48988-1547">Alterados os comandos `blob [download|upload|delete-batch]` para ler o token de sas da url do contêiner</span><span class="sxs-lookup"><span data-stu-id="48988-1547">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="48988-1548">VM</span><span class="sxs-lookup"><span data-stu-id="48988-1548">VM</span></span>

* <span data-ttu-id="48988-1549">Adicionado filtros comuns à `vm list-skus` para facilidade de uso</span><span class="sxs-lookup"><span data-stu-id="48988-1549">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="48988-1550">31 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="48988-1550">July 31, 2018</span></span>

<span data-ttu-id="48988-1551">Versão 2.0.43</span><span class="sxs-lookup"><span data-stu-id="48988-1551">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="48988-1552">ACR</span><span class="sxs-lookup"><span data-stu-id="48988-1552">ACR</span></span>

* <span data-ttu-id="48988-1553">Sinalizador `--with-secure-properties` adicionado ao comando `acr build-task show`</span><span class="sxs-lookup"><span data-stu-id="48988-1553">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="48988-1554">Adicionado o comando `acr build-task update-build`</span><span class="sxs-lookup"><span data-stu-id="48988-1554">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="48988-1555">ACS</span><span class="sxs-lookup"><span data-stu-id="48988-1555">ACS</span></span>

* <span data-ttu-id="48988-1556">Alterado para retornar 0 (êxito) ao terminar `az aks browse` pressionando [Ctrl+C]</span><span class="sxs-lookup"><span data-stu-id="48988-1556">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="48988-1557">Lote</span><span class="sxs-lookup"><span data-stu-id="48988-1557">Batch</span></span>

* <span data-ttu-id="48988-1558">Bug corrigido ao mostrar o token AAD no cloudshell</span><span class="sxs-lookup"><span data-stu-id="48988-1558">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="48988-1559">Contêiner</span><span class="sxs-lookup"><span data-stu-id="48988-1559">Container</span></span>

* <span data-ttu-id="48988-1560">Requisito removido de `--log-analytics-workspace-key` para o nome ou a ID ao definir assinatura</span><span class="sxs-lookup"><span data-stu-id="48988-1560">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="48988-1561">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-1561">Network</span></span>

* <span data-ttu-id="48988-1562">Suporte a DNS adicionado a 2017-03-09-profile para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="48988-1562">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="48988-1563">Recurso</span><span class="sxs-lookup"><span data-stu-id="48988-1563">Resource</span></span>

* <span data-ttu-id="48988-1564">`--rollback-on-error` a `group deployment create` adicionado para executar uma implantação válida no erro</span><span class="sxs-lookup"><span data-stu-id="48988-1564">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="48988-1565">Problema corrigido onde `--parameters {}` com `group deployment create` resultou em um erro</span><span class="sxs-lookup"><span data-stu-id="48988-1565">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="48988-1566">Função</span><span class="sxs-lookup"><span data-stu-id="48988-1566">Role</span></span>

* <span data-ttu-id="48988-1567">Suporte adicionado para o perfil da pilha 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="48988-1567">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="48988-1568">Problema corrigido onde os parâmetros de atualização genéricos para `app update` não funcionariam corretamente</span><span class="sxs-lookup"><span data-stu-id="48988-1568">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="48988-1569">Search</span><span class="sxs-lookup"><span data-stu-id="48988-1569">Search</span></span>

* <span data-ttu-id="48988-1570">Comandos adicionados para o serviço Azure Search</span><span class="sxs-lookup"><span data-stu-id="48988-1570">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="48988-1571">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="48988-1571">Service Bus</span></span>

* <span data-ttu-id="48988-1572">Grupo de comandos de migração adicionados para migrar um namespace do Barramento de Serviço Standard para Premium</span><span class="sxs-lookup"><span data-stu-id="48988-1572">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="48988-1573">Novas propriedades opcionais adicionadas à fila do Barramento de Serviço e à Assinatura</span><span class="sxs-lookup"><span data-stu-id="48988-1573">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="48988-1574">`--enable-batched-operations` e `--enable-dead-lettering-on-message-expiration` em `queue`</span><span class="sxs-lookup"><span data-stu-id="48988-1574">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="48988-1575">`--dead-letter-on-filter-exceptions` em `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="48988-1575">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="48988-1576">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48988-1576">Storage</span></span>

* <span data-ttu-id="48988-1577">Suporte adicionado para o download de arquivos grandes usando uma única conexão</span><span class="sxs-lookup"><span data-stu-id="48988-1577">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="48988-1578">Comandos `show` convertidos que foram perdidos na falha com código de saída 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="48988-1578">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="48988-1579">VM</span><span class="sxs-lookup"><span data-stu-id="48988-1579">VM</span></span>

* <span data-ttu-id="48988-1580">Suporte adicionado para listar conjuntos de disponibilidade por assinatura</span><span class="sxs-lookup"><span data-stu-id="48988-1580">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="48988-1581">Adicionado o suporte para `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="48988-1581">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="48988-1582">Suporte adicionado para o grupo de segurança do aplicativo ao criar um conjunto de dimensionamento da VM</span><span class="sxs-lookup"><span data-stu-id="48988-1582">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="48988-1583">[ALTERAÇÃO SIGNIFICATIVA] `[vm|vmss] create`, `[vm|vmss] identity assign` e `[vm|vmss] identity remove` alterados para produzir identidades de usuário atribuídas no formato de dicionário</span><span class="sxs-lookup"><span data-stu-id="48988-1583">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="48988-1584">18 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="48988-1584">July 18, 2018</span></span>

<span data-ttu-id="48988-1585">Versão 2.0.42</span><span class="sxs-lookup"><span data-stu-id="48988-1585">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="48988-1586">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48988-1586">Core</span></span>

* <span data-ttu-id="48988-1587">Adicionado suporte para logon baseado em navegador, na janela de bash WSL</span><span class="sxs-lookup"><span data-stu-id="48988-1587">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="48988-1588">O sinalizador `--force-string` foi adicionado a todos os comandos de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="48988-1588">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="48988-1589">[ALTERAÇÃO SIGNIFICATIVA] Os comandos 'show' foram alterados para registrar mensagens de erro e falha com código de saída 3 quando um recurso está ausente</span><span class="sxs-lookup"><span data-stu-id="48988-1589">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="48988-1590">ACR</span><span class="sxs-lookup"><span data-stu-id="48988-1590">ACR</span></span>

* <span data-ttu-id="48988-1591">[ALTERAÇÃO SIGNIFICATIVA] '--no-push' foi atualizado para um sinalizador puro no comando 'acr build'</span><span class="sxs-lookup"><span data-stu-id="48988-1591">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="48988-1592">Foram adicionados os comandos `show` e `update` no grupo `acr repository`</span><span class="sxs-lookup"><span data-stu-id="48988-1592">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="48988-1593">Foi adicionado o sinalizador `--detail` a `show-manifests` e `show-tags` para mostrar informações mais detalhadas</span><span class="sxs-lookup"><span data-stu-id="48988-1593">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="48988-1594">Foi adicionado o parâmetro `--image` para dar suporte aos detalhes do build get ou aos logs por meio de uma imagem</span><span class="sxs-lookup"><span data-stu-id="48988-1594">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="48988-1595">ACS</span><span class="sxs-lookup"><span data-stu-id="48988-1595">ACS</span></span>

* <span data-ttu-id="48988-1596">`az aks create` foi alterado para excluir o erro se `--max-pods` for menor que 5</span><span class="sxs-lookup"><span data-stu-id="48988-1596">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="48988-1597">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-1597">AppService</span></span>

* <span data-ttu-id="48988-1598">Suporte adicionado para skus PremiumV2</span><span class="sxs-lookup"><span data-stu-id="48988-1598">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="48988-1599">Lote</span><span class="sxs-lookup"><span data-stu-id="48988-1599">Batch</span></span>

* <span data-ttu-id="48988-1600">Corrigido o bug sobre como usar a credencial de token no modo do Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="48988-1600">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="48988-1601">Alterada a entrada JSON para diferenciar maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="48988-1601">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="48988-1602">Lote AI</span><span class="sxs-lookup"><span data-stu-id="48988-1602">Batch AI</span></span>

* <span data-ttu-id="48988-1603">Corrigido o comando `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="48988-1603">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="48988-1604">Contêiner</span><span class="sxs-lookup"><span data-stu-id="48988-1604">Container</span></span>

* <span data-ttu-id="48988-1605">Removido o requisito de nome de usuário e senha para os registros não dockerhub</span><span class="sxs-lookup"><span data-stu-id="48988-1605">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="48988-1606">Correção de erro durante a criação de grupos de contêineres de arquivo yaml</span><span class="sxs-lookup"><span data-stu-id="48988-1606">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="48988-1607">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-1607">Network</span></span>

* <span data-ttu-id="48988-1608">Adicionado o suporte `--no-wait` para `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="48988-1608">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="48988-1609">Adicionado `network nic wait`</span><span class="sxs-lookup"><span data-stu-id="48988-1609">Added `network nic wait`</span></span>
* <span data-ttu-id="48988-1610">Preterido o argumento `--ids` para `network vnet [subnet|peering] list`</span><span class="sxs-lookup"><span data-stu-id="48988-1610">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="48988-1611">Adicionado o sinalizador `--include-default` para incluir regras de segurança padrão na saída do `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="48988-1611">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="48988-1612">Recurso</span><span class="sxs-lookup"><span data-stu-id="48988-1612">Resource</span></span>

* <span data-ttu-id="48988-1613">Adicionado o suporte `--no-wait` para `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="48988-1613">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="48988-1614">Adicionado o suporte `--no-wait` para `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="48988-1614">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="48988-1615">Adicionado o comando `deployment wait`</span><span class="sxs-lookup"><span data-stu-id="48988-1615">Added `deployment wait` command</span></span>
* <span data-ttu-id="48988-1616">Correção do problema em que os comandos de nível de assinatura `az deployment` erroneamente apareceram no perfil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="48988-1616">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="48988-1617">SQL</span><span class="sxs-lookup"><span data-stu-id="48988-1617">SQL</span></span>

* <span data-ttu-id="48988-1618">O erro “O nome de grupo de recursos fornecido ... não correspondeu ao nome na Url” foi fixado ao especificar o nome do pool elástico para os comandos `sql db copy` e `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="48988-1618">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="48988-1619">Permitir a configuração do padrão do SQL Server, executando `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="48988-1619">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="48988-1620">Os formatadores de tabela foram implementados aos comandos `sql server`, `sql server firewall-rule`, `sql list-usages` e `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="48988-1620">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="48988-1621">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48988-1621">Storage</span></span>

* <span data-ttu-id="48988-1622">Adicionada a propriedade `pageRanges` à saída `storage blob show` que será preenchida para blobs de página</span><span class="sxs-lookup"><span data-stu-id="48988-1622">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="48988-1623">VM</span><span class="sxs-lookup"><span data-stu-id="48988-1623">VM</span></span>

* <span data-ttu-id="48988-1624">[ALTERAÇÃO SIGNIFICATIVA] Alterado `vmss create` para usar o `Standard_DS1_v2` como o tamanho de instância padrão</span><span class="sxs-lookup"><span data-stu-id="48988-1624">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="48988-1625">Adicionado o suporte `--no-wait` para `vm extension [set|delete]` e `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="48988-1625">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="48988-1626">Adicionado `vm extension wait`</span><span class="sxs-lookup"><span data-stu-id="48988-1626">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="48988-1627">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="48988-1627">July 3, 2018</span></span>

<span data-ttu-id="48988-1628">Versão 2.0.41</span><span class="sxs-lookup"><span data-stu-id="48988-1628">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="48988-1629">AKS</span><span class="sxs-lookup"><span data-stu-id="48988-1629">AKS</span></span>

* <span data-ttu-id="48988-1630">Monitoramento alterado para usar a ID de assinatura</span><span class="sxs-lookup"><span data-stu-id="48988-1630">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="48988-1631">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="48988-1631">July 3, 2018</span></span>

<span data-ttu-id="48988-1632">Versão 2.0.40</span><span class="sxs-lookup"><span data-stu-id="48988-1632">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="48988-1633">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48988-1633">Core</span></span>

* <span data-ttu-id="48988-1634">Adicionado um novo fluxo de código de autorização para o logon interativo</span><span class="sxs-lookup"><span data-stu-id="48988-1634">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="48988-1635">ACR</span><span class="sxs-lookup"><span data-stu-id="48988-1635">ACR</span></span>

* <span data-ttu-id="48988-1636">Status da compilação de sondagem adicionado</span><span class="sxs-lookup"><span data-stu-id="48988-1636">Added polling build status</span></span>
* <span data-ttu-id="48988-1637">Suporte adicionado para valores de enumeração que não diferenciam maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="48988-1637">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="48988-1638">Parâmetros `--top` e `--orderby` adicionados para `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="48988-1638">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="48988-1639">ACS</span><span class="sxs-lookup"><span data-stu-id="48988-1639">ACS</span></span>

* <span data-ttu-id="48988-1640">[ALTERAÇÃO SIGNIFICATIVA] Habilitar controle de acesso baseado em funções do Kubernetes por padrão</span><span class="sxs-lookup"><span data-stu-id="48988-1640">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="48988-1641">Argumento `--disable-rbac` e preterido `--enable-rbac` adicionados, pois é o padrão agora</span><span class="sxs-lookup"><span data-stu-id="48988-1641">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="48988-1642">Opções atualizadas do comando `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="48988-1642">Updated options for `aks browse` command.</span></span> <span data-ttu-id="48988-1643">Suporte `--listen-port` adicionado</span><span class="sxs-lookup"><span data-stu-id="48988-1643">Added `--listen-port` support</span></span>
* <span data-ttu-id="48988-1644">Atualizado o pacote de gráficos do helm padrão para o comando `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="48988-1644">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="48988-1645">Usar virtual-kubelet-para-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="48988-1645">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="48988-1646">Comandos `aks enable-addons` e `aks disable-addons` adicionados para atualizar um cluster existente</span><span class="sxs-lookup"><span data-stu-id="48988-1646">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="48988-1647">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-1647">AppService</span></span>

* <span data-ttu-id="48988-1648">Suporte adicionado para desabilitar a identidade via `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="48988-1648">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="48988-1649">Marca `preview` removida para o recurso de Identidade</span><span class="sxs-lookup"><span data-stu-id="48988-1649">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="48988-1650">Backup</span><span class="sxs-lookup"><span data-stu-id="48988-1650">Backup</span></span>

* <span data-ttu-id="48988-1651">Definição do módulo atualizada</span><span class="sxs-lookup"><span data-stu-id="48988-1651">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="48988-1652">BatchAI</span><span class="sxs-lookup"><span data-stu-id="48988-1652">BatchAI</span></span>

* <span data-ttu-id="48988-1653">Saída da tabela corrigida para comandos `batchai cluster node list` e `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="48988-1653">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="48988-1654">Nuvem</span><span class="sxs-lookup"><span data-stu-id="48988-1654">Cloud</span></span>

* <span data-ttu-id="48988-1655">Sufixo do servidor `acr login` adicionado à configuração de nuvem</span><span class="sxs-lookup"><span data-stu-id="48988-1655">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="48988-1656">Contêiner</span><span class="sxs-lookup"><span data-stu-id="48988-1656">Container</span></span>

* <span data-ttu-id="48988-1657">`container create` alterado para padrão para a operação de longa execução</span><span class="sxs-lookup"><span data-stu-id="48988-1657">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="48988-1658">Parâmetros `--log-analytics-workspace` e `--log-analytics-workspace-key` adicionados do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="48988-1658">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="48988-1659">Parâmetro `--protocol` adicionado para especificar qual protocolo de rede usar</span><span class="sxs-lookup"><span data-stu-id="48988-1659">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="48988-1660">Extensão</span><span class="sxs-lookup"><span data-stu-id="48988-1660">Extension</span></span>

* <span data-ttu-id="48988-1661">`extension list-available` alterado para mostrar apenas as extensões compatíveis com a versão da CLI</span><span class="sxs-lookup"><span data-stu-id="48988-1661">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="48988-1662">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-1662">Network</span></span>

* <span data-ttu-id="48988-1663">Corrigido o problema onde os tipos de registro diferenciam maiúsculas de minúsculas ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="48988-1663">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="48988-1664">Rdbms</span><span class="sxs-lookup"><span data-stu-id="48988-1664">Rdbms</span></span>

* <span data-ttu-id="48988-1665">Adicionados os comandos `[postgres|myql] server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="48988-1665">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="48988-1666">Recurso</span><span class="sxs-lookup"><span data-stu-id="48988-1666">Resource</span></span>

* <span data-ttu-id="48988-1667">Novo grupo de operação `deployment` adicionado</span><span class="sxs-lookup"><span data-stu-id="48988-1667">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="48988-1668">VM</span><span class="sxs-lookup"><span data-stu-id="48988-1668">VM</span></span>

* <span data-ttu-id="48988-1669">Suporte adicionado para remover a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="48988-1669">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="48988-1670">25 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="48988-1670">June 25, 2018</span></span>

<span data-ttu-id="48988-1671">Versão 2.0.39</span><span class="sxs-lookup"><span data-stu-id="48988-1671">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="48988-1672">CLI</span><span class="sxs-lookup"><span data-stu-id="48988-1672">CLI</span></span>

* <span data-ttu-id="48988-1673">Corte de arquivo atualizado no instalador MSI para corrigir o problema de instalação da extensão</span><span class="sxs-lookup"><span data-stu-id="48988-1673">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="48988-1674">19 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="48988-1674">June 19, 2018</span></span>

<span data-ttu-id="48988-1675">Versão 2.0.38</span><span class="sxs-lookup"><span data-stu-id="48988-1675">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="48988-1676">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48988-1676">Core</span></span>

* <span data-ttu-id="48988-1677">Suporte global adicionado para `--subscription` a maioria dos comandos</span><span class="sxs-lookup"><span data-stu-id="48988-1677">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="48988-1678">ACR</span><span class="sxs-lookup"><span data-stu-id="48988-1678">ACR</span></span>

* <span data-ttu-id="48988-1679">`azure-storage-blob` foi adicionado como dependência</span><span class="sxs-lookup"><span data-stu-id="48988-1679">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="48988-1680">A configuração de CPU padrão foi alterada com `acr build-task create` para usar 2 núcleos</span><span class="sxs-lookup"><span data-stu-id="48988-1680">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="48988-1681">ACS</span><span class="sxs-lookup"><span data-stu-id="48988-1681">ACS</span></span>

* <span data-ttu-id="48988-1682">As opções do comando `aks use-dev-spaces` foram atualizadas.</span><span class="sxs-lookup"><span data-stu-id="48988-1682">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="48988-1683">Suporte `--update` adicionado</span><span class="sxs-lookup"><span data-stu-id="48988-1683">Added `--update` support</span></span>
* <span data-ttu-id="48988-1684">`aks get-credentials --admin` foi alterado para substituir o contexto do usuário em `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="48988-1684">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="48988-1685">A propriedade `nodeResourceGroup` somente leitura foi exposta em clusters gerenciados</span><span class="sxs-lookup"><span data-stu-id="48988-1685">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="48988-1686">O erro de comando `acs browse` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="48988-1686">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="48988-1687">Foram feitas `--connector-name` opcional para `aks install-connector`, `aks upgrade-connector` e `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="48988-1687">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="48988-1688">Novas regiões de Instância de Contêiner do Azure foram adicionadas para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="48988-1688">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="48988-1689">O local normalizado foi adicionado no nome de versão do comando e no nome do nó para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="48988-1689">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="48988-1690">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-1690">AppService</span></span>

* <span data-ttu-id="48988-1691">Foi adicionado suporte para versões mais recentes do urllib</span><span class="sxs-lookup"><span data-stu-id="48988-1691">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="48988-1692">Foi adicionado suporte para `functionapp create` para usar o plano de serviço de aplicativo de grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="48988-1692">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="48988-1693">Lote</span><span class="sxs-lookup"><span data-stu-id="48988-1693">Batch</span></span>

* <span data-ttu-id="48988-1694">A dependência `azure-batch-extensions` foi removida</span><span class="sxs-lookup"><span data-stu-id="48988-1694">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="48988-1695">Lote AI</span><span class="sxs-lookup"><span data-stu-id="48988-1695">Batch AI</span></span>

* <span data-ttu-id="48988-1696">Foi adicionado suporte aos workspaces.</span><span class="sxs-lookup"><span data-stu-id="48988-1696">Added support for workspaces.</span></span> <span data-ttu-id="48988-1697">Os workspaces permitem agrupar clusters, servidores de arquivos e experimentos, removendo a limitação no número de recursos que podem ser criados</span><span class="sxs-lookup"><span data-stu-id="48988-1697">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="48988-1698">Foi adicionado suporte para os experimentos.</span><span class="sxs-lookup"><span data-stu-id="48988-1698">Added support for experiments.</span></span> <span data-ttu-id="48988-1699">Os experimentos permitem agrupar trabalhos em coleções removendo a limitação no número de trabalhos criados</span><span class="sxs-lookup"><span data-stu-id="48988-1699">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="48988-1700">Foi adicionado suporte para configurar `/dev/shm` para trabalhos em execução em um contêiner de docker</span><span class="sxs-lookup"><span data-stu-id="48988-1700">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="48988-1701">Foram adicionados os comandos `batchai cluster node exec` e `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="48988-1701">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="48988-1702">Esses comandos permitem executar qualquer comando diretamente nos nós e fornece a funcionalidade de encaminhamento de porta.</span><span class="sxs-lookup"><span data-stu-id="48988-1702">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="48988-1703">Foi adicionado suporte a `--ids` para os comandos `batchai`</span><span class="sxs-lookup"><span data-stu-id="48988-1703">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="48988-1704">[ALTERAÇÃO SIGNIFICATIVA] Todos os clusters e servidores de arquivos devem ser criados nos workspaces</span><span class="sxs-lookup"><span data-stu-id="48988-1704">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="48988-1705">[ALTERAÇÃO SIGNIFICATIVA] Os trabalhos devem ser criados nas experiências</span><span class="sxs-lookup"><span data-stu-id="48988-1705">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="48988-1706">[ALTERAÇÃO SIGNIFICATIVA] `--nfs-resource-group` foi removido dos comandos `cluster create` e `job create`.</span><span class="sxs-lookup"><span data-stu-id="48988-1706">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="48988-1707">Para montar um NFS pertencente a outro workspace/grupo de recursos, forneça a ID de ARM do servidor de arquivos através da opção `--nfs`</span><span class="sxs-lookup"><span data-stu-id="48988-1707">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="48988-1708">[ALTERAÇÃO SIGNIFICATIVA] `--cluster-resource-group` foi removido do comando `job create`.</span><span class="sxs-lookup"><span data-stu-id="48988-1708">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="48988-1709">Para enviar um trabalho em um cluster pertencente a outro workspace/grupo de recursos, forneça a ID de ARM do cluster através da opção `--cluster`</span><span class="sxs-lookup"><span data-stu-id="48988-1709">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="48988-1710">[ALTERAÇÃO SIGNIFICATIVA] O atributo `location` foi removido de trabalhos, cluster e servidores de arquivos.</span><span class="sxs-lookup"><span data-stu-id="48988-1710">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="48988-1711">Agora, o local é um atributo de um workspace.</span><span class="sxs-lookup"><span data-stu-id="48988-1711">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="48988-1712">[ALTERAÇÃO SIGNIFICATIVA] `--location` foi removido dos comandos `job create` e `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="48988-1712">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="48988-1713">[ALTERAÇÃO SIGNIFICATIVA] Os nomes das opções curtas foi alterado para tornar a interface mais consistente:</span><span class="sxs-lookup"><span data-stu-id="48988-1713">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="48988-1714">[`--config`, `-c`] foi renomeado para [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="48988-1714">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="48988-1715">[`--cluster`, `-r`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="48988-1715">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="48988-1716">[`--cluster`, `-n`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="48988-1716">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="48988-1717">[`--job`, `-n`] foi renomeado para [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="48988-1717">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="48988-1718">Mapas</span><span class="sxs-lookup"><span data-stu-id="48988-1718">Maps</span></span>

* <span data-ttu-id="48988-1719">[ALTERAÇÃO SIGNIFICATIVA] `maps account create` foi alterado para exigir a aceitação dos Termos de Serviço pelo prompt interativo ou sinalizador `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="48988-1719">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="48988-1720">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-1720">Network</span></span>

* <span data-ttu-id="48988-1721">Foi adicionado suporte a `https` para `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="48988-1721">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="48988-1722">Foi corrigido o problema em que `--endpoint-status` diferenciava maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="48988-1722">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="48988-1723">#6502</span><span class="sxs-lookup"><span data-stu-id="48988-1723">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="48988-1724">Reservas</span><span class="sxs-lookup"><span data-stu-id="48988-1724">Reservations</span></span>

* <span data-ttu-id="48988-1725">[ALTERAÇÃO SIGNIFICATIVA] Foi adicionado o parâmetro `ReservedResourceType` necessário a `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="48988-1725">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="48988-1726">Parâmetro `Location` adicionado a `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="48988-1726">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="48988-1727">[ALTERAÇÃO SIGNIFICATIVA] `kind` foi removido de `ReservationProperties`</span><span class="sxs-lookup"><span data-stu-id="48988-1727">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="48988-1728">[ALTERAÇÃO SIGNIFICATIVA] `capabilities` foi renomeado para `sku_properties` em `Catalog`</span><span class="sxs-lookup"><span data-stu-id="48988-1728">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="48988-1729">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `size` e `tier` foram removidas de `Catalog`</span><span class="sxs-lookup"><span data-stu-id="48988-1729">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="48988-1730">Parâmetro `InstanceFlexibility` adicionado a `reservations reservation update`</span><span class="sxs-lookup"><span data-stu-id="48988-1730">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="48988-1731">Função</span><span class="sxs-lookup"><span data-stu-id="48988-1731">Role</span></span>

* <span data-ttu-id="48988-1732">Tratamento de erro melhorado</span><span class="sxs-lookup"><span data-stu-id="48988-1732">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="48988-1733">SQL</span><span class="sxs-lookup"><span data-stu-id="48988-1733">SQL</span></span>

* <span data-ttu-id="48988-1734">Foi corrigido um erro confuso ao executar `az sql db list-editions` para um local que não está disponível para sua assinatura</span><span class="sxs-lookup"><span data-stu-id="48988-1734">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="48988-1735">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48988-1735">Storage</span></span>

* <span data-ttu-id="48988-1736">A saída da tabela foi alterada para `storage blob download` para ser mais legível</span><span class="sxs-lookup"><span data-stu-id="48988-1736">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="48988-1737">VM</span><span class="sxs-lookup"><span data-stu-id="48988-1737">VM</span></span>

* <span data-ttu-id="48988-1738">A verificação da refinação do tamanho da VM foi aprimorada para o suporte de rede acelerada em `vm create`</span><span class="sxs-lookup"><span data-stu-id="48988-1738">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="48988-1739">Foi adicionado um aviso para `vmss create` informando que o tamanho padrão da VM será alternado de `Standard_D1_v2` para `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="48988-1739">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="48988-1740">Foi adicionado `--force-update` a `[vm|vmss] extension set` para atualizar a extensão mesmo quando a configuração não foi alterada</span><span class="sxs-lookup"><span data-stu-id="48988-1740">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="48988-1741">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="48988-1741">June 13, 2018</span></span>

<span data-ttu-id="48988-1742">Versão 2.0.37</span><span class="sxs-lookup"><span data-stu-id="48988-1742">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="48988-1743">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48988-1743">Core</span></span>

* <span data-ttu-id="48988-1744">A telemetria interativa foi melhorada</span><span class="sxs-lookup"><span data-stu-id="48988-1744">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="48988-1745">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="48988-1745">June 13, 2018</span></span>

<span data-ttu-id="48988-1746">Versão 2.0.36</span><span class="sxs-lookup"><span data-stu-id="48988-1746">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="48988-1747">AKS</span><span class="sxs-lookup"><span data-stu-id="48988-1747">AKS</span></span>

* <span data-ttu-id="48988-1748">Foram adicionadas opções avançadas de rede para `aks create`</span><span class="sxs-lookup"><span data-stu-id="48988-1748">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="48988-1749">Foram adicionados argumentos para `aks create` para habilitar o monitoramento e roteamento de HTTP</span><span class="sxs-lookup"><span data-stu-id="48988-1749">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="48988-1750">Adicionado o argumento `--no-ssh-key` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="48988-1750">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="48988-1751">Adicionado o argumento `--enable-rbac` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="48988-1751">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="48988-1752">[VERSÃO PRÉVIA] Suporte adicionado para a autenticação do Azure Active Directory no `aks create`</span><span class="sxs-lookup"><span data-stu-id="48988-1752">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="48988-1753">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-1753">AppService</span></span>

* <span data-ttu-id="48988-1754">Foi corrigido um problema com as versões urllib incompatíveis</span><span class="sxs-lookup"><span data-stu-id="48988-1754">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="48988-1755">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="48988-1755">June 5, 2018</span></span>

<span data-ttu-id="48988-1756">Versão 2.0.35</span><span class="sxs-lookup"><span data-stu-id="48988-1756">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="48988-1757">Interativo</span><span class="sxs-lookup"><span data-stu-id="48988-1757">Interactive</span></span>

* <span data-ttu-id="48988-1758">Foram adicionados limites para as dependências do modo interativo</span><span class="sxs-lookup"><span data-stu-id="48988-1758">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="48988-1759">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="48988-1759">June 5, 2018</span></span>

<span data-ttu-id="48988-1760">Versão 2.0.34</span><span class="sxs-lookup"><span data-stu-id="48988-1760">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="48988-1761">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48988-1761">Core</span></span>

* <span data-ttu-id="48988-1762">Suporte adicionado para referência de recursos de locatário cruzado</span><span class="sxs-lookup"><span data-stu-id="48988-1762">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="48988-1763">Melhor confiabilidade de carregamento de telemetria</span><span class="sxs-lookup"><span data-stu-id="48988-1763">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="48988-1764">ACR</span><span class="sxs-lookup"><span data-stu-id="48988-1764">ACR</span></span>

* <span data-ttu-id="48988-1765">Suporte adicionado para VSTS como um local de origem remota</span><span class="sxs-lookup"><span data-stu-id="48988-1765">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="48988-1766">Adicionado o comando `acr import`</span><span class="sxs-lookup"><span data-stu-id="48988-1766">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="48988-1767">AKS</span><span class="sxs-lookup"><span data-stu-id="48988-1767">AKS</span></span>

* <span data-ttu-id="48988-1768">`aks get-credentials` foi alterado para criar o arquivo de configuração kube com permissões de sistema de arquivos mais seguras</span><span class="sxs-lookup"><span data-stu-id="48988-1768">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="48988-1769">Lote</span><span class="sxs-lookup"><span data-stu-id="48988-1769">Batch</span></span>

* <span data-ttu-id="48988-1770">Correção do bug na formatação de tabela da lista de Pool [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="48988-1770">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="48988-1771">IOT</span><span class="sxs-lookup"><span data-stu-id="48988-1771">IOT</span></span>

* <span data-ttu-id="48988-1772">Suporte adicionado para a criação de Hubs IoT de Camada Básica</span><span class="sxs-lookup"><span data-stu-id="48988-1772">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="48988-1773">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-1773">Network</span></span>

* <span data-ttu-id="48988-1774">`network vnet peering` melhorado</span><span class="sxs-lookup"><span data-stu-id="48988-1774">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="48988-1775">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="48988-1775">Policy Insights</span></span>

* <span data-ttu-id="48988-1776">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="48988-1776">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="48988-1777">ARM</span><span class="sxs-lookup"><span data-stu-id="48988-1777">ARM</span></span>

* <span data-ttu-id="48988-1778">Comandos `account management-group` adicionados.</span><span class="sxs-lookup"><span data-stu-id="48988-1778">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="48988-1779">SQL</span><span class="sxs-lookup"><span data-stu-id="48988-1779">SQL</span></span>

* <span data-ttu-id="48988-1780">Novos comandos de instância gerenciada adicionados:</span><span class="sxs-lookup"><span data-stu-id="48988-1780">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="48988-1781">Novos comandos de banco de dados gerenciado adicionados:</span><span class="sxs-lookup"><span data-stu-id="48988-1781">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="48988-1782">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48988-1782">Storage</span></span>

* <span data-ttu-id="48988-1783">Mimetypes extra adicionados para json e javascript para ser deduzido de extensões de arquivo</span><span class="sxs-lookup"><span data-stu-id="48988-1783">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="48988-1784">VM</span><span class="sxs-lookup"><span data-stu-id="48988-1784">VM</span></span>

* <span data-ttu-id="48988-1785">`vm list-skus` foi alterado para usar colunas fixas e adicionar o aviso de que `Tier` e `Size` serão removidos</span><span class="sxs-lookup"><span data-stu-id="48988-1785">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="48988-1786">Opção `--accelerated-networking` adicionada a `vm create`</span><span class="sxs-lookup"><span data-stu-id="48988-1786">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="48988-1787">`--tags` foi adicionado a `identity create`</span><span class="sxs-lookup"><span data-stu-id="48988-1787">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="48988-1788">22 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="48988-1788">May 22, 2018</span></span>

<span data-ttu-id="48988-1789">Versão 2.0.33</span><span class="sxs-lookup"><span data-stu-id="48988-1789">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="48988-1790">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48988-1790">Core</span></span>

* <span data-ttu-id="48988-1791">Suporte adicionado para expandir `@` em nomes de arquivos</span><span class="sxs-lookup"><span data-stu-id="48988-1791">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="48988-1792">ACS</span><span class="sxs-lookup"><span data-stu-id="48988-1792">ACS</span></span>

* <span data-ttu-id="48988-1793">Novos comandos de espaços de desenvolvimento `aks use-dev-spaces` e `aks remove-dev-spaces` foram adicionados</span><span class="sxs-lookup"><span data-stu-id="48988-1793">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="48988-1794">Erro de digitação corrigido na mensagem de ajuda</span><span class="sxs-lookup"><span data-stu-id="48988-1794">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="48988-1795">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-1795">AppService</span></span>

* <span data-ttu-id="48988-1796">Comandos melhorados de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="48988-1796">Improved generic update commands</span></span>
* <span data-ttu-id="48988-1797">Suporte assíncrono adicionado para `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="48988-1797">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="48988-1798">Contêiner</span><span class="sxs-lookup"><span data-stu-id="48988-1798">Container</span></span>

* <span data-ttu-id="48988-1799">Suporte adicionado para a exportação de um grupo de contêiner no formato yaml</span><span class="sxs-lookup"><span data-stu-id="48988-1799">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="48988-1800">Suporte adicionado para usar um arquivo yaml para criar/atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="48988-1800">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="48988-1801">Extensão</span><span class="sxs-lookup"><span data-stu-id="48988-1801">Extension</span></span>

* <span data-ttu-id="48988-1802">Remoção de extensões melhorada</span><span class="sxs-lookup"><span data-stu-id="48988-1802">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="48988-1803">Interativo</span><span class="sxs-lookup"><span data-stu-id="48988-1803">Interactive</span></span>

* <span data-ttu-id="48988-1804">Log de alterações alterado para silenciar o analisador para conclusões</span><span class="sxs-lookup"><span data-stu-id="48988-1804">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="48988-1805">Manipulação aprimorada de caches de ajuda inválida</span><span class="sxs-lookup"><span data-stu-id="48988-1805">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="48988-1806">KeyVault</span><span class="sxs-lookup"><span data-stu-id="48988-1806">KeyVault</span></span>

* <span data-ttu-id="48988-1807">Comandos de keyvault corrigidos para trabalhar no cloud shell ou VMs com identidade</span><span class="sxs-lookup"><span data-stu-id="48988-1807">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="48988-1808">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-1808">Network</span></span>

* <span data-ttu-id="48988-1809">Corrija o problema em que `network watcher show-topology` não funcionará com o nome de rede virtual e/ou sub-rede [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="48988-1809">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="48988-1810">Corrija o problema onde alguns comandos `network watcher` iriam declarar que o Observador de Rede não está habilitado para regiões quando na verdade é [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="48988-1810">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="48988-1811">SQL</span><span class="sxs-lookup"><span data-stu-id="48988-1811">SQL</span></span>

* <span data-ttu-id="48988-1812">[ALTERAÇÃO SIGNIFICATIVA] Objetos de resposta alterados retornados dos comandos `db` e `dw`:</span><span class="sxs-lookup"><span data-stu-id="48988-1812">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="48988-1813">A propriedade `serviceLevelObjective` foi renomeada para `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="48988-1813">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="48988-1814">As propriedades `currentServiceObjectiveId` e `requestedServiceObjectiveId` foram removidas</span><span class="sxs-lookup"><span data-stu-id="48988-1814">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="48988-1815">A propriedade `maxSizeBytes` foi alterada para ser um valor inteiro em vez de uma cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="48988-1815">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="48988-1816">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `db` e `dw` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="48988-1816">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="48988-1817">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="48988-1817">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="48988-1818">Para atualizar, use o parâmetro `--service-objective` ou defina a propriedade `sku.name`</span><span class="sxs-lookup"><span data-stu-id="48988-1818">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="48988-1819">`edition`.</span><span class="sxs-lookup"><span data-stu-id="48988-1819">`edition`.</span></span> <span data-ttu-id="48988-1820">Para atualizar, use o parâmetro `--edition` ou defina a propriedade `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="48988-1820">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="48988-1821">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="48988-1821">`elasticPoolName`.</span></span> <span data-ttu-id="48988-1822">Para atualizar, use o parâmetro `--elastic-pool` ou defina a propriedade `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="48988-1822">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="48988-1823">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `elastic-pool` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="48988-1823">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="48988-1824">`edition`.</span><span class="sxs-lookup"><span data-stu-id="48988-1824">`edition`.</span></span> <span data-ttu-id="48988-1825">Para atualizar, use o parâmetro `--edition`</span><span class="sxs-lookup"><span data-stu-id="48988-1825">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="48988-1826">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="48988-1826">`dtu`.</span></span> <span data-ttu-id="48988-1827">Para atualizar, use o parâmetro `--capacity`</span><span class="sxs-lookup"><span data-stu-id="48988-1827">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="48988-1828">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="48988-1828">`databaseDtuMin`.</span></span> <span data-ttu-id="48988-1829">Para atualizar, use o parâmetro `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="48988-1829">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="48988-1830">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="48988-1830">`databaseDtuMax`.</span></span> <span data-ttu-id="48988-1831">Para atualizar, use o parâmetro `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="48988-1831">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="48988-1832">Os parâmetros `--family` e `--capacity` foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="48988-1832">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="48988-1833">Os formatadores de tabela foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="48988-1833">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="48988-1834">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48988-1834">Storage</span></span>

* <span data-ttu-id="48988-1835">Complemento adicionado ao argumento `--account-name`</span><span class="sxs-lookup"><span data-stu-id="48988-1835">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="48988-1836">O problema com `storage entity query` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="48988-1836">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="48988-1837">VM</span><span class="sxs-lookup"><span data-stu-id="48988-1837">VM</span></span>

* <span data-ttu-id="48988-1838">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="48988-1838">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="48988-1839">O mesmo suporte pode ser acessado por meio de `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="48988-1839">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="48988-1840">Imagem de extensão fixa correspondente em `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="48988-1840">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="48988-1841">`--boot-diagnostics-storage` foi adicionado a `vm create` para capturar o log de inicialização</span><span class="sxs-lookup"><span data-stu-id="48988-1841">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="48988-1842">`--license-type` foi adicionado a `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="48988-1842">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="48988-1843">7 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="48988-1843">May 7, 2018</span></span>

<span data-ttu-id="48988-1844">Versão 2.0.32</span><span class="sxs-lookup"><span data-stu-id="48988-1844">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="48988-1845">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48988-1845">Core</span></span>

* <span data-ttu-id="48988-1846">Foi corrigida uma exceção sem tratamento ao recuperar segredos de uma conta de entidade de serviço com certificado</span><span class="sxs-lookup"><span data-stu-id="48988-1846">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="48988-1847">Adicionado suporte limitado para argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="48988-1847">Added limited support for positional arguments</span></span>
* <span data-ttu-id="48988-1848">Corrigir problema no qual `--query` não pôde ser usado com `--ids`.</span><span class="sxs-lookup"><span data-stu-id="48988-1848">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="48988-1849">#5591</span><span class="sxs-lookup"><span data-stu-id="48988-1849">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="48988-1850">Foram melhorados os cenários de redirecionamento de comandos ao usar `--ids`.</span><span class="sxs-lookup"><span data-stu-id="48988-1850">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="48988-1851">Oferece suporte a `-o tsv` com uma consulta especificada ou `-o json` sem especificar uma consulta</span><span class="sxs-lookup"><span data-stu-id="48988-1851">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="48988-1852">Foram adicionadas sugestões de comando sobre o erro se os usuários cometeram algum erro de digitação em seus comandos</span><span class="sxs-lookup"><span data-stu-id="48988-1852">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="48988-1853">Erro corrigido quando os usuários digitam `az ''`</span><span class="sxs-lookup"><span data-stu-id="48988-1853">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="48988-1854">Foram adicionados tipos de recursos personalizados com suporte para módulos de comando e extensões</span><span class="sxs-lookup"><span data-stu-id="48988-1854">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="48988-1855">ACR</span><span class="sxs-lookup"><span data-stu-id="48988-1855">ACR</span></span>

* <span data-ttu-id="48988-1856">Foram adicionados comandos de compilação de ACR</span><span class="sxs-lookup"><span data-stu-id="48988-1856">Added ACR Build commands</span></span>
* <span data-ttu-id="48988-1857">O recurso aprimorado não encontrou mensagens de erro</span><span class="sxs-lookup"><span data-stu-id="48988-1857">Improved resource not found error messages</span></span>
* <span data-ttu-id="48988-1858">Desempenho de criação de recurso aprimorado e tratamento de erros</span><span class="sxs-lookup"><span data-stu-id="48988-1858">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="48988-1859">Logon de acr aprimorado em consoles não padrão e WSL</span><span class="sxs-lookup"><span data-stu-id="48988-1859">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="48988-1860">Mensagens de erro de comandos de repositório aprimoradas</span><span class="sxs-lookup"><span data-stu-id="48988-1860">Improved repository commands error messages</span></span>
* <span data-ttu-id="48988-1861">Colunas de tabela e ordenação atualizadas</span><span class="sxs-lookup"><span data-stu-id="48988-1861">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="48988-1862">ACS</span><span class="sxs-lookup"><span data-stu-id="48988-1862">ACS</span></span>

* <span data-ttu-id="48988-1863">Foi adicionado um aviso informando que `az aks` é um serviço de versão prévia</span><span class="sxs-lookup"><span data-stu-id="48988-1863">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="48988-1864">Foi corrigido um problema de permissão em `aks install-connector` quando `--aci-resource-group` não for especificado</span><span class="sxs-lookup"><span data-stu-id="48988-1864">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="48988-1865">AMS</span><span class="sxs-lookup"><span data-stu-id="48988-1865">AMS</span></span>

* <span data-ttu-id="48988-1866">Versão inicial — Gerenciar recursos dos Serviços de Mídia do Azure</span><span class="sxs-lookup"><span data-stu-id="48988-1866">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="48988-1867">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-1867">Appservice</span></span>

* <span data-ttu-id="48988-1868">Correção de bug no `webapp delete` quando `--slot` é fornecido</span><span class="sxs-lookup"><span data-stu-id="48988-1868">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="48988-1869">`--runtime-version` foi removido de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="48988-1869">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="48988-1870">Foi adicionado suporte para min\_tls\_versão e https2.0</span><span class="sxs-lookup"><span data-stu-id="48988-1870">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="48988-1871">Suporte adicionado para vários contêineres</span><span class="sxs-lookup"><span data-stu-id="48988-1871">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="48988-1872">Lote AI</span><span class="sxs-lookup"><span data-stu-id="48988-1872">Batch AI</span></span>

* <span data-ttu-id="48988-1873">O `batchai create cluster` foi alterado para respeitar a prioridade de VM configurada no arquivo de configuração do cluster</span><span class="sxs-lookup"><span data-stu-id="48988-1873">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="48988-1874">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="48988-1874">Cognitive Services</span></span>

* <span data-ttu-id="48988-1875">Foi corrigido um erro de digitação no exemplo para `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="48988-1875">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="48988-1876">Consumo</span><span class="sxs-lookup"><span data-stu-id="48988-1876">Consumption</span></span>

* <span data-ttu-id="48988-1877">Foram adicionados novos comandos para a API de orçamento</span><span class="sxs-lookup"><span data-stu-id="48988-1877">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="48988-1878">Contêiner</span><span class="sxs-lookup"><span data-stu-id="48988-1878">Container</span></span>

* <span data-ttu-id="48988-1879">Requisito removido para `--registry-server` e `container create` quando um servidor de registro estiver incluído no nome da imagem</span><span class="sxs-lookup"><span data-stu-id="48988-1879">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="48988-1880">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="48988-1880">Cosmos DB</span></span>

* <span data-ttu-id="48988-1881">Introdução ao suporte de rede virtual para a CLI do Azure — Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="48988-1881">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="48988-1882">DMS</span><span class="sxs-lookup"><span data-stu-id="48988-1882">DMS</span></span>

* <span data-ttu-id="48988-1883">Versão inicial — Adiciona suporte ao SQL para o cenário de migração do SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="48988-1883">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="48988-1884">Extensão</span><span class="sxs-lookup"><span data-stu-id="48988-1884">Extension</span></span>

* <span data-ttu-id="48988-1885">Correção do bug em que os metadados de extensão pararam de ser exibidos</span><span class="sxs-lookup"><span data-stu-id="48988-1885">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="48988-1886">Interativo</span><span class="sxs-lookup"><span data-stu-id="48988-1886">Interactive</span></span>

* <span data-ttu-id="48988-1887">Permitir que complementos interativos funcionem com argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="48988-1887">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="48988-1888">Resultado mais simplificado quando os usuários digitam '\'</span><span class="sxs-lookup"><span data-stu-id="48988-1888">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="48988-1889">Conclusões corrigidas para parâmetros sem ajuda</span><span class="sxs-lookup"><span data-stu-id="48988-1889">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="48988-1890">Descrições corrigidas para grupos de comando</span><span class="sxs-lookup"><span data-stu-id="48988-1890">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="48988-1891">Laboratório</span><span class="sxs-lookup"><span data-stu-id="48988-1891">Lab</span></span>

* <span data-ttu-id="48988-1892">Regressões corrigidas de conversão de aptidão</span><span class="sxs-lookup"><span data-stu-id="48988-1892">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="48988-1893">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-1893">Network</span></span>

* <span data-ttu-id="48988-1894">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--ids` removido de:</span><span class="sxs-lookup"><span data-stu-id="48988-1894">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="48988-1895">Perfil</span><span class="sxs-lookup"><span data-stu-id="48988-1895">Profile</span></span>

* <span data-ttu-id="48988-1896">Detecção de origem do `disk create` corrigida</span><span class="sxs-lookup"><span data-stu-id="48988-1896">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="48988-1897">[ALTERAÇÃO SIGNIFICATIVA] `--msi-port` e `--identity-port` removidos porque não são mais usados</span><span class="sxs-lookup"><span data-stu-id="48988-1897">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="48988-1898">Erro de digitação corrigido no resumo do `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="48988-1898">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="48988-1899">Redis</span><span class="sxs-lookup"><span data-stu-id="48988-1899">Redis</span></span>

* <span data-ttu-id="48988-1900">`redis patch-schedule patch-schedule show` preterido em favor de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="48988-1900">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="48988-1901">`redis list-all` preterido.</span><span class="sxs-lookup"><span data-stu-id="48988-1901">Deprecated `redis list-all`.</span></span> <span data-ttu-id="48988-1902">Esta funcionalidade foi dobrada em `redis list`</span><span class="sxs-lookup"><span data-stu-id="48988-1902">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="48988-1903">`redis import-method` preterido em favor de `redis import`</span><span class="sxs-lookup"><span data-stu-id="48988-1903">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="48988-1904">Foi adicionado suporte a `--ids` para vários comandos</span><span class="sxs-lookup"><span data-stu-id="48988-1904">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="48988-1905">Função</span><span class="sxs-lookup"><span data-stu-id="48988-1905">Role</span></span>

* <span data-ttu-id="48988-1906">[ALTERAÇÃO SIGNIFICATIVA] Remoção de `ad sp reset-credentials` preterido</span><span class="sxs-lookup"><span data-stu-id="48988-1906">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="48988-1907">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48988-1907">Storage</span></span>

* <span data-ttu-id="48988-1908">Permitir que o token SAS de destino aplique na origem a cópia do blob se a SAS de origem e a chave de conta não forem especificadas</span><span class="sxs-lookup"><span data-stu-id="48988-1908">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="48988-1909">Exposto -- tempo limite do soquete para carregamentos e downloads de blobs</span><span class="sxs-lookup"><span data-stu-id="48988-1909">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="48988-1910">Tratar os nomes de blobs que começam com separadores de caminho como caminhos relativos</span><span class="sxs-lookup"><span data-stu-id="48988-1910">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="48988-1911">Permitir `storage blob copy --source-sas` com a inicialização char de consulta, '?'</span><span class="sxs-lookup"><span data-stu-id="48988-1911">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="48988-1912">`storage entity query --marker` foi corrigido para aceitar a lista de chaves = valores</span><span class="sxs-lookup"><span data-stu-id="48988-1912">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="48988-1913">VM</span><span class="sxs-lookup"><span data-stu-id="48988-1913">VM</span></span>

* <span data-ttu-id="48988-1914">Uma lógica de detecção inválida foi corrigida no URI do blob não gerenciado</span><span class="sxs-lookup"><span data-stu-id="48988-1914">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="48988-1915">Adicionada criptografia de disco de suporte sem entidades de serviço fornecidas pelo usuário</span><span class="sxs-lookup"><span data-stu-id="48988-1915">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="48988-1916">[ALTERAÇÃO SIGNIFICATIVA] Não usar a VM 'ManagedIdentityExtension' para suporte de MSI</span><span class="sxs-lookup"><span data-stu-id="48988-1916">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="48988-1917">Suporte adicionado para a política de remoção em `vmss`</span><span class="sxs-lookup"><span data-stu-id="48988-1917">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="48988-1918">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--ids` de:</span><span class="sxs-lookup"><span data-stu-id="48988-1918">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="48988-1919">Foi adicionado suporte do acelerador de gravação</span><span class="sxs-lookup"><span data-stu-id="48988-1919">Added write accelerator support</span></span>
* <span data-ttu-id="48988-1920">Adicionado `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="48988-1920">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="48988-1921">`vm diagnostics set` foi corrigido para detectar o tipo de sistema operacional da VM de forma confiável</span><span class="sxs-lookup"><span data-stu-id="48988-1921">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="48988-1922">`vm resize` foi alterado para verificar se o tamanho solicitado é diferente daquele definido no momento e atualizar somente na alteração</span><span class="sxs-lookup"><span data-stu-id="48988-1922">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="48988-1923">10 de abril de 2018</span><span class="sxs-lookup"><span data-stu-id="48988-1923">April 10, 2018</span></span>

<span data-ttu-id="48988-1924">Versão 2.0.31</span><span class="sxs-lookup"><span data-stu-id="48988-1924">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="48988-1925">ACR</span><span class="sxs-lookup"><span data-stu-id="48988-1925">ACR</span></span>

* <span data-ttu-id="48988-1926">Melhoria do tratamento de erros do fallback do wincred</span><span class="sxs-lookup"><span data-stu-id="48988-1926">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="48988-1927">ACS</span><span class="sxs-lookup"><span data-stu-id="48988-1927">ACS</span></span>

* <span data-ttu-id="48988-1928">Alteração da validade de SPNs criados pelo AKS para 5 anos</span><span class="sxs-lookup"><span data-stu-id="48988-1928">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="48988-1929">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-1929">Appservice</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="48988-1931">Correção da exceção não identificada de planos de webapp inexistentes</span><span class="sxs-lookup"><span data-stu-id="48988-1931">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="48988-1932">BatchAI</span><span class="sxs-lookup"><span data-stu-id="48988-1932">BatchAI</span></span>

* <span data-ttu-id="48988-1933">Adição de suporte para a API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="48988-1933">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="48988-1934">Montagem de nível de trabalho</span><span class="sxs-lookup"><span data-stu-id="48988-1934">Job level mounting</span></span>
  - <span data-ttu-id="48988-1935">Variáveis de ambiente com valores secretos</span><span class="sxs-lookup"><span data-stu-id="48988-1935">Environment variables with secret values</span></span>
  - <span data-ttu-id="48988-1936">Configurações de contadores de desempenho</span><span class="sxs-lookup"><span data-stu-id="48988-1936">Performance counters settings</span></span>
  - <span data-ttu-id="48988-1937">Relatório de segmento de linha específico de trabalho</span><span class="sxs-lookup"><span data-stu-id="48988-1937">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="48988-1938">Suporte para subpastas na API de arquivos de lista</span><span class="sxs-lookup"><span data-stu-id="48988-1938">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="48988-1939">Relatório de uso e limites</span><span class="sxs-lookup"><span data-stu-id="48988-1939">Usage and limits reporting</span></span>
  - <span data-ttu-id="48988-1940">Permitir a especificação do tipo de cache para servidores NFS</span><span class="sxs-lookup"><span data-stu-id="48988-1940">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="48988-1941">Suporte para imagens personalizadas</span><span class="sxs-lookup"><span data-stu-id="48988-1941">Support for custom images</span></span>
  - <span data-ttu-id="48988-1942">Adição de suporte para o kit de ferramentas pyTorch</span><span class="sxs-lookup"><span data-stu-id="48988-1942">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="48988-1943">Adição do comando `job wait`, que permite aguardar a conclusão do trabalho e relata o código de saída de trabalho</span><span class="sxs-lookup"><span data-stu-id="48988-1943">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="48988-1944">Adição do comando `usage show` para listar o uso e os limites do IA do Lote atual para diferentes regiões</span><span class="sxs-lookup"><span data-stu-id="48988-1944">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="48988-1945">Há suporte para nuvens nacionais</span><span class="sxs-lookup"><span data-stu-id="48988-1945">National clouds are supported</span></span>
* <span data-ttu-id="48988-1946">Adição de argumentos de linha de comando do trabalho para montar sistemas de arquivos no nível de trabalho, além de arquivos de configuração</span><span class="sxs-lookup"><span data-stu-id="48988-1946">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="48988-1947">Adição de mais opções para personalizar clusters — prioridade de VM, sub-rede, contagem inicial de nós para clusters de dimensionamento automático, especificando a imagem personalizada</span><span class="sxs-lookup"><span data-stu-id="48988-1947">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="48988-1948">Adição de opção de linha de comando para especificar o tipo de cache de NFS gerenciado por IA do Lote</span><span class="sxs-lookup"><span data-stu-id="48988-1948">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="48988-1949">Simplificação da especificação do sistema de arquivos de montagem nos arquivos de configuração.</span><span class="sxs-lookup"><span data-stu-id="48988-1949">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="48988-1950">Agora é possível omitir as credenciais do Compartilhamento de arquivos do Azure e Contêineres de Blob do Azure — a CLI preencherá credenciais ausentes usando a chave da conta de armazenamento fornecida por meio dos parâmetros de linha de comando ou especificada por meio da variável de ambiente ou consultará a chave a partir do Armazenamento do Azure (se a conta de armazenamento pertencer à assinatura atual)</span><span class="sxs-lookup"><span data-stu-id="48988-1950">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="48988-1951">O comando do fluxo de arquivo de trabalho agora é preenchido automaticamente quando o trabalho é concluído (com êxito, com falha, encerrado ou excluído)</span><span class="sxs-lookup"><span data-stu-id="48988-1951">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="48988-1952">Melhoria da saída de `table` para operações de `show`</span><span class="sxs-lookup"><span data-stu-id="48988-1952">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="48988-1953">Adição da opção `--use-auto-storage` para a criação de cluster.</span><span class="sxs-lookup"><span data-stu-id="48988-1953">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="48988-1954">Essa opção simplifica o gerenciamento de contas de armazenamento e a montagem do Compartilhamento de arquivos do Azure e dos Contêineres de Blob do Azure para clusters</span><span class="sxs-lookup"><span data-stu-id="48988-1954">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="48988-1955">Adição da opção `--generate-ssh-keys` para `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="48988-1955">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="48988-1956">Adição da capacidade de fornecer a tarefa de configuração de nó por meio da linha de comando</span><span class="sxs-lookup"><span data-stu-id="48988-1956">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="48988-1957">[ALTERAÇÃO SIGNIFICATIVA] Comandos `job stream-file` e `job list-files` movidos para o grupo `job file`</span><span class="sxs-lookup"><span data-stu-id="48988-1957">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="48988-1958">[ALTERAÇÃO SIGNIFICATIVA] `--admin-user-name` renomeado para `--user-name` no comando `file-server create` para ser consistente com o comando `cluster create`</span><span class="sxs-lookup"><span data-stu-id="48988-1958">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="48988-1959">Cobrança</span><span class="sxs-lookup"><span data-stu-id="48988-1959">Billing</span></span>

* <span data-ttu-id="48988-1960">Adição de comandos da conta de registro</span><span class="sxs-lookup"><span data-stu-id="48988-1960">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="48988-1961">Consumo</span><span class="sxs-lookup"><span data-stu-id="48988-1961">Consumption</span></span>

* <span data-ttu-id="48988-1962">Adicionados os comandos `marketplace`</span><span class="sxs-lookup"><span data-stu-id="48988-1962">Added `marketplace` commands</span></span>
* <span data-ttu-id="48988-1963">[ALTERAÇÃO SIGNIFICATIVA] `reservations summaries` renomeado para `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="48988-1963">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="48988-1964">[ALTERAÇÃO SIGNIFICATIVA] `reservations details` renomeado para `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="48988-1964">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="48988-1965">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--reservation-order-id` e `--reservation-id` para os comandos `reservation`</span><span class="sxs-lookup"><span data-stu-id="48988-1965">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="48988-1966">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--grain` para os comandos `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="48988-1966">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="48988-1967">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--include-meter-details` para os comandos `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="48988-1967">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="48988-1968">Contêiner</span><span class="sxs-lookup"><span data-stu-id="48988-1968">Container</span></span>

* <span data-ttu-id="48988-1969">Adição dos parâmetros de montagem de volume de repositório git `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` e `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="48988-1969">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="48988-1970">Correção de [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` com falha com --container-name especificado</span><span class="sxs-lookup"><span data-stu-id="48988-1970">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="48988-1971">Extensão</span><span class="sxs-lookup"><span data-stu-id="48988-1971">Extension</span></span>

* <span data-ttu-id="48988-1972">Alteração da mensagem de verificação de distribuição para ser de nível de depuração</span><span class="sxs-lookup"><span data-stu-id="48988-1972">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="48988-1973">Interativo</span><span class="sxs-lookup"><span data-stu-id="48988-1973">Interactive</span></span>

* <span data-ttu-id="48988-1974">Alteração para interromper as conclusões após comandos não reconhecidos</span><span class="sxs-lookup"><span data-stu-id="48988-1974">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="48988-1975">Adição de ganchos de eventos antes e depois da criação da subárvore do comando</span><span class="sxs-lookup"><span data-stu-id="48988-1975">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="48988-1976">Adição de conclusão para parâmetros `--ids`</span><span class="sxs-lookup"><span data-stu-id="48988-1976">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="48988-1977">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-1977">Network</span></span>

* <span data-ttu-id="48988-1978">Correção de [#5936](https://github.com/Azure/azure-cli/issues/5936): as marcas `application-gateway create` não podiam ser definidas</span><span class="sxs-lookup"><span data-stu-id="48988-1978">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="48988-1979">Adição do argumento `--auth-certs` para anexar certificados de autenticação para `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="48988-1979">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="48988-1980">#4910</span><span class="sxs-lookup"><span data-stu-id="48988-1980">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="48988-1981">Adição dos comandos `ddos-protection` para criar planos de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="48988-1981">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="48988-1982">Adição de suporte de `--ddos-protection-plan` a `vnet [create|update]` para associar uma VNET a um plano de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="48988-1982">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="48988-1983">Correção do problema com o sinalizador `--disable-bgp-route-propagation` em `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48988-1983">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="48988-1984">Remoção de argumentos fictícios `--public-ip-address-type` e `--subnet-type` para `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48988-1984">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="48988-1985">Adição de suporte para registros TXT com sequências de escape RFC 1035 para `network dns zone [import|export]` e `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="48988-1985">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="48988-1986">Perfil</span><span class="sxs-lookup"><span data-stu-id="48988-1986">Profile</span></span>

* <span data-ttu-id="48988-1987">Adição de suporte para contas clássicas do Azure em `account list`</span><span class="sxs-lookup"><span data-stu-id="48988-1987">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="48988-1988">[ALTERAÇÃO SIGNIFICATIVA] Remoção dos argumentos `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="48988-1988">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="48988-1989">RDBMS</span><span class="sxs-lookup"><span data-stu-id="48988-1989">RDBMS</span></span>

* <span data-ttu-id="48988-1990">Adicionado o comando `georestore`</span><span class="sxs-lookup"><span data-stu-id="48988-1990">Added `georestore` command</span></span>
* <span data-ttu-id="48988-1991">Remoção da restrição de tamanho de armazenamento do comando `create`</span><span class="sxs-lookup"><span data-stu-id="48988-1991">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="48988-1992">Recurso</span><span class="sxs-lookup"><span data-stu-id="48988-1992">Resource</span></span>

* <span data-ttu-id="48988-1993">Adicionado o suporte ao `--metadata` para `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="48988-1993">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="48988-1994">Adição de suporte para `--metadata`, `--set`, `--add`, `--remove` para `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="48988-1994">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="48988-1995">SQL</span><span class="sxs-lookup"><span data-stu-id="48988-1995">SQL</span></span>

* <span data-ttu-id="48988-1996">Adição de `sql elastic-pool op list` e `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="48988-1996">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="48988-1997">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48988-1997">Storage</span></span>

* <span data-ttu-id="48988-1998">Melhoria de mensagens de erro para cadeias de conexão malformadas</span><span class="sxs-lookup"><span data-stu-id="48988-1998">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="48988-1999">VM</span><span class="sxs-lookup"><span data-stu-id="48988-1999">VM</span></span>

* <span data-ttu-id="48988-2000">Adição de suporte para configurar a contagem de domínios de falha da plataforma para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="48988-2000">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="48988-2001">Alteração de `vmss create` para balanceador de carga padrão para um conjunto de dimensionamento desabilitado zonal, grande ou de único grupo de posicionamento</span><span class="sxs-lookup"><span data-stu-id="48988-2001">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [ALTERAÇÃO SIGNIFICATIVA]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="48988-2003">Adição de suporte para a SKU de IP público para `vm create`</span><span class="sxs-lookup"><span data-stu-id="48988-2003">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="48988-2004">Adição dos argumentos `--keyvault` e `--resource-group` para `vm secret format` para oferecer suporte a cenários em que o comando não é capaz de resolver a ID do cofre.</span><span class="sxs-lookup"><span data-stu-id="48988-2004">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="48988-2005">#5718</span><span class="sxs-lookup"><span data-stu-id="48988-2005">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="48988-2006">Melhoria de erros de `[vm|vmss create]` quando um local do grupo de recursos não tem suporte de zona</span><span class="sxs-lookup"><span data-stu-id="48988-2006">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="48988-2007">27 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="48988-2007">March 27, 2018</span></span>

<span data-ttu-id="48988-2008">Versão 2.0.30</span><span class="sxs-lookup"><span data-stu-id="48988-2008">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="48988-2009">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48988-2009">Core</span></span>

* <span data-ttu-id="48988-2010">Mostrar mensagem para extensões marcadas como versão prévia na Ajuda</span><span class="sxs-lookup"><span data-stu-id="48988-2010">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="48988-2011">ACS</span><span class="sxs-lookup"><span data-stu-id="48988-2011">ACS</span></span>

* <span data-ttu-id="48988-2012">Corrija o erro de verificação de certificado SSL para `aks install-cli` no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="48988-2012">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="48988-2013">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-2013">Appservice</span></span>

* <span data-ttu-id="48988-2014">Adição do suporte somente para HTTPS para `webapp update`</span><span class="sxs-lookup"><span data-stu-id="48988-2014">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="48988-2015">Adição do suporte para os slots `az webapp identity [assign|show]` e `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="48988-2015">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="48988-2016">Backup</span><span class="sxs-lookup"><span data-stu-id="48988-2016">Backup</span></span>

* <span data-ttu-id="48988-2017">Adição do novo comando `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="48988-2017">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="48988-2018">Esse comando pode ser usado para verificar se o backup de uma VM é realizado por qualquer cofre na assinatura</span><span class="sxs-lookup"><span data-stu-id="48988-2018">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="48988-2019">Habilitação das IDs de objeto do Azure para os parâmetros `--resource-group` e `--vault-name` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="48988-2019">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="48988-2020">`--name` parâmetros alterados a fim de aceitar o formato de saída dos comandos `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="48988-2020">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="48988-2021">Contêiner</span><span class="sxs-lookup"><span data-stu-id="48988-2021">Container</span></span>

* <span data-ttu-id="48988-2022">Adição do comando `container exec`.</span><span class="sxs-lookup"><span data-stu-id="48988-2022">Added `container exec` command.</span></span> <span data-ttu-id="48988-2023">Executa comandos em um contêiner para um grupo de contêiner em execução</span><span class="sxs-lookup"><span data-stu-id="48988-2023">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="48988-2024">Permitir a saída da tabela para criar e atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="48988-2024">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="48988-2025">Extensão</span><span class="sxs-lookup"><span data-stu-id="48988-2025">Extension</span></span>

* <span data-ttu-id="48988-2026">Mensagem adicionada para `extension add`, se a extensão estiver no modo de versão prévia</span><span class="sxs-lookup"><span data-stu-id="48988-2026">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="48988-2027">`extension list-available` alterado para mostrar dados de extensão total com `--show-details`</span><span class="sxs-lookup"><span data-stu-id="48988-2027">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="48988-2028">[ALTERAÇÃO SIGNIFICATIVA] `extension list-available` alterado para mostrar dados de extensão simplificados por padrão</span><span class="sxs-lookup"><span data-stu-id="48988-2028">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="48988-2029">Interativo</span><span class="sxs-lookup"><span data-stu-id="48988-2029">Interactive</span></span>

* <span data-ttu-id="48988-2030">Alteração nas conclusões para ativar após a conclusão do carregamento da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="48988-2030">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="48988-2031">Correção de bug usando o parâmetro `--style`</span><span class="sxs-lookup"><span data-stu-id="48988-2031">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="48988-2032">Analisador léxico interativo instanciado após a falta do despejo da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="48988-2032">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="48988-2033">Suporte aprimorado ao completador</span><span class="sxs-lookup"><span data-stu-id="48988-2033">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="48988-2034">Laboratório</span><span class="sxs-lookup"><span data-stu-id="48988-2034">Lab</span></span>

* <span data-ttu-id="48988-2035">Correção de bugs com o comando `create environment`</span><span class="sxs-lookup"><span data-stu-id="48988-2035">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="48988-2036">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="48988-2036">Monitor</span></span>

* <span data-ttu-id="48988-2037">Adição de suporte para `--top`, `--orderby` e `--namespace` para `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="48988-2037">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="48988-2038">Corrigido [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` aceita uma lista separada por espaços de métricas para recuperação</span><span class="sxs-lookup"><span data-stu-id="48988-2038">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="48988-2039">Adição de suporte para `--namespace` para `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="48988-2039">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="48988-2040">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-2040">Network</span></span>

* <span data-ttu-id="48988-2041">Adição de suporte para zonas DNS privado</span><span class="sxs-lookup"><span data-stu-id="48988-2041">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="48988-2042">Perfil</span><span class="sxs-lookup"><span data-stu-id="48988-2042">Profile</span></span>

* <span data-ttu-id="48988-2043">Adição de avisos para `--identity-port` e `--msi-port` para `login`</span><span class="sxs-lookup"><span data-stu-id="48988-2043">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="48988-2044">RDBMS</span><span class="sxs-lookup"><span data-stu-id="48988-2044">RDBMS</span></span>

* <span data-ttu-id="48988-2045">Adição de modelo de negócios GA API versão 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="48988-2045">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="48988-2046">Recurso</span><span class="sxs-lookup"><span data-stu-id="48988-2046">Resource</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="48988-2048">Função</span><span class="sxs-lookup"><span data-stu-id="48988-2048">Role</span></span>

* <span data-ttu-id="48988-2049">Adição de suporte para configurações de acesso necessário e clientes nativos para `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="48988-2049">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="48988-2050">`rbac` comandos alterados para retornar menos de 1000 IDs na resolução do objeto</span><span class="sxs-lookup"><span data-stu-id="48988-2050">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="48988-2051">Adição de comandos de gerenciamento de credencial `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="48988-2051">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="48988-2052">[ALTERAÇÃO SIGNIFICATIVA] "Propriedades" removidas da saída `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="48988-2052">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="48988-2053">Adição de suporte para as permissões `dataActions` e `notDataActions` para `role definition`</span><span class="sxs-lookup"><span data-stu-id="48988-2053">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="48988-2054">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48988-2054">Storage</span></span>

* <span data-ttu-id="48988-2055">Correção de problema ao carregar um arquivo com tamanho entre 195 e 200 GB</span><span class="sxs-lookup"><span data-stu-id="48988-2055">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="48988-2056">Corrigido [#4049](https://github.com/Azure/azure-cli/issues/4049): problemas com o acréscimo de uploads de blob ignorando os parâmetros da condição</span><span class="sxs-lookup"><span data-stu-id="48988-2056">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="48988-2057">VM</span><span class="sxs-lookup"><span data-stu-id="48988-2057">VM</span></span>

* <span data-ttu-id="48988-2058">Adição de aviso para `vmss create` para alterações de falha futuras para conjuntos com mais de 100 instâncias</span><span class="sxs-lookup"><span data-stu-id="48988-2058">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="48988-2059">Adição de suporte com flexibilidade de região para `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="48988-2059">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="48988-2060">Alteração no modo de exibição de instância de disco para reportar status de criptografia mais adequados</span><span class="sxs-lookup"><span data-stu-id="48988-2060">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="48988-2061">[ALTERAÇÃO SIGNIFICATIVA] `vm extension delete` alterado para não retornar mais a saída</span><span class="sxs-lookup"><span data-stu-id="48988-2061">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="48988-2062">13 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="48988-2062">March 13, 2018</span></span>

<span data-ttu-id="48988-2063">Versão 2.0.29</span><span class="sxs-lookup"><span data-stu-id="48988-2063">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="48988-2064">ACR</span><span class="sxs-lookup"><span data-stu-id="48988-2064">ACR</span></span>

* <span data-ttu-id="48988-2065">Suporte adicionado do parâmetro `--image` a `repository delete`</span><span class="sxs-lookup"><span data-stu-id="48988-2065">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="48988-2066">Parâmetros `--manifest` e `--tag` preteridos do comando `repository delete`</span><span class="sxs-lookup"><span data-stu-id="48988-2066">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="48988-2067">Comando `repository untag` adicionado para remover uma marcação sem excluir dados</span><span class="sxs-lookup"><span data-stu-id="48988-2067">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="48988-2068">ACS</span><span class="sxs-lookup"><span data-stu-id="48988-2068">ACS</span></span>

* <span data-ttu-id="48988-2069">Comando `aks upgrade-connector` adicionado para atualizar um conector existente</span><span class="sxs-lookup"><span data-stu-id="48988-2069">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="48988-2070">Arquivos de configuração `kubectl` alterados para usar um YAML mais legível em bloco</span><span class="sxs-lookup"><span data-stu-id="48988-2070">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="48988-2071">Supervisor</span><span class="sxs-lookup"><span data-stu-id="48988-2071">Advisor</span></span>

* <span data-ttu-id="48988-2072">[ALTERAÇÃO SIGNIFICATIVA] `advisor configuration get` renomeado para `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="48988-2072">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="48988-2073">[ALTERAÇÃO SIGNIFICATIVA] `advisor configuration set` renomeado para `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="48988-2073">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="48988-2074">[ALTERAÇÃO SIGNIFICATIVA] `advisor recommendation generate` removido</span><span class="sxs-lookup"><span data-stu-id="48988-2074">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="48988-2075">Parâmetro `--refresh` adicionado a `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="48988-2075">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="48988-2076">Adicionado o comando `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="48988-2076">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="48988-2077">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-2077">Appservice</span></span>

* <span data-ttu-id="48988-2078">Preterido `[webapp|functionapp] assign-identity`</span><span class="sxs-lookup"><span data-stu-id="48988-2078">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="48988-2079">Comandos de identidade gerenciada `webapp identity [assign|show]` e `functionapp identity [assign|show]` adicionados</span><span class="sxs-lookup"><span data-stu-id="48988-2079">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="48988-2080">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="48988-2080">Eventhubs</span></span>

* <span data-ttu-id="48988-2081">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="48988-2081">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="48988-2082">Extensão</span><span class="sxs-lookup"><span data-stu-id="48988-2082">Extension</span></span>

* <span data-ttu-id="48988-2083">Verificação adicionada para avisar ao usuário se a distribuição usada é diferente da armazenado no arquivo de origem do pacote, pois isso pode levar a erros</span><span class="sxs-lookup"><span data-stu-id="48988-2083">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="48988-2084">Interativo</span><span class="sxs-lookup"><span data-stu-id="48988-2084">Interactive</span></span>

* <span data-ttu-id="48988-2085">Corrigido [#5625](https://github.com/Azure/azure-cli/issues/5625): manter histórico em sessões diferentes</span><span class="sxs-lookup"><span data-stu-id="48988-2085">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="48988-2086">Corrigido [#3016](https://github.com/Azure/azure-cli/issues/3016): histórico não registrado no escopo</span><span class="sxs-lookup"><span data-stu-id="48988-2086">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="48988-2087">Corrigido [#5688](https://github.com/Azure/azure-cli/issues/5688): as conclusões não aparecerão se o carregamento da tabela de comando encontrar uma exceção</span><span class="sxs-lookup"><span data-stu-id="48988-2087">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="48988-2088">Medidor de progresso corrigido para operações de longa execução</span><span class="sxs-lookup"><span data-stu-id="48988-2088">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="48988-2089">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="48988-2089">Monitor</span></span>

* <span data-ttu-id="48988-2090">Comandos `monitor autoscale-settings` preteridos</span><span class="sxs-lookup"><span data-stu-id="48988-2090">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="48988-2091">Adicionados os comandos `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="48988-2091">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="48988-2092">Adicionados os comandos `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="48988-2092">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="48988-2093">Adicionados os comandos `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="48988-2093">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="48988-2094">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-2094">Network</span></span>

* <span data-ttu-id="48988-2095">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--tags` removido de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="48988-2095">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="48988-2096">Valores padrão incorretos removidos dos seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="48988-2096">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="48988-2097">Comandos `network watcher connection-monitor` adicionados</span><span class="sxs-lookup"><span data-stu-id="48988-2097">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="48988-2098">Parâmetros `--vnet` e `--subnet` adicionados a `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="48988-2098">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="48988-2099">Perfil</span><span class="sxs-lookup"><span data-stu-id="48988-2099">Profile</span></span>

* <span data-ttu-id="48988-2100">Parâmetro `--msi` preterido de `az login`</span><span class="sxs-lookup"><span data-stu-id="48988-2100">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="48988-2101">Parâmetro `--identity` adicionado de `az login` para substituir `--msi`</span><span class="sxs-lookup"><span data-stu-id="48988-2101">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="48988-2102">RDBMS</span><span class="sxs-lookup"><span data-stu-id="48988-2102">RDBMS</span></span>

* <span data-ttu-id="48988-2103">[VISUALIZAÇÃO] Alterado para usar a API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="48988-2103">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="48988-2104">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="48988-2104">Service Bus</span></span>

* <span data-ttu-id="48988-2105">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="48988-2105">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="48988-2106">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48988-2106">Storage</span></span>

* <span data-ttu-id="48988-2107">[#4971](https://github.com/Azure/azure-cli/issues/4971) corrigido: `storage blob copy` agora dá suporte a outras nuvens do Azure</span><span class="sxs-lookup"><span data-stu-id="48988-2107">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="48988-2108">Corrigido [#5286](https://github.com/Azure/azure-cli/issues/5286): os comandos em lotes `storage blob [delete-batch|download-batch|upload-batch]` não geram mais um erro após falhas da pré-condição</span><span class="sxs-lookup"><span data-stu-id="48988-2108">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="48988-2109">VM</span><span class="sxs-lookup"><span data-stu-id="48988-2109">VM</span></span>

* <span data-ttu-id="48988-2110">Suporte adicionado a `[vm|vmss] create` anexar discos de dados não gerenciados e configurar o cache</span><span class="sxs-lookup"><span data-stu-id="48988-2110">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="48988-2111">`[vm|vmss] assign-identity` e `[vm|vmss] remove-identity` preteridos</span><span class="sxs-lookup"><span data-stu-id="48988-2111">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="48988-2112">Comandos `vm identity [assign|remove|show]` e `vmss identity [assign|remove|show]` adicionados para substituir comandos preteridos</span><span class="sxs-lookup"><span data-stu-id="48988-2112">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="48988-2113">Prioridade padrão alterada em `vmss create` para None</span><span class="sxs-lookup"><span data-stu-id="48988-2113">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="48988-2114">27 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="48988-2114">February 27, 2018</span></span>

<span data-ttu-id="48988-2115">Versão 2.0.28</span><span class="sxs-lookup"><span data-stu-id="48988-2115">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="48988-2116">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48988-2116">Core</span></span>

* <span data-ttu-id="48988-2117">Corrigido [#5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="48988-2117">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="48988-2118">Adição de suporte para telemetria de extensão com chaves personalizadas</span><span class="sxs-lookup"><span data-stu-id="48988-2118">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="48988-2119">Adição de log HTTP em `--debug`</span><span class="sxs-lookup"><span data-stu-id="48988-2119">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="48988-2120">ACS</span><span class="sxs-lookup"><span data-stu-id="48988-2120">ACS</span></span>

* <span data-ttu-id="48988-2121">Alteração para usa o gráfico `virtual-kubelet-for-aks` do Helm para `aks install-connector` por padrão</span><span class="sxs-lookup"><span data-stu-id="48988-2121">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="48988-2122">Problema corrigido: permissão insuficiente para entidades de serviço criarem um grupo de contêiner ACI</span><span class="sxs-lookup"><span data-stu-id="48988-2122">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="48988-2123">Adição dos parâmetros `--aci-container-group`, `--location` e `--image-tag` ao `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="48988-2123">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="48988-2124">Remoção do aviso de reprovação de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="48988-2124">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="48988-2125">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-2125">Appservice</span></span>

* <span data-ttu-id="48988-2126">Atualizações para a nova versão do SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="48988-2126">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="48988-2127">Correção [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` relatado como SKU inválido</span><span class="sxs-lookup"><span data-stu-id="48988-2127">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="48988-2128">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="48988-2128">Cognitive Services</span></span>

* <span data-ttu-id="48988-2129">Atualização do “aviso” ao criar uma nova conta dos Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="48988-2129">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="48988-2130">Consumo</span><span class="sxs-lookup"><span data-stu-id="48988-2130">Consumption</span></span>

* <span data-ttu-id="48988-2131">Adição de novos comandos para a API pricesheet</span><span class="sxs-lookup"><span data-stu-id="48988-2131">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="48988-2132">Atualização dos formatos existentes de Detalhes de uso e Detalhes de reserva</span><span class="sxs-lookup"><span data-stu-id="48988-2132">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="48988-2133">Contêiner</span><span class="sxs-lookup"><span data-stu-id="48988-2133">Container</span></span>

* <span data-ttu-id="48988-2134">Adição dos argumentos `--secrets` e `--secrets-mount-path` ao `container create` para usar segredos na ACI</span><span class="sxs-lookup"><span data-stu-id="48988-2134">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="48988-2135">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-2135">Network</span></span>

* <span data-ttu-id="48988-2136">Corrigido [#5559](https://github.com/Azure/azure-cli/issues/5559): cliente ausente em `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="48988-2136">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="48988-2137">Recurso</span><span class="sxs-lookup"><span data-stu-id="48988-2137">Resource</span></span>

* <span data-ttu-id="48988-2138">Alteração do `group deployment export` para exibir um modelo parcial e erros ao falhar</span><span class="sxs-lookup"><span data-stu-id="48988-2138">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="48988-2139">Função</span><span class="sxs-lookup"><span data-stu-id="48988-2139">Role</span></span>

* <span data-ttu-id="48988-2140">Adição de `role assignment list-changelogs` para permitir a auditoria das funções da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="48988-2140">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="48988-2141">SQL</span><span class="sxs-lookup"><span data-stu-id="48988-2141">SQL</span></span>

* <span data-ttu-id="48988-2142">Adição de suporte para a redundância de zona para os bancos de dados e pools elásticos em criação ou atualização</span><span class="sxs-lookup"><span data-stu-id="48988-2142">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="48988-2143">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48988-2143">Storage</span></span>

* <span data-ttu-id="48988-2144">Habilitação de especificação de caminho de destino/prefixo do `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="48988-2144">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="48988-2145">VM</span><span class="sxs-lookup"><span data-stu-id="48988-2145">VM</span></span>

* <span data-ttu-id="48988-2146">Adição de suporte para anexar/desanexar discos em uma instância única de VMSS</span><span class="sxs-lookup"><span data-stu-id="48988-2146">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="48988-2147">13 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="48988-2147">February 13, 2018</span></span>

<span data-ttu-id="48988-2148">Versão 2.0.27</span><span class="sxs-lookup"><span data-stu-id="48988-2148">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="48988-2149">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48988-2149">Core</span></span>

* <span data-ttu-id="48988-2150">Alterada a autenticação para chave tanto na ID de assinatura quanto no nome de logon do MSI</span><span class="sxs-lookup"><span data-stu-id="48988-2150">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="48988-2151">ACS</span><span class="sxs-lookup"><span data-stu-id="48988-2151">ACS</span></span>

* <span data-ttu-id="48988-2152">[ALTERAÇÃO SIGNIFICATIVA] `aks get-versions` renomeado para `aks get-upgrades` para fins de precisão</span><span class="sxs-lookup"><span data-stu-id="48988-2152">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="48988-2153">`aks get-versions` alterado para mostrar versões do Kubernetes disponíveis para `aks create`</span><span class="sxs-lookup"><span data-stu-id="48988-2153">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="48988-2154">Alterados os padrões de `aks create` para permitir que o servidor escolha a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="48988-2154">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="48988-2155">Atualizadas as mensagens de ajuda sobre a entidade de serviço gerada pelo AKS</span><span class="sxs-lookup"><span data-stu-id="48988-2155">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="48988-2156">Alterados os tamanhos de nó padrão para `aks create` de “Standard\_D1\_v2” para “Standard\_DS1\_v2”</span><span class="sxs-lookup"><span data-stu-id="48988-2156">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="48988-2157">Aumentada a confiabilidade ao localizar o pod de painel para `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="48988-2157">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="48988-2158">`aks get-credentials` corrigido para tratar de erros de Unicode ao carregar arquivos de configuração do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="48988-2158">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="48988-2159">Adicionada uma mensagem para `az aks install-cli` para ajudar a obter `kubectl` em `$PATH`</span><span class="sxs-lookup"><span data-stu-id="48988-2159">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="48988-2160">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-2160">Appservice</span></span>

* <span data-ttu-id="48988-2161">Corrigido o problema em que `webapp [backup|restore]` falhou devido a uma referência nula</span><span class="sxs-lookup"><span data-stu-id="48988-2161">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="48988-2162">Adicionado suporte para planos de serviço de aplicativo padrão por meio de `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="48988-2162">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="48988-2163">CDN</span><span class="sxs-lookup"><span data-stu-id="48988-2163">CDN</span></span>

* <span data-ttu-id="48988-2164">Adicionados os comandos `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="48988-2164">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="48988-2165">Contêiner</span><span class="sxs-lookup"><span data-stu-id="48988-2165">Container</span></span>

* <span data-ttu-id="48988-2166">Adicionada a opção `--follow` para `az container logs` para logs de streaming</span><span class="sxs-lookup"><span data-stu-id="48988-2166">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="48988-2167">Adicionado o comando `container attach` que anexa fluxos locais de saída e erro padrão para um contêiner em um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="48988-2167">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="48988-2168">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="48988-2168">CosmosDB</span></span>

* <span data-ttu-id="48988-2169">Adicionado suporte para a configuração de recursos</span><span class="sxs-lookup"><span data-stu-id="48988-2169">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="48988-2170">Extensão</span><span class="sxs-lookup"><span data-stu-id="48988-2170">Extension</span></span>

* <span data-ttu-id="48988-2171">Adicionado suporte para parâmetro `--pip-proxy` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="48988-2171">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="48988-2172">Adicionado suporte para argumento `--pip-extra-index-urls` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="48988-2172">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="48988-2173">Comentários</span><span class="sxs-lookup"><span data-stu-id="48988-2173">Feedback</span></span>

* <span data-ttu-id="48988-2174">Adicionadas informações de extensão aos dados de telemetria</span><span class="sxs-lookup"><span data-stu-id="48988-2174">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="48988-2175">Interativo</span><span class="sxs-lookup"><span data-stu-id="48988-2175">Interactive</span></span>

* <span data-ttu-id="48988-2176">Corrigido o problema em que o usuário é solicitado a fazer logon ao usar o modo interativo no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="48988-2176">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="48988-2177">Corrigida a regressão com conclusões de parâmetro ausentes</span><span class="sxs-lookup"><span data-stu-id="48988-2177">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="48988-2178">IoT</span><span class="sxs-lookup"><span data-stu-id="48988-2178">IoT</span></span>

* <span data-ttu-id="48988-2179">Correção do problema em que `iot dps access policy [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="48988-2179">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="48988-2180">Correção do problema em que `iot dps linked-hub [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="48988-2180">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="48988-2181">Adicionado o suporte `--no-wait` para `iot dps access policy [create|update]` e `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48988-2181">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="48988-2182">`iot hub create` alterado para permitir a especificação do número de partições</span><span class="sxs-lookup"><span data-stu-id="48988-2182">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="48988-2183">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="48988-2183">Monitor</span></span>

* <span data-ttu-id="48988-2184">Corrigido o comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="48988-2184">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="48988-2185">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-2185">Network</span></span>

* <span data-ttu-id="48988-2186">Corrigida a opção `--tags` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="48988-2186">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="48988-2187">Perfil</span><span class="sxs-lookup"><span data-stu-id="48988-2187">Profile</span></span>

* <span data-ttu-id="48988-2188">`az login` habilitado no modo interativo</span><span class="sxs-lookup"><span data-stu-id="48988-2188">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="48988-2189">Recurso</span><span class="sxs-lookup"><span data-stu-id="48988-2189">Resource</span></span>

* <span data-ttu-id="48988-2190">`feature show` adicionado novamente</span><span class="sxs-lookup"><span data-stu-id="48988-2190">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="48988-2191">Função</span><span class="sxs-lookup"><span data-stu-id="48988-2191">Role</span></span>

* <span data-ttu-id="48988-2192">Adicionado o argumento `--available-to-other-tenants` para `ad app update`</span><span class="sxs-lookup"><span data-stu-id="48988-2192">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="48988-2193">SQL</span><span class="sxs-lookup"><span data-stu-id="48988-2193">SQL</span></span>

* <span data-ttu-id="48988-2194">Adicionados os comandos `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="48988-2194">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="48988-2195">Adicionado `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="48988-2195">Added `sql db rename`</span></span>
* <span data-ttu-id="48988-2196">Adicionado suporte para o argumento `--ids` para todos os comandos sql</span><span class="sxs-lookup"><span data-stu-id="48988-2196">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="48988-2197">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48988-2197">Storage</span></span>

* <span data-ttu-id="48988-2198">Adicionados os comandos `storage blob service-properties delete-policy` e `storage blob undelete` para habilitar a exclusão reversível</span><span class="sxs-lookup"><span data-stu-id="48988-2198">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="48988-2199">VM</span><span class="sxs-lookup"><span data-stu-id="48988-2199">VM</span></span>

* <span data-ttu-id="48988-2200">Corrigida uma falha quando a criptografia de VM não pode ser totalmente inicializada</span><span class="sxs-lookup"><span data-stu-id="48988-2200">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="48988-2201">Adicionada saída de ID de entidade de segurança ao habilitar o MSI</span><span class="sxs-lookup"><span data-stu-id="48988-2201">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="48988-2202">`vm boot-diagnostics get-boot-log` fixo</span><span class="sxs-lookup"><span data-stu-id="48988-2202">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="48988-2203">31 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="48988-2203">January 31, 2018</span></span>

<span data-ttu-id="48988-2204">Versão 2.0.26</span><span class="sxs-lookup"><span data-stu-id="48988-2204">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="48988-2205">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48988-2205">Core</span></span>

* <span data-ttu-id="48988-2206">Adicionado suporte para recuperação de token bruto no contexto MSI</span><span class="sxs-lookup"><span data-stu-id="48988-2206">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="48988-2207">Removida a cadeia de caracteres do indicador de sondagem depois de terminar o LRO no Windows cmd.exe</span><span class="sxs-lookup"><span data-stu-id="48988-2207">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="48988-2208">Adicionado um aviso que aparece ao usar um padrão configurado que foi alterado para uma entrada de nível de informações.</span><span class="sxs-lookup"><span data-stu-id="48988-2208">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="48988-2209">Usar `--verbose` para ver</span><span class="sxs-lookup"><span data-stu-id="48988-2209">Use `--verbose` to see</span></span>
* <span data-ttu-id="48988-2210">Adicionar um indicador de progresso para comandos de espera</span><span class="sxs-lookup"><span data-stu-id="48988-2210">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="48988-2211">ACS</span><span class="sxs-lookup"><span data-stu-id="48988-2211">ACS</span></span>

* <span data-ttu-id="48988-2212">Argumento `--disable-browser` esclarecido</span><span class="sxs-lookup"><span data-stu-id="48988-2212">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="48988-2213">Preenchimento de guia melhorado para argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="48988-2213">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="48988-2214">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-2214">Appservice</span></span>

* <span data-ttu-id="48988-2215">`webapp log [tail|download]` fixo</span><span class="sxs-lookup"><span data-stu-id="48988-2215">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="48988-2216">Removida a verificação de `kind` em aplicativos Web e funções</span><span class="sxs-lookup"><span data-stu-id="48988-2216">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="48988-2217">CDN</span><span class="sxs-lookup"><span data-stu-id="48988-2217">CDN</span></span>

* <span data-ttu-id="48988-2218">Corrigido o problema de cliente ausente com `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="48988-2218">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="48988-2219">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="48988-2219">CosmosDB</span></span>

* <span data-ttu-id="48988-2220">Corrigida a descrição do parâmetro para políticas de failover</span><span class="sxs-lookup"><span data-stu-id="48988-2220">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="48988-2221">Interativo</span><span class="sxs-lookup"><span data-stu-id="48988-2221">Interactive</span></span>

* <span data-ttu-id="48988-2222">Corrigido o problema em que as conclusões de opção de comando não aparecem mais</span><span class="sxs-lookup"><span data-stu-id="48988-2222">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="48988-2223">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-2223">Network</span></span>

* <span data-ttu-id="48988-2224">Adicionada a proteção para `--cert-password` para `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="48988-2224">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="48988-2225">Corrigido o problema com `application-gateway update` em que `--sku` aplicou um valor padrão de forma errada</span><span class="sxs-lookup"><span data-stu-id="48988-2225">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="48988-2226">Adicionada proteção para `--shared-key` e `--authorization-key` para `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="48988-2226">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="48988-2227">Corrigido o problema de cliente ausente com `asg create`</span><span class="sxs-lookup"><span data-stu-id="48988-2227">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="48988-2228">Adicionado o parâmetro `--file-name / -f` para nomes exportados para `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="48988-2228">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="48988-2229">Os seguintes problemas foram corrigidos com `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="48988-2229">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="48988-2230">Corrigido o problema em que registros TXT longos foram exportados incorretamente</span><span class="sxs-lookup"><span data-stu-id="48988-2230">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="48988-2231">Corrigido o problema em que registros TXT entre aspas foram exportados incorretamente sem as aspas com caracteres de escape</span><span class="sxs-lookup"><span data-stu-id="48988-2231">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="48988-2232">Corrigido o problema em que determinados registros foram importados duas vezes com `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="48988-2232">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="48988-2233">Restaurados os comandos `vnet-gateway root-cert` e `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="48988-2233">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="48988-2234">Perfil</span><span class="sxs-lookup"><span data-stu-id="48988-2234">Profile</span></span>

* <span data-ttu-id="48988-2235">`get-access-token` corrigido para trabalhar em uma VM com identidade</span><span class="sxs-lookup"><span data-stu-id="48988-2235">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="48988-2236">Recurso</span><span class="sxs-lookup"><span data-stu-id="48988-2236">Resource</span></span>

* <span data-ttu-id="48988-2237">Corrigido o bug com `deployment [create|validate]` em que um aviso era exibido incorretamente quando um campo ‘tipo’ do modelo continha valores maiúsculos</span><span class="sxs-lookup"><span data-stu-id="48988-2237">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="48988-2238">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48988-2238">Storage</span></span>

* <span data-ttu-id="48988-2239">Corrigido o problema com a migração de contas de Armazenamento V1 para Armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="48988-2239">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="48988-2240">Adicionado o relatório de andamento de todos os comandos de upload/download</span><span class="sxs-lookup"><span data-stu-id="48988-2240">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="48988-2241">Corrigido o bug que impedia a opção “-n” arg com `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="48988-2241">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="48988-2242">Adicionada a coluna ‘instantâneo’ à saída de tabela para `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="48988-2242">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="48988-2243">Corrigidos bugs com vários parâmetros que precisam ser analisados como ints</span><span class="sxs-lookup"><span data-stu-id="48988-2243">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="48988-2244">VM</span><span class="sxs-lookup"><span data-stu-id="48988-2244">VM</span></span>

* <span data-ttu-id="48988-2245">Adicionado o comando `vm image accept-terms` para permitir a criação de VMs a partir de imagens com encargos adicionais</span><span class="sxs-lookup"><span data-stu-id="48988-2245">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="48988-2246">`[vm|vmss create]` corrigido para garantir que comandos possam ser executados sob o proxy com certificados não assinados</span><span class="sxs-lookup"><span data-stu-id="48988-2246">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="48988-2247">[VERSÃO PRÉVIA] Adicionado suporte para “baixa” prioridade para VMSS</span><span class="sxs-lookup"><span data-stu-id="48988-2247">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="48988-2248">Adicionada a proteção para `--admin-password` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="48988-2248">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="48988-2249">17 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="48988-2249">January 17, 2018</span></span>

<span data-ttu-id="48988-2250">Versão 2.0.25</span><span class="sxs-lookup"><span data-stu-id="48988-2250">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="48988-2251">ACR</span><span class="sxs-lookup"><span data-stu-id="48988-2251">ACR</span></span>

* <span data-ttu-id="48988-2252">Adicionado fallback de logon de acr em erros de credencial do Windows</span><span class="sxs-lookup"><span data-stu-id="48988-2252">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="48988-2253">Habilitados os logs de registro</span><span class="sxs-lookup"><span data-stu-id="48988-2253">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="48988-2254">ACS</span><span class="sxs-lookup"><span data-stu-id="48988-2254">ACS</span></span>

* <span data-ttu-id="48988-2255">Corrigido o comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="48988-2255">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="48988-2256">Removido o requisito de função do SPN</span><span class="sxs-lookup"><span data-stu-id="48988-2256">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="48988-2257">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-2257">Appservice</span></span>

* <span data-ttu-id="48988-2258">Corrigido o bug com `config ssl upload` onde `hosting_environment_profile` era nulo</span><span class="sxs-lookup"><span data-stu-id="48988-2258">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="48988-2259">Adicionado suporte para URLs personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="48988-2259">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="48988-2260">Corrigido o suporte de slot para `log tail`</span><span class="sxs-lookup"><span data-stu-id="48988-2260">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="48988-2261">Backup</span><span class="sxs-lookup"><span data-stu-id="48988-2261">Backup</span></span>

* <span data-ttu-id="48988-2262">Alterada a opção `--container-name` de `backup item list` para ser opcional</span><span class="sxs-lookup"><span data-stu-id="48988-2262">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="48988-2263">Adicionadas opções da conta de armazenamento para `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="48988-2263">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="48988-2264">Corrigido o check-in de local de `backup protection enable-for-vm` para não diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="48988-2264">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="48988-2265">Corrigido o problema em que os comandos falhavam com um nome de contêiner inválido</span><span class="sxs-lookup"><span data-stu-id="48988-2265">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="48988-2266">Alterado `backup item list` para incluir o 'Status de Integridade' como padrão</span><span class="sxs-lookup"><span data-stu-id="48988-2266">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="48988-2267">Lote</span><span class="sxs-lookup"><span data-stu-id="48988-2267">Batch</span></span>

* <span data-ttu-id="48988-2268">Alterado `batch login` para retornar detalhes de autenticação</span><span class="sxs-lookup"><span data-stu-id="48988-2268">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="48988-2269">Nuvem</span><span class="sxs-lookup"><span data-stu-id="48988-2269">Cloud</span></span>

* <span data-ttu-id="48988-2270">Alterado para não exigir pontos de extremidade ao definir `--profile` em uma nuvem</span><span class="sxs-lookup"><span data-stu-id="48988-2270">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="48988-2271">Consumo</span><span class="sxs-lookup"><span data-stu-id="48988-2271">Consumption</span></span>

* <span data-ttu-id="48988-2272">Adicionados novos comandos para reservas: `consumption reservations summaries` e `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="48988-2272">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="48988-2273">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="48988-2273">Event Grid</span></span>

* <span data-ttu-id="48988-2274">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid topic event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="48988-2274">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="48988-2275">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid resource event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="48988-2275">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="48988-2276">[ALTERAÇÃO SIGNIFICATIVA] Comando `eventgrid event-subscription show-endpoint-url` removido.</span><span class="sxs-lookup"><span data-stu-id="48988-2276">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="48988-2277">Usar `eventgrid event-subscription show --include-full-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="48988-2277">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="48988-2278">Adicionado o comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="48988-2278">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="48988-2279">Adicionado o comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="48988-2279">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="48988-2280">Adicionado o parâmetro `--ids` para comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="48988-2280">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="48988-2281">Adicionado o suporte de conclusão de guia para nomes de tópico</span><span class="sxs-lookup"><span data-stu-id="48988-2281">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="48988-2282">Interativo</span><span class="sxs-lookup"><span data-stu-id="48988-2282">Interactive</span></span>

* <span data-ttu-id="48988-2283">Corrigido o problema em que o modo interativo não funcionava com o Python 2.x</span><span class="sxs-lookup"><span data-stu-id="48988-2283">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="48988-2284">Corrigidos os erros na inicialização</span><span class="sxs-lookup"><span data-stu-id="48988-2284">Fixed errors on startup</span></span>
* <span data-ttu-id="48988-2285">Corrigido o problema com alguns comandos que não estavam em execução no modo interativo</span><span class="sxs-lookup"><span data-stu-id="48988-2285">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="48988-2286">IoT</span><span class="sxs-lookup"><span data-stu-id="48988-2286">IoT</span></span>

* <span data-ttu-id="48988-2287">Adicionado suporte para o serviço de provisionamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="48988-2287">Added support for device provisioning service</span></span>
* <span data-ttu-id="48988-2288">Adicionadas mensagens de reprovação em comandos e ajuda de comando</span><span class="sxs-lookup"><span data-stu-id="48988-2288">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="48988-2289">Adicionada verificação de IoT para informar os usuários da Extensão de IoT</span><span class="sxs-lookup"><span data-stu-id="48988-2289">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="48988-2290">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="48988-2290">Monitor</span></span>

* <span data-ttu-id="48988-2291">Adicionado o suporte de configuração de vários diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="48988-2291">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="48988-2292">Agora o parâmetro `--name` é necessário para `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="48988-2292">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="48988-2293">Adicionado o comando `monitor diagnostic-settings categories` para obter a categoria de configurações de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="48988-2293">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="48988-2294">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-2294">Network</span></span>

* <span data-ttu-id="48988-2295">Corrigido o problema ao tentar alterar de/para o modo ativo-em espera com `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="48988-2295">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="48988-2296">Adicionado o suporte para HTTP2 para `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48988-2296">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="48988-2297">Perfil</span><span class="sxs-lookup"><span data-stu-id="48988-2297">Profile</span></span>

* <span data-ttu-id="48988-2298">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="48988-2298">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="48988-2299">Função</span><span class="sxs-lookup"><span data-stu-id="48988-2299">Role</span></span>

* <span data-ttu-id="48988-2300">Adicionado o argumento `--assignee-object-id` para `role assignment create` para ignorar a consulta do gráfico</span><span class="sxs-lookup"><span data-stu-id="48988-2300">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="48988-2301">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="48988-2301">Service Fabric</span></span>

* <span data-ttu-id="48988-2302">Adicionados erros detalhados à resposta de validação ao criar cluster</span><span class="sxs-lookup"><span data-stu-id="48988-2302">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="48988-2303">Corrigido o problema de cliente ausente com vários comandos</span><span class="sxs-lookup"><span data-stu-id="48988-2303">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="48988-2304">VM</span><span class="sxs-lookup"><span data-stu-id="48988-2304">VM</span></span>

* <span data-ttu-id="48988-2305">[VERSÃO PRÉVIA] Suporte entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="48988-2305">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="48988-2306">[ALTERAÇÃO SIGNIFICATIVA] Alterada única zona `vmss` padrão para o balanceador de carga "Padrão"</span><span class="sxs-lookup"><span data-stu-id="48988-2306">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="48988-2307">[ALTERAÇÃO SIGNIFICATIVA] `externalIdentities` alterado para `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="48988-2307">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="48988-2308">[VERSÃO PRÉVIA] Adicionado o suporte para a troca de disco do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="48988-2308">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="48988-2309">Adicionado o suporte para o uso de imagens da VM de outras assinaturas</span><span class="sxs-lookup"><span data-stu-id="48988-2309">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="48988-2310">Adicionados os argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` e `--plan-publisher` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="48988-2310">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="48988-2311">Corrigidos os problemas de erro com `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="48988-2311">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="48988-2312">Corrigido o uso excessivo de recursos causados por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="48988-2312">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="48988-2313">19 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="48988-2313">December 19, 2017</span></span>

<span data-ttu-id="48988-2314">Versão 2.0.23</span><span class="sxs-lookup"><span data-stu-id="48988-2314">Version 2.0.23</span></span>

* <span data-ttu-id="48988-2315">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="48988-2315">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="48988-2316">Contêiner</span><span class="sxs-lookup"><span data-stu-id="48988-2316">Container</span></span>

* <span data-ttu-id="48988-2317">Corrigida a ordem incorreta de parâmetros para logs de contêiner</span><span class="sxs-lookup"><span data-stu-id="48988-2317">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="48988-2318">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-2318">Network</span></span>

* <span data-ttu-id="48988-2319">Adicionado o argumento `--disable-bgp-route-propagation` para `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48988-2319">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="48988-2320">Adicionado o argumento `--ip-tags` para `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48988-2320">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="48988-2321">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48988-2321">Storage</span></span>

* <span data-ttu-id="48988-2322">Adicionado suporte para armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="48988-2322">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="48988-2323">VM</span><span class="sxs-lookup"><span data-stu-id="48988-2323">VM</span></span>

* <span data-ttu-id="48988-2324">[VERSÃO PRÉVIA] Adicionado suporte para identidades atribuídas a usuários para VMs e VMSSes</span><span class="sxs-lookup"><span data-stu-id="48988-2324">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="48988-2325">5 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="48988-2325">December 5, 2017</span></span>

<span data-ttu-id="48988-2326">Versão 2.0.22</span><span class="sxs-lookup"><span data-stu-id="48988-2326">Version 2.0.22</span></span>

* <span data-ttu-id="48988-2327">Comandos `az component` removidos.</span><span class="sxs-lookup"><span data-stu-id="48988-2327">Removed `az component` commands.</span></span> <span data-ttu-id="48988-2328">Usar `az extension`</span><span class="sxs-lookup"><span data-stu-id="48988-2328">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="48988-2329">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48988-2329">Core</span></span>
* <span data-ttu-id="48988-2330">Modificou o ponto de extremidade de autoridade AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com para login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="48988-2330">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="48988-2331">Corrigido o problema onde a telemetria reenviaria continuamente</span><span class="sxs-lookup"><span data-stu-id="48988-2331">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="48988-2332">ACS</span><span class="sxs-lookup"><span data-stu-id="48988-2332">ACS</span></span>

* <span data-ttu-id="48988-2333">Comandos `aks install-connector` e `aks remove-connector` adicionados</span><span class="sxs-lookup"><span data-stu-id="48988-2333">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="48988-2334">Relatório de erros aprimorado para `acs create`</span><span class="sxs-lookup"><span data-stu-id="48988-2334">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="48988-2335">Corrigido o uso de `aks get-credentials -f` sem um caminho totalmente qualificado</span><span class="sxs-lookup"><span data-stu-id="48988-2335">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="48988-2336">Supervisor</span><span class="sxs-lookup"><span data-stu-id="48988-2336">Advisor</span></span>

* <span data-ttu-id="48988-2337">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="48988-2337">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="48988-2338">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-2338">Appservice</span></span>

* <span data-ttu-id="48988-2339">Corrigida a geração de nome do certificado com `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="48988-2339">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="48988-2340">Corrigidos `webapp [list|show]` e `functionapp [list|show]` para exibir os aplicativos corretos</span><span class="sxs-lookup"><span data-stu-id="48988-2340">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="48988-2341">Valor padrão adicionado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="48988-2341">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="48988-2342">Consumo</span><span class="sxs-lookup"><span data-stu-id="48988-2342">Consumption</span></span>

* <span data-ttu-id="48988-2343">Suporte adicionado para a API versão de 30/11/2017</span><span class="sxs-lookup"><span data-stu-id="48988-2343">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="48988-2344">Contêiner</span><span class="sxs-lookup"><span data-stu-id="48988-2344">Container</span></span>

* <span data-ttu-id="48988-2345">Corrigida a regressão de portas padrão</span><span class="sxs-lookup"><span data-stu-id="48988-2345">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="48988-2346">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="48988-2346">Monitor</span></span>

* <span data-ttu-id="48988-2347">Suporte de várias dimensões adicionado ao comando de métricas</span><span class="sxs-lookup"><span data-stu-id="48988-2347">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="48988-2348">Recurso</span><span class="sxs-lookup"><span data-stu-id="48988-2348">Resource</span></span>

* <span data-ttu-id="48988-2349">Adicionado o argumento `--include-response-body` para `resource show`</span><span class="sxs-lookup"><span data-stu-id="48988-2349">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="48988-2350">Função</span><span class="sxs-lookup"><span data-stu-id="48988-2350">Role</span></span>

* <span data-ttu-id="48988-2351">Exibição de atribuições padrão adicionada dos administradores "clássicos" para `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="48988-2351">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="48988-2352">Suporte adicionado a `ad sp reset-credentials` para adicionar as credenciais em vez de substituir</span><span class="sxs-lookup"><span data-stu-id="48988-2352">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="48988-2353">Relatório de erros aprimorado para `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="48988-2353">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="48988-2354">SQL</span><span class="sxs-lookup"><span data-stu-id="48988-2354">SQL</span></span>

* <span data-ttu-id="48988-2355">Comandos `sql db list-usages` e `sql db show-usage` adicionados</span><span class="sxs-lookup"><span data-stu-id="48988-2355">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="48988-2356">Comandos `sql server conn-policy show` e `sql server conn-policy update` adicionados</span><span class="sxs-lookup"><span data-stu-id="48988-2356">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="48988-2357">VM</span><span class="sxs-lookup"><span data-stu-id="48988-2357">VM</span></span>

* <span data-ttu-id="48988-2358">Informações da zona adicionadas a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="48988-2358">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="48988-2359">14 de novembro de 2017</span><span class="sxs-lookup"><span data-stu-id="48988-2359">November 14, 2017</span></span>

<span data-ttu-id="48988-2360">Versão 2.0.21</span><span class="sxs-lookup"><span data-stu-id="48988-2360">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="48988-2361">ACR</span><span class="sxs-lookup"><span data-stu-id="48988-2361">ACR</span></span>

* <span data-ttu-id="48988-2362">Suporte adicionado para criar webhooks em regiões de replicação</span><span class="sxs-lookup"><span data-stu-id="48988-2362">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="48988-2363">ACS</span><span class="sxs-lookup"><span data-stu-id="48988-2363">ACS</span></span>

* <span data-ttu-id="48988-2364">Alteradas todas as palavras "agente" para "nó" no AKS</span><span class="sxs-lookup"><span data-stu-id="48988-2364">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="48988-2365">Opção `--orchestrator-release` preterida para `acs create`</span><span class="sxs-lookup"><span data-stu-id="48988-2365">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="48988-2366">Tamanho alterado da VM padrão do AKS para `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="48988-2366">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="48988-2367">`az aks browse` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="48988-2367">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="48988-2368">`az aks get-credentials` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="48988-2368">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="48988-2369">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-2369">Appservice</span></span>

* <span data-ttu-id="48988-2370">Origem da implantação adicional `config-zip` para webapps e aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="48988-2370">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="48988-2371">Opção `--docker-container-logging` adicionada a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="48988-2371">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="48988-2372">Removida a opção `storage` do parâmetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="48988-2372">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="48988-2373">Mensagens de erro aprimoradas para `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="48988-2373">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="48988-2374">Suporte adicionado para criar aplicativos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="48988-2374">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="48988-2375">`list-locations` fixo</span><span class="sxs-lookup"><span data-stu-id="48988-2375">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="48988-2376">Lote</span><span class="sxs-lookup"><span data-stu-id="48988-2376">Batch</span></span>

* <span data-ttu-id="48988-2377">Bug corrigido no comando pool create quando uma ID do recurso foi usada com o sinalizador `--image`</span><span class="sxs-lookup"><span data-stu-id="48988-2377">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="48988-2378">Batchai</span><span class="sxs-lookup"><span data-stu-id="48988-2378">Batchai</span></span>

* <span data-ttu-id="48988-2379">Opção curta adicionada `-s` para `--vm-size` ao fornecer o tamanho da VM no comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="48988-2379">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="48988-2380">Nome da conta de armazenamento e argumentos-chave adicionados aos parâmetros `cluster create`</span><span class="sxs-lookup"><span data-stu-id="48988-2380">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="48988-2381">Documentação corrigida para `job list-files` e `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="48988-2381">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="48988-2382">Opção curta adicionada `-r` para `--cluster-name` ao fornecer o nome do cluster no comando `job create`</span><span class="sxs-lookup"><span data-stu-id="48988-2382">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="48988-2383">Nuvem</span><span class="sxs-lookup"><span data-stu-id="48988-2383">Cloud</span></span>

* <span data-ttu-id="48988-2384">`cloud [register|update]` alterado para evitar registrar nuvens sem os pontos de extremidade necessários</span><span class="sxs-lookup"><span data-stu-id="48988-2384">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="48988-2385">Contêiner</span><span class="sxs-lookup"><span data-stu-id="48988-2385">Container</span></span>

* <span data-ttu-id="48988-2386">Suporte adicionado para abrir várias portas</span><span class="sxs-lookup"><span data-stu-id="48988-2386">Added support to open multiple ports</span></span>
* <span data-ttu-id="48988-2387">Política de reinicialização do grupo de contêiner adicionada</span><span class="sxs-lookup"><span data-stu-id="48988-2387">Added container group restart policy</span></span>
* <span data-ttu-id="48988-2388">Suporte adicionado para montar o compartilhamento de Arquivos do Azure como um volume</span><span class="sxs-lookup"><span data-stu-id="48988-2388">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="48988-2389">Documentos de ajuda atualizados</span><span class="sxs-lookup"><span data-stu-id="48988-2389">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="48988-2390">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="48988-2390">Data Lake Analytics</span></span>

* <span data-ttu-id="48988-2391">`[job|account] list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="48988-2391">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="48988-2392">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="48988-2392">Data Lake Store</span></span>

* <span data-ttu-id="48988-2393">`account list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="48988-2393">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="48988-2394">Extensão</span><span class="sxs-lookup"><span data-stu-id="48988-2394">Extension</span></span>

* <span data-ttu-id="48988-2395">`extension list-available` adicionado para permitir a listagem de extensões oficiais da Microsoft</span><span class="sxs-lookup"><span data-stu-id="48988-2395">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="48988-2396">`--name` adicionado a `extension [add|update]` para permitir a instalação de extensões por nome</span><span class="sxs-lookup"><span data-stu-id="48988-2396">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="48988-2397">IoT</span><span class="sxs-lookup"><span data-stu-id="48988-2397">IoT</span></span>

* <span data-ttu-id="48988-2398">Suporte adicionado para as autoridades de certificação (CA) e cadeias de certificado</span><span class="sxs-lookup"><span data-stu-id="48988-2398">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="48988-2399">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="48988-2399">Monitor</span></span>

* <span data-ttu-id="48988-2400">Adicionados os comandos `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="48988-2400">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="48988-2401">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-2401">Network</span></span>

* <span data-ttu-id="48988-2402">Suporte adicionado para registros DNS da CAA</span><span class="sxs-lookup"><span data-stu-id="48988-2402">Added support for CAA DNS records</span></span>
* <span data-ttu-id="48988-2403">Problema corrigido onde os pontos de extremidade não podem ser atualizados com `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="48988-2403">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="48988-2404">Problema corrigido onde `vnet update --dns-servers` não funcionou dependendo de como a VNET foi criada</span><span class="sxs-lookup"><span data-stu-id="48988-2404">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="48988-2405">Problema corrigido onde os nomes DNS relativos foram importados incorretamente por`dns zone import`</span><span class="sxs-lookup"><span data-stu-id="48988-2405">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="48988-2406">Reservas</span><span class="sxs-lookup"><span data-stu-id="48988-2406">Reservations</span></span>

* <span data-ttu-id="48988-2407">Versão prévia inicial</span><span class="sxs-lookup"><span data-stu-id="48988-2407">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="48988-2408">Recurso</span><span class="sxs-lookup"><span data-stu-id="48988-2408">Resource</span></span>

* <span data-ttu-id="48988-2409">Suporte adicionado das IDs de recurso ao parâmetro `--resource` e bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="48988-2409">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="48988-2410">SQL</span><span class="sxs-lookup"><span data-stu-id="48988-2410">SQL</span></span>

* <span data-ttu-id="48988-2411">Parâmetro `--ignore-missing-vnet-service-endpoint` adicionado a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48988-2411">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="48988-2412">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48988-2412">Storage</span></span>

* <span data-ttu-id="48988-2413">`storage account create` criado ao usar o SKU `Standard_RAGRS` como padrão</span><span class="sxs-lookup"><span data-stu-id="48988-2413">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="48988-2414">Bugs corrigidos ao lidar com nomes de arquivo/blob que incluem caracteres não ascii</span><span class="sxs-lookup"><span data-stu-id="48988-2414">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="48988-2415">Bug corrigido que impedia usar `--source-uri` com `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="48988-2415">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="48988-2416">Comandos adicionados para usar o glob e excluir vários objetos com `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="48988-2416">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="48988-2417">Problema corrigido ao habilitar métricas com `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="48988-2417">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="48988-2418">Problema corrigido com arquivos acima de 200 GB ao usar `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="48988-2418">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="48988-2419">Problema corrigido onde `--bypass` e `--default-action` foram ignorados por `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48988-2419">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="48988-2420">VM</span><span class="sxs-lookup"><span data-stu-id="48988-2420">VM</span></span>

* <span data-ttu-id="48988-2421">Bug corrigido com `vmss create`, que impediu o uso da camada de tamanho `Basic`</span><span class="sxs-lookup"><span data-stu-id="48988-2421">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="48988-2422">Argumentos `--plan` adicionados a `[vm|vmss] create` para ter imagens personalizadas com informações de cobrança</span><span class="sxs-lookup"><span data-stu-id="48988-2422">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="48988-2423">Comandos `vm secret `[add|remove|list]\` adicionados</span><span class="sxs-lookup"><span data-stu-id="48988-2423">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="48988-2424">`vm format-secret` renomeado para `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="48988-2424">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="48988-2425">Adicionado o argumento `--encrypt format` para `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="48988-2425">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="48988-2426">24 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="48988-2426">October 24, 2017</span></span>

<span data-ttu-id="48988-2427">Versão 2.0.20</span><span class="sxs-lookup"><span data-stu-id="48988-2427">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="48988-2428">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48988-2428">Core</span></span>

* <span data-ttu-id="48988-2429">Atualizado `2017-03-09-profile` para usar a `MGMT_STORAGE` versão da API`2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="48988-2429">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="48988-2430">ACR</span><span class="sxs-lookup"><span data-stu-id="48988-2430">ACR</span></span>

* <span data-ttu-id="48988-2431">Gerenciamento de recursos atualizado para apontar para a versão da API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="48988-2431">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="48988-2432">SKU 'traga seu próprio armazenamento' alterada para Clássico</span><span class="sxs-lookup"><span data-stu-id="48988-2432">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="48988-2433">SKUs de registro renomeados como Básico, Standard e Premium</span><span class="sxs-lookup"><span data-stu-id="48988-2433">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="48988-2434">ACS</span><span class="sxs-lookup"><span data-stu-id="48988-2434">ACS</span></span>

* <span data-ttu-id="48988-2435">[VERSÃO PRÉVIA] Comandos `az aks` adicionados</span><span class="sxs-lookup"><span data-stu-id="48988-2435">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="48988-2436">Kubernetes `get-credentials` corrigido</span><span class="sxs-lookup"><span data-stu-id="48988-2436">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="48988-2437">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-2437">Appservice</span></span>

* <span data-ttu-id="48988-2438">Problema corrigido onde os logs `webapp` baixados podem ser inválidos</span><span class="sxs-lookup"><span data-stu-id="48988-2438">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="48988-2439">Componente</span><span class="sxs-lookup"><span data-stu-id="48988-2439">Component</span></span>

* <span data-ttu-id="48988-2440">Mensagem de reprovação mais clara adicionada para todos os instaladores e prompt de confirmação</span><span class="sxs-lookup"><span data-stu-id="48988-2440">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="48988-2441">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="48988-2441">Monitor</span></span>

* <span data-ttu-id="48988-2442">Adicionados os comandos `action-group`</span><span class="sxs-lookup"><span data-stu-id="48988-2442">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="48988-2443">Recurso</span><span class="sxs-lookup"><span data-stu-id="48988-2443">Resource</span></span>

* <span data-ttu-id="48988-2444">Incompatibilidade corrigida com a versão mais recente de dependência msrest em `group export`</span><span class="sxs-lookup"><span data-stu-id="48988-2444">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="48988-2445">`policy assignment create` corrigido para trabalhar com as definições de política internas e as definições do conjunto de políticas</span><span class="sxs-lookup"><span data-stu-id="48988-2445">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="48988-2446">VM</span><span class="sxs-lookup"><span data-stu-id="48988-2446">VM</span></span>

* <span data-ttu-id="48988-2447">Adicionado o argumento `--accelerated-networking` para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="48988-2447">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="48988-2448">9 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="48988-2448">October 9, 2017</span></span>

<span data-ttu-id="48988-2449">Versão 2.0.19</span><span class="sxs-lookup"><span data-stu-id="48988-2449">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="48988-2450">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48988-2450">Core</span></span>

* <span data-ttu-id="48988-2451">Tratamento de URLs de autoridade do AD FS adicionado com uma barra à direita para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="48988-2451">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="48988-2452">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-2452">Appservice</span></span>

* <span data-ttu-id="48988-2453">Atualização genérica adicionada com o novo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="48988-2453">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="48988-2454">Lote</span><span class="sxs-lookup"><span data-stu-id="48988-2454">Batch</span></span>

* <span data-ttu-id="48988-2455">Atualizado para o SDK do Lote 4.0.0</span><span class="sxs-lookup"><span data-stu-id="48988-2455">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="48988-2456">A opção `--image` de VirtualMachineConfiguration foi atualizada para dar suporte a referências de imagem ARM além de publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="48988-2456">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="48988-2457">Suporte adicionado para o novo modelo de extensão da CLI para comandos de Extensões de Lote</span><span class="sxs-lookup"><span data-stu-id="48988-2457">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="48988-2458">Removeu o suporte de Lote do modelo de componente</span><span class="sxs-lookup"><span data-stu-id="48988-2458">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="48988-2459">Batchai</span><span class="sxs-lookup"><span data-stu-id="48988-2459">Batchai</span></span>

* <span data-ttu-id="48988-2460">Versão inicial do módulo de IA de Lote</span><span class="sxs-lookup"><span data-stu-id="48988-2460">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="48988-2461">Keyvault</span><span class="sxs-lookup"><span data-stu-id="48988-2461">Keyvault</span></span>

* <span data-ttu-id="48988-2462">Correção do problema de autenticação do Cofre de Chaves ao usar o AD FS no Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="48988-2462">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="48988-2463">(#4448)</span><span class="sxs-lookup"><span data-stu-id="48988-2463">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="48988-2464">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-2464">Network</span></span>

* <span data-ttu-id="48988-2465">Alterado `--server` argumento de `application-gateway address-pool create` para ser opcional, permitindo pools de endereços vazios</span><span class="sxs-lookup"><span data-stu-id="48988-2465">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="48988-2466">`traffic-manager` foi atualizado para oferecer suporte aos recursos mais recentes</span><span class="sxs-lookup"><span data-stu-id="48988-2466">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="48988-2467">Recurso</span><span class="sxs-lookup"><span data-stu-id="48988-2467">Resource</span></span>

* <span data-ttu-id="48988-2468">Suporte adicionado para `--resource-group/-g` opções do nome do grupo de recursos para `group`</span><span class="sxs-lookup"><span data-stu-id="48988-2468">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="48988-2469">Comandos adicionados a `account lock` para funcionar com bloqueios no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="48988-2469">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="48988-2470">Comandos adicionados a `group lock` para funcionar com bloqueios no nível do grupo</span><span class="sxs-lookup"><span data-stu-id="48988-2470">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="48988-2471">Comandos adicionados a `resource lock` para funcionar com bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="48988-2471">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="48988-2472">Sql</span><span class="sxs-lookup"><span data-stu-id="48988-2472">Sql</span></span>

* <span data-ttu-id="48988-2473">Suporte adicionado para SQL TDE (Transparent Data Encryption) e TDE com Traga sua própria chave</span><span class="sxs-lookup"><span data-stu-id="48988-2473">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="48988-2474">Comando `db list-deleted` e parâmetro `db restore --deleted-time` adicionados, permitindo localizar e restaurar bancos de dados excluídos</span><span class="sxs-lookup"><span data-stu-id="48988-2474">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="48988-2475">`db op list` e `db op cancel` adicionados, permitindo listar e cancelar operações em andamento no banco de dados</span><span class="sxs-lookup"><span data-stu-id="48988-2475">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="48988-2476">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48988-2476">Storage</span></span>

* <span data-ttu-id="48988-2477">Suporte adicionado para instantâneo de compartilhamento de arquivos</span><span class="sxs-lookup"><span data-stu-id="48988-2477">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="48988-2478">VM</span><span class="sxs-lookup"><span data-stu-id="48988-2478">Vm</span></span>

* <span data-ttu-id="48988-2479">Correção de um bug em `vm show` onde o uso de `-d` causou uma falha nos endereços IP privados ausentes</span><span class="sxs-lookup"><span data-stu-id="48988-2479">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="48988-2480">[VERSÃO PRÉVIA] Suporte adicionado para atualização sem interrupção para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="48988-2480">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="48988-2481">Suporte adicionado para atualizar as configurações de criptografia com `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="48988-2481">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="48988-2482">Parâmetro `--os-disk-size-gb` adicionado a `vm create`</span><span class="sxs-lookup"><span data-stu-id="48988-2482">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="48988-2483">Parâmetro `--license-type` adicionado ao Windows para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="48988-2483">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="48988-2484">22 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="48988-2484">September 22, 2017</span></span>

<span data-ttu-id="48988-2485">Versão 2.0.1.8</span><span class="sxs-lookup"><span data-stu-id="48988-2485">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="48988-2486">Recurso</span><span class="sxs-lookup"><span data-stu-id="48988-2486">Resource</span></span>

* <span data-ttu-id="48988-2487">Suporte adicionado para mostrar as definições de políticas internas</span><span class="sxs-lookup"><span data-stu-id="48988-2487">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="48988-2488">Parâmetro de modo de suporte adicionado para a criação de definições de política</span><span class="sxs-lookup"><span data-stu-id="48988-2488">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="48988-2489">Suporte adicionado para definições de interface do usuário e modelos em `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="48988-2489">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="48988-2490">[ALTERAÇÃO SIGNIFICATIVA] Tipo de recurso `managedapp` alterado de `appliances` para `applications` e de `applianceDefinitions` para `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="48988-2490">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="48988-2491">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-2491">Network</span></span>

* <span data-ttu-id="48988-2492">Suporte adicionado para a zona de disponibilidade para os subcomandos `network lb` e `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="48988-2492">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="48988-2493">Suporte adicionado ao Emparelhamento IPv6 da Microsoft para `express-route`</span><span class="sxs-lookup"><span data-stu-id="48988-2493">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="48988-2494">Adicionados `asg` comandos de grupo de segurança do aplicativo</span><span class="sxs-lookup"><span data-stu-id="48988-2494">Added `asg` application security group commands</span></span>
* <span data-ttu-id="48988-2495">Adicionado o argumento `--application-security-groups` para `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="48988-2495">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="48988-2496">Adicionados os argumentos `--source-asgs` e `--destination-asgs` para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48988-2496">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="48988-2497">Adicionados os argumentos `--ddos-protection` e `--vm-protection` para `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48988-2497">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="48988-2498">Adicionados os comandos `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="48988-2498">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="48988-2499">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48988-2499">Storage</span></span>

* <span data-ttu-id="48988-2500">Correção do problema onde `storage account network-rule` comandos poderão falhar após a atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="48988-2500">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="48988-2501">Grade de eventos</span><span class="sxs-lookup"><span data-stu-id="48988-2501">Eventgrid</span></span>

* <span data-ttu-id="48988-2502">Atualizada SDK Python da Grade de Eventos do Azure para usar a versão de API mais recente "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="48988-2502">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="48988-2503">SQL</span><span class="sxs-lookup"><span data-stu-id="48988-2503">SQL</span></span>

* <span data-ttu-id="48988-2504">Alterado o `sql server list` argumento `--resource-group` para ser opcional.</span><span class="sxs-lookup"><span data-stu-id="48988-2504">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="48988-2505">Se não for especificado, todos os servidores sql na assinatura serão retornados</span><span class="sxs-lookup"><span data-stu-id="48988-2505">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="48988-2506">Adicionado o `--no-wait` parâmetro para `db [create|copy|restore|update|replica create|create|update]` e `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48988-2506">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="48988-2507">Keyvault</span><span class="sxs-lookup"><span data-stu-id="48988-2507">Keyvault</span></span>

* <span data-ttu-id="48988-2508">Adicionado suporte para comandos Keyvault por trás de um proxy</span><span class="sxs-lookup"><span data-stu-id="48988-2508">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="48988-2509">VM</span><span class="sxs-lookup"><span data-stu-id="48988-2509">VM</span></span>

* <span data-ttu-id="48988-2510">Adicionado suporte à zona de disponibilidade para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="48988-2510">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="48988-2511">Correção do problema onde usar`--app-gateway ID` com `vmss create` poderia causar uma falha</span><span class="sxs-lookup"><span data-stu-id="48988-2511">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="48988-2512">Adicionado o argumento `--asgs` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="48988-2512">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="48988-2513">Suporte adicionado para executar comandos em VMs com `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="48988-2513">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="48988-2514">[VERSÃO PRÉVIA] Adicionado suporte para criptografia de disco VMSS com `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="48988-2514">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="48988-2515">Suporte adicionado para realizar a manutenção em VMs com `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="48988-2515">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="48988-2516">ACS</span><span class="sxs-lookup"><span data-stu-id="48988-2516">ACS</span></span>

* <span data-ttu-id="48988-2517">[VERSÃO PRÉVIA] Adicionado `--orchestrator-release` argumento para `acs create` para regiões de versão prévia do ACS</span><span class="sxs-lookup"><span data-stu-id="48988-2517">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="48988-2518">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-2518">Appservice</span></span>

* <span data-ttu-id="48988-2519">Adicionada a capacidade para atualizar e mostrar as configurações de autenticação com `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="48988-2519">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="48988-2520">Backup</span><span class="sxs-lookup"><span data-stu-id="48988-2520">Backup</span></span>

* <span data-ttu-id="48988-2521">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="48988-2521">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="48988-2522">11 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="48988-2522">September 11, 2017</span></span>

<span data-ttu-id="48988-2523">Versão 2.0.17</span><span class="sxs-lookup"><span data-stu-id="48988-2523">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="48988-2524">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48988-2524">Core</span></span>

* <span data-ttu-id="48988-2525">Módulo de comando habilitado para definir sua própria ID de correlação na telemetria</span><span class="sxs-lookup"><span data-stu-id="48988-2525">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="48988-2526">Problema de despejo de JSON corrigido quando a telemetria é definida como modo de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="48988-2526">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="48988-2527">Acs</span><span class="sxs-lookup"><span data-stu-id="48988-2527">Acs</span></span>

* <span data-ttu-id="48988-2528">Adicionado o comando `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="48988-2528">Added `acs list-locations` command</span></span>
* <span data-ttu-id="48988-2529">Fez `ssh-key-file` vir com o valor padrão esperado</span><span class="sxs-lookup"><span data-stu-id="48988-2529">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="48988-2530">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-2530">Appservice</span></span>

* <span data-ttu-id="48988-2531">Foi incluída a capacidade de criar um aplicativo Web em um grupo de recursos que não seja o plano de serviço ativo</span><span class="sxs-lookup"><span data-stu-id="48988-2531">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="48988-2532">CDN</span><span class="sxs-lookup"><span data-stu-id="48988-2532">CDN</span></span>

* <span data-ttu-id="48988-2533">Foi corrigido o bug 'Não é possível interar CustomDomain' para `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="48988-2533">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="48988-2534">Extensão</span><span class="sxs-lookup"><span data-stu-id="48988-2534">Extension</span></span>

* <span data-ttu-id="48988-2535">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="48988-2535">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="48988-2536">Keyvault</span><span class="sxs-lookup"><span data-stu-id="48988-2536">Keyvault</span></span>

* <span data-ttu-id="48988-2537">Foi corrigido o problema onde permissões diferenciavam maiúsculas de minúsculas para `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="48988-2537">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="48988-2538">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-2538">Network</span></span>

* <span data-ttu-id="48988-2539">`vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="48988-2539">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="48988-2540">Foi renomeado o argumento `--private-access-services` para `--service-endpoints` para `vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="48988-2540">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="48988-2541">Foi adicionado suporte a vários intervalos de IP e intervalos de portas para `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="48988-2541">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="48988-2542">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="48988-2542">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="48988-2543">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="48988-2543">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="48988-2544">Recurso</span><span class="sxs-lookup"><span data-stu-id="48988-2544">Resource</span></span>

* <span data-ttu-id="48988-2545">Permitir a passagem de definições de parâmetro de políticas de recursos em `policy definition create` e`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="48988-2545">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="48988-2546">Permitir a passagem de valores de parâmetro para`policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="48988-2546">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="48988-2547">Permitir a passagem de JSON ou arquivo para todos os parâmetros</span><span class="sxs-lookup"><span data-stu-id="48988-2547">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="48988-2548">Versão da API incrementada</span><span class="sxs-lookup"><span data-stu-id="48988-2548">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="48988-2549">SQL</span><span class="sxs-lookup"><span data-stu-id="48988-2549">SQL</span></span>

* <span data-ttu-id="48988-2550">Adicionados os comandos `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="48988-2550">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="48988-2551">VM</span><span class="sxs-lookup"><span data-stu-id="48988-2551">VM</span></span>

* <span data-ttu-id="48988-2552">Corrigido: não atribuir acesso, a menos que `--scope` seja fornecido</span><span class="sxs-lookup"><span data-stu-id="48988-2552">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="48988-2553">Corrigido: usar a mesma nomenclatura de extensão do que o portal</span><span class="sxs-lookup"><span data-stu-id="48988-2553">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="48988-2554">Foi removido `subscription` da saída de `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="48988-2554">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="48988-2555">Corrigido: SKU de armazenamento do `[vm|vmss] create` não é aplicada em discos de dados com uma imagem</span><span class="sxs-lookup"><span data-stu-id="48988-2555">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="48988-2556">Corrigido: `vm format-secret --secrets` não aceita IDs de separados de nova linha</span><span class="sxs-lookup"><span data-stu-id="48988-2556">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="48988-2557">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="48988-2557">August 31, 2017</span></span>

<span data-ttu-id="48988-2558">Versão 2.0.16</span><span class="sxs-lookup"><span data-stu-id="48988-2558">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="48988-2559">Keyvault</span><span class="sxs-lookup"><span data-stu-id="48988-2559">Keyvault</span></span>

* <span data-ttu-id="48988-2560">Correção do bug ao tentar resolver automaticamente a codificação secreta com `secret download`</span><span class="sxs-lookup"><span data-stu-id="48988-2560">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="48988-2561">Sf</span><span class="sxs-lookup"><span data-stu-id="48988-2561">Sf</span></span>

* <span data-ttu-id="48988-2562">Substituição de todos os comandos em favor da CLI do Service Fabric (sfctl)</span><span class="sxs-lookup"><span data-stu-id="48988-2562">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="48988-2563">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48988-2563">Storage</span></span>

* <span data-ttu-id="48988-2564">Correção de problema onde as contas de armazenamento não conseguiam ser criadas em regiões sem suporte ao recurso NetworkACLs</span><span class="sxs-lookup"><span data-stu-id="48988-2564">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="48988-2565">Determinar o tipo de conteúdo e a codificação do conteúdo durante o upload de arquivo e de blob se nem o tipo de conteúdo nem a codificação de conteúdo forem especificados</span><span class="sxs-lookup"><span data-stu-id="48988-2565">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="48988-2566">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="48988-2566">August 28, 2017</span></span>

<span data-ttu-id="48988-2567">Versão 2.0.15</span><span class="sxs-lookup"><span data-stu-id="48988-2567">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="48988-2568">CLI</span><span class="sxs-lookup"><span data-stu-id="48988-2568">CLI</span></span>

* <span data-ttu-id="48988-2569">Nota legal adicionada ao `--version`</span><span class="sxs-lookup"><span data-stu-id="48988-2569">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="48988-2570">ACS</span><span class="sxs-lookup"><span data-stu-id="48988-2570">ACS</span></span>

* <span data-ttu-id="48988-2571">Corrigidas as regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="48988-2571">Corrected preview regions</span></span>
* <span data-ttu-id="48988-2572">Corrigida a formatação padrão de `dns_name_prefix`</span><span class="sxs-lookup"><span data-stu-id="48988-2572">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="48988-2573">Saída de comando ACS otimizada</span><span class="sxs-lookup"><span data-stu-id="48988-2573">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="48988-2574">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-2574">Appservice</span></span>

* <span data-ttu-id="48988-2575">[ALTERAÇÃO SIGNIFICATIVA] Corrigidas as inconsistências na saída de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="48988-2575">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="48988-2576">Adicionado um novo alias de `-i` para `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="48988-2576">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="48988-2577">Exposto `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="48988-2577">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="48988-2578">Expostos novos argumentos de `az webapp delete` para manter o plano, as métricas ou o registro de DNS do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="48988-2578">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="48988-2579">Corrigido: detectar as configurações de slot corretamente</span><span class="sxs-lookup"><span data-stu-id="48988-2579">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="48988-2580">IoT</span><span class="sxs-lookup"><span data-stu-id="48988-2580">IoT</span></span>

* <span data-ttu-id="48988-2581">Corrigido #3934: a criação de uma política não limpa mais as políticas existentes</span><span class="sxs-lookup"><span data-stu-id="48988-2581">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="48988-2582">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-2582">Network</span></span>

* <span data-ttu-id="48988-2583">[ALTERAÇÃO SIGNIFICATIVA] `vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="48988-2583">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="48988-2584">[ALTERAÇÃO SIGNIFICATIVA] Opção `--private-access-services` renomeada como `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48988-2584">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="48988-2585">Adicionado suporte para vários  intervalos de IP e portas para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48988-2585">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="48988-2586">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="48988-2586">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="48988-2587">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="48988-2587">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="48988-2588">Perfil</span><span class="sxs-lookup"><span data-stu-id="48988-2588">Profile</span></span>

* <span data-ttu-id="48988-2589">`--msi` e `--msi-port` expostos a logon usando a identidade de uma máquina virtual</span><span class="sxs-lookup"><span data-stu-id="48988-2589">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="48988-2590">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="48988-2590">Service Fabric</span></span>

* <span data-ttu-id="48988-2591">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="48988-2591">Preview release</span></span>
* <span data-ttu-id="48988-2592">Simplificadas as regras de registro de usuário/senha para comando</span><span class="sxs-lookup"><span data-stu-id="48988-2592">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="48988-2593">Corrigido o prompt de senha para o usuário mesmo após a passagem do parâmetro</span><span class="sxs-lookup"><span data-stu-id="48988-2593">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="48988-2594">Adicionado suporte para `registry_cred` vazio</span><span class="sxs-lookup"><span data-stu-id="48988-2594">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="48988-2595">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48988-2595">Storage</span></span>

* <span data-ttu-id="48988-2596">Habilitada a camada de blob de configuração</span><span class="sxs-lookup"><span data-stu-id="48988-2596">Enabled setting blob tier</span></span>
* <span data-ttu-id="48988-2597">Adicionados os argumentos `--bypass` e `--default-action` ao `storage account [create|update]` para dar suporte ao serviço de túnel</span><span class="sxs-lookup"><span data-stu-id="48988-2597">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="48988-2598">Comandos adicionados ao `storage account network-rule` para adicionar as regras de rede virtual e regras baseadas em IP</span><span class="sxs-lookup"><span data-stu-id="48988-2598">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="48988-2599">Habilitada a criptografia de serviço por chave gerenciada de cliente</span><span class="sxs-lookup"><span data-stu-id="48988-2599">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="48988-2600">[ALTERAÇÃO SIGNIFICATIVA] Opção `--encryption` renomeada como `--encryption-services` para o comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="48988-2600">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="48988-2601">Correção #4220: `az storage account update encryption` - incompatibilidade de sintaxe</span><span class="sxs-lookup"><span data-stu-id="48988-2601">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="48988-2602">VM</span><span class="sxs-lookup"><span data-stu-id="48988-2602">VM</span></span>

* <span data-ttu-id="48988-2603">Corrigido o problema em que informações incorretas extras eram exibidas para `vmss get-instance-view` ao usar `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="48988-2603">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="48988-2604">Adicionado suporte ao `--lb-sku` para `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="48988-2604">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="48988-2605">Removidos nomes humanos da lista de bloqueio de nome de administrador para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="48988-2605">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="48988-2606">Corrigido o problema onde `[vm|vmss] create` geraria um erro se não for possível extrair informações do plano de uma imagem</span><span class="sxs-lookup"><span data-stu-id="48988-2606">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="48988-2607">Corrigida uma falha ao criar um conjunto de dimensionamento de máquinas virtuais com um balanceamento de carga interno</span><span class="sxs-lookup"><span data-stu-id="48988-2607">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="48988-2608">Corrigido o problema onde o argumento `--no-wait` não funcionava com `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="48988-2608">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="48988-2609">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="48988-2609">August 15, 2017</span></span>

<span data-ttu-id="48988-2610">Versão 2.0.14</span><span class="sxs-lookup"><span data-stu-id="48988-2610">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="48988-2611">ACS</span><span class="sxs-lookup"><span data-stu-id="48988-2611">ACS</span></span>

* <span data-ttu-id="48988-2612">Corrigido o número da porta SSH Master0 para kubernetes</span><span class="sxs-lookup"><span data-stu-id="48988-2612">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="48988-2613">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-2613">Appservice</span></span>

* <span data-ttu-id="48988-2614">Corrigida uma exceção ao criar um novo GIT com base no aplicativo Web Linux</span><span class="sxs-lookup"><span data-stu-id="48988-2614">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="48988-2615">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="48988-2615">Event Grid</span></span>

* <span data-ttu-id="48988-2616">Adicionadas dependências SDK</span><span class="sxs-lookup"><span data-stu-id="48988-2616">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="48988-2617">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="48988-2617">August 11, 2017</span></span>

<span data-ttu-id="48988-2618">Versão 2.0.13</span><span class="sxs-lookup"><span data-stu-id="48988-2618">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="48988-2619">ACS</span><span class="sxs-lookup"><span data-stu-id="48988-2619">ACS</span></span>

* <span data-ttu-id="48988-2620">Adicionadas mais regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="48988-2620">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="48988-2621">Lote</span><span class="sxs-lookup"><span data-stu-id="48988-2621">Batch</span></span>

* <span data-ttu-id="48988-2622">Atualizado para o Lote SDK 3.1.0 e Gerenciamento de Lote SDK 4.1.0</span><span class="sxs-lookup"><span data-stu-id="48988-2622">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="48988-2623">Adicionado um novo comando que mostra as contagens de tarefas de um trabalho</span><span class="sxs-lookup"><span data-stu-id="48988-2623">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="48988-2624">Corrigido o bug no processamento de URL de SAS do arquivo de recurso</span><span class="sxs-lookup"><span data-stu-id="48988-2624">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="48988-2625">Ponto de extremidade da conta de lote agora dá suporte ao prefixo opcional “https://”</span><span class="sxs-lookup"><span data-stu-id="48988-2625">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="48988-2626">Suporte para adicionar listas de mais de 100 tarefas a um trabalho</span><span class="sxs-lookup"><span data-stu-id="48988-2626">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="48988-2627">Adicionado log de depuração para carregar o módulo do comando de Extensões</span><span class="sxs-lookup"><span data-stu-id="48988-2627">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="48988-2628">Componente</span><span class="sxs-lookup"><span data-stu-id="48988-2628">Component</span></span>

* <span data-ttu-id="48988-2629">Aviso de substituição adicionado aos comandos 'az component'</span><span class="sxs-lookup"><span data-stu-id="48988-2629">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="48988-2630">Contêiner</span><span class="sxs-lookup"><span data-stu-id="48988-2630">Container</span></span>

* <span data-ttu-id="48988-2631">`create`: corrigido o problema em que o sinal de igual não era permitido dentro de uma variável de ambiente</span><span class="sxs-lookup"><span data-stu-id="48988-2631">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="48988-2632">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="48988-2632">Data Lake Store</span></span>

* <span data-ttu-id="48988-2633">Habilitado o controle do andamento</span><span class="sxs-lookup"><span data-stu-id="48988-2633">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="48988-2634">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="48988-2634">Event Grid</span></span>

* <span data-ttu-id="48988-2635">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="48988-2635">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="48988-2636">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-2636">Network</span></span>

* <span data-ttu-id="48988-2637">`lb`: corrigido o problema em que os nomes de recursos filhos específicos não eram resolvidos corretamente quando omitidos</span><span class="sxs-lookup"><span data-stu-id="48988-2637">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="48988-2638">`application-gateway {subresource} delete`: corrigido o problema em que `--no-wait` não foi liquidado</span><span class="sxs-lookup"><span data-stu-id="48988-2638">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="48988-2639">`application-gateway http-settings update`: corrigido o problema em que `--connection-draining-timeout` não podia ser desativado</span><span class="sxs-lookup"><span data-stu-id="48988-2639">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="48988-2640">Corrigido o erro de argumento de palavra-chave inesperado `sa_data_size_kilobyes` com `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="48988-2640">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="48988-2641">Perfil</span><span class="sxs-lookup"><span data-stu-id="48988-2641">Profile</span></span>

* <span data-ttu-id="48988-2642">`account list`: adicionado `--refresh` para sincronizar as assinaturas mais recentes do servidor</span><span class="sxs-lookup"><span data-stu-id="48988-2642">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="48988-2643">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48988-2643">Storage</span></span>

* <span data-ttu-id="48988-2644">Habilitar atualização de conta de armazenamento com a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="48988-2644">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="48988-2645">VM</span><span class="sxs-lookup"><span data-stu-id="48988-2645">VM</span></span>

* <span data-ttu-id="48988-2646">`availability-set`: exposta a contagem de domínios de falha durante a conversão</span><span class="sxs-lookup"><span data-stu-id="48988-2646">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="48988-2647">Exposto o comando `list-skus`</span><span class="sxs-lookup"><span data-stu-id="48988-2647">Exposed `list-skus` command</span></span>
* <span data-ttu-id="48988-2648">Suporte para atribuir identidade sem criar atribuições de função</span><span class="sxs-lookup"><span data-stu-id="48988-2648">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="48988-2649">Aplicar o SKU de armazenamento ao anexar discos de dados</span><span class="sxs-lookup"><span data-stu-id="48988-2649">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="48988-2650">Removido o nome do disco do sistema operacional padrão e SKU de armazenamento ao usar discos gerenciados</span><span class="sxs-lookup"><span data-stu-id="48988-2650">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="48988-2651">28 de julho de 2017</span><span class="sxs-lookup"><span data-stu-id="48988-2651">July 28, 2017</span></span>

<span data-ttu-id="48988-2652">Versão 2.0.12</span><span class="sxs-lookup"><span data-stu-id="48988-2652">Version 2.0.12</span></span>

* <span data-ttu-id="48988-2653">Adicionado os comandos de contêiner</span><span class="sxs-lookup"><span data-stu-id="48988-2653">Added container commands</span></span>
* <span data-ttu-id="48988-2654">Adicionados módulos de cobrança e de consumo</span><span class="sxs-lookup"><span data-stu-id="48988-2654">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="48988-2655">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48988-2655">Core</span></span>

* <span data-ttu-id="48988-2656">Informações de autenticação de SDK de saída para entidades de serviço com certificados</span><span class="sxs-lookup"><span data-stu-id="48988-2656">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="48988-2657">Corrigidas as exceções de andamento da implantação</span><span class="sxs-lookup"><span data-stu-id="48988-2657">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="48988-2658">Usar o ponto de extremidade do ARM da nuvem atual para criar cliente da assinatura</span><span class="sxs-lookup"><span data-stu-id="48988-2658">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="48988-2659">Melhor manipulação simultânea do arquivo clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="48988-2659">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="48988-2660">Atualização da ID de solicitação do cliente para cada execução de comando</span><span class="sxs-lookup"><span data-stu-id="48988-2660">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="48988-2661">Criar clientes de assinatura com o perfil correto do SDK (#3635)</span><span class="sxs-lookup"><span data-stu-id="48988-2661">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="48988-2662">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="48988-2662">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="48988-2663">Adicionado suporte para escolher campos de saída da tabela através da consulta JMESpath (#3581)</span><span class="sxs-lookup"><span data-stu-id="48988-2663">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="48988-2664">Aprimoramento da desativação de áudio de argumentos de análise e da adição do histórico com gestos (#3434)</span><span class="sxs-lookup"><span data-stu-id="48988-2664">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="48988-2665">Criar clientes de assinatura com o perfil correto do SDK</span><span class="sxs-lookup"><span data-stu-id="48988-2665">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="48988-2666">Mover todos os arquivos existentes de gravação para a pasta mais recente</span><span class="sxs-lookup"><span data-stu-id="48988-2666">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="48988-2667">Corrigida a idempotência para a criação de VM/VMSS (#3586)</span><span class="sxs-lookup"><span data-stu-id="48988-2667">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="48988-2668">Os caminhos de comando não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="48988-2668">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="48988-2669">Determinados parâmetros do tipo booliano não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="48988-2669">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="48988-2670">Suporte para logon do ADFS em um servidor local como o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="48988-2670">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="48988-2671">Corrigidas as gravações simultâneas para clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="48988-2671">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="48988-2672">ACR</span><span class="sxs-lookup"><span data-stu-id="48988-2672">ACR</span></span>

* <span data-ttu-id="48988-2673">Adicionado o comando `show-usage` para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="48988-2673">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="48988-2674">Suporte para atualização do SKU para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="48988-2674">Support SKU update for managed registries</span></span>
* <span data-ttu-id="48988-2675">Adicionados registros gerenciados com o SKU gerenciado</span><span class="sxs-lookup"><span data-stu-id="48988-2675">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="48988-2676">Adicionados webhooks para registros gerenciados com o módulo de comando de webhook do ACR</span><span class="sxs-lookup"><span data-stu-id="48988-2676">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="48988-2677">Adicionada autenticação do AAD com o comando de logon de ACR</span><span class="sxs-lookup"><span data-stu-id="48988-2677">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="48988-2678">Adicionado comando de exclusão para marcas, manifestos e repositórios do Docker</span><span class="sxs-lookup"><span data-stu-id="48988-2678">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="48988-2679">ACS</span><span class="sxs-lookup"><span data-stu-id="48988-2679">ACS</span></span>

* <span data-ttu-id="48988-2680">Suporte para a API versão 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="48988-2680">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="48988-2681">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-2681">Appservice</span></span>

* <span data-ttu-id="48988-2682">Corrigido o bug onde listar o aplicativo Web Linux não retornava nada</span><span class="sxs-lookup"><span data-stu-id="48988-2682">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="48988-2683">Suporte para recuperar credenciais de ACR</span><span class="sxs-lookup"><span data-stu-id="48988-2683">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="48988-2684">Remover todos os comandos em `appservice web`</span><span class="sxs-lookup"><span data-stu-id="48988-2684">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="48988-2685">Ocultar as senhas de registro do Docker da saída do comando (#3656)</span><span class="sxs-lookup"><span data-stu-id="48988-2685">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="48988-2686">Verifique se o navegador padrão é usado no macOS sem erros (#3623)</span><span class="sxs-lookup"><span data-stu-id="48988-2686">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="48988-2687">Aprimorada a Ajuda de `webapp log tail` e `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="48988-2687">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="48988-2688">Exposto o comando `traffic-routing` para configurar roteamento estático (#3566)</span><span class="sxs-lookup"><span data-stu-id="48988-2688">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="48988-2689">Adicionadas correções de confiabilidade na configuração de controle do código-fonte (#3245)</span><span class="sxs-lookup"><span data-stu-id="48988-2689">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="48988-2690">Removido o argumento `--node-version` sem suporte de `webapp config update` para aplicativos Web do Windows.</span><span class="sxs-lookup"><span data-stu-id="48988-2690">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="48988-2691">Em vez disso, use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="48988-2691">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="48988-2692">Lote</span><span class="sxs-lookup"><span data-stu-id="48988-2692">Batch</span></span>

* <span data-ttu-id="48988-2693">Atualizado para o Lote SDK 3.0.0 com suporte para VMs de baixa prioridade em pools</span><span class="sxs-lookup"><span data-stu-id="48988-2693">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="48988-2694">Opção `pool create` renomeada como `--target-dedicated` para `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="48988-2694">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="48988-2695">Adicionadas as opções `pool create` e `--target-low-priority-nodes` de `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="48988-2695">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="48988-2696">CDN</span><span class="sxs-lookup"><span data-stu-id="48988-2696">CDN</span></span>

* <span data-ttu-id="48988-2697">Uma mensagem de erro mais adequada foi fornecida para `cdn endpoint list` quando o perfil especificado por `--profile-name` não existir</span><span class="sxs-lookup"><span data-stu-id="48988-2697">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="48988-2698">Nuvem</span><span class="sxs-lookup"><span data-stu-id="48988-2698">Cloud</span></span>

* <span data-ttu-id="48988-2699">Alterada a versão de API do ponto de extremidade de metadados de nuvem para o formato AAAA-MM-DD</span><span class="sxs-lookup"><span data-stu-id="48988-2699">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="48988-2700">Ponto de extremidade da galeria não é necessário</span><span class="sxs-lookup"><span data-stu-id="48988-2700">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="48988-2701">Suporte para registrar a nuvem somente com o ponto de extremidade de gerenciador de recursos do ARM</span><span class="sxs-lookup"><span data-stu-id="48988-2701">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="48988-2702">Fornecida uma opção para `cloud set` para escolher o perfil ao selecionar a nuvem atual</span><span class="sxs-lookup"><span data-stu-id="48988-2702">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="48988-2703">Exposto `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="48988-2703">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="48988-2704">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="48988-2704">CosmosDB</span></span>

* <span data-ttu-id="48988-2705">Corrigida a permissão para criação de coleção com chave de partição personalizada</span><span class="sxs-lookup"><span data-stu-id="48988-2705">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="48988-2706">Adicionado suporte para o TTL padrão de coleção</span><span class="sxs-lookup"><span data-stu-id="48988-2706">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="48988-2707">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="48988-2707">Data Lake Analytics</span></span>

* <span data-ttu-id="48988-2708">Adicionados comandos para gerenciamento de política de computação sob o título `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="48988-2708">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="48988-2709">Adicionado `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="48988-2709">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="48988-2710">Adicionado `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="48988-2710">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="48988-2711">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="48988-2711">Data Lake Store</span></span>

* <span data-ttu-id="48988-2712">Adicionado suporte para a rotação de chave de cofre de chaves gerenciado do usuário em `dls account update`</span><span class="sxs-lookup"><span data-stu-id="48988-2712">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="48988-2713">Atualizada a versão SDK do sistema de arquivos do Data Lake Store subjacente para resolver um problema de desempenho</span><span class="sxs-lookup"><span data-stu-id="48988-2713">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="48988-2714">Adicionado o comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="48988-2714">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="48988-2715">Esse comando tenta permitir que um Cofre de Chaves fornecido pelo usuário use a criptografia de dados em uma conta do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="48988-2715">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="48988-2716">Interativo</span><span class="sxs-lookup"><span data-stu-id="48988-2716">Interactive</span></span>

* <span data-ttu-id="48988-2717">Melhor tempo de inicialização, usando comandos em cache</span><span class="sxs-lookup"><span data-stu-id="48988-2717">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="48988-2718">Maior cobertura de teste</span><span class="sxs-lookup"><span data-stu-id="48988-2718">Increased test coverage</span></span>
* <span data-ttu-id="48988-2719">Aprimorado o gesto “?” para injetar também o próximo comando</span><span class="sxs-lookup"><span data-stu-id="48988-2719">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="48988-2720">Corrigidos os erros interativos com o perfil 2017-03-09-profile-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="48988-2720">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="48988-2721">Permitido `--version` como um parâmetro para o modo interativo (#3645)</span><span class="sxs-lookup"><span data-stu-id="48988-2721">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="48988-2722">Impedir que o modo interativo gere erros de conclusões de validação (#3570)</span><span class="sxs-lookup"><span data-stu-id="48988-2722">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="48988-2723">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="48988-2723">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="48988-2724">Adicionado o sinalizador `--progress`</span><span class="sxs-lookup"><span data-stu-id="48988-2724">Added `--progress` flag</span></span>
* <span data-ttu-id="48988-2725">Removidos `--debug` e `--verbose` de conclusões</span><span class="sxs-lookup"><span data-stu-id="48988-2725">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="48988-2726">Removido `interactive` de conclusões (#3324)</span><span class="sxs-lookup"><span data-stu-id="48988-2726">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="48988-2727">IoT</span><span class="sxs-lookup"><span data-stu-id="48988-2727">IoT</span></span>

* <span data-ttu-id="48988-2728">A criação de uma política não limpa as políticas existentes.</span><span class="sxs-lookup"><span data-stu-id="48988-2728">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="48988-2729">(#3934)</span><span class="sxs-lookup"><span data-stu-id="48988-2729">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="48988-2730">Cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="48988-2730">Key vault</span></span>

* <span data-ttu-id="48988-2731">Comandos adicionados para recursos de recuperação do cofre de chaves:</span><span class="sxs-lookup"><span data-stu-id="48988-2731">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="48988-2732">Subcomandos `purge`, `recover`, `keyvault list-deleted` de `keyvault`</span><span class="sxs-lookup"><span data-stu-id="48988-2732">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="48988-2733">Subcomandos `backup`, `restore`, `purge`, `recover`, `list-deleted` de `keyvault secret`</span><span class="sxs-lookup"><span data-stu-id="48988-2733">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="48988-2734">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault certificate`</span><span class="sxs-lookup"><span data-stu-id="48988-2734">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="48988-2735">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault key`</span><span class="sxs-lookup"><span data-stu-id="48988-2735">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="48988-2736">Adicionada a integração do cofre de chaves da entidade de serviço (#3133)</span><span class="sxs-lookup"><span data-stu-id="48988-2736">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="48988-2737">Atualizado o plano de dados de cofre de chaves para 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="48988-2737">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="48988-2738">(#3307)</span><span class="sxs-lookup"><span data-stu-id="48988-2738">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="48988-2739">Laboratório</span><span class="sxs-lookup"><span data-stu-id="48988-2739">Lab</span></span>

* <span data-ttu-id="48988-2740">Adicionado o suporte para reivindicar qualquer VM no laboratório através de `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="48988-2740">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="48988-2741">Adicionado o formatador de saída da tabela para `az lab vm list` e `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="48988-2741">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="48988-2742">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="48988-2742">Monitor</span></span>

* <span data-ttu-id="48988-2743">Correção para o arquivo de modelo com o comando `monitor autoscale-settings get-parameters-template` (#3349)</span><span class="sxs-lookup"><span data-stu-id="48988-2743">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="48988-2744">`monitor alert-rule-incidents list` renomeado para `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="48988-2744">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="48988-2745">`monitor alert-rule-incidents show` renomeado para `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="48988-2745">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="48988-2746">`monitor metric-defintions list` renomeado para `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="48988-2746">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="48988-2747">`monitor alert-rules` renomeado para `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="48988-2747">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="48988-2748">Alterado `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="48988-2748">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="48988-2749">Os subcomandos `condition` e `action` não aceitarão mais JSON</span><span class="sxs-lookup"><span data-stu-id="48988-2749">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="48988-2750">Adicionar vários parâmetros para simplificar o processo de criação de regra</span><span class="sxs-lookup"><span data-stu-id="48988-2750">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="48988-2751">`location` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="48988-2751">`location` no longer required</span></span>
  * <span data-ttu-id="48988-2752">Adicionar nome e o suporte a ID de destino</span><span class="sxs-lookup"><span data-stu-id="48988-2752">Add name and ID support for target</span></span>
  * <span data-ttu-id="48988-2753">Remover `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="48988-2753">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="48988-2754">Renomear `is-enabled` para `enabled` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="48988-2754">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="48988-2755">Padrões de `description` agora baseados na condição fornecida</span><span class="sxs-lookup"><span data-stu-id="48988-2755">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="48988-2756">Adicionar exemplos para ajudar a esclarecer o novo formato</span><span class="sxs-lookup"><span data-stu-id="48988-2756">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="48988-2757">Suporte para nomes ou IDs para comandos `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="48988-2757">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="48988-2758">Exemplos e argumentos de conveniência adicionados ao `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="48988-2758">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="48988-2759">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-2759">Network</span></span>

* <span data-ttu-id="48988-2760">Adicionado o comando `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="48988-2760">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="48988-2761">Adicionado argumento `--private-access-services` para `vnet subnet create` e `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="48988-2761">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="48988-2762">Corrigido o problema onde `application-gateway redirect-config create` falhava</span><span class="sxs-lookup"><span data-stu-id="48988-2762">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="48988-2763">Corrigido o problema onde `application-gateway redirect-config update` com `--no-wait` não funcionava</span><span class="sxs-lookup"><span data-stu-id="48988-2763">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="48988-2764">Corrigido o bug ao usar o argumento `--servers` com `application-gateway address-pool create` e `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="48988-2764">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="48988-2765">Adicionados os comandos `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="48988-2765">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="48988-2766">Adicionados os comandos para `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="48988-2766">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="48988-2767">Adicionados os argumentos para `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="48988-2767">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="48988-2768">Adicionados os argumentos para `application-gateway http-settings create` e `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="48988-2768">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="48988-2769">Adicionados os argumentos para `application-gateway url-path-map create` e `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="48988-2769">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="48988-2770">Adicionado o argumento `--redirect-config` para `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="48988-2770">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="48988-2771">Adicionado o suporte ao `--no-wait` para `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="48988-2771">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="48988-2772">Adicionados os argumentos para `application-gateway probe create` e `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="48988-2772">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="48988-2773">Adicionado o argumento `--redirect-config` para `application-gateway rule create` e `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="48988-2773">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="48988-2774">Adicionado o suporte ao `--accelerated-networking` para `nic create` e `nic update`</span><span class="sxs-lookup"><span data-stu-id="48988-2774">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="48988-2775">Removido o argumento `--internal-dns-name-suffix` de `nic create`</span><span class="sxs-lookup"><span data-stu-id="48988-2775">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="48988-2776">Adicionado o suporte ao `--dns-servers` para `nic update` e `nic create`: Adicionar suporte para --dns-servers</span><span class="sxs-lookup"><span data-stu-id="48988-2776">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="48988-2777">Corrigido o bug onde `local-gateway create` ignorava `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="48988-2777">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="48988-2778">Adicionado o suporte ao `--dns-servers` para `vnet update`</span><span class="sxs-lookup"><span data-stu-id="48988-2778">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="48988-2779">Corrigido o bug ao criar um emparelhamento sem filtragem de rotas com `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="48988-2779">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="48988-2780">Corrigido o bug onde os argumentos `--provider` e `--bandwidth` não funcionavam com `express-route update`</span><span class="sxs-lookup"><span data-stu-id="48988-2780">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="48988-2781">Corrigido o bug com a lógica padrão de `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="48988-2781">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="48988-2782">Aprimorada a formatação de saída para `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="48988-2782">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="48988-2783">Usar IP de front-end padrão para `application-gateway http-listener create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="48988-2783">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="48988-2784">Usar o pool padrão de endereços, configurações de HTTP e o ouvinte HTTP para `application-gateway rule create`, se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="48988-2784">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="48988-2785">Usar IP de front-end e pool de back-end padrão para `lb rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="48988-2785">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="48988-2786">Usar IP de front-end padrão para `lb inbound-nat-rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="48988-2786">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="48988-2787">Perfil</span><span class="sxs-lookup"><span data-stu-id="48988-2787">Profile</span></span>

* <span data-ttu-id="48988-2788">Suporte a logon em uma VM com uma identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="48988-2788">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="48988-2789">Suporte a saída para `account show` em formato de arquivo de autenticação do SDK</span><span class="sxs-lookup"><span data-stu-id="48988-2789">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="48988-2790">Mostrar avisos de código obsoleto ao usar o “modo de exibição expandido”</span><span class="sxs-lookup"><span data-stu-id="48988-2790">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="48988-2791">Adicionado o comando `get-access-token` para fornecer o token bruto do AAD</span><span class="sxs-lookup"><span data-stu-id="48988-2791">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="48988-2792">Suporte a logon com uma conta de usuário sem nenhuma assinatura associada</span><span class="sxs-lookup"><span data-stu-id="48988-2792">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="48988-2793">RDBMS</span><span class="sxs-lookup"><span data-stu-id="48988-2793">RDBMS</span></span>

* <span data-ttu-id="48988-2794">Suporte para listar servidores em uma assinatura (#3417)</span><span class="sxs-lookup"><span data-stu-id="48988-2794">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="48988-2795">Corrigido o `%s` não processado devido à ausência de `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="48988-2795">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="48988-2796">Corrigido o mapa do código-fonte do documento e adicionada a tarefa CI para verificação (#3361)</span><span class="sxs-lookup"><span data-stu-id="48988-2796">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="48988-2797">Corrigida a ajuda de MySQL e PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="48988-2797">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="48988-2798">Recurso</span><span class="sxs-lookup"><span data-stu-id="48988-2798">Resource</span></span>

* <span data-ttu-id="48988-2799">Aprimorados os prompts para parâmetros ausentes para `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="48988-2799">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="48988-2800">Aprimorada a análise da sintaxe `--parameters KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="48988-2800">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="48988-2801">Corrigidos os problemas onde os arquivos de parâmetros `group deployment create` não eram mais reconhecidos usando a sintaxe `@<file>`</span><span class="sxs-lookup"><span data-stu-id="48988-2801">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="48988-2802">Suporte do argumento `--ids` para os comandos `resource` e `managedapp`</span><span class="sxs-lookup"><span data-stu-id="48988-2802">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="48988-2803">Corrigidas algumas mensagens de erro e análise (#3584)</span><span class="sxs-lookup"><span data-stu-id="48988-2803">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="48988-2804">Corrigida a análise de `--resource-type` para o comando `lock` aceitar `<resource-namespace>` e `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="48988-2804">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="48988-2805">Adicionados parâmetros de verificação para modelos de link do modelo (#3629)</span><span class="sxs-lookup"><span data-stu-id="48988-2805">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="48988-2806">Adicionado suporte para especificar parâmetros de implantação usando a sintaxe `KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="48988-2806">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="48988-2807">Função</span><span class="sxs-lookup"><span data-stu-id="48988-2807">Role</span></span>

* <span data-ttu-id="48988-2808">Suporte à saída no formato de arquivo de autenticação do SDK para `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="48988-2808">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="48988-2809">Limpar as atribuições de função e aplicativos relacionados ao AAD ao excluir uma entidade de serviço (#3610)</span><span class="sxs-lookup"><span data-stu-id="48988-2809">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="48988-2810">Incluir o formato de hora nos argumentos `app create` e descrições `--start-date` e `--end-date`</span><span class="sxs-lookup"><span data-stu-id="48988-2810">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="48988-2811">Mostrar avisos de código obsoleto ao usar `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="48988-2811">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="48988-2812">Adicionada a integração do cofre de chaves para os comandos `create-for-rbac` e `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="48988-2812">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="48988-2813">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="48988-2813">Service Fabric</span></span>
* <span data-ttu-id="48988-2814">Corrigido um problema com arquivos grandes em aplicativos que eram truncados ao serem carregados (#3666)</span><span class="sxs-lookup"><span data-stu-id="48988-2814">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="48988-2815">Adicionados testes para os comandos do Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="48988-2815">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="48988-2816">Corrigidos vários comandos do Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="48988-2816">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="48988-2817">SQL</span><span class="sxs-lookup"><span data-stu-id="48988-2817">SQL</span></span>

* <span data-ttu-id="48988-2818">Removido o parâmetro `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="48988-2818">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="48988-2819">Remover os valores de senha da saída dos comandos `sql server create` e `sql server update`</span><span class="sxs-lookup"><span data-stu-id="48988-2819">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="48988-2820">Adicionados os comandos para `sql db list-editions` e `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="48988-2820">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="48988-2821">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48988-2821">Storage</span></span>

* <span data-ttu-id="48988-2822">Removida a opção `--marker` dos comandos `storage blob list`, `storage container list`, e `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="48988-2822">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="48988-2823">Habilitado a criação de uma conta de armazenamento somente para https</span><span class="sxs-lookup"><span data-stu-id="48988-2823">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="48988-2824">Atualizadas as métricas de armazenamento, registro em log e os comandos do CORS (#3495)</span><span class="sxs-lookup"><span data-stu-id="48988-2824">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="48988-2825">Mensagem de exceção reformulada do ADD do CORS adicionar (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="48988-2825">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="48988-2826">Convertido o gerador para uma lista no modo de simulação de comando do lote de download (#3592)</span><span class="sxs-lookup"><span data-stu-id="48988-2826">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="48988-2827">Corrigido o problema de simulação do lote de download de blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="48988-2827">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="48988-2828">VM</span><span class="sxs-lookup"><span data-stu-id="48988-2828">VM</span></span>

* <span data-ttu-id="48988-2829">Suporte para configuração de NSG</span><span class="sxs-lookup"><span data-stu-id="48988-2829">Support configuring nsg</span></span>
* <span data-ttu-id="48988-2830">Corrigido o bug onde o servidor DNS não era configurado corretamente</span><span class="sxs-lookup"><span data-stu-id="48988-2830">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="48988-2831">Suporte às identidades de serviço gerenciado</span><span class="sxs-lookup"><span data-stu-id="48988-2831">Support managed service identities</span></span>
* <span data-ttu-id="48988-2832">Corrigido o problema onde `cmss create` com um balanceador de carga existente exigia `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="48988-2832">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="48988-2833">Os discos de dados criados com LUN do `vm image create` agora começam com 0</span><span class="sxs-lookup"><span data-stu-id="48988-2833">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="48988-2834">10 de maio de 2017</span><span class="sxs-lookup"><span data-stu-id="48988-2834">May 10, 2017</span></span>

<span data-ttu-id="48988-2835">Versão 2.0.6</span><span class="sxs-lookup"><span data-stu-id="48988-2835">Version 2.0.6</span></span>

* <span data-ttu-id="48988-2836">Renomeação do DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="48988-2836">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="48988-2837">Adição do RDBMS (MySQL, Postgres)</span><span class="sxs-lookup"><span data-stu-id="48988-2837">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="48988-2838">Inclusão dos módulos Data Lake Analytics e Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="48988-2838">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="48988-2839">Inclusão do módulo Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="48988-2839">Include Cognitive Services module</span></span>
* <span data-ttu-id="48988-2840">Inclusão do módulo Service Fabric</span><span class="sxs-lookup"><span data-stu-id="48988-2840">Include Service Fabric module</span></span>
* <span data-ttu-id="48988-2841">Inclusão do módulo Interativo (renomeação de az-shell)</span><span class="sxs-lookup"><span data-stu-id="48988-2841">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="48988-2842">Adição de suporte para comandos CDN</span><span class="sxs-lookup"><span data-stu-id="48988-2842">Add support for CDN commands</span></span>
* <span data-ttu-id="48988-2843">Remoção do módulo Contêiner</span><span class="sxs-lookup"><span data-stu-id="48988-2843">Remove Container module</span></span>
* <span data-ttu-id="48988-2844">Adição de “az -v” como atalho para “az --version” ([nº 2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="48988-2844">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="48988-2845">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="48988-2845">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="48988-2846">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48988-2846">Core</span></span>

* <span data-ttu-id="48988-2847">núcleo: captura de exceções causadas por um provedor não registrado e seu registro automático</span><span class="sxs-lookup"><span data-stu-id="48988-2847">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="48988-2848">desempenho: persistência do cache de tokens do ADAL na memória até o encerramento do processo ([nº 2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="48988-2848">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="48988-2849">Correção de bytes retornados da impressão digital hexadecimal -o tsv ([nº 3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="48988-2849">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="48988-2850">Melhoria do download do Certificado do Key Vault e da integração de SP do AAD ([nº 3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="48988-2850">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="48988-2851">Adição da localização do Python a “az —version” ([nº 2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="48988-2851">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="48988-2852">logon: suporte ao logon quando não há nenhuma assinatura ([nº 2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="48988-2852">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="48988-2853">núcleo: correção de uma falha ao fazer logon usando uma entidade de serviço duas vezes ([nº 2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="48988-2853">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="48988-2854">núcleo: permitir que o caminho do arquivo accessTokens.json seja configurável por meio de uma variável de ambiente ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="48988-2854">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="48988-2855">núcleo: permitir que padrões configurados sejam aplicados em argumentos opcionais ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="48988-2855">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="48988-2856">núcleo: desempenho aprimorado</span><span class="sxs-lookup"><span data-stu-id="48988-2856">core: Improved performance</span></span>
* <span data-ttu-id="48988-2857">núcleo: certificados de AC personalizados – suporte à configuração da variável de ambiente REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="48988-2857">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="48988-2858">núcleo: configuração na nuvem – uso do ponto de extremidade do “Resource Manager” caso o ponto de extremidade de “Gerenciamento” não esteja definido</span><span class="sxs-lookup"><span data-stu-id="48988-2858">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="48988-2859">ACS</span><span class="sxs-lookup"><span data-stu-id="48988-2859">ACS</span></span>

* <span data-ttu-id="48988-2860">correção da contagem mestre e de agente para ser inteiro em vez de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="48988-2860">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="48988-2861">exposição de “az acs create --no-wait” e “az acs wait” para a criação assíncrona</span><span class="sxs-lookup"><span data-stu-id="48988-2861">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="48988-2862">exposição de “az acs create --validate” para validações de simulação</span><span class="sxs-lookup"><span data-stu-id="48988-2862">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="48988-2863">remoção do perfil do Windows antes da chamada PUT ao comando scale ([nº 2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="48988-2863">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="48988-2864">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-2864">AppService</span></span>

* <span data-ttu-id="48988-2865">functionapp: adição de suportes completos a functionapp, incluindo create, show, list, delete, hostname, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="48988-2865">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="48988-2866">Adição do VSTS (Team Services) como uma opção de entrega contínua a “appservice web source-control config”</span><span class="sxs-lookup"><span data-stu-id="48988-2866">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="48988-2867">Criação de “az webapp” para substituição de “az appservice web” (para compatibilidade com versões anteriores, “az appservice web” permanecerá por duas versões)</span><span class="sxs-lookup"><span data-stu-id="48988-2867">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="48988-2868">Exposição de argumentos para configurar a implantação e as “pilhas em runtime” em webapp create</span><span class="sxs-lookup"><span data-stu-id="48988-2868">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="48988-2869">Exposição de “webapp list-runtimes”</span><span class="sxs-lookup"><span data-stu-id="48988-2869">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="48988-2870">suporte à configuração de cadeias de conexão ([nº 2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="48988-2870">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="48988-2871">suporte à permuta de slots com visualização</span><span class="sxs-lookup"><span data-stu-id="48988-2871">support slot swap with preview</span></span>
* <span data-ttu-id="48988-2872">Correção de erros em comandos appservice ([nº 2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="48988-2872">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="48988-2873">Uso do grupo de recursos do plano do serviço de aplicativo para operações de certificado ([nº 2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="48988-2873">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="48988-2874">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="48988-2874">CosmosDB</span></span>

* <span data-ttu-id="48988-2875">Renomeação do módulo DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="48988-2875">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="48988-2876">Adição de suporte para APIs do plano de dados do DocumentDB: gerenciamento de banco de dados e de coleção</span><span class="sxs-lookup"><span data-stu-id="48988-2876">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="48988-2877">Adição de suporte para habilitar o failover automático em contas de banco de dados</span><span class="sxs-lookup"><span data-stu-id="48988-2877">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="48988-2878">Adição de suporte para nova política de consistência ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="48988-2878">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="48988-2879">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="48988-2879">Data Lake Analytics</span></span>

* <span data-ttu-id="48988-2880">Correção de um bug em que a filtragem no resultado e no estado das listas de trabalho gera um erro</span><span class="sxs-lookup"><span data-stu-id="48988-2880">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="48988-2881">Adição de suporte para o novo tipo de item de catálogo: pacote.</span><span class="sxs-lookup"><span data-stu-id="48988-2881">Add support for new catalog item type: package.</span></span> <span data-ttu-id="48988-2882">acessado por meio de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="48988-2882">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="48988-2883">Possibilidade de listar os seguintes itens de catálogo no banco de dados (sem a necessidade de especificação de esquema):</span><span class="sxs-lookup"><span data-stu-id="48988-2883">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="48988-2884">Tabela</span><span class="sxs-lookup"><span data-stu-id="48988-2884">Table</span></span>
  * <span data-ttu-id="48988-2885">Função com valor de tabela</span><span class="sxs-lookup"><span data-stu-id="48988-2885">Table valued function</span></span>
  * <span data-ttu-id="48988-2886">Visualizar</span><span class="sxs-lookup"><span data-stu-id="48988-2886">View</span></span>
  * <span data-ttu-id="48988-2887">Estatísticas de Tabela.</span><span class="sxs-lookup"><span data-stu-id="48988-2887">Table Statistics.</span></span> <span data-ttu-id="48988-2888">Isso também pode ser listado com um esquema, mas sem a especificação de um nome de tabela</span><span class="sxs-lookup"><span data-stu-id="48988-2888">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="48988-2889">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="48988-2889">Data Lake Store</span></span>

* <span data-ttu-id="48988-2890">Atualização da versão do SDK do sistema de arquivos subjacente, que fornece melhor suporte para lidar com cenários de limitação do servidor</span><span class="sxs-lookup"><span data-stu-id="48988-2890">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="48988-2891">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="48988-2891">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="48988-2892">Ausência de ajuda para mostrar o acesso.</span><span class="sxs-lookup"><span data-stu-id="48988-2892">missed help for access show.</span></span> <span data-ttu-id="48988-2893">Adição em andamento.</span><span class="sxs-lookup"><span data-stu-id="48988-2893">adding it.</span></span> <span data-ttu-id="48988-2894">([nº 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="48988-2894">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="48988-2895">Localizar</span><span class="sxs-lookup"><span data-stu-id="48988-2895">Find</span></span>

* <span data-ttu-id="48988-2896">melhoria dos resultados da pesquisa e permissão de controle de versão do índice de pesquisa</span><span class="sxs-lookup"><span data-stu-id="48988-2896">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="48988-2897">KeyVault</span><span class="sxs-lookup"><span data-stu-id="48988-2897">KeyVault</span></span>

* <span data-ttu-id="48988-2898">BC:`az keyvault certificate download` alteração de -e da cadeia de caracteres ou do binário para PEM ou DER a fim de representar melhor as opções</span><span class="sxs-lookup"><span data-stu-id="48988-2898">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="48988-2899">BC: remoção de --expires e --not-before de `keyvault certificate create`, pois estes parâmetros não têm suporte no serviço</span><span class="sxs-lookup"><span data-stu-id="48988-2899">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="48988-2900">Adição do parâmetro --validity a `keyvault certificate create` para substituir seletivamente o valor em --policy</span><span class="sxs-lookup"><span data-stu-id="48988-2900">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="48988-2901">Correção do problema em `keyvault certificate get-default-policy`, em que “expires” e “not_before” eram expostos, ao contrário de “validity_in_months”</span><span class="sxs-lookup"><span data-stu-id="48988-2901">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="48988-2902">Correção do cofre de chaves para importação de PEM e PFX ([nº 2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="48988-2902">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="48988-2903">Laboratório</span><span class="sxs-lookup"><span data-stu-id="48988-2903">Lab</span></span>

* <span data-ttu-id="48988-2904">Adição dos comandos create, show, delete e list ao ambiente do laboratório</span><span class="sxs-lookup"><span data-stu-id="48988-2904">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="48988-2905">Adição dos comandos show e list para exibir modelos ARM no laboratório</span><span class="sxs-lookup"><span data-stu-id="48988-2905">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="48988-2906">Adição do sinalizador --environment a `az lab vm list` para filtrar as VMs por ambiente no laboratório</span><span class="sxs-lookup"><span data-stu-id="48988-2906">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="48988-2907">Adição do comando de conveniência `az lab formula export-artifacts` para exportar o scaffold de artefato em uma fórmula do Laboratório</span><span class="sxs-lookup"><span data-stu-id="48988-2907">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="48988-2908">Adição de comandos para gerenciar segredos em um Laboratório</span><span class="sxs-lookup"><span data-stu-id="48988-2908">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="48988-2909">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="48988-2909">Monitor</span></span>

* <span data-ttu-id="48988-2910">Correção de bug: modelagem de `--actions` de `az alert-rules create` para consumir a cadeia de caracteres JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="48988-2910">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="48988-2911">Correção de bug – as configurações de diagnóstico criam, mas não aceitam logs e métrica de comandos show ([nº 2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="48988-2911">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="48988-2912">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-2912">Network</span></span>

* <span data-ttu-id="48988-2913">Adição do comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="48988-2913">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="48988-2914">Adição de suporte para o parâmetro `--filters` de `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="48988-2914">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="48988-2915">Adição de suporte para drenagem de conexão do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="48988-2915">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="48988-2916">Adição de suporte para a configuração do conjunto de regras WAF do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="48988-2916">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="48988-2917">Adição de suporte para filtros de rota e regras do ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="48988-2917">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="48988-2918">Adição de suporte para o roteamento geográfico do Gerenciador de Tráfego</span><span class="sxs-lookup"><span data-stu-id="48988-2918">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="48988-2919">Adição de suporte para seletores de tráfego baseados em política da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="48988-2919">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="48988-2920">Adição de suporte para políticas IPsec da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="48988-2920">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="48988-2921">Correção de um bug com `vpn-connection create` ao usar os parâmetros `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="48988-2921">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="48988-2922">Adição de suporte para gateways de VNet ativos/ativos</span><span class="sxs-lookup"><span data-stu-id="48988-2922">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="48988-2923">Remoção de valores nulos na saída de comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="48988-2923">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="48988-2924">BC: corrigido um bug na saída de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="48988-2924">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="48988-2925">Correção de um bug em que o argumento “--key-length” de “vpn-connection create” não é analisado corretamente</span><span class="sxs-lookup"><span data-stu-id="48988-2925">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="48988-2926">Correção de um bug em `dns zone import`, em que os registros não são importados corretamente</span><span class="sxs-lookup"><span data-stu-id="48988-2926">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="48988-2927">Correção de um bug em que `traffic-manager endpoint update` não funciona</span><span class="sxs-lookup"><span data-stu-id="48988-2927">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="48988-2928">Adição de comandos de visualização “network watcher”</span><span class="sxs-lookup"><span data-stu-id="48988-2928">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="48988-2929">Perfil</span><span class="sxs-lookup"><span data-stu-id="48988-2929">Profile</span></span>

* <span data-ttu-id="48988-2930">Suporte ao logon quando não há nenhuma assinatura encontrada ([nº 2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="48988-2930">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="48988-2931">Suporte ao nome curto do parâmetro em az account set --subscription ([nº 2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="48988-2931">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="48988-2932">Redis</span><span class="sxs-lookup"><span data-stu-id="48988-2932">Redis</span></span>

* <span data-ttu-id="48988-2933">Adição do comando update que também adiciona a capacidade de dimensionar o Cache Redis</span><span class="sxs-lookup"><span data-stu-id="48988-2933">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="48988-2934">Preterição do comando “update-settings”</span><span class="sxs-lookup"><span data-stu-id="48988-2934">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="48988-2935">Recurso</span><span class="sxs-lookup"><span data-stu-id="48988-2935">Resource</span></span>

* <span data-ttu-id="48988-2936">Adição dos comandos de definição managedapp e managedapp ([nº 2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="48988-2936">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="48988-2937">Suporte aos comandos “provider operation” ([nº 2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="48988-2937">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="48988-2938">Suporte à criação de recurso genérico ([nº 2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="48988-2938">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="48988-2939">Correção da análise de recurso e da pesquisa de versão de API.</span><span class="sxs-lookup"><span data-stu-id="48988-2939">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="48988-2940">([nº 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="48988-2940">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="48988-2941">Adição de documentos a az lock update.</span><span class="sxs-lookup"><span data-stu-id="48988-2941">Add docs for az lock update.</span></span> <span data-ttu-id="48988-2942">([nº 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="48988-2942">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="48988-2943">Erro ao tentar listar recursos de um grupo que não existe.</span><span class="sxs-lookup"><span data-stu-id="48988-2943">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="48988-2944">([nº 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="48988-2944">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="48988-2945">[Computação] Correção de problemas com a atualização do conjunto de disponibilidade da VMSS e da VM.</span><span class="sxs-lookup"><span data-stu-id="48988-2945">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="48988-2946">([nº 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="48988-2946">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="48988-2947">Correção de lock create e delete se parent-resource-path é None ([nº 2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="48988-2947">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="48988-2948">Função</span><span class="sxs-lookup"><span data-stu-id="48988-2948">Role</span></span>

* <span data-ttu-id="48988-2949">create-for-rbac: garantia de que a data de término do SP não excederá a data de validade do certificado ([nº 2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="48988-2949">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="48988-2950">RBAC: adição de suporte completo a “ad group” ([nº 2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="48988-2950">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="48988-2951">função: correção de problemas na atualização de definição de função ([nº 2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="48988-2951">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="48988-2952">create-for-rbac: garantia de que a senha fornecida pelo usuário é coletada</span><span class="sxs-lookup"><span data-stu-id="48988-2952">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="48988-2953">SQL</span><span class="sxs-lookup"><span data-stu-id="48988-2953">SQL</span></span>

* <span data-ttu-id="48988-2954">Adição dos comandos az sql server list-usages e az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="48988-2954">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="48988-2955">SQL – capacidade de se conectar diretamente ao provedor de recursos ([nº 2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="48988-2955">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="48988-2956">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48988-2956">Storage</span></span>

* <span data-ttu-id="48988-2957">Localização padrão da localização do grupo de recursos de `storage account create`</span><span class="sxs-lookup"><span data-stu-id="48988-2957">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="48988-2958">Adição de suporte para cópia incremental de blob</span><span class="sxs-lookup"><span data-stu-id="48988-2958">Add support for incremental blob copy</span></span>
* <span data-ttu-id="48988-2959">Adição de suporte para upload de blobs de blocos grandes</span><span class="sxs-lookup"><span data-stu-id="48988-2959">Add support for large block blob upload</span></span>
* <span data-ttu-id="48988-2960">Alteração do tamanho do bloco para 100MB quando o arquivo a ser carregado é maior que 200GB</span><span class="sxs-lookup"><span data-stu-id="48988-2960">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="48988-2961">VM</span><span class="sxs-lookup"><span data-stu-id="48988-2961">VM</span></span>

* <span data-ttu-id="48988-2962">avail-set: as contagens de domínio de UD e FD agora são opcionais</span><span class="sxs-lookup"><span data-stu-id="48988-2962">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="48988-2963">observação: em comandos da VM em nuvens soberanas, evite recursos relacionados ao disco gerenciado, incluindo os seguintes:</span><span class="sxs-lookup"><span data-stu-id="48988-2963">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="48988-2964">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="48988-2964">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="48988-2965">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="48988-2965">az vm/vmss disk</span></span>
  3. <span data-ttu-id="48988-2966">Em “az vm/vmss create”, use “—use-unmanaged-disk” para evitar o disco gerenciado Outros comandos deverão funcionar</span><span class="sxs-lookup"><span data-stu-id="48988-2966">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="48988-2967">VM/VMSS: melhoria do texto de aviso ao gerar pares de chaves SSH</span><span class="sxs-lookup"><span data-stu-id="48988-2967">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="48988-2968">VM/VMSS: suporte à criação com base em uma imagem do Marketplace que exige informações de plano ([nº 1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="48988-2968">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="48988-2969">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="48988-2969">April 3, 2017</span></span>

<span data-ttu-id="48988-2970">Versão 2.0.2</span><span class="sxs-lookup"><span data-stu-id="48988-2970">Version 2.0.2</span></span>

<span data-ttu-id="48988-2971">Lançamos os componentes ACR, Batch, KeyVault, e SQL nessa versão</span><span class="sxs-lookup"><span data-stu-id="48988-2971">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="48988-2972">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48988-2972">Core</span></span>

* <span data-ttu-id="48988-2973">Adicionar módulos acr, laboratório, monitor e localizar à lista padrão</span><span class="sxs-lookup"><span data-stu-id="48988-2973">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="48988-2974">Logon: ignorar locatário errado ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="48988-2974">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="48988-2975">logon: definir assinatura padrão como um com o estado de "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="48988-2975">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="48988-2976">Adicionar comandos de espera e suporte --no-wait para mais comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="48988-2976">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="48988-2977">núcleo: suporte a logon usando a entidade de serviço com um certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="48988-2977">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="48988-2978">Adicione solicitação para parâmetros de modelo ausentes.</span><span class="sxs-lookup"><span data-stu-id="48988-2978">Add prompting for missing template parameters.</span></span> <span data-ttu-id="48988-2979">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="48988-2979">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="48988-2980">Suporte à definição de valores padrão para os argumentos comuns como grupo de recursos padrão, Web padrão, vm padrão</span><span class="sxs-lookup"><span data-stu-id="48988-2980">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="48988-2981">Suporte a logon para um locatário específico</span><span class="sxs-lookup"><span data-stu-id="48988-2981">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="48988-2982">ACS</span><span class="sxs-lookup"><span data-stu-id="48988-2982">ACS</span></span>

* <span data-ttu-id="48988-2983">[ACS] Adicionar suporte para configurar um cluster do ACS padrão ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="48988-2983">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="48988-2984">Adicione suporte para solicitação de senha de chave ssh.</span><span class="sxs-lookup"><span data-stu-id="48988-2984">Add support for ssh key password prompting.</span></span> <span data-ttu-id="48988-2985">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="48988-2985">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="48988-2986">Adicione suporte para clusters do windows.</span><span class="sxs-lookup"><span data-stu-id="48988-2986">Add support for windows clusters.</span></span> <span data-ttu-id="48988-2987">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="48988-2987">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="48988-2988">Alterne da função Proprietário para Colaborador.</span><span class="sxs-lookup"><span data-stu-id="48988-2988">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="48988-2989">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="48988-2989">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="48988-2990">AppService</span><span class="sxs-lookup"><span data-stu-id="48988-2990">AppService</span></span>

* <span data-ttu-id="48988-2991">AppService: suporte para obter o endereço ip externo usado para registros de DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="48988-2991">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="48988-2992">AppService: suporte à associação de certificados curinga ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="48988-2992">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="48988-2993">AppService: lista de suporte à publicação de perfis ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="48988-2993">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="48988-2994">AppService - Aciona a sincronização de controle de origem após a configuração ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="48988-2994">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="48988-2995">DataLake</span><span class="sxs-lookup"><span data-stu-id="48988-2995">DataLake</span></span>

* <span data-ttu-id="48988-2996">Versão inicial do módulo do Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="48988-2996">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="48988-2997">Versão inicial do módulo do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="48988-2997">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="48988-2998">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="48988-2998">DocuemntDB</span></span>

* <span data-ttu-id="48988-2999">DocumentDB: adicionado suporte para a listagem de cadeias de conexão ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="48988-2999">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="48988-3000">VM</span><span class="sxs-lookup"><span data-stu-id="48988-3000">VM</span></span>

* <span data-ttu-id="48988-3001">[Compute] Adicionar suporte a AppGateway para criar o conjunto de dimensionamento de máquinas virtuais ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="48988-3001">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="48988-3002">[VM/VMSS] Suporte aprimorado ao cache de disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="48988-3002">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="48988-3003">VM/VMSS: incorporar a lógica de validação de credenciais usada pelo portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="48988-3003">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="48988-3004">Adicionar comandos de espera e suporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="48988-3004">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="48988-3005">Conjunto de dimensionamento de máquinas virtuais: suporte à \* para listar a exibição de instâncias em vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="48988-3005">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="48988-3006">Adicionar: segredos da VM e do conjunto de dimensionamento de máquinas virtuais ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="48988-3006">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="48988-3007">Permitir a criação de VMs com VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="48988-3007">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="48988-3008">27 de fevereiro de 2017</span><span class="sxs-lookup"><span data-stu-id="48988-3008">February 27, 2017</span></span>

<span data-ttu-id="48988-3009">Versão 2.0.0</span><span class="sxs-lookup"><span data-stu-id="48988-3009">Version 2.0.0</span></span>

<span data-ttu-id="48988-3010">Esta versão da CLI do Azure 2.0 é a primeira versão "Amplamente Disponível". A disponibilidade geral se aplica a estes módulos de comando:</span><span class="sxs-lookup"><span data-stu-id="48988-3010">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="48988-3011">Serviço de Contêiner (acs)</span><span class="sxs-lookup"><span data-stu-id="48988-3011">Container Service (acs)</span></span>
- <span data-ttu-id="48988-3012">Computação (incluindo Gerenciador de Recursos, VM, conjunto de dimensionamento de máquinas virtuais, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="48988-3012">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="48988-3013">Rede</span><span class="sxs-lookup"><span data-stu-id="48988-3013">Networking</span></span>
- <span data-ttu-id="48988-3014">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48988-3014">Storage</span></span>

<span data-ttu-id="48988-3015">Esses módulos de comando podem ser usados na produção e têm suporte do SLA padrão da Microsoft. Você pode abrir problemas diretamente com o suporte da Microsoft ou em nossa [lista de problemas do github](https://github.com/azure/azure-cli/issues/). Faça perguntas no [StackOverflow usando a marca azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contate a equipe de produto em [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) Forneça comentários na linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="48988-3015">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="48988-3016">Os comandos nesses módulos são estáveis e a sintaxe não deve ser alterada em versões futuras dessa versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="48988-3016">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="48988-3017">Para verificar a versão da CLI, use `az --version` A saída lista a versão da CLI (2.0.0 nessa versão), os módulos de comando individuais, as versões do Python e GCC que você está usando</span><span class="sxs-lookup"><span data-stu-id="48988-3017">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="48988-3018">Alguns dos módulos de comando têm um sufixo "b*n*" ou "rc*n*". Esses módulos de comando ainda estão em versão prévia e estarão disponíveis no futuro</span><span class="sxs-lookup"><span data-stu-id="48988-3018">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="48988-3019">Também temos compilações de versão prévia noturnas da CLI. Para obter informações, consulte essas instruções sobre [como obter as compilações diárias](https://github.com/Azure/azure-cli#nightly-builds) e essas instruções sobre [configuração do desenvolvedor e código de contribuição](https://github.com/Azure/azure-cli#developer-setup)</span><span class="sxs-lookup"><span data-stu-id="48988-3019">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="48988-3020">Você pode relatar problemas com as compilações de visualização diárias das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="48988-3020">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="48988-3021">Relatar problemas na [lista de problemas do github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="48988-3021">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="48988-3022">Entre em contato com a equipe do produto no endereço [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="48988-3022">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="48988-3023">Forneça comentários a partir da linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="48988-3023">Provide feedback from the command line with the `az feedback` command</span></span>

