---
title: Notas de versão da CLI do Azure
description: Saiba mais sobre as últimas atualizações da CLI do Azure
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 10/27/2020
ms.topic: article
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 4e1f03268ccd001d6fe371b1ecdecb869791b198
ms.sourcegitcommit: 1187fb75b68426c46e84b3f294c509ee7b7da9be
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/27/2020
ms.locfileid: "92687123"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="69b8c-103">Notas de versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="69b8c-103">Azure CLI release notes</span></span>

# <a name="current-release-notes"></a>[<span data-ttu-id="69b8c-104">Notas sobre a versão atuais</span><span class="sxs-lookup"><span data-stu-id="69b8c-104">Current release notes</span></span>](#tab/azure-cli)

## <a name="october-27-2020"></a><span data-ttu-id="69b8c-105">27 de outubro de 2020</span><span class="sxs-lookup"><span data-stu-id="69b8c-105">October 27, 2020</span></span>

<span data-ttu-id="69b8c-106">Versão 2.14.0</span><span class="sxs-lookup"><span data-stu-id="69b8c-106">Version 2.14.0</span></span>

### <a name="aks"></a><span data-ttu-id="69b8c-107">AKS</span><span class="sxs-lookup"><span data-stu-id="69b8c-107">AKS</span></span>

* <span data-ttu-id="69b8c-108">Adição de suporte a PPG</span><span class="sxs-lookup"><span data-stu-id="69b8c-108">Add PPG support</span></span>
* <span data-ttu-id="69b8c-109">Atualização do tempo limite máximo Standard Load Balancer para 100 minutos</span><span class="sxs-lookup"><span data-stu-id="69b8c-109">Update max standard load balancer timeout to 100 minutes</span></span>

### <a name="apim"></a><span data-ttu-id="69b8c-110">APIM</span><span class="sxs-lookup"><span data-stu-id="69b8c-110">APIM</span></span>

* <span data-ttu-id="69b8c-111">Correção de um problema com a criação da instância da camada de consumo</span><span class="sxs-lookup"><span data-stu-id="69b8c-111">Fix issue with creating consumption tier instance</span></span>

### <a name="app-config"></a><span data-ttu-id="69b8c-112">Configuração do Aplicativo</span><span class="sxs-lookup"><span data-stu-id="69b8c-112">App Config</span></span>

* <span data-ttu-id="69b8c-113">Correção da consulta de pares chave-valor por rótulos separados por vírgula</span><span class="sxs-lookup"><span data-stu-id="69b8c-113">Fix querying key-values by comma separated labels</span></span>

### <a name="app-service"></a><span data-ttu-id="69b8c-114">Serviço de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="69b8c-114">App Service</span></span>

* <span data-ttu-id="69b8c-115">Correção de bug: falha no comando az webapp up quando o usuário não tem permissões de gravação no diretório pai do projeto</span><span class="sxs-lookup"><span data-stu-id="69b8c-115">Bugfix: az webapp up fails when user doesn't have write permissions to project's parent directory</span></span>
* <span data-ttu-id="69b8c-116">Correção nº 13777: Correção para remover caracteres de escape do XML</span><span class="sxs-lookup"><span data-stu-id="69b8c-116">Fix #13777: Fix to remove escape chars from XML</span></span>
* <span data-ttu-id="69b8c-117">Correção nº 15441: falha no comando az webapp create-remote-connection com AttributeError: o objeto 'Thread' não tem nenhum atributo 'isAlive'</span><span class="sxs-lookup"><span data-stu-id="69b8c-117">Fix #15441: az webapp create-remote-connection fails with AttributeError: 'Thread' object has no attribute 'isAlive'</span></span>
* <span data-ttu-id="69b8c-118">[ALTERAÇÃO DA FALHA] az webapp up: adição de parâmetros opcionais (sistema operacional e runtime) e atualização de runtimes</span><span class="sxs-lookup"><span data-stu-id="69b8c-118">[BREAKING CHANGE] az webapp up: add optional params (os & runtime) and updated runtimes</span></span>

### <a name="arm"></a><span data-ttu-id="69b8c-119">ARM</span><span class="sxs-lookup"><span data-stu-id="69b8c-119">ARM</span></span>

* <span data-ttu-id="69b8c-120">Migração para GA de comandos What-If de implantação de modelo</span><span class="sxs-lookup"><span data-stu-id="69b8c-120">Make template deployment What-If commands GA</span></span>
* <span data-ttu-id="69b8c-121">[ALTERAÇÃO DA FALHA] Adição da confirmação do usuário ao comando az ts create</span><span class="sxs-lookup"><span data-stu-id="69b8c-121">[BREAKING CHANGE] Add user confirmation for az ts create</span></span>
* <span data-ttu-id="69b8c-122">Correção dos dados retornados na marcação de vários recursos</span><span class="sxs-lookup"><span data-stu-id="69b8c-122">Fix the returned data when tagging multiple resources</span></span>

### <a name="backup"></a><span data-ttu-id="69b8c-123">Backup</span><span class="sxs-lookup"><span data-stu-id="69b8c-123">Backup</span></span>

* <span data-ttu-id="69b8c-124">`az backup policy create`: adição de suporte para criação da política de backup de IaaSVM por meio da CLI</span><span class="sxs-lookup"><span data-stu-id="69b8c-124">`az backup policy create`: Add support for IaaSVM backup policy creation from CLI</span></span>
* <span data-ttu-id="69b8c-125">Aumento do limite de proteção da VM de 100 para 1.000</span><span class="sxs-lookup"><span data-stu-id="69b8c-125">Increasing VM protection limit from 100 to 1000</span></span>

### <a name="compute"></a><span data-ttu-id="69b8c-126">Computação</span><span class="sxs-lookup"><span data-stu-id="69b8c-126">Compute</span></span>

* <span data-ttu-id="69b8c-127">sig image-definition create: add --features</span><span class="sxs-lookup"><span data-stu-id="69b8c-127">sig image-definition create: add --features</span></span>
* <span data-ttu-id="69b8c-128">Nova versão de API de gallery_images 2020-09-30</span><span class="sxs-lookup"><span data-stu-id="69b8c-128">New API version of gallery_images 2020-09-30</span></span>
* <span data-ttu-id="69b8c-129">`az vm update / az sig image-version update`: suporte à atualização da versão de VM/imagem mesmo quando ela usa uma imagem entre locatários</span><span class="sxs-lookup"><span data-stu-id="69b8c-129">`az vm update / az sig image-version update`: Support update vm/image-version even it uses a cross tenant image</span></span>
* <span data-ttu-id="69b8c-130">Remoção da validação de SKUs de host de VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-130">Remove validation of vm host SKUs</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="69b8c-131">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="69b8c-131">Cosmos DB</span></span>

* <span data-ttu-id="69b8c-132">`az cosmosdb create/update`: aprimoramento da mensagem de erro da entrada incorreta de --locations</span><span class="sxs-lookup"><span data-stu-id="69b8c-132">`az cosmosdb create/update`: Improve error message from incorrect --locations input</span></span>
* <span data-ttu-id="69b8c-133">`az cosmosdb sql container create/update`: adição do parâmetro --analytical-storage-ttl</span><span class="sxs-lookup"><span data-stu-id="69b8c-133">`az cosmosdb sql container create/update`: Add --analytical-storage-ttl parameter</span></span>

### <a name="hdinsight"></a><span data-ttu-id="69b8c-134">HDInsight</span><span class="sxs-lookup"><span data-stu-id="69b8c-134">HDInsight</span></span>

* <span data-ttu-id="69b8c-135">[ALTERAÇÃO DA FALHA] az hdinsight create: remoção de dois parâmetros: --public-network-access-type e --outbound-public-network-access-type</span><span class="sxs-lookup"><span data-stu-id="69b8c-135">[BREAKING CHANGE] az hdinsight create: remove two parameters: --public-network-access-type and  --outbound-public-network-access-type</span></span>

### <a name="iot-central"></a><span data-ttu-id="69b8c-136">Central da IoT</span><span class="sxs-lookup"><span data-stu-id="69b8c-136">IoT Central</span></span>

* <span data-ttu-id="69b8c-137">Remoção do aviso de versão prévia, pois ela já está em GA</span><span class="sxs-lookup"><span data-stu-id="69b8c-137">Remove preview warning since it is already GAed</span></span>

### <a name="key-vault"></a><span data-ttu-id="69b8c-138">Key Vault</span><span class="sxs-lookup"><span data-stu-id="69b8c-138">Key Vault</span></span>

* <span data-ttu-id="69b8c-139">Invalidação de `--enable-soft-delete false` na criação ou na atualização de cofres</span><span class="sxs-lookup"><span data-stu-id="69b8c-139">Invalidate `--enable-soft-delete false` while creating or updating vaults</span></span>
* <span data-ttu-id="69b8c-140">Alteração para que `--bypass` e `--default-action` trabalhem em conjunto com parâmetros da ACL de rede na criação de cofres</span><span class="sxs-lookup"><span data-stu-id="69b8c-140">Make `--bypass` and `--default-action` work together with network acl parameters while creating vaults</span></span>

### <a name="misc"></a><span data-ttu-id="69b8c-141">Diversos.</span><span class="sxs-lookup"><span data-stu-id="69b8c-141">Misc.</span></span>

* <span data-ttu-id="69b8c-142">Adição de bash-completion a Dockerfile</span><span class="sxs-lookup"><span data-stu-id="69b8c-142">Add bash-completion to Dockerfile</span></span>

### <a name="rdbms"></a><span data-ttu-id="69b8c-143">RDBMS</span><span class="sxs-lookup"><span data-stu-id="69b8c-143">RDBMS</span></span>

* <span data-ttu-id="69b8c-144">Adição do comando list-SKUS, de transformadores de tabela e do contexto local para o Postgres, o MySQL e o MariaDB – Servidor Único</span><span class="sxs-lookup"><span data-stu-id="69b8c-144">Add List-SKUS Command, Table Transformers, Local Context for Postgres, MySQL, Mariadb Single Server</span></span>
* <span data-ttu-id="69b8c-145">[ALTERAÇÃO DA FALHA] Atualizações de nomes de parâmetros.</span><span class="sxs-lookup"><span data-stu-id="69b8c-145">[BREAKING CHANGE] Parameter name updates.</span></span> <span data-ttu-id="69b8c-146">Aprimoramentos no plano de gerenciamento para o MySQL e o PostgreSQL</span><span class="sxs-lookup"><span data-stu-id="69b8c-146">Improvements to Management Plane for MySQL and PostgreSQL</span></span>
* <span data-ttu-id="69b8c-147">`az postgres|mariadb|mysql server create`: atualização da experiência de criação para o Postgres, o MySQL e o MariaDB: novos campos na saída e introdução de novos valores para o parâmetro `--public` no comando create (tudo, <IP>, <IPRange>, 0.0.0.0)</span><span class="sxs-lookup"><span data-stu-id="69b8c-147">`az postgres|mariadb|mysql server create` : Update create experience for Postgres, MySQL and MariaDB - new fields in the output , Introduce new values for `--public` parameter in create command (all,<IP>,<IPRange>,0.0.0.0)</span></span>

### <a name="signalr"></a><span data-ttu-id="69b8c-148">SignalR</span><span class="sxs-lookup"><span data-stu-id="69b8c-148">SignalR</span></span>

* <span data-ttu-id="69b8c-149">`az signalr create`: adição da nova opção `--enable-messaging-logs` para controlar o serviço na geração de logs de mensagens ou não</span><span class="sxs-lookup"><span data-stu-id="69b8c-149">`az signalr create`: Add new option `--enable-messaging-logs` for controling service generate messaging logs or not</span></span>
* <span data-ttu-id="69b8c-150">`az signalr update`: adição da nova opção `--enable-messaging-logs` para controlar o serviço na geração de logs de mensagens ou não</span><span class="sxs-lookup"><span data-stu-id="69b8c-150">`az signalr update`: Add new option `--enable-messaging-logs` for controling service generate messaging logs or not</span></span>

### <a name="sql"></a><span data-ttu-id="69b8c-151">SQL</span><span class="sxs-lookup"><span data-stu-id="69b8c-151">SQL</span></span>

* <span data-ttu-id="69b8c-152">[ALTERAÇÃO DA FALHA] Correção da resposta do nome de parâmetro de redundância do armazenamento de backup e do valor para a MI</span><span class="sxs-lookup"><span data-stu-id="69b8c-152">[BREAKING CHANGE] Fix response for backup storage redundancy param name and value for MI</span></span>
* <span data-ttu-id="69b8c-153">`az sql db audit-policy show`: extensão para mostrar a política de auditoria do banco de dados, incluindo os dados de LA e EH</span><span class="sxs-lookup"><span data-stu-id="69b8c-153">`az sql db audit-policy show`: extend to show database's audit policy including LA and EH data</span></span>
* <span data-ttu-id="69b8c-154">`az sql db audit-policy update`: extensão para permitir a atualização de LA e EH juntamente com a política de auditoria do banco de dados</span><span class="sxs-lookup"><span data-stu-id="69b8c-154">`az sql db audit-policy update`: extend to allow LA and EH update along with database's audit policy</span></span>
* <span data-ttu-id="69b8c-155">`az sql db audit-policy wait`: colocação da CLI em um estado de espera até que uma condição da política de auditoria do banco de dados seja atendida.</span><span class="sxs-lookup"><span data-stu-id="69b8c-155">`az sql db audit-policy wait`: place the CLI in a waiting state until a condition of the database's audit policy is met.</span></span>
* <span data-ttu-id="69b8c-156">`az sql server audit-policy show`: extensão para mostrar a política de auditoria do servidor, incluindo os dados de LA e EH</span><span class="sxs-lookup"><span data-stu-id="69b8c-156">`az sql server audit-policy show`: extend to show servers's audit policy including LA and EH data</span></span>
* <span data-ttu-id="69b8c-157">`az sql server audit-policy update`: extensão para permitir a atualização de LA e EH juntamente com a política de auditoria do servidor</span><span class="sxs-lookup"><span data-stu-id="69b8c-157">`az sql server audit-policy update`: extend to allow LA and EH update along with server's audit policy</span></span>
* <span data-ttu-id="69b8c-158">`az sql server audit-policy wait`: colocação da CLI em um estado de espera até que uma condição da política de auditoria do servidor seja atendida.</span><span class="sxs-lookup"><span data-stu-id="69b8c-158">`az sql server audit-policy wait`: place the CLI in a waiting state until a condition of the server's audit policy is met.</span></span>
* <span data-ttu-id="69b8c-159">Adição de suporte somente ao AAD para Servidores e Instâncias Gerenciadas de SQL</span><span class="sxs-lookup"><span data-stu-id="69b8c-159">Add AAD-only Support for SQL Managed Instances and Servers</span></span>
* <span data-ttu-id="69b8c-160">`az sql db replica create`: adição do argumento --partner-database</span><span class="sxs-lookup"><span data-stu-id="69b8c-160">`az sql db replica create`: Add --partner-database argument</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-161">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-161">Storage</span></span>

* <span data-ttu-id="69b8c-162">Correção nº 15111: falha no comando `az storage logging update` sem argumento opcional</span><span class="sxs-lookup"><span data-stu-id="69b8c-162">Fix #15111: `az storage logging update` fails without optional argument</span></span>
* <span data-ttu-id="69b8c-163">Correção de bug no uso do comando set-tier com o logon da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="69b8c-163">Fix bug when using set-tier command with service principal login</span></span>
* <span data-ttu-id="69b8c-164">Atualização da versão do data lake do arquivo para 2020-02-10</span><span class="sxs-lookup"><span data-stu-id="69b8c-164">Upgrade version for file datalake to 2020-02-10</span></span>
* <span data-ttu-id="69b8c-165">`az storage queue list`: suporte a Track2</span><span class="sxs-lookup"><span data-stu-id="69b8c-165">`az storage queue list`: Track2 supported</span></span>
* <span data-ttu-id="69b8c-166">`az storage fs access`: suporte ao gerenciamento de ACLs de maneira recursiva</span><span class="sxs-lookup"><span data-stu-id="69b8c-166">`az storage fs access`: Support managing ACLs recursively</span></span>

### <a name="synapse"></a><span data-ttu-id="69b8c-167">Synapse</span><span class="sxs-lookup"><span data-stu-id="69b8c-167">Synapse</span></span>

* <span data-ttu-id="69b8c-168">adição de cmdlets relacionados a pipeline, serviço vinculado, gatilho, notebook, fluxo de dados e conjunto de dados</span><span class="sxs-lookup"><span data-stu-id="69b8c-168">Add pipeline, linked service, trigger, notebook, data flow and dataset related cmdlets</span></span>

## <a name="october-13-2020"></a><span data-ttu-id="69b8c-169">13 de outubro de 2020</span><span class="sxs-lookup"><span data-stu-id="69b8c-169">October 13, 2020</span></span>

<span data-ttu-id="69b8c-170">Versão 2.13.0</span><span class="sxs-lookup"><span data-stu-id="69b8c-170">Version 2.13.0</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-171">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-171">ACR</span></span>

* <span data-ttu-id="69b8c-172">`az acr helm`: atualizar a URL de substituição</span><span class="sxs-lookup"><span data-stu-id="69b8c-172">`az acr helm`: Update deprecation url</span></span>
* <span data-ttu-id="69b8c-173">Adicionar alterações de logtemplate e systemtask para Tarefas do ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-173">Add logtemplate and systemtask changes for ACR Tasks</span></span>

### <a name="aks"></a><span data-ttu-id="69b8c-174">AKS</span><span class="sxs-lookup"><span data-stu-id="69b8c-174">AKS</span></span>

* <span data-ttu-id="69b8c-175">Dar suporte ao nó virtual com o comando aks create: `az aks create --enable-addons virtual-node`</span><span class="sxs-lookup"><span data-stu-id="69b8c-175">Support virtual-node with aks create: `az aks create --enable-addons virtual-node`</span></span>
* <span data-ttu-id="69b8c-176">Adicionar a única opção de imagem de nó para a CLI</span><span class="sxs-lookup"><span data-stu-id="69b8c-176">Add node image only option for CLI</span></span>
* <span data-ttu-id="69b8c-177">Esperar que o complemento kube-dashboard seja desabilitado por padrão</span><span class="sxs-lookup"><span data-stu-id="69b8c-177">Expect kube-dashboard addon be disabled by default</span></span>
* <span data-ttu-id="69b8c-178">`az aks create/update`: adicionar suporte ao LicenseType para o Windows</span><span class="sxs-lookup"><span data-stu-id="69b8c-178">`az aks create/update`: Add LicenseType support for Windows</span></span>
* <span data-ttu-id="69b8c-179">Dar suporte para adicionar pools de nós spot</span><span class="sxs-lookup"><span data-stu-id="69b8c-179">Support add Spot node pool</span></span>
* <span data-ttu-id="69b8c-180">Respeitar os nomes de complementos definidos na CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="69b8c-180">Honor addon names defined in Azure CLI</span></span>

### <a name="ams"></a><span data-ttu-id="69b8c-181">AMS</span><span class="sxs-lookup"><span data-stu-id="69b8c-181">AMS</span></span>

* <span data-ttu-id="69b8c-182">Correção nº 14687: o grupo de recursos e o nome da conta misturados no comando "az ams streaming-endpoint show"</span><span class="sxs-lookup"><span data-stu-id="69b8c-182">Fix #14687: Mixed resource group and account name in command "az ams streaming-endpoint show"</span></span>

### <a name="app-config"></a><span data-ttu-id="69b8c-183">Configuração do Aplicativo</span><span class="sxs-lookup"><span data-stu-id="69b8c-183">App Config</span></span>

* <span data-ttu-id="69b8c-184">Corrigir o bug de teste</span><span class="sxs-lookup"><span data-stu-id="69b8c-184">Fix test bug</span></span>
* <span data-ttu-id="69b8c-185">Dar suporte à autenticação do AAD para operações de dados</span><span class="sxs-lookup"><span data-stu-id="69b8c-185">Support AAD auth for data operations</span></span>

### <a name="app-service"></a><span data-ttu-id="69b8c-186">Serviço de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="69b8c-186">App Service</span></span>

* <span data-ttu-id="69b8c-187">`az functionapp deployment source config-zip`: correção de um problema em que o config-zip poderia gerar uma exceção em caso de sucesso no consumo em Linux</span><span class="sxs-lookup"><span data-stu-id="69b8c-187">`az functionapp deployment source config-zip`: Fixed an issue where config-zip could throw an exception on success on linux consumption</span></span>
* <span data-ttu-id="69b8c-188">Bugfix: mensagens de erro aprimoradas para comandos webapp</span><span class="sxs-lookup"><span data-stu-id="69b8c-188">Bugfix: Better error messages for webapp commands</span></span>
* <span data-ttu-id="69b8c-189">`az appservice domain create, show-terms`: adicionar a capacidade de criar um domínio do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="69b8c-189">`az appservice domain create, show-terms`: Add ability to create app service domain</span></span>
* <span data-ttu-id="69b8c-190">`az functionapp create`: o sinalizador de visualização do Java 11 foi removido durante a criação de um aplicativo de funções</span><span class="sxs-lookup"><span data-stu-id="69b8c-190">`az functionapp create`: Removed the preview flag from Java 11 when creating a new function app</span></span>
* <span data-ttu-id="69b8c-191">[ALTERAÇÃO DA FALHA] az webapp create e az webapp up – Atualizar runtimes de webapp disponíveis</span><span class="sxs-lookup"><span data-stu-id="69b8c-191">[BREAKING CHANGE] az webapp create, az webapp up - Update available webapp runtimes</span></span>

### <a name="arm"></a><span data-ttu-id="69b8c-192">ARM</span><span class="sxs-lookup"><span data-stu-id="69b8c-192">ARM</span></span>

* <span data-ttu-id="69b8c-193">`az ts`: adicionar novos comandos para especificações de modelo</span><span class="sxs-lookup"><span data-stu-id="69b8c-193">`az ts`: Add new commands for template specs</span></span>
* <span data-ttu-id="69b8c-194">`az deployment`: adicionar suporte para --template-spec -s</span><span class="sxs-lookup"><span data-stu-id="69b8c-194">`az deployment` : Add support for --template-spec -s</span></span>

### <a name="compute"></a><span data-ttu-id="69b8c-195">Computação</span><span class="sxs-lookup"><span data-stu-id="69b8c-195">Compute</span></span>

* <span data-ttu-id="69b8c-196">Corrigir a limitação de contagem FD de criação de grupos de hosts</span><span class="sxs-lookup"><span data-stu-id="69b8c-196">Fix host group creation FD count limitation</span></span>
* <span data-ttu-id="69b8c-197">Adicionar um novo comando para dar suporte à atualização de extensões para VMSS</span><span class="sxs-lookup"><span data-stu-id="69b8c-197">Add new command to support upgrading extensions for VMSS</span></span>
* <span data-ttu-id="69b8c-198">Não há problemas na correção da referência da imagem</span><span class="sxs-lookup"><span data-stu-id="69b8c-198">Fix the image reference is missing issue</span></span>

### <a name="hdinsight"></a><span data-ttu-id="69b8c-199">HDInsight</span><span class="sxs-lookup"><span data-stu-id="69b8c-199">HDInsight</span></span>

* <span data-ttu-id="69b8c-200">`az hdinsight create`: adicionar informações preteridas para os argumentos --public-networrk-access-type e --outbound-public-network-access-type</span><span class="sxs-lookup"><span data-stu-id="69b8c-200">`az hdinsight create`: add deprecate information for argument --public-networrk-access-type and --outbound-public-network-access-type</span></span>
* <span data-ttu-id="69b8c-201">`az hdinsight create`: adicionar informações preteridas para os argumentos `--public-networrk-access-type` e `--outbound-public-network-access-type`</span><span class="sxs-lookup"><span data-stu-id="69b8c-201">`az hdinsight create`: add deprecate information for argument `--public-networrk-access-type` and `--outbound-public-network-access-type`</span></span>
* <span data-ttu-id="69b8c-202">`az hdinsight create`: adicionar o parâmetro `--idbroker` para dar suporte ao cliente a fim de criar um cluster ESP com o Agente de IDs do HDInsight</span><span class="sxs-lookup"><span data-stu-id="69b8c-202">`az hdinsight create`:  add parameter `--idbroker` to support customer to create ESP cluster with HDInsight Id Broker</span></span>

### <a name="iot-central"></a><span data-ttu-id="69b8c-203">Central da IoT</span><span class="sxs-lookup"><span data-stu-id="69b8c-203">IoT Central</span></span>

* <span data-ttu-id="69b8c-204">Remover o módulo de comando 'az iotcentral' preterido</span><span class="sxs-lookup"><span data-stu-id="69b8c-204">Remove deprecated 'az iotcentral' command module</span></span>

### <a name="key-vault"></a><span data-ttu-id="69b8c-205">Key Vault</span><span class="sxs-lookup"><span data-stu-id="69b8c-205">Key Vault</span></span>

* <span data-ttu-id="69b8c-206">Dar suporte à `--hsm-name` para `az keyvault key encrypt/decrypt`</span><span class="sxs-lookup"><span data-stu-id="69b8c-206">Support `--hsm-name` for `az keyvault key encrypt/decrypt`</span></span>

### <a name="lab"></a><span data-ttu-id="69b8c-207">Laboratório</span><span class="sxs-lookup"><span data-stu-id="69b8c-207">Lab</span></span>

* <span data-ttu-id="69b8c-208">Correção nº 14127: `__init__()` precisa de um argumento posicional, porém dois foram fornecidos</span><span class="sxs-lookup"><span data-stu-id="69b8c-208">Fix #14127: `__init__()` takes 1 positional argument but 2 were given</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-209">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-209">Network</span></span>

* <span data-ttu-id="69b8c-210">`az network application-gateway ssl-cert show`: adicionar um exemplo para demonstrar o formato do certificado e buscar informações</span><span class="sxs-lookup"><span data-stu-id="69b8c-210">`az network application-gateway ssl-cert show`: Add example to demonstrate certificate format and fetch information</span></span>
* <span data-ttu-id="69b8c-211">`az network application-gateway rule`: dar suporte a --priority option</span><span class="sxs-lookup"><span data-stu-id="69b8c-211">`az network application-gateway rule`: Support --priority option</span></span>
* <span data-ttu-id="69b8c-212">`az network application-gateway create`: corrigir um bug que não pode ser criado sem um IP especificado</span><span class="sxs-lookup"><span data-stu-id="69b8c-212">`az network application-gateway create`: Fix bug that cannot create without public IP sepcified</span></span>
* <span data-ttu-id="69b8c-213">`az network application-gateway waf-policy managed-rule rule-set add`: expor o erro do servidor ao usuário para fornecer uma mensagem de dica mais intuitiva.</span><span class="sxs-lookup"><span data-stu-id="69b8c-213">`az network application-gateway waf-policy managed-rule rule-set add`: Expose server error to user to give more intuitive hint message.</span></span>
* <span data-ttu-id="69b8c-214">`az network application-gateway waf-policy managed-rule rule-set update`: dar suporte para alterar a versão do tipo de conjunto de regras.</span><span class="sxs-lookup"><span data-stu-id="69b8c-214">`az network application-gateway waf-policy managed-rule rule-set update`: Support to change rule set type version.</span></span>

### <a name="rdbms"></a><span data-ttu-id="69b8c-215">RDBMS</span><span class="sxs-lookup"><span data-stu-id="69b8c-215">RDBMS</span></span>

* <span data-ttu-id="69b8c-216">Bugfix: az postgres flexible-server create. Remover a versão de API codificada do cliente de rede.</span><span class="sxs-lookup"><span data-stu-id="69b8c-216">Bugfix: az postgres flexible-server create Remove hardcoded API version from network client.</span></span>

### <a name="role"></a><span data-ttu-id="69b8c-217">Função</span><span class="sxs-lookup"><span data-stu-id="69b8c-217">Role</span></span>

* <span data-ttu-id="69b8c-218">Correção nº 15278: `az role assignment list/delete`: proibir argumentos de cadeias de caracteres vazias</span><span class="sxs-lookup"><span data-stu-id="69b8c-218">Fix #15278: `az role assignment list/delete`: Forbid empty string arguments</span></span>

### <a name="sql"></a><span data-ttu-id="69b8c-219">SQL</span><span class="sxs-lookup"><span data-stu-id="69b8c-219">SQL</span></span>

* <span data-ttu-id="69b8c-220">`az sql midb log-replay`: dar suporte para serviços de reprodução de log em um banco de dados gerenciado</span><span class="sxs-lookup"><span data-stu-id="69b8c-220">`az sql midb log-replay`: Support for log replay service on managed database</span></span>
* <span data-ttu-id="69b8c-221">Ignorar a formatação de maiúsculas/minúsculas dos caracteres para o valor de parâmetro de redundância de armazenamento de backup para uma instância gerenciada</span><span class="sxs-lookup"><span data-stu-id="69b8c-221">Ignore character casing for backup storage redundancy param value for managed instance</span></span>
* <span data-ttu-id="69b8c-222">[ALTERAÇÃO DA FALHA] az sql db create: adicionar o parâmetro --backup-storage-redundancy. Adicionar um aviso para o bsr/bsr == Geo não especificado.</span><span class="sxs-lookup"><span data-stu-id="69b8c-222">[BREAKING CHANGE] az sql db create: Add --backup-storage-redundancy parameter; add warning for unspecified bsr/bsr == Geo.</span></span>

### <a name="sql-vm"></a><span data-ttu-id="69b8c-223">SQL VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-223">SQL VM</span></span>

* <span data-ttu-id="69b8c-224">`az sql vm show`: adicionar opções de configuração ao sinalizador --expand</span><span class="sxs-lookup"><span data-stu-id="69b8c-224">`az sql vm show`: Add configuration options to --expand flag</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-225">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-225">Storage</span></span>

* <span data-ttu-id="69b8c-226">[ALTERAÇÃO DA FALHA] `az storage blob copy start`: corrigir o problema de formato para `--destination-if-modified-since` e `--destination-if-unmodified-since`</span><span class="sxs-lookup"><span data-stu-id="69b8c-226">[BREAKING CHANGE] `az storage blob copy start`: Fix format issue for `--destination-if-modified-since` and `--destination-if-unmodified-since`</span></span>
* <span data-ttu-id="69b8c-227">[ALTERAÇÃO DA FALHA] `az storage blob incremental-copy start`: corrigir o problema de formato para `--destination-if-modified-since` e `--destination-if-unmodified-since`</span><span class="sxs-lookup"><span data-stu-id="69b8c-227">[BREAKING CHANGE] `az storage blob incremental-copy start`: Fix format issue for `--destination-if-modified-since` and `--destination-if-unmodified-since`</span></span>
* <span data-ttu-id="69b8c-228">`az storage fs`: corrigir um problema de cadeia de conexão</span><span class="sxs-lookup"><span data-stu-id="69b8c-228">`az storage fs`: Fix connection string issue</span></span>
* <span data-ttu-id="69b8c-229">`az storage share-rm`: camada de acesso da versão de GA</span><span class="sxs-lookup"><span data-stu-id="69b8c-229">`az storage share-rm`: GA release access tier</span></span>
* <span data-ttu-id="69b8c-230">`az storage container-rm`: adicionar um novo grupo de comandos com o objetivo de usar o provedor de recursos Microsoft.Storage para operações de gerenciamento de contêineres.</span><span class="sxs-lookup"><span data-stu-id="69b8c-230">`az storage container-rm`: Add a new command group to use the Microsoft.Storage resource provider for container management operations.</span></span>

## <a name="september-29-2020"></a><span data-ttu-id="69b8c-231">29 de setembro de 2020</span><span class="sxs-lookup"><span data-stu-id="69b8c-231">September 29, 2020</span></span>

<span data-ttu-id="69b8c-232">Versão 2.12.1</span><span class="sxs-lookup"><span data-stu-id="69b8c-232">Version 2.12.1</span></span>

### <a name="rdbms"></a><span data-ttu-id="69b8c-233">RDBMS</span><span class="sxs-lookup"><span data-stu-id="69b8c-233">RDBMS</span></span>

* <span data-ttu-id="69b8c-234">Hotfix: `az postgres flexible-server create`: Atualizar o VnetName para excluir o nome do servidor e atualizar a região padrão para MySQL</span><span class="sxs-lookup"><span data-stu-id="69b8c-234">Hotfix: `az postgres flexible-server create` : Update VnetName to exclude servername and update default region for MySQL</span></span>

## <a name="september-22-2020"></a><span data-ttu-id="69b8c-235">22 de setembro de 2020</span><span class="sxs-lookup"><span data-stu-id="69b8c-235">September 22, 2020</span></span>

<span data-ttu-id="69b8c-236">Versão 2.12.0</span><span class="sxs-lookup"><span data-stu-id="69b8c-236">Version 2.12.0</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-237">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-237">ACR</span></span>

* <span data-ttu-id="69b8c-238">Correção nº 14811: adicionar suporte para substituição dockerignore</span><span class="sxs-lookup"><span data-stu-id="69b8c-238">Fix #14811 Add support for dockerignore override</span></span>

### <a name="aks"></a><span data-ttu-id="69b8c-239">AKS</span><span class="sxs-lookup"><span data-stu-id="69b8c-239">AKS</span></span>

* <span data-ttu-id="69b8c-240">A CLI deve tolerar kubeconfig vazio</span><span class="sxs-lookup"><span data-stu-id="69b8c-240">CLI should tolerate empty kubeconfig</span></span>
* <span data-ttu-id="69b8c-241">CORREÇÃO nº 12871: az aks enable-addons: o exemplo de ajuda gerada automaticamente está errado para a opção virtual-node</span><span class="sxs-lookup"><span data-stu-id="69b8c-241">FIX #12871: az aks enable-addons: Autogenerated help example is wrong for vitual-node option</span></span>
* <span data-ttu-id="69b8c-242">Remover ações do conector do aci herdado</span><span class="sxs-lookup"><span data-stu-id="69b8c-242">Remove legacy aci connector actions</span></span>
* <span data-ttu-id="69b8c-243">Dar suporte ao complemento do Azure Policy em azure-cli</span><span class="sxs-lookup"><span data-stu-id="69b8c-243">Support azure policy addon in azure-cli</span></span>
* <span data-ttu-id="69b8c-244">Corrigir o problema de diferenciação de maiúsculas e minúsculas do complemento do painel do AKS</span><span class="sxs-lookup"><span data-stu-id="69b8c-244">Fix case sensitive issue for AKS dashboard addon</span></span>
* <span data-ttu-id="69b8c-245">Atualizar mgmt-containerservice para a versão 9.4.0 e habilitar a API 09-01</span><span class="sxs-lookup"><span data-stu-id="69b8c-245">Update mgmt-containerservice to 9.4.0 and enable 09-01 API</span></span>

### <a name="apim"></a><span data-ttu-id="69b8c-246">APIM</span><span class="sxs-lookup"><span data-stu-id="69b8c-246">APIM</span></span>

* <span data-ttu-id="69b8c-247">Dar suporte aos comandos de entidade product/productapi/namedValue e a versão do SDK bump &&</span><span class="sxs-lookup"><span data-stu-id="69b8c-247">Support product / productapi / namedValue entity commands && bump sdk version</span></span>

### <a name="app-config"></a><span data-ttu-id="69b8c-248">Configuração do Aplicativo</span><span class="sxs-lookup"><span data-stu-id="69b8c-248">App Config</span></span>

* <span data-ttu-id="69b8c-249">Dar suporte para habilitar/desabilitar PublicNetworkAccess para armazenamentos existentes</span><span class="sxs-lookup"><span data-stu-id="69b8c-249">Support enabling/disabling PublicNetworkAccess for existing stores</span></span>

### <a name="app-service"></a><span data-ttu-id="69b8c-250">Serviço de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="69b8c-250">App Service</span></span>

* <span data-ttu-id="69b8c-251">Adicionar suporte para o tipo de preço Premium V3</span><span class="sxs-lookup"><span data-stu-id="69b8c-251">Add support for Premium V3 pricing tier</span></span>
* <span data-ttu-id="69b8c-252">Correção nº12653: az webapp log config --application-logging false não o desativa</span><span class="sxs-lookup"><span data-stu-id="69b8c-252">Fix #12653: az webapp log config --application-logging false doesn't turn it off</span></span>
* <span data-ttu-id="69b8c-253">Correção nº 14684: a remoção de access-restriction por endereço IP não funcionava; nº 13837-az webapp create – Exemplo para diferentes RSgroups para Plan e WebApp</span><span class="sxs-lookup"><span data-stu-id="69b8c-253">Fix #14684: access-restriction remove by ip address does not work; #13837-az webapp create - Example for different RSgroups for Plan and WebApp</span></span>
* <span data-ttu-id="69b8c-254">functionapp: Adicionar suporte para manipuladores personalizados.</span><span class="sxs-lookup"><span data-stu-id="69b8c-254">functionapp: Add support for custom handlers.</span></span> <span data-ttu-id="69b8c-255">PowerShell 6.2 preterido.</span><span class="sxs-lookup"><span data-stu-id="69b8c-255">Deprecated Powershell 6.2.</span></span>
* <span data-ttu-id="69b8c-256">functionapp: Correção do problema em que a configuração do aplicativo estava sendo definida incorretamente para imagens personalizadas do Linux</span><span class="sxs-lookup"><span data-stu-id="69b8c-256">functionapp: Fix issue where app setting was being incorrectly set for linux custom images</span></span>

### <a name="arm"></a><span data-ttu-id="69b8c-257">ARM</span><span class="sxs-lookup"><span data-stu-id="69b8c-257">ARM</span></span>

* <span data-ttu-id="69b8c-258">`az deployment group/sub/mg/tenant what-if`: Mostrar alterações de recurso "Ignorar" por último</span><span class="sxs-lookup"><span data-stu-id="69b8c-258">`az deployment group/sub/mg/tenant what-if`: Show "Ignore" resource changes last</span></span>

### <a name="compute"></a><span data-ttu-id="69b8c-259">Computação</span><span class="sxs-lookup"><span data-stu-id="69b8c-259">Compute</span></span>

* <span data-ttu-id="69b8c-260">Adicionar novo license_type na criação/atualização de VM: RHEL_BYOS, SLES_BYOS</span><span class="sxs-lookup"><span data-stu-id="69b8c-260">Add new license_type in vm create/update: RHEL_BYOS, SLES_BYOS</span></span>
* <span data-ttu-id="69b8c-261">Atualizar a API do disco para a versão 2020-06-30</span><span class="sxs-lookup"><span data-stu-id="69b8c-261">Upgrade disk API version to 2020-06-30</span></span>
* <span data-ttu-id="69b8c-262">criação do disco: add --logical-sector-size, --tier</span><span class="sxs-lookup"><span data-stu-id="69b8c-262">disk create: add --logical-sector-size, --tier</span></span>
* <span data-ttu-id="69b8c-263">atualização do disco: Suporte a --disk-iops-read-only, --disk-mbps-read-only, --max-shares</span><span class="sxs-lookup"><span data-stu-id="69b8c-263">disk update: Support --disk-iops-read-only, --disk-mbps-read-only, --max-shares</span></span>
* <span data-ttu-id="69b8c-264">Novo comando disk-encryption-set list-associated-resources</span><span class="sxs-lookup"><span data-stu-id="69b8c-264">New command disk-encryption-set list-associated-resources</span></span>
* <span data-ttu-id="69b8c-265">Habilitação de vm boot-diagnostics: --storage se torna opcional</span><span class="sxs-lookup"><span data-stu-id="69b8c-265">vm boot-diagnostics enable: --storage becomes optional</span></span>
* <span data-ttu-id="69b8c-266">Novo comando: vm boot-diagnostics get-boot-log-uris</span><span class="sxs-lookup"><span data-stu-id="69b8c-266">New command: vm boot-diagnostics get-boot-log-uris</span></span>
* <span data-ttu-id="69b8c-267">vm boot-diagnostics get-boot-log: suporte ao armazenamento gerenciado</span><span class="sxs-lookup"><span data-stu-id="69b8c-267">vm boot-diagnostics get-boot-log: support managed storage</span></span>

### <a name="config"></a><span data-ttu-id="69b8c-268">Config</span><span class="sxs-lookup"><span data-stu-id="69b8c-268">Config</span></span>

* <span data-ttu-id="69b8c-269">Renomear local-context para configurar param-persist</span><span class="sxs-lookup"><span data-stu-id="69b8c-269">Rename local-context to config param-persist</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="69b8c-270">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="69b8c-270">Cosmos DB</span></span>

* <span data-ttu-id="69b8c-271">Dar suporte a APIs de Migração para o recurso de taxa de transferência para o recurso de dimensionamento automático no CosmosDB</span><span class="sxs-lookup"><span data-stu-id="69b8c-271">Support for Migration APIs for Throughput resource for Autoscale feature in CosmosDB</span></span>

### <a name="eventhub"></a><span data-ttu-id="69b8c-272">Eventhub</span><span class="sxs-lookup"><span data-stu-id="69b8c-272">Eventhub</span></span>

<span data-ttu-id="69b8c-273">Adição de comandos de cluster e do parâmetro trusted_service_access_enabled para Networkruleset</span><span class="sxs-lookup"><span data-stu-id="69b8c-273">Added Cluster commands and trusted_service_access_enabled parameter for Networkruleset</span></span>

### <a name="extension"></a><span data-ttu-id="69b8c-274">Extensão</span><span class="sxs-lookup"><span data-stu-id="69b8c-274">Extension</span></span>

* <span data-ttu-id="69b8c-275">`az extension add`: adicionar a opção `--upgrade` para atualizar a extensão, se ela já estiver instalada</span><span class="sxs-lookup"><span data-stu-id="69b8c-275">`az extension add`: Add `--upgrade` option to update the extension if already installed</span></span>
* <span data-ttu-id="69b8c-276">Ativar a instalação dinâmica por padrão</span><span class="sxs-lookup"><span data-stu-id="69b8c-276">Turn on dynamic install by default</span></span>

### <a name="iot"></a><span data-ttu-id="69b8c-277">IoT</span><span class="sxs-lookup"><span data-stu-id="69b8c-277">IoT</span></span>

* <span data-ttu-id="69b8c-278">Versão mínima do TLS habilitada na criação do Hub IoT</span><span class="sxs-lookup"><span data-stu-id="69b8c-278">Enabled minimum TLS version on IoT Hub Create</span></span>

### <a name="iot-central"></a><span data-ttu-id="69b8c-279">IoT Central</span><span class="sxs-lookup"><span data-stu-id="69b8c-279">IoT Central</span></span>

* <span data-ttu-id="69b8c-280">A operação de exclusão de aplicativo agora é uma operação de execução prolongada</span><span class="sxs-lookup"><span data-stu-id="69b8c-280">App delete operation is now long running operation</span></span>

### <a name="iot-hub"></a><span data-ttu-id="69b8c-281">Hub IoT</span><span class="sxs-lookup"><span data-stu-id="69b8c-281">Iot Hub</span></span>

* <span data-ttu-id="69b8c-282">Comando 'show-connection-string' preterido</span><span class="sxs-lookup"><span data-stu-id="69b8c-282">Deprecated 'show-connection-string' command</span></span>

### <a name="key-vault"></a><span data-ttu-id="69b8c-283">Key Vault</span><span class="sxs-lookup"><span data-stu-id="69b8c-283">Key Vault</span></span>

* <span data-ttu-id="69b8c-284">Versão prévia pública do HSM gerenciado</span><span class="sxs-lookup"><span data-stu-id="69b8c-284">Managed HSM public preview</span></span>
* <span data-ttu-id="69b8c-285">Corrigir o problema em que `--maxresults` não entrou em vigor durante a listagem de recursos ou versões de recursos</span><span class="sxs-lookup"><span data-stu-id="69b8c-285">Fix the issue that `--maxresults` does not take effect while listing resources or resource versions</span></span>

### <a name="kusto"></a><span data-ttu-id="69b8c-286">Kusto</span><span class="sxs-lookup"><span data-stu-id="69b8c-286">Kusto</span></span>

* <span data-ttu-id="69b8c-287">Adicionar mensagem de substituição</span><span class="sxs-lookup"><span data-stu-id="69b8c-287">Add deprecating message</span></span>

### <a name="monitor"></a><span data-ttu-id="69b8c-288">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="69b8c-288">Monitor</span></span>

* <span data-ttu-id="69b8c-289">`az monitor log-analytics workspace linked-storage`: expor a mensagem de erro detalhada aos clientes</span><span class="sxs-lookup"><span data-stu-id="69b8c-289">`az monitor log-analytics workspace linked-storage`: expose detailed error message to customers</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-290">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-290">Network</span></span>

* <span data-ttu-id="69b8c-291">`az network vnet subnet`: dar suporte a --disable-private-endpoint-network-policies e --disable-private-link-service-network-policies</span><span class="sxs-lookup"><span data-stu-id="69b8c-291">`az network vnet subnet`: Support --disable-private-endpoint-network-policies and --disable-private-link-service-network-policies</span></span>
* <span data-ttu-id="69b8c-292">Corrigir o bug durante a atualização do log de fluxos quando a subpropriedade network_watcher_flow_analytics_configuration for None</span><span class="sxs-lookup"><span data-stu-id="69b8c-292">Fix bug while updateing flow-log when its subproperty network_watcher_flow_analytics_configuration is None</span></span>
* <span data-ttu-id="69b8c-293">Elevação da API para a versão 2020-06-01</span><span class="sxs-lookup"><span data-stu-id="69b8c-293">API version bump to 2020-06-01</span></span>
* <span data-ttu-id="69b8c-294">Dar suporte --tcp-port-behavior durante a definição da configuração do TCP de um Monitor da Conexão V2</span><span class="sxs-lookup"><span data-stu-id="69b8c-294">Support --tcp-port-behavior while configuring a TCP configuration of a Connection Monitor V2</span></span>
* <span data-ttu-id="69b8c-295">Dar suporte a mais tipos e ao nível de cobertura durante a criação do ponto de extremidade do Monitor da Conexão v2</span><span class="sxs-lookup"><span data-stu-id="69b8c-295">Support more types and coverage level while creating Endpoint of Connection Monitor V2</span></span>
* <span data-ttu-id="69b8c-296">Dar suporte a --host-subnet para criar o VirtualHub abaixo como VirtualRouter</span><span class="sxs-lookup"><span data-stu-id="69b8c-296">Support --host-subnet to create VirtualHub underneath as VirtualRouter</span></span>

### <a name="rdbms"></a><span data-ttu-id="69b8c-297">RDBMS</span><span class="sxs-lookup"><span data-stu-id="69b8c-297">RDBMS</span></span>

* <span data-ttu-id="69b8c-298">Atualizações do Plano de Gerenciamento para PostgreSQL e MySQL</span><span class="sxs-lookup"><span data-stu-id="69b8c-298">Management Plane updates for PostgreSQL and MySQL</span></span>

### <a name="role"></a><span data-ttu-id="69b8c-299">Função</span><span class="sxs-lookup"><span data-stu-id="69b8c-299">Role</span></span>

* <span data-ttu-id="69b8c-300">`az role assignment create/update`: dar suporte a `--description`, `--condition` e `--condition-version`</span><span class="sxs-lookup"><span data-stu-id="69b8c-300">`az role assignment create/update`: Support `--description`, `--condition` and `--condition-version`</span></span>
* <span data-ttu-id="69b8c-301">`az ad app permission delete`: dar suporte a `--api-permissions` para excluir o `ResourceAccess` específico</span><span class="sxs-lookup"><span data-stu-id="69b8c-301">`az ad app permission delete`: Support `--api-permissions` to delete specific `ResourceAccess`</span></span>

### <a name="service-fabric"></a><span data-ttu-id="69b8c-302">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="69b8c-302">Service Fabric</span></span>

* <span data-ttu-id="69b8c-303">Adicionar comandos de tipo de nó e cluster gerenciado</span><span class="sxs-lookup"><span data-stu-id="69b8c-303">Add managed cluster and node type commands</span></span>

### <a name="sql"></a><span data-ttu-id="69b8c-304">SQL</span><span class="sxs-lookup"><span data-stu-id="69b8c-304">SQL</span></span>

* <span data-ttu-id="69b8c-305">Atualizar azure-mgmt-sql para 0.20.0</span><span class="sxs-lookup"><span data-stu-id="69b8c-305">Upgrade azure-mgmt-sql to 0.20.0</span></span>
* <span data-ttu-id="69b8c-306">Adicionar parâmetro opcional de redundância de armazenamento de backup ao cmdlet MI create</span><span class="sxs-lookup"><span data-stu-id="69b8c-306">Add backup storage redundancy optional parameter to MI create cmdlet</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-307">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-307">Storage</span></span>

* <span data-ttu-id="69b8c-308">`az storage share-rm stats`: obter os bytes de uso dos dados armazenados no compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="69b8c-308">`az storage share-rm stats`: Get the usage bytes of the data stored on the share.</span></span>
* <span data-ttu-id="69b8c-309">PITR de blob de armazenamento de versão GA</span><span class="sxs-lookup"><span data-stu-id="69b8c-309">GA release storage blob PITR</span></span>
* <span data-ttu-id="69b8c-310">`az storage blob query`: dar suporte à Aceleração de Consulta do Armazenamento do Azure</span><span class="sxs-lookup"><span data-stu-id="69b8c-310">`az storage blob query`: Support Azure Storage Query Acceleration</span></span>
* <span data-ttu-id="69b8c-311">Dar suporte à exclusão reversível para o compartilhamento de arquivo</span><span class="sxs-lookup"><span data-stu-id="69b8c-311">Support Soft Delete for file share</span></span>
* <span data-ttu-id="69b8c-312">`az storage copy`: adicionar suporte a credenciais de conta e substituir `--source-local-path`, `--destination-local-path`, `--destination-account-name`</span><span class="sxs-lookup"><span data-stu-id="69b8c-312">`az storage copy`: Add account credentials support and deprecate `--source-local-path`, `--destination-local-path`, `--destination-account-name`</span></span>
* <span data-ttu-id="69b8c-313">`az storage account blob-service-properties update`: adicionar suporte à política de retenção de exclusão de contêiner</span><span class="sxs-lookup"><span data-stu-id="69b8c-313">`az storage account blob-service-properties update`: Add container delete retention policy support</span></span>

### <a name="synapse"></a><span data-ttu-id="69b8c-314">Synapse</span><span class="sxs-lookup"><span data-stu-id="69b8c-314">Synapse</span></span>

* <span data-ttu-id="69b8c-315">Correção de erro de digitação no exemplo de criação e exclusão de atribuição de função do az synapse</span><span class="sxs-lookup"><span data-stu-id="69b8c-315">Fixed typo in example of az synapse role assignment create and delete</span></span>

## <a name="august-28-2020"></a><span data-ttu-id="69b8c-316">28 de agosto de 2020</span><span class="sxs-lookup"><span data-stu-id="69b8c-316">August 28, 2020</span></span>

<span data-ttu-id="69b8c-317">Versão 2.11.1</span><span class="sxs-lookup"><span data-stu-id="69b8c-317">Version 2.11.1</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-318">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-318">ACR</span></span>

* <span data-ttu-id="69b8c-319">Adição de camada isolada ao pool de agentes</span><span class="sxs-lookup"><span data-stu-id="69b8c-319">Add Isolated Tier to Agent Pool</span></span>
* <span data-ttu-id="69b8c-320">Adição de contexto de origem do artefato de OCI</span><span class="sxs-lookup"><span data-stu-id="69b8c-320">Add OCI Artifact Source Context</span></span>

### <a name="aks"></a><span data-ttu-id="69b8c-321">AKS</span><span class="sxs-lookup"><span data-stu-id="69b8c-321">AKS</span></span>

* <span data-ttu-id="69b8c-322">Correção de um problema de criação do cluster do AKS</span><span class="sxs-lookup"><span data-stu-id="69b8c-322">Fix aks cluster create issue</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="69b8c-323">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="69b8c-323">Cognitive Services</span></span>

* <span data-ttu-id="69b8c-324">[ALTERAÇÃO DA FALHA] Mostrar um termo legal adicional para determinadas APIs</span><span class="sxs-lookup"><span data-stu-id="69b8c-324">[BREAKING CHANGE] Show additional legal term for certain APIs</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-325">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-325">Network</span></span>

* <span data-ttu-id="69b8c-326">[ALTERAÇÃO DA FALHA] Permitir a criação de IP público e IP privado ao criar um Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="69b8c-326">[BREAKING CHANGE] Allow to create both public and private IP while creating an Application Gateway</span></span>
* <span data-ttu-id="69b8c-327">`az network list-service-tags`: adição de detalhes sobre o uso de parâmetro de localização para a mensagem de ajuda</span><span class="sxs-lookup"><span data-stu-id="69b8c-327">`az network list-service-tags`: add details on location parameter use to the help message</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-328">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-328">Storage</span></span>

* <span data-ttu-id="69b8c-329">`az storage blob list`: suporte OU propriedades com a nova versão de API</span><span class="sxs-lookup"><span data-stu-id="69b8c-329">`az storage blob list`: Support OR properties with new api version</span></span>

## <a name="august-25-2020"></a><span data-ttu-id="69b8c-330">25 de agosto de 2020</span><span class="sxs-lookup"><span data-stu-id="69b8c-330">August 25, 2020</span></span>

<span data-ttu-id="69b8c-331">Versão 2.11.0</span><span class="sxs-lookup"><span data-stu-id="69b8c-331">Version 2.11.0</span></span>

### <a name="aks"></a><span data-ttu-id="69b8c-332">AKS</span><span class="sxs-lookup"><span data-stu-id="69b8c-332">AKS</span></span>

* <span data-ttu-id="69b8c-333">Remoção da marca de visualização do complemento de Nó Virtual</span><span class="sxs-lookup"><span data-stu-id="69b8c-333">Remove preview tag from Virtual Node add-on</span></span>
* <span data-ttu-id="69b8c-334">Adição do argumento CMK do AKS na criação do cluster</span><span class="sxs-lookup"><span data-stu-id="69b8c-334">Add AKS CMK argument in cluster creation</span></span>
* <span data-ttu-id="69b8c-335">Definição do perfil de rede durante o uso do balanceador de carga básico.</span><span class="sxs-lookup"><span data-stu-id="69b8c-335">Set network profile when using basic load balancer.</span></span>
* <span data-ttu-id="69b8c-336">Remoção da validação máxima de pods da CLI e permissão para que a simulação lide com ela</span><span class="sxs-lookup"><span data-stu-id="69b8c-336">Remove max pods validation from CLI and let preflight handle it</span></span>
* <span data-ttu-id="69b8c-337">Correção de complementos disponíveis na mensagem de ajuda em `az aks create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-337">Fixing add-ons available in the help message in `az aks create`</span></span>
* <span data-ttu-id="69b8c-338">Introdução de suporte para o perfil de dimensionamento automático do cluster na CLI principal</span><span class="sxs-lookup"><span data-stu-id="69b8c-338">Bring in support for cluster autoscaler profile in core CLI</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-339">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-339">AppService</span></span>

* <span data-ttu-id="69b8c-340">`az webapp`: adição do comando list-instances</span><span class="sxs-lookup"><span data-stu-id="69b8c-340">`az webapp`: Add list-instances command</span></span>
* <span data-ttu-id="69b8c-341">`az webapp ssh`: adição do parâmetro --instance para se conectar a uma instância específica</span><span class="sxs-lookup"><span data-stu-id="69b8c-341">`az webapp ssh`: Add --instance parameter to connect to a specific instance</span></span>
* <span data-ttu-id="69b8c-342">`az webapp create-remote-connection`: adição do parâmetro --instance para se conectar a uma instância específica</span><span class="sxs-lookup"><span data-stu-id="69b8c-342">`az webapp create-remote-connection`: Add --instance parameter to connect to a specific instance</span></span>
* <span data-ttu-id="69b8c-343">Correção nº 14758: erros de az webapp create durante a criação de um aplicativo do Windows com --runtime dotnetcore</span><span class="sxs-lookup"><span data-stu-id="69b8c-343">Fix #14758: az webapp create errors when creating windows app with --runtime dotnetcore</span></span>
* <span data-ttu-id="69b8c-344">Correção nº 14701: implementação de functionapp create --assign-identity</span><span class="sxs-lookup"><span data-stu-id="69b8c-344">Fix #14701: Implement functionapp create --assign-identity</span></span>
* <span data-ttu-id="69b8c-345">Correção nº 11244: `az webapp auth update`: adição do parâmetro opcional para atualizar client-secret-certificate-thumbprint</span><span class="sxs-lookup"><span data-stu-id="69b8c-345">Fix #11244: `az webapp auth update`: Add optional parameter to update client-secret-certificate-thumbprint</span></span>
* <span data-ttu-id="69b8c-346">`az functionapp keys`: comandos adicionados que permitem aos usuários gerenciar as chaves do aplicativo de funções</span><span class="sxs-lookup"><span data-stu-id="69b8c-346">`az functionapp keys`: Added commands that allow users to manage their function app keys</span></span>
* <span data-ttu-id="69b8c-347">`az functionapp function`: comandos adicionados que permitem aos usuários gerenciar as funções individuais</span><span class="sxs-lookup"><span data-stu-id="69b8c-347">`az functionapp function`: Added commands that allow users to manage their individual functions</span></span>
* <span data-ttu-id="69b8c-348">`az functionapp function keys`: comandos adicionados que permitem aos usuários gerenciar as chaves de função</span><span class="sxs-lookup"><span data-stu-id="69b8c-348">`az functionapp function keys`: Added commands that allow users to manage their function keys</span></span>
* <span data-ttu-id="69b8c-349">Correção nº14788: az webapp create não obtém o webapp correto quando os nomes são substrings</span><span class="sxs-lookup"><span data-stu-id="69b8c-349">Fix #14788: az webapp create not getting correct webapp when names are substrings</span></span>
* <span data-ttu-id="69b8c-350">`az functionapp create`: capacidade removida para criar funções 2.x em regiões que não têm compatibilidade</span><span class="sxs-lookup"><span data-stu-id="69b8c-350">`az functionapp create`: Removed ability to create 2.x Functions in regions that don't support it</span></span>

### <a name="arm"></a><span data-ttu-id="69b8c-351">ARM</span><span class="sxs-lookup"><span data-stu-id="69b8c-351">ARM</span></span>

* <span data-ttu-id="69b8c-352">`az resource list`: extensão dos dados retornados de `createdTime`, `changedTime` e `provisioningState`</span><span class="sxs-lookup"><span data-stu-id="69b8c-352">`az resource list`: Extend the return data of `createdTime`, `changedTime` and `provisioningState`</span></span>
* <span data-ttu-id="69b8c-353">`az resource`: adição do parâmetro `--latest-include-preview` para dar suporte ao uso da api-version mais recente se ela for versão prévia</span><span class="sxs-lookup"><span data-stu-id="69b8c-353">`az resource`: Add parameter `--latest-include-preview` to support using the latest api-version whether this version is preview</span></span>

### <a name="aro"></a><span data-ttu-id="69b8c-354">ARO</span><span class="sxs-lookup"><span data-stu-id="69b8c-354">ARO</span></span>

* <span data-ttu-id="69b8c-355">Aprimoramentos da CLI, incluindo permissões de verificação da tabela de rotas</span><span class="sxs-lookup"><span data-stu-id="69b8c-355">CLI enhancements, including route table checking permissions</span></span>

### <a name="cloud"></a><span data-ttu-id="69b8c-356">Nuvem</span><span class="sxs-lookup"><span data-stu-id="69b8c-356">Cloud</span></span>

* <span data-ttu-id="69b8c-357">`az cloud register`: correção do registro de nuvens com um arquivo de configuração</span><span class="sxs-lookup"><span data-stu-id="69b8c-357">`az cloud register`: Fix registering clouds with a config file</span></span>

### <a name="compute"></a><span data-ttu-id="69b8c-358">Computação</span><span class="sxs-lookup"><span data-stu-id="69b8c-358">Compute</span></span>

* <span data-ttu-id="69b8c-359">Atualização de SKUs de VM compatíveis com rede acelerada</span><span class="sxs-lookup"><span data-stu-id="69b8c-359">Update VM SKUs that support accelerated networking</span></span>
* <span data-ttu-id="69b8c-360">`az vm create`: aplicação automática de patches no convidado</span><span class="sxs-lookup"><span data-stu-id="69b8c-360">`az vm create`: Automatic in-guest patching</span></span>
* <span data-ttu-id="69b8c-361">`az image builder create`: adição de --vm-size, --os-disk-size, --vnet, --subnet</span><span class="sxs-lookup"><span data-stu-id="69b8c-361">`az image builder create`: Add --vm-size, --os-disk-size, --vnet, --subnet</span></span>
* <span data-ttu-id="69b8c-362">Novo comando az vm assess-patches</span><span class="sxs-lookup"><span data-stu-id="69b8c-362">New command az vm assess-patches</span></span>

### <a name="container"></a><span data-ttu-id="69b8c-363">Contêiner</span><span class="sxs-lookup"><span data-stu-id="69b8c-363">Container</span></span>

* <span data-ttu-id="69b8c-364">Correção nº 6235: atualização do texto de ajuda para o parâmetro de portas na criação do contêiner</span><span class="sxs-lookup"><span data-stu-id="69b8c-364">Fix #6235: Update help text for ports parameter in container create</span></span>

### <a name="datalake-store"></a><span data-ttu-id="69b8c-365">Datalake Store</span><span class="sxs-lookup"><span data-stu-id="69b8c-365">Datalake Store</span></span>

* <span data-ttu-id="69b8c-366">Correção do problema nº 14545 para a operação de ingresso no data lake</span><span class="sxs-lookup"><span data-stu-id="69b8c-366">Fix issue #14545 for data lake join operation</span></span>

### <a name="eventhub"></a><span data-ttu-id="69b8c-367">EventHub</span><span class="sxs-lookup"><span data-stu-id="69b8c-367">EventHub</span></span>

* <span data-ttu-id="69b8c-368">`az eventhubs eventhub create/update`: alterar a documentação de destination_name</span><span class="sxs-lookup"><span data-stu-id="69b8c-368">`az eventhubs eventhub create/update`: Change documentation of destination_name</span></span>

### <a name="extension"></a><span data-ttu-id="69b8c-369">Extensão</span><span class="sxs-lookup"><span data-stu-id="69b8c-369">Extension</span></span>

* <span data-ttu-id="69b8c-370">Adição do comando `az extension list-versions` para listar todas as versões disponíveis de uma extensão</span><span class="sxs-lookup"><span data-stu-id="69b8c-370">Add `az extension list-versions` command to list all available versions of an extension</span></span>

### <a name="hdinsight"></a><span data-ttu-id="69b8c-371">HDInsight</span><span class="sxs-lookup"><span data-stu-id="69b8c-371">HDInsight</span></span>

* <span data-ttu-id="69b8c-372">Suporte à criação de cluster com configuração de dimensionamento automático e suporte ao gerenciamento de configuração de dimensionamento automático</span><span class="sxs-lookup"><span data-stu-id="69b8c-372">Support creating cluster with autoscale configuration and Support managing autoscale configuration</span></span>
* <span data-ttu-id="69b8c-373">Suporte à criação de cluster com criptografia no host</span><span class="sxs-lookup"><span data-stu-id="69b8c-373">Support creating cluster with encryption at host</span></span>

### <a name="iotcentral"></a><span data-ttu-id="69b8c-374">IoT Central</span><span class="sxs-lookup"><span data-stu-id="69b8c-374">IoTCentral</span></span>

* <span data-ttu-id="69b8c-375">Aprimoramentos na documentação da CLI</span><span class="sxs-lookup"><span data-stu-id="69b8c-375">CLI documentation improvements</span></span>

### <a name="monitor"></a><span data-ttu-id="69b8c-376">Monitor</span><span class="sxs-lookup"><span data-stu-id="69b8c-376">Monitor</span></span>

* <span data-ttu-id="69b8c-377">`az monitor metrics alert create`: suporte a RG e Sub como os valores de escopo</span><span class="sxs-lookup"><span data-stu-id="69b8c-377">`az monitor metrics alert create`: support RG and Sub as the scope values</span></span>

### <a name="netappfiles"></a><span data-ttu-id="69b8c-378">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="69b8c-378">NetAppFiles</span></span>

* <span data-ttu-id="69b8c-379">[ALTERAÇÃO DA FALHA] az netappfiles snapshot create: file-system-id removido dos parâmetros</span><span class="sxs-lookup"><span data-stu-id="69b8c-379">[BREAKING CHANGE] az netappfiles snapshot create: Removed file-system-id from parameters</span></span>
* <span data-ttu-id="69b8c-380">[ALTERAÇÃO DA FALHA] az netappfiles snapshot show: o instantâneo não tem mais o parâmetro file-system-id</span><span class="sxs-lookup"><span data-stu-id="69b8c-380">[BREAKING CHANGE] az netappfiles snapshot show: Snapshot no longer has parameter file-system-id</span></span>
* <span data-ttu-id="69b8c-381">`az netappfiles account`: Model ActiveDirectory tem um novo parâmetro backup_operators</span><span class="sxs-lookup"><span data-stu-id="69b8c-381">`az netappfiles account`: Model ActiveDirectory has a new parameter backup_operators</span></span>
* <span data-ttu-id="69b8c-382">`az netappfiles volume show`: Model dataProtection tem um novo parâmetro snapshot</span><span class="sxs-lookup"><span data-stu-id="69b8c-382">`az netappfiles volume show`: Model dataProtection has a new parameter snapshot</span></span>
* <span data-ttu-id="69b8c-383">`az netappfiles volume show`: Model Volume tem um novo parâmetro snapshot_directory_visible</span><span class="sxs-lookup"><span data-stu-id="69b8c-383">`az netappfiles volume show`: Model Volume has a new parameter snapshot_directory_visible</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-384">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-384">Network</span></span>

* <span data-ttu-id="69b8c-385">`az network dns export`: exportação do FQDN para o tipo MX, PTR, NS e SRV em vez do caminho relativo</span><span class="sxs-lookup"><span data-stu-id="69b8c-385">`az network dns export`: export FQDN for MX, PTR, NS and SRV type instead of relative path</span></span>
* <span data-ttu-id="69b8c-386">Suporte ao link privado para discos gerenciados</span><span class="sxs-lookup"><span data-stu-id="69b8c-386">Support private link for managed disks</span></span>
* <span data-ttu-id="69b8c-387">`az network application-gateway auth-cert show`: adição de exemplo para demonstrar o formato do certificado</span><span class="sxs-lookup"><span data-stu-id="69b8c-387">`az network application-gateway auth-cert show`: Add example to demonstrate certificate format</span></span>
* <span data-ttu-id="69b8c-388">`az network private-endpoint-connection`: suporte à configuração de aplicativos</span><span class="sxs-lookup"><span data-stu-id="69b8c-388">`az network private-endpoint-connection`: support app configuration</span></span>

### <a name="rbac"></a><span data-ttu-id="69b8c-389">RBAC</span><span class="sxs-lookup"><span data-stu-id="69b8c-389">RBAC</span></span>

* <span data-ttu-id="69b8c-390">`az ad group create`: suporte à especificação da descrição durante a criação de um grupo</span><span class="sxs-lookup"><span data-stu-id="69b8c-390">`az ad group create`: support specify description when creating a group</span></span>
* <span data-ttu-id="69b8c-391">`az role definition create`: impressão de mensagem legível em vez de exceção quando assignableScope for uma matriz vazia</span><span class="sxs-lookup"><span data-stu-id="69b8c-391">`az role definition create`: print human readable message instead of exception when assignableScope is an empty array</span></span>
* <span data-ttu-id="69b8c-392">[ALTERAÇÃO DA FALHA] `az ad sp create-for-rbac`: alteração da permissão padrão do certificado criado</span><span class="sxs-lookup"><span data-stu-id="69b8c-392">[BREAKING CHANGE] `az ad sp create-for-rbac`: change default permission of created certificate</span></span>

### <a name="sql"></a><span data-ttu-id="69b8c-393">SQL</span><span class="sxs-lookup"><span data-stu-id="69b8c-393">SQL</span></span>

* <span data-ttu-id="69b8c-394">`az sql server audit-policy`: adição de suporte à auditoria do SQL Server</span><span class="sxs-lookup"><span data-stu-id="69b8c-394">`az sql server audit-policy`: Add sql server auditing support</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-395">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-395">Storage</span></span>

* <span data-ttu-id="69b8c-396">`az storage blob copy start-batch`: correção nº 6018 para --source-sas</span><span class="sxs-lookup"><span data-stu-id="69b8c-396">`az storage blob copy start-batch`: Fix #6018 for --source-sas</span></span>
* <span data-ttu-id="69b8c-397">`az storage account or-policy`: suporte à política de replicação de objeto de conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-397">`az storage account or-policy`: Support storage account object replication policy</span></span>
* <span data-ttu-id="69b8c-398">Correção do problema nº 14083 para atualizar a versão do pacote do azure-multiapi-storage para o problema do pacote e suporte da versão à nova API</span><span class="sxs-lookup"><span data-stu-id="69b8c-398">Fix issue #14083 to upgrade azure-multiapi-storage package version for package issue and new api version support</span></span>
* <span data-ttu-id="69b8c-399">`az storage blob generate-sas`: adição de exemplos para --ip e refinamento da mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="69b8c-399">`az storage blob generate-sas`: add examples for --ip  and refine error message</span></span>
* <span data-ttu-id="69b8c-400">`az storage blob list`: correção do problema de next_marker</span><span class="sxs-lookup"><span data-stu-id="69b8c-400">`az storage blob list`: Fix next_marker issue</span></span>

### <a name="synapse"></a><span data-ttu-id="69b8c-401">Synapse</span><span class="sxs-lookup"><span data-stu-id="69b8c-401">Synapse</span></span>

* <span data-ttu-id="69b8c-402">Adição de cmdlets relacionados a workspace, sparkpool e sqlpool</span><span class="sxs-lookup"><span data-stu-id="69b8c-402">Add workspace, sparkpool, sqlpool related cmdlets</span></span>
* <span data-ttu-id="69b8c-403">Adição de comandos relacionados a spark job com base no track2 sdk</span><span class="sxs-lookup"><span data-stu-id="69b8c-403">Add spark job releated commands based on track2 sdk</span></span>
* <span data-ttu-id="69b8c-404">Adição de comandos relacionados ao recurso accesscontrol com base no track2 sdk</span><span class="sxs-lookup"><span data-stu-id="69b8c-404">Add accesscontrol feature related commands based on track2 sdk</span></span>

### <a name="upgrade"></a><span data-ttu-id="69b8c-405">Atualizar</span><span class="sxs-lookup"><span data-stu-id="69b8c-405">Upgrade</span></span>

* <span data-ttu-id="69b8c-406">Adição do comando `az upgrade` para atualizar a CLI do Azure e as extensões</span><span class="sxs-lookup"><span data-stu-id="69b8c-406">Add `az upgrade` command to upgrade azure cli and extensions</span></span>

## <a name="august-11-2020"></a><span data-ttu-id="69b8c-407">11 de agosto de 2020</span><span class="sxs-lookup"><span data-stu-id="69b8c-407">August 11, 2020</span></span>

<span data-ttu-id="69b8c-408">Versão 2.10.1</span><span class="sxs-lookup"><span data-stu-id="69b8c-408">Version 2.10.1</span></span>

### <a name="app-service"></a><span data-ttu-id="69b8c-409">Serviço de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="69b8c-409">App Service</span></span>

* <span data-ttu-id="69b8c-410">Correção nº 9887 webapp e functionapp, dar suporte à atribuição/remoção de identidade gerenciada pelo usuário</span><span class="sxs-lookup"><span data-stu-id="69b8c-410">Fix #9887 webapp and functionapp, support assigning/removing user managed identity</span></span>
* <span data-ttu-id="69b8c-411">Correção nº 1382, 14055: atualizar mensagens de erro para az webapp create e az webapp config container set</span><span class="sxs-lookup"><span data-stu-id="69b8c-411">Fix #1382, #14055: Update error messages for az webapp create and az webapp config container set</span></span>
* <span data-ttu-id="69b8c-412">`az webapp up`: corrigir a lógica de seleção padrão do ASP quando o parâmetro --plan não é fornecido</span><span class="sxs-lookup"><span data-stu-id="69b8c-412">`az webapp up`: Fix default ASP selection logic when --plan parameter is not provided</span></span>

### <a name="appconfig"></a><span data-ttu-id="69b8c-413">AppConfig</span><span class="sxs-lookup"><span data-stu-id="69b8c-413">AppConfig</span></span>

* <span data-ttu-id="69b8c-414">Dar suporte para habilitar/desabilitar PublicNetworkAccess durante a criação da loja</span><span class="sxs-lookup"><span data-stu-id="69b8c-414">Support enabling/disabling PublicNetworkAccess during store creation</span></span>

### <a name="compute"></a><span data-ttu-id="69b8c-415">Computação</span><span class="sxs-lookup"><span data-stu-id="69b8c-415">Compute</span></span>

* <span data-ttu-id="69b8c-416">Dar suporte à associação de disco e instantâneo com um recurso de acesso a disco</span><span class="sxs-lookup"><span data-stu-id="69b8c-416">Support associating disk and snapshot with a disk-access resource</span></span>

### <a name="lab"></a><span data-ttu-id="69b8c-417">Laboratório</span><span class="sxs-lookup"><span data-stu-id="69b8c-417">Lab</span></span>

* <span data-ttu-id="69b8c-418">Correção do problema nº 7904: bug de validação de data na criação de VM do laboratório</span><span class="sxs-lookup"><span data-stu-id="69b8c-418">Fix for issue #7904 date validation bug in lab vm creation</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-419">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-419">Storage</span></span>

* <span data-ttu-id="69b8c-420">`az storage blob upload-batch`: correção do problema nº 14660 com argumentos não posicionais</span><span class="sxs-lookup"><span data-stu-id="69b8c-420">`az storage blob upload-batch`: Fix issue #14660 with unpositional arguments</span></span>

## <a name="august-04-2020"></a><span data-ttu-id="69b8c-421">04 de agosto de 2020</span><span class="sxs-lookup"><span data-stu-id="69b8c-421">August 04, 2020</span></span>

<span data-ttu-id="69b8c-422">Versão 2.10.0</span><span class="sxs-lookup"><span data-stu-id="69b8c-422">Version 2.10.0</span></span>

### <a name="aks"></a><span data-ttu-id="69b8c-423">AKS</span><span class="sxs-lookup"><span data-stu-id="69b8c-423">AKS</span></span>

* <span data-ttu-id="69b8c-424">`az aks update`: Alteração do argumento --enable-aad para migrar um cluster não AAD habilitado para RBAC para um cluster AAD gerenciado por AKS</span><span class="sxs-lookup"><span data-stu-id="69b8c-424">`az aks update`: Change --enable-aad argument to migrate a RBAC-enabled non-AAD cluster to a AKS-managed AAD cluster</span></span>
* <span data-ttu-id="69b8c-425">`az aks install-cli`: Adição de argumentos --kubelogin-version e --kubelogin-install-location para instalar o kubelogin</span><span class="sxs-lookup"><span data-stu-id="69b8c-425">`az aks install-cli`: Add --kubelogin-version and --kubelogin-install-location arguments to install kubelogin</span></span>
* <span data-ttu-id="69b8c-426">Adição do comando az aks nodepool get-upgrades</span><span class="sxs-lookup"><span data-stu-id="69b8c-426">Add az aks nodepool get-upgrades command</span></span>

### <a name="ams"></a><span data-ttu-id="69b8c-427">AMS</span><span class="sxs-lookup"><span data-stu-id="69b8c-427">AMS</span></span>

* <span data-ttu-id="69b8c-428">Correção nº 14021: az ams account sp não é idempotente</span><span class="sxs-lookup"><span data-stu-id="69b8c-428">Fix #14021: az ams account sp is not idempotent</span></span>

### <a name="apim"></a><span data-ttu-id="69b8c-429">APIM</span><span class="sxs-lookup"><span data-stu-id="69b8c-429">APIM</span></span>

* <span data-ttu-id="69b8c-430">importação da API de APIM: suporte à importação de API e aprimoramento de outros comandos da CLI de nível da API</span><span class="sxs-lookup"><span data-stu-id="69b8c-430">apim api import: support API import and enchance other api level cli commands</span></span>

### <a name="app-service"></a><span data-ttu-id="69b8c-431">Serviço de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="69b8c-431">App Service</span></span>

* <span data-ttu-id="69b8c-432">Correção nº 13035: Adição de validação para az webapp config access-restriction para evitar a adição de duplicatas</span><span class="sxs-lookup"><span data-stu-id="69b8c-432">Fix #13035: Add validation for az webapp config access-restriction to avoid adding duplicates</span></span>

### <a name="appconfig"></a><span data-ttu-id="69b8c-433">AppConfig</span><span class="sxs-lookup"><span data-stu-id="69b8c-433">AppConfig</span></span>

* <span data-ttu-id="69b8c-434">Adoção de SKU padrão se não for especificado</span><span class="sxs-lookup"><span data-stu-id="69b8c-434">Default to standard sku if not specified</span></span>
* <span data-ttu-id="69b8c-435">[ALTERAÇÃO SIGNIFICATIVA] Configurações de suporte com tipo de conteúdo JSON</span><span class="sxs-lookup"><span data-stu-id="69b8c-435">[BREAKING CHANGE] Support settings with JSON content type</span></span>

### <a name="arm"></a><span data-ttu-id="69b8c-436">ARM</span><span class="sxs-lookup"><span data-stu-id="69b8c-436">ARM</span></span>

* <span data-ttu-id="69b8c-437">`az resource tag`: Correção do bug de marcação managedApp e alguns problemas de teste relacionados</span><span class="sxs-lookup"><span data-stu-id="69b8c-437">`az resource tag`: Fix the bug of managedApp tagging and some related test issues</span></span>
* <span data-ttu-id="69b8c-438">`az deployment mg/tenant what-if`: Adição de suporte ao grupo de gerenciamento e à implantação de nível de locatário What-If</span><span class="sxs-lookup"><span data-stu-id="69b8c-438">`az deployment mg/tenant what-if`: Add support to management group and tenant level deployment What-If</span></span>
* <span data-ttu-id="69b8c-439">`az deployment mg/tenant create`: Adição do parâmetro --confirm-with-what-if/-c.</span><span class="sxs-lookup"><span data-stu-id="69b8c-439">`az deployment mg/tenant create`: Add --confirm-with-what-if/-c parameter.</span></span>
* <span data-ttu-id="69b8c-440">`az deployment mg/tenant create`: Adição do parâmetro --what-if-result-format/-r.</span><span class="sxs-lookup"><span data-stu-id="69b8c-440">`az deployment mg/tenant create`: Add --what-if-result-format/-r parameter.</span></span>
* <span data-ttu-id="69b8c-441">`az deployment mg/tenant create`: adicionar parâmetro --what-if-exclude-change-types/-x.</span><span class="sxs-lookup"><span data-stu-id="69b8c-441">`az deployment mg/tenant create`: Add --what-if-exclude-change-types/-x parameter.</span></span>
* <span data-ttu-id="69b8c-442">`az tag`: az tag support para parâmetro ID de recurso</span><span class="sxs-lookup"><span data-stu-id="69b8c-442">`az tag`: az tag support for resource id parameter</span></span>

### <a name="backup"></a><span data-ttu-id="69b8c-443">Backup</span><span class="sxs-lookup"><span data-stu-id="69b8c-443">Backup</span></span>

* <span data-ttu-id="69b8c-444">Disparar a descoberta de contêiner/item AFS somente quando necessário</span><span class="sxs-lookup"><span data-stu-id="69b8c-444">Trigger AFS container/item discovery only when needed</span></span>

### <a name="cdn"></a><span data-ttu-id="69b8c-445">CDN</span><span class="sxs-lookup"><span data-stu-id="69b8c-445">CDN</span></span>

* <span data-ttu-id="69b8c-446">Adicionar campos de link privado à origem</span><span class="sxs-lookup"><span data-stu-id="69b8c-446">Add private link fields to origin</span></span>

### <a name="compute"></a><span data-ttu-id="69b8c-447">Computação</span><span class="sxs-lookup"><span data-stu-id="69b8c-447">Compute</span></span>

* <span data-ttu-id="69b8c-448">`az vm/vmss create`: Selecione um nome de usuário válido para usuário se o nome de usuário padrão for inválido</span><span class="sxs-lookup"><span data-stu-id="69b8c-448">`az vm/vmss create`: Select a valid username for user if the default username is invalid</span></span>
* <span data-ttu-id="69b8c-449">`az vm update`: suporte à imagem entre locatários</span><span class="sxs-lookup"><span data-stu-id="69b8c-449">`az vm update`: support cross tenant image</span></span>
* <span data-ttu-id="69b8c-450">`az disk-access`: Adicionar novo grupo de comandos para operar o recurso de acesso ao disco</span><span class="sxs-lookup"><span data-stu-id="69b8c-450">`az disk-access`: Add new command group to operate disk access resource</span></span>
* <span data-ttu-id="69b8c-451">Suporte ao posicionamento automático do grupo de hosts dedicado</span><span class="sxs-lookup"><span data-stu-id="69b8c-451">Support dedicated host group automatic placement</span></span>
* <span data-ttu-id="69b8c-452">Suporte a PPG e SPG no modo de orquestração de VMSS</span><span class="sxs-lookup"><span data-stu-id="69b8c-452">Support ppg and spg in VMSS orchestration mode</span></span>

### <a name="config"></a><span data-ttu-id="69b8c-453">Config</span><span class="sxs-lookup"><span data-stu-id="69b8c-453">Config</span></span>

* <span data-ttu-id="69b8c-454">`az config`: Adição do novo módulo de comando `config`</span><span class="sxs-lookup"><span data-stu-id="69b8c-454">`az config`: Add new `config` command module</span></span>

### <a name="extension"></a><span data-ttu-id="69b8c-455">Extensão</span><span class="sxs-lookup"><span data-stu-id="69b8c-455">Extension</span></span>

* <span data-ttu-id="69b8c-456">Suporte à instalação automática de uma extensão se a extensão de um comando não estiver instalada</span><span class="sxs-lookup"><span data-stu-id="69b8c-456">Support automatically installing an extension if the extension of a command is not installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="69b8c-457">HDInsight</span><span class="sxs-lookup"><span data-stu-id="69b8c-457">HDInsight</span></span>

* <span data-ttu-id="69b8c-458">Adição de três parâmetros ao comando `az hdinsight create` para compatibilidade com o link privado e o recurso de criptografia em trânsito:</span><span class="sxs-lookup"><span data-stu-id="69b8c-458">Add 3 parameters to the command `az hdinsight create` to support private link and encryption in transit feature:</span></span>

### <a name="iot-hub"></a><span data-ttu-id="69b8c-459">Hub IoT</span><span class="sxs-lookup"><span data-stu-id="69b8c-459">Iot Hub</span></span>

* <span data-ttu-id="69b8c-460">Correção nº 7792: A criação do Hub IoT não é idempotente</span><span class="sxs-lookup"><span data-stu-id="69b8c-460">Fix #7792: IoT Hub Create is not idempotent</span></span>

### <a name="iot-central"></a><span data-ttu-id="69b8c-461">Central da IoT</span><span class="sxs-lookup"><span data-stu-id="69b8c-461">IoT Central</span></span>

* <span data-ttu-id="69b8c-462">Adição de lista de opções de parâmetros para IoT Central</span><span class="sxs-lookup"><span data-stu-id="69b8c-462">Add paramater option list for iot central</span></span>

### <a name="keyvault"></a><span data-ttu-id="69b8c-463">KeyVault</span><span class="sxs-lookup"><span data-stu-id="69b8c-463">KeyVault</span></span>

* <span data-ttu-id="69b8c-464">`az keyvault key encrypt/decrypt`: adição de parâmetro `--data-type` para especificar explicitamente o tipo de dado original</span><span class="sxs-lookup"><span data-stu-id="69b8c-464">`az keyvault key encrypt/decrypt`: add parameter `--data-type` for explicitly specifing the type of original data</span></span>

### <a name="monitor"></a><span data-ttu-id="69b8c-465">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="69b8c-465">Monitor</span></span>

* <span data-ttu-id="69b8c-466">`az monitor log-analytics workspace data-export`: suporte ao namespace do hub de eventos como o destino.</span><span class="sxs-lookup"><span data-stu-id="69b8c-466">`az monitor log-analytics workspace data-export`: support event hub namespace as the destination.</span></span>
* <span data-ttu-id="69b8c-467">`az monitor autoscale`: suporte a namespace e dimensões para --condition</span><span class="sxs-lookup"><span data-stu-id="69b8c-467">`az monitor autoscale`: support namespace and dimensions for --condition</span></span>

### <a name="netappfiles"></a><span data-ttu-id="69b8c-468">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="69b8c-468">NetAppFiles</span></span>

* <span data-ttu-id="69b8c-469">`az volume revert`:  Adição de Reversão de Volume para reverter um volume para um de seus instantâneos.</span><span class="sxs-lookup"><span data-stu-id="69b8c-469">`az volume revert`:  Add Volume Revert to revert a volume to one of its snapshots.</span></span>
* <span data-ttu-id="69b8c-470">[ALTERAÇÃO SIGNIFICATIVA] Remoção de `az netappfiles mount-target`.</span><span class="sxs-lookup"><span data-stu-id="69b8c-470">[BREAKING CHANGE] Remove `az netappfiles mount-target`.</span></span>
* <span data-ttu-id="69b8c-471">`az volume show`: Adição de site para Propriedades do Active Directory</span><span class="sxs-lookup"><span data-stu-id="69b8c-471">`az volume show`: Add site to Active Directory Properties</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-472">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-472">Network</span></span>

* <span data-ttu-id="69b8c-473">`az application-gateway private-link add`: suporte para especificar uma sub-rede existente por ID</span><span class="sxs-lookup"><span data-stu-id="69b8c-473">`az application-gateway private-link add`: support to specify an existing subnet by ID</span></span>
* <span data-ttu-id="69b8c-474">`az network application-gateway waf-policy create`: versão e tipo de suporte</span><span class="sxs-lookup"><span data-stu-id="69b8c-474">`az network application-gateway waf-policy create`: support version and type</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-475">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-475">Storage</span></span>

* <span data-ttu-id="69b8c-476">Correção nº 10302: Suporte à estimativa de tipo de conteúdo ao sincronizar arquivos</span><span class="sxs-lookup"><span data-stu-id="69b8c-476">Fix #10302: Support guess content-type when synchronizing files</span></span>
* <span data-ttu-id="69b8c-477">`az storage blob lease`: Aplicação de nova versão de API para operações de concessão de blob</span><span class="sxs-lookup"><span data-stu-id="69b8c-477">`az storage blob lease`: Apply new api version for blob lease operations</span></span>
* <span data-ttu-id="69b8c-478">`az storage fs access`: Suporte a credencial do AAD no gerenciamento de controle de acesso para conta do ADLS Gen2</span><span class="sxs-lookup"><span data-stu-id="69b8c-478">`az storage fs access`: Support AAD credential in managing access control for ADLS Gen2 account</span></span>
* <span data-ttu-id="69b8c-479">`az storage share-rm create/update`: adição de --access-tier para dar suporte à camada de acesso</span><span class="sxs-lookup"><span data-stu-id="69b8c-479">`az storage share-rm create/update`: add --access-tier to support access tier</span></span>

## <a name="july-16-2020"></a><span data-ttu-id="69b8c-480">16 de julho de 2020</span><span class="sxs-lookup"><span data-stu-id="69b8c-480">July 16, 2020</span></span>

<span data-ttu-id="69b8c-481">Versão 2.9.1</span><span class="sxs-lookup"><span data-stu-id="69b8c-481">Version 2.9.1</span></span>

### <a name="aks"></a><span data-ttu-id="69b8c-482">AKS</span><span class="sxs-lookup"><span data-stu-id="69b8c-482">AKS</span></span>

* <span data-ttu-id="69b8c-483">Remove a configuração explícita de VMSS no comando de exemplo do Windows, pois ele agora é padrão</span><span class="sxs-lookup"><span data-stu-id="69b8c-483">Remove explicit setting of VMSS in Windows example command since it is now default</span></span>

### <a name="iot"></a><span data-ttu-id="69b8c-484">IoT</span><span class="sxs-lookup"><span data-stu-id="69b8c-484">IoT</span></span>

* <span data-ttu-id="69b8c-485">[ALTERAÇÃO DA FALHA] `az iot pnp`: Remove comandos de versão prévia do IoT PNP da CLI principal</span><span class="sxs-lookup"><span data-stu-id="69b8c-485">[BREAKING CHANGE] `az iot pnp`: Remove IoT PNP preview commands from core CLI</span></span>

### <a name="rest"></a><span data-ttu-id="69b8c-486">REST</span><span class="sxs-lookup"><span data-stu-id="69b8c-486">REST</span></span>

* <span data-ttu-id="69b8c-487">Correção nº14152: `az rest`: aceita URLs do ARM sem a ID de assinatura</span><span class="sxs-lookup"><span data-stu-id="69b8c-487">Fix #14152: `az rest`: Accept ARM URLs without subscription ID</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-488">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-488">Storage</span></span>

* <span data-ttu-id="69b8c-489">Correção nº 14138: torna algumas permissões opcionais</span><span class="sxs-lookup"><span data-stu-id="69b8c-489">Fix #14138: Make some permissions optional</span></span>

## <a name="july-14-2020"></a><span data-ttu-id="69b8c-490">14 de julho de 2020</span><span class="sxs-lookup"><span data-stu-id="69b8c-490">July 14, 2020</span></span>

<span data-ttu-id="69b8c-491">Versão 2.9.0</span><span class="sxs-lookup"><span data-stu-id="69b8c-491">Version 2.9.0</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-492">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-492">ACR</span></span>

* <span data-ttu-id="69b8c-493">Manipular o link do artefato de log do Registro para os logs de fluxo</span><span class="sxs-lookup"><span data-stu-id="69b8c-493">Handle log artifact link from Registry to stream logs</span></span>
* <span data-ttu-id="69b8c-494">Substituir comandos helm2</span><span class="sxs-lookup"><span data-stu-id="69b8c-494">Deprecate helm2 commands</span></span>

### <a name="aks"></a><span data-ttu-id="69b8c-495">AKS</span><span class="sxs-lookup"><span data-stu-id="69b8c-495">AKS</span></span>

* <span data-ttu-id="69b8c-496">`az aks create`: adiciona o argumento --enable-aad</span><span class="sxs-lookup"><span data-stu-id="69b8c-496">`az aks create`: add --enable-aad argument</span></span>
* <span data-ttu-id="69b8c-497">`az aks update`: adiciona o argumento --enable-aad</span><span class="sxs-lookup"><span data-stu-id="69b8c-497">`az aks update`: add --enable-aad argument</span></span>

### <a name="apim"></a><span data-ttu-id="69b8c-498">APIM</span><span class="sxs-lookup"><span data-stu-id="69b8c-498">APIM</span></span>

* <span data-ttu-id="69b8c-499">Comandos az apim api gerais adicionados</span><span class="sxs-lookup"><span data-stu-id="69b8c-499">Added general az apim api commands</span></span>

### <a name="appconfig"></a><span data-ttu-id="69b8c-500">AppConfig</span><span class="sxs-lookup"><span data-stu-id="69b8c-500">AppConfig</span></span>

* <span data-ttu-id="69b8c-501">Adicionar exemplo para usar --fields na revisão do appconfig</span><span class="sxs-lookup"><span data-stu-id="69b8c-501">Add example for using --fields in appconfig revision</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-502">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-502">AppService</span></span>

* <span data-ttu-id="69b8c-503">`az functionapp create`: Suporte para Java 11 e PowerShell 7 adicionado.</span><span class="sxs-lookup"><span data-stu-id="69b8c-503">`az functionapp create`: Added support for Java 11 and Powershell 7.</span></span> <span data-ttu-id="69b8c-504">Suporte à API de pilhas adicionado.</span><span class="sxs-lookup"><span data-stu-id="69b8c-504">Added Stacks API Support.</span></span>
* <span data-ttu-id="69b8c-505">Correção nº 14208 falha na criação de um aplicativo com vários contêineres</span><span class="sxs-lookup"><span data-stu-id="69b8c-505">Fix #14208 multi-container app creation fails</span></span>
* <span data-ttu-id="69b8c-506">Corrige az webapp create – usa pilhas de runtime embutidas em código</span><span class="sxs-lookup"><span data-stu-id="69b8c-506">Fix az webapp create - use hardcoded runtime stacks</span></span>

### <a name="arm"></a><span data-ttu-id="69b8c-507">ARM</span><span class="sxs-lookup"><span data-stu-id="69b8c-507">ARM</span></span>

* <span data-ttu-id="69b8c-508">`az resource tag`: corrige o problema de marcar recursos com o tipo de recurso `Microsoft.ContainerInstance/containerGroups`</span><span class="sxs-lookup"><span data-stu-id="69b8c-508">`az resource tag`: Fix the problem of tagging resources with resource type `Microsoft.ContainerInstance/containerGroups`</span></span>

### <a name="compute"></a><span data-ttu-id="69b8c-509">Computação</span><span class="sxs-lookup"><span data-stu-id="69b8c-509">Compute</span></span>

* <span data-ttu-id="69b8c-510">Avançar os discos de versão 2020-05-01, computação 2020-06-01</span><span class="sxs-lookup"><span data-stu-id="69b8c-510">Bump version disks 2020-05-01, compute 2020-06-01</span></span>
* <span data-ttu-id="69b8c-511">Criptografia dupla do conjunto de criptografia de disco</span><span class="sxs-lookup"><span data-stu-id="69b8c-511">Double encryption of disk encryption set</span></span>
* <span data-ttu-id="69b8c-512">`az vmss update`: dá suporte à especificação de imagem entre locatários.</span><span class="sxs-lookup"><span data-stu-id="69b8c-512">`az vmss update`: support specify cross tenant image.</span></span>
* <span data-ttu-id="69b8c-513">`az sig image-version create`: dá suporte à especificação de imagem entre locatários.</span><span class="sxs-lookup"><span data-stu-id="69b8c-513">`az sig image-version create`: support specify cross tenant image.</span></span>
* <span data-ttu-id="69b8c-514">vm/vmss create: Criptografia de cache e dados em trânsito para discos do sistema operacional/de dados e discos temporários para VM e VMSS</span><span class="sxs-lookup"><span data-stu-id="69b8c-514">vm/vmss create: Encryption of cache & data-in-transit for OS/Data disks and temp disks for VM & VMSS</span></span>
* <span data-ttu-id="69b8c-515">Adicionar operação de remoção simulada para VM e VMSS</span><span class="sxs-lookup"><span data-stu-id="69b8c-515">Add simulate-eviction operation for VM and VMSS</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="69b8c-516">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="69b8c-516">CosmosDB</span></span>

* <span data-ttu-id="69b8c-517">Recursos recentes: Autoscale, IpRules, EnableFreeTier e EnableAnalyticalStorage</span><span class="sxs-lookup"><span data-stu-id="69b8c-517">Recent features: Autoscale, IpRules, EnableFreeTier and EnableAnalyticalStorage</span></span>

### <a name="eventgrid"></a><span data-ttu-id="69b8c-518">EventGrid</span><span class="sxs-lookup"><span data-stu-id="69b8c-518">EventGrid</span></span>

* <span data-ttu-id="69b8c-519">Adicionar suporte de CLI para 2020-04-01-preview e marcar a versão prévia dos recursos com is_Preview=True</span><span class="sxs-lookup"><span data-stu-id="69b8c-519">Add CLI support for 2020-04-01-preview and mark preview features with is_Preview=True</span></span>

### <a name="find"></a><span data-ttu-id="69b8c-520">Localizar</span><span class="sxs-lookup"><span data-stu-id="69b8c-520">Find</span></span>

* <span data-ttu-id="69b8c-521">Correção nº 14094 az find Corrige consultas que falhavam quando não estavam conectadas e quando a telemetria estava desabilitada</span><span class="sxs-lookup"><span data-stu-id="69b8c-521">Fix #14094 az find Fix Queries failing when not logged in and when telemetry is disabled</span></span>

### <a name="hdinsight"></a><span data-ttu-id="69b8c-522">HDInsight</span><span class="sxs-lookup"><span data-stu-id="69b8c-522">HDInsight</span></span>

* <span data-ttu-id="69b8c-523">Adicionar dois comandos para dar suporte ao recurso de reinicialização do nó do hdinsight</span><span class="sxs-lookup"><span data-stu-id="69b8c-523">Add two commands to support hdinsight node reboot feature</span></span>

### <a name="monitor"></a><span data-ttu-id="69b8c-524">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="69b8c-524">Monitor</span></span>

* <span data-ttu-id="69b8c-525">Remover sinalizador de visualização para comandos no workspace do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="69b8c-525">Remove preview flag for commands under Log Analytics workspace</span></span>
* <span data-ttu-id="69b8c-526">`az monitor diagnostic-settings subscription`: Dar suporte às configurações de diagnóstico para a assinatura</span><span class="sxs-lookup"><span data-stu-id="69b8c-526">`az monitor diagnostic-settings subscription`: Support diagnositc settings for subscription</span></span>
* <span data-ttu-id="69b8c-527">`az monitor metrics`: dá suporte para ', ' e '|' no nome da métrica</span><span class="sxs-lookup"><span data-stu-id="69b8c-527">`az monitor metrics`: support ',' and '|' in metric name</span></span>
* <span data-ttu-id="69b8c-528">`az monitor log-analytics workspace data-export`: suporte à exportação de dados do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="69b8c-528">`az monitor log-analytics workspace data-export`: support log analytics data export</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-529">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-529">Network</span></span>

* <span data-ttu-id="69b8c-530">`az network application-gateway frontend-ip update`: Substituir o parâmetro --public-ip-address</span><span class="sxs-lookup"><span data-stu-id="69b8c-530">`az network application-gateway frontend-ip update`: Deprecating the --public-ip-address parameter</span></span>
* <span data-ttu-id="69b8c-531">Avançar azure-mgmt-network para 11.0.0</span><span class="sxs-lookup"><span data-stu-id="69b8c-531">Bump azure-mgmt-network to 11.0.0</span></span>
* <span data-ttu-id="69b8c-532">`az network express-route gateway connection`: dá suporte à configuração de roteamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-532">`az network express-route gateway connection`: support routing configuration</span></span>
* <span data-ttu-id="69b8c-533">`az network virtual-appliance`: dá suporte à solução de virtualização de rede do Azure.</span><span class="sxs-lookup"><span data-stu-id="69b8c-533">`az network virtual-appliance`: Support Azure network virtual appliance.</span></span>
* <span data-ttu-id="69b8c-534">Recurso de link privado de suporte do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="69b8c-534">Application Gateway support private link feature</span></span>

### <a name="policyinsights"></a><span data-ttu-id="69b8c-535">PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="69b8c-535">PolicyInsights</span></span>

* <span data-ttu-id="69b8c-536">`az policy state`: adiciona o comando trigger-scan para disparar avaliações de conformidade de política</span><span class="sxs-lookup"><span data-stu-id="69b8c-536">`az policy state`: add trigger-scan command to trigger policy compliance evaluations</span></span>
* <span data-ttu-id="69b8c-537">`az policy state list`: expõe versões de entidades de política em cada registro de conformidade</span><span class="sxs-lookup"><span data-stu-id="69b8c-537">`az policy state list`: expose versions of policy entities in each compliance record</span></span>

### <a name="profile"></a><span data-ttu-id="69b8c-538">Perfil</span><span class="sxs-lookup"><span data-stu-id="69b8c-538">Profile</span></span>

* <span data-ttu-id="69b8c-539">`az account get-access-token`: Mostra expiresOn para Identidade Gerenciada</span><span class="sxs-lookup"><span data-stu-id="69b8c-539">`az account get-access-token`: Show expiresOn for Managed Identity</span></span>

### <a name="rdbms"></a><span data-ttu-id="69b8c-540">RDBMS</span><span class="sxs-lookup"><span data-stu-id="69b8c-540">RDBMS</span></span>

* <span data-ttu-id="69b8c-541">Dar suporte à versão mínima do TLS</span><span class="sxs-lookup"><span data-stu-id="69b8c-541">Support Minimum TLS version</span></span>
* <span data-ttu-id="69b8c-542">Adicionar criptografia de infraestrutura para o Azure Postgres e MySQL</span><span class="sxs-lookup"><span data-stu-id="69b8c-542">Add Infrastructure Encryption for Azure Postgres and MySQL</span></span>

### <a name="security"></a><span data-ttu-id="69b8c-543">Segurança</span><span class="sxs-lookup"><span data-stu-id="69b8c-543">Security</span></span>

* <span data-ttu-id="69b8c-544">Adicionar comandos allowed_connections</span><span class="sxs-lookup"><span data-stu-id="69b8c-544">Add allowed_connections commands</span></span>
* <span data-ttu-id="69b8c-545">Adicionar comandos hardeningss da rede adaptável</span><span class="sxs-lookup"><span data-stu-id="69b8c-545">Add Adaptive network hardeningss commands</span></span>
* <span data-ttu-id="69b8c-546">Adicionar comandos adaptive_application_controls</span><span class="sxs-lookup"><span data-stu-id="69b8c-546">Add adaptive_application_controls commands</span></span>
* <span data-ttu-id="69b8c-547">Adição de az security iot-solution/ iot-alerts/iot-recommendations/iot-analytics REST à CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="69b8c-547">Addition of az security iot-solution/ iot-alerts/iot-recommendations/iot-analytics REST to Azure CLI</span></span>
* <span data-ttu-id="69b8c-548">Adicionar CLI de conformidade regulatória</span><span class="sxs-lookup"><span data-stu-id="69b8c-548">Add regulatory compliance CLI</span></span>

### <a name="signalr"></a><span data-ttu-id="69b8c-549">SignalR</span><span class="sxs-lookup"><span data-stu-id="69b8c-549">SignalR</span></span>

* <span data-ttu-id="69b8c-550">Adicionar recursos, incluindo o gerenciamento de conexões de ponto de extremidade privado, regras de rede e upstream</span><span class="sxs-lookup"><span data-stu-id="69b8c-550">Add features including managing private endpoint connections, network rules and upstream</span></span>

### <a name="sql"></a><span data-ttu-id="69b8c-551">SQL</span><span class="sxs-lookup"><span data-stu-id="69b8c-551">SQL</span></span>

* <span data-ttu-id="69b8c-552">`az sql mi create`, `az sql mi update`: adiciona o parâmetro `--tags` para dar suporte à marcação de recursos</span><span class="sxs-lookup"><span data-stu-id="69b8c-552">`az sql mi create`, `az sql mi update`: Add `--tags` parameter to support resource tagging</span></span>
* <span data-ttu-id="69b8c-553">`az sql mi failover`: dá suporte ao failover de um ponto primário ou secundário</span><span class="sxs-lookup"><span data-stu-id="69b8c-553">`az sql mi failover`: Support failover from primary or secondary point</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-554">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-554">Storage</span></span>

* <span data-ttu-id="69b8c-555">`az storage account create/update`: adiciona --allow-blob-public-access para permitir ou não permitir acesso público para blob e contêineres</span><span class="sxs-lookup"><span data-stu-id="69b8c-555">`az storage account create/update`: Add --allow-blob-public-access to allow or disallow public access for blob and containers</span></span>
* <span data-ttu-id="69b8c-556">`az storage account create/update`: adiciona `--min-tls-version` para dar suporte à definição da versão mínima do TLS a ser permitida em solicitações de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="69b8c-556">`az storage account create/update`: Add `--min-tls-version` to support setting the minimum TLS version to be permitted on requests to storage.</span></span>
* <span data-ttu-id="69b8c-557">Remover credencial de token de check-in</span><span class="sxs-lookup"><span data-stu-id="69b8c-557">Remove check in token credential</span></span>
* <span data-ttu-id="69b8c-558">Corrigir o nome da conta de armazenamento em exemplos</span><span class="sxs-lookup"><span data-stu-id="69b8c-558">Fix the storage account name in examples</span></span>

### <a name="webapp"></a><span data-ttu-id="69b8c-559">Webapp</span><span class="sxs-lookup"><span data-stu-id="69b8c-559">Webapp</span></span>

* <span data-ttu-id="69b8c-560">Bugfix: az webapp log deployment show – retorna logs de implantação em vez de metadados de log</span><span class="sxs-lookup"><span data-stu-id="69b8c-560">Bugfix: az webapp log deployment show - return deployment logs instead of log metadata</span></span>
* <span data-ttu-id="69b8c-561">Bugfix: az webapp vnet-integration add – corrige o tratamento de erro se o nome da VNet é inadequado, dá suporte à ID do recurso da vnet</span><span class="sxs-lookup"><span data-stu-id="69b8c-561">Bugfix: az webapp vnet-integration add - fix error handling if bad vnet name, support vnet resource ID</span></span>

## <a name="june-23-2020"></a><span data-ttu-id="69b8c-562">23 de junho de 2020</span><span class="sxs-lookup"><span data-stu-id="69b8c-562">June 23, 2020</span></span>

<span data-ttu-id="69b8c-563">Versão 2.8.0</span><span class="sxs-lookup"><span data-stu-id="69b8c-563">Version 2.8.0</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-564">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-564">ACR</span></span>

* <span data-ttu-id="69b8c-565">Adicionar suporte para desabilitar roteamento/ponto de extremidade da região</span><span class="sxs-lookup"><span data-stu-id="69b8c-565">Add support for region endpoint disable / routing disable</span></span>
* <span data-ttu-id="69b8c-566">[ALTERAÇÃO DA FALHA] `az acr login --expose-token` não aceita nome de usuário e senha</span><span class="sxs-lookup"><span data-stu-id="69b8c-566">[BREAKING CHANGE] `az acr login --expose-token` does not accept username and password</span></span>

### <a name="acs"></a><span data-ttu-id="69b8c-567">ACS</span><span class="sxs-lookup"><span data-stu-id="69b8c-567">ACS</span></span>

* <span data-ttu-id="69b8c-568">Remover o cluster privado e a API 2019-10-27-preview</span><span class="sxs-lookup"><span data-stu-id="69b8c-568">Remove private cluster and 2019-10-27-preview API</span></span>

### <a name="aks"></a><span data-ttu-id="69b8c-569">AKS</span><span class="sxs-lookup"><span data-stu-id="69b8c-569">AKS</span></span>

* <span data-ttu-id="69b8c-570">Suporte a --yes para az aks upgrade</span><span class="sxs-lookup"><span data-stu-id="69b8c-570">Support --yes for az aks upgrade</span></span>
* <span data-ttu-id="69b8c-571">Reverter "alteração da sku de vm padrão para Standard_D2s_v3 (#13541)"</span><span class="sxs-lookup"><span data-stu-id="69b8c-571">Revert "change default vm sku to Standard_D2s_v3 (#13541)"</span></span>
* <span data-ttu-id="69b8c-572">Adicionar "az aks update --uptime-sla"</span><span class="sxs-lookup"><span data-stu-id="69b8c-572">Add "az aks update --uptime-sla"</span></span>
* <span data-ttu-id="69b8c-573">Corrigir erro de digitação no comando az aks update</span><span class="sxs-lookup"><span data-stu-id="69b8c-573">Fix typo in az aks update command</span></span>
* <span data-ttu-id="69b8c-574">Alteração para dar suporte ao pool de agentes do nó 0 e bloquear a escala manual do pool habilitado para CAS</span><span class="sxs-lookup"><span data-stu-id="69b8c-574">Change to support 0 node agent pool and block manual scale for CAS enabled pool</span></span>
* <span data-ttu-id="69b8c-575">Corrigir erro de digitação em VirtualMachineScaleSets e atualizar referências a versões do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="69b8c-575">Fix typo on VirtualMachineScaleSets and update references to Kubernetes versions</span></span>

### <a name="ams"></a><span data-ttu-id="69b8c-576">AMS</span><span class="sxs-lookup"><span data-stu-id="69b8c-576">AMS</span></span>

* <span data-ttu-id="69b8c-577">ALTERAR o texto da ajuda do parâmetro "--expiry".</span><span class="sxs-lookup"><span data-stu-id="69b8c-577">CHANGE help text for "--expiry" parameter.</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-578">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-578">AppService</span></span>

* <span data-ttu-id="69b8c-579">`az webapp log deployment show`: mostrar o log de implantação mais recente ou os logs de uma implantação específica se a ID da implantação for especificada</span><span class="sxs-lookup"><span data-stu-id="69b8c-579">`az webapp log deployment show`: Show the latest deployment log, or the deployment logs of a specific deployment if deployment-id is specified</span></span>
* <span data-ttu-id="69b8c-580">`az webapp log deployment list`: lista de logs de implantação disponíveis</span><span class="sxs-lookup"><span data-stu-id="69b8c-580">`az webapp log deployment list`: List of deployment logs available</span></span>
* <span data-ttu-id="69b8c-581">Correção: erro de superfície quando um nome de webapp inválido é fornecido</span><span class="sxs-lookup"><span data-stu-id="69b8c-581">Fix: Surface error when invalid webapp name provided</span></span>
* <span data-ttu-id="69b8c-582">Correção #13261: az webapp list-runtimes usa a lista estática até que a nova API de Pilhas Disponíveis esteja disponível</span><span class="sxs-lookup"><span data-stu-id="69b8c-582">Fix #13261 az webapp list-runtimes use static list until new Available Stacks API is available</span></span>
* <span data-ttu-id="69b8c-583">`az appservice ase create`: correção na criação do problema #13361</span><span class="sxs-lookup"><span data-stu-id="69b8c-583">`az appservice ase create`: Fix create issue #13361</span></span>
* <span data-ttu-id="69b8c-584">`az appservice ase list-addresses`: correção na alteração do SDK #13140.</span><span class="sxs-lookup"><span data-stu-id="69b8c-584">`az appservice ase list-addresses`: Fix change of SDK #13140.</span></span>
* <span data-ttu-id="69b8c-585">Correção da criação de webapp/slot para Contêineres do Windows</span><span class="sxs-lookup"><span data-stu-id="69b8c-585">Fix webapp/slot creation for Windows Containers</span></span>
* <span data-ttu-id="69b8c-586">`az webapp auth update`: adicionar parâmetro opcional para atualizar a versão do runtime</span><span class="sxs-lookup"><span data-stu-id="69b8c-586">`az webapp auth update`: Add optional parameter to update runtime-version</span></span>
* <span data-ttu-id="69b8c-587">Suporte para listar, excluir, aprovar e rejeitar conexão de ponto de extremidade privado para webapp na CLI</span><span class="sxs-lookup"><span data-stu-id="69b8c-587">Support list, delete, approve and reject private endpoint connection for webapp in CLI</span></span>
* <span data-ttu-id="69b8c-588">Correção #13888: adicionar suporte para WebApps Estáticos: comandos get, list, create</span><span class="sxs-lookup"><span data-stu-id="69b8c-588">Fix #13888 : Add support for Static WebApps: get, list, create commands</span></span>
* <span data-ttu-id="69b8c-589">Mensagens de erro aprimoradas para Conexão de Túnel SSH</span><span class="sxs-lookup"><span data-stu-id="69b8c-589">Improved error messages for SSH Tunnel Connection</span></span>

### <a name="arm"></a><span data-ttu-id="69b8c-590">ARM</span><span class="sxs-lookup"><span data-stu-id="69b8c-590">ARM</span></span>

* <span data-ttu-id="69b8c-591">`az tag`: adicionar exemplos para -h</span><span class="sxs-lookup"><span data-stu-id="69b8c-591">`az tag`: Add examples for -h</span></span>
* <span data-ttu-id="69b8c-592">`az deployment group/sub what-if`: adicionar parâmetro --exclude-change-types/-x.</span><span class="sxs-lookup"><span data-stu-id="69b8c-592">`az deployment group/sub what-if`: Add --exclude-change-types/-x parameter.</span></span>
* <span data-ttu-id="69b8c-593">`az deployment group/sub/mg/tenant create`: adicionar parâmetro --what-if-exclude-change-types/-x.</span><span class="sxs-lookup"><span data-stu-id="69b8c-593">`az deployment group/sub/mg/tenant create`: Add --what-if-exclude-change-types/-x parameter.</span></span>
* <span data-ttu-id="69b8c-594">`az deployment group/sub/mg/tenant validate`: mostrar mensagens de erro em um formato melhor.</span><span class="sxs-lookup"><span data-stu-id="69b8c-594">`az deployment group/sub/mg/tenant validate`: Show error messages in a better format.</span></span>
* <span data-ttu-id="69b8c-595">`az group export`: adicionar novos parâmetros `--skip-resource-name-params` e `--skip-all-params` para dar suporte para ignorar parametrização</span><span class="sxs-lookup"><span data-stu-id="69b8c-595">`az group export`: Add new parameters `--skip-resource-name-params` and `--skip-all-params` to support skip parameterization</span></span>
* <span data-ttu-id="69b8c-596">Adicionar az feature unregister api</span><span class="sxs-lookup"><span data-stu-id="69b8c-596">Add az feature unregister api</span></span>

### <a name="aro"></a><span data-ttu-id="69b8c-597">ARO</span><span class="sxs-lookup"><span data-stu-id="69b8c-597">ARO</span></span>

* <span data-ttu-id="69b8c-598">Adicionar Public e Private aos parâmetros para obter ajuda com a visibilidade de entrada/apiserver</span><span class="sxs-lookup"><span data-stu-id="69b8c-598">Add Public, Private to params for help with ingress/apiserver visibility</span></span>

### <a name="batch"></a><span data-ttu-id="69b8c-599">Lote</span><span class="sxs-lookup"><span data-stu-id="69b8c-599">Batch</span></span>

* <span data-ttu-id="69b8c-600">`az batch account create`: adicionar novo parâmetro `--public-network-access`</span><span class="sxs-lookup"><span data-stu-id="69b8c-600">`az batch account create`: Add new parameter `--public-network-access`</span></span>
* <span data-ttu-id="69b8c-601">`az batch account create`: adicionar novo parâmetro `--identity-type`</span><span class="sxs-lookup"><span data-stu-id="69b8c-601">`az batch account create`: Add new parameter `--identity-type`</span></span>
* <span data-ttu-id="69b8c-602">`az batch account set`: adicionar novo parâmetro `--identity-type`</span><span class="sxs-lookup"><span data-stu-id="69b8c-602">`az batch account set`: Add new parameter `--identity-type`</span></span>
* <span data-ttu-id="69b8c-603">[ALTERAÇÃO SIGNIFICATIVA] az batch pool create: ao criar um pool usando uma imagem personalizada, a propriedade --image agora pode se referir apenas a uma imagem da Galeria de Imagens Compartilhadas.</span><span class="sxs-lookup"><span data-stu-id="69b8c-603">[BREAKING CHANGE] az batch pool create: When creating a pool using a custom image, the --image property of can now only refer to a Shared Image Gallery image.</span></span>
* <span data-ttu-id="69b8c-604">[ALTERAÇÃO SIGNIFICATIVA] az batch pool create: ao criar um pool com a opção --json-file e especificar uma networkConfiguration, a propriedade publicIPs foi movida para uma nova propriedade publicIPAddressConfiguration.</span><span class="sxs-lookup"><span data-stu-id="69b8c-604">[BREAKING CHANGE] az batch pool create: When creating a pool with --json-file option and specifying a networkConfiguration, the publicIPs property has moved in to a new property publicIPAddressConfiguration.</span></span> <span data-ttu-id="69b8c-605">Essa nova propriedade também dá suporte a uma nova propriedade ipAddressProvisioningType, que especifica como o pool deve alocar os IPs, e a uma propriedade publicIPs, que permite a configuração de uma lista de recursos de PublicIP a serem usados caso ipAddressProvisioningType seja definido como UserManaged</span><span class="sxs-lookup"><span data-stu-id="69b8c-605">This new property also supports a new ipAddressProvisioningType property which specifies how the pool should allocate IP's and a publicIPs property which allows for configuration of a list of PublicIP resources to use in the case ipAddressProvisioningType is set to UserManaged</span></span>
* <span data-ttu-id="69b8c-606">`az network private-link-resource`: adicionar suporte para o recurso Microsoft.Batch batchAccount</span><span class="sxs-lookup"><span data-stu-id="69b8c-606">`az network private-link-resource`: Add support for the Microsoft.Batch batchAccount resource</span></span>
* <span data-ttu-id="69b8c-607">`az network private-endpoint-connection`: adicionar suporte para o recurso Microsoft.Batch batchAccount</span><span class="sxs-lookup"><span data-stu-id="69b8c-607">`az network private-endpoint-connection`: Add support for the Microsoft.Batch batchAccount resource</span></span>

### <a name="cdn"></a><span data-ttu-id="69b8c-608">CDN</span><span class="sxs-lookup"><span data-stu-id="69b8c-608">CDN</span></span>

* <span data-ttu-id="69b8c-609">`az cdn custom-domain enable-https`: adicionar suporte para BYOC.</span><span class="sxs-lookup"><span data-stu-id="69b8c-609">`az cdn custom-domain enable-https`: Add BYOC support.</span></span>
* <span data-ttu-id="69b8c-610">`az cdn custom-domain enable-https`: corrigir a habilitação de HTTPS personalizado com certificados gerenciados da CDN para os SKUs Standard_Verizon e Standard_Microsoft.</span><span class="sxs-lookup"><span data-stu-id="69b8c-610">`az cdn custom-domain enable-https`: Fix enabling custom HTTPS with CDN managed certificates for Standard_Verizon and Standard_Microsoft SKUs.</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="69b8c-611">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="69b8c-611">Cognitive Services</span></span>

* <span data-ttu-id="69b8c-612">[ALTERAÇÃO DA FALHA] `az cognitiveservices account` agora, há uma estrutura unificada para todos os comandos.</span><span class="sxs-lookup"><span data-stu-id="69b8c-612">[BREAKING CHANGE] `az cognitiveservices account` now have a unified structure for all commands.</span></span>
* <span data-ttu-id="69b8c-613">`az cognitiveservices account identity`: adicionar gerenciamento de identidades para os Serviços Cognitivos.</span><span class="sxs-lookup"><span data-stu-id="69b8c-613">`az cognitiveservices account identity`: Add identity management for Cognitive Services.</span></span>

### <a name="compute"></a><span data-ttu-id="69b8c-614">Computação</span><span class="sxs-lookup"><span data-stu-id="69b8c-614">Compute</span></span>

* <span data-ttu-id="69b8c-615">`az image builder`: atualização da versão da API para 2020-02-14</span><span class="sxs-lookup"><span data-stu-id="69b8c-615">`az image builder`: Upgrade API version to 2020-02-14</span></span>
* <span data-ttu-id="69b8c-616">`az image builder create`: adicionar `--identity` para dar suporte à configuração de identidade</span><span class="sxs-lookup"><span data-stu-id="69b8c-616">`az image builder create`: Add `--identity` to support identity configuration</span></span>
* <span data-ttu-id="69b8c-617">`az image builder customizer add`: suporte para o personalizador de atualização do Windows</span><span class="sxs-lookup"><span data-stu-id="69b8c-617">`az image builder customizer add`: Support Windows update customizer</span></span>
* <span data-ttu-id="69b8c-618">Novo comando `az image builder cancel`</span><span class="sxs-lookup"><span data-stu-id="69b8c-618">New command `az image builder cancel`</span></span>
* <span data-ttu-id="69b8c-619">Mostrar um aviso quando um usuário implanta um VMSS fixado a uma versão de uma imagem específica em vez da mais recente</span><span class="sxs-lookup"><span data-stu-id="69b8c-619">Show a warning when a user deploys a VMSS pinned to a specific image version rather than latest</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="69b8c-620">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="69b8c-620">Cosmos DB</span></span>

* <span data-ttu-id="69b8c-621">`az cosmosdb`: adicionar o comando exists ao banco de dados e aos grupos de contêineres</span><span class="sxs-lookup"><span data-stu-id="69b8c-621">`az cosmosdb`: Add exists command to database and container groups</span></span>
* <span data-ttu-id="69b8c-622">Permitir a criação de coleções fixas</span><span class="sxs-lookup"><span data-stu-id="69b8c-622">Allow creating fixed collections</span></span>

### <a name="eventhub"></a><span data-ttu-id="69b8c-623">EventHub</span><span class="sxs-lookup"><span data-stu-id="69b8c-623">EventHub</span></span>

* <span data-ttu-id="69b8c-624">`az eventhubs namespace create`: adicionar parâmetros de identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="69b8c-624">`az eventhubs namespace create` : Add managed identity parameters</span></span>

### <a name="extension"></a><span data-ttu-id="69b8c-625">Extensão</span><span class="sxs-lookup"><span data-stu-id="69b8c-625">Extension</span></span>

* <span data-ttu-id="69b8c-626">Adicionar --version para dar suporte à instalação de uma versão específica</span><span class="sxs-lookup"><span data-stu-id="69b8c-626">Add --version to support to install from a specific version</span></span>
* <span data-ttu-id="69b8c-627">Habilitar as extensões da CLI a incluírem pacotes no namespace 'azure'</span><span class="sxs-lookup"><span data-stu-id="69b8c-627">Enable CLI extensions to include packages in the 'azure' namespace</span></span>

### <a name="iot-hub"></a><span data-ttu-id="69b8c-628">Hub IoT</span><span class="sxs-lookup"><span data-stu-id="69b8c-628">Iot Hub</span></span>

* <span data-ttu-id="69b8c-629">[ALTERAÇÃO SIGNIFICATIVA] az iot hub job: remover comandos de trabalho preteridos</span><span class="sxs-lookup"><span data-stu-id="69b8c-629">[BREAKING CHANGE] az iot hub job: Remove deprecated job commands</span></span>

### <a name="keyvault"></a><span data-ttu-id="69b8c-630">KeyVault</span><span class="sxs-lookup"><span data-stu-id="69b8c-630">KeyVault</span></span>

* <span data-ttu-id="69b8c-631">`az keyvault key import`: dá suporte à importação de cadeias de caracteres por meio de dois novos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="69b8c-631">`az keyvault key import`: Supports importing from strings via two new parameters.</span></span>
* <span data-ttu-id="69b8c-632">Suporte à criptografia e descriptografia de cadeias de caracteres/bytes com chaves armazenadas</span><span class="sxs-lookup"><span data-stu-id="69b8c-632">Support string/bytes encryption and decryption with stored keys</span></span>

### <a name="monitor"></a><span data-ttu-id="69b8c-633">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="69b8c-633">Monitor</span></span>

* <span data-ttu-id="69b8c-634">Suporte para não aguardar a criação do cluster</span><span class="sxs-lookup"><span data-stu-id="69b8c-634">Support no wait for cluster creation</span></span>
* <span data-ttu-id="69b8c-635">`az monitor log-analytics workspace saved-search`: suporte para novos comandos para a pesquisa salva</span><span class="sxs-lookup"><span data-stu-id="69b8c-635">`az monitor log-analytics workspace saved-search`: Support new commands for saved search</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-636">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-636">Network</span></span>

* <span data-ttu-id="69b8c-637">`az network application-gateway address-pool update`: refinar a mensagem de ajuda e adicionar exemplos.</span><span class="sxs-lookup"><span data-stu-id="69b8c-637">`az network application-gateway address-pool update`: Refine help message and add examples.</span></span>
* <span data-ttu-id="69b8c-638">`az network vnet create`: suporte para o argumento --nsg</span><span class="sxs-lookup"><span data-stu-id="69b8c-638">`az network vnet create`: Support --nsg argument</span></span>
* <span data-ttu-id="69b8c-639">`az network lb address-pool`: suporte para criar o pool de back-end de lb com endereço de back-end.</span><span class="sxs-lookup"><span data-stu-id="69b8c-639">`az network lb address-pool`: Support create lb backend pool with backend address.</span></span>
* <span data-ttu-id="69b8c-640">`az network application-gateway address-pool`: correção para o argumento --add</span><span class="sxs-lookup"><span data-stu-id="69b8c-640">`az network application-gateway address-pool`: Fix for --add argument</span></span>

### <a name="rbac"></a><span data-ttu-id="69b8c-641">RBAC</span><span class="sxs-lookup"><span data-stu-id="69b8c-641">RBAC</span></span>

* <span data-ttu-id="69b8c-642">`az ad sp create-for-rabc`: suporte para nome com espaço, barra e barra invertida</span><span class="sxs-lookup"><span data-stu-id="69b8c-642">`az ad sp create-for-rabc`: Support name with space, slash and back slash</span></span>
* <span data-ttu-id="69b8c-643">`az ad sp create-for-rbac`: refinar mensagem de erro quando o usuário especifica um escopo inválido</span><span class="sxs-lookup"><span data-stu-id="69b8c-643">`az ad sp create-for-rbac`: Refine error message when user specify an invalid scope</span></span>

### <a name="security"></a><span data-ttu-id="69b8c-644">Segurança</span><span class="sxs-lookup"><span data-stu-id="69b8c-644">Security</span></span>

* <span data-ttu-id="69b8c-645">Adicionar comandos de avaliação de segurança</span><span class="sxs-lookup"><span data-stu-id="69b8c-645">Add security assessment commands</span></span>

### <a name="sql"></a><span data-ttu-id="69b8c-646">SQL</span><span class="sxs-lookup"><span data-stu-id="69b8c-646">SQL</span></span>

* <span data-ttu-id="69b8c-647">`az sql db ltr-policy/ltr-backup`: atualizar/mostrar política de retenção de longo prazo, mostrar/excluir backups de retenção de longo prazo, restaurar backup de retenção de longo prazo</span><span class="sxs-lookup"><span data-stu-id="69b8c-647">`az sql db ltr-policy/ltr-backup`: update/show long term retention policy, show/delete long term retention backups, restore long term retention backup</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-648">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-648">Storage</span></span>

* <span data-ttu-id="69b8c-649">Corrigir problema de autenticação para dar suporte a get token para --subscription</span><span class="sxs-lookup"><span data-stu-id="69b8c-649">Fix authentication issue to support get token for --subscription</span></span>
* <span data-ttu-id="69b8c-650">`az storage remove`: correção do problema #13459 para gerar exceção para a falha da operação</span><span class="sxs-lookup"><span data-stu-id="69b8c-650">`az storage remove`: Fix issue #13459 to raise exception for operation failure</span></span>
* <span data-ttu-id="69b8c-651">Correção dos problemas #13012, #13632 e #13657 para remover argumentos não utilizados para comandos relacionados à geração de SAS</span><span class="sxs-lookup"><span data-stu-id="69b8c-651">Fix issues #13012, #13632 and #13657 to remove unused arguments for generate-sas related commands</span></span>
* <span data-ttu-id="69b8c-652">`az storage logging update`: adicionar verificação da versão de log</span><span class="sxs-lookup"><span data-stu-id="69b8c-652">`az storage logging update`: Add check for logging version</span></span>
* <span data-ttu-id="69b8c-653">`az storage blob show`: adicionar mais propriedades para o blob com o SDK da faixa 2</span><span class="sxs-lookup"><span data-stu-id="69b8c-653">`az storage blob show`: Add more properties for blob with track 2 SDK</span></span>
* <span data-ttu-id="69b8c-654">Correção #13708: refinar a mensagem de aviso para a credencial</span><span class="sxs-lookup"><span data-stu-id="69b8c-654">Fix #13708: Refine warning message for credential</span></span>
* <span data-ttu-id="69b8c-655">`az storage share-rm create/update`: adicionar suporte para protocolo NFS e squash raiz</span><span class="sxs-lookup"><span data-stu-id="69b8c-655">`az storage share-rm create/update`: Add NFS protocol and root squash support</span></span>
* <span data-ttu-id="69b8c-656">`az storage account create`: adicionar suporte para criptografia dupla</span><span class="sxs-lookup"><span data-stu-id="69b8c-656">`az storage account create`: Add support for double encryption</span></span>
* <span data-ttu-id="69b8c-657">[ALTERAÇÃO DA FALHA] `az storage blob/container/file/share/table/queue generate-sas`: tornar --expiry e --permissions obrigatórios</span><span class="sxs-lookup"><span data-stu-id="69b8c-657">[BREAKING CHANGE] `az storage blob/container/file/share/table/queue generate-sas`: make --expiry and --permissions required</span></span>
* <span data-ttu-id="69b8c-658">`az storage blob set-tier`: migrar para a Faixa 2 para dar suporte à definição da prioridade de reidratação</span><span class="sxs-lookup"><span data-stu-id="69b8c-658">`az storage blob set-tier`: Migrate to Track 2 to support setting rehydrate priority</span></span>

## <a name="june-02-2020"></a><span data-ttu-id="69b8c-659">02 de Junho de 2020</span><span class="sxs-lookup"><span data-stu-id="69b8c-659">June 02, 2020</span></span>

<span data-ttu-id="69b8c-660">Versão 2.7.0</span><span class="sxs-lookup"><span data-stu-id="69b8c-660">Version 2.7.0</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-661">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-661">ACR</span></span>

* <span data-ttu-id="69b8c-662">Correção de um erro de digitação em uma mensagem de erro de criação de token</span><span class="sxs-lookup"><span data-stu-id="69b8c-662">Fix a typo in an error message of token creation</span></span>

### <a name="aks"></a><span data-ttu-id="69b8c-663">AKS</span><span class="sxs-lookup"><span data-stu-id="69b8c-663">AKS</span></span>

* <span data-ttu-id="69b8c-664">Alteração da sku de vm padrão para Standard_D2s_v3</span><span class="sxs-lookup"><span data-stu-id="69b8c-664">Change default vm sku to Standard_D2s_v3</span></span>
* <span data-ttu-id="69b8c-665">Correção da criação de atribuição de função para sub-rede personalizada MSI cluster Plus</span><span class="sxs-lookup"><span data-stu-id="69b8c-665">Fix creating role assignment for MSI clsuter plus custom subnet</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-666">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-666">AppService</span></span>

* <span data-ttu-id="69b8c-667">A correção #12739 az appservice list-locations retorna alguns locais inválidos</span><span class="sxs-lookup"><span data-stu-id="69b8c-667">Fix #12739 az appservice list-locations returns some invalid locations</span></span>

### <a name="arm"></a><span data-ttu-id="69b8c-668">ARM</span><span class="sxs-lookup"><span data-stu-id="69b8c-668">ARM</span></span>

* <span data-ttu-id="69b8c-669">`az deployment`: Correção do problema #13159 de mensagem incorreta do JSON após a remoção de comentários e a compactação</span><span class="sxs-lookup"><span data-stu-id="69b8c-669">`az deployment`: Fix issue #13159 of incorrect message of JSON after removing comments and compressing</span></span>
* <span data-ttu-id="69b8c-670">`az resource tag`: Correção do problema #13255 de marcação de recursos com o tipo de recurso `Microsoft.ContainerRegistry/registries/webhooks`</span><span class="sxs-lookup"><span data-stu-id="69b8c-670">`az resource tag`: Fix issue #13255 of tagging resources with resource type `Microsoft.ContainerRegistry/registries/webhooks`</span></span>
* <span data-ttu-id="69b8c-671">Melhoria dos exemplos do módulo de recursos</span><span class="sxs-lookup"><span data-stu-id="69b8c-671">Improve the examples for the resource module</span></span>

### <a name="aro"></a><span data-ttu-id="69b8c-672">ARO</span><span class="sxs-lookup"><span data-stu-id="69b8c-672">ARO</span></span>

* <span data-ttu-id="69b8c-673">Alteração do CLIError para corrigir o sinalizador para --worker-vm-disk-size-gb</span><span class="sxs-lookup"><span data-stu-id="69b8c-673">Change CLIError to correct flag for --worker-vm-disk-size-gb</span></span>

### <a name="eventhub"></a><span data-ttu-id="69b8c-674">EventHub</span><span class="sxs-lookup"><span data-stu-id="69b8c-674">EventHub</span></span>

* <span data-ttu-id="69b8c-675">Correção do problema #12406 Argumento --capture-interval não atualiza o "intervalInSeconds"</span><span class="sxs-lookup"><span data-stu-id="69b8c-675">Fix for issue #12406 Argument --capture-interval does not update the "intervalInSeconds"</span></span>

### <a name="hdinsight"></a><span data-ttu-id="69b8c-676">HDInsight</span><span class="sxs-lookup"><span data-stu-id="69b8c-676">HDInsight</span></span>

* <span data-ttu-id="69b8c-677">Alteração de get_json_object para shell_safe_json_parse</span><span class="sxs-lookup"><span data-stu-id="69b8c-677">Change get_json_object to shell_safe_json_parse</span></span>

### <a name="monitor"></a><span data-ttu-id="69b8c-678">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="69b8c-678">Monitor</span></span>

* <span data-ttu-id="69b8c-679">`az monitor metrics alert`: ajuste de várias mensagens de ajuda</span><span class="sxs-lookup"><span data-stu-id="69b8c-679">`az monitor metrics alert`: refine several help messages</span></span>
* <span data-ttu-id="69b8c-680">`az monitor diagnostic-settings create`: suporte ao argumento --export-to-resource-specific</span><span class="sxs-lookup"><span data-stu-id="69b8c-680">`az monitor diagnostic-settings create`: support --export-to-resource-specific argument</span></span>
* <span data-ttu-id="69b8c-681">Suporte para recuperar o workspace de LA</span><span class="sxs-lookup"><span data-stu-id="69b8c-681">Support LA workspace recover</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-682">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-682">Network</span></span>

* <span data-ttu-id="69b8c-683">`az network dns zone`: suporte – caractere</span><span class="sxs-lookup"><span data-stu-id="69b8c-683">`az network dns zone`: support - character</span></span>
* <span data-ttu-id="69b8c-684">`az network vpn-connection ipsec-policy`: alteração do --sa-lifetime e do --sa-max-size para valores maiores no exemplo</span><span class="sxs-lookup"><span data-stu-id="69b8c-684">`az network vpn-connection ipsec-policy`: change the --sa-lifetime and --sa-max-size to larger values in example</span></span>
* <span data-ttu-id="69b8c-685">Aumento da rede para 2020-04-01</span><span class="sxs-lookup"><span data-stu-id="69b8c-685">Bump network to 2020-04-01</span></span>
* <span data-ttu-id="69b8c-686">`az network private-endpoint-connection`: suporte à grade de eventos</span><span class="sxs-lookup"><span data-stu-id="69b8c-686">`az network private-endpoint-connection`: support event grid</span></span>
* <span data-ttu-id="69b8c-687">`az network express-route list-route-tables`: correção do bug que faz não ser possível listar rotas como tabela</span><span class="sxs-lookup"><span data-stu-id="69b8c-687">`az network express-route list-route-tables`: fix bug that cannot list routes as table</span></span>

### <a name="packaging"></a><span data-ttu-id="69b8c-688">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-688">Packaging</span></span>

* <span data-ttu-id="69b8c-689">Adição do Pacote Focal do Ubuntu</span><span class="sxs-lookup"><span data-stu-id="69b8c-689">Add Ubuntu Focal Package</span></span>

### <a name="rbac"></a><span data-ttu-id="69b8c-690">RBAC</span><span class="sxs-lookup"><span data-stu-id="69b8c-690">RBAC</span></span>

* <span data-ttu-id="69b8c-691">`az ad sp credential reset`: modificar a geração de credenciais para evitar caracteres especiais problemáticos</span><span class="sxs-lookup"><span data-stu-id="69b8c-691">`az ad sp credential reset`: modify credential generation to avoid troublesome special characters</span></span>

### <a name="redis"></a><span data-ttu-id="69b8c-692">Redis</span><span class="sxs-lookup"><span data-stu-id="69b8c-692">Redis</span></span>

* <span data-ttu-id="69b8c-693">Correção #13529: alteração da documentação do parâmetro enable_non_ssl_port</span><span class="sxs-lookup"><span data-stu-id="69b8c-693">Fix #13529: Change documentation of parameter enable_non_ssl_port</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-694">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-694">Storage</span></span>

* <span data-ttu-id="69b8c-695">`az storage copy`: adição do parâmetro `--follow-symlinks` para dar suporte ao symlinks</span><span class="sxs-lookup"><span data-stu-id="69b8c-695">`az storage copy`: Add parameter `--follow-symlinks` to support symlinks</span></span>
* <span data-ttu-id="69b8c-696">Habilitar contexto local para a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-696">Enable local context for storage account</span></span>
* <span data-ttu-id="69b8c-697">`az storage logging`: Correção do problema #11969 para ajustar a mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="69b8c-697">`az storage logging`: Fix issue #11969 to refine error message</span></span>

## <a name="may-19-2020"></a><span data-ttu-id="69b8c-698">19 de maio de 2020</span><span class="sxs-lookup"><span data-stu-id="69b8c-698">May 19, 2020</span></span>

<span data-ttu-id="69b8c-699">Versão 2.6.0</span><span class="sxs-lookup"><span data-stu-id="69b8c-699">Version 2.6.0</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-700">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-700">ACR</span></span>

* <span data-ttu-id="69b8c-701">Adiciona tempo limite padrão de 5 minutos para solicitações ao ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-701">Add default timeout of 5 minutes for any requests to ACR</span></span>
* <span data-ttu-id="69b8c-702">Suporte para desabilitar o acesso à redes públicas</span><span class="sxs-lookup"><span data-stu-id="69b8c-702">Support disable public network access</span></span>
* <span data-ttu-id="69b8c-703">`az acr token create`: expõe o argumento --days</span><span class="sxs-lookup"><span data-stu-id="69b8c-703">`az acr token create`: expose --days argument</span></span>
* <span data-ttu-id="69b8c-704">`az acr import`: aceita valores do argumento --source que contêm logon no nome do servidor por meio da correção final do cliente</span><span class="sxs-lookup"><span data-stu-id="69b8c-704">`az acr import`: accept --source argument values which contain login in server name through client end correction</span></span>

### <a name="acs"></a><span data-ttu-id="69b8c-705">ACS</span><span class="sxs-lookup"><span data-stu-id="69b8c-705">ACS</span></span>

* <span data-ttu-id="69b8c-706">Correção de bug: remover limpeza de campos para campos que não existem mais</span><span class="sxs-lookup"><span data-stu-id="69b8c-706">Bug fix: remove fields cleanup for fields that no longer exist</span></span>

### <a name="aks"></a><span data-ttu-id="69b8c-707">AKS</span><span class="sxs-lookup"><span data-stu-id="69b8c-707">AKS</span></span>

* <span data-ttu-id="69b8c-708">Atualiza o tempo de atividade do contexto de ajuda de comando do SLA</span><span class="sxs-lookup"><span data-stu-id="69b8c-708">Update uptime-sla command help context</span></span>
* <span data-ttu-id="69b8c-709">Remove a verificação do intervalo para a atualização da contagem de minutos do dimensionador automático</span><span class="sxs-lookup"><span data-stu-id="69b8c-709">Remove range check for updating min count for autoscaler</span></span>
* <span data-ttu-id="69b8c-710">Corrige o problema que fazia com que a CLI falhasse quando o usuário especificava apenas a senha do Windows</span><span class="sxs-lookup"><span data-stu-id="69b8c-710">Fix that cli doe not fail when user only specifies Windows password</span></span>

### <a name="ams"></a><span data-ttu-id="69b8c-711">AMS</span><span class="sxs-lookup"><span data-stu-id="69b8c-711">AMS</span></span>

* <span data-ttu-id="69b8c-712">`az ams transform create`: Adiciona a capacidade de criar uma transformação com um FaceDetector predefinido</span><span class="sxs-lookup"><span data-stu-id="69b8c-712">`az ams transform create`: Add ability to create a transform with a FaceDetector preset</span></span>
* <span data-ttu-id="69b8c-713">`az ams content-key-policy create`: Adiciona a capacidade de criar uma política de chave de conteúdo do FairPlay com uma configuração de aluguel offline</span><span class="sxs-lookup"><span data-stu-id="69b8c-713">`az ams content-key-policy create` : Add ability to create a FairPlay content key policy with an offline rental configuration</span></span>

### <a name="appconfig"></a><span data-ttu-id="69b8c-714">AppConfig</span><span class="sxs-lookup"><span data-stu-id="69b8c-714">AppConfig</span></span>

* <span data-ttu-id="69b8c-715">Correção de bug para valores de chave da lista com campos</span><span class="sxs-lookup"><span data-stu-id="69b8c-715">Bug fix for list key values with fields</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-716">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-716">AppService</span></span>

* <span data-ttu-id="69b8c-717">`az functionapp create`: AzureWebJobsDashboard será definido somente se AppInsights estiver desabilitado</span><span class="sxs-lookup"><span data-stu-id="69b8c-717">`az functionapp create`: AzureWebJobsDashboard will only be set if AppInsights is disabled</span></span>
* <span data-ttu-id="69b8c-718">Correção #10664 – Integração VNet – Problema de Verificação de Localização e Correção #13257-AZ Web App falha quando o RG precisar ser criado</span><span class="sxs-lookup"><span data-stu-id="69b8c-718">Fix #10664- VNet Integration - Location Check Issue & fix #13257- az webapp up failing when RG needs to be created</span></span>
* <span data-ttu-id="69b8c-719">`az webapp|functionapp config ssl import`: Pesquisa o cofre de chaves em grupos de recursos na assinatura e aprimora a ajuda e os exemplos.</span><span class="sxs-lookup"><span data-stu-id="69b8c-719">`az webapp|functionapp config ssl import`: Lookup key vault across resources groups in subscription and improve help and examples.</span></span>
* <span data-ttu-id="69b8c-720">Integra o contexto local para o serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="69b8c-720">Onboard local context for app service</span></span>

### <a name="arm"></a><span data-ttu-id="69b8c-721">ARM</span><span class="sxs-lookup"><span data-stu-id="69b8c-721">ARM</span></span>

* <span data-ttu-id="69b8c-722">`az deployment`: Corrige o problema que faz com que o templateLink não seja retornado ao implantar ou validar o template-uri</span><span class="sxs-lookup"><span data-stu-id="69b8c-722">`az deployment`: Fix the problem that the templateLink will not be returned when deploying or validating template-uri</span></span>
* <span data-ttu-id="69b8c-723">`az deployment`: Corrige o problema que faz com que implantação/validação não dê suporte ao caractere codificado especialmente</span><span class="sxs-lookup"><span data-stu-id="69b8c-723">`az deployment`: Fix the problem that deployment/validate does not support specially encoded character</span></span>
* <span data-ttu-id="69b8c-724">`az deployment sub/group what-if`: Corrige o alinhamento de matriz e o tratamento de erro</span><span class="sxs-lookup"><span data-stu-id="69b8c-724">`az deployment sub/group what-if`: Fix array alignment and error handling</span></span>
* <span data-ttu-id="69b8c-725">`az deployment operation`: Modifica as informações preteridas</span><span class="sxs-lookup"><span data-stu-id="69b8c-725">`az deployment operation`: Modify the deprecate information</span></span>

### <a name="aro"></a><span data-ttu-id="69b8c-726">ARO</span><span class="sxs-lookup"><span data-stu-id="69b8c-726">ARO</span></span>

* <span data-ttu-id="69b8c-727">Adiciona exemplos para az aro create, list, list-credentials, show, delete</span><span class="sxs-lookup"><span data-stu-id="69b8c-727">Add examples to az aro create, list, list-credentials, show, delete</span></span>
* <span data-ttu-id="69b8c-728">Adiciona a função generate_random_id</span><span class="sxs-lookup"><span data-stu-id="69b8c-728">Add generate_random_id function</span></span>

### <a name="backup"></a><span data-ttu-id="69b8c-729">Backup</span><span class="sxs-lookup"><span data-stu-id="69b8c-729">Backup</span></span>

* <span data-ttu-id="69b8c-730">Permite FriendlyName ao habilitar proteção para o comando AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="69b8c-730">Allow FriendlyName in enable protection for AzureFileShare command</span></span>
* <span data-ttu-id="69b8c-731">Correção do comando restore-disks da IaasVM</span><span class="sxs-lookup"><span data-stu-id="69b8c-731">Fix in IaasVM restore-disks Command</span></span>
* <span data-ttu-id="69b8c-732">Adiciona o BackupManagementType "MAB" ao comando item list</span><span class="sxs-lookup"><span data-stu-id="69b8c-732">Add "MAB" BackupManagementType to item list command</span></span>
* <span data-ttu-id="69b8c-733">Adiciona suporte para a repetição de tentativas de atualização da política para itens com falha.</span><span class="sxs-lookup"><span data-stu-id="69b8c-733">Add support for retrying policy update for failed items.</span></span>
* <span data-ttu-id="69b8c-734">Adiciona a funcionalidade de Retomada de Proteção para as Máquinas Virtuais do Azure</span><span class="sxs-lookup"><span data-stu-id="69b8c-734">Add Resume Protection functionality for Azure Virtual Machine</span></span>
* <span data-ttu-id="69b8c-735">Adiciona suporte para especificar o ResourceGroup para armazenar instantRP durante a Criação ou Modificação de Política</span><span class="sxs-lookup"><span data-stu-id="69b8c-735">Add support to specify ResourceGroup for storing instantRP during Create or Modify Policy</span></span>

### <a name="ci"></a><span data-ttu-id="69b8c-736">CI</span><span class="sxs-lookup"><span data-stu-id="69b8c-736">CI</span></span>

* <span data-ttu-id="69b8c-737">Suporte para flake8 3.8.0</span><span class="sxs-lookup"><span data-stu-id="69b8c-737">Support flake8 3.8.0</span></span>

### <a name="compute"></a><span data-ttu-id="69b8c-738">Computação</span><span class="sxs-lookup"><span data-stu-id="69b8c-738">Compute</span></span>

* <span data-ttu-id="69b8c-739">Novo comando az vm auto-shutdown</span><span class="sxs-lookup"><span data-stu-id="69b8c-739">New command az vm auto-shutdown</span></span>
* <span data-ttu-id="69b8c-740">`az vm list-skus`: Atualização do comportamento --zone, retorna SKUs de todos os tipos agora</span><span class="sxs-lookup"><span data-stu-id="69b8c-740">`az vm list-skus`: Update --zone behavior, return all type skus now</span></span>

### <a name="core"></a><span data-ttu-id="69b8c-741">Núcleo</span><span class="sxs-lookup"><span data-stu-id="69b8c-741">Core</span></span>

* <span data-ttu-id="69b8c-742">Atualiza o status de ativado/desativado do contexto local para o nível de usuário global</span><span class="sxs-lookup"><span data-stu-id="69b8c-742">Update local context on/off status to global user level</span></span>

### <a name="extension"></a><span data-ttu-id="69b8c-743">Extensão</span><span class="sxs-lookup"><span data-stu-id="69b8c-743">Extension</span></span>

* <span data-ttu-id="69b8c-744">`az extension add`: Adiciona --system para habilitar a instalação de extensões em um caminho do sistema</span><span class="sxs-lookup"><span data-stu-id="69b8c-744">`az extension add`: Add --system to enable installing extensions in a system path</span></span>
* <span data-ttu-id="69b8c-745">Suporte para .egg-info para armazenar metadados de extensão de tipo de roda</span><span class="sxs-lookup"><span data-stu-id="69b8c-745">Support .egg-info to store wheel type extension metadata</span></span>

### <a name="iot"></a><span data-ttu-id="69b8c-746">IoT</span><span class="sxs-lookup"><span data-stu-id="69b8c-746">IoT</span></span>

* <span data-ttu-id="69b8c-747">`az iot`: Atualiza a mensagem de reconhecimento de extensão da primeira execução do módulo de comando IoT para a ID precisa e moderna não preterida `azure-iot`.</span><span class="sxs-lookup"><span data-stu-id="69b8c-747">`az iot`: Update the IoT command module first run extension awareness message to the accurate, non-deprecated modern Id `azure-iot`.</span></span>

### <a name="iot-hub"></a><span data-ttu-id="69b8c-748">Hub IoT</span><span class="sxs-lookup"><span data-stu-id="69b8c-748">IoT Hub</span></span>

* <span data-ttu-id="69b8c-749">Suporte para comandos de isolamento de rede e API 2020-03-01</span><span class="sxs-lookup"><span data-stu-id="69b8c-749">Support for 2020-03-01 API and Network Isolation commands</span></span>

### <a name="netappfiles"></a><span data-ttu-id="69b8c-750">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="69b8c-750">NetAppFiles</span></span>

* <span data-ttu-id="69b8c-751">`az volume create`: Adiciona snapshot-id como um parâmetro para criar volume – isso permitirá que os usuários criem um volume por meio de um instantâneo existente.</span><span class="sxs-lookup"><span data-stu-id="69b8c-751">`az volume create`: Adds snapshot-id as a parameter to create volume this will allow users to create a volume from existing snapshot.</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-752">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-752">Network</span></span>

* <span data-ttu-id="69b8c-753">Corrige o valor TTL alterado não destinado ao DNS add-record</span><span class="sxs-lookup"><span data-stu-id="69b8c-753">Fix ttl value changed unintended for dns add-record</span></span>
* <span data-ttu-id="69b8c-754">`az network public-ip create`: Informa os clientes sobre futuras alterações da falha</span><span class="sxs-lookup"><span data-stu-id="69b8c-754">`az network public-ip create`: Inform customers of a coming breaking change</span></span>
* <span data-ttu-id="69b8c-755">Suporte para comandos genéricos para cenários de link privado</span><span class="sxs-lookup"><span data-stu-id="69b8c-755">Support generic commands for private link scenario</span></span>
* <span data-ttu-id="69b8c-756">`az network private-endpoint-connection`: Suporte para tipos mysql, postgre e mariadb</span><span class="sxs-lookup"><span data-stu-id="69b8c-756">`az network private-endpoint-connection`: Support mysql, postgre and mariadb types</span></span>
* <span data-ttu-id="69b8c-757">`az network private-endpoint-connection`: Suporte para tipos cosmosdb</span><span class="sxs-lookup"><span data-stu-id="69b8c-757">`az network private-endpoint-connection`: Support cosmosdb types</span></span>
* <span data-ttu-id="69b8c-758">`az network private-endpoint`: pretere --group-ids e redireciona para --group-id</span><span class="sxs-lookup"><span data-stu-id="69b8c-758">`az network private-endpoint`: deprecate --group-ids and redirect to --group-id</span></span>

### <a name="output"></a><span data-ttu-id="69b8c-759">Saída</span><span class="sxs-lookup"><span data-stu-id="69b8c-759">Output</span></span>

* <span data-ttu-id="69b8c-760">Mostra instruções de atualização em localizar, comentários e --help</span><span class="sxs-lookup"><span data-stu-id="69b8c-760">Show update instruction in find, feedback and --help</span></span>

### <a name="packaging"></a><span data-ttu-id="69b8c-761">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-761">Packaging</span></span>

* <span data-ttu-id="69b8c-762">Cria pacotes MSI/Homebrew com dependências resolvidas de requirements.txt</span><span class="sxs-lookup"><span data-stu-id="69b8c-762">Build MSI/Homebrew packages with dependecies resolved from requirements.txt</span></span>

### <a name="rbac"></a><span data-ttu-id="69b8c-763">RBAC</span><span class="sxs-lookup"><span data-stu-id="69b8c-763">RBAC</span></span>

* <span data-ttu-id="69b8c-764">`az ad sp credential reset`: corrige a geração de credenciais fracas</span><span class="sxs-lookup"><span data-stu-id="69b8c-764">`az ad sp credential reset`: fix weak credential generation</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-765">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-765">Storage</span></span>

* <span data-ttu-id="69b8c-766">`az storage account file-service-properties update/show`: Adiciona suporte a propriedades de arquivo para a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-766">`az storage account file-service-properties update/show`: Add File Properties Support for Storage Account</span></span>
* <span data-ttu-id="69b8c-767">`az storage container create`: Correção #13373 ao adicionar o validador para acesso público</span><span class="sxs-lookup"><span data-stu-id="69b8c-767">`az storage container create`: Fix #13373 by adding validator for public access</span></span>
* <span data-ttu-id="69b8c-768">Adiciona suporte a ADLS Gen2 track2</span><span class="sxs-lookup"><span data-stu-id="69b8c-768">Add ADLS Gen2 track2 support</span></span>
* <span data-ttu-id="69b8c-769">`az storage blob sync`: Dar suporte à `--connection-string`</span><span class="sxs-lookup"><span data-stu-id="69b8c-769">`az storage blob sync`: Support `--connection-string`</span></span>
* <span data-ttu-id="69b8c-770">`az storage blob sync`: Corrige a mensagem de erro incorreta quando azcopy não consegue encontrar o local de instalação</span><span class="sxs-lookup"><span data-stu-id="69b8c-770">`az storage blob sync`: Fix the incorrect error message when azcopy cannot find the installation location</span></span>

## <a name="april-30-2020"></a><span data-ttu-id="69b8c-771">30 de abril de 2020</span><span class="sxs-lookup"><span data-stu-id="69b8c-771">April 30, 2020</span></span>

<span data-ttu-id="69b8c-772">Versão 2.5.1</span><span class="sxs-lookup"><span data-stu-id="69b8c-772">Version 2.5.1</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-773">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-773">ACR</span></span>

* <span data-ttu-id="69b8c-774">`az acr check-health`: correção de "DOCKER_PULL_ERROR" no Windows</span><span class="sxs-lookup"><span data-stu-id="69b8c-774">`az acr check-health`: Fix "DOCKER_PULL_ERROR" on Windows</span></span>

### <a name="compute"></a><span data-ttu-id="69b8c-775">Computação</span><span class="sxs-lookup"><span data-stu-id="69b8c-775">Compute</span></span>

* <span data-ttu-id="69b8c-776">`az vm list-ip-addresses`: Tratamento de erros</span><span class="sxs-lookup"><span data-stu-id="69b8c-776">`az vm list-ip-addresses`: Error handling</span></span>
* <span data-ttu-id="69b8c-777">Correção de um bug de criação de VM caso endpoint_vm_image_alias_doc não estivesse definido no perfil de nuvem</span><span class="sxs-lookup"><span data-stu-id="69b8c-777">Fix a bug of vm create if endpoint_vm_image_alias_doc is not set in cloud profile</span></span>
* <span data-ttu-id="69b8c-778">`az vmss create`: adição de --os-disk-size-gb</span><span class="sxs-lookup"><span data-stu-id="69b8c-778">`az vmss create`: Add --os-disk-size-gb</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="69b8c-779">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="69b8c-779">Cosmos DB</span></span>

* <span data-ttu-id="69b8c-780">`az cosmosdb create/update`: adição de suporte a --enable-public-network</span><span class="sxs-lookup"><span data-stu-id="69b8c-780">`az cosmosdb create/update`: add --enable-public-network support</span></span>

### <a name="extension"></a><span data-ttu-id="69b8c-781">Extensão</span><span class="sxs-lookup"><span data-stu-id="69b8c-781">Extension</span></span>

* <span data-ttu-id="69b8c-782">Correção do carregamento de metadados errados para a extensão de tipo roda</span><span class="sxs-lookup"><span data-stu-id="69b8c-782">Fix loading wrong metadata for wheel type extension</span></span>

### <a name="packaging"></a><span data-ttu-id="69b8c-783">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-783">Packaging</span></span>

* <span data-ttu-id="69b8c-784">Adição de script az para Git Bash/Cygwin no Windows</span><span class="sxs-lookup"><span data-stu-id="69b8c-784">Add az script for Git Bash/Cygwin on Windows</span></span>

### <a name="sql"></a><span data-ttu-id="69b8c-785">SQL</span><span class="sxs-lookup"><span data-stu-id="69b8c-785">SQL</span></span>

* <span data-ttu-id="69b8c-786">`az sql instance-pool`: adição de grupo de comando de pools de instância</span><span class="sxs-lookup"><span data-stu-id="69b8c-786">`az sql instance-pool`: Add instance pools command group</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-787">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-787">Storage</span></span>

* <span data-ttu-id="69b8c-788">Atualização do pacote azure-multiapi-storage para 0.3.0</span><span class="sxs-lookup"><span data-stu-id="69b8c-788">Upgrade package azure-multiapi-storage to 0.3.0</span></span>
* <span data-ttu-id="69b8c-789">Dá suporte ao GZRS para a criação e atualização da conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-789">Support GZRS for storage account creation and update</span></span>
* <span data-ttu-id="69b8c-790">`az storage account failover`: adição de suporte para failover da conta de armazenamento de GRS/GZRS</span><span class="sxs-lookup"><span data-stu-id="69b8c-790">`az storage account failover`: Add support for grs/gzrs storage account failover</span></span>
* <span data-ttu-id="69b8c-791">`az storage blob upload`: adição do parâmetro --encryption-scope para dar suporte à especificação da informação do escopo da criptografia</span><span class="sxs-lookup"><span data-stu-id="69b8c-791">`az storage blob upload`: Add --encryption-scope parameter to support specifying encryption scope information</span></span>

## <a name="april-28-2020"></a><span data-ttu-id="69b8c-792">28 de abril de 2020</span><span class="sxs-lookup"><span data-stu-id="69b8c-792">April 28, 2020</span></span>

<span data-ttu-id="69b8c-793">Versão 2.5.0</span><span class="sxs-lookup"><span data-stu-id="69b8c-793">Version 2.5.0</span></span>

### <a name="acs"></a><span data-ttu-id="69b8c-794">ACS</span><span class="sxs-lookup"><span data-stu-id="69b8c-794">ACS</span></span>

* <span data-ttu-id="69b8c-795">[ALTERAÇÃO SIGNIFICATIVA] az openshift create: remove o parâmetro --vnet-peer.</span><span class="sxs-lookup"><span data-stu-id="69b8c-795">[BREAKING CHANGE] az openshift create: remove --vnet-peer parameter.</span></span>
* <span data-ttu-id="69b8c-796">`az openshift create`: adição de sinalizadores para dar suporte a clusters privados.</span><span class="sxs-lookup"><span data-stu-id="69b8c-796">`az openshift create`: add flags to support private cluster.</span></span>
* <span data-ttu-id="69b8c-797">`az openshift`: atualização para a versão `2019-10-27-preview` da API.</span><span class="sxs-lookup"><span data-stu-id="69b8c-797">`az openshift`: upgrade to `2019-10-27-preview` API version.</span></span>
* <span data-ttu-id="69b8c-798">`az openshift`: adição do comando `update`.</span><span class="sxs-lookup"><span data-stu-id="69b8c-798">`az openshift`: add `update` command.</span></span>

### <a name="aks"></a><span data-ttu-id="69b8c-799">AKS</span><span class="sxs-lookup"><span data-stu-id="69b8c-799">AKS</span></span>

* <span data-ttu-id="69b8c-800">`az aks create`: adição do suporte para Windows</span><span class="sxs-lookup"><span data-stu-id="69b8c-800">`az aks create`: Add support for Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-801">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-801">AppService</span></span>

* <span data-ttu-id="69b8c-802">`az webapp deployment source config-zip`: remoção da suspensão após request.get()</span><span class="sxs-lookup"><span data-stu-id="69b8c-802">`az webapp deployment source config-zip`: remove sleep after request.get()</span></span>

### <a name="arm"></a><span data-ttu-id="69b8c-803">ARM</span><span class="sxs-lookup"><span data-stu-id="69b8c-803">ARM</span></span>

* <span data-ttu-id="69b8c-804">Adição de comandos What-If de implantação de modelo</span><span class="sxs-lookup"><span data-stu-id="69b8c-804">Add template deployment What-If commands</span></span>

### <a name="aro"></a><span data-ttu-id="69b8c-805">ARO</span><span class="sxs-lookup"><span data-stu-id="69b8c-805">ARO</span></span>

* <span data-ttu-id="69b8c-806">`az aro`: correção da saída da tabela</span><span class="sxs-lookup"><span data-stu-id="69b8c-806">`az aro`: Fix table output</span></span>

### <a name="ci"></a><span data-ttu-id="69b8c-807">CI</span><span class="sxs-lookup"><span data-stu-id="69b8c-807">CI</span></span>

* <span data-ttu-id="69b8c-808">Integração do pytest e preterição do nose para o teste de automação</span><span class="sxs-lookup"><span data-stu-id="69b8c-808">Onboard pytest and deprecate nose for Automation Test</span></span>

### <a name="compute"></a><span data-ttu-id="69b8c-809">Computação</span><span class="sxs-lookup"><span data-stu-id="69b8c-809">Compute</span></span>

* <span data-ttu-id="69b8c-810">`az vmss disk detach`: correção do problema de NoneType do disco de dados</span><span class="sxs-lookup"><span data-stu-id="69b8c-810">`az vmss disk detach`: fix data disk NoneType issue</span></span>
* <span data-ttu-id="69b8c-811">`az vm availability-set list`: suporte à exibição da lista de VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-811">`az vm availability-set list`: Support showing VM list</span></span>
* <span data-ttu-id="69b8c-812">`az vm list-skus`: correção do problema de exibição do formato de tabela</span><span class="sxs-lookup"><span data-stu-id="69b8c-812">`az vm list-skus`: Fix display problem of table format</span></span>

### <a name="keyvault"></a><span data-ttu-id="69b8c-813">KeyVault</span><span class="sxs-lookup"><span data-stu-id="69b8c-813">KeyVault</span></span>

* <span data-ttu-id="69b8c-814">Adição de novo parâmetro `--enable-rbac-authorization` durante a criação ou atualização</span><span class="sxs-lookup"><span data-stu-id="69b8c-814">Add new parameter `--enable-rbac-authorization` during creating or updating</span></span>

### <a name="monitor"></a><span data-ttu-id="69b8c-815">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="69b8c-815">Monitor</span></span>

* <span data-ttu-id="69b8c-816">Suporte aos recursos de CMK do cluster de LA</span><span class="sxs-lookup"><span data-stu-id="69b8c-816">Support LA cluster CMK features</span></span>
* <span data-ttu-id="69b8c-817">`az monitor log-analytics workspace linked-storage`: dá suporte aos recursos BYOS</span><span class="sxs-lookup"><span data-stu-id="69b8c-817">`az monitor log-analytics workspace linked-storage`: supports BYOS features</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-818">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-818">Network</span></span>

* <span data-ttu-id="69b8c-819">`az network security-partner`: suporte para provedor de segurança de parceiros</span><span class="sxs-lookup"><span data-stu-id="69b8c-819">`az network security-partner`: support security partner provider</span></span>

### <a name="privatedns"></a><span data-ttu-id="69b8c-820">Privatedns</span><span class="sxs-lookup"><span data-stu-id="69b8c-820">Privatedns</span></span>

* <span data-ttu-id="69b8c-821">Adição do recurso na zona DNS privada para importar o arquivo da zona de exportação</span><span class="sxs-lookup"><span data-stu-id="69b8c-821">Add feature in private DNS zone to import export zone file</span></span>

## <a name="april-21-2020"></a><span data-ttu-id="69b8c-822">21 de abril de 2020</span><span class="sxs-lookup"><span data-stu-id="69b8c-822">April 21, 2020</span></span>

<span data-ttu-id="69b8c-823">Versão 2.4.0</span><span class="sxs-lookup"><span data-stu-id="69b8c-823">Version 2.4.0</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-824">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-824">ACR</span></span>

* <span data-ttu-id="69b8c-825">`az acr run --cmd`: desabilitar a substituição do diretório de trabalho</span><span class="sxs-lookup"><span data-stu-id="69b8c-825">`az acr run --cmd`: disable working directory override</span></span>
* <span data-ttu-id="69b8c-826">Suporte ao ponto de extremidade dos dados dedicados</span><span class="sxs-lookup"><span data-stu-id="69b8c-826">Support dedicated data endpoint</span></span>

### <a name="aks"></a><span data-ttu-id="69b8c-827">AKS</span><span class="sxs-lookup"><span data-stu-id="69b8c-827">AKS</span></span>

* <span data-ttu-id="69b8c-828">`az aks list -o table` deve mostrar privateFqdn como fqdn para clusters privados</span><span class="sxs-lookup"><span data-stu-id="69b8c-828">`az aks list -o table` should show privateFqdn as fqdn for private clusters</span></span>
* <span data-ttu-id="69b8c-829">Adicionar --uptime-sla</span><span class="sxs-lookup"><span data-stu-id="69b8c-829">Add --uptime-sla</span></span>
* <span data-ttu-id="69b8c-830">Atualizar pacote containerservice</span><span class="sxs-lookup"><span data-stu-id="69b8c-830">Update containerservice package</span></span>
* <span data-ttu-id="69b8c-831">Adicionar suporte ao IP público do nó</span><span class="sxs-lookup"><span data-stu-id="69b8c-831">Add node public IP support</span></span>
* <span data-ttu-id="69b8c-832">Corrigir erros de digitação no comando de ajuda</span><span class="sxs-lookup"><span data-stu-id="69b8c-832">Fix typo in the help command</span></span>

### <a name="appconfig"></a><span data-ttu-id="69b8c-833">AppConfig</span><span class="sxs-lookup"><span data-stu-id="69b8c-833">AppConfig</span></span>

* <span data-ttu-id="69b8c-834">Resolver referência do cofre de chaves para os comandos kv list e export</span><span class="sxs-lookup"><span data-stu-id="69b8c-834">Resolve key vault reference for kv list and export commands</span></span>
* <span data-ttu-id="69b8c-835">Correção de bug para valores de chave da lista</span><span class="sxs-lookup"><span data-stu-id="69b8c-835">Bug fix for list key values</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-836">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-836">AppService</span></span>

* <span data-ttu-id="69b8c-837">`az functionapp create`: mudou a maneira como o linuxFxVersion estava sendo definido para os aplicativos de funções dotnet linux.</span><span class="sxs-lookup"><span data-stu-id="69b8c-837">`az functionapp create`: Changed the way linuxFxVersion was being set for dotnet linux function apps.</span></span> <span data-ttu-id="69b8c-838">Isso deve corrigir um bug que estava impedindo a criação de aplicativos de consumo em dotnet linux</span><span class="sxs-lookup"><span data-stu-id="69b8c-838">This should fix a bug that was preventing dotnet linux consumption apps from being created</span></span>
* <span data-ttu-id="69b8c-839">[ALTERAÇÃO DA FALHA] `az webapp create`: correção para manter o AppSettings existente com o az webapp create</span><span class="sxs-lookup"><span data-stu-id="69b8c-839">[BREAKING CHANGE] `az webapp create`: fix to keep existing AppSettings with az webapp create</span></span>
* <span data-ttu-id="69b8c-840">[ALTERAÇÃO DA FALHA] `az webapp up`: correção para criar o RG para o comando az webapp up ao usar o sinalizador -g</span><span class="sxs-lookup"><span data-stu-id="69b8c-840">[BREAKING CHANGE] `az webapp up`: fix to create RG for az webapp up command when using -g flag</span></span>
* <span data-ttu-id="69b8c-841">[ALTERAÇÃO DA FALHA] `az webapp config`: correção para mostrar valores de saída não JSON com o az webapp config connection-string list</span><span class="sxs-lookup"><span data-stu-id="69b8c-841">[BREAKING CHANGE] `az webapp config`: fix to show values for non-JSON output with az webapp config connection-string list</span></span>

### <a name="arm"></a><span data-ttu-id="69b8c-842">ARM</span><span class="sxs-lookup"><span data-stu-id="69b8c-842">ARM</span></span>

* <span data-ttu-id="69b8c-843">`az deployment create/validate`: adicionar o parâmetro `--no-prompt` para dar suporte à ação de ignorar o prompt de parâmetros ausentes para o modelo do Resource Manager</span><span class="sxs-lookup"><span data-stu-id="69b8c-843">`az deployment create/validate`: Add parameter `--no-prompt` to support skipping the prompt of missing parameters for ARM template</span></span>
* <span data-ttu-id="69b8c-844">`az deployment group/mg/sub/tenant validate`: dar suporte aos comentários no arquivo de parâmetro de implantação</span><span class="sxs-lookup"><span data-stu-id="69b8c-844">`az deployment group/mg/sub/tenant validate`: Support comments in deployment parameter file</span></span>
* <span data-ttu-id="69b8c-845">`az deployment`: remover `is_preview` para o parâmetro `--handle-extended-json-format`</span><span class="sxs-lookup"><span data-stu-id="69b8c-845">`az deployment`: Remove `is_preview` for parameter `--handle-extended-json-format`</span></span>
* <span data-ttu-id="69b8c-846">`az deployment group/mg/sub/tenant cancel`: dar suporte para cancelar a implantação do modelo do Resource Manager</span><span class="sxs-lookup"><span data-stu-id="69b8c-846">`az deployment group/mg/sub/tenant cancel`: Support cancel deployment for ARM template</span></span>
* <span data-ttu-id="69b8c-847">`az deployment group/mg/sub/tenant validate`: melhorar a mensagem de erro quando a verificação de implantação falhar</span><span class="sxs-lookup"><span data-stu-id="69b8c-847">`az deployment group/mg/sub/tenant validate`: Improve the error message when deployment verification fails</span></span>
* <span data-ttu-id="69b8c-848">`az deployment-scripts`: adicionar novos comandos para DeploymentScripts</span><span class="sxs-lookup"><span data-stu-id="69b8c-848">`az deployment-scripts`: Add new commands for DeploymentScripts</span></span>
* <span data-ttu-id="69b8c-849">`az resource tag`: adicionar o parâmetro `--is-incremental` para dar suporte à adição de marcas ao recurso de maneira incremental</span><span class="sxs-lookup"><span data-stu-id="69b8c-849">`az resource tag`: Add parameter `--is-incremental` to support adding tags to resource incrementally</span></span>

### <a name="aro"></a><span data-ttu-id="69b8c-850">ARO</span><span class="sxs-lookup"><span data-stu-id="69b8c-850">ARO</span></span>

* <span data-ttu-id="69b8c-851">`az aro`:  adicionar módulo de comando aro do Azure RedHat OpenShift V4</span><span class="sxs-lookup"><span data-stu-id="69b8c-851">`az aro`:  Add Azure RedHat OpenShift V4 aro command module</span></span>

### <a name="batch"></a><span data-ttu-id="69b8c-852">Lote</span><span class="sxs-lookup"><span data-stu-id="69b8c-852">Batch</span></span>

* <span data-ttu-id="69b8c-853">Atualizar a API do Lote</span><span class="sxs-lookup"><span data-stu-id="69b8c-853">Update Batch API</span></span>

### <a name="compute"></a><span data-ttu-id="69b8c-854">Computação</span><span class="sxs-lookup"><span data-stu-id="69b8c-854">Compute</span></span>

* <span data-ttu-id="69b8c-855">`az sig image-version create`: adicionar o tipo da conta de armazenamento Premium_LRS</span><span class="sxs-lookup"><span data-stu-id="69b8c-855">`az sig image-version create`: Add storage account type Premium_LRS</span></span>
* <span data-ttu-id="69b8c-856">`az vmss update`: corrigir problema de atualização de notificação de término</span><span class="sxs-lookup"><span data-stu-id="69b8c-856">`az vmss update`: Fix terminate notification update issue</span></span>
* <span data-ttu-id="69b8c-857">`az vm/vmss create`: adicionar suporte para a versão de imagem especializada</span><span class="sxs-lookup"><span data-stu-id="69b8c-857">`az vm/vmss create`: Add support for specialized image version</span></span>
* <span data-ttu-id="69b8c-858">Versão da API SIG 2019-12-01</span><span class="sxs-lookup"><span data-stu-id="69b8c-858">SIG API Version 2019-12-01</span></span>
* <span data-ttu-id="69b8c-859">`az sig image-version create`: Adicionar --target-region-encryption</span><span class="sxs-lookup"><span data-stu-id="69b8c-859">`az sig image-version create`: Add --target-region-encryption</span></span>
* <span data-ttu-id="69b8c-860">Os testes de correção falham quando executados em série, pois o nome do keyvault está duplicado no cache global na memória</span><span class="sxs-lookup"><span data-stu-id="69b8c-860">Fix tests fail when running in serial due to keyvault name is duplicated in global in-momery cache</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="69b8c-861">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="69b8c-861">CosmosDB</span></span>

* <span data-ttu-id="69b8c-862">Dar suporte à `az cosmosdb private-link-resource/private-endpoint-connection`</span><span class="sxs-lookup"><span data-stu-id="69b8c-862">Support `az cosmosdb private-link-resource/private-endpoint-connection`</span></span>

### <a name="iot-central"></a><span data-ttu-id="69b8c-863">Central da IoT</span><span class="sxs-lookup"><span data-stu-id="69b8c-863">IoT Central</span></span>

* <span data-ttu-id="69b8c-864">Preterir `az iotcentral`</span><span class="sxs-lookup"><span data-stu-id="69b8c-864">Deprecate `az iotcentral`</span></span>
* <span data-ttu-id="69b8c-865">Adicionar o módulo de comando `az iot central`</span><span class="sxs-lookup"><span data-stu-id="69b8c-865">Add `az iot central` command module</span></span>

### <a name="monitor"></a><span data-ttu-id="69b8c-866">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="69b8c-866">Monitor</span></span>

* <span data-ttu-id="69b8c-867">Dar suporte ao cenário de link privado para monitoramento</span><span class="sxs-lookup"><span data-stu-id="69b8c-867">Support private link scenario for monitor</span></span>
* <span data-ttu-id="69b8c-868">Corrigir a maneira incorreta de simulação em test_monitor_general_operations.py</span><span class="sxs-lookup"><span data-stu-id="69b8c-868">Fix wrong mocking way in test_monitor_general_operations.py</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-869">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-869">Network</span></span>

* <span data-ttu-id="69b8c-870">Preterir o sku para o comando de atualização de ip público</span><span class="sxs-lookup"><span data-stu-id="69b8c-870">Deprecate sku for public ip update command</span></span>
* <span data-ttu-id="69b8c-871">`az network private-endpoint`: dar suporte ao grupo de zona dns privada</span><span class="sxs-lookup"><span data-stu-id="69b8c-871">`az network private-endpoint`: Support private dns zone group</span></span>
* <span data-ttu-id="69b8c-872">Habilitar o recurso de contexto local para o parâmetro vnet/sub-rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-872">Enable local context feature for vnet/subnet parameter</span></span>
* <span data-ttu-id="69b8c-873">Corrigir o exemplo de uso incorreto em test_nw_flow_log_delete</span><span class="sxs-lookup"><span data-stu-id="69b8c-873">Fix wrong usage example in test_nw_flow_log_delete</span></span>

### <a name="packaging"></a><span data-ttu-id="69b8c-874">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-874">Packaging</span></span>

* <span data-ttu-id="69b8c-875">Descartar o suporte para o pacote Ubuntu/Disco</span><span class="sxs-lookup"><span data-stu-id="69b8c-875">Drop support for Ubuntu/Disco package</span></span>

### <a name="rbac"></a><span data-ttu-id="69b8c-876">RBAC</span><span class="sxs-lookup"><span data-stu-id="69b8c-876">RBAC</span></span>

* <span data-ttu-id="69b8c-877">`az ad app create/update`: dar suporte a --optional-claims como um parâmetro</span><span class="sxs-lookup"><span data-stu-id="69b8c-877">`az ad app create/update`: support --optional-claims as a parameter</span></span>

### <a name="rdbms"></a><span data-ttu-id="69b8c-878">RDBMS</span><span class="sxs-lookup"><span data-stu-id="69b8c-878">RDBMS</span></span>

* <span data-ttu-id="69b8c-879">Adicionar comandos do administrador do Azure Active Directory para PostgreSQL e MySQL</span><span class="sxs-lookup"><span data-stu-id="69b8c-879">Add Azure active directory administrator commands for PostgreSQL and MySQL</span></span>

### <a name="service-fabric"></a><span data-ttu-id="69b8c-880">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="69b8c-880">Service Fabric</span></span>

* <span data-ttu-id="69b8c-881">Correção nº 12891: `az sf application update --application-parameters` remove parâmetros antigos que não estão na solicitação</span><span class="sxs-lookup"><span data-stu-id="69b8c-881">Fix #12891: `az sf application update --application-parameters` removes old parameters that are not in the request</span></span>
* <span data-ttu-id="69b8c-882">Correção nº 12470 az sf create cluster, corrigir bugs na atualização de durabilidade e confiabilidade e encontrar vmss corretamente por meio do código, dado um nome de tipo de nó</span><span class="sxs-lookup"><span data-stu-id="69b8c-882">Fix #12470 az sf create cluster, fix bugs in update durability and reliability and find vmss correctly through the code given a node type name</span></span>

### <a name="sql"></a><span data-ttu-id="69b8c-883">SQL</span><span class="sxs-lookup"><span data-stu-id="69b8c-883">SQL</span></span>

* <span data-ttu-id="69b8c-884">Adicionar `az sql mi op list`, `az sql mi op get`, `az sql mi op cancel`</span><span class="sxs-lookup"><span data-stu-id="69b8c-884">Add `az sql mi op list`, `az sql mi op get`, `az sql mi op cancel`</span></span>
* <span data-ttu-id="69b8c-885">`az sql midb`: atualizar/mostrar política de retenção de longo prazo, mostrar/excluir backups de retenção de longo prazo, restaurar backup de retenção de longo prazo</span><span class="sxs-lookup"><span data-stu-id="69b8c-885">`az sql midb`: update/show long term retention policy,  show/delete long term retention backups, restore long term retention backup</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-886">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-886">Storage</span></span>

* <span data-ttu-id="69b8c-887">Atualizar azure-mgmt-storage para 9.0.0</span><span class="sxs-lookup"><span data-stu-id="69b8c-887">Upgrade azure-mgmt-storage to 9.0.0</span></span>
* <span data-ttu-id="69b8c-888">`az storage logging off`: dar suporte à desativação do registro em log de uma conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-888">`az storage logging off`: Support turning off logging for a storage account</span></span>
* <span data-ttu-id="69b8c-889">`az storage account update`: habilitar rotação automática de chave para CMK</span><span class="sxs-lookup"><span data-stu-id="69b8c-889">`az storage account update`: Enable key auto-rotated for CMK</span></span>
* <span data-ttu-id="69b8c-890">`az storage account encryption-scope create/update/list/show`: adicionar suporte para personalizar o escopo de criptografia</span><span class="sxs-lookup"><span data-stu-id="69b8c-890">`az storage account encryption-scope create/update/list/show`: Add support to customize encryption scope</span></span>
* <span data-ttu-id="69b8c-891">`az storage container create`: adicionar --default-encryption-scope e --deny-encryption-scope-override a fim de definir o escopo de criptografia para o nível de contêiner</span><span class="sxs-lookup"><span data-stu-id="69b8c-891">`az storage container create`: Add --default-encryption-scope and --deny-encryption-scope-override to set encryption scope for container level</span></span>

### <a name="survey"></a><span data-ttu-id="69b8c-892">Pesquisa</span><span class="sxs-lookup"><span data-stu-id="69b8c-892">Survey</span></span>

* <span data-ttu-id="69b8c-893">Adicionar opção para desligar o link de pesquisa</span><span class="sxs-lookup"><span data-stu-id="69b8c-893">Add switch to turn off survey link</span></span>

## <a name="april-01-2020"></a><span data-ttu-id="69b8c-894">1º de abril de 2020</span><span class="sxs-lookup"><span data-stu-id="69b8c-894">April 01, 2020</span></span>

<span data-ttu-id="69b8c-895">Versão 2.3.1</span><span class="sxs-lookup"><span data-stu-id="69b8c-895">Version 2.3.1</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-896">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-896">ACR</span></span>

* <span data-ttu-id="69b8c-897">Corrigir a versão errada do azure-mgmt-containerregistry para Linux</span><span class="sxs-lookup"><span data-stu-id="69b8c-897">Fix wrong version of azure-mgmt-containerregistry for Linux</span></span>

### <a name="profile"></a><span data-ttu-id="69b8c-898">Perfil</span><span class="sxs-lookup"><span data-stu-id="69b8c-898">Profile</span></span>

* <span data-ttu-id="69b8c-899">az login: Corrigir falha de logon com perfis de nuvem diferentes de `latest`</span><span class="sxs-lookup"><span data-stu-id="69b8c-899">az login: Fix login failure with cloud profiles other than `latest`</span></span>

## <a name="march-31-2020"></a><span data-ttu-id="69b8c-900">31 de março de 2020</span><span class="sxs-lookup"><span data-stu-id="69b8c-900">March 31, 2020</span></span>

<span data-ttu-id="69b8c-901">Versão 2.3.0</span><span class="sxs-lookup"><span data-stu-id="69b8c-901">Version 2.3.0</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-902">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-902">ACR</span></span>

* <span data-ttu-id="69b8c-903">'az acr task update': exceção de ponteiro nulo</span><span class="sxs-lookup"><span data-stu-id="69b8c-903">'az acr task update': null pointer exception</span></span>
* <span data-ttu-id="69b8c-904">`az acr import`: Modificar a mensagem de ajuda e de erro para esclarecer o uso de --source e --registry</span><span class="sxs-lookup"><span data-stu-id="69b8c-904">`az acr import`: Modify help and error message to clarify the usage of --source and --registry</span></span>
* <span data-ttu-id="69b8c-905">Adicionar um validador para o argumento 'registry_name'</span><span class="sxs-lookup"><span data-stu-id="69b8c-905">Add a validator for argument 'registry_name'</span></span>
* <span data-ttu-id="69b8c-906">`az acr login`: remover o sinalizador de visualização em '--expose-token'</span><span class="sxs-lookup"><span data-stu-id="69b8c-906">`az acr login`:Remove the preview flag on '--expose-token'</span></span>
* <span data-ttu-id="69b8c-907">O parâmetro de branch 'az acr task create/update' de [ALTERAÇÃO SIGNIFICATIVA] foi removido</span><span class="sxs-lookup"><span data-stu-id="69b8c-907">[BREAKING CHANGE] 'az acr task create/update' Branch parameter is removed</span></span>
* <span data-ttu-id="69b8c-908">O cliente 'az acr task update' agora pode atualizar o contexto, o token do git e/ou os gatilhos individualmente</span><span class="sxs-lookup"><span data-stu-id="69b8c-908">'az acr task update' Customer now can update context, git-token, and or triggers individually</span></span>
* <span data-ttu-id="69b8c-909">'az acr agentpool': novo recurso</span><span class="sxs-lookup"><span data-stu-id="69b8c-909">'az acr agentpool': new feature</span></span>

### <a name="aks"></a><span data-ttu-id="69b8c-910">AKS</span><span class="sxs-lookup"><span data-stu-id="69b8c-910">AKS</span></span>

* <span data-ttu-id="69b8c-911">Corrigir apiServerAccessProfile ao atualizar --api-server-authorized-ip-ranges</span><span class="sxs-lookup"><span data-stu-id="69b8c-911">Fix apiServerAccessProfile when updating --api-server-authorized-ip-ranges</span></span>
* <span data-ttu-id="69b8c-912">aks update: Substituir IPs de saída por valores de entrada ao atualizar</span><span class="sxs-lookup"><span data-stu-id="69b8c-912">aks update: Override outbound IPs with input values when update</span></span>
* <span data-ttu-id="69b8c-913">Não criar SPN para clusters MSI e dar suporte à anexação de ACR a clusters MSI</span><span class="sxs-lookup"><span data-stu-id="69b8c-913">Do not create SPN for MSI clusters and support attach acr to MSI clusters</span></span>

### <a name="ams"></a><span data-ttu-id="69b8c-914">AMS</span><span class="sxs-lookup"><span data-stu-id="69b8c-914">AMS</span></span>

* <span data-ttu-id="69b8c-915">Correção nº. 12469: a adição da política de chave de conteúdo Fairplay falha devido a problemas com o parâmetro 'ask'</span><span class="sxs-lookup"><span data-stu-id="69b8c-915">Fix #12469: adding Fairplay content-key-policy fails due to problems with 'ask' parameter</span></span>

### <a name="appconfig"></a><span data-ttu-id="69b8c-916">AppConfig</span><span class="sxs-lookup"><span data-stu-id="69b8c-916">AppConfig</span></span>

* <span data-ttu-id="69b8c-917">Adicionar --skip-keyvault a kv export</span><span class="sxs-lookup"><span data-stu-id="69b8c-917">Add --skip-keyvault for kv export</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-918">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-918">AppService</span></span>

* <span data-ttu-id="69b8c-919">Correção nº 12509: remover a marca para az webapp up por padrão</span><span class="sxs-lookup"><span data-stu-id="69b8c-919">Fix #12509: Remove the tag to az webapp up by default</span></span>
* <span data-ttu-id="69b8c-920">az functionapp create: o menu de ajuda de --runtime-version foi atualizado e um aviso foi adicionado quando o usuário especifica --runtime-version para dotnet</span><span class="sxs-lookup"><span data-stu-id="69b8c-920">az functionapp create: Updated --runtime-version help menu and added warning when user specifies --runtime-version for dotnet</span></span>
* <span data-ttu-id="69b8c-921">az functionapp create: atualizado o modo como o javaVersion estava sendo definido para aplicativos de funções do Windows</span><span class="sxs-lookup"><span data-stu-id="69b8c-921">az functionapp create: Updated the way javaVersion was being set for Windows function apps</span></span>

### <a name="arm"></a><span data-ttu-id="69b8c-922">ARM</span><span class="sxs-lookup"><span data-stu-id="69b8c-922">ARM</span></span>

* <span data-ttu-id="69b8c-923">az deployment create/validate: usar --handle-extended-json-format por padrão</span><span class="sxs-lookup"><span data-stu-id="69b8c-923">az deployment create/validate: Use --handle-extended-json-format by default</span></span>
* <span data-ttu-id="69b8c-924">az lock create: adicionar exemplos de criação de subrecurso na documentação da ajuda</span><span class="sxs-lookup"><span data-stu-id="69b8c-924">az lock create: Add examples of creating subresource in the help documentation</span></span>
* <span data-ttu-id="69b8c-925">az deployment {group/mg/sub/tenant} list: dar suporte à filtragem de provisioningState</span><span class="sxs-lookup"><span data-stu-id="69b8c-925">az deployment {group/mg/sub/tenant} list: Support provisioningState filtering</span></span>
* <span data-ttu-id="69b8c-926">az deployment: corrigir o bug de análise para o comentário no último argumento</span><span class="sxs-lookup"><span data-stu-id="69b8c-926">az deployment: Fix the parse bug for comment under the last argument</span></span>

### <a name="backup"></a><span data-ttu-id="69b8c-927">Backup</span><span class="sxs-lookup"><span data-stu-id="69b8c-927">Backup</span></span>

* <span data-ttu-id="69b8c-928">Adicionadas várias funcionalidades de restauração de arquivo</span><span class="sxs-lookup"><span data-stu-id="69b8c-928">Added multiple files restore capabilities</span></span>
* <span data-ttu-id="69b8c-929">Adicionado suporte para backup somente de discos do SO</span><span class="sxs-lookup"><span data-stu-id="69b8c-929">Added support for Backing up OS Disks only</span></span>
* <span data-ttu-id="69b8c-930">Adicionado o parâmetro restore-as-unmanaged-disk para especificar a restauração não gerenciada</span><span class="sxs-lookup"><span data-stu-id="69b8c-930">Added restore-as-unmanaged-disk parameter to specify unmanaged restore</span></span>

### <a name="compute"></a><span data-ttu-id="69b8c-931">Computação</span><span class="sxs-lookup"><span data-stu-id="69b8c-931">Compute</span></span>

* <span data-ttu-id="69b8c-932">az vm create: adicionar opção NONE de --nsg-rule</span><span class="sxs-lookup"><span data-stu-id="69b8c-932">az vm create: Add NONE option of --nsg-rule</span></span>
* <span data-ttu-id="69b8c-933">az vmss create/update: remover a marca de visualização de reparos automáticos do vmss</span><span class="sxs-lookup"><span data-stu-id="69b8c-933">az vmss create/update: remove vmss automatic repairs preview tag</span></span>
* <span data-ttu-id="69b8c-934">az vm update: dar suporte a --workspace</span><span class="sxs-lookup"><span data-stu-id="69b8c-934">az vm update: Support --workspace</span></span>
* <span data-ttu-id="69b8c-935">Corrigir um bug no código de inicialização de VirtualMachineScaleSetExtension</span><span class="sxs-lookup"><span data-stu-id="69b8c-935">Fix a bug in VirtualMachineScaleSetExtension initialization code</span></span>
* <span data-ttu-id="69b8c-936">Atualizar a versão do VMAccessAgent para 2.4</span><span class="sxs-lookup"><span data-stu-id="69b8c-936">Upgrade VMAccessAgent version to 2.4</span></span>
* <span data-ttu-id="69b8c-937">az vmss set-orchestration-service-state: dar suporte para o estado de definição do serviço de orquestração do vmss</span><span class="sxs-lookup"><span data-stu-id="69b8c-937">az vmss set-orchestration-service-state: support vmss set orchestration service state</span></span>
* <span data-ttu-id="69b8c-938">Atualizar a API do disco para a versão 2019-11-01</span><span class="sxs-lookup"><span data-stu-id="69b8c-938">Upgrade disk API version to 2019-11-01</span></span>
* <span data-ttu-id="69b8c-939">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun</span><span class="sxs-lookup"><span data-stu-id="69b8c-939">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="69b8c-940">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="69b8c-940">Cosmos DB</span></span>

* <span data-ttu-id="69b8c-941">Corrigir a ausência da opção --type para redirecionamentos de preterimento</span><span class="sxs-lookup"><span data-stu-id="69b8c-941">Fix missing --type option for deprecation redirections</span></span>

### <a name="docker"></a><span data-ttu-id="69b8c-942">Docker</span><span class="sxs-lookup"><span data-stu-id="69b8c-942">Docker</span></span>

* <span data-ttu-id="69b8c-943">Atualizar para Alpine 3.11 e Python 3.6.10</span><span class="sxs-lookup"><span data-stu-id="69b8c-943">Update to Alpine 3.11 and Python 3.6.10</span></span>

### <a name="extension"></a><span data-ttu-id="69b8c-944">Extensão</span><span class="sxs-lookup"><span data-stu-id="69b8c-944">Extension</span></span>

* <span data-ttu-id="69b8c-945">Permitir carregar extensões no caminho do sistema por meio de pacotes</span><span class="sxs-lookup"><span data-stu-id="69b8c-945">Allow to load extensions in the system path via packages</span></span>

### <a name="hdinsight"></a><span data-ttu-id="69b8c-946">HDInsight</span><span class="sxs-lookup"><span data-stu-id="69b8c-946">HDInsight</span></span>

* <span data-ttu-id="69b8c-947">(az hdinsight create:) dar suporte à especificação da versão de TLS mínima pelos clientes usando o parâmetro `--minimal-tls-version`.</span><span class="sxs-lookup"><span data-stu-id="69b8c-947">(az hdinsight create:) Support customers specify minimal supported tls version by using parameter `--minimal-tls-version`.</span></span> <span data-ttu-id="69b8c-948">O valor permitido é 1.0,1.1,1.2</span><span class="sxs-lookup"><span data-stu-id="69b8c-948">The allowed value is 1.0,1.1,1.2</span></span>

### <a name="iot"></a><span data-ttu-id="69b8c-949">IoT</span><span class="sxs-lookup"><span data-stu-id="69b8c-949">IoT</span></span>

* <span data-ttu-id="69b8c-950">Adicionar codeowner</span><span class="sxs-lookup"><span data-stu-id="69b8c-950">Add codeowner</span></span>
* <span data-ttu-id="69b8c-951">az iot hub create : alterar o SKU padrão de F1 para S1</span><span class="sxs-lookup"><span data-stu-id="69b8c-951">az iot hub create : Change default sku to S1 from F1</span></span>
* <span data-ttu-id="69b8c-952">iot hub: dar suporte a IotHub no perfil de 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="69b8c-952">iot hub: Support IotHub in the profile of 2019-03-01-hybrid</span></span>

### <a name="iotcentral"></a><span data-ttu-id="69b8c-953">IoT Central</span><span class="sxs-lookup"><span data-stu-id="69b8c-953">IoTCentral</span></span>

* <span data-ttu-id="69b8c-954">Atualizar detalhes do erro, atualizar modelo de aplicativo padrão e a mensagem de aviso</span><span class="sxs-lookup"><span data-stu-id="69b8c-954">Update error details, update default application template and prompt message</span></span>

### <a name="keyvault"></a><span data-ttu-id="69b8c-955">KeyVault</span><span class="sxs-lookup"><span data-stu-id="69b8c-955">KeyVault</span></span>

* <span data-ttu-id="69b8c-956">Suporte para backup/restauração de certificado</span><span class="sxs-lookup"><span data-stu-id="69b8c-956">Support certificate backup/restore</span></span>
* <span data-ttu-id="69b8c-957">keyvault create/update: Suporte a --retention-days</span><span class="sxs-lookup"><span data-stu-id="69b8c-957">keyvault create/update: Support --retention-days</span></span>
* <span data-ttu-id="69b8c-958">Não exibir mais chaves/segredos gerenciados durante a listagem</span><span class="sxs-lookup"><span data-stu-id="69b8c-958">No longer display managed keys/secrets while listing</span></span>
* <span data-ttu-id="69b8c-959">az keyvault create: suporte a `--network-acls`, `--network-acls-ips` e `--network-acls-vnets` para especificar regras de rede ao criar o cofre</span><span class="sxs-lookup"><span data-stu-id="69b8c-959">az keyvault create: support `--network-acls`, `--network-acls-ips` and `--network-acls-vnets` for specifying network rules while creating vault</span></span>

### <a name="lock"></a><span data-ttu-id="69b8c-960">Bloqueio</span><span class="sxs-lookup"><span data-stu-id="69b8c-960">Lock</span></span>

* <span data-ttu-id="69b8c-961">az lock delete fix bug: az lock delete não funciona no Microsoft.DocumentDB</span><span class="sxs-lookup"><span data-stu-id="69b8c-961">az lock delete fix bug: az lock delete does not work on Microsoft.DocumentDB</span></span>

### <a name="monitor"></a><span data-ttu-id="69b8c-962">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="69b8c-962">Monitor</span></span>

* <span data-ttu-id="69b8c-963">az monitor clone: suporte a regras de métrica de clone de um recurso para outro</span><span class="sxs-lookup"><span data-stu-id="69b8c-963">az monitor clone: support clone metric rules from one resource to another</span></span>
* <span data-ttu-id="69b8c-964">Corrigir IcM179210086: não é possível criar um alerta de métrica personalizado para a métrica de Application Insights</span><span class="sxs-lookup"><span data-stu-id="69b8c-964">Fix IcM179210086: unable to create custom metric alert for their Application Insights metric</span></span>

### <a name="netappfiles"></a><span data-ttu-id="69b8c-965">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="69b8c-965">NetAppFiles</span></span>

* <span data-ttu-id="69b8c-966">az volume create: permitir volumes de proteção de dados adicionando operações de replicação: approve, suspend, resume, status, remove</span><span class="sxs-lookup"><span data-stu-id="69b8c-966">az volume create: Allow data protection volumes adding replication operations: approve, suspend, resume, status, remove</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-967">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-967">Network</span></span>

* <span data-ttu-id="69b8c-968">az network application-gateway waf-policy managed-rule rule-set add: dar suporte a Microsoft_BotManagerRuleSet</span><span class="sxs-lookup"><span data-stu-id="69b8c-968">az network application-gateway waf-policy managed-rule rule-set add: support Microsoft_BotManagerRuleSet</span></span>
* <span data-ttu-id="69b8c-969">network watcher flow-log show: corrigir informações erradas em preterimento</span><span class="sxs-lookup"><span data-stu-id="69b8c-969">network watcher flow-log show: fix wrong deprecating info</span></span>
* <span data-ttu-id="69b8c-970">dar suporte a nomes de host no ouvinte do gateway de aplicativo</span><span class="sxs-lookup"><span data-stu-id="69b8c-970">support host names in application gateway listener</span></span>
* <span data-ttu-id="69b8c-971">az network nat gateway: dar suporte para criar um recurso vazio sem IP público nem prefixo de IP público</span><span class="sxs-lookup"><span data-stu-id="69b8c-971">az network nat gateway: support create empty resource without public ip or public ip prefix</span></span>
* <span data-ttu-id="69b8c-972">Dar suporte à geração de gateway de VPN</span><span class="sxs-lookup"><span data-stu-id="69b8c-972">Support vpn gateway generation</span></span>
* <span data-ttu-id="69b8c-973">Dar suporte a `--if-none-match` em `az network dns record-set {} add-record`</span><span class="sxs-lookup"><span data-stu-id="69b8c-973">Support `--if-none-match` in `az network dns record-set {} add-record`</span></span>

### <a name="packaging"></a><span data-ttu-id="69b8c-974">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-974">Packaging</span></span>

* <span data-ttu-id="69b8c-975">Remover o suporte ao Python 3.5</span><span class="sxs-lookup"><span data-stu-id="69b8c-975">Drop support for python 3.5</span></span>

### <a name="profile"></a><span data-ttu-id="69b8c-976">Perfil</span><span class="sxs-lookup"><span data-stu-id="69b8c-976">Profile</span></span>

* <span data-ttu-id="69b8c-977">az login: Mostrar aviso para erro de MFA</span><span class="sxs-lookup"><span data-stu-id="69b8c-977">az login: Show warning for MFA error</span></span>

### <a name="rdbms"></a><span data-ttu-id="69b8c-978">RDBMS</span><span class="sxs-lookup"><span data-stu-id="69b8c-978">RDBMS</span></span>

* <span data-ttu-id="69b8c-979">Adicionar comandos de gerenciamento de chaves de criptografia de dados do servidor para PostgreSQL e MySQL</span><span class="sxs-lookup"><span data-stu-id="69b8c-979">Add server data encryption key management commands for PostgreSQL and MySQL</span></span>

## <a name="march-10-2020"></a><span data-ttu-id="69b8c-980">10 de março de 2020</span><span class="sxs-lookup"><span data-stu-id="69b8c-980">March 10, 2020</span></span>

<span data-ttu-id="69b8c-981">Versão 2.2.0</span><span class="sxs-lookup"><span data-stu-id="69b8c-981">Version 2.2.0</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-982">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-982">ACR</span></span>

* <span data-ttu-id="69b8c-983">Correção: `az acr login` gerava erro incorretamente</span><span class="sxs-lookup"><span data-stu-id="69b8c-983">Fix: `az acr login` wrongly raise error</span></span>
* <span data-ttu-id="69b8c-984">Adicionou o novo comando `az acr helm install-cli`</span><span class="sxs-lookup"><span data-stu-id="69b8c-984">Add new command `az acr helm install-cli`</span></span>
* <span data-ttu-id="69b8c-985">Adicionou link privado e suporte do CMK</span><span class="sxs-lookup"><span data-stu-id="69b8c-985">Add private link and CMK support</span></span>
* <span data-ttu-id="69b8c-986">Adicionou o comando 'private-link-resource list'</span><span class="sxs-lookup"><span data-stu-id="69b8c-986">add 'private-link-resource list' command</span></span>

### <a name="aks"></a><span data-ttu-id="69b8c-987">AKS</span><span class="sxs-lookup"><span data-stu-id="69b8c-987">AKS</span></span>

* <span data-ttu-id="69b8c-988">correção da busca do AKS no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="69b8c-988">fix the aks browse in cloud shell</span></span>
* <span data-ttu-id="69b8c-989">az aks: correção dos erros de complemento de monitoramento e de agentpool NoneType</span><span class="sxs-lookup"><span data-stu-id="69b8c-989">az aks: Fix monitoring addon and agentpool NoneType errors</span></span>
* <span data-ttu-id="69b8c-990">Adicionou --nodepool-tags ao pool de nós ao criar o cluster do Kubernetes do Azure</span><span class="sxs-lookup"><span data-stu-id="69b8c-990">Add --nodepool-tags to node pool when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="69b8c-991">Adicionou --tags ao adicionar ou atualizar um pool de nós para o cluster</span><span class="sxs-lookup"><span data-stu-id="69b8c-991">Add --tags when adding or updating a nodepool to cluster</span></span>
* <span data-ttu-id="69b8c-992">AKS create: adicionou `--enable-private-cluster`</span><span class="sxs-lookup"><span data-stu-id="69b8c-992">aks create: add `--enable-private-cluster`</span></span>
* <span data-ttu-id="69b8c-993">Adicionou --nodepool-labels ao criar o cluster do Kubernetes do Azure</span><span class="sxs-lookup"><span data-stu-id="69b8c-993">add --nodepool-labels when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="69b8c-994">Adicionou --labels ao adicionar um novo pool de nós ao cluster do Kubernetes do Azure</span><span class="sxs-lookup"><span data-stu-id="69b8c-994">add --labels when adding a new nodepool to azure kubernetes cluster</span></span>
* <span data-ttu-id="69b8c-995">Adicionou / ausente na URL do painel</span><span class="sxs-lookup"><span data-stu-id="69b8c-995">add missing / in the dashboard url</span></span>
* <span data-ttu-id="69b8c-996">Suporte para criar clusters do AKS habilitando identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="69b8c-996">Support create aks clusters enabling managed identity</span></span>
* <span data-ttu-id="69b8c-997">az aks: validou o plug-in de rede como "Azure" ou "Kubenet"</span><span class="sxs-lookup"><span data-stu-id="69b8c-997">az aks: Validate network plugin to be either "azure" or "kubenet"</span></span>
* <span data-ttu-id="69b8c-998">az aks: adicionou suporte da chave da sessão do AAD</span><span class="sxs-lookup"><span data-stu-id="69b8c-998">az aks: Add aad session key support</span></span>
* <span data-ttu-id="69b8c-999">[ALTERAÇÃO SIGNIFICATIVA] AZ AKS: suporte para alterações de MSI para GF e BF para omsagent (Monitoramento de contêiner) (#1)</span><span class="sxs-lookup"><span data-stu-id="69b8c-999">[BREAKING CHANGE] az aks: support msi changes for GF and BF for omsagent (Container monitoring)(#1)</span></span>
* <span data-ttu-id="69b8c-1000">az aks use-dev-spaces: adicionou a opção de tipo de ponto de extremidade ao comando use-dev-spaces para personalizar o ponto de extremidade criado em um controlador Azure Dev Spaces</span><span class="sxs-lookup"><span data-stu-id="69b8c-1000">az aks use-dev-spaces: Adding endpoint type option to the use-dev-spaces command to customize the endpoint created on an Azure Dev Spaces controller</span></span>

### <a name="appconfig"></a><span data-ttu-id="69b8c-1001">AppConfig</span><span class="sxs-lookup"><span data-stu-id="69b8c-1001">AppConfig</span></span>

* <span data-ttu-id="69b8c-1002">Desbloqueou usando "KV set" para adicionar o recurso e a referência do keyvault...</span><span class="sxs-lookup"><span data-stu-id="69b8c-1002">Unblock using "kv set" to add keyvault reference and feature …</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-1003">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-1003">AppService</span></span>

* <span data-ttu-id="69b8c-1004">az webapp create: correção do problema ao executar o comando com --runtime</span><span class="sxs-lookup"><span data-stu-id="69b8c-1004">az webapp create : Fix issue when running the command with --runtime</span></span>
* <span data-ttu-id="69b8c-1005">az functionapp deployment source config-zip: adicionou uma mensagem de erro se o grupo de recursos ou o nome da função forem inválidos/não existirem</span><span class="sxs-lookup"><span data-stu-id="69b8c-1005">az functionapp deployment source config-zip: Add an error message if resource group or function name are invalid/don't exist</span></span>
* <span data-ttu-id="69b8c-1006">functionapp create: correção da mensagem de aviso que aparece com `functionapp create` hoje, que cita um sinalizador de `--functions_version`, mas usa erroneamente `_` em vez de `-` no nome do sinalizador</span><span class="sxs-lookup"><span data-stu-id="69b8c-1006">functionapp create: Fix the warning message that appears with `functionapp create` today which cites a `--functions_version` flag but erroneously uses a `_` instead of a `-` in the flag name</span></span>
* <span data-ttu-id="69b8c-1007">az functionapp create: atualizou o modo como linuxFxVersion e o nome da imagem de contêiner eram definidos para aplicativos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="69b8c-1007">az functionapp create: Updated the way linuxFxVersion and container image name were being set for linux function apps</span></span>
* <span data-ttu-id="69b8c-1008">az functionapp deployment source config-zip: correção de um problema causado pelas configurações do aplicativo que alterava a condição de corrida durante a implantação do zip, provocando erros 5xx durante a implantação</span><span class="sxs-lookup"><span data-stu-id="69b8c-1008">az functionapp deployment source config-zip: Fix an issue caused by app settings change racing condition during zip deploy, giving 5xx errors during deployment</span></span>
* <span data-ttu-id="69b8c-1009">Correção #5720946: AZ WebApp backup falha ao definir o nome</span><span class="sxs-lookup"><span data-stu-id="69b8c-1009">Fix #5720946: az webapp backup fails to set name</span></span>

### <a name="arm"></a><span data-ttu-id="69b8c-1010">ARM</span><span class="sxs-lookup"><span data-stu-id="69b8c-1010">ARM</span></span>

* <span data-ttu-id="69b8c-1011">az resource: aprimorou os exemplos do módulo de recurso</span><span class="sxs-lookup"><span data-stu-id="69b8c-1011">az resource: Improve the examples of the resource module</span></span>
* <span data-ttu-id="69b8c-1012">az policy assignment list: suporte à listagem de atribuições de política no escopo do Grupo de Gerenciamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-1012">az policy assignment list: Support listing policy assignments at Management Group scope</span></span>
* <span data-ttu-id="69b8c-1013">Adicionou `az deployment group` e `az deployment operation group` para a implantação de modelos nos grupos de recursos.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1013">Add `az deployment group` and `az deployment operation group` for template deployment at resource groups.</span></span> <span data-ttu-id="69b8c-1014">Esta é uma duplicata de `az group deployment` e `az group deployment operation`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1014">This is a duplicate of `az group deployment` and `az group deployment operation`</span></span>
* <span data-ttu-id="69b8c-1015">Adicionou `az deployment sub` e `az deployment operation sub` para a implantação de modelos no escopo da assinatura.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1015">Add `az deployment sub` and `az deployment operation sub` for template deployment at subscription scope.</span></span> <span data-ttu-id="69b8c-1016">Esta é uma duplicata de `az deployment` e `az deployment operation`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1016">This is a duplicate of `az deployment` and `az deployment operation`</span></span>
* <span data-ttu-id="69b8c-1017">Adicionou `az deployment mg` e `az deployment operation mg` para implantação de modelos nos grupos de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1017">Add `az deployment mg` and `az deployment operation mg` for template deployment at management groups</span></span>
* <span data-ttu-id="69b8c-1018">Adicionou `az deployment tenant` e `az deployment operation tenant` para implantação de modelos no escopo do locatário.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1018">Add `az deployment tenant` and `az deployment operation tenant` for template deployment at tenant scope</span></span>
* <span data-ttu-id="69b8c-1019">az policy assignment create: adicionou descrição ao parâmetro `--location`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1019">az policy assignment create: Add a description to the `--location` parameter</span></span>
* <span data-ttu-id="69b8c-1020">az group deployment create: adicionou o parâmetro `--aux-tenants` para dar suporte a locatários cruzados</span><span class="sxs-lookup"><span data-stu-id="69b8c-1020">az group deployment create: Add parameter `--aux-tenants` to support cross tenants</span></span>

### <a name="cdn"></a><span data-ttu-id="69b8c-1021">CDN</span><span class="sxs-lookup"><span data-stu-id="69b8c-1021">CDN</span></span>

* <span data-ttu-id="69b8c-1022">Adicionou comandos do WAF da CDN</span><span class="sxs-lookup"><span data-stu-id="69b8c-1022">Add CDN WAF commands</span></span>

### <a name="compute"></a><span data-ttu-id="69b8c-1023">Computação</span><span class="sxs-lookup"><span data-stu-id="69b8c-1023">Compute</span></span>

* <span data-ttu-id="69b8c-1024">az sig image-version: adicionar --data-snapshot-luns</span><span class="sxs-lookup"><span data-stu-id="69b8c-1024">az sig image-version: add --data-snapshot-luns</span></span>
* <span data-ttu-id="69b8c-1025">AZ PPG show: adicionou --outlocation-status para habilitar a busca do status de colocalização de todos os recursos no grupo de posicionamento por proximidade</span><span class="sxs-lookup"><span data-stu-id="69b8c-1025">az ppg show: add --colocation-status to enable fetching the colocation status of all the resources in the proximity placement group</span></span>
* <span data-ttu-id="69b8c-1026">az vmss create/update: suporte a reparos automáticos</span><span class="sxs-lookup"><span data-stu-id="69b8c-1026">az vmss create/update: support automatic repairs</span></span>
* <span data-ttu-id="69b8c-1027">[ALTERAÇÃO SIGNIFICATIVA] modelo de imagem AZ: renomear modelo para builder</span><span class="sxs-lookup"><span data-stu-id="69b8c-1027">[BREAKING CHANGE] az image template: rename template to builder</span></span>
* <span data-ttu-id="69b8c-1028">AZ Image Builder Create: adicionou --Image-template</span><span class="sxs-lookup"><span data-stu-id="69b8c-1028">az image builder create: add --image-template</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="69b8c-1029">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="69b8c-1029">Cosmos DB</span></span>

* <span data-ttu-id="69b8c-1030">Adicionou procedimento armazenado do SQL, UDF e disparar cmdlets</span><span class="sxs-lookup"><span data-stu-id="69b8c-1030">Add Sql stored procedure, udf and trigger cmdlets</span></span>
* <span data-ttu-id="69b8c-1031">az cosmosdb create: adicionou --key-uri para dar suporte à adição de informações de criptografia do cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="69b8c-1031">az cosmosdb create: add --key-uri to support adding key vault encryption information</span></span>

### <a name="keyvault"></a><span data-ttu-id="69b8c-1032">KeyVault</span><span class="sxs-lookup"><span data-stu-id="69b8c-1032">KeyVault</span></span>

* <span data-ttu-id="69b8c-1033">keyvault create: habilitou a exclusão reversível por padrão</span><span class="sxs-lookup"><span data-stu-id="69b8c-1033">keyvault create: enable soft-delete by default</span></span>

### <a name="monitor"></a><span data-ttu-id="69b8c-1034">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="69b8c-1034">Monitor</span></span>

* <span data-ttu-id="69b8c-1035">az monitor metrics alert create: suporte a `~` em `--condition`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1035">az monitor metrics alert create: support `~` in `--condition`</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-1036">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-1036">Network</span></span>

* <span data-ttu-id="69b8c-1037">az network application-gateway rewrite-rule create: suporte à configuração de URL</span><span class="sxs-lookup"><span data-stu-id="69b8c-1037">az network application-gateway rewrite-rule create: support url configuration</span></span>
* <span data-ttu-id="69b8c-1038">az network dns zone import: --zone-name não diferenciará maiúsculas de minúsculas no futuro</span><span class="sxs-lookup"><span data-stu-id="69b8c-1038">az network dns zone import: --zone-name will be case insensitive in the future</span></span>
* <span data-ttu-id="69b8c-1039">az network private-endpoint/private-link-service: removeu rótulo de visualização</span><span class="sxs-lookup"><span data-stu-id="69b8c-1039">az network private-endpoint/private-link-service: remove preview label</span></span>
* <span data-ttu-id="69b8c-1040">az network bastion: suporte a bastions</span><span class="sxs-lookup"><span data-stu-id="69b8c-1040">az network bastion: support bastion</span></span>
* <span data-ttu-id="69b8c-1041">az network vnet list-available-ips: dar suporte à lista de IPs disponíveis em uma vnet</span><span class="sxs-lookup"><span data-stu-id="69b8c-1041">az network vnet list-available-ips: support list available ips in a vnet</span></span>
* <span data-ttu-id="69b8c-1042">az network watcher flow-log create/list/delete/update: adicionou novos comandos para gerenciar o log de fluxo do Inspetor e expor o --local para identificá-lo explicitamente</span><span class="sxs-lookup"><span data-stu-id="69b8c-1042">az network watcher flow-log create/list/delete/update: add new commands to manage watcher flow log and exposing --location to identify watcher explicitly</span></span>
* <span data-ttu-id="69b8c-1043">az network watcher flow-log configure: preterido</span><span class="sxs-lookup"><span data-stu-id="69b8c-1043">az network watcher flow-log configure: deprecated</span></span>
* <span data-ttu-id="69b8c-1044">az network watcher flow-log show: dá suporte a --location e --name para obter o resultado formatado por ARM, saída formatada antiga preterida</span><span class="sxs-lookup"><span data-stu-id="69b8c-1044">az network watcher flow-log show: support --location and --name to get ARM-formatted result, deprecated old formatted output</span></span>

### <a name="policy"></a><span data-ttu-id="69b8c-1045">Política</span><span class="sxs-lookup"><span data-stu-id="69b8c-1045">Policy</span></span>

* <span data-ttu-id="69b8c-1046">az policy assignment create: correção do bug que gerou automaticamente o nome da atribuição de política, que excede o limite</span><span class="sxs-lookup"><span data-stu-id="69b8c-1046">az policy assignment create: Fix the bug that automatically generated name of policy assignment exceeds the limit</span></span>

### <a name="rbac"></a><span data-ttu-id="69b8c-1047">RBAC</span><span class="sxs-lookup"><span data-stu-id="69b8c-1047">RBAC</span></span>

* <span data-ttu-id="69b8c-1048">az ad group show: correção do valor --group, que é tratado como um problema de regex</span><span class="sxs-lookup"><span data-stu-id="69b8c-1048">az ad group show: fix --group value treated as regex problem</span></span>

### <a name="rdbms"></a><span data-ttu-id="69b8c-1049">RDBMS</span><span class="sxs-lookup"><span data-stu-id="69b8c-1049">RDBMS</span></span>

* <span data-ttu-id="69b8c-1050">Trocou a versão do zure-mgmt-rdbms SDK para 2.0.0</span><span class="sxs-lookup"><span data-stu-id="69b8c-1050">Bump the azure-mgmt-rdbms SDK version to 2.0.0</span></span>
* <span data-ttu-id="69b8c-1051">az postgres private-endpoint-connection: gerenciou conexões de ponto de extremidade privado do Postgres</span><span class="sxs-lookup"><span data-stu-id="69b8c-1051">az postgres private-endpoint-connection: manage postgres private endpoint connections</span></span>
* <span data-ttu-id="69b8c-1052">az postgres private-link-resource: gerenciou recursos de link privado do Postgres</span><span class="sxs-lookup"><span data-stu-id="69b8c-1052">az postgres private-link-resource: manage postgres private link resources</span></span>
* <span data-ttu-id="69b8c-1053">az mysql private-endpoint-connection: gerenciar conexões de ponto de extremidade privado do MySQL</span><span class="sxs-lookup"><span data-stu-id="69b8c-1053">az mysql private-endpoint-connection: manage mysql private endpoint connections</span></span>
* <span data-ttu-id="69b8c-1054">az mysql private-link-resource: gerenciou recursos de link privado do MySQL</span><span class="sxs-lookup"><span data-stu-id="69b8c-1054">az mysql private-link-resource: manage mysql private link resources</span></span>
* <span data-ttu-id="69b8c-1055">az mariadb private-endpoint-connection: gerenciou conexões de ponto de extremidade privado do MariaDB</span><span class="sxs-lookup"><span data-stu-id="69b8c-1055">az mariadb private-endpoint-connection: manage mariadb private endpoint connections</span></span>
* <span data-ttu-id="69b8c-1056">az mariadb private-link-resource: gerenciou recursos de link privado do MariaDB</span><span class="sxs-lookup"><span data-stu-id="69b8c-1056">az mariadb private-link-resource: manage mariadb private link resources</span></span>
* <span data-ttu-id="69b8c-1057">Atualizando testes de ponto de extremidade privado do RDBMS</span><span class="sxs-lookup"><span data-stu-id="69b8c-1057">Updating RDBMS Private Endpoint Tests</span></span>

### <a name="sql"></a><span data-ttu-id="69b8c-1058">SQL</span><span class="sxs-lookup"><span data-stu-id="69b8c-1058">SQL</span></span>

* <span data-ttu-id="69b8c-1059">Sql midb Add: list-deleted, show-deleted, update-retention, show-retention</span><span class="sxs-lookup"><span data-stu-id="69b8c-1059">Sql midb Add: list-deleted, show-deleted, update-retention, show-retention</span></span>
* <span data-ttu-id="69b8c-1060">(sql server create:) adicionou o sinalizador ' habilitar '/' desabilitar ' opcional public-network-access ao SQL Server create</span><span class="sxs-lookup"><span data-stu-id="69b8c-1060">(sql server create:) Add optional public-network-access 'Enable'/'Disable' flag to sql server create</span></span>
* <span data-ttu-id="69b8c-1061">(sql server update:) fez algumas alterações voltadas para o cliente</span><span class="sxs-lookup"><span data-stu-id="69b8c-1061">(sql server update:) make some customer-facing change</span></span>
* <span data-ttu-id="69b8c-1062">adicionou a propriedade minimal_tls_version para o banco de BD de MI e SQL</span><span class="sxs-lookup"><span data-stu-id="69b8c-1062">Add minimal_tls_version property for MI and SQL DB</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-1063">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-1063">Storage</span></span>

* <span data-ttu-id="69b8c-1064">az storage blob delete-batch: sinalizador `--dryrun` de comportamento inadequado</span><span class="sxs-lookup"><span data-stu-id="69b8c-1064">az storage blob delete-batch: Misbehaving `--dryrun` flag</span></span>
* <span data-ttu-id="69b8c-1065">az storage account network-rule add (correção de bug): a operação de adição deve ser idempotente</span><span class="sxs-lookup"><span data-stu-id="69b8c-1065">az storage account network-rule add (bug fix): add operation should be idempotent</span></span>
* <span data-ttu-id="69b8c-1066">az storage account create/update: Adicionou suporte de preferência de roteamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-1066">az storage account create/update: Add Routing Preference support</span></span>
* <span data-ttu-id="69b8c-1067">Atualizou a versão do azure-mgmt-storage para 8.0.0</span><span class="sxs-lookup"><span data-stu-id="69b8c-1067">Upgrade azure-mgmt-storage version to 8.0.0</span></span>
* <span data-ttu-id="69b8c-1068">az storage container immutability create: adicionou o parâmetro --allow-protected-append-write</span><span class="sxs-lookup"><span data-stu-id="69b8c-1068">az storage container immutability create: add --allow-protected-append-write parameter</span></span>
* <span data-ttu-id="69b8c-1069">az storage account private-link-resource list: Adicionou suporte para lista de recursos de link privado para a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-1069">az storage account private-link-resource list: Add support to list private link resources for storage account</span></span>
* <span data-ttu-id="69b8c-1070">az storage account private-endpoint-connection approve/reject/show/delete: Suporte para gerenciar conexões de ponto de extremidade privado</span><span class="sxs-lookup"><span data-stu-id="69b8c-1070">az storage account private-endpoint-connection approve/reject/show/delete: Support to manage private endpoint connections</span></span>
* <span data-ttu-id="69b8c-1071">az storage account blob-service-properties update: adicionou --enable-restore-policy e --restore-days</span><span class="sxs-lookup"><span data-stu-id="69b8c-1071">az storage account blob-service-properties update: add --enable-restore-policy and --restore-days</span></span>
* <span data-ttu-id="69b8c-1072">az storage blob restore: adicionou suporte para restaurar intervalos de blob</span><span class="sxs-lookup"><span data-stu-id="69b8c-1072">az storage blob restore: Add support to restore blob ranges</span></span>

## <a name="february-18-2020"></a><span data-ttu-id="69b8c-1073">18 de fevereiro de 2020</span><span class="sxs-lookup"><span data-stu-id="69b8c-1073">February 18, 2020</span></span>

<span data-ttu-id="69b8c-1074">Versão 2.1.0</span><span class="sxs-lookup"><span data-stu-id="69b8c-1074">Version 2.1.0</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-1075">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-1075">ACR</span></span>

* <span data-ttu-id="69b8c-1076">Adicionar um novo argumento `--expose-token` a `az acr login`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1076">Add a new argument `--expose-token` for `az acr login`</span></span>
* <span data-ttu-id="69b8c-1077">Corrigir a saída incorreta de `az acr task identity show -n Name -r Registry -o table`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1077">Fix the incorrect output of `az acr task identity show -n Name -r Registry -o table`</span></span>
* <span data-ttu-id="69b8c-1078">az acr login: Gerar CLIError se erros forem retornados pelo comando docker</span><span class="sxs-lookup"><span data-stu-id="69b8c-1078">az acr login: Throw a CLIError if there are errors returned by docker command</span></span>

### <a name="acs"></a><span data-ttu-id="69b8c-1079">ACS</span><span class="sxs-lookup"><span data-stu-id="69b8c-1079">ACS</span></span>

* <span data-ttu-id="69b8c-1080">aks create/update: adicionar a validação `--vnet-subnet-id`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1080">aks create/update: add `--vnet-subnet-id` validation</span></span>

### <a name="aladdin"></a><span data-ttu-id="69b8c-1081">Aladdin</span><span class="sxs-lookup"><span data-stu-id="69b8c-1081">Aladdin</span></span>

* <span data-ttu-id="69b8c-1082">Analisar os exemplos gerados no _help.py do comando</span><span class="sxs-lookup"><span data-stu-id="69b8c-1082">Parse generated examples into commands' _help.py</span></span>

### <a name="ams"></a><span data-ttu-id="69b8c-1083">AMS</span><span class="sxs-lookup"><span data-stu-id="69b8c-1083">AMS</span></span>

* <span data-ttu-id="69b8c-1084">az ams já está em GA</span><span class="sxs-lookup"><span data-stu-id="69b8c-1084">az ams is GA now</span></span>

### <a name="appconfig"></a><span data-ttu-id="69b8c-1085">AppConfig</span><span class="sxs-lookup"><span data-stu-id="69b8c-1085">AppConfig</span></span>

* <span data-ttu-id="69b8c-1086">Revisar a mensagem de ajuda para excluir o filtro de chave/rótulo não compatível</span><span class="sxs-lookup"><span data-stu-id="69b8c-1086">Revise help message to exclude unsupported key/label filter</span></span>
* <span data-ttu-id="69b8c-1087">Remover a marca de versão prévia da maioria dos comandos que excluem a identidade gerenciada e têm sinalizadores</span><span class="sxs-lookup"><span data-stu-id="69b8c-1087">Remove preview tag for most commands excluding managed identity and feature flags</span></span>
* <span data-ttu-id="69b8c-1088">Adicionar a chave gerenciada do cliente ao atualizar os repositórios</span><span class="sxs-lookup"><span data-stu-id="69b8c-1088">Add customer managed key when updating stores</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-1089">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-1089">AppService</span></span>

* <span data-ttu-id="69b8c-1090">az webapp list-runtimes: Corrigir o bug de list-runtimes</span><span class="sxs-lookup"><span data-stu-id="69b8c-1090">az webapp list-runtimes: Fix the bug for list-runtimes</span></span>
* <span data-ttu-id="69b8c-1091">Adicionar az webapp|functionapp config ssl create</span><span class="sxs-lookup"><span data-stu-id="69b8c-1091">Add az webapp|functionapp config ssl create</span></span>
* <span data-ttu-id="69b8c-1092">Adicionar compatibilidade com aplicativos de funções v3 e nó 12</span><span class="sxs-lookup"><span data-stu-id="69b8c-1092">Add support for v3 function apps and node 12</span></span>

### <a name="arm"></a><span data-ttu-id="69b8c-1093">ARM</span><span class="sxs-lookup"><span data-stu-id="69b8c-1093">ARM</span></span>

* <span data-ttu-id="69b8c-1094">az policy assignment create: Corrigir a mensagem de erro quando o parâmetro `--policy` for inválido</span><span class="sxs-lookup"><span data-stu-id="69b8c-1094">az policy assignment create: Fix the error message when the `--policy` parameter is invalid</span></span>
* <span data-ttu-id="69b8c-1095">az group deployment create: Corrigir o erro "stat: o caminho é muito longo para o Windows" ao usar o arquivo grande parameters.json</span><span class="sxs-lookup"><span data-stu-id="69b8c-1095">az group deployment create: Fix "stat: path too long for Windows" error when using large parameters.json file</span></span>

### <a name="backup"></a><span data-ttu-id="69b8c-1096">Backup</span><span class="sxs-lookup"><span data-stu-id="69b8c-1096">Backup</span></span>

* <span data-ttu-id="69b8c-1097">Corrigir o fluxo de recuperação de nível de item no OLR</span><span class="sxs-lookup"><span data-stu-id="69b8c-1097">Fix for item level recovery flow in OLR</span></span>
* <span data-ttu-id="69b8c-1098">Adicionar compatibilidade com restauração como arquivo aos bancos de dados SQL e SAP</span><span class="sxs-lookup"><span data-stu-id="69b8c-1098">Add restore as files support for SQL and SAP Databases</span></span>

### <a name="compute"></a><span data-ttu-id="69b8c-1099">Computação</span><span class="sxs-lookup"><span data-stu-id="69b8c-1099">Compute</span></span>

* <span data-ttu-id="69b8c-1100">vm/vmss/availability-set update: adicionar --ppg para permitir a atualização de ProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="69b8c-1100">vm/vmss/availability-set update: add --ppg to allowing updating ProximityPlacementGroup</span></span>
* <span data-ttu-id="69b8c-1101">vmss create: adicionar --data-disk-iops e --data-disk-mbps</span><span class="sxs-lookup"><span data-stu-id="69b8c-1101">vmss create: add --data-disk-iops and --data-disk-mbps</span></span>
* <span data-ttu-id="69b8c-1102">az vm host: remover a marca de versão prévia de `vm host` e `vm host group`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1102">az vm host: remove preview tag for `vm host` and `vm host group`</span></span>
* <span data-ttu-id="69b8c-1103">[ALTERAÇÃO SIGNIFICATIVA] Correção nº 10.728: `az vm create`: criar uma sub-rede automaticamente quando a vnet for especificada e não houver uma sub-rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-1103">[BREAKING CHANGE] Fix #10728: `az vm create`: create subnet automatically if vnet is specified and subnet not exists</span></span>
* <span data-ttu-id="69b8c-1104">Aumentar a robustez da lista de imagens de VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-1104">Increase robustness of vm image list</span></span>

### <a name="eventhub"></a><span data-ttu-id="69b8c-1105">Eventhub</span><span class="sxs-lookup"><span data-stu-id="69b8c-1105">Eventhub</span></span>

* <span data-ttu-id="69b8c-1106">Compatibilidade com o Azure Stack para o perfil 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="69b8c-1106">Azure Stack support for 2019-03-01-hybrid profile</span></span>

### <a name="keyvault"></a><span data-ttu-id="69b8c-1107">KeyVault</span><span class="sxs-lookup"><span data-stu-id="69b8c-1107">KeyVault</span></span>

* <span data-ttu-id="69b8c-1108">az keyvault key create: adicionar um novo valor `import` ao parâmetro `--ops`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1108">az keyvault key create: add a new value `import` for parameter `--ops`</span></span>
* <span data-ttu-id="69b8c-1109">az keyvault key list-versions: compatibilidade com o parâmetro `--id` para especificar chaves</span><span class="sxs-lookup"><span data-stu-id="69b8c-1109">az keyvault key list-versions: support parameter `--id` for specifying keys</span></span>
* <span data-ttu-id="69b8c-1110">Compatibilidade com conexões de ponto de extremidade privado</span><span class="sxs-lookup"><span data-stu-id="69b8c-1110">Support private endpoint connections</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-1111">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-1111">Network</span></span>

* <span data-ttu-id="69b8c-1112">Avançar para azure-mgmt-network 9.0.0</span><span class="sxs-lookup"><span data-stu-id="69b8c-1112">Bump to azure-mgmt-network 9.0.0</span></span>
* <span data-ttu-id="69b8c-1113">az network private-link-service update/create: dá suporte a --enable-proxy-protocol</span><span class="sxs-lookup"><span data-stu-id="69b8c-1113">az network private-link-service update/create: support --enable-proxy-protocol</span></span>
* <span data-ttu-id="69b8c-1114">Adicionar o recurso de Monitor de conexão V2</span><span class="sxs-lookup"><span data-stu-id="69b8c-1114">Add connection Monitor V2 feature</span></span>

### <a name="packaging"></a><span data-ttu-id="69b8c-1115">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-1115">Packaging</span></span>

* <span data-ttu-id="69b8c-1116">[ALTERAÇÃO SIGNIFICATIVA] Fim da compatibilidade com o Python 2.7</span><span class="sxs-lookup"><span data-stu-id="69b8c-1116">[BREAKING CHANGE] Drop support for Python 2.7</span></span>

### <a name="profile"></a><span data-ttu-id="69b8c-1117">Perfil</span><span class="sxs-lookup"><span data-stu-id="69b8c-1117">Profile</span></span>

* <span data-ttu-id="69b8c-1118">Visualização: Adicionar novos atributos `homeTenantId` e `managedByTenants` às contas de assinatura.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1118">Preview: Add new attributes `homeTenantId` and `managedByTenants` to subscription accounts.</span></span> <span data-ttu-id="69b8c-1119">Executar `az login` novamente para as alterações entrarem em vigor</span><span class="sxs-lookup"><span data-stu-id="69b8c-1119">Please re-run `az login` for the changes to take effect</span></span>
* <span data-ttu-id="69b8c-1120">az login: Mostrar um aviso quando uma assinatura estiver listada de mais de um locatário e definir a primeira como padrão.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1120">az login: Show a warning when a subscription is listed from more than one tenants and default to the first one.</span></span> <span data-ttu-id="69b8c-1121">Para selecionar um locatário específico ao acessar essa assinatura, inclua `--tenant` em `az login`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1121">To select a specific tenant when accessing this subscription, please include `--tenant` in `az login`</span></span>

### <a name="role"></a><span data-ttu-id="69b8c-1122">Função</span><span class="sxs-lookup"><span data-stu-id="69b8c-1122">Role</span></span>

* <span data-ttu-id="69b8c-1123">az role assignment create: Corrigir o erro em que atribuir uma função a uma entidade de serviço pelo nome de exibição gera um HTTP 400</span><span class="sxs-lookup"><span data-stu-id="69b8c-1123">az role assignment create: Fix the error that assigning a role to a service principal by display name yields a HTTP 400</span></span>

### <a name="sql"></a><span data-ttu-id="69b8c-1124">SQL</span><span class="sxs-lookup"><span data-stu-id="69b8c-1124">SQL</span></span>

* <span data-ttu-id="69b8c-1125">Atualizar o cmdlet da Instância Gerenciada do SQL `az sql mi update` com dois novos parâmetros: nível e família</span><span class="sxs-lookup"><span data-stu-id="69b8c-1125">Update SQL Managed Instance cmdlet `az sql mi update` with two new parameters: tier and family</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-1126">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-1126">Storage</span></span>

* <span data-ttu-id="69b8c-1127">[ALTERAÇÃO DA FALHA] `az storage account create`: Alterar o tipo de conta de armazenamento padrão para StorageV2</span><span class="sxs-lookup"><span data-stu-id="69b8c-1127">[BREAKING CHANGE] `az storage account create`: Change default storage account kind to StorageV2</span></span>

## <a name="february-04-2020"></a><span data-ttu-id="69b8c-1128">4 de fevereiro de 2020</span><span class="sxs-lookup"><span data-stu-id="69b8c-1128">February 04, 2020</span></span>

<span data-ttu-id="69b8c-1129">Versão 2.0.81</span><span class="sxs-lookup"><span data-stu-id="69b8c-1129">Version 2.0.81</span></span>

### <a name="acs"></a><span data-ttu-id="69b8c-1130">ACS</span><span class="sxs-lookup"><span data-stu-id="69b8c-1130">ACS</span></span>

* <span data-ttu-id="69b8c-1131">Adicionar suporte para definir portas alocadas de saída e tempos limite ociosos no balanceador de carga standard</span><span class="sxs-lookup"><span data-stu-id="69b8c-1131">Add support to set outbound allocated ports and idle timeouts on standard load balancer</span></span>
* <span data-ttu-id="69b8c-1132">Atualizar para a versão da API 2019-11-01</span><span class="sxs-lookup"><span data-stu-id="69b8c-1132">Update to API Version 2019-11-01</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-1133">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-1133">ACR</span></span>

* <span data-ttu-id="69b8c-1134">A [ALTERAÇÃO DA FALHA] `az acr delete` será exibida</span><span class="sxs-lookup"><span data-stu-id="69b8c-1134">[BREAKING CHANGE] `az acr delete` will prompt</span></span>
* <span data-ttu-id="69b8c-1135">A [ALTERAÇÃO SIGNIFICATIVA] 'az acr task delete’ será exibida</span><span class="sxs-lookup"><span data-stu-id="69b8c-1135">[BREAKING CHANGE] 'az acr task delete' will prompt</span></span>
* <span data-ttu-id="69b8c-1136">Adicionar um novo grupo de comandos ‘az acr taskrun show/list/delete’ para o gerenciamento de taskrun</span><span class="sxs-lookup"><span data-stu-id="69b8c-1136">Add a new command group 'az acr taskrun show/list/delete' for taskrun management</span></span>

### <a name="aks"></a><span data-ttu-id="69b8c-1137">AKS</span><span class="sxs-lookup"><span data-stu-id="69b8c-1137">AKS</span></span>

* <span data-ttu-id="69b8c-1138">Cada cluster obtém uma entidade de serviço separada para aprimorar o isolamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-1138">Each cluster gets a separate service principal to improve isolation</span></span>

### <a name="appconfig"></a><span data-ttu-id="69b8c-1139">AppConfig</span><span class="sxs-lookup"><span data-stu-id="69b8c-1139">AppConfig</span></span>

* <span data-ttu-id="69b8c-1140">Dar suporte à importação/exportação de referências keyvault de/a appservice</span><span class="sxs-lookup"><span data-stu-id="69b8c-1140">Support import/export of keyvault references from/to appservice</span></span>
* <span data-ttu-id="69b8c-1141">Dar suporte à importação/exportação de todos os rótulos de appconfig para appconfig</span><span class="sxs-lookup"><span data-stu-id="69b8c-1141">Support import/export of all labels from appconfig to appconfig</span></span>
* <span data-ttu-id="69b8c-1142">Validar nomes de chave e recursos antes de configurar e importar</span><span class="sxs-lookup"><span data-stu-id="69b8c-1142">Validate key and feature names before setting and importing</span></span>
* <span data-ttu-id="69b8c-1143">Exponha a modificação do sku para o repositório de configurações.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1143">Expose sku modification for configuration store.</span></span>
* <span data-ttu-id="69b8c-1144">Adicione o grupo de comandos à identidade gerenciada.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1144">Add command group for managed identity.</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-1145">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-1145">AppService</span></span>

* <span data-ttu-id="69b8c-1146">Azure Stack: comandos de superfície no perfil de 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="69b8c-1146">Azure Stack: surface commands under the profile of 2019-03-01-hybrid</span></span>
* <span data-ttu-id="69b8c-1147">functionapp: adicionar a capacidade de criar aplicativos de funções Java no Linux</span><span class="sxs-lookup"><span data-stu-id="69b8c-1147">functionapp: Add ability to create Java function apps in Linux</span></span>

### <a name="arm"></a><span data-ttu-id="69b8c-1148">ARM</span><span class="sxs-lookup"><span data-stu-id="69b8c-1148">ARM</span></span>

* <span data-ttu-id="69b8c-1149">Correção de problema nº 10246: `az resource tag` falha quando o parâmetro `--ids` passado é a ID do grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="69b8c-1149">Fix issue #10246: `az resource tag` crashes when the parameter `--ids` passed in is resource group ID</span></span>
* <span data-ttu-id="69b8c-1150">Correção de problema nº 11658: o comando `az group export` não é compatível com os parâmetros `--query` e `--output`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1150">Fix issue #11658: `az group export` command does not support `--query` and `--output` parameters</span></span>
* <span data-ttu-id="69b8c-1151">Correção de problema nº 10279: O código de saída `az group deployment validate` é 0 quando a verificação falha</span><span class="sxs-lookup"><span data-stu-id="69b8c-1151">Fix issue #10279: The exit code of `az group deployment validate` is 0 when the verification fails</span></span>
* <span data-ttu-id="69b8c-1152">Correção de problema nº 9916: aprimorar a mensagem de erro do conflito entre a marca e outras condições de filtro para o comando `az resource list`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1152">Fix issue #9916: Improve the error message of the conflict between tag and other filter conditions for `az resource list` command</span></span>
* <span data-ttu-id="69b8c-1153">Adicionar novo parâmetro `--managed-by` para dar suporte à adição de informações managedBy para o comando `az group create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1153">Add new parameter `--managed-by` to support adding managedBy information for command `az group create`</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="69b8c-1154">Red Hat OpenShift no Azure</span><span class="sxs-lookup"><span data-stu-id="69b8c-1154">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="69b8c-1155">Adicionar o subgrupo `monitor` para gerenciar o monitoramento do Log Analytics no cluster do Red Hat OpensShift no Azure</span><span class="sxs-lookup"><span data-stu-id="69b8c-1155">Add `monitor` subgroup to manage Log Analytics monitoring in Azure Red Hat OpensShift cluster</span></span>

### <a name="botservice"></a><span data-ttu-id="69b8c-1156">BotService</span><span class="sxs-lookup"><span data-stu-id="69b8c-1156">BotService</span></span>

* <span data-ttu-id="69b8c-1157">Correção de problema nº 11697: `az bot create` não é idempotente</span><span class="sxs-lookup"><span data-stu-id="69b8c-1157">Fix issue #11697: `az bot create` is not idempotent</span></span>
* <span data-ttu-id="69b8c-1158">Alterar testes de correção de nomes para serem executados somente em modo Ao vivo</span><span class="sxs-lookup"><span data-stu-id="69b8c-1158">Change name-correcting tests to run in Live-mode only</span></span>

### <a name="cdn"></a><span data-ttu-id="69b8c-1159">CDN</span><span class="sxs-lookup"><span data-stu-id="69b8c-1159">CDN</span></span>

* <span data-ttu-id="69b8c-1160">Adicionar suporte ao recurso rulesEngine</span><span class="sxs-lookup"><span data-stu-id="69b8c-1160">Add support for rulesEngine feature</span></span>
* <span data-ttu-id="69b8c-1161">Adicionar o novo grupo de comandos ‘cdn endpoint rule’ para gerenciar regras</span><span class="sxs-lookup"><span data-stu-id="69b8c-1161">Add new commands group 'cdn endpoint rule' to manage rules</span></span>
* <span data-ttu-id="69b8c-1162">Atualizar a versão azure-mgmt-cdn para a 4.0.0 para usar a versão da API 2019-04-15</span><span class="sxs-lookup"><span data-stu-id="69b8c-1162">Update azure-mgmt-cdn version to 4.0.0 to use api version 2019-04-15</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="69b8c-1163">Gerenciador de Implantação</span><span class="sxs-lookup"><span data-stu-id="69b8c-1163">Deployment Manager</span></span>

* <span data-ttu-id="69b8c-1164">Adicione a operação de lista para todos os recursos.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1164">Add list operation for all resources.</span></span>
* <span data-ttu-id="69b8c-1165">Aprimore o recurso de etapa do novo tipo de etapa.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1165">Enhance step resource for new step type.</span></span>
* <span data-ttu-id="69b8c-1166">Atualize o pacote azure-mgmt-deploymentmanager para usar a versão 0.2.0.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1166">Update azure-mgmt-deploymentmanager package to use version 0.2.0.</span></span>

### <a name="iot"></a><span data-ttu-id="69b8c-1167">IoT</span><span class="sxs-lookup"><span data-stu-id="69b8c-1167">IoT</span></span>

* <span data-ttu-id="69b8c-1168">Substitua os comandos ‘IoT hub Job’.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1168">Deprecate 'IoT hub Job' commands.</span></span>

### <a name="iot-central"></a><span data-ttu-id="69b8c-1169">Central da IoT</span><span class="sxs-lookup"><span data-stu-id="69b8c-1169">IoT Central</span></span>

* <span data-ttu-id="69b8c-1170">Dê suporte à atualização/criação de aplicativos com o novo nome do SKU ST0, ST1, ST2.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1170">Support app creation/update with the new sku name ST0, ST1, ST2.</span></span>

### <a name="key-vault"></a><span data-ttu-id="69b8c-1171">Key Vault</span><span class="sxs-lookup"><span data-stu-id="69b8c-1171">Key Vault</span></span>

* <span data-ttu-id="69b8c-1172">Adicione um novo comando `az keyvault key download` para baixar chaves.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1172">Add a new command `az keyvault key download` for downloading keys.</span></span>

### <a name="misc"></a><span data-ttu-id="69b8c-1173">Diversos</span><span class="sxs-lookup"><span data-stu-id="69b8c-1173">Misc</span></span>

* <span data-ttu-id="69b8c-1174">Correção nº 6371: dar suporte à conclusão da variável de nome de arquivo e de ambiente em Bash</span><span class="sxs-lookup"><span data-stu-id="69b8c-1174">Fix #6371: Support filename and environment variable completion in Bash</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-1175">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-1175">Network</span></span>

* <span data-ttu-id="69b8c-1176">Correção nº 2092: az network dns record-set add/remove: adicione um aviso quando record-set não é encontrado.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1176">Fix #2092: az network dns record-set add/remove: add warning when record-set is not found.</span></span> <span data-ttu-id="69b8c-1177">No futuro, haverá suporte para um argumento extra para confirmar essa criação automática.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1177">In the future, an extra argument will be supported to confirm this auto creation.</span></span>

### <a name="policy"></a><span data-ttu-id="69b8c-1178">Política</span><span class="sxs-lookup"><span data-stu-id="69b8c-1178">Policy</span></span>

* <span data-ttu-id="69b8c-1179">Adicionar o novo comando `az policy metadata` para recuperar recursos avançados de metadados de política</span><span class="sxs-lookup"><span data-stu-id="69b8c-1179">Add new command `az policy metadata` to retrieve rich policy metadata resources</span></span>
* <span data-ttu-id="69b8c-1180">`az policy remediation create`: Especifique se a conformidade deve ser reavaliada antes da correção com o parâmetro `--resource-discovery-mode`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1180">`az policy remediation create`: Specify whether compliance should be re-evaluated prior to remediation with the `--resource-discovery-mode` parameter</span></span>

### <a name="profile"></a><span data-ttu-id="69b8c-1181">Perfil</span><span class="sxs-lookup"><span data-stu-id="69b8c-1181">Profile</span></span>

* <span data-ttu-id="69b8c-1182">`az account get-access-token`: Adicionar parâmetro `--tenant` para adquirir o token do locatário diretamente, sem a necessidade de especificar uma assinatura</span><span class="sxs-lookup"><span data-stu-id="69b8c-1182">`az account get-access-token`: Add `--tenant` parameter to acquire token for the tenant directly, needless to specify a subscription</span></span>

### <a name="rbac"></a><span data-ttu-id="69b8c-1183">RBAC</span><span class="sxs-lookup"><span data-stu-id="69b8c-1183">RBAC</span></span>

* <span data-ttu-id="69b8c-1184">[ALTERAÇÃO SIGNIFICATIVA] Correção nº 11883: `az role assignment create`: o escopo vazio exibirá erro</span><span class="sxs-lookup"><span data-stu-id="69b8c-1184">[BREAKING CHANGE] Fix #11883: `az role assignment create`: empty scope will prompt error</span></span>

### <a name="security"></a><span data-ttu-id="69b8c-1185">Segurança</span><span class="sxs-lookup"><span data-stu-id="69b8c-1185">Security</span></span>

* <span data-ttu-id="69b8c-1186">Adicione novos comandos `az atp show` e `az atp update` para exibir e gerenciar configurações avançadas de proteção contra ameaças para contas de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1186">Add new commands `az atp show` and `az atp update` to view and manage advanced threat protection settings for storage accounts.</span></span>

### <a name="sql"></a><span data-ttu-id="69b8c-1187">SQL</span><span class="sxs-lookup"><span data-stu-id="69b8c-1187">SQL</span></span>

* <span data-ttu-id="69b8c-1188">`sql dw create`: substitua os parâmetros `--zone-redundant` e `--read-replica-count`.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1188">`sql dw create`: deprecate `--zone-redundant` and `--read-replica-count` parameters.</span></span> <span data-ttu-id="69b8c-1189">Esses parâmetros não se aplicam ao DataWarehouse.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1189">These parameters do not apply to DataWarehouse.</span></span>
* <span data-ttu-id="69b8c-1190">[ALTERAÇÃO DA FALHA] `az sql db create`: Remova "WideWorldImportersStd" e "WideWorldImportersFull" como valores permitidos documentados para "az sql db create --sample-name".</span><span class="sxs-lookup"><span data-stu-id="69b8c-1190">[BREAKING CHANGE] `az sql db create`: Remove "WideWorldImportersStd" and "WideWorldImportersFull" as documented allowed values for "az sql db create --sample-name".</span></span> <span data-ttu-id="69b8c-1191">Esses bancos de dados de exemplo sempre farão a criação falhar.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1191">These sample databases would always cause creation to fail.</span></span>
* <span data-ttu-id="69b8c-1192">Adicione os novos comandos `sql db classification show/list/update/delete` e `sql db classification recommendation list/enable/disable` para gerenciar classificações de confidencialidade para bancos de dados SQL.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1192">Add New commands `sql db classification show/list/update/delete` and `sql db classification recommendation list/enable/disable` to manage sensitivity classifications for SQL databases.</span></span>
* <span data-ttu-id="69b8c-1193">`az sql db audit-policy`: Correção para ações e grupos de auditoria vazios</span><span class="sxs-lookup"><span data-stu-id="69b8c-1193">`az sql db audit-policy`: Fix for empty audit actions and groups</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-1194">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-1194">Storage</span></span>

* <span data-ttu-id="69b8c-1195">Adicione um novo grupo de comandos `az storage share-rm` para usar o provedor de recursos Microsoft.Storage para operações de gerenciamento de compartilhamento de arquivo do Azure.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1195">Add a new command group `az storage share-rm` to use the Microsoft.Storage resource provider for Azure file share management operations.</span></span>
* <span data-ttu-id="69b8c-1196">Correção de problema nº 11415: erro de permissão para `az storage blob update`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1196">Fix issue #11415: permission error for `az storage blob update`</span></span>
* <span data-ttu-id="69b8c-1197">Integre Azcopy 10.3.3 e dê suporte a Win32.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1197">Integrate Azcopy 10.3.3 and support Win32.</span></span>
* <span data-ttu-id="69b8c-1198">`az storage copy`: Adicione os parâmetros `--include-path`, `--include-pattern`, `--exclude-path` e `--exclude-pattern`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1198">`az storage copy`: Add `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="69b8c-1199">`az storage remove`: Altere os parâmetros `--inlcude` e `--exclude` para os parâmetros `--include-path`, `--include-pattern`, `--exclude-path` e `--exclude-pattern`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1199">`az storage remove`: Change `--inlcude` and `--exclude` parameters to `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="69b8c-1200">`az storage sync`: Adicione os parâmetros `--include-pattern`, `--exclude-path` e `--exclude-pattern`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1200">`az storage sync`: Add `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>

### <a name="servicefabric"></a><span data-ttu-id="69b8c-1201">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="69b8c-1201">ServiceFabric</span></span>

* <span data-ttu-id="69b8c-1202">Adicione novos comandos para gerenciar o aplicativo e os serviços.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1202">Add new commands to manage appliaction and services.</span></span>

## <a name="january-13-2020"></a><span data-ttu-id="69b8c-1203">13 de janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="69b8c-1203">January 13, 2020</span></span>

<span data-ttu-id="69b8c-1204">Versão 2.0.80</span><span class="sxs-lookup"><span data-stu-id="69b8c-1204">Version 2.0.80</span></span>

### <a name="compute"></a><span data-ttu-id="69b8c-1205">Computação</span><span class="sxs-lookup"><span data-stu-id="69b8c-1205">Compute</span></span>

* <span data-ttu-id="69b8c-1206">atualização do disco: Adicionar --disk-encryption-set e --encryption-type</span><span class="sxs-lookup"><span data-stu-id="69b8c-1206">disk update: Add --disk-encryption-set and --encryption-type</span></span>
* <span data-ttu-id="69b8c-1207">criação/atualização do instantâneo: Adicionar --disk-encryption-set e --encryption-type</span><span class="sxs-lookup"><span data-stu-id="69b8c-1207">snapshot create/update: Add --disk-encryption-set and --encryption-type</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-1208">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-1208">Storage</span></span>

* <span data-ttu-id="69b8c-1209">Atualizar a versão do azure-mgmt-storage para 7.1.0</span><span class="sxs-lookup"><span data-stu-id="69b8c-1209">Upgrade azure-mgmt-storage version to 7.1.0</span></span>
* <span data-ttu-id="69b8c-1210">`az storage account create`: Adicionar `--encryption-key-type-for-table` e `--encryption-key-type-for-queue` para dar suporte ao Serviço de Criptografia de Tabela e de Fila</span><span class="sxs-lookup"><span data-stu-id="69b8c-1210">`az storage account create`: Add `--encryption-key-type-for-table` and `--encryption-key-type-for-queue` to support Table and Queue Encryption Service</span></span>

## <a name="january-07-2020"></a><span data-ttu-id="69b8c-1211">07 de janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="69b8c-1211">January 07, 2020</span></span>

<span data-ttu-id="69b8c-1212">Versão 2.0.79</span><span class="sxs-lookup"><span data-stu-id="69b8c-1212">Version 2.0.79</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-1213">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-1213">ACR</span></span>

* <span data-ttu-id="69b8c-1214">[ALTERAÇÃO SIGNIFICATIVA] Remover o parâmetro '--os' para 'acr build', 'acr task create/update', 'acr run' e 'acr pack'.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1214">[BREAKING CHANGE] Remove '--os' parameter for 'acr build', 'acr task create/update', 'acr run', and 'acr pack'.</span></span> <span data-ttu-id="69b8c-1215">Em vez disso, use '--platform'.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1215">Use '--platform' instead.</span></span>

### <a name="appconfig"></a><span data-ttu-id="69b8c-1216">AppConfig</span><span class="sxs-lookup"><span data-stu-id="69b8c-1216">AppConfig</span></span>

* <span data-ttu-id="69b8c-1217">Adicionar suporte para importar/exportar sinalizadores de recurso</span><span class="sxs-lookup"><span data-stu-id="69b8c-1217">Add support for importing/exporting feature flags</span></span>
* <span data-ttu-id="69b8c-1218">Adicione o novo comando 'az appconfig kv set-keyvault' para criar a referência do keyvault</span><span class="sxs-lookup"><span data-stu-id="69b8c-1218">Add new command 'az appconfig kv set-keyvault' for creating keyvault reference</span></span>
* <span data-ttu-id="69b8c-1219">Suporte a várias convenções de nomenclatura ao exportar os sinalizadores de recurso para o arquivo</span><span class="sxs-lookup"><span data-stu-id="69b8c-1219">Support various naming conventions when exporting feature flags to file</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-1220">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-1220">AppService</span></span>

* <span data-ttu-id="69b8c-1221">Corrigir o problema #7154: Atualizar a documentação para o comando <> para usar acentos grave em vez de aspas simples</span><span class="sxs-lookup"><span data-stu-id="69b8c-1221">Fix issue #7154: Updating documentation for command <> to use back ticks instead of single quotes</span></span>
* <span data-ttu-id="69b8c-1222">Corrigir o problema #11287: webapp up: Por padrão, faça o aplicativo criado usando 'should be 'SSL enabled'</span><span class="sxs-lookup"><span data-stu-id="69b8c-1222">Fix issue #11287: webapp up: By default make the app created using up 'should be 'SSL enabled'</span></span>
* <span data-ttu-id="69b8c-1223">Corrigir o problema #11592: Adicionar o sinalizador az webapp up para sites HTML estáticos</span><span class="sxs-lookup"><span data-stu-id="69b8c-1223">Fix issue #11592: Add az webapp up flag for html static sites</span></span>

### <a name="arm"></a><span data-ttu-id="69b8c-1224">ARM</span><span class="sxs-lookup"><span data-stu-id="69b8c-1224">ARM</span></span>

* <span data-ttu-id="69b8c-1225">Corrigir `az resource tag`: As marcas do Cofre dos Serviços de Recuperação não podem ser atualizadas</span><span class="sxs-lookup"><span data-stu-id="69b8c-1225">Fix `az resource tag`: Recovery Services Vault tags cannot be updated</span></span>

### <a name="backup"></a><span data-ttu-id="69b8c-1226">Backup</span><span class="sxs-lookup"><span data-stu-id="69b8c-1226">Backup</span></span>

* <span data-ttu-id="69b8c-1227">Novo comando 'backup protection undelete' adicionado para habilitar o recurso de exclusão reversível para carga de trabalho IaasVM</span><span class="sxs-lookup"><span data-stu-id="69b8c-1227">Added new command 'backup protection undelete' to enable soft-delete feature for IaasVM workload</span></span>
* <span data-ttu-id="69b8c-1228">Novo parâmetro '--soft-delete-feature-state' adicionado para definir o comando propriedades do backup</span><span class="sxs-lookup"><span data-stu-id="69b8c-1228">Added new parameter '--soft-delete-feature-state' to set backup-properties command</span></span>
* <span data-ttu-id="69b8c-1229">Suporte de exclusão de disco adicionado para carga de trabalho IaasVM</span><span class="sxs-lookup"><span data-stu-id="69b8c-1229">Added disk exclusion support for IaasVM workload</span></span>

### <a name="compute"></a><span data-ttu-id="69b8c-1230">Computação</span><span class="sxs-lookup"><span data-stu-id="69b8c-1230">Compute</span></span>

* <span data-ttu-id="69b8c-1231">Corrigir a falha `vm create` no perfil do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1231">Fix `vm create` failure in Azure Stack profile.</span></span>
* <span data-ttu-id="69b8c-1232">parte final/listar definições de métricas de monitor de vm: suporte a métricas de consulta e definições de lista para uma vm.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1232">vm monitor metrics tail/list-definitions: support query metric and list definitions for a vm.</span></span>
* <span data-ttu-id="69b8c-1233">Adicionar nova ação de comando de reaplicação para az vm</span><span class="sxs-lookup"><span data-stu-id="69b8c-1233">Add new reapply command action for az vm</span></span>

### <a name="hdinsight"></a><span data-ttu-id="69b8c-1234">HDInsight</span><span class="sxs-lookup"><span data-stu-id="69b8c-1234">HDInsight</span></span>

* <span data-ttu-id="69b8c-1235">Suporte para criar um cluster Kafka com o Proxy REST do Kafka</span><span class="sxs-lookup"><span data-stu-id="69b8c-1235">Support for creating a Kafka cluster with Kafka Rest Proxy</span></span>
* <span data-ttu-id="69b8c-1236">Atualizar azure-mgmt-hdinsight para 1.3.0</span><span class="sxs-lookup"><span data-stu-id="69b8c-1236">Upgrade azure-mgmt-hdinsight to 1.3.0</span></span>

### <a name="misc"></a><span data-ttu-id="69b8c-1237">Diversos.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1237">Misc.</span></span>

* <span data-ttu-id="69b8c-1238">Adicionar comando de visualização `az version show` para mostrar as versões dos módulos e das extensões da CLI do Azure no formato JSON por padrão ou no formato configurado por --output</span><span class="sxs-lookup"><span data-stu-id="69b8c-1238">Add preview command `az version show` to show the versions of Azure CLI modules and extensions in JSON format by default or format configured by --output</span></span>

### <a name="event-hubs"></a><span data-ttu-id="69b8c-1239">Hubs de Eventos</span><span class="sxs-lookup"><span data-stu-id="69b8c-1239">Event Hubs</span></span>

* <span data-ttu-id="69b8c-1240">[ALTERAÇÃO SIGNIFICATIVA] Remover a opção de status 'ReceiveDisabled' do comando 'az eventhubs eventhub update' e 'az eventhubs eventhub create'.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1240">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az eventhubs eventhub update' and 'az eventhubs eventhub create'.</span></span> <span data-ttu-id="69b8c-1241">Essa opção não é válida para entidades do Hub de Eventos.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1241">This option is not valid for Event Hub entities.</span></span>

### <a name="service-bus"></a><span data-ttu-id="69b8c-1242">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="69b8c-1242">Service Bus</span></span>

* <span data-ttu-id="69b8c-1243">[ALTERAÇÃO SIGNIFICATIVA] Remover a opção de status 'ReceiveDisabled' do comando 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create' e 'az servicebus queue update'.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1243">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create', and 'az servicebus queue update'.</span></span> <span data-ttu-id="69b8c-1244">Essa opção não é válida para tópicos e filas do Barramento de Serviço.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1244">This option is not valid for Service Bus topics and queues.</span></span>

### <a name="rbac"></a><span data-ttu-id="69b8c-1245">RBAC</span><span class="sxs-lookup"><span data-stu-id="69b8c-1245">RBAC</span></span>

* <span data-ttu-id="69b8c-1246">Correção #11712: `az ad app/sp show` não devolve o código de saída 3 quando o aplicativo ou a entidade de serviço não existir</span><span class="sxs-lookup"><span data-stu-id="69b8c-1246">Fix #11712: `az ad app/sp show` does not return exit code 3 when the application or service principal does not exist</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-1247">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-1247">Storage</span></span>

* <span data-ttu-id="69b8c-1248">`az storage account create`: Remover o sinalizador de visualização do parâmetro --enable-hierarchical-namespace</span><span class="sxs-lookup"><span data-stu-id="69b8c-1248">`az storage account create`: Remove preview flag for --enable-hierarchical-namespace parameter</span></span>
* <span data-ttu-id="69b8c-1249">Atualizar a versão azure-mgmt-storage para 7.0.0 para usar a versão de API 2019-06-01</span><span class="sxs-lookup"><span data-stu-id="69b8c-1249">Update azure-mgmt-storage version to 7.0.0 to use api version 2019-06-01</span></span>
* <span data-ttu-id="69b8c-1250">Adicionar novos parâmetros `--enable-delete-retention` e `--delete-retention-days` para dar suporte ao gerenciamento da política de retenção de exclusão para a conta de armazenamento blob-service-properties.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1250">Add new parameters `--enable-delete-retention` and `--delete-retention-days` to support managing delete retention policy for storage account blob-service-properties.</span></span>

## <a name="december-17-2019"></a><span data-ttu-id="69b8c-1251">17 de dezembro de 2019</span><span class="sxs-lookup"><span data-stu-id="69b8c-1251">December 17, 2019</span></span>

<span data-ttu-id="69b8c-1252">2.0.78</span><span class="sxs-lookup"><span data-stu-id="69b8c-1252">2.0.78</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-1253">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-1253">ACR</span></span>

* <span data-ttu-id="69b8c-1254">Contexto local de suporte adicionado na execução da tarefa acr</span><span class="sxs-lookup"><span data-stu-id="69b8c-1254">Added support Local context in acr task run</span></span>

### <a name="acs"></a><span data-ttu-id="69b8c-1255">ACS</span><span class="sxs-lookup"><span data-stu-id="69b8c-1255">ACS</span></span>

* <span data-ttu-id="69b8c-1256">[ALTERAÇÃO SIGNIFICATIVA]criar az openshift: renomear `--workspace-resource-id` para `--workspace-id`.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1256">[BREAKING CHANGE]az openshift create: rename `--workspace-resource-id` to `--workspace-id`.</span></span>

### <a name="ams"></a><span data-ttu-id="69b8c-1257">AMS</span><span class="sxs-lookup"><span data-stu-id="69b8c-1257">AMS</span></span>

* <span data-ttu-id="69b8c-1258">Comandos de exibição atualizados para devolver 3 quando o recurso não for encontrado</span><span class="sxs-lookup"><span data-stu-id="69b8c-1258">Updated show commands to return 3 when resource not found</span></span>

### <a name="appconfig"></a><span data-ttu-id="69b8c-1259">AppConfig</span><span class="sxs-lookup"><span data-stu-id="69b8c-1259">AppConfig</span></span>

* <span data-ttu-id="69b8c-1260">Bug corrigido ao acrescentar a versão de API à URL de solicitação.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1260">Fixed bug when appending api-version to request url.</span></span> <span data-ttu-id="69b8c-1261">A solução existente não funciona com a paginação.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1261">The existing solution doesn't work with pagination.</span></span>
* <span data-ttu-id="69b8c-1262">Suporte adicionado para a exibição de idiomas além do inglês, pois nosso serviço de back-end é compatível com unicode para globalização.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1262">Added support for showing languages besides English as our backend service support unicode for globalization.</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-1263">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-1263">AppService</span></span>

* <span data-ttu-id="69b8c-1264">Problema corrigido nº 11217: webapp: o upload ssl de configuração do az webapp deve ser compatível com o parâmetro do slot</span><span class="sxs-lookup"><span data-stu-id="69b8c-1264">Fixed issue #11217: webapp: az webapp config ssl upload should support slot parameter</span></span>
* <span data-ttu-id="69b8c-1265">Problema corrigido nº 10965: Erro: O nome não pode estar vazio.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1265">Fixed issue #10965: Error: Name cannot be empty.</span></span> <span data-ttu-id="69b8c-1266">Permitir remoção por ip_address e sub-rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-1266">Allow remove by ip_address and subnet</span></span>
* <span data-ttu-id="69b8c-1267">Suporte adicionado para importar certificados do Key Vault `az webapp config ssl import`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1267">Added support for importing certificates from Key Vault `az webapp config ssl import`</span></span>

### <a name="arm"></a><span data-ttu-id="69b8c-1268">ARM</span><span class="sxs-lookup"><span data-stu-id="69b8c-1268">ARM</span></span>

* <span data-ttu-id="69b8c-1269">Pacote azure-mgmt-resource atualizado para usar 6.0.0</span><span class="sxs-lookup"><span data-stu-id="69b8c-1269">Updated azure-mgmt-resource package to use 6.0.0</span></span>
* <span data-ttu-id="69b8c-1270">Suporte entre locatários para o comando `az group deployment create` adicionando o novo parâmetro `--aux-subs`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1270">Cross Tenant Support for `az group deployment create` command by adding new parameter `--aux-subs`</span></span>
* <span data-ttu-id="69b8c-1271">Novo parâmetro `--metadata` adicionado para dar suporte à adição de informações de metadados para definições de conjunto de políticas.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1271">Added new parameter `--metadata` to support adding metadata information for policy set definitions.</span></span>

### <a name="backup"></a><span data-ttu-id="69b8c-1272">Backup</span><span class="sxs-lookup"><span data-stu-id="69b8c-1272">Backup</span></span>

* <span data-ttu-id="69b8c-1273">Suporte de backup adicionado para carga de trabalho SQL e SAP Hana.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1273">Added Backup support for SQL and SAP Hana workload.</span></span>

### <a name="botservice"></a><span data-ttu-id="69b8c-1274">BotService</span><span class="sxs-lookup"><span data-stu-id="69b8c-1274">BotService</span></span>

* <span data-ttu-id="69b8c-1275">[ALTERAÇÃO SIGNIFICATIVA] Remover o sinalizador '--version ' do comando de visualização 'az bot create'.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1275">[Breaking change] Remove '--version' flag from preview command 'az bot create'.</span></span> <span data-ttu-id="69b8c-1276">Somente os bots do SDK v4 são compatíveis.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1276">Only v4 SDK bots are supported.</span></span>
* <span data-ttu-id="69b8c-1277">Verificação de disponibilidade de nome adicionada para 'az bot create'.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1277">Added name availability check for 'az bot create'.</span></span>
* <span data-ttu-id="69b8c-1278">Suporte adicionado para atualizar a URL do ícone para um bot por meio de 'az bot update'.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1278">Added support for updating the icon URL for a bot via 'az bot update'.</span></span>
* <span data-ttu-id="69b8c-1279">Suporte adicionado para atualizar um canal Direct Line por meio de 'az bot directline update'.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1279">Added support for updating a Direct Line channel via 'az bot directline update'.</span></span>
* <span data-ttu-id="69b8c-1280">Suporte ao sinalizador '--enable-enhanced-auth' adicionado para 'az bot directline create'.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1280">Added '--enable-enhanced-auth' flag support to 'az bot directline create'.</span></span>
* <span data-ttu-id="69b8c-1281">Os seguintes grupos de comandos estão em GA e não estão em versão prévia: 'az bot authsetting'.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1281">The following command groups are GA and not in preview: 'az bot authsetting'.</span></span>
* <span data-ttu-id="69b8c-1282">Os seguintes comandos em 'az bot' estão em GA e não na versão prévia: 'criar', 'preparar-implantar', 'mostrar', 'excluir', 'atualizar'.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1282">The following commands in 'az bot' are GA and not in preview: 'create', 'prepare-deploy', 'show', 'delete', 'update'.</span></span>
* <span data-ttu-id="69b8c-1283">Correção do valor 'az bot prepare-deploy' alterando '--proj-file-path ' para letras minúsculas (por exemplo, "Test. csproj" para "Test. csproj").</span><span class="sxs-lookup"><span data-stu-id="69b8c-1283">Fixed 'az bot prepare-deploy' changing '--proj-file-path' value to lower case (e.g. "Test.csproj" to "test.csproj").</span></span>

### <a name="compute"></a><span data-ttu-id="69b8c-1284">Computação</span><span class="sxs-lookup"><span data-stu-id="69b8c-1284">Compute</span></span>

* <span data-ttu-id="69b8c-1285">Criar/atualizar vmss: --scale-in-policy adicionado, que decide quais máquinas virtuais são escolhidas para remoção quando um VMSS é dimensionado.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1285">vmss create/update: Added --scale-in-policy, which decides which virtual machines are chosen for removal when a VMSS is scaled-in.</span></span>
* <span data-ttu-id="69b8c-1286">atualização de vm/vmss: --priority adicionado.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1286">vm/vmss update: Added --priority.</span></span>
* <span data-ttu-id="69b8c-1287">atualização de vm/vmss: --max-price adicionado.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1287">vm/vmss update: Added --max-price.</span></span>
* <span data-ttu-id="69b8c-1288">Grupo de comandos do conjunto de criptografia de disco adicionado (criar, mostrar, atualizar, excluir e listar).</span><span class="sxs-lookup"><span data-stu-id="69b8c-1288">Added disk-encryption-set command group (create, show, update, delete, list).</span></span>
* <span data-ttu-id="69b8c-1289">criação de disco: --encryption-type e --disk-encryption-set adicionados.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1289">disk create: Added --encryption-type and --disk-encryption-set.</span></span>
* <span data-ttu-id="69b8c-1290">vm/vmss create: --os-disk-encryption-set e --data-disk-encryption-sets adicionados.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1290">vm/vmss create: Added --os-disk-encryption-set and --data-disk-encryption-sets.</span></span>

### <a name="core"></a><span data-ttu-id="69b8c-1291">Núcleo</span><span class="sxs-lookup"><span data-stu-id="69b8c-1291">Core</span></span>

* <span data-ttu-id="69b8c-1292">Suporte para Python 3.4 removido</span><span class="sxs-lookup"><span data-stu-id="69b8c-1292">Removed support for Python 3.4</span></span>
* <span data-ttu-id="69b8c-1293">Pesquisa de funções de plug-in em vários comandos</span><span class="sxs-lookup"><span data-stu-id="69b8c-1293">Plug in HaTS survey in multiple commands</span></span>

### <a name="dls"></a><span data-ttu-id="69b8c-1294">DLS</span><span class="sxs-lookup"><span data-stu-id="69b8c-1294">DLS</span></span>

* <span data-ttu-id="69b8c-1295">Versão atualizada do SDK do ADLS (0.0.48).</span><span class="sxs-lookup"><span data-stu-id="69b8c-1295">Updated ADLS sdk version (0.0.48).</span></span>

### <a name="install"></a><span data-ttu-id="69b8c-1296">Instalar</span><span class="sxs-lookup"><span data-stu-id="69b8c-1296">Install</span></span>

* <span data-ttu-id="69b8c-1297">Instalar suporte de script Python 3.8</span><span class="sxs-lookup"><span data-stu-id="69b8c-1297">Install script support python 3.8</span></span>

### <a name="iot"></a><span data-ttu-id="69b8c-1298">IOT</span><span class="sxs-lookup"><span data-stu-id="69b8c-1298">IOT</span></span>

* <span data-ttu-id="69b8c-1299">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro--failover-region removido de failover manual.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1299">[BREAKING CHANGE] Removed --failover-region parameter from manual-failover.</span></span> <span data-ttu-id="69b8c-1300">Agora ele fará failover para a região secundária emparelhada atribuída geograficamente.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1300">Now it will failover to assigned geo-paired secondary region.</span></span>

### <a name="key-vault"></a><span data-ttu-id="69b8c-1301">Key Vault</span><span class="sxs-lookup"><span data-stu-id="69b8c-1301">Key Vault</span></span>

* <span data-ttu-id="69b8c-1302">Nº 8095 corrigido: `az keyvault storage remove`: melhorar a mensagem de ajuda</span><span class="sxs-lookup"><span data-stu-id="69b8c-1302">Fixed #8095: `az keyvault storage remove`: improve the help message</span></span>
* <span data-ttu-id="69b8c-1303">Nº 8921 corrigido: `az keyvault key/secret/certificate list/list-deleted/list-versions`: corrigir o bug de validação no parâmetro `--maxresults`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1303">Fixed #8921: `az keyvault key/secret/certificate list/list-deleted/list-versions`: fix the validation bug on parameter `--maxresults`</span></span>
* <span data-ttu-id="69b8c-1304">Nº 10512 corrigido: `az keyvault set-policy`: melhorar a mensagem de erro quando nenhuma das `--object-id`, `--spn` ou `--upn` for especificada</span><span class="sxs-lookup"><span data-stu-id="69b8c-1304">Fixed #10512: `az keyvault set-policy`: improve the error message when none of `--object-id`, `--spn` or `--upn` is specified</span></span>
* <span data-ttu-id="69b8c-1305">Nº 10846 corrigido: `az keyvault secret show-deleted`: quando `--id` for especificado, `--name/-n` não será necessário</span><span class="sxs-lookup"><span data-stu-id="69b8c-1305">Fixed #10846: `az keyvault secret show-deleted`: when `--id` is specified, `--name/-n` is not required</span></span>
* <span data-ttu-id="69b8c-1306">Nº 11084 corrigido: `az keyvault secret download`: melhorar a mensagem de ajuda do parâmetro `--encoding`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1306">Fixed #11084: `az keyvault secret download`: improve the help message of parameter `--encoding`</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-1307">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-1307">Network</span></span>

* <span data-ttu-id="69b8c-1308">Investigação de gateway de aplicativo de rede az: Suporte --port option adicionado para especificar uma porta para sondar servidores de back-end ao criar e atualizar</span><span class="sxs-lookup"><span data-stu-id="69b8c-1308">az network application-gateway probe: Added support --port option to specify a port for probing backend servers when create and update</span></span>
* <span data-ttu-id="69b8c-1309">az network application-gateway url-path-map create/update: correção de bug para `--waf-policy`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1309">az network application-gateway url-path-map create/update: bug fix for `--waf-policy`</span></span>
* <span data-ttu-id="69b8c-1310">az network application-gateway: Suporte `--rewrite-rule-set` adicionado</span><span class="sxs-lookup"><span data-stu-id="69b8c-1310">az network application-gateway: Added support `--rewrite-rule-set`</span></span>
* <span data-ttu-id="69b8c-1311">az network list-service-aliases: Foram adicionados aliases de serviço da lista de suporte que podem ser usados para políticas de ponto de extremidade de serviço</span><span class="sxs-lookup"><span data-stu-id="69b8c-1311">az network list-service-aliases: Added support list service aliases which can be used for Service Endpoint Policies</span></span>
* <span data-ttu-id="69b8c-1312">importar zona dns da rede az: Suporte adicionado. @ no nome do registro</span><span class="sxs-lookup"><span data-stu-id="69b8c-1312">az network dns zone import: Added support .@ in record name</span></span>

### <a name="packaging"></a><span data-ttu-id="69b8c-1313">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-1313">Packaging</span></span>

* <span data-ttu-id="69b8c-1314">Compilações de back edge adicionadas para instalação de pip</span><span class="sxs-lookup"><span data-stu-id="69b8c-1314">Added back edge builds for pip install</span></span>
* <span data-ttu-id="69b8c-1315">Pacote eoan do Ubuntu adicionado</span><span class="sxs-lookup"><span data-stu-id="69b8c-1315">Added Ubuntu eoan package</span></span>

### <a name="policy"></a><span data-ttu-id="69b8c-1316">Política</span><span class="sxs-lookup"><span data-stu-id="69b8c-1316">Policy</span></span>

* <span data-ttu-id="69b8c-1317">Inclusão de compatibilidade com a API de Política, versão de 01/09/2019.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1317">Added support for Policy API version 2019-09-01.</span></span>
* <span data-ttu-id="69b8c-1318">az policy set-definition: Agrupamento de suporte adicionado nas definições do conjunto de políticas com `--definition-groups` parâmetro</span><span class="sxs-lookup"><span data-stu-id="69b8c-1318">az policy set-definition: Added support grouping within policy set definitions with `--definition-groups` parameter</span></span>

### <a name="redis"></a><span data-ttu-id="69b8c-1319">Redis</span><span class="sxs-lookup"><span data-stu-id="69b8c-1319">Redis</span></span>

* <span data-ttu-id="69b8c-1320">Adicionado o parâmetro de visualização `--replicas-per-master` ao comando `az redis create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1320">Added preview param `--replicas-per-master` to `az redis create` command</span></span>
* <span data-ttu-id="69b8c-1321">Azure-MGMT-Redis adicionado do 6.0.0 para o 7.0.0rc1</span><span class="sxs-lookup"><span data-stu-id="69b8c-1321">Updated azure-mgmt-redis from 6.0.0 to 7.0.0rc1</span></span>

### <a name="servicefabric"></a><span data-ttu-id="69b8c-1322">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="69b8c-1322">ServiceFabric</span></span>

* <span data-ttu-id="69b8c-1323">Corrigido em nó-tipo adicionar lógica, incluindo #10963: A adição do novo tipo de nó com nível de durabilidade Gold sempre gerará erro da CLI</span><span class="sxs-lookup"><span data-stu-id="69b8c-1323">Fixed in node-type add logic including #10963: Adding new node type with durability level Gold will always throw CLI error</span></span>
* <span data-ttu-id="69b8c-1324">Versão do ServiceFabricNodeVmExt atualizada para 1.1 no modelo de criação</span><span class="sxs-lookup"><span data-stu-id="69b8c-1324">Updated ServiceFabricNodeVmExt version to 1.1 in creation template</span></span>

### <a name="sql"></a><span data-ttu-id="69b8c-1325">SQL</span><span class="sxs-lookup"><span data-stu-id="69b8c-1325">SQL</span></span>

* <span data-ttu-id="69b8c-1326">Adicionados os parâmetros "--read-scale" e "--read-replicas" aos comandos criar e atualizar do BD SQL para dar suporte ao gerenciamento de escala de leitura.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1326">Added "--read-scale" and "--read-replicas" parameters to sql db create and update commands, to support read scale management.</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-1327">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-1327">Storage</span></span>

* <span data-ttu-id="69b8c-1328">Propriedade de compartilhamentos de arquivos grandes da versão GA para o comando criar e atualizar da conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-1328">GA Release Large File Shares property for storage account create and update command</span></span>
* <span data-ttu-id="69b8c-1329">Suporte ao token SAS de delegação de usuário da versão GA</span><span class="sxs-lookup"><span data-stu-id="69b8c-1329">GA Release User Delegation SAS token Support</span></span>
* <span data-ttu-id="69b8c-1330">Novos comandos adicionados `az storage account blob-service-properties show` e `az storage account blob-service-properties update --enable-change-feed` para gerenciar Propriedades do serviço blob para a conta de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1330">Added new commands `az storage account blob-service-properties show` and `az storage account blob-service-properties update --enable-change-feed` to manage blob service properties for storage account.</span></span>
* <span data-ttu-id="69b8c-1331">[PRÓXIMA ALTERAÇÃO DA FALHA] `az storage copy`: `*` não há mais suporte para o caractere de como um curinga na URL, mas novos parâmetros--include-pattern e --exclude-pattern serão adicionados com suporte a curinga `*`.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1331">[COMING BREAKING CHANGE] `az storage copy`: `*` character is no longer supported as a wildcard in URL, but new parameters --include-pattern and --exclude-pattern will be added with `*` wildcard support.</span></span>
* <span data-ttu-id="69b8c-1332">Problema corrigido nº 11043: Suporte adicionado para remover contêiner/compartilhamento inteiro no comando `az storage remove`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1332">Fixed issue #11043: Added support to remove whole container/share in `az storage remove` command</span></span>

## <a name="november-26-2019"></a><span data-ttu-id="69b8c-1333">26 de novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="69b8c-1333">November 26, 2019</span></span>

<span data-ttu-id="69b8c-1334">Versão 2.0.77</span><span class="sxs-lookup"><span data-stu-id="69b8c-1334">Version 2.0.77</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-1335">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-1335">ACR</span></span>

* <span data-ttu-id="69b8c-1336">Parâmetro `--branch` preterido da criação/atualização da tarefa ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-1336">Deprecated parameter `--branch` from acr task create/update</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="69b8c-1337">Red Hat OpenShift no Azure</span><span class="sxs-lookup"><span data-stu-id="69b8c-1337">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="69b8c-1338">Sinalizador `--workspace-resource-id` adicionado para permitir a criação do cluster do Red Hat OpenShift no Azure com monitoramento</span><span class="sxs-lookup"><span data-stu-id="69b8c-1338">Added `--workspace-resource-id` flag to allow creation of Azure Red Hat Openshift cluster with monitoring</span></span>
* <span data-ttu-id="69b8c-1339">`monitor_profile` adicionado para criar o cluster do Red Hat OpenShift no Azure com monitoramento</span><span class="sxs-lookup"><span data-stu-id="69b8c-1339">Added `monitor_profile` to create Azure Red Hat OpenShift cluster with monitoring</span></span>

### <a name="aks"></a><span data-ttu-id="69b8c-1340">AKS</span><span class="sxs-lookup"><span data-stu-id="69b8c-1340">AKS</span></span>

* <span data-ttu-id="69b8c-1341">Operação de rotação de certificado de cluster de suporte adicionada usando "az aks rotate-certs".</span><span class="sxs-lookup"><span data-stu-id="69b8c-1341">Added support cluster certificate rotation operation using "az aks rotate-certs".</span></span>

### <a name="appconfig"></a><span data-ttu-id="69b8c-1342">AppConfig</span><span class="sxs-lookup"><span data-stu-id="69b8c-1342">AppConfig</span></span>

* <span data-ttu-id="69b8c-1343">Suporte adicionado para usar ":" para o separador `as az appconfig kv import`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1343">Added support for using ":" for `as az appconfig kv import` separator</span></span>
* <span data-ttu-id="69b8c-1344">Problema corrigido para listar valores de chave com vários rótulos incluindo o rótulo nulo.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1344">Fixed issue for listing key values with multiple labels including null label.</span></span> 
* <span data-ttu-id="69b8c-1345">SDK do plano de gerenciamento atualizado, azure-mgmt-appconfiguration, para a versão 0.3.0.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1345">Updated management plane sdk, azure-mgmt-appconfiguration, to version 0.3.0.</span></span> 

### <a name="appservice"></a><span data-ttu-id="69b8c-1346">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-1346">AppService</span></span>

* <span data-ttu-id="69b8c-1347">Problema corrigido nº 11100: AttributeError para az webapp up ao criar o plano de serviço</span><span class="sxs-lookup"><span data-stu-id="69b8c-1347">Fixed issue #11100: AttributeError for az webapp up when create service plan</span></span>
* <span data-ttu-id="69b8c-1348">az webapp up: Forçar a criação ou a implantação em um site para linguagens com suporte, nenhum padrão usado.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1348">az webapp up: Forcing the creation or deployment to a site for supported languages, no defaults used.</span></span>
* <span data-ttu-id="69b8c-1349">Suporte adicionado para o Ambiente do Serviço de Aplicativo: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span><span class="sxs-lookup"><span data-stu-id="69b8c-1349">Added support for App Service Environment: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span></span>

### <a name="backup"></a><span data-ttu-id="69b8c-1350">Backup</span><span class="sxs-lookup"><span data-stu-id="69b8c-1350">Backup</span></span>

* <span data-ttu-id="69b8c-1351">Problema corrigido em list-associated-items da política de backup az.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1351">Fixed issue in az backup policy list-associated-items.</span></span> <span data-ttu-id="69b8c-1352">Parâmetro BackupManagementType opcional adicionado.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1352">Added optional BackupManagementType parameter.</span></span>

### <a name="compute"></a><span data-ttu-id="69b8c-1353">Computação</span><span class="sxs-lookup"><span data-stu-id="69b8c-1353">Compute</span></span>

* <span data-ttu-id="69b8c-1354">Versão de API de computação, discos e instantâneos atualizados para 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="69b8c-1354">Upgraded API version of compute, disks, snapshots to 2019-07-01</span></span>
* <span data-ttu-id="69b8c-1355">vmss create: melhoria para --orchestration-mode</span><span class="sxs-lookup"><span data-stu-id="69b8c-1355">vmss create: Improvement for --orchestration-mode</span></span>
* <span data-ttu-id="69b8c-1356">sig image-definition create: --os-state adicionado para permitir a especificação se as máquinas virtuais criadas nessa imagem são 'Generalizadas' ou 'Especializadas'</span><span class="sxs-lookup"><span data-stu-id="69b8c-1356">sig image-definition create: Added --os-state to allow specifying whether the virtual machines created under this image are 'Generalized' or 'Specialized'</span></span>
* <span data-ttu-id="69b8c-1357">sig image-definition create: --hyper-v-generation adicionado para permitir a especificação da geração do hipervisor</span><span class="sxs-lookup"><span data-stu-id="69b8c-1357">sig image-definition create: Added --hyper-v-generation to allow specifying the hypervisor generation</span></span>
* <span data-ttu-id="69b8c-1358">sig image-version create: --os-snapshot e --data-snapshots de suporte adicionados</span><span class="sxs-lookup"><span data-stu-id="69b8c-1358">sig image-version create: Added support --os-snapshot and --data-snapshots</span></span>
* <span data-ttu-id="69b8c-1359">image create: --data-disk-caching adicionado para permitir a especificação da configuração de cache de discos de dados</span><span class="sxs-lookup"><span data-stu-id="69b8c-1359">image create: Added --data-disk-caching to allow specifying caching setting of data disks</span></span>
* <span data-ttu-id="69b8c-1360">SDK de computação do Python atualizado para 10.0.0</span><span class="sxs-lookup"><span data-stu-id="69b8c-1360">Upgraded Python Compute SDK to 10.0.0</span></span>
* <span data-ttu-id="69b8c-1361">vm/vmss create: 'Spot' adicionado à propriedade de enumeração 'Priority'</span><span class="sxs-lookup"><span data-stu-id="69b8c-1361">vm/vmss create: Added 'Spot' to 'Priority' enum property</span></span>
* <span data-ttu-id="69b8c-1362">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro '--max-billing' renomeado para '--max-price', para a VM e o VMSS, a fim de que seja consistente com os cmdlets do Swagger e do PowerShell</span><span class="sxs-lookup"><span data-stu-id="69b8c-1362">[Breaking change] Renamed '--max-billing' parameter to '--max-price', for both VM and VMSS, to be consistent with Swagger and Powershell cmdlets</span></span>
* <span data-ttu-id="69b8c-1363">vm monitor log show: suporte adicionado para consultar o log pelo workspace do Log Analytics vinculado.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1363">vm monitor log show: Added support for querying log over linked log analytics workspace.</span></span>

### <a name="iot"></a><span data-ttu-id="69b8c-1364">IOT</span><span class="sxs-lookup"><span data-stu-id="69b8c-1364">IOT</span></span>

* <span data-ttu-id="69b8c-1365">Correção nº 2531: argumentos de conveniência adicionados para a atualização do hub.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1365">Fix #2531: Added convenience arguments for hub update.</span></span>
* <span data-ttu-id="69b8c-1366">Correção nº 8323: parâmetros ausentes adicionados para criar o ponto de extremidade personalizado de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1366">Fix #8323: Added missing parameters to create storage custom endpoint.</span></span>
* <span data-ttu-id="69b8c-1367">Corrigir bug de regressão: as alterações que substituem o ponto de extremidade de armazenamento padrão foram revertidas.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1367">Fix regression bug: Reverted the changes which overrides the default storage endpoint.</span></span>

### <a name="key-vault"></a><span data-ttu-id="69b8c-1368">Key Vault</span><span class="sxs-lookup"><span data-stu-id="69b8c-1368">Key Vault</span></span>

* <span data-ttu-id="69b8c-1369">Correção nº 11121: ao usar `az keyvault certificate list`, passar `--include-pending` agora não exige um valor de `true` ou `false`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1369">Fixed #11121: When using `az keyvault certificate list`, passing `--include-pending` now doesn't require a value of `true` or `false`</span></span>

### <a name="netappfiles"></a><span data-ttu-id="69b8c-1370">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="69b8c-1370">NetAppFiles</span></span>

* <span data-ttu-id="69b8c-1371">azure-mgmt-netapp atualizado para 0.7.0 que inclui algumas propriedades de volume adicionais associadas a operações de replicação futuras</span><span class="sxs-lookup"><span data-stu-id="69b8c-1371">Upgraded azure-mgmt-netapp to 0.7.0 which includes some additional volume properties associated with upcoming replication operations</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-1372">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-1372">Network</span></span>

* <span data-ttu-id="69b8c-1373">application-gateway waf-config: preterido</span><span class="sxs-lookup"><span data-stu-id="69b8c-1373">application-gateway waf-config: deprecated</span></span>
* <span data-ttu-id="69b8c-1374">application-gateway waf-policy: subgrupo managed-rules adicionado para gerenciar os conjuntos de regras e regras de exclusão gerenciados</span><span class="sxs-lookup"><span data-stu-id="69b8c-1374">application-gateway waf-policy: Added subgroup managed-rules to manage managed rule sets and exclusion rules</span></span>
* <span data-ttu-id="69b8c-1375">application-gateway waf-policy: subgrupo policy-setting adicionado para gerenciar a configuração global de um waf-policy</span><span class="sxs-lookup"><span data-stu-id="69b8c-1375">application-gateway waf-policy: Added subgroup policy-setting to manage global configuration of a waf-policy</span></span>
* <span data-ttu-id="69b8c-1376">[ALTERAÇÃO SIGNIFICATIVA] application-gateway waf-policy: subgrupo rule renomeado para custom-rule</span><span class="sxs-lookup"><span data-stu-id="69b8c-1376">[BREAKING CHANGE] application-gateway waf-policy: Renamed subgroup rule to custom-rule</span></span>
* <span data-ttu-id="69b8c-1377">application-gateway http-listener: --firewall-policy adicionado durante a criação</span><span class="sxs-lookup"><span data-stu-id="69b8c-1377">application-gateway http-listener: Added --firewall-policy when create</span></span>
* <span data-ttu-id="69b8c-1378">application-gateway url-path-map rule: --firewall-policy adicionado durante a criação</span><span class="sxs-lookup"><span data-stu-id="69b8c-1378">application-gateway url-path-map rule: Added --firewall-policy when create</span></span>

### <a name="packaging"></a><span data-ttu-id="69b8c-1379">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-1379">Packaging</span></span>

* <span data-ttu-id="69b8c-1380">Wrapper az reescrito no Python</span><span class="sxs-lookup"><span data-stu-id="69b8c-1380">Rewrote the az wrapper in Python</span></span>
* <span data-ttu-id="69b8c-1381">Suporte adicionado para Python 3.8</span><span class="sxs-lookup"><span data-stu-id="69b8c-1381">Added support for Python 3.8</span></span>
* <span data-ttu-id="69b8c-1382">Alterado para Python 3 para o pacote RPM</span><span class="sxs-lookup"><span data-stu-id="69b8c-1382">Changed to Python 3 for RPM package</span></span>

### <a name="profile"></a><span data-ttu-id="69b8c-1383">Perfil</span><span class="sxs-lookup"><span data-stu-id="69b8c-1383">Profile</span></span>

* <span data-ttu-id="69b8c-1384">Erro aperfeiçoado ao executar `az login -u {} -p {}` com a conta Microsoft</span><span class="sxs-lookup"><span data-stu-id="69b8c-1384">Polished error when running `az login -u {} -p {}` with Microsoft account</span></span>
* <span data-ttu-id="69b8c-1385">`SSLError` aperfeiçoado ao executar `az login` atrás de um proxy com o certificado raiz autoassinado</span><span class="sxs-lookup"><span data-stu-id="69b8c-1385">Polished `SSLError` when running `az login` behind a proxy with self-signed root certificate</span></span>
* <span data-ttu-id="69b8c-1386">Correção nº 10578: `az login` trava quando mais de uma instância é iniciada ao mesmo tempo no Windows ou WSL</span><span class="sxs-lookup"><span data-stu-id="69b8c-1386">Fixed #10578: `az login` hangs when more than one instances are launched at the same time on Windows or WSL</span></span>
* <span data-ttu-id="69b8c-1387">Correção nº 11059: `az login --allow-no-subscriptions` falhará se houver assinaturas no locatário</span><span class="sxs-lookup"><span data-stu-id="69b8c-1387">Fixed #11059: `az login --allow-no-subscriptions` fails if there are subscriptions in the tenant</span></span>
* <span data-ttu-id="69b8c-1388">Correção nº 11238: após renomear uma assinatura, fazer logon com a MSI fará a mesma assinatura aparecer duas vezes</span><span class="sxs-lookup"><span data-stu-id="69b8c-1388">Fixed #11238: After renaming a subscription, logging in with MSI will result in the same subscription appearing twice</span></span>

### <a name="rbac"></a><span data-ttu-id="69b8c-1389">RBAC</span><span class="sxs-lookup"><span data-stu-id="69b8c-1389">RBAC</span></span>

* <span data-ttu-id="69b8c-1390">Correção nº 10996: erro aperfeiçoado para `--force-change-password-next-login` em `az ad user update` quando `--password` não for especificado</span><span class="sxs-lookup"><span data-stu-id="69b8c-1390">Fixed #10996: Polish error for `--force-change-password-next-login` in `az ad user update` when `--password` is not specified</span></span>

### <a name="redis"></a><span data-ttu-id="69b8c-1391">Redis</span><span class="sxs-lookup"><span data-stu-id="69b8c-1391">Redis</span></span>

* <span data-ttu-id="69b8c-1392">Correção nº 2902: evite definir configurações de memória ao atualizar o cache do SKU básico</span><span class="sxs-lookup"><span data-stu-id="69b8c-1392">Fixed #2902: Avoid setting memory configs while updating Basic SKU cache</span></span>

### <a name="reservations"></a><span data-ttu-id="69b8c-1393">Reservas</span><span class="sxs-lookup"><span data-stu-id="69b8c-1393">Reservations</span></span>

* <span data-ttu-id="69b8c-1394">Versão do SDK atualizada para 0.6.0</span><span class="sxs-lookup"><span data-stu-id="69b8c-1394">Upgraded SDK Version to 0.6.0</span></span>
* <span data-ttu-id="69b8c-1395">Informações de detalhes do plano de cobrança atualizadas após chamar Get-Gatalogs</span><span class="sxs-lookup"><span data-stu-id="69b8c-1395">Added billingplan details info after calling Get-Gatalogs</span></span>
* <span data-ttu-id="69b8c-1396">Novo comando `az reservations reservation-order calculate` adicionado para calcular o preço de uma reserva</span><span class="sxs-lookup"><span data-stu-id="69b8c-1396">Added new command `az reservations reservation-order calculate` to calculate the price for a reservation</span></span>
* <span data-ttu-id="69b8c-1397">Novo comando `az reservations reservation-order purchase` adicionado para comprar uma nova reserva</span><span class="sxs-lookup"><span data-stu-id="69b8c-1397">Added new command `az reservations reservation-order purchase` to purchase a new reservation</span></span>

### <a name="rest"></a><span data-ttu-id="69b8c-1398">Rest</span><span class="sxs-lookup"><span data-stu-id="69b8c-1398">Rest</span></span>
* <span data-ttu-id="69b8c-1399">`az rest` alterado para GA</span><span class="sxs-lookup"><span data-stu-id="69b8c-1399">Changed `az rest` to GA</span></span>

### <a name="sql"></a><span data-ttu-id="69b8c-1400">SQL</span><span class="sxs-lookup"><span data-stu-id="69b8c-1400">SQL</span></span>

* <span data-ttu-id="69b8c-1401">azure-mgmt-sql atualizado para 0.15.0.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1401">Updated azure-mgmt-sql to version 0.15.0.</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-1402">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-1402">Storage</span></span>

* <span data-ttu-id="69b8c-1403">storage account create: --enable-hierarchical-namespace adicionado para dar suporte à semântica do sistema de arquivos no serviço Blob.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1403">storage account create: Added --enable-hierarchical-namespace to support filesystem semantics in blob service.</span></span>
* <span data-ttu-id="69b8c-1404">Exceção não relacionada removida da mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="69b8c-1404">Removed unrelated exception from error message</span></span>
* <span data-ttu-id="69b8c-1405">Problemas corrigidos com a mensagem de erro incorreta "Você não tem as permissões necessárias para executar essa operação."</span><span class="sxs-lookup"><span data-stu-id="69b8c-1405">Fixed issues with incorrect error message "You do not have the required permissions needed to perform this operation."</span></span> <span data-ttu-id="69b8c-1406">quando bloqueado pelas regras de rede ou AuthenticationFailed.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1406">when blocked by network rules or AuthenticationFailed.</span></span>

## <a name="november-4-2019"></a><span data-ttu-id="69b8c-1407">4 de novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="69b8c-1407">November 4, 2019</span></span>

<span data-ttu-id="69b8c-1408">Versão 2.0.76</span><span class="sxs-lookup"><span data-stu-id="69b8c-1408">Version 2.0.76</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-1409">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-1409">ACR</span></span>

* <span data-ttu-id="69b8c-1410">O parâmetro de versão prévia `--pack-image-tag` foi adicionado ao comando `az acr pack build`.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1410">Added a preview parameter `--pack-image-tag` to command `az acr pack build`.</span></span>
* <span data-ttu-id="69b8c-1411">Suporte adicionado para habilitar a auditoria na criação de um registro</span><span class="sxs-lookup"><span data-stu-id="69b8c-1411">Added support for enabling auditing on creating a registry</span></span>
* <span data-ttu-id="69b8c-1412">Suporte adicionado para o RBAC com escopo de repositório</span><span class="sxs-lookup"><span data-stu-id="69b8c-1412">Added support for Repository-scoped RBAC</span></span>

### <a name="aks"></a><span data-ttu-id="69b8c-1413">AKS</span><span class="sxs-lookup"><span data-stu-id="69b8c-1413">AKS</span></span>

* <span data-ttu-id="69b8c-1414">`--enable-cluster-autoscaler`, `--min-count` e `--max-count` foram adicionados ao comando `az aks create`, que habilita o dimensionamento automático do cluster para o pool de nós.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1414">Added `--enable-cluster-autoscaler`, `--min-count` and `--max-count` to the `az aks create` command, which enables cluster autoscaler for the node pool.</span></span>
* <span data-ttu-id="69b8c-1415">Foram adicionados os sinalizadores acima, bem como `--update-cluster-autoscaler` e `--disable-cluster-autoscaler` ao comando `az aks update`, permitindo atualizações do cluster de dimensionamento automático.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1415">Added the above flags as well as `--update-cluster-autoscaler` and `--disable-cluster-autoscaler` to the `az aks update` command, allowing updates to cluster autoscaler.</span></span>

### <a name="appconfig"></a><span data-ttu-id="69b8c-1416">AppConfig</span><span class="sxs-lookup"><span data-stu-id="69b8c-1416">AppConfig</span></span>

* <span data-ttu-id="69b8c-1417">O grupo de comandos do recurso AppConfig foi adicionado para gerenciar os sinalizadores de recurso armazenados em uma Configuração de Aplicativos.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1417">Added appconfig feature command group to manage feature flags stored in an App Configuration.</span></span>
* <span data-ttu-id="69b8c-1418">Foi corrigido um bug secundário do comando de exportação para arquivo appconfig kv.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1418">Fixed minor bug for appconfig kv export to file command.</span></span> <span data-ttu-id="69b8c-1419">Foi interrompida a leitura de conteúdo do arquivo de destino durante a exportação.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1419">Stop reading dest file contents during export.</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-1420">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-1420">AppService</span></span>

* <span data-ttu-id="69b8c-1421">`az appservice plan create`: Foi adicionado o suporte para definir 'persitecalling' no comando appservice plan create.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1421">`az appservice plan create`: Added support to set 'persitescaling' on appservice plan create.</span></span>
* <span data-ttu-id="69b8c-1422">Foi corrigido um problema em que a operação webapp config ssl bind estava removendo as marcas existentes do recurso</span><span class="sxs-lookup"><span data-stu-id="69b8c-1422">Fixed an issue where webapp config ssl bind operation was removing existing tags from the resource</span></span>
* <span data-ttu-id="69b8c-1423">Foi adicionado o sinalizador `--build-remote` para `az functionapp deployment source config-zip` para dar suporte à ação de build remoto durante a implantação do aplicativo de funções.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1423">Added `--build-remote` flag for `az functionapp deployment source config-zip` to support remote build action during function app deployment.</span></span>
* <span data-ttu-id="69b8c-1424">Foi alterada a versão do nó padrão em aplicativos de funções para ~10 para Windows</span><span class="sxs-lookup"><span data-stu-id="69b8c-1424">Changed default node version on function apps to ~10 for Windows</span></span>
* <span data-ttu-id="69b8c-1425">A propriedade `--runtime-version` foi adicionada a `az functionapp create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1425">Added `--runtime-version` property to `az functionapp create`</span></span>

### <a name="arm"></a><span data-ttu-id="69b8c-1426">ARM</span><span class="sxs-lookup"><span data-stu-id="69b8c-1426">ARM</span></span>

* <span data-ttu-id="69b8c-1427">`az deployment/group deployment validate`: Foi adicionado o parâmetro `--handle-extended-json-format` para dar suporte a várias linhas e comentários no modelo JSON durante a implantação.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1427">`az deployment/group deployment validate`: Added `--handle-extended-json-format` parameter to support multiline and comments in json template when deployment.</span></span>
* <span data-ttu-id="69b8c-1428">O azure-mgmt-resource passou a usar a 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="69b8c-1428">Bumped azure-mgmt-resource to 2019-07-01</span></span>

### <a name="backup"></a><span data-ttu-id="69b8c-1429">Backup</span><span class="sxs-lookup"><span data-stu-id="69b8c-1429">Backup</span></span>

* <span data-ttu-id="69b8c-1430">Foi adicionado o suporte de backup aos Arquivos do Azure</span><span class="sxs-lookup"><span data-stu-id="69b8c-1430">Added AzureFiles backup support</span></span>

### <a name="compute"></a><span data-ttu-id="69b8c-1431">Computação</span><span class="sxs-lookup"><span data-stu-id="69b8c-1431">Compute</span></span>

* <span data-ttu-id="69b8c-1432">`az vm create`: foi adicionado um aviso ao especificar a rede acelerada e um adaptador de rede existente juntos.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1432">`az vm create`: Added warning when specifying accelerated networking and an existing NIC together.</span></span>
* <span data-ttu-id="69b8c-1433">`az vm create`: foi adicionado `--vmss` para especificar um conjunto de dimensionamento de máquinas virtuais existente ao qual a máquina virtual deve ser atribuída.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1433">`az vm create`: Added `--vmss` to specify an existing virtual machine scale set that the virtual machine should be assigned to.</span></span>
* <span data-ttu-id="69b8c-1434">`az vm/vmss create`: foi adicionada uma cópia local do arquivo de alias de imagem para que ele possa ser acessado em um ambiente de rede restrita.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1434">`az vm/vmss create`: Added a local copy of image alias file so that it can be accessed in a restricted network environment.</span></span>
* <span data-ttu-id="69b8c-1435">`az vmss create`: foi adicionado `--orchestration-mode` para especificar como as máquinas virtuais são gerenciadas pelo conjunto de dimensionamento.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1435">`az vmss create`: Added `--orchestration-mode` to specify how virtual machines are managed by the scale set.</span></span>
* <span data-ttu-id="69b8c-1436">`az vm/vmss update`: foi adicionado `--ultra-ssd-enabled` para permitir a atualização da configuração de SSD Ultra.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1436">`az vm/vmss update`: Added `--ultra-ssd-enabled` to allow updating ultra SSD setting.</span></span>
* <span data-ttu-id="69b8c-1437">[ALTERAÇÃO DA FALHA] `az vm extension set`: foi corrigido o bug em que os usuários não podiam definir uma extensão em uma VM com `--ids`.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1437">[BREAKING CHANGE] `az vm extension set`: Fixed bug where users could not set an extension on a VM with `--ids`.</span></span>
* <span data-ttu-id="69b8c-1438">Foram adicionados os novos comandos `az vm image terms accept/cancel/show` para gerenciar os termos de imagem do Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1438">Added new commands `az vm image terms accept/cancel/show` to manage Azure Marketplace image terms.</span></span>
* <span data-ttu-id="69b8c-1439">O VMAccessForLinux foi atualizado para a versão 1.5</span><span class="sxs-lookup"><span data-stu-id="69b8c-1439">Updated VMAccessForLinux to version 1.5</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="69b8c-1440">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="69b8c-1440">CosmosDB</span></span>

* <span data-ttu-id="69b8c-1441">[ALTERAÇÃO DA FALHA] `az sql container create`: `--partition-key-path` foi alterado para parâmetro obrigatório</span><span class="sxs-lookup"><span data-stu-id="69b8c-1441">[BREAKING CHANGE] `az sql container create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="69b8c-1442">[ALTERAÇÃO DA FALHA] `az gremlin graph create`: `--partition-key-path` foi alterado para parâmetro obrigatório</span><span class="sxs-lookup"><span data-stu-id="69b8c-1442">[BREAKING CHANGE] `az gremlin graph create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="69b8c-1443">`az sql container create`: Adição de `--unique-key-policy` e `--conflict-resolution-policy`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1443">`az sql container create`: Added `--unique-key-policy` and `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="69b8c-1444">`az sql container create/update`: o esquema padrão `--idx` foi atualizado</span><span class="sxs-lookup"><span data-stu-id="69b8c-1444">`az sql container create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="69b8c-1445">`gremlin graph create`: Adicionado `--conflict-resolution-policy`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1445">`gremlin graph create`: Added `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="69b8c-1446">`gremlin graph create/update`: o esquema padrão `--idx` foi atualizado</span><span class="sxs-lookup"><span data-stu-id="69b8c-1446">`gremlin graph create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="69b8c-1447">Erro de digitação corrigido na mensagem de ajuda</span><span class="sxs-lookup"><span data-stu-id="69b8c-1447">Fixed typo in help message</span></span>
* <span data-ttu-id="69b8c-1448">banco de dados: Foram adicionadas informações sobre preteridos</span><span class="sxs-lookup"><span data-stu-id="69b8c-1448">database: Added deprecation information</span></span>
* <span data-ttu-id="69b8c-1449">coleção: Foram adicionadas informações sobre preteridos</span><span class="sxs-lookup"><span data-stu-id="69b8c-1449">collection: Added deprecation information</span></span>

### <a name="iot"></a><span data-ttu-id="69b8c-1450">IoT</span><span class="sxs-lookup"><span data-stu-id="69b8c-1450">IoT</span></span>

* <span data-ttu-id="69b8c-1451">Um novo tipo de fonte de roteamento foi adicionado: DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="69b8c-1451">Added new routing source type: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="69b8c-1452">Foi corrigido o erro de recursos ausentes no `az iot hub create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1452">Fixed missing features in `az iot hub create`</span></span>

### <a name="key-vault"></a><span data-ttu-id="69b8c-1453">Key Vault</span><span class="sxs-lookup"><span data-stu-id="69b8c-1453">Key Vault</span></span>

* <span data-ttu-id="69b8c-1454">Foi corrigido um erro inesperado quando o arquivo de certificado não existe</span><span class="sxs-lookup"><span data-stu-id="69b8c-1454">Fixed an unexpected error when certificate file does not exist</span></span>
* <span data-ttu-id="69b8c-1455">Foi corrigido o problema em que o `az keyvault recover/purge` não funcionava</span><span class="sxs-lookup"><span data-stu-id="69b8c-1455">Fixed `az keyvault recover/purge` not working</span></span>

### <a name="netappfiles"></a><span data-ttu-id="69b8c-1456">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="69b8c-1456">NetAppFiles</span></span>

* <span data-ttu-id="69b8c-1457">O azure-mgmt-netapp foi atualizado para 0.6.0 para usar a versão da API 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1457">Upgraded azure-mgmt-netapp to 0.6.0 to use API version 2019-07-01.</span></span> <span data-ttu-id="69b8c-1458">Essa nova versão da API inclui:</span><span class="sxs-lookup"><span data-stu-id="69b8c-1458">This new API version includes:</span></span>

    - <span data-ttu-id="69b8c-1459">A criação de volume `--protocol-types` agora aceita "NFSv4.1" não "NFSv4"</span><span class="sxs-lookup"><span data-stu-id="69b8c-1459">Volume creation `--protocol-types` accepts now "NFSv4.1" not "NFSv4"</span></span>
    - <span data-ttu-id="69b8c-1460">A propriedade da política de exportação de volume agora é chamada 'nfsv41' não 'nfsv4'</span><span class="sxs-lookup"><span data-stu-id="69b8c-1460">Volume export policy property now named 'nfsv41' not 'nfsv4'</span></span>
    - <span data-ttu-id="69b8c-1461">O volume `--creation-token` foi renomeado para `--file-path`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1461">Volume `--creation-token` renamed to `--file-path`</span></span>
    - <span data-ttu-id="69b8c-1462">A data de criação do instantâneo agora é chamada apenas de 'criação'</span><span class="sxs-lookup"><span data-stu-id="69b8c-1462">Snapshot creation date now named just 'created'</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-1463">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-1463">Network</span></span>

* <span data-ttu-id="69b8c-1464">`az network private-dns link vnet create/update`: suporte à vinculação de rede virtual entre locatários.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1464">`az network private-dns link vnet create/update`: Support cross-tenant virtual network linking.</span></span>
* <span data-ttu-id="69b8c-1465">[ALTERAÇÃO DA FALHA] `az network vnet subnet list`: `--resource-group` e `--vnet-name` foram alterados para serem obrigatórios agora.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1465">[BREAKING CHANGE] `az network vnet subnet list`: Changed `--resource-group` and `--vnet-name` to be required now.</span></span>
* <span data-ttu-id="69b8c-1466">`az network public-ip prefix create`: Suporte adicionado para especificar a versão do endereço IP (IPv4, IPv6) durante a criação</span><span class="sxs-lookup"><span data-stu-id="69b8c-1466">`az network public-ip prefix create`: Added support to specify IP address version (IPv4, IPv6) when creation</span></span>
* <span data-ttu-id="69b8c-1467">O azure-mgmt-network foi atualizado para 7.0.0 e a api-version para 2019-09-01</span><span class="sxs-lookup"><span data-stu-id="69b8c-1467">Bumped azure-mgmt-network to 7.0.0 and api-version to 2019-09-01</span></span>
* <span data-ttu-id="69b8c-1468">`az network vrouter`: Suporte adicionado para o novo roteador virtual de serviço e o emparelhamento do roteador virtual</span><span class="sxs-lookup"><span data-stu-id="69b8c-1468">`az network vrouter`: Added support for new service virtual router and virtual router peering</span></span>
* <span data-ttu-id="69b8c-1469">`az network express-route gateway connection`: Adicionado o suporte para `--internet-security`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1469">`az network express-route gateway connection`: Added support for `--internet-security`</span></span>

### <a name="profile"></a><span data-ttu-id="69b8c-1470">Perfil</span><span class="sxs-lookup"><span data-stu-id="69b8c-1470">Profile</span></span>

* <span data-ttu-id="69b8c-1471">Foi corrigido o problema em que o `az account get-access-token --resource-type ms-graph` não funcionava</span><span class="sxs-lookup"><span data-stu-id="69b8c-1471">Fixed `az account get-access-token --resource-type ms-graph` not working</span></span>
* <span data-ttu-id="69b8c-1472">O aviso foi removido de `az login`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1472">Removed warning from `az login`</span></span>

### <a name="rbac"></a><span data-ttu-id="69b8c-1473">RBAC</span><span class="sxs-lookup"><span data-stu-id="69b8c-1473">RBAC</span></span>

* <span data-ttu-id="69b8c-1474">Foi corrigido o problema em que o `az ad app update --id {} --display-name {}` não funcionava</span><span class="sxs-lookup"><span data-stu-id="69b8c-1474">Fixed `az ad app update --id {} --display-name {}` doesn't work</span></span>

### <a name="servicefabric"></a><span data-ttu-id="69b8c-1475">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="69b8c-1475">ServiceFabric</span></span>

* <span data-ttu-id="69b8c-1476">`az sf cluster create`: foi corrigido um problema que ocorria ao modificar o VMSS de computação do template.json do Linux e do Windows, do Service Fabric, de discos Standard para discos gerenciados</span><span class="sxs-lookup"><span data-stu-id="69b8c-1476">`az sf cluster create`: Fixed an issue by modifying service fabric linux and windows template.json compute vmss from standard to managed disks</span></span>

### <a name="sql"></a><span data-ttu-id="69b8c-1477">SQL</span><span class="sxs-lookup"><span data-stu-id="69b8c-1477">SQL</span></span>

* <span data-ttu-id="69b8c-1478">Os parâmetros `--compute-model`, `--auto-pause-delay` e `--min-capacity` foram adicionados para dar suporte a operações CRUD para a nova oferta de Banco de Dados SQL: Modelo de computação sem servidor.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1478">Added `--compute-model`, `--auto-pause-delay`, and `--min-capacity` parameters to support CRUD operations for new SQL Database offering: Serverless compute model.</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-1479">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-1479">Storage</span></span>

* <span data-ttu-id="69b8c-1480">`az storage account create/update`: Foram adicionados o parâmetro --enable-files-adds e o grupo Argumentos de Propriedades do Azure Active Directory para dar suporte à Autenticação do Serviço de Domínio do Active Directory do Arquivos do Azure</span><span class="sxs-lookup"><span data-stu-id="69b8c-1480">`az storage account create/update`: Added --enable-files-adds parameter and Azure Active Directory Properties Argument group to support Azure Files Active Directory Domain Service Authentication</span></span>
* <span data-ttu-id="69b8c-1481">O `az storage account keys list/renew` foi expandido para dar suporte à listagem ou à regeneração de chaves Kerberos da conta de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1481">Expanded `az storage account keys list/renew` to support listing or regenerating Kerberos keys of storage account.</span></span>

## <a name="october-15-2019"></a><span data-ttu-id="69b8c-1482">15 de outubro de 2019</span><span class="sxs-lookup"><span data-stu-id="69b8c-1482">October 15, 2019</span></span>

<span data-ttu-id="69b8c-1483">Versão 2.0.75</span><span class="sxs-lookup"><span data-stu-id="69b8c-1483">Version 2.0.75</span></span>

### <a name="aks"></a><span data-ttu-id="69b8c-1484">AKS</span><span class="sxs-lookup"><span data-stu-id="69b8c-1484">AKS</span></span>

* <span data-ttu-id="69b8c-1485">Alteração do valor padrão `--load-balancer-sku` para `standard` se for compatível com a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="69b8c-1485">Changed `--load-balancer-sku` default value to `standard` if supported by the kubernetes version</span></span>
* <span data-ttu-id="69b8c-1486">Alteração do valor padrão `--vm-set-type` para `virtualmachinescalesets` se for compatível com a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="69b8c-1486">Changed `--vm-set-type` default value to `virtualmachinescalesets` if supported by the kubernetes version</span></span>

### <a name="ams"></a><span data-ttu-id="69b8c-1487">AMS</span><span class="sxs-lookup"><span data-stu-id="69b8c-1487">AMS</span></span>

* <span data-ttu-id="69b8c-1488">[ALTERAÇÃO SIGNIFICATIVA] Alteração do nome de `job start` para `job create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1488">[BREAKING CHANGE] Changed the name of `job start` to `job create`</span></span>
* <span data-ttu-id="69b8c-1489">[ALTERAÇÃO SIGNIFICATIVA] Alteração do parâmetro `--ask` de `content-key-policy create` para usar uma cadeia de 32 caracteres hexadecimais em vez do UTF8</span><span class="sxs-lookup"><span data-stu-id="69b8c-1489">[BREAKING CHANGE] Changed the `--ask` parameter of `content-key-policy create` to use a 32-character hex string instead of UTF8</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-1490">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-1490">AppService</span></span>

* <span data-ttu-id="69b8c-1491">Adição dos comandos `webapp config access-restriction show|set|add|remove`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1491">Added commands `webapp config access-restriction show|set|add|remove`</span></span>
* <span data-ttu-id="69b8c-1492">Adição de um melhor tratamento de erro a `webapp up`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1492">Added better error handling to `webapp up`</span></span>
* <span data-ttu-id="69b8c-1493">Adição de suporte do SKU `Isolated` para `appservice plan update`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1493">Added support for `Isolated` SKU to `appservice plan update`</span></span>

### <a name="arm"></a><span data-ttu-id="69b8c-1494">ARM</span><span class="sxs-lookup"><span data-stu-id="69b8c-1494">ARM</span></span>

* <span data-ttu-id="69b8c-1495">Adição do parâmetro `--handle-extended-json-format``deployment create` para dar suporte a várias linhas e a comentários no modelo json</span><span class="sxs-lookup"><span data-stu-id="69b8c-1495">Added `--handle-extended-json-format` parameter `deployment create` to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="69b8c-1496">Computação</span><span class="sxs-lookup"><span data-stu-id="69b8c-1496">Compute</span></span>

* <span data-ttu-id="69b8c-1497">Parâmetro `--enable-agent` adicionado a `vm create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1497">Added `--enable-agent` parameter to `vm create`</span></span>
* <span data-ttu-id="69b8c-1498">Alteração de `vm create` para usar um SKU de IP público padrão automaticamente ao usar zonas</span><span class="sxs-lookup"><span data-stu-id="69b8c-1498">Changed `vm create` to use standard public IP SKU automatically when using zones</span></span>
* <span data-ttu-id="69b8c-1499">Alteração de `vm create` para criar automaticamente um nome de computador válido para uma VM, caso nenhum tenha sido fornecido</span><span class="sxs-lookup"><span data-stu-id="69b8c-1499">Changed `vm create` to automatically create a valid computer name for a VM if none is provided</span></span>
* <span data-ttu-id="69b8c-1500">Adição do parâmetro `--computer-name-prefix` a `vmss create` para dar suporte ao prefixo de nome de computador personalizado de máquinas virtuais no VMSS</span><span class="sxs-lookup"><span data-stu-id="69b8c-1500">Added `--computer-name-prefix` parameter to `vmss create` to support custom computer name prefix of virtual machines in the VMSS</span></span>
* <span data-ttu-id="69b8c-1501">Adicione o parâmetro `--workspace` a `vm create` para habilitar o workspace de análise de logs automaticamente</span><span class="sxs-lookup"><span data-stu-id="69b8c-1501">Add `--workspace` parameter to `vm create` to enable log analytics workspace automatically</span></span>
* <span data-ttu-id="69b8c-1502">Versão de API de galerias atualizadas para 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="69b8c-1502">Updated galleries API version to 2019-07-01</span></span>

### <a name="core"></a><span data-ttu-id="69b8c-1503">Núcleo</span><span class="sxs-lookup"><span data-stu-id="69b8c-1503">Core</span></span>

* <span data-ttu-id="69b8c-1504">Adição da verificação de sintaxe para o parâmetro `--set` no comando de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="69b8c-1504">Added syntax check for `--set` parameter in generic update command</span></span>

### <a name="iot"></a><span data-ttu-id="69b8c-1505">IoT</span><span class="sxs-lookup"><span data-stu-id="69b8c-1505">IoT</span></span>

* <span data-ttu-id="69b8c-1506">Correção de um problema em que o `iot hub show` retornaria incorretamente um erro com "recurso não encontrado"</span><span class="sxs-lookup"><span data-stu-id="69b8c-1506">Fixed an issue where `iot hub show` would incorrectly error with "resource not found"</span></span>

### <a name="monitor"></a><span data-ttu-id="69b8c-1507">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="69b8c-1507">Monitor</span></span>

* <span data-ttu-id="69b8c-1508">Adição de suporte para CRUD a `monitor log-analytics workspace`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1508">Added support for CRUD to `monitor log-analytics workspace`</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-1509">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-1509">Network</span></span>

* <span data-ttu-id="69b8c-1510">Adição de suporte para vinculação virtual entre locatários para `network private-dns link vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1510">Added support for cross-tenant virtual linking to `network private-dns link vnet [create|update]`</span></span>
* <span data-ttu-id="69b8c-1511">[ALTERAÇÃO SIGNIFICATIVA] Alteração de `network vnet subnet list` para exigir os parâmetros `--resource-group` e `--vnet-name`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1511">[BREAKING CHANGE] Changed `network vnet subnet list` to require `--resource-group` and `--vnet-name` parameters</span></span>

### <a name="sql"></a><span data-ttu-id="69b8c-1512">SQL</span><span class="sxs-lookup"><span data-stu-id="69b8c-1512">SQL</span></span>

* <span data-ttu-id="69b8c-1513">Adição de comandos a `sql mi ad-admin` que dão suporte à configuração de um administrador do AAD em instâncias gerenciadas</span><span class="sxs-lookup"><span data-stu-id="69b8c-1513">Added commands to `sql mi ad-admin` that support setting an AAD administrator on managed instances</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-1514">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-1514">Storage</span></span>

* <span data-ttu-id="69b8c-1515">Adição do parâmetro `--preserve-s2s-access-tier``storage copy` para preservar a camada de acesso durante a cópia do serviço para serviço</span><span class="sxs-lookup"><span data-stu-id="69b8c-1515">Added `--preserve-s2s-access-tier` parameter `storage copy` to preserve access tier during service to service copy</span></span>
* <span data-ttu-id="69b8c-1516">Adição do parâmetro `--enable-large-file-share` a `storage account [create|update]` para dar suporte a compartilhamentos de arquivos grandes para a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-1516">Added `--enable-large-file-share` parameter to `storage account [create|update]` to support large file shares for storage account</span></span>

## <a name="september-24-2019"></a><span data-ttu-id="69b8c-1517">24 de setembro de 2019</span><span class="sxs-lookup"><span data-stu-id="69b8c-1517">September 24, 2019</span></span>

<span data-ttu-id="69b8c-1518">Versão 2.0.74</span><span class="sxs-lookup"><span data-stu-id="69b8c-1518">Version 2.0.74</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-1519">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-1519">ACR</span></span>

* <span data-ttu-id="69b8c-1520">Inclusão de um parâmetro `--type` obrigatório em `acr config retention update`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1520">Added a required `--type` parameter to `acr config retention update`</span></span>
* <span data-ttu-id="69b8c-1521">[ALTERAÇÃO SIGNIFICATIVA] O parâmetro renomeado `--name -n` foi alterado para `--registry -r ` para o grupo de comando `acr config`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1521">[BREAKING CHANGE] Renamed parameter `--name -n` changed to `--registry -r ` for `acr config` command group</span></span>

### <a name="aks"></a><span data-ttu-id="69b8c-1522">AKS</span><span class="sxs-lookup"><span data-stu-id="69b8c-1522">AKS</span></span>

* <span data-ttu-id="69b8c-1523">Inclusão do parâmetro `--load-balancer-sku` no comando `aks create`, o que permite criar um cluster do AKS com SLB</span><span class="sxs-lookup"><span data-stu-id="69b8c-1523">Added `--load-balancer-sku` parameter to `aks create` command, which allows for creating AKS cluster with SLB</span></span>
* <span data-ttu-id="69b8c-1524">Inclusão dos parâmetros `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` e `--load-balancer-outbound-ip-prefixes` nos comandos `aks [create|update]`, o que permite atualizar o perfil do balanceador de carga de um cluster do AKS com SLB</span><span class="sxs-lookup"><span data-stu-id="69b8c-1524">Added `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` and `--load-balancer-outbound-ip-prefixes` parameters to `aks [create|update]` commands, which allow for updating load balancer profile of an AKS cluster with SLB</span></span>
* <span data-ttu-id="69b8c-1525">Inclusão do parâmetro `--vm-set-type` no comando `aks create`, o que permite especificar os tipos de VM de um cluster do AKS (vmas ou vmss)</span><span class="sxs-lookup"><span data-stu-id="69b8c-1525">Added `--vm-set-type` parameter to `aks create` command, which allows to specify vm types of an AKS Cluster (vmas or vmss)</span></span>

### <a name="arm"></a><span data-ttu-id="69b8c-1526">ARM</span><span class="sxs-lookup"><span data-stu-id="69b8c-1526">ARM</span></span>

* <span data-ttu-id="69b8c-1527">Inclusão do parâmetro `--handle-extended-json-format` no comando `group deployment create` para compatibilidade com várias linhas e comentários no modelo JSON</span><span class="sxs-lookup"><span data-stu-id="69b8c-1527">Added `--handle-extended-json-format` parameter to `group deployment create` command to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="69b8c-1528">Computação</span><span class="sxs-lookup"><span data-stu-id="69b8c-1528">Compute</span></span>

* <span data-ttu-id="69b8c-1529">Inclusão do parâmetro `--terminate-notification-time` nos comandos `vmss [create|update]` para compatibilidade com a capacidade de configurar o encerramento de eventos agendados</span><span class="sxs-lookup"><span data-stu-id="69b8c-1529">Added `--terminate-notification-time` parameter to `vmss [create|update]` commands to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="69b8c-1530">Inclusão do parâmetro `--enable-terminate-notification` no comando `vmss update` para compatibilidade com a capacidade de configurar o encerramento de eventos agendados</span><span class="sxs-lookup"><span data-stu-id="69b8c-1530">Added `--enable-terminate-notification` parameter to `vmss update` command to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="69b8c-1531">Inclusão dos parâmetros `--priority,`, `--eviction-policy,` e `--max-billing` nos comandos `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1531">Added `--priority,` `--eviction-policy,` `--max-billing` parameters to `[vm|vmss] create` commands</span></span>
* <span data-ttu-id="69b8c-1532">Alteração de `disk create` para permitir a especificação do tamanho exato do carregamento de disco</span><span class="sxs-lookup"><span data-stu-id="69b8c-1532">Changed `disk create` to allow specifying the exact size of the disk upload</span></span>
* <span data-ttu-id="69b8c-1533">Inclusão de compatibilidade com instantâneos incrementais para discos gerenciados para `snapshot create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1533">Added support for incremental snapshots for managed disks to `snapshot create`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="69b8c-1534">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="69b8c-1534">Cosmos DB</span></span>

* <span data-ttu-id="69b8c-1535">Inclusão do parâmetro `--type <key-type>` no comando `cosmosdb keys list` para mostrar a chave, as chaves somente leitura ou cadeias de conexão</span><span class="sxs-lookup"><span data-stu-id="69b8c-1535">Added `--type <key-type>` parameter to `cosmosdb keys list` command to show key, read only keys or connection strings</span></span>
* <span data-ttu-id="69b8c-1536">Adicionado o comando `cosmosdb keys regenerate`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1536">Added `cosmosdb keys regenerate` command</span></span>
* <span data-ttu-id="69b8c-1537">[PRETERIDO] Comandos `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` e `cosmosdb list-read-only-keys` preteridos</span><span class="sxs-lookup"><span data-stu-id="69b8c-1537">[DEPRECATED] Deprecated `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` and `cosmosdb list-read-only-keys` commands</span></span>

### <a name="eventgrid"></a><span data-ttu-id="69b8c-1538">EventGrid</span><span class="sxs-lookup"><span data-stu-id="69b8c-1538">EventGrid</span></span>

* <span data-ttu-id="69b8c-1539">Correção do texto de ajuda do ponto de extremidade para fazer referência ao parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="69b8c-1539">Fixed the endpoint help text to refer to the right parameter</span></span>

### <a name="key-vault"></a><span data-ttu-id="69b8c-1540">Key Vault</span><span class="sxs-lookup"><span data-stu-id="69b8c-1540">Key Vault</span></span>

* <span data-ttu-id="69b8c-1541">Correção do problema em que fazer logon com um locatário (`login -t`) poderia causar uma falha no `keyvault create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1541">Fixed issue where logging in with a tenant (`login -t`) could cause `keyvault create` to fail</span></span>

### <a name="monitor"></a><span data-ttu-id="69b8c-1542">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="69b8c-1542">Monitor</span></span>

* <span data-ttu-id="69b8c-1543">Correção do problema em que o caractere `:` não era permitido no argumento `--condition` para `monitor metrics alert create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1543">Fixed issue where `:` character was not allowed in `--condition` argument to `monitor metrics alert create`</span></span>

### <a name="policy"></a><span data-ttu-id="69b8c-1544">Política</span><span class="sxs-lookup"><span data-stu-id="69b8c-1544">Policy</span></span>

* <span data-ttu-id="69b8c-1545">Inclusão de compatibilidade com a API de Política, versão de 01/06/2019</span><span class="sxs-lookup"><span data-stu-id="69b8c-1545">Added support for Policy API version 2019-06-01</span></span>
* <span data-ttu-id="69b8c-1546">Inclusão do parâmetro `--enforcement-mode` no comando `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1546">Added `--enforcement-mode` parameter to `policy assignment create` command</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-1547">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-1547">Storage</span></span>

* <span data-ttu-id="69b8c-1548">Inclusão do parâmetro `--blob-type` no comando `az storage copy`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1548">Added `--blob-type` parameter to `az storage copy` command</span></span>

## <a name="september-10-2019"></a><span data-ttu-id="69b8c-1549">10 de setembro de 2019</span><span class="sxs-lookup"><span data-stu-id="69b8c-1549">September 10, 2019</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-1550">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-1550">ACR</span></span>

* <span data-ttu-id="69b8c-1551">Adição do grupo de comandos `acr config retention` para configurar a política de retenção</span><span class="sxs-lookup"><span data-stu-id="69b8c-1551">Added command group `acr config retention` to configure retention policy</span></span>

### <a name="aks"></a><span data-ttu-id="69b8c-1552">AKS</span><span class="sxs-lookup"><span data-stu-id="69b8c-1552">AKS</span></span>

* <span data-ttu-id="69b8c-1553">Adição de suporte para integração do ACR com os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="69b8c-1553">Added support for ACR integration with the following commands:</span></span>
  * <span data-ttu-id="69b8c-1554">Adição do parâmetro `--attach-acr` a `aks [create|update]` para anexar um ACR a um cluster do AKS</span><span class="sxs-lookup"><span data-stu-id="69b8c-1554">Added `--attach-acr` parameter to `aks [create|update]` to attach an ACR to an AKS cluster</span></span>
  * <span data-ttu-id="69b8c-1555">Adição do parâmetro `--detach-acr` a `aks update` para desanexar o ACR de um cluster do AKS</span><span class="sxs-lookup"><span data-stu-id="69b8c-1555">Added `--detach-acr` parameter to `aks update` to detach the ACR from an AKS cluster</span></span>

### <a name="arm"></a><span data-ttu-id="69b8c-1556">ARM</span><span class="sxs-lookup"><span data-stu-id="69b8c-1556">ARM</span></span>

* <span data-ttu-id="69b8c-1557">Atualização para uso da versão de API 2019-05-10</span><span class="sxs-lookup"><span data-stu-id="69b8c-1557">Updated to use API version 2019-05-10</span></span>

### <a name="batch"></a><span data-ttu-id="69b8c-1558">Lote</span><span class="sxs-lookup"><span data-stu-id="69b8c-1558">Batch</span></span>

* <span data-ttu-id="69b8c-1559">Adição de novas definições de configuração JSON de `--json-file` para `batch pool create`:</span><span class="sxs-lookup"><span data-stu-id="69b8c-1559">Added new JSON configuration settings to `--json-file` for `batch pool create`:</span></span>
  * <span data-ttu-id="69b8c-1560">Adição de `MountConfigurations` para montagens do sistema de arquivos (confira https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body para obter detalhes)</span><span class="sxs-lookup"><span data-stu-id="69b8c-1560">Added `MountConfigurations` for file system mounts (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
  * <span data-ttu-id="69b8c-1561">Adição da propriedade opcional `publicIPs` a `NetworkConfiguration` para IPs públicos em pools (confira https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body para obter detalhes)</span><span class="sxs-lookup"><span data-stu-id="69b8c-1561">Added optional property `publicIPs` on `NetworkConfiguration` for public IPs on pools (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
* <span data-ttu-id="69b8c-1562">Adição de suporte para galerias de imagens compartilhadas a `--image`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1562">Added support for shared image galleries to `--image`</span></span>
* <span data-ttu-id="69b8c-1563">[ALTERAÇÃO SIGNIFICATIVA] Alteração do valor padrão de `--start-task-wait-for-success` em `batch pool create` para `true`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1563">[BREAKING CHANGE] Changed default value of `--start-task-wait-for-success` on `batch pool create` to be `true`</span></span>
* <span data-ttu-id="69b8c-1564">[ALTERAÇÃO SIGNIFICATIVA] Alteração do valor padrão de `Scope` em `AutoUserSpecification` para sempre ser Pool (anteriormente, `Task` em nós do Windows e `Pool` em nós do Linux)</span><span class="sxs-lookup"><span data-stu-id="69b8c-1564">[BREAKING CHANGE] Changed default value for `Scope` on `AutoUserSpecification` to always be Pool (was `Task` on Windows nodes, `Pool` on Linux nodes)</span></span>
  * <span data-ttu-id="69b8c-1565">Esse argumento só pode ser definido em uma configuração JSON com `--json-file`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1565">This argument can only be set from a JSON configuration with `--json-file`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="69b8c-1566">HDInsight</span><span class="sxs-lookup"><span data-stu-id="69b8c-1566">HDInsight</span></span>

* <span data-ttu-id="69b8c-1567">Versão de GA</span><span class="sxs-lookup"><span data-stu-id="69b8c-1567">GA release</span></span>
* <span data-ttu-id="69b8c-1568">[ALTERAÇÃO SIGNIFICATIVA] Alteração do parâmetro `--workernode-count/-c` de `az hdinsight resize` para ser obrigatório.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1568">[BREAKING CHANGE] Changed parameter `--workernode-count/-c` of `az hdinsight resize` to be required.</span></span>

### <a name="key-vault"></a><span data-ttu-id="69b8c-1569">Key Vault</span><span class="sxs-lookup"><span data-stu-id="69b8c-1569">Key Vault</span></span>

* <span data-ttu-id="69b8c-1570">Correção do problema em que as sub-redes não podiam ser excluídas das regras da rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-1570">Fixed issue where subnets couldn't be deleted from network rules</span></span>
* <span data-ttu-id="69b8c-1571">Correção do problema em que sub-redes e endereços IP duplicados podiam ser adicionados às regras da rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-1571">Fixed issue where duplicated subnets and IP addresses could be added to network rules</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-1572">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-1572">Network</span></span>

* <span data-ttu-id="69b8c-1573">Adição do parâmetro `--interval` a `network watcher flow-log` para definir o valor do intervalo de análise de tráfego</span><span class="sxs-lookup"><span data-stu-id="69b8c-1573">Added `--interval` parameter to `network watcher flow-log` to set traffic analysis interval value</span></span>
* <span data-ttu-id="69b8c-1574">Adição de `network application-gateway identity` para gerenciar a identidade do gateway</span><span class="sxs-lookup"><span data-stu-id="69b8c-1574">Added `network application-gateway identity` to manage gateway identity</span></span>
* <span data-ttu-id="69b8c-1575">Adição de suporte para definir a ID do Key Vault como `network application-gateway ssl-cert`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1575">Added support for setting Key Vault ID to `network application-gateway ssl-cert`</span></span>
* <span data-ttu-id="69b8c-1576">Adicionado `network express-route peering peer-connection [show|list]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1576">Added `network express-route peering peer-connection [show|list]`</span></span>

### <a name="policy"></a><span data-ttu-id="69b8c-1577">Política</span><span class="sxs-lookup"><span data-stu-id="69b8c-1577">Policy</span></span>

* <span data-ttu-id="69b8c-1578">Atualização para uso da versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="69b8c-1578">Updated to use API version 2019-01-01</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="69b8c-1579">27 de agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="69b8c-1579">August 27, 2019</span></span>

<span data-ttu-id="69b8c-1580">Versão 2.0.72</span><span class="sxs-lookup"><span data-stu-id="69b8c-1580">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-1581">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-1581">ACR</span></span>

* <span data-ttu-id="69b8c-1582">[ALTERAÇÃO SIGNIFICATIVA] Remoção da compatibilidade com o SKU `classic`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1582">[BREAKING CHANGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="69b8c-1583">Gerenciamento de API</span><span class="sxs-lookup"><span data-stu-id="69b8c-1583">API Management</span></span>

* <span data-ttu-id="69b8c-1584">[VERSÃO PRÉVIA] Adição do grupo de comandos `apim`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1584">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-1585">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-1585">AppService</span></span>

* <span data-ttu-id="69b8c-1586">Correção do problema com o comando `webapp webjob continuous start` ao especificar um slot</span><span class="sxs-lookup"><span data-stu-id="69b8c-1586">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="69b8c-1587">Alteração de `webapp up` para detectar a pasta `env` e removê-la do arquivo usado para implantação</span><span class="sxs-lookup"><span data-stu-id="69b8c-1587">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="69b8c-1588">Keyvault</span><span class="sxs-lookup"><span data-stu-id="69b8c-1588">Keyvault</span></span>

* <span data-ttu-id="69b8c-1589">Correção de um bug no `keyvault secret set` que ignorava o argumento `--expires`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1589">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-1590">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-1590">Network</span></span>

* <span data-ttu-id="69b8c-1591">Adição de suporte para endereços IPv6 a argumentos `--private-ip-address-version`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1591">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="69b8c-1592">Adição de novos comandos `network private-endpoint [create|update|list-types]` para o gerenciamento de ponto de extremidade privado</span><span class="sxs-lookup"><span data-stu-id="69b8c-1592">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="69b8c-1593">Adição do grupo de comandos `network private-link-service`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1593">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="69b8c-1594">Adicionados os argumentos `--private-endpoint-network-policies` e `--private-link-service-network-policies` para `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1594">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="69b8c-1595">RBAC</span><span class="sxs-lookup"><span data-stu-id="69b8c-1595">RBAC</span></span>

* <span data-ttu-id="69b8c-1596">Correção de um problema com `ad app update --homepage` em que a página inicial não era atualizada</span><span class="sxs-lookup"><span data-stu-id="69b8c-1596">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="69b8c-1597">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="69b8c-1597">ServiceFabric</span></span>

* <span data-ttu-id="69b8c-1598">Adição de suporte para nomes de Key Vault grafados com maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="69b8c-1598">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="69b8c-1599">Correção de um problema ao usar certificados no Key Vault</span><span class="sxs-lookup"><span data-stu-id="69b8c-1599">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="69b8c-1600">Correção de um problema com o uso de arquivos de certificado PFX</span><span class="sxs-lookup"><span data-stu-id="69b8c-1600">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="69b8c-1601">Correção de um problema com `sf cluster certificate add` quando o grupo de recursos do Key Vault não era especificado</span><span class="sxs-lookup"><span data-stu-id="69b8c-1601">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="69b8c-1602">Correção de um problema em que `sf cluster set` não funcionava</span><span class="sxs-lookup"><span data-stu-id="69b8c-1602">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="69b8c-1603">SignalR</span><span class="sxs-lookup"><span data-stu-id="69b8c-1603">SignalR</span></span>

* <span data-ttu-id="69b8c-1604">Novos comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="69b8c-1604">Added new commands:</span></span>
  * <span data-ttu-id="69b8c-1605">`signalr cors`: gerenciar CORS do SignalR</span><span class="sxs-lookup"><span data-stu-id="69b8c-1605">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="69b8c-1606">`signalr restart`: reiniciar um serviço do SignalR</span><span class="sxs-lookup"><span data-stu-id="69b8c-1606">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="69b8c-1607">`signalr update`: atualizar um serviço do SignalR</span><span class="sxs-lookup"><span data-stu-id="69b8c-1607">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="69b8c-1608">Adicionado o argumento `--service-mode` para `signalr create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1608">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-1609">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-1609">Storage</span></span>

* <span data-ttu-id="69b8c-1610">Adicionado o comando `storage account revoke-delegation-keys`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1610">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="69b8c-1611">13 de agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="69b8c-1611">August 13, 2019</span></span>

<span data-ttu-id="69b8c-1612">Versão 2.0.71</span><span class="sxs-lookup"><span data-stu-id="69b8c-1612">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-1613">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-1613">AppService</span></span>

* <span data-ttu-id="69b8c-1614">Um problema de falha de slots com os comandos `webapp webjob continuous` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="69b8c-1614">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="69b8c-1615">BotService</span><span class="sxs-lookup"><span data-stu-id="69b8c-1615">BotService</span></span>

* <span data-ttu-id="69b8c-1616">[ALTERAÇÃO SIGNIFICATIVA] O suporte para a criação de bots SDK v3 foi removido</span><span class="sxs-lookup"><span data-stu-id="69b8c-1616">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="69b8c-1617">CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="69b8c-1617">CognitiveServices</span></span>

* <span data-ttu-id="69b8c-1618">Adicionados os comandos `cognitiveservices account network-rule`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1618">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="69b8c-1619">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="69b8c-1619">Cosmos DB</span></span>

* <span data-ttu-id="69b8c-1620">Removido o aviso ao atualizar vários locais de gravação</span><span class="sxs-lookup"><span data-stu-id="69b8c-1620">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="69b8c-1621">Foram adicionados os comandos CRUD para o CosmosDB SQL, MongoDB, Cassandra, Gremlin e Recursos de tabela e taxa de transferência do recurso</span><span class="sxs-lookup"><span data-stu-id="69b8c-1621">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="69b8c-1622">HDInsight</span><span class="sxs-lookup"><span data-stu-id="69b8c-1622">HDInsight</span></span>

<span data-ttu-id="69b8c-1623">Esta versão contém um grande número de alterações da falha.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1623">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="69b8c-1624">[ALTERAÇÃO SIGNIFICATIVA] Parâmetros renomeados para `hdinsight create`:</span><span class="sxs-lookup"><span data-stu-id="69b8c-1624">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="69b8c-1625">`--storage-default-container` renomeado para `--storage-container`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1625">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="69b8c-1626">`--storage-default-filesystem` renomeado para `--storage-filesystem`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1626">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="69b8c-1627">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--name` de `application create` foi alterado para representar o nome do aplicativo em vez do nome do cluster</span><span class="sxs-lookup"><span data-stu-id="69b8c-1627">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="69b8c-1628">O argumento `--cluster-name` foi adicionado a `application create` para substituir a funcionalidade `--name` antiga</span><span class="sxs-lookup"><span data-stu-id="69b8c-1628">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="69b8c-1629">[ALTERAÇÃO SIGNIFICATIVA] Parâmetros renomeados para `application create`:</span><span class="sxs-lookup"><span data-stu-id="69b8c-1629">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="69b8c-1630">`--application-type` renomeado para `--type`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1630">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="69b8c-1631">`--marketplace-identifier` renomeado para `--marketplace-id`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1631">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="69b8c-1632">`--https-endpoint-access-mode` renomeado para `--access-mode`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1632">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="69b8c-1633">Renomeado de `--https-endpoint-destination-port` para `--destination-port`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1633">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="69b8c-1634">[ALTERAÇÃO SIGNIFICATIVA] Parâmetros removidos para `application create`:</span><span class="sxs-lookup"><span data-stu-id="69b8c-1634">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="69b8c-1635">[ALTERAÇÃO DA FALHA] Renomeado de `--target-instance-count` para `--workernode-count` para `hdinsight resize`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1635">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="69b8c-1636">[ALTERAÇÃO SIGNIFICATIVA] Todos os comandos no grupo `hdinsight script-action` foram alterados para usar o parâmetro `--name` como o nome da ação de script.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1636">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="69b8c-1637">O argumento `--cluster-name` foi adicionado a todos os comandos `hdinsight script-action` para substituir a funcionalidade `--name` antiga</span><span class="sxs-lookup"><span data-stu-id="69b8c-1637">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="69b8c-1638">[ALTERAÇÃO SIGNIFICATIVA] Renomeado de `--script-execution-id` para `--execution-id` para todos os comandos `hdinsight script-action`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1638">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="69b8c-1639">[ALTERAÇÃO SIGNIFICATIVA]`hdinsight script-action show` renomeado para `hdinsight script-action show-execution-details`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1639">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="69b8c-1640">[ALTERAÇÃO DA FALHA] Os parâmetros foram alterados para `hdinsight script-action execute --roles` para serem separados por espaços em vez de separados por vírgula</span><span class="sxs-lookup"><span data-stu-id="69b8c-1640">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="69b8c-1641">[ALTERAÇÃO SIGNIFICATIVA] O parâmetro `--persisted` de `hdinsight script-action list` foi removido</span><span class="sxs-lookup"><span data-stu-id="69b8c-1641">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="69b8c-1642">O parâmetro `hdinsight create --cluster-configurations` foi alterado para aceitar um caminho para um arquivo JSON local ou uma cadeia de caracteres JSON</span><span class="sxs-lookup"><span data-stu-id="69b8c-1642">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="69b8c-1643">Adicionado o comando `hdinsight script-action list-execution-history`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1643">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="69b8c-1644">Alterado `hdinsight monitor enable --workspace` para aceitar uma ID do workspace ou nome do workspace do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="69b8c-1644">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="69b8c-1645">O argumento `hdinsight monitor enable --primary-key`, que será necessário caso uma ID do workspace seja fornecida como o parâmetro, foi adicionado</span><span class="sxs-lookup"><span data-stu-id="69b8c-1645">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="69b8c-1646">Foram adicionados mais exemplos e atualização das descrições das mensagens de erro</span><span class="sxs-lookup"><span data-stu-id="69b8c-1646">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="69b8c-1647">Interativo</span><span class="sxs-lookup"><span data-stu-id="69b8c-1647">Interactive</span></span>

* <span data-ttu-id="69b8c-1648">Um erro no carregamento foi corrigido</span><span class="sxs-lookup"><span data-stu-id="69b8c-1648">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="69b8c-1649">Kubernetes</span><span class="sxs-lookup"><span data-stu-id="69b8c-1649">Kubernetes</span></span>

* <span data-ttu-id="69b8c-1650">Alterado para usar `https` se a porta do contêiner do painel estiver usando `https`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1650">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-1651">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-1651">Network</span></span>

* <span data-ttu-id="69b8c-1652">O argumento `--yes` foi adicionado a `network dns record-set cname delete`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1652">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="69b8c-1653">Perfil</span><span class="sxs-lookup"><span data-stu-id="69b8c-1653">Profile</span></span>

* <span data-ttu-id="69b8c-1654">O argumento `--resource-type` foi adicionado a `account get-access-token` para obter tokens de acesso de recurso</span><span class="sxs-lookup"><span data-stu-id="69b8c-1654">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="69b8c-1655">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="69b8c-1655">ServiceFabric</span></span>

* <span data-ttu-id="69b8c-1656">Todas as versões de sistema operacional com suporte para criação do cluster sf foram adicionadas</span><span class="sxs-lookup"><span data-stu-id="69b8c-1656">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="69b8c-1657">Foi corrigido o bug de validação do certificado primário</span><span class="sxs-lookup"><span data-stu-id="69b8c-1657">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-1658">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-1658">Storage</span></span>

* <span data-ttu-id="69b8c-1659">Adicionado o comando `storage copy`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1659">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="69b8c-1660">30 de julho de 2019</span><span class="sxs-lookup"><span data-stu-id="69b8c-1660">July 30, 2019</span></span>

<span data-ttu-id="69b8c-1661">Versão 2.0.70</span><span class="sxs-lookup"><span data-stu-id="69b8c-1661">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-1662">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-1662">ACR</span></span>

* <span data-ttu-id="69b8c-1663">Corrigido o problema #9952 (uma regressão no comando `acr pack build`)</span><span class="sxs-lookup"><span data-stu-id="69b8c-1663">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="69b8c-1664">Removido o nome da imagem do construtor padrão em `acr pack build`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1664">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-1665">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-1665">Appservice</span></span>

* <span data-ttu-id="69b8c-1666">Alterado `webapp config ssl` para mostrar uma mensagem se um recurso não for encontrado</span><span class="sxs-lookup"><span data-stu-id="69b8c-1666">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="69b8c-1667">Corrigido o problema em que `functionapp create` não aceita o tipo de conta de armazenamento `Standard_RAGRS`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1667">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="69b8c-1668">Corrigido um problema em que `webapp up` falharia se fosse executado usando versões mais antigas do Python</span><span class="sxs-lookup"><span data-stu-id="69b8c-1668">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-1669">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-1669">Network</span></span>

* <span data-ttu-id="69b8c-1670">Removido parâmetro inválido `--ids` de `network nic ip-config add` (corrige o #9861)</span><span class="sxs-lookup"><span data-stu-id="69b8c-1670">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="69b8c-1671">Corrige o #9604.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1671">Fixes #9604.</span></span> <span data-ttu-id="69b8c-1672">Adicionado o parâmetro `--root-certs` ao `network application-gateway http-settings [create|update]` para dar suporte a certificados raiz confiáveis associados ao usuário.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1672">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="69b8c-1673">Fixado argumento `--subscription` para `network dns record-set ns create` (#9965)</span><span class="sxs-lookup"><span data-stu-id="69b8c-1673">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="69b8c-1674">RBAC</span><span class="sxs-lookup"><span data-stu-id="69b8c-1674">RBAC</span></span>

* <span data-ttu-id="69b8c-1675">Adicionado o comando `user update`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1675">Added `user update` command</span></span>
* <span data-ttu-id="69b8c-1676">[PRETERIDO] Preterido `--upn-or-object-id` de comandos relacionados ao usuário</span><span class="sxs-lookup"><span data-stu-id="69b8c-1676">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="69b8c-1677">Usar argumento de substituição `--id`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1677">Use replacement argument `--id`</span></span>
* <span data-ttu-id="69b8c-1678">Adicionado argumento `--id` para comandos relacionados ao usuário</span><span class="sxs-lookup"><span data-stu-id="69b8c-1678">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="69b8c-1679">SQL</span><span class="sxs-lookup"><span data-stu-id="69b8c-1679">SQL</span></span>

* <span data-ttu-id="69b8c-1680">Adicionados comandos de gerenciamento para chaves de instância gerenciada e protetor de TDE</span><span class="sxs-lookup"><span data-stu-id="69b8c-1680">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-1681">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-1681">Storage</span></span>

* <span data-ttu-id="69b8c-1682">Adicionado o comando `storage remove`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1682">Added `storage remove` command</span></span>
* <span data-ttu-id="69b8c-1683">Corrigido um problema com `storage blob update`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1683">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="69b8c-1684">VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-1684">VM</span></span>

* <span data-ttu-id="69b8c-1685">Alterado `list-skus` para usar versão de API mais recente a fim de externar detalhes de zona</span><span class="sxs-lookup"><span data-stu-id="69b8c-1685">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="69b8c-1686">Alterado o padrão de `--single-placement-group` para `false` para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1686">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="69b8c-1687">Adicionada a capacidade de selecionar SKUs de armazenamento ZRS para `[snapshot|disk] create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1687">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="69b8c-1688">Adicionado novo grupo de comandos `vm host` para dar suporte a hosts dedicados</span><span class="sxs-lookup"><span data-stu-id="69b8c-1688">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="69b8c-1689">Adicionados parâmetros `--host` e `--host-group` em `vm create` para definir o host dedicado da VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-1689">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="69b8c-1690">16 de julho de 2019</span><span class="sxs-lookup"><span data-stu-id="69b8c-1690">July 16, 2019</span></span>

<span data-ttu-id="69b8c-1691">Versão 2.0.69</span><span class="sxs-lookup"><span data-stu-id="69b8c-1691">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-1692">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-1692">Appservice</span></span>

* <span data-ttu-id="69b8c-1693">Os comandos `webapp identity` foram alterados para retornar uma mensagem de erro apropriada se o nome do aplicativo ou ResourceGroupName for inválido</span><span class="sxs-lookup"><span data-stu-id="69b8c-1693">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="69b8c-1694">`webapp list` corrigido para retornar o valor correto para numberOfSites se nenhum ResourceGroup foi fornecido</span><span class="sxs-lookup"><span data-stu-id="69b8c-1694">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="69b8c-1695">Corrigidos os efeitos colaterais de `appservice plan create` e `webapp create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1695">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="69b8c-1696">Núcleo</span><span class="sxs-lookup"><span data-stu-id="69b8c-1696">Core</span></span>

* <span data-ttu-id="69b8c-1697">Corrigido um problema em que `--subscription` aparecia apesar de não ser aplicável</span><span class="sxs-lookup"><span data-stu-id="69b8c-1697">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="69b8c-1698">Lote</span><span class="sxs-lookup"><span data-stu-id="69b8c-1698">Batch</span></span>

* <span data-ttu-id="69b8c-1699">[ALTERAÇÃO SIGNIFICATIVA]`batch pool node-agent-skus list` foi substituído por `batch pool supported-images list`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1699">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="69b8c-1700">Adicionado suporte para regras de segurança bloqueando o acesso de rede a um pool com base na porta de origem do tráfego ao usar a opção `--json-file` de `batch pool create network`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1700">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="69b8c-1701">Suporte adicionado para executar a tarefa no diretório de trabalho de contêiner ou no diretório de trabalho de tarefa em lotes ao usar a opção `--json-file` de `batch task create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1701">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="69b8c-1702">Corrigido o erro na opção `--application-package-references` de `batch pool create` em que ela funcionaria apenas com padrões</span><span class="sxs-lookup"><span data-stu-id="69b8c-1702">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="69b8c-1703">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="69b8c-1703">Eventhubs</span></span>

* <span data-ttu-id="69b8c-1704">Adicionada validação para o parâmetro `--rights` dos comandos `authorizationrule`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1704">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="69b8c-1705">RDBMS</span><span class="sxs-lookup"><span data-stu-id="69b8c-1705">RDBMS</span></span>

* <span data-ttu-id="69b8c-1706">Adicionado um parâmetro opcional para especificar a réplica de SKU para criar o comando de réplica</span><span class="sxs-lookup"><span data-stu-id="69b8c-1706">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="69b8c-1707">Corrigido o problema com a falha no teste de CI com a criação de réplica de MySQL</span><span class="sxs-lookup"><span data-stu-id="69b8c-1707">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="69b8c-1708">Retransmissão</span><span class="sxs-lookup"><span data-stu-id="69b8c-1708">Relay</span></span>

* <span data-ttu-id="69b8c-1709">Corrigido o problema com a conexão híbrida quando a autorização do cliente desabilitava [#8775](https://github.com/azure/azure-cli/issues/8775)</span><span class="sxs-lookup"><span data-stu-id="69b8c-1709">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="69b8c-1710">Parâmetro `--requires-transport-security` adicionado a `relay wcfrelay create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1710">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="69b8c-1711">Barramento de serviço</span><span class="sxs-lookup"><span data-stu-id="69b8c-1711">Servicebus</span></span>

* <span data-ttu-id="69b8c-1712">Adicionada validação para o parâmetro `--rights` dos comandos `authorizationrule`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1712">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-1713">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-1713">Storage</span></span>

* <span data-ttu-id="69b8c-1714">Habilitar AADDS de arquivos para atualização da conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-1714">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="69b8c-1715">Problema corrigido `storage blob service-properties update --set`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1715">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="69b8c-1716">2 de julho de 2019</span><span class="sxs-lookup"><span data-stu-id="69b8c-1716">July 2, 2019</span></span>

<span data-ttu-id="69b8c-1717">Versão 2.0.68</span><span class="sxs-lookup"><span data-stu-id="69b8c-1717">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="69b8c-1718">Núcleo</span><span class="sxs-lookup"><span data-stu-id="69b8c-1718">Core</span></span>

* <span data-ttu-id="69b8c-1719">Agora, os módulos de comando são consolidados em um único Python distribuível.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1719">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="69b8c-1720">Isso substitui o uso direto de muitos pacotes `azure-cli-` no PyPI.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1720">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="69b8c-1721">Assim, o tamanho da instalação será reduzido e apenas os usuários que tiverem instalado diretamente por meio do `pip` serão afetados.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1721">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-1722">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-1722">ACR</span></span>

* <span data-ttu-id="69b8c-1723">Foi adicionado o suporte para gatilhos de temporizador para tarefa</span><span class="sxs-lookup"><span data-stu-id="69b8c-1723">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-1724">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-1724">Appservice</span></span>

* <span data-ttu-id="69b8c-1725">O `functionapp create` foi alterado para habilitar o Application Insights por padrão</span><span class="sxs-lookup"><span data-stu-id="69b8c-1725">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="69b8c-1726">[ALTERAÇÃO SIGNIFICATIVA] Foi removido o comando `functionapp devops-build` preterido.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1726">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="69b8c-1727">Agora, use o novo comando `az functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1727">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="69b8c-1728">Foi adicionado o suporte ao plano de aplicativo de funções Consumo em Linux ao `functionapp deployment config-zip`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1728">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="69b8c-1729">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="69b8c-1729">Cosmos DB</span></span>

* <span data-ttu-id="69b8c-1730">Foi adicionado o suporte para desabilitar a TTL</span><span class="sxs-lookup"><span data-stu-id="69b8c-1730">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="69b8c-1731">DLS</span><span class="sxs-lookup"><span data-stu-id="69b8c-1731">DLS</span></span>

* <span data-ttu-id="69b8c-1732">Versão atualizada do ADLS (0.0.45)</span><span class="sxs-lookup"><span data-stu-id="69b8c-1732">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="69b8c-1733">Comentários</span><span class="sxs-lookup"><span data-stu-id="69b8c-1733">Feedback</span></span>

* <span data-ttu-id="69b8c-1734">Ao relatar um comando de extensão com falha, agora, o `az feedback` tenta abrir o navegador na URL do projeto/repositório da extensão por meio do índice</span><span class="sxs-lookup"><span data-stu-id="69b8c-1734">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="69b8c-1735">HDInsight</span><span class="sxs-lookup"><span data-stu-id="69b8c-1735">HDInsight</span></span>

* <span data-ttu-id="69b8c-1736">[ALTERAÇÃO SIGNIFICATIVA] O nome do grupo de comandos `oms` foi alterado para `monitor`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1736">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="69b8c-1737">[ALTERAÇÃO SIGNIFICATIVA]`--http-password/-p` tornou-se um parâmetro obrigatório</span><span class="sxs-lookup"><span data-stu-id="69b8c-1737">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="69b8c-1738">Foram adicionados preenchedores para o preenchedor dos parâmetros `--cluster-admin-account` e `cluster-users-group-dns`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1738">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="69b8c-1739">O parâmetro `cluster-users-group-dns` foi alterado para ser obrigatório quando `—esp` estiver presente</span><span class="sxs-lookup"><span data-stu-id="69b8c-1739">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="69b8c-1740">Foi adicionado um tempo limite para todos os preenchedores automáticos de argumento existentes</span><span class="sxs-lookup"><span data-stu-id="69b8c-1740">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="69b8c-1741">Foi adicionado um tempo limite para transformar o nome do recurso na ID de recurso</span><span class="sxs-lookup"><span data-stu-id="69b8c-1741">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="69b8c-1742">Os preenchedores automáticos foram alterados para selecionar recursos de qualquer grupo de recursos.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1742">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="69b8c-1743">Pode ser um grupo de recursos diferente daquele especificado com `-g`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1743">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="69b8c-1744">Foi adicionado o suporte para os parâmetros `--sub-domain-suffix` e `--disable_gateway_auth` no comando `hdinsight application create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1744">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="69b8c-1745">Serviços gerenciados</span><span class="sxs-lookup"><span data-stu-id="69b8c-1745">Managed Services</span></span>

* <span data-ttu-id="69b8c-1746">Introdução ao módulo de comando de serviço gerenciado em versão prévia</span><span class="sxs-lookup"><span data-stu-id="69b8c-1746">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="69b8c-1747">Perfil</span><span class="sxs-lookup"><span data-stu-id="69b8c-1747">Profile</span></span>
* <span data-ttu-id="69b8c-1748">Suprimir o argumento `--subscription` para o comando de logoff</span><span class="sxs-lookup"><span data-stu-id="69b8c-1748">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="69b8c-1749">RBAC</span><span class="sxs-lookup"><span data-stu-id="69b8c-1749">RBAC</span></span>

* <span data-ttu-id="69b8c-1750">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--password` foi removido de `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1750">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="69b8c-1751">Foi adicionado o parâmetro `--assignee-principal-type` ao comando `create` para evitar falhas intermitentes causadas pela latência de replicação do servidor do AAD Graph</span><span class="sxs-lookup"><span data-stu-id="69b8c-1751">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="69b8c-1752">Foi corrigida uma falha em `ad signed-in-user` ao listar objetos de propriedade</span><span class="sxs-lookup"><span data-stu-id="69b8c-1752">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="69b8c-1753">Foi corrigido um problema em que o `ad sp` não localizava o aplicativo certo de uma entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="69b8c-1753">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="69b8c-1754">RDBMS</span><span class="sxs-lookup"><span data-stu-id="69b8c-1754">RDBMS</span></span>

* <span data-ttu-id="69b8c-1755">Foi adicionado o suporte à replicação para o MariaDB</span><span class="sxs-lookup"><span data-stu-id="69b8c-1755">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="69b8c-1756">SQL</span><span class="sxs-lookup"><span data-stu-id="69b8c-1756">SQL</span></span>

* <span data-ttu-id="69b8c-1757">Valores permitidos documentados para `sql db create --sample-name`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1757">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-1758">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-1758">Storage</span></span>

* <span data-ttu-id="69b8c-1759">Foi adicionado o suporte ao token SAS de delegação de usuário com `--as-user` para `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1759">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="69b8c-1760">Foi adicionado o suporte ao token SAS de delegação de usuário com `--as-user` para `storage container generate-sas`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1760">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="69b8c-1761">VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-1761">VM</span></span>

* <span data-ttu-id="69b8c-1762">Foi corrigido o bug em que o `vmss create` retornava uma mensagem de erro quando era executado com `--no-wait`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1762">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="69b8c-1763">Foi removida a validação do lado do cliente de `vmss create --single-placement-group`.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1763">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="69b8c-1764">Não falha quando `--single-placement-group` é definido como `true` e `--instance-count` é maior que 100 ou quando são especificadas zonas de disponibilidade, mas deixa essa validação para o serviço de computação</span><span class="sxs-lookup"><span data-stu-id="69b8c-1764">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="69b8c-1765">Foi corrigido o bug em que o `[vm|vmss] extension image list` falhava quando era usado com `--latest`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1765">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="69b8c-1766">18 de junho de 2019</span><span class="sxs-lookup"><span data-stu-id="69b8c-1766">June 18, 2019</span></span>

<span data-ttu-id="69b8c-1767">Versão 2.0.67</span><span class="sxs-lookup"><span data-stu-id="69b8c-1767">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="69b8c-1768">Núcleo</span><span class="sxs-lookup"><span data-stu-id="69b8c-1768">Core</span></span>

<span data-ttu-id="69b8c-1769">Esta versão apresenta uma nova marca [Versão prévia] para comunicar com mais clareza aos clientes quando um comando, um grupo de comandos ou um argumento está no status de versão prévia.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1769">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="69b8c-1770">Anteriormente, essa informação era transmitida no texto de ajuda ou, implicitamente, pelo número da versão do módulo de comando.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1770">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="69b8c-1771">A CLI removerá os números de versão dos pacotes individuais no futuro.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1771">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="69b8c-1772">Se um comando estiver em versão prévia, todos os seus argumentos também estarão.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1772">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="69b8c-1773">Se um grupo de comandos for rotulado com o status de versão prévia, então todos os seus comandos e argumentos também serão considerados em versão prévia.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1773">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="69b8c-1774">Como resultado dessa alteração, diversos grupos de comandos podem parecer surgir "de repente" com o status de versão prévia com esta liberação.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1774">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="69b8c-1775">O que realmente aconteceu é que a maioria dos pacotes já estava com status de versão prévia, mas estão sendo consideradas GA com esta liberação</span><span class="sxs-lookup"><span data-stu-id="69b8c-1775">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-1776">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-1776">ACR</span></span>
* <span data-ttu-id="69b8c-1777">Adicionado o comando 'acr check-health'</span><span class="sxs-lookup"><span data-stu-id="69b8c-1777">Added 'acr check-health' command</span></span>
* <span data-ttu-id="69b8c-1778">Melhorado o tratamento de erro para tokens do AAD e para recuperar comandos externos</span><span class="sxs-lookup"><span data-stu-id="69b8c-1778">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="69b8c-1779">ACS</span><span class="sxs-lookup"><span data-stu-id="69b8c-1779">ACS</span></span>
* <span data-ttu-id="69b8c-1780">Comandos preteridos do ACS agora ficam ocultos da exibição da ajuda</span><span class="sxs-lookup"><span data-stu-id="69b8c-1780">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="69b8c-1781">AMS</span><span class="sxs-lookup"><span data-stu-id="69b8c-1781">AMS</span></span>
* <span data-ttu-id="69b8c-1782">[ALTERAÇÃO SIGNIFICATIVA] Alterada para retornar cadeias de caracteres de tempo da ISO 8601 para archive-window-length e key-frame-interval-duration</span><span class="sxs-lookup"><span data-stu-id="69b8c-1782">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-1783">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-1783">AppService</span></span>
* <span data-ttu-id="69b8c-1784">Adicionado roteamento com base no local para `webapp deleted list` e `webapp deleted restore`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1784">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="69b8c-1785">Corrigido problema em que a URL de destino registrada do webapp ("Não é possível iniciar o aplicativo em...") não era clicável no Azure Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="69b8c-1785">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="69b8c-1786">Corrigido um problema em que a criação de aplicativos com algumas SKUs falhava com um erro de AlwaysOn</span><span class="sxs-lookup"><span data-stu-id="69b8c-1786">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="69b8c-1787">Adicionada a pré-validação para o `[appservice|webapp] create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1787">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="69b8c-1788">Corrigido o `[webapp|functionapp] traffic-routing` para usar o actionHostName correto</span><span class="sxs-lookup"><span data-stu-id="69b8c-1788">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="69b8c-1789">Adicionado o suporte de slot para comandos `functionapp`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1789">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="69b8c-1790">Lote</span><span class="sxs-lookup"><span data-stu-id="69b8c-1790">Batch</span></span>
* <span data-ttu-id="69b8c-1791">Corrigida a regressão de autenticação do AAD causada pela geração de relatórios de erros superagressiva para autenticação de chave compartilhada</span><span class="sxs-lookup"><span data-stu-id="69b8c-1791">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="69b8c-1792">BatchAI</span><span class="sxs-lookup"><span data-stu-id="69b8c-1792">BatchAI</span></span>
* <span data-ttu-id="69b8c-1793">Agora os comandos do BatchAI estão preteridos e ocultos</span><span class="sxs-lookup"><span data-stu-id="69b8c-1793">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="69b8c-1794">BotService</span><span class="sxs-lookup"><span data-stu-id="69b8c-1794">BotService</span></span>
* <span data-ttu-id="69b8c-1795">Adição das mensagens de aviso "suporte descontinuado"/"modo de manutenção" para os comandos compatíveis com a v3 do SDK</span><span class="sxs-lookup"><span data-stu-id="69b8c-1795">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="69b8c-1796">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="69b8c-1796">CosmosDB</span></span>
* <span data-ttu-id="69b8c-1797">[PRETERIDO] Preterido o comando `cosmosdb list-keys`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1797">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="69b8c-1798">Adicionado o comando `cosmosdb keys list` – substitui o `cosmosdb list-keys`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1798">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="69b8c-1799">`cosmsodb create/update`: Adicionado novo formato para --location a fim de permitir a configuração da propriedade "isZoneRedundant".</span><span class="sxs-lookup"><span data-stu-id="69b8c-1799">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="69b8c-1800">Formato antigo preterido</span><span class="sxs-lookup"><span data-stu-id="69b8c-1800">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="69b8c-1801">EventGrid</span><span class="sxs-lookup"><span data-stu-id="69b8c-1801">EventGrid</span></span>
* <span data-ttu-id="69b8c-1802">Adicionados comandos do `eventgrid domain` para operações de CRUD no domínio</span><span class="sxs-lookup"><span data-stu-id="69b8c-1802">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="69b8c-1803">Adicionados comandos do `eventgrid domain topic` para operações de CRUD nos tópicos do domínio</span><span class="sxs-lookup"><span data-stu-id="69b8c-1803">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="69b8c-1804">Adicionado argumento do `--odata-query` ao `eventgrid [topic|event-subscription] list` para filtrar os resultados usando a sintaxe do OData</span><span class="sxs-lookup"><span data-stu-id="69b8c-1804">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="69b8c-1805">`event-subscription create/update`: Adicionado o servicebusqueue como novos valores para o parâmetro `--endpoint-type`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1805">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="69b8c-1806">[ALTERAÇÃO SIGNIFICATIVA] Removido o suporte para `--included-event-types All` com `eventgrid event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1806">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="69b8c-1807">HDInsight</span><span class="sxs-lookup"><span data-stu-id="69b8c-1807">HDInsight</span></span>
* <span data-ttu-id="69b8c-1808">Adicionado suporte para o parâmetro `--ssh-public-key` no comando `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1808">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="69b8c-1809">IoT</span><span class="sxs-lookup"><span data-stu-id="69b8c-1809">IoT</span></span>
* <span data-ttu-id="69b8c-1810">Adicionado suporte para regenerar as chaves da política de autorização</span><span class="sxs-lookup"><span data-stu-id="69b8c-1810">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="69b8c-1811">Adicionados SDK e suporte para o serviço de provisionamento de repositórios do DigitalTwin</span><span class="sxs-lookup"><span data-stu-id="69b8c-1811">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-1812">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-1812">Network</span></span>
* <span data-ttu-id="69b8c-1813">Adicionado suporte de zona para o Gateway da NAT</span><span class="sxs-lookup"><span data-stu-id="69b8c-1813">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="69b8c-1814">Adicionado o comando `network list-service-tags`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1814">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="69b8c-1815">Corrigido o problema com o `dns zone import` em que os usuários não conseguiam importar registros do curinga A</span><span class="sxs-lookup"><span data-stu-id="69b8c-1815">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="69b8c-1816">Corrigido o problema com o `watcher flow-log configure` em que o registro de fluxo não podia ser habilitado em determinadas regiões</span><span class="sxs-lookup"><span data-stu-id="69b8c-1816">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="69b8c-1817">Recurso</span><span class="sxs-lookup"><span data-stu-id="69b8c-1817">Resource</span></span>
* <span data-ttu-id="69b8c-1818">Adicionado o comando do `az rest` para fazer chamadas REST</span><span class="sxs-lookup"><span data-stu-id="69b8c-1818">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="69b8c-1819">Corrigido o erro ao usar o `policy assignment list` com um grupo de recursos ou o nível de assinatura `--scope`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1819">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="69b8c-1820">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="69b8c-1820">ServiceBus</span></span>
* <span data-ttu-id="69b8c-1821">Corrigido o problema com o `servicebus topic create --max-size`[nº9319](https://github.com/azure/azure-cli/issues/9319)</span><span class="sxs-lookup"><span data-stu-id="69b8c-1821">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="69b8c-1822">SQL</span><span class="sxs-lookup"><span data-stu-id="69b8c-1822">SQL</span></span>
* <span data-ttu-id="69b8c-1823">Alterado o `--location` para ser opcional para `sql [server|mi] create` – usa o local do grupo de recursos se não especificado</span><span class="sxs-lookup"><span data-stu-id="69b8c-1823">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="69b8c-1824">Corrigido o erro "objeto 'NoneType' não é iterável" para `sql db list-editions --available`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1824">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="69b8c-1825">SQLVm</span><span class="sxs-lookup"><span data-stu-id="69b8c-1825">SQLVm</span></span>
* <span data-ttu-id="69b8c-1826">[ALTERAÇÃO DA FALHA] Alterado `sql vm create` para exigir o parâmetro `--license-type`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1826">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="69b8c-1827">Alterado para permitir a configuração da SKU da imagem do SQL ao criar ou atualizar uma VM do SQL</span><span class="sxs-lookup"><span data-stu-id="69b8c-1827">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-1828">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-1828">Storage</span></span>
* <span data-ttu-id="69b8c-1829">Corrigido o problema com a chave de conta ignorada para `storage container generate-sas`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1829">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="69b8c-1830">Corrigido o problema com o `storage blob sync` no Linux</span><span class="sxs-lookup"><span data-stu-id="69b8c-1830">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="69b8c-1831">VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-1831">VM</span></span>
* <span data-ttu-id="69b8c-1832">[VERSÃO PRÉVIA] Adicionados os comandos `vm image template` para criar imagens de VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-1832">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="69b8c-1833">4 de junho de 2019</span><span class="sxs-lookup"><span data-stu-id="69b8c-1833">June 4, 2019</span></span>

<span data-ttu-id="69b8c-1834">Versão 2.0.66</span><span class="sxs-lookup"><span data-stu-id="69b8c-1834">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="69b8c-1835">Núcleo</span><span class="sxs-lookup"><span data-stu-id="69b8c-1835">Core</span></span>
* <span data-ttu-id="69b8c-1836">Foi corrigido o bug em que os comandos falhavam quando `--output yaml` era usado com `--query`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1836">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-1837">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-1837">ACR</span></span>
* <span data-ttu-id="69b8c-1838">Foi adicionado o grupo de comando 'pack acr' para a criação de Tarefas de build rápida usando Buildpacks.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1838">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="69b8c-1839">ACS</span><span class="sxs-lookup"><span data-stu-id="69b8c-1839">ACS</span></span>
* <span data-ttu-id="69b8c-1840">Permitir a opção de habilitar/desabilitar o complemento kube-dashboard do AKS</span><span class="sxs-lookup"><span data-stu-id="69b8c-1840">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="69b8c-1841">Imprimir uma mensagem amigável quando a assinatura não estiver na lista de permissões para usar o Red Hat OpenShift no Azure</span><span class="sxs-lookup"><span data-stu-id="69b8c-1841">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="69b8c-1842">Lote</span><span class="sxs-lookup"><span data-stu-id="69b8c-1842">Batch</span></span>
* <span data-ttu-id="69b8c-1843">Melhoria no tratamento de erro quando você não está conectado a uma conta \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span><span class="sxs-lookup"><span data-stu-id="69b8c-1843">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="69b8c-1844">IoT</span><span class="sxs-lookup"><span data-stu-id="69b8c-1844">IoT</span></span>
* <span data-ttu-id="69b8c-1845">Foi adicionado o suporte para failover manual</span><span class="sxs-lookup"><span data-stu-id="69b8c-1845">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-1846">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-1846">Network</span></span>
* <span data-ttu-id="69b8c-1847">Foram adicionados os comandos `network application-gateway waf-policy` para oferecer suporte às regras de WAF personalizadas.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1847">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="69b8c-1848">Adicionados os argumentos `--waf-policy` e `--max-capacity` para `network application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1848">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="69b8c-1849">Recurso</span><span class="sxs-lookup"><span data-stu-id="69b8c-1849">Resource</span></span>
* <span data-ttu-id="69b8c-1850">Melhoria da mensagem de erro do `deployment create` quando não há nenhum TTY disponível</span><span class="sxs-lookup"><span data-stu-id="69b8c-1850">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="69b8c-1851">Função</span><span class="sxs-lookup"><span data-stu-id="69b8c-1851">Role</span></span>
* <span data-ttu-id="69b8c-1852">O texto da Ajuda foi atualizado.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1852">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="69b8c-1853">Computação</span><span class="sxs-lookup"><span data-stu-id="69b8c-1853">Compute</span></span>
* <span data-ttu-id="69b8c-1854">Foi adicionado o suporte para `vm create` para as VMs de uma imagem gerenciada com LUNs de disco de dados que não começam em 0 ou que ignoram números</span><span class="sxs-lookup"><span data-stu-id="69b8c-1854">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="69b8c-1855">21 de maio de 2019</span><span class="sxs-lookup"><span data-stu-id="69b8c-1855">May 21, 2019</span></span>

<span data-ttu-id="69b8c-1856">Versão 2.0.65</span><span class="sxs-lookup"><span data-stu-id="69b8c-1856">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="69b8c-1857">Núcleo</span><span class="sxs-lookup"><span data-stu-id="69b8c-1857">Core</span></span>
* <span data-ttu-id="69b8c-1858">Foram adicionados comentários melhores para erros de autenticação</span><span class="sxs-lookup"><span data-stu-id="69b8c-1858">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="69b8c-1859">Corrigido um problema em que a CLI carregava extensões que não eram compatíveis com a versão do núcleo</span><span class="sxs-lookup"><span data-stu-id="69b8c-1859">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="69b8c-1860">Corrigido um problema com a inicialização quando `clouds.config` está corrompido</span><span class="sxs-lookup"><span data-stu-id="69b8c-1860">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-1861">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-1861">ACR</span></span>
* <span data-ttu-id="69b8c-1862">Foi adicionado suporte das Identidades Gerenciadas para Tarefas</span><span class="sxs-lookup"><span data-stu-id="69b8c-1862">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="69b8c-1863">ACS</span><span class="sxs-lookup"><span data-stu-id="69b8c-1863">ACS</span></span>
* <span data-ttu-id="69b8c-1864">Corrigido o comando `openshift create` quando usado com o cliente AAD do consumidor</span><span class="sxs-lookup"><span data-stu-id="69b8c-1864">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-1865">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-1865">AppService</span></span>
* <span data-ttu-id="69b8c-1866">[PRETERIDO] Preterido o comando `functionapp devops-build` – Será removido na próxima versão</span><span class="sxs-lookup"><span data-stu-id="69b8c-1866">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="69b8c-1867">`functionapp devops-pipeline` foi alterado para buscar o log de build do Azure DevOps no modo detalhado</span><span class="sxs-lookup"><span data-stu-id="69b8c-1867">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="69b8c-1868">[ALTERAÇÃO SIGNIFICATIVA] O sinalizador `--use_local_settings` foi removido do comando `functionapp devops-pipeline` – não estava operacional</span><span class="sxs-lookup"><span data-stu-id="69b8c-1868">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="69b8c-1869">`webapp up` foi alterado para retornar uma saída JSON se `--logs` não for usado</span><span class="sxs-lookup"><span data-stu-id="69b8c-1869">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="69b8c-1870">Foi adicionado suporte para escrever recursos padrão para a configuração local de `webapp up`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1870">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="69b8c-1871">Foi adicionado suporte para `webapp up` reimplantar um aplicativo sem usar o argumento `--location`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1871">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="69b8c-1872">Corrigido um problema em que o valor do SKU gratuito não funcionava na criação do ASP do SKU gratuito do Linux</span><span class="sxs-lookup"><span data-stu-id="69b8c-1872">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="69b8c-1873">BotService</span><span class="sxs-lookup"><span data-stu-id="69b8c-1873">BotService</span></span>
* <span data-ttu-id="69b8c-1874">Alterado para permitir todas as capitalizações para parâmetros `--lang` em todos os comandos</span><span class="sxs-lookup"><span data-stu-id="69b8c-1874">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="69b8c-1875">Descrição atualizada do módulo de comando</span><span class="sxs-lookup"><span data-stu-id="69b8c-1875">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="69b8c-1876">Consumo</span><span class="sxs-lookup"><span data-stu-id="69b8c-1876">Consumption</span></span>
* <span data-ttu-id="69b8c-1877">O parâmetro obrigatório ausente foi adicionado para executar `consumption usage list --billing-period-name`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1877">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="69b8c-1878">IoT</span><span class="sxs-lookup"><span data-stu-id="69b8c-1878">IoT</span></span>
* <span data-ttu-id="69b8c-1879">Suporte adicionado para listar todas as chaves</span><span class="sxs-lookup"><span data-stu-id="69b8c-1879">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-1880">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-1880">Network</span></span>
* [ALTERAÇÃO SIGNIFICATIVA]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="69b8c-1882">O argumento `--nat-gateway` foi adicionado a `network vnet subnet [create|update]` para anexar a um gateway NAT</span><span class="sxs-lookup"><span data-stu-id="69b8c-1882">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="69b8c-1883">Corrigido o problema de `dns zone import`, em que os nomes de registro não correspondiam ao tipo de registro</span><span class="sxs-lookup"><span data-stu-id="69b8c-1883">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="69b8c-1884">RDBMS</span><span class="sxs-lookup"><span data-stu-id="69b8c-1884">RDBMS</span></span>
* <span data-ttu-id="69b8c-1885">Suporte a postgres e mysql adicionado para replicação geográfica</span><span class="sxs-lookup"><span data-stu-id="69b8c-1885">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="69b8c-1886">RBAC</span><span class="sxs-lookup"><span data-stu-id="69b8c-1886">RBAC</span></span>
* <span data-ttu-id="69b8c-1887">Adição de suporte do escopo de grupo de gerenciamento a `role assignment`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1887">Added support for management group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-1888">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-1888">Storage</span></span>
* <span data-ttu-id="69b8c-1889">`storage blob sync`: adicionar um comando de sincronização ao armazenamento de blobs</span><span class="sxs-lookup"><span data-stu-id="69b8c-1889">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="69b8c-1890">Computação</span><span class="sxs-lookup"><span data-stu-id="69b8c-1890">Compute</span></span>
* <span data-ttu-id="69b8c-1891">`--computer-name` foi adicionado a `vm create` para configurar o nome do computador da VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-1891">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="69b8c-1892">`--ssh-key-value` foi renomeado para `--ssh-key-values` para `[vm|vmss] create` – Agora, pode aceitar vários valores de chave pública ou caminhos ssh</span><span class="sxs-lookup"><span data-stu-id="69b8c-1892">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="69b8c-1893">__Observação__ : Isso **não** é uma alteração da falha – `--ssh-key-value` será analisado corretamente, pois corresponde somente a `--ssh-key-values`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1893">__Note__ : This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="69b8c-1894">O argumento `--type` de `ppg create` foi alterado para ser opcional</span><span class="sxs-lookup"><span data-stu-id="69b8c-1894">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="69b8c-1895">6 de maio de 2019</span><span class="sxs-lookup"><span data-stu-id="69b8c-1895">May 6, 2019</span></span>

<span data-ttu-id="69b8c-1896">Versão 2.0.64</span><span class="sxs-lookup"><span data-stu-id="69b8c-1896">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="69b8c-1897">ACS</span><span class="sxs-lookup"><span data-stu-id="69b8c-1897">ACS</span></span>
* <span data-ttu-id="69b8c-1898">[ALTERAÇÃO SIGNIFICATIVA] O sinalizador `--fqdn` foi removido dos comandos `openshift`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1898">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="69b8c-1899">Alterado para usar a versão da API do Red Hat OpenShift no Azure em disponibilidade geral</span><span class="sxs-lookup"><span data-stu-id="69b8c-1899">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="69b8c-1900">O sinalizador `customer-admin-group-id` foi adicionado a `openshift create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1900">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="69b8c-1901">[GA] `(PREVIEW)` foi removido da opção `aks create``--network-policy`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1901">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-1902">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-1902">Appservice</span></span>
* <span data-ttu-id="69b8c-1903">[PRETERIDO] O comando `functionapp devops-build` foi preterido</span><span class="sxs-lookup"><span data-stu-id="69b8c-1903">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="69b8c-1904">Renomeado para `functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1904">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="69b8c-1905">Corrigido ao obter o nome de usuário correto para cloudshell que estava causando a falha em `webapp up`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1905">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="69b8c-1906">Documentação `appservice plan --sku` atualizada para refletir o appserviceplans com suporte</span><span class="sxs-lookup"><span data-stu-id="69b8c-1906">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="69b8c-1907">Adicionado argumentos opcionais para o grupo de recursos e plano a `webapp up`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1907">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="69b8c-1908">Adicionado suporte a `webapp ssh` para respeitar a variável de ambiente `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1908">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="69b8c-1909">Adicionado suporte `appserviceplan create` para a SKU gratuita do Linux</span><span class="sxs-lookup"><span data-stu-id="69b8c-1909">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="69b8c-1910">Alterado `webapp up` para ter uma suspensão de 30 segundos depois de definir appsetting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` para lidar com a inicialização a frio kudu</span><span class="sxs-lookup"><span data-stu-id="69b8c-1910">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="69b8c-1911">Adicionado suporte para runtime `powershell` a `functionapp create` no Windows</span><span class="sxs-lookup"><span data-stu-id="69b8c-1911">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="69b8c-1912">Adicionado o comando `create-remote-connection`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1912">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="69b8c-1913">Lote</span><span class="sxs-lookup"><span data-stu-id="69b8c-1913">Batch</span></span>
* <span data-ttu-id="69b8c-1914">Corrigido o bug no validador para as opções `--application-package-references`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1914">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="69b8c-1915">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="69b8c-1915">Botservice</span></span>
* <span data-ttu-id="69b8c-1916">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v4 -k webapp` foi alterado para criar um Bot de Aplicativo Web vazio por padrão (ou seja, nenhum bot será implantado no Serviço de Aplicativo)</span><span class="sxs-lookup"><span data-stu-id="69b8c-1916">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="69b8c-1917">O sinalizador `--echo` foi adicionado ao `bot create` para usar o comportamento antigo com `-v v4`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1917">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="69b8c-1918">[ALTERAÇÃO SIGNIFICATIVA] O valor padrão de `--version` foi alterado para `v4`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1918">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="69b8c-1919">__OBSERVAÇÃO:__ `bot prepare-publish` ainda usa o padrão antigo</span><span class="sxs-lookup"><span data-stu-id="69b8c-1919">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="69b8c-1920">[ALTERAÇÃO SIGNIFICATIVA]`--lang` foi alterado para não definir mais `Csharp` como padrão.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1920">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="69b8c-1921">Se o comando exigir `--lang` e ele não for fornecido, o comando será um erro</span><span class="sxs-lookup"><span data-stu-id="69b8c-1921">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="69b8c-1922">[ALTERAÇÃO SIGNIFICATIVA] Os argumentos `--appid` e `--password` foram alterados para `bot create` ser obrigatório e agora podem ser criados por meio de `ad app create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1922">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="69b8c-1923">Foi adicionada validação a `--appid` e `--password`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1923">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="69b8c-1924">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v4` foi alterado para não criar ou usar uma Conta de Armazenamento ou o Application Insights</span><span class="sxs-lookup"><span data-stu-id="69b8c-1924">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="69b8c-1925">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v3` foi alterado para exigir uma região em que o Application Insights está disponível</span><span class="sxs-lookup"><span data-stu-id="69b8c-1925">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="69b8c-1926">[ALTERAÇÃO SIGNIFICATIVA] O `bot update` foi alterado para afetar somente as propriedades específicas de um bot</span><span class="sxs-lookup"><span data-stu-id="69b8c-1926">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="69b8c-1927">[ALTERAÇÃO SIGNIFICATIVA] Os sinalizadores `--lang` foram alterados para aceitar `Javascript` em vez de `Node`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1927">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="69b8c-1928">[ALTERAÇÃO SIGNIFICATIVA] O `Node` foi removido como um valor `--lang` permitido</span><span class="sxs-lookup"><span data-stu-id="69b8c-1928">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="69b8c-1929">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v4 -k webapp` foi alterado para não definir mais `SCM_DO_BUILD_DURING_DEPLOYMENT` como verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="69b8c-1929">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="69b8c-1930">Todas as implantações por meio do Kudu atuarão de acordo com o comportamento padrão</span><span class="sxs-lookup"><span data-stu-id="69b8c-1930">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="69b8c-1931">O `bot download` foi alterado para os bots sem arquivos `.bot` para criar o arquivo de configuração específico a um idioma com os valores das Configurações de Aplicativo do bot</span><span class="sxs-lookup"><span data-stu-id="69b8c-1931">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="69b8c-1932">Adicionado o suporte `Typescript` para `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1932">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="69b8c-1933">Uma mensagem de aviso foi adicionada a `bot prepare-deploy` para os bots `Javascript` e `Typescript` para quando `--code-dir` não contiver `package.json`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1933">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="69b8c-1934">O `bot prepare-deploy` foi alterado para retornar `true`, se bem-sucedido</span><span class="sxs-lookup"><span data-stu-id="69b8c-1934">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="69b8c-1935">O log detalhado foi adicionado a `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1935">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="69b8c-1936">Mais regiões disponíveis do Application Insights foram adicionadas ao `az bot create -v v3`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1936">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="69b8c-1937">Configurar</span><span class="sxs-lookup"><span data-stu-id="69b8c-1937">Configure</span></span>
* <span data-ttu-id="69b8c-1938">Adicionado suporte para configurações de valor padrão do argumento baseado em pasta</span><span class="sxs-lookup"><span data-stu-id="69b8c-1938">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="69b8c-1939">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="69b8c-1939">Eventhubs</span></span>
* <span data-ttu-id="69b8c-1940">Adicionados os comandos `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1940">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="69b8c-1941">O argumento `--default-action` foi adicionado às regras de rede de `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1941">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-1942">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-1942">Network</span></span>
* <span data-ttu-id="69b8c-1943">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--cache` foi substituído por `--defer` para `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1943">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="69b8c-1944">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="69b8c-1944">Policy Insights</span></span>
* <span data-ttu-id="69b8c-1945">Suporte adicionado a `--expand PolicyEvaluationDetails` para detalhes de avaliação de política de consulta no recurso</span><span class="sxs-lookup"><span data-stu-id="69b8c-1945">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="69b8c-1946">Função</span><span class="sxs-lookup"><span data-stu-id="69b8c-1946">Role</span></span>
* <span data-ttu-id="69b8c-1947">[PRETERIDO] Alterado argumento ocultar '--password' `create-for-rbac` - suporte será removido em maio de 2019</span><span class="sxs-lookup"><span data-stu-id="69b8c-1947">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="69b8c-1948">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="69b8c-1948">Service Bus</span></span>
* <span data-ttu-id="69b8c-1949">Adicionados os comandos `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1949">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="69b8c-1950">O argumento `--default-action` foi adicionado às regras de rede de `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1950">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="69b8c-1951">`topic [create|update]` foi fixado para permitir suporte a `--max-size` para valores de 10, 20, 40 e 80 GB com a SKU Premium</span><span class="sxs-lookup"><span data-stu-id="69b8c-1951">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="69b8c-1952">SQL</span><span class="sxs-lookup"><span data-stu-id="69b8c-1952">SQL</span></span>
* <span data-ttu-id="69b8c-1953">Adicionados os comandos `sql virtual-cluster [list|show|delete]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1953">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="69b8c-1954">VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-1954">VM</span></span>
* <span data-ttu-id="69b8c-1955">O `--protect-from-scale-in` e o `--protect-from-scale-set-actions` foram adicionados a `vmss update` para habilitar atualizações à política de proteção das instâncias de VM VMSS</span><span class="sxs-lookup"><span data-stu-id="69b8c-1955">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="69b8c-1956">Adicionado a `--instance-id` e `vmss update` para habilitar atualização genérica das instâncias de VM VMSS</span><span class="sxs-lookup"><span data-stu-id="69b8c-1956">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="69b8c-1957">`--instance-id` foi adicionado a `vmss wait`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1957">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="69b8c-1958">Adição do novo grupo de comandos `ppg` para gerenciar Grupos de Posicionamento de Proximidade</span><span class="sxs-lookup"><span data-stu-id="69b8c-1958">Added new `ppg` command group for managing Proximity Placement Groups</span></span>
* <span data-ttu-id="69b8c-1959">Adicionado a `--ppg`, `[vm|vmss] create` e `vm availability-set create` para gerenciar PPGs</span><span class="sxs-lookup"><span data-stu-id="69b8c-1959">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="69b8c-1960">Parâmetro `--hyper-v-generation` adicionado a `image create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1960">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="69b8c-1961">23 de abril de 2019</span><span class="sxs-lookup"><span data-stu-id="69b8c-1961">April 23, 2019</span></span>

<span data-ttu-id="69b8c-1962">Versão 2.0.63</span><span class="sxs-lookup"><span data-stu-id="69b8c-1962">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="69b8c-1963">ACS</span><span class="sxs-lookup"><span data-stu-id="69b8c-1963">ACS</span></span>
* <span data-ttu-id="69b8c-1964">Alterado `aks get-credentials` para solicitar substituição dos valores duplicados</span><span class="sxs-lookup"><span data-stu-id="69b8c-1964">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="69b8c-1965">Removido `(PREVIEW)` dos comandos de espaços de desenvolvimento "aks use-dev-espaces" e "aks remove-dev-espaces"</span><span class="sxs-lookup"><span data-stu-id="69b8c-1965">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="69b8c-1966">AMS</span><span class="sxs-lookup"><span data-stu-id="69b8c-1966">AMS</span></span>
* <span data-ttu-id="69b8c-1967">Corrigido o bug com a atualização de filtros de conta e de ativo</span><span class="sxs-lookup"><span data-stu-id="69b8c-1967">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-1968">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-1968">AppService</span></span>
* <span data-ttu-id="69b8c-1969">Adicionado suporte para o ASE e o tempo limite para `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1969">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="69b8c-1970">Adicionado suporte para o estabelecimento de CI CD em um pipeline do Azure DevOps de um repositório do Github para aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="69b8c-1970">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="69b8c-1971">Adicionado argumento `--github-pat` a `functionapp devops-build create` para aceitar o token de acesso pessoal do Github</span><span class="sxs-lookup"><span data-stu-id="69b8c-1971">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="69b8c-1972">Adicionado argumento `--github-repository` a `functionapp devops-build create` para aceitar o repositório Github que contém um código-fonte functionapp</span><span class="sxs-lookup"><span data-stu-id="69b8c-1972">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="69b8c-1973">Problema corrigido em que `az webapp up --logs` estava falhando com um erro e atualização da versão .NETCORE padrão para 2.1</span><span class="sxs-lookup"><span data-stu-id="69b8c-1973">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="69b8c-1974">Configurações de functionapp desnecessárias removidas durante a criação de um aplicativo de funções com plano de consumo</span><span class="sxs-lookup"><span data-stu-id="69b8c-1974">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="69b8c-1975">Alterado `webapp up` para que a cadeia de caracteres padrão asp agora acrescente o número no final para criar um novo ASP com base nas opções de SKU</span><span class="sxs-lookup"><span data-stu-id="69b8c-1975">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="69b8c-1976">Adicionado `-b` como uma opção a `webapp up` para iniciar o aplicativo no navegador</span><span class="sxs-lookup"><span data-stu-id="69b8c-1976">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="69b8c-1977">Alterado `webapp deployment source config zip` para lidar com a variável de ambiente `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1977">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="69b8c-1978">Gerenciador de Implantação</span><span class="sxs-lookup"><span data-stu-id="69b8c-1978">Deployment Manager</span></span>
* <span data-ttu-id="69b8c-1979">[VERSÃO PRÉVIA] Criar e gerenciar artefatos que dão suporte a distribuições</span><span class="sxs-lookup"><span data-stu-id="69b8c-1979">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="69b8c-1980">Laboratório</span><span class="sxs-lookup"><span data-stu-id="69b8c-1980">Lab</span></span>
* <span data-ttu-id="69b8c-1981">Corrigido o bug que causa uma saída inicial</span><span class="sxs-lookup"><span data-stu-id="69b8c-1981">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-1982">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-1982">Network</span></span>
* <span data-ttu-id="69b8c-1983">Adicionada delegação de servidor de nome automática a `dns zone create` no pai durante a criação da zona filho</span><span class="sxs-lookup"><span data-stu-id="69b8c-1983">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="69b8c-1984">Recurso</span><span class="sxs-lookup"><span data-stu-id="69b8c-1984">Resource</span></span>
* <span data-ttu-id="69b8c-1985">[PRETERIDO] Argumentos `--link-id`, `--target-id` e `--filter-string` preteridos de `resource link`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1985">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="69b8c-1986">Use os argumentos `--link`, `--target` e `--filter`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1986">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="69b8c-1987">Corrigido o problema em que os comandos `resource link [create|update]` não funcionavam</span><span class="sxs-lookup"><span data-stu-id="69b8c-1987">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="69b8c-1988">Corrigido um problema em que a exclusão usando uma ID de recurso poderia causar falha no erro</span><span class="sxs-lookup"><span data-stu-id="69b8c-1988">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="69b8c-1989">SQL</span><span class="sxs-lookup"><span data-stu-id="69b8c-1989">SQL</span></span>
* <span data-ttu-id="69b8c-1990">Adicionado suporte para fuso horário personalizado nas instâncias gerenciadas</span><span class="sxs-lookup"><span data-stu-id="69b8c-1990">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="69b8c-1991">Alterado para permitir que o nome do pool Elástico seja usado com `sql db update`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1991">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="69b8c-1992">Adicionado o suporte `--no-wait` para `sql server [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1992">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="69b8c-1993">Adicionado o comando `sql server wait`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1993">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-1994">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-1994">Storage</span></span>
* <span data-ttu-id="69b8c-1995">Corrigido o problema com tokens SAS com codificação dupla em `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="69b8c-1995">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="69b8c-1996">VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-1996">VM</span></span>
* <span data-ttu-id="69b8c-1997">Adicionado sinalizador `--skip-shutdown` a `vm|vmss stop` para desligar as VMs sem o desligamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-1997">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="69b8c-1998">Adicionado argumento `--storage-account-type` a `sig image-version create` para definir o tipo de conta do perfil de publicação</span><span class="sxs-lookup"><span data-stu-id="69b8c-1998">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="69b8c-1999">Adicionado argumento `--target-regions` a `sig image-version create` para permitir definir os tipos de conta de armazenamento específico da região</span><span class="sxs-lookup"><span data-stu-id="69b8c-1999">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="69b8c-2000">9 de abril de 2019</span><span class="sxs-lookup"><span data-stu-id="69b8c-2000">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="69b8c-2001">Núcleo</span><span class="sxs-lookup"><span data-stu-id="69b8c-2001">Core</span></span>
* <span data-ttu-id="69b8c-2002">Correção do problema em que algumas extensões mostraram uma versão do `Unknown` e não podiam ser atualizadas</span><span class="sxs-lookup"><span data-stu-id="69b8c-2002">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-2003">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-2003">ACR</span></span>
* <span data-ttu-id="69b8c-2004">Adição de suporte para execução de uma imagem sem contexto</span><span class="sxs-lookup"><span data-stu-id="69b8c-2004">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="69b8c-2005">AMS</span><span class="sxs-lookup"><span data-stu-id="69b8c-2005">AMS</span></span>
* [PRETERIDO]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [ALTERAÇÃO SIGNIFICATIVA]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="69b8c-2008">Adição de suporte para novos parâmetros de criptografia em `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2008">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="69b8c-2009">Adição de novo parâmetro `--filters` a `ams streaming-locator create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2009">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-2010">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-2010">AppService</span></span>
* <span data-ttu-id="69b8c-2011">Adicionado o suporte `--logs` para `webapp up`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2011">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="69b8c-2012">Correção de problemas do comando `functionapp devops-build create` de geração de `azure-pipelines.yml`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2012">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="69b8c-2013">Melhoria do tratamento de erros e indicadores `unctionapp devops-build create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2013">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="69b8c-2014">[ALTERAÇÃO SIGNIFICATIVA] Remoção do sinalizador `--local-git` para o comando `devops-build`; a detecção de git local e a manipulação são obrigatórias para a criação de pipelines do Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="69b8c-2014">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="69b8c-2015">Adição de suporte para a criação de planos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="69b8c-2015">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="69b8c-2016">Adição da capacidade de trocar um plano sob um aplicativo de funções usando `functionapp update --plan`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2016">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="69b8c-2017">Adição de suporte para configurações de expansão de plano Premium do Azure Functions</span><span class="sxs-lookup"><span data-stu-id="69b8c-2017">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="69b8c-2018">CDN</span><span class="sxs-lookup"><span data-stu-id="69b8c-2018">CDN</span></span>
* <span data-ttu-id="69b8c-2019">Adição de suporte para `Microsoft_Standard` e `Standard_ChinaCdn`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2019">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="69b8c-2020">Comentários</span><span class="sxs-lookup"><span data-stu-id="69b8c-2020">Feedback</span></span>
* <span data-ttu-id="69b8c-2021">Alteração de `feedback` para mostrar metadados em comandos executados recentemente</span><span class="sxs-lookup"><span data-stu-id="69b8c-2021">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="69b8c-2022">Alteração de `feedback` para solicitar o auxílio do usuário no processo de criação de problema abrindo um navegador e usando um modelo de problema</span><span class="sxs-lookup"><span data-stu-id="69b8c-2022">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="69b8c-2023">Alteração do `feedback` para imprimir o corpo do problema ao executar com '--verbose'</span><span class="sxs-lookup"><span data-stu-id="69b8c-2023">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="69b8c-2024">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="69b8c-2024">Monitor</span></span>
* <span data-ttu-id="69b8c-2025">Correção de um problema em que “count” não era um valor permitido com `metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2025">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="69b8c-2026">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-2026">Network</span></span>
* <span data-ttu-id="69b8c-2027">Correção do formato de tabela que não estava sendo exibido com `vnet-gateway list-bgp-peer-status`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2027">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="69b8c-2028">Adição dos comandos `list-request-headers` e `list-response-headers` para `application-gateway rewrite-rule`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2028">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="69b8c-2029">Adição do comando `list-server-variables` para `application-gateway rewrite-rule condition`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2029">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="69b8c-2030">Correção de um problema em que a atualização do estado do link em uma porta express-route geraria uma exceção de atributo desconhecido `express-route port update`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2030">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="69b8c-2031">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="69b8c-2031">PrivateDNS</span></span>
* <span data-ttu-id="69b8c-2032">Adição de `network private-dns` para zonas de DNS privado</span><span class="sxs-lookup"><span data-stu-id="69b8c-2032">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="69b8c-2033">Recurso</span><span class="sxs-lookup"><span data-stu-id="69b8c-2033">Resource</span></span>
* <span data-ttu-id="69b8c-2034">Correção do problema com `deployment create` e `group deployment create`, em que um arquivo de parâmetros com um conjunto vazio de parâmetros não funcionaria</span><span class="sxs-lookup"><span data-stu-id="69b8c-2034">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="69b8c-2035">Função</span><span class="sxs-lookup"><span data-stu-id="69b8c-2035">Role</span></span>
* <span data-ttu-id="69b8c-2036">Correção de `create-for-rbac` para lidar corretamente com `--years`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2036">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="69b8c-2037">[ALTERAÇÃO SIGNIFICATIVA] Alteração de `role assignment delete` para solicitar ao excluir todas as atribuições na assinatura incondicionalmente</span><span class="sxs-lookup"><span data-stu-id="69b8c-2037">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="69b8c-2038">SQL</span><span class="sxs-lookup"><span data-stu-id="69b8c-2038">SQL</span></span>
* <span data-ttu-id="69b8c-2039">Atualização de `sql mi [create|update]` com as propriedades proxyOverride e publicDataEndpointEnabled</span><span class="sxs-lookup"><span data-stu-id="69b8c-2039">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-2040">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-2040">Storage</span></span>
* <span data-ttu-id="69b8c-2041">[ALTERAÇÃO SIGNIFICATIVA] Remoção do resultado de `storage blob delete`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2041">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="69b8c-2042">Adição de `--full-uri` a `storage blob generate-sas` para criar o URI completo para o blob com SAS</span><span class="sxs-lookup"><span data-stu-id="69b8c-2042">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="69b8c-2043">Adição de `--file-snapshot` a `storage file copy start` para copiar arquivo do instantâneo</span><span class="sxs-lookup"><span data-stu-id="69b8c-2043">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="69b8c-2044">Alteração de `storage blob copy cancel` para mostrar apenas o erro em vez da exceção para NoPendingCopyOperation</span><span class="sxs-lookup"><span data-stu-id="69b8c-2044">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="69b8c-2045">26 de março de 2019</span><span class="sxs-lookup"><span data-stu-id="69b8c-2045">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="69b8c-2046">Núcleo</span><span class="sxs-lookup"><span data-stu-id="69b8c-2046">Core</span></span>
* <span data-ttu-id="69b8c-2047">Correção de problemas com incompatibilidade da extensão de desenvolvimento</span><span class="sxs-lookup"><span data-stu-id="69b8c-2047">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="69b8c-2048">Agora o tratamento de erros encaminha os clientes para a página de problemas</span><span class="sxs-lookup"><span data-stu-id="69b8c-2048">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="69b8c-2049">Nuvem</span><span class="sxs-lookup"><span data-stu-id="69b8c-2049">Cloud</span></span>
* <span data-ttu-id="69b8c-2050">Erro de “assinatura não encontrada” corrigido em `cloud set`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2050">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-2051">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-2051">ACR</span></span>
* <span data-ttu-id="69b8c-2052">Corrigidas fontes redundantes na importação de imagem.</span><span class="sxs-lookup"><span data-stu-id="69b8c-2052">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="69b8c-2053">`--auth-mode` adicionado aos comandos `acr build`, `acr run`, `acr task create` e `acr task update`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2053">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="69b8c-2054">Grupo de comandos “acr task credential” adicionado para gerenciar as credenciais de uma Tarefa</span><span class="sxs-lookup"><span data-stu-id="69b8c-2054">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="69b8c-2055">“--no-wait” adicionado ao comando `acr build`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2055">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-2056">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-2056">AppService</span></span>
* <span data-ttu-id="69b8c-2057">Bug corrigido onde `webapp up` não estava lidando corretamente com a execução do diretório vazio ou do cenário de código desconhecido</span><span class="sxs-lookup"><span data-stu-id="69b8c-2057">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="69b8c-2058">Bug corrigido onde os slots não funcionavam para `[webapp|functionapp] config ssl bind`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2058">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="69b8c-2059">Serviço de BOT</span><span class="sxs-lookup"><span data-stu-id="69b8c-2059">BOT Service</span></span>
* <span data-ttu-id="69b8c-2060">`bot prepare-deploy` adicionado para se preparar para a implantação de bots via `webapp`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2060">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="69b8c-2061">`bot create --kind registration` alterado para mostrar a senha se ela não for fornecida</span><span class="sxs-lookup"><span data-stu-id="69b8c-2061">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="69b8c-2062">[ALTERAÇÃO SIGNIFICATIVA]`--endpoint` alterado em `bot create --kind registration` como padrão para uma cadeia de caracteres vazia, em vez de ser requerido</span><span class="sxs-lookup"><span data-stu-id="69b8c-2062">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="69b8c-2063">Adicionado `SCM_DO_BUILD_DURING_DEPLOYMENT` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.</span><span class="sxs-lookup"><span data-stu-id="69b8c-2063">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="69b8c-2064">CDN</span><span class="sxs-lookup"><span data-stu-id="69b8c-2064">CDN</span></span>
* <span data-ttu-id="69b8c-2065">Adicionado o suporte ao `--no-wait` para `cdn endpoint [create|update|start|stop|delete|load|purge]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2065">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* [ALTERAÇÃO SIGNIFICATIVA]: `cdn endpoint create` alterado para o comportamento de cache da cadeia de consulta padrão.
[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour. <span data-ttu-id="69b8c-2067">Não há mais padrão para "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="69b8c-2067">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="69b8c-2068">Agora, ele é definido pelo serviço</span><span class="sxs-lookup"><span data-stu-id="69b8c-2068">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="69b8c-2069">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="69b8c-2069">Cosmosdb</span></span>
* <span data-ttu-id="69b8c-2070">Suporte adicionado para `--enable-multiple-write-locations` na atualização da conta</span><span class="sxs-lookup"><span data-stu-id="69b8c-2070">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="69b8c-2071">O subgrupo `network-rule` foi adicionado com os comandos `add`, `remove` e `list` para gerenciar as regras de VNET de uma conta do Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="69b8c-2071">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="69b8c-2072">Interativo</span><span class="sxs-lookup"><span data-stu-id="69b8c-2072">Interactive</span></span>
* <span data-ttu-id="69b8c-2073">Incompatibilidade corrigida com a extensão Interativa instalada por meio do azdev</span><span class="sxs-lookup"><span data-stu-id="69b8c-2073">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="69b8c-2074">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="69b8c-2074">Monitor</span></span>
* <span data-ttu-id="69b8c-2075">Alterado para permitir o valor de dimensão `*` para `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2075">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-2076">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-2076">Network</span></span>
* <span data-ttu-id="69b8c-2077">Grupo de comandos `rewrite-rule` adicionado em `application-gateway`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2077">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="69b8c-2078">Perfil</span><span class="sxs-lookup"><span data-stu-id="69b8c-2078">Profile</span></span>
* <span data-ttu-id="69b8c-2079">Suporte de conta no nível do locatário para a identidade de serviço gerenciado adicionado em `login`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2079">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="69b8c-2080">Postgres</span><span class="sxs-lookup"><span data-stu-id="69b8c-2080">Postgres</span></span> 
* <span data-ttu-id="69b8c-2081">Adicionados os comandos postgresql `replica` e `restart server`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2081">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="69b8c-2082">Alterado para obter o local padrão do grupo de recursos quando não fornecido para criar servidores e adicionar validação para os dias de retenção</span><span class="sxs-lookup"><span data-stu-id="69b8c-2082">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="69b8c-2083">Recurso</span><span class="sxs-lookup"><span data-stu-id="69b8c-2083">Resource</span></span>
* <span data-ttu-id="69b8c-2084">Saída da tabela aperfeiçoada para `deployment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2084">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="69b8c-2085">Corrigido o problema com `deployment [create|validate]` onde o tipo secureObject não era reconhecido</span><span class="sxs-lookup"><span data-stu-id="69b8c-2085">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="69b8c-2086">Grafo</span><span class="sxs-lookup"><span data-stu-id="69b8c-2086">Graph</span></span>
* <span data-ttu-id="69b8c-2087">Adicionado o suporte ao `--end-date` para `ad [app|sp] credential reset`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2087">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="69b8c-2088">Suporte adicionado para acrescentar permissões com `ad app permission add`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2088">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="69b8c-2089">Bug corrigido com `ad app permission list` quando não havia nenhuma permissão</span><span class="sxs-lookup"><span data-stu-id="69b8c-2089">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="69b8c-2090">`ad sp delete` alterado para ignorar a exclusão da atribuição de função se a conta atual não tem nenhuma assinatura</span><span class="sxs-lookup"><span data-stu-id="69b8c-2090">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="69b8c-2091">`ad app create` alterado para `--identifier-uris` passar para lista vazia como padrão se não fornecido</span><span class="sxs-lookup"><span data-stu-id="69b8c-2091">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-2092">armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-2092">storage</span></span>
* <span data-ttu-id="69b8c-2093">`--snapshot` adicionado a `storage file download-batch` para baixar de um instantâneo de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-2093">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="69b8c-2094">Barra de progresso `storage blob [download-batch|upload-batch]` alterada para ser menos detalhada e indicar o blob atual</span><span class="sxs-lookup"><span data-stu-id="69b8c-2094">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="69b8c-2095">Problema corrigido com `storage account update` ao atualizar os parâmetros de criptografia</span><span class="sxs-lookup"><span data-stu-id="69b8c-2095">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="69b8c-2096">Problema corrigido onde `storage blob show` falharia ao usar o oauth (`--auth-mode=login`)</span><span class="sxs-lookup"><span data-stu-id="69b8c-2096">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="69b8c-2097">VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-2097">VM</span></span>
* <span data-ttu-id="69b8c-2098">Adicionado o comando `image update`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2098">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="69b8c-2099">12 de março de 2019</span><span class="sxs-lookup"><span data-stu-id="69b8c-2099">March 12, 2019</span></span>

<span data-ttu-id="69b8c-2100">Versão 2.0.60</span><span class="sxs-lookup"><span data-stu-id="69b8c-2100">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="69b8c-2101">Núcleo</span><span class="sxs-lookup"><span data-stu-id="69b8c-2101">Core</span></span>

* <span data-ttu-id="69b8c-2102">Foi corrigido um erro incorreto no `cloud set` sobre assinatura não encontrada.</span><span class="sxs-lookup"><span data-stu-id="69b8c-2102">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-2103">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-2103">ACR</span></span>

* <span data-ttu-id="69b8c-2104">Corrigidas fontes redundantes na importação de imagem.</span><span class="sxs-lookup"><span data-stu-id="69b8c-2104">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="69b8c-2105">ACS</span><span class="sxs-lookup"><span data-stu-id="69b8c-2105">ACS</span></span>

* <span data-ttu-id="69b8c-2106">Alteração para ignorar o parâmetro `--listen-address` para `aks browse` se ele não for compatível com kubectl</span><span class="sxs-lookup"><span data-stu-id="69b8c-2106">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="69b8c-2107">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-2107">AppService</span></span>

* <span data-ttu-id="69b8c-2108">Adicionado `[webapp|functionapp] deployment list-publishing-credentials` para obter a URL de publicação do Kudu e suas credenciais.</span><span class="sxs-lookup"><span data-stu-id="69b8c-2108">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="69b8c-2109">Removida a instrução de impressão errônea de `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="69b8c-2109">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="69b8c-2110">Corrigido `functionapp` para definir a imagem correta do runtime nos planos do Serviço de Aplicativo no Linux.</span><span class="sxs-lookup"><span data-stu-id="69b8c-2110">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="69b8c-2111">Removida a marca de versão prévia do `webapp up` e adicionadas melhorias ao comando.</span><span class="sxs-lookup"><span data-stu-id="69b8c-2111">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="69b8c-2112">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="69b8c-2112">Botservice</span></span>

* <span data-ttu-id="69b8c-2113">Adicionado `SCM_DO_BUILD_DURING_DEPLOYMENT` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.</span><span class="sxs-lookup"><span data-stu-id="69b8c-2113">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="69b8c-2114">Adicionados `Microsoft-BotFramework-AppId` e `Microsoft-BotFramework-AppPassword` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.</span><span class="sxs-lookup"><span data-stu-id="69b8c-2114">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="69b8c-2115">Removidas as aspas simples da saída de comando `bot publish`, no final de `bot create`.</span><span class="sxs-lookup"><span data-stu-id="69b8c-2115">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="69b8c-2116">Alterado `bot publish` para que seja assíncrono.</span><span class="sxs-lookup"><span data-stu-id="69b8c-2116">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="69b8c-2117">Contêiner</span><span class="sxs-lookup"><span data-stu-id="69b8c-2117">Container</span></span>

* <span data-ttu-id="69b8c-2118">Adicionado o argumento `--no-wait` para `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2118">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="69b8c-2119">EventHub</span><span class="sxs-lookup"><span data-stu-id="69b8c-2119">EventHub</span></span>

* <span data-ttu-id="69b8c-2120">Adicionado o sinalizador `--skip-empty-archives` a `eventhub create|update` para dar suporte a arquivos vazios na captura.</span><span class="sxs-lookup"><span data-stu-id="69b8c-2120">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="69b8c-2121">Localizar</span><span class="sxs-lookup"><span data-stu-id="69b8c-2121">Find</span></span>

* <span data-ttu-id="69b8c-2122">Atualização de funcionalidade principal</span><span class="sxs-lookup"><span data-stu-id="69b8c-2122">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="69b8c-2123">HDInsight</span><span class="sxs-lookup"><span data-stu-id="69b8c-2123">HDInsight</span></span>

* <span data-ttu-id="69b8c-2124">Adicionado o parâmetro `--storage-account-managed-identity` a `hdinsight create` para oferecer suporte ao MSI do ADLS Gen2.</span><span class="sxs-lookup"><span data-stu-id="69b8c-2124">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-2125">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-2125">Network</span></span>

* <span data-ttu-id="69b8c-2126">Corrigido o problema com `vpn-connection update`, onde a atualização de uma conexão VPN entre gateways em assinaturas diferentes falharia.</span><span class="sxs-lookup"><span data-stu-id="69b8c-2126">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="69b8c-2127">Rdbms</span><span class="sxs-lookup"><span data-stu-id="69b8c-2127">Rdbms</span></span>

* <span data-ttu-id="69b8c-2128">Correções secundárias para obter a localização padrão do grupo de recursos, quando não fornecida, para criar servidores e adicionar validação nos dias de retenção.</span><span class="sxs-lookup"><span data-stu-id="69b8c-2128">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="69b8c-2129">Função</span><span class="sxs-lookup"><span data-stu-id="69b8c-2129">Role</span></span>

* <span data-ttu-id="69b8c-2130">Corrigido `role definition update` para usar ID a fim de resolver a definição corretamente.</span><span class="sxs-lookup"><span data-stu-id="69b8c-2130">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="69b8c-2131">Alterado `ad app credential reset` para remover a suposição de que a entidade de serviço do aplicativo já existe.</span><span class="sxs-lookup"><span data-stu-id="69b8c-2131">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="69b8c-2132">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="69b8c-2132">Service Fabric</span></span>

* <span data-ttu-id="69b8c-2133">Corrigido o problema com o fato de `sf cluster list` não ser iterável.</span><span class="sxs-lookup"><span data-stu-id="69b8c-2133">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="69b8c-2134">26 de fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="69b8c-2134">February 26, 2019</span></span>

<span data-ttu-id="69b8c-2135">Versão 2.0.59</span><span class="sxs-lookup"><span data-stu-id="69b8c-2135">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="69b8c-2136">Núcleo</span><span class="sxs-lookup"><span data-stu-id="69b8c-2136">Core</span></span>

* <span data-ttu-id="69b8c-2137">Corrigido o problema onde algumas instâncias usando `--subscription NAME` produziriam uma exceção</span><span class="sxs-lookup"><span data-stu-id="69b8c-2137">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-2138">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-2138">ACR</span></span>

* <span data-ttu-id="69b8c-2139">Parâmetro `--target` adicionado para os comandos `acr build`, `acr task create` e `acr task update`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2139">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="69b8c-2140">Melhor tratamento de erros para os comandos de execução quando não conectado ao Azure</span><span class="sxs-lookup"><span data-stu-id="69b8c-2140">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="69b8c-2141">ACS</span><span class="sxs-lookup"><span data-stu-id="69b8c-2141">ACS</span></span>

* <span data-ttu-id="69b8c-2142">Opção `--listen-address` adicionada a `aks port-forward`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2142">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-2143">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-2143">AppService</span></span>

* <span data-ttu-id="69b8c-2144">Adicionado o comando `functionapp devops-build`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2144">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="69b8c-2145">Lote</span><span class="sxs-lookup"><span data-stu-id="69b8c-2145">Batch</span></span>
* <span data-ttu-id="69b8c-2146">[ALTERAÇÃO SIGNIFICATIVA] Comando `batch pool upgrade os` removido</span><span class="sxs-lookup"><span data-stu-id="69b8c-2146">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="69b8c-2147">[ALTERAÇÃO SIGNIFICATIVA] Propriedade `Pacakges` removida das respostas `Application`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2147">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="69b8c-2148">Comando `batch application package list` adicionado para listar os pacotes de um aplicativo</span><span class="sxs-lookup"><span data-stu-id="69b8c-2148">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="69b8c-2149">[ALTERAÇÃO SIGNIFICATIVA]`--application-id` alterado para `--application-name` em todos os comandos `batch application`,</span><span class="sxs-lookup"><span data-stu-id="69b8c-2149">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="69b8c-2150">O argumento `--json-file` foi adicionado aos comandos para a solicitação de resposta da API bruta</span><span class="sxs-lookup"><span data-stu-id="69b8c-2150">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="69b8c-2151">Validação atualizada para incluir automaticamente `https://` em todos os pontos de extremidade, se ausente</span><span class="sxs-lookup"><span data-stu-id="69b8c-2151">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="69b8c-2152">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="69b8c-2152">CosmosDB</span></span>

* <span data-ttu-id="69b8c-2153">O subgrupo `network-rule` foi adicionado com os comandos `add`, `remove` e `list` para gerenciar as regras de VNET de uma conta do Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="69b8c-2153">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="69b8c-2154">Kusto</span><span class="sxs-lookup"><span data-stu-id="69b8c-2154">Kusto</span></span>

* <span data-ttu-id="69b8c-2155">[ALTERAÇÃO SIGNIFICATIVA] Os tipos `hot_cache_period` e `soft_delete_period` foram alterados do banco de dados para o formato de duração ISO8601</span><span class="sxs-lookup"><span data-stu-id="69b8c-2155">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-2156">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-2156">Network</span></span>

* <span data-ttu-id="69b8c-2157">Adicionado o argumento `--express-route-gateway-bypass` para `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2157">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="69b8c-2158">Foram adicionados os grupos de comando a partir das extensões `express-route`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2158">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="69b8c-2159">Os grupos de comando `express-route gateway` e `express-route port` foram adicionados</span><span class="sxs-lookup"><span data-stu-id="69b8c-2159">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="69b8c-2160">Adicionado o argumento `--legacy-mode` para `express-route peering [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2160">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="69b8c-2161">Os argumentos `--allow-classic-operations` e `--express-route-port` foram adicionados a `express-route [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2161">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="69b8c-2162">Adicionado o argumento `--gateway-default-site` para `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2162">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="69b8c-2163">Os comandos `ipsec-policy` foram adicionados a `vnet-gateway`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2163">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="69b8c-2164">Recurso</span><span class="sxs-lookup"><span data-stu-id="69b8c-2164">Resource</span></span>

* <span data-ttu-id="69b8c-2165">Foi corrigido o problema com `deployment create` em que o campo do tipo diferencia letras maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="69b8c-2165">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="69b8c-2166">Foi adicionado o suporte para arquivo de parâmetros de URI a `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2166">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="69b8c-2167">Foi adicionado o suporte para parâmetros de URI e definições a `policy set-definition update`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2167">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="69b8c-2168">Foi corrigido o tratamento de parâmetros e regras para `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2168">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="69b8c-2169">Foi corrigido o problema com `resource show/update/delete/tag/invoke-action` em que as IDs de assinatura cruzada não respeitaram corretamente a ID da assinatura</span><span class="sxs-lookup"><span data-stu-id="69b8c-2169">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="69b8c-2170">Função</span><span class="sxs-lookup"><span data-stu-id="69b8c-2170">Role</span></span>

* <span data-ttu-id="69b8c-2171">Foi adicionado o suporte para as funções do aplicativo a `ad app [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2171">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="69b8c-2172">VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-2172">VM</span></span>

* <span data-ttu-id="69b8c-2173">Foi corrigido o problema com `vm create where ` – a rede acelerada não foi habilitada por padrão no Ubuntu 18.0</span><span class="sxs-lookup"><span data-stu-id="69b8c-2173">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="69b8c-2174">12 de fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="69b8c-2174">February 12, 2019</span></span>

<span data-ttu-id="69b8c-2175">Versão 2.0.58</span><span class="sxs-lookup"><span data-stu-id="69b8c-2175">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="69b8c-2176">Núcleo</span><span class="sxs-lookup"><span data-stu-id="69b8c-2176">Core</span></span>

* <span data-ttu-id="69b8c-2177">`az --version` agora exibe uma notificação se você tiver pacotes para atualização</span><span class="sxs-lookup"><span data-stu-id="69b8c-2177">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="69b8c-2178">A regressão em que `--ids` não pode ser usado com a saída JSON foi corrigida</span><span class="sxs-lookup"><span data-stu-id="69b8c-2178">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-2179">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-2179">ACR</span></span>
* <span data-ttu-id="69b8c-2180">[ALTERAÇÃO SIGNIFICATIVA] O grupo de comandos `acr build-task` foi removido</span><span class="sxs-lookup"><span data-stu-id="69b8c-2180">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="69b8c-2181">[ALTERAÇÃO SIGNIFICATIVA] As opções `--tag` e `--manifest` de `acr repository delete` foram removidas</span><span class="sxs-lookup"><span data-stu-id="69b8c-2181">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="69b8c-2182">ACS</span><span class="sxs-lookup"><span data-stu-id="69b8c-2182">ACS</span></span>
* <span data-ttu-id="69b8c-2183">Suporte adicionado a `aks [enable-addons|disable-addons]` para nomes que não diferenciam maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="69b8c-2183">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="69b8c-2184">Suporte adicionado para a operação de atualização do Azure Active Directory usando `aks update-credentials --reset-aad`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2184">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="69b8c-2185">Um esclarecimento informando que `--output` é ignorado para `aks get-credentials` foi adicionado</span><span class="sxs-lookup"><span data-stu-id="69b8c-2185">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="69b8c-2186">AMS</span><span class="sxs-lookup"><span data-stu-id="69b8c-2186">AMS</span></span>
* <span data-ttu-id="69b8c-2187">Adicionados os comandos `ams streaming-endpoint [start | stop | create | update] wait`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2187">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="69b8c-2188">Adicionados os comandos `ams live-event [create | start | stop | reset] wait`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2188">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-2189">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-2189">Appservice</span></span>
* <span data-ttu-id="69b8c-2190">Foi adicionada a capacidade de criar e configurar funções usando contêineres de ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-2190">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="69b8c-2191">Suporte adicionado para a atualização das configurações de aplicativos Web por meio de JSON</span><span class="sxs-lookup"><span data-stu-id="69b8c-2191">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="69b8c-2192">A ajuda foi aprimorada para `appservice-plan-update`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2192">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="69b8c-2193">Suporte adicionado para o App Insights para auxiliar na criação de aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="69b8c-2193">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="69b8c-2194">Os problemas com o SSH do aplicativo Web foram corrigidos</span><span class="sxs-lookup"><span data-stu-id="69b8c-2194">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="69b8c-2195">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="69b8c-2195">Botservice</span></span>
* <span data-ttu-id="69b8c-2196">A experiência do usuário para `bot publish` foi aprimorada</span><span class="sxs-lookup"><span data-stu-id="69b8c-2196">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="69b8c-2197">Foram adicionados avisos de tempos limite ao executar `npm install` durante `az bot publish`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2197">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="69b8c-2198">O caractere inválido `.` de `--name` em `az bot create` foi removido</span><span class="sxs-lookup"><span data-stu-id="69b8c-2198">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="69b8c-2199">Alteração para interromper a geração aleatória de nomes de recursos durante a criação do Armazenamento do Azure, Plano do Serviço de Aplicativo, Aplicativo Web/de funções e Application Insights</span><span class="sxs-lookup"><span data-stu-id="69b8c-2199">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="69b8c-2200">[PRETERIDO] O argumento `--proj-name` foi preterido em favor de `--proj-file-path`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2200">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="69b8c-2201">`az bot publish` foi alterado para remover arquivos de implantação do Node.js do IIS buscados, caso eles já não existissem</span><span class="sxs-lookup"><span data-stu-id="69b8c-2201">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="69b8c-2202">Foi adicionado o argumento `--keep-node-modules` para `az bot publish` para não excluir a pasta `node_modules` no Serviço de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="69b8c-2202">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="69b8c-2203">O par chave-valor `"publishCommand"` foi adicionado à saída de `az bot create` durante a criação de uma função do Azure ou bot de aplicativo Web</span><span class="sxs-lookup"><span data-stu-id="69b8c-2203">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="69b8c-2204">O valor de `"publishCommand"` é um comando `az bot publish` que é automaticamente preenchido com os parâmetros necessários para publicar o bot recém-criado</span><span class="sxs-lookup"><span data-stu-id="69b8c-2204">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="69b8c-2205">O `"WEBSITE_NODE_DEFAULT_VERSION"` foi atualizado no modelo do ARM para que os bots de SDK v4 usem 10.14.1 em vez de 8.9.4</span><span class="sxs-lookup"><span data-stu-id="69b8c-2205">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="69b8c-2206">Key Vault</span><span class="sxs-lookup"><span data-stu-id="69b8c-2206">Key Vault</span></span>
* <span data-ttu-id="69b8c-2207">Foi corrigido o problema com `keyvault secret backup`, em que alguns usuários recebiam um erro `unexpected_keyword` ao usar `--id`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2207">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="69b8c-2208">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="69b8c-2208">Monitor</span></span>
* <span data-ttu-id="69b8c-2209">`monitor metrics alert [create|update]` foi alterado para permitir o valor dimensional `*`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2209">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-2210">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-2210">Network</span></span>
* <span data-ttu-id="69b8c-2211">`dns zone export` foi alterado para garantir que CNAMEs exportados fossem FQDNs</span><span class="sxs-lookup"><span data-stu-id="69b8c-2211">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="69b8c-2212">O parâmetro `--gateway-name` foi adicionado a `nic ip-config address-pool [add|remove]` para dar suporte a pools de endereços de back-end de gateway de aplicativo</span><span class="sxs-lookup"><span data-stu-id="69b8c-2212">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="69b8c-2213">Os argumentos `--traffic-analytics` e `--workspace` foram adicionados a `network watcher flow-log configure` para dar suporte à análise de tráfego por meio de um espaço de trabalho do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="69b8c-2213">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="69b8c-2214">`--idle-timeout` e `--floating-ip` foram adicionados a `lb inbound-nat-pool [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2214">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="69b8c-2215">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="69b8c-2215">Policy Insights</span></span>
* <span data-ttu-id="69b8c-2216">Os comandos `policy remediation` foram adicionados para dar suporte a recursos de correção de política de recursos</span><span class="sxs-lookup"><span data-stu-id="69b8c-2216">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="69b8c-2217">RDBMS</span><span class="sxs-lookup"><span data-stu-id="69b8c-2217">RDBMS</span></span>
* <span data-ttu-id="69b8c-2218">A mensagem e os parâmetros de comando de ajuda foram aprimorados</span><span class="sxs-lookup"><span data-stu-id="69b8c-2218">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="69b8c-2219">Redis</span><span class="sxs-lookup"><span data-stu-id="69b8c-2219">Redis</span></span>
* <span data-ttu-id="69b8c-2220">Foram adicionados comandos para gerenciar regras de firewall (criar, atualizar, excluir, mostrar, listar)</span><span class="sxs-lookup"><span data-stu-id="69b8c-2220">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="69b8c-2221">Foram adicionados comandos para gerenciar links do servidor (criar, excluir, mostrar, listar)</span><span class="sxs-lookup"><span data-stu-id="69b8c-2221">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="69b8c-2222">Foram adicionados comandos para gerenciar o agendamento de patches (criar, atualizar, excluir, mostrar)</span><span class="sxs-lookup"><span data-stu-id="69b8c-2222">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="69b8c-2223">Suporte adicionado para Zonas de Disponibilidade e versão mínima de TLS para criar Redis</span><span class="sxs-lookup"><span data-stu-id="69b8c-2223">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="69b8c-2224">[ALTERAÇÃO SIGNIFICATIVA] Os comandos `redis update-settings` e `redis list-all` foram removidos</span><span class="sxs-lookup"><span data-stu-id="69b8c-2224">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="69b8c-2225">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro para `redis create`: “configurações de locatário” não é aceito no formato chave[=valor]</span><span class="sxs-lookup"><span data-stu-id="69b8c-2225">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="69b8c-2226">[PRETERIDO] Uma mensagem de aviso foi adicionada para preterir o comando `redis import-method`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2226">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="69b8c-2227">Função</span><span class="sxs-lookup"><span data-stu-id="69b8c-2227">Role</span></span>
* <span data-ttu-id="69b8c-2228">[ALTERAÇÃO SIGNIFICATIVA] O comando `az identity` foi movido dos comandos `vm` para esta localização</span><span class="sxs-lookup"><span data-stu-id="69b8c-2228">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="69b8c-2229">SQL VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-2229">SQL VM</span></span>
* <span data-ttu-id="69b8c-2230">[PRETERIDO] O argumento `--boostrap-acc-pwd` foi preterido devido a um erro de digitação</span><span class="sxs-lookup"><span data-stu-id="69b8c-2230">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="69b8c-2231">VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-2231">VM</span></span>
* <span data-ttu-id="69b8c-2232">`vm list-skus` foi alterado para permitir o uso de `--all` no lugar de `--all true`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2232">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="69b8c-2233">Adicionado `vmss run-command [invoke | list | show]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2233">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="69b8c-2234">Foi corrigido o bug em que `vmss encryption enable` falhava se fosse executado anteriormente</span><span class="sxs-lookup"><span data-stu-id="69b8c-2234">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="69b8c-2235">[ALTERAÇÃO SIGNIFICATIVA] O comando `az identity` foi movido para os comandos `role`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2235">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="69b8c-2236">31 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="69b8c-2236">January 31, 2019</span></span>

<span data-ttu-id="69b8c-2237">Versão 2.0.57</span><span class="sxs-lookup"><span data-stu-id="69b8c-2237">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="69b8c-2238">Núcleo</span><span class="sxs-lookup"><span data-stu-id="69b8c-2238">Core</span></span>

* <span data-ttu-id="69b8c-2239">Hotfix para o [problema 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="69b8c-2239">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="69b8c-2240">28 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="69b8c-2240">January 28, 2019</span></span>

<span data-ttu-id="69b8c-2241">Versão 2.0.56</span><span class="sxs-lookup"><span data-stu-id="69b8c-2241">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-2242">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-2242">ACR</span></span>
* <span data-ttu-id="69b8c-2243">Suporte adicionado para regras de rede virtual/IP</span><span class="sxs-lookup"><span data-stu-id="69b8c-2243">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="69b8c-2244">ACS</span><span class="sxs-lookup"><span data-stu-id="69b8c-2244">ACS</span></span>
* <span data-ttu-id="69b8c-2245">Adicionada visualização dos nós virtuais</span><span class="sxs-lookup"><span data-stu-id="69b8c-2245">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="69b8c-2246">Comandos do OpenShift gerenciado foram adicionados</span><span class="sxs-lookup"><span data-stu-id="69b8c-2246">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="69b8c-2247">Suporte adicionado para operações de atualização da entidade de serviço com `aks update-credentials -reset-service-principal`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2247">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="69b8c-2248">AMS</span><span class="sxs-lookup"><span data-stu-id="69b8c-2248">AMS</span></span>
* <span data-ttu-id="69b8c-2249">[ALTERAÇÃO SIGNIFICATIVA]`ams asset get-streaming-locators` renomeado para `ams asset list-streaming-locators`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2249">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="69b8c-2250">[ALTERAÇÃO SIGNIFICATIVA]`ams streaming-locator get-content-keys` renomeado para `ams streaming-locator list-content-keys`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2250">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-2251">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-2251">Appservice</span></span>
* <span data-ttu-id="69b8c-2252">Suporte adicionado para o App Insights no `functionapp create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2252">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="69b8c-2253">Suporte adicionado para a criação do plano de serviço de aplicativo (incluindo Elástico Premium) para Aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="69b8c-2253">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="69b8c-2254">Foram corrigidos os problemas com de configuração de aplicativo com os planos Elástico Premium</span><span class="sxs-lookup"><span data-stu-id="69b8c-2254">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="69b8c-2255">Contêiner</span><span class="sxs-lookup"><span data-stu-id="69b8c-2255">Container</span></span>
* <span data-ttu-id="69b8c-2256">Adicionado o comando `container start`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2256">Added `container start` command</span></span>
* <span data-ttu-id="69b8c-2257">Alteração para permitir o uso de valores decimais para CPU durante a criação do contêiner</span><span class="sxs-lookup"><span data-stu-id="69b8c-2257">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="69b8c-2258">EventGrid</span><span class="sxs-lookup"><span data-stu-id="69b8c-2258">EventGrid</span></span>
* <span data-ttu-id="69b8c-2259">Parâmetro `--deadletter-endpoint` adicionado a `event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2259">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="69b8c-2260">Storagequeue e hybridconnection foram adicionados como novos valores para 'event-subscription [create|update] --endpoint-type\`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2260">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="69b8c-2261">Os parâmetros `--max-delivery-attempts` e `--event-ttl` foram adicionados a `event-subscription create` para especificar a política de repetição para eventos</span><span class="sxs-lookup"><span data-stu-id="69b8c-2261">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="69b8c-2262">Uma mensagem de aviso foi adicionada a `event-subscription [create|update]` quando o webhook como destino for usado para uma assinatura de evento</span><span class="sxs-lookup"><span data-stu-id="69b8c-2262">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="69b8c-2263">O parâmetro source-resource-id foi adicionado para todos os comandos relacionados a eventos e marcar todos os outros parâmetros relacionados ao recurso de origem como preteridos</span><span class="sxs-lookup"><span data-stu-id="69b8c-2263">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="69b8c-2264">HDInsight</span><span class="sxs-lookup"><span data-stu-id="69b8c-2264">HDInsight</span></span>
* <span data-ttu-id="69b8c-2265">[ALTERAÇÃO SIGNIFICATIVA] Os parâmetros `--virtual-network` e `--subnet-name` de `hdinsight [application] create` foram removidos</span><span class="sxs-lookup"><span data-stu-id="69b8c-2265">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="69b8c-2266">[ALTERAÇÃO SIGNIFICATIVA]`hdinsight create --storage-account` foi alterado para aceitar o nome ou ID da conta de armazenamento, em vez de pontos de extremidade de blob</span><span class="sxs-lookup"><span data-stu-id="69b8c-2266">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="69b8c-2267">Parâmetros `--vnet-name` e `--subnet-name` adicionados a `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2267">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="69b8c-2268">Suporte adicionado para a criptografia de disco e Enterprise Security Package ao `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2268">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="69b8c-2269">Adicionado o comando `hdinsight rotate-disk-encryption-key`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2269">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="69b8c-2270">Adicionado o comando `hdinsight update`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2270">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="69b8c-2271">IoT</span><span class="sxs-lookup"><span data-stu-id="69b8c-2271">IoT</span></span>
* <span data-ttu-id="69b8c-2272">O formato de codificação foi adicionado ao comando routing-endpoint</span><span class="sxs-lookup"><span data-stu-id="69b8c-2272">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="69b8c-2273">Kusto</span><span class="sxs-lookup"><span data-stu-id="69b8c-2273">Kusto</span></span>
* <span data-ttu-id="69b8c-2274">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="69b8c-2274">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="69b8c-2275">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="69b8c-2275">Monitor</span></span>
* <span data-ttu-id="69b8c-2276">A comparação de ID foi alterada para diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="69b8c-2276">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="69b8c-2277">Perfil</span><span class="sxs-lookup"><span data-stu-id="69b8c-2277">Profile</span></span>
* <span data-ttu-id="69b8c-2278">A conta de nível de locatário foi habilitada para a identidade de serviço gerenciada de `login`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2278">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-2279">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-2279">Network</span></span>
* <span data-ttu-id="69b8c-2280">Foi corrigido o problema com `express-route update`: em que o argumento `--bandwidth` era ignorado</span><span class="sxs-lookup"><span data-stu-id="69b8c-2280">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="69b8c-2281">Foi corrigido o problema com `ddos-protection update` em que definir a compreensão levava ao rastreamento de pilha</span><span class="sxs-lookup"><span data-stu-id="69b8c-2281">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="69b8c-2282">Recurso</span><span class="sxs-lookup"><span data-stu-id="69b8c-2282">Resource</span></span>
* <span data-ttu-id="69b8c-2283">Suporte adicionado para o arquivo de parâmetros de URI à `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2283">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="69b8c-2284">Suporte adicionado para a identidade gerenciada à `policy assignment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2284">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="69b8c-2285">Máquina virtual SQL</span><span class="sxs-lookup"><span data-stu-id="69b8c-2285">SQL Virtual Machine</span></span>
* <span data-ttu-id="69b8c-2286">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="69b8c-2286">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-2287">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-2287">Storage</span></span>
* <span data-ttu-id="69b8c-2288">Alteração na correção para atualizar apenas as propriedades que são alteradas no mesmo objeto</span><span class="sxs-lookup"><span data-stu-id="69b8c-2288">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="69b8c-2289">#8021 foi corrigido, dados binários são codificados em base 64 quando retornados</span><span class="sxs-lookup"><span data-stu-id="69b8c-2289">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="69b8c-2290">VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-2290">VM</span></span>
* <span data-ttu-id="69b8c-2291">Alteração de `vm encryption enable` para validar o cofre de chaves de criptografia de disco e se esse cofre de chaves de criptografia de chave existe</span><span class="sxs-lookup"><span data-stu-id="69b8c-2291">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="69b8c-2292">O sinalizador `--force` foi adicionado a `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2292">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="69b8c-2293">15 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="69b8c-2293">January 15, 2019</span></span>

<span data-ttu-id="69b8c-2294">Versão 2.0.55</span><span class="sxs-lookup"><span data-stu-id="69b8c-2294">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-2295">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-2295">ACR</span></span>
* <span data-ttu-id="69b8c-2296">Alteração para permitir forçar o envio por push de um gráfico Helm que não existe</span><span class="sxs-lookup"><span data-stu-id="69b8c-2296">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="69b8c-2297">Alteração para permitir operações de runtime sem solicitações ARM</span><span class="sxs-lookup"><span data-stu-id="69b8c-2297">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="69b8c-2298">[PRETERIDO] O parâmetro `--resource-group` foi preterido nos comandos:</span><span class="sxs-lookup"><span data-stu-id="69b8c-2298">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="69b8c-2299">ACS</span><span class="sxs-lookup"><span data-stu-id="69b8c-2299">ACS</span></span>
* <span data-ttu-id="69b8c-2300">Suporte adicionado para novas regiões ACI</span><span class="sxs-lookup"><span data-stu-id="69b8c-2300">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-2301">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-2301">Appservice</span></span>
* <span data-ttu-id="69b8c-2302">Foi corrigido o problema com o carregamento de certificados para aplicativos que são hospedados em um ASE, em que o RG do ASE e o RG do aplicativo são diferentes</span><span class="sxs-lookup"><span data-stu-id="69b8c-2302">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="69b8c-2303">Alteração de `webapp up` para usar a SKU P1V1 como padrão para Linux</span><span class="sxs-lookup"><span data-stu-id="69b8c-2303">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="69b8c-2304">`[webapp|functionapp] deployment source config-zip` foi corrigido para mostrar a mensagem de erro adequada quando uma implantação falhar</span><span class="sxs-lookup"><span data-stu-id="69b8c-2304">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="69b8c-2305">Adicionado o comando `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2305">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="69b8c-2306">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="69b8c-2306">Botservice</span></span>
* <span data-ttu-id="69b8c-2307">Atualizações de status de implantação foram adicionadas a `bot create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2307">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="69b8c-2308">Configurar</span><span class="sxs-lookup"><span data-stu-id="69b8c-2308">Configure</span></span>
* <span data-ttu-id="69b8c-2309">`none` foi adicionado como um formato de saída configurável</span><span class="sxs-lookup"><span data-stu-id="69b8c-2309">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="69b8c-2310">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="69b8c-2310">CosmosDB</span></span>
* <span data-ttu-id="69b8c-2311">Suporte adicionado para criar o banco de dados com taxa de transferência compartilhada</span><span class="sxs-lookup"><span data-stu-id="69b8c-2311">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="69b8c-2312">HDInsight</span><span class="sxs-lookup"><span data-stu-id="69b8c-2312">HDInsight</span></span>
* <span data-ttu-id="69b8c-2313">Foram adicionados comandos para o gerenciamento de aplicativos</span><span class="sxs-lookup"><span data-stu-id="69b8c-2313">Added commands for managing applications</span></span>
* <span data-ttu-id="69b8c-2314">Foram adicionados comandos para o gerenciamento de ações de script</span><span class="sxs-lookup"><span data-stu-id="69b8c-2314">Added commands for managing script actions</span></span>
* <span data-ttu-id="69b8c-2315">Foram adicionados comandos para o gerenciamento do Operations Management Suite (OMS)</span><span class="sxs-lookup"><span data-stu-id="69b8c-2315">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="69b8c-2316">Suporte adicionado para listar a utilização regional ao `hdinsight list-usage`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2316">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="69b8c-2317">[ALTERAÇÃO SIGNIFICATIVA] O tipo de cluster padrão de `hdinsight create` foi removido</span><span class="sxs-lookup"><span data-stu-id="69b8c-2317">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-2318">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-2318">Network</span></span>
* <span data-ttu-id="69b8c-2319">Adicionados os argumentos `--custom-headers` e `--status-code-ranges` para `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2319">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="69b8c-2320">Novos tipos de roteamento foram adicionados: Subrede e múltiplos valores</span><span class="sxs-lookup"><span data-stu-id="69b8c-2320">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="69b8c-2321">Adicionados os argumentos `--custom-headers` e `--subnets` para `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2321">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="69b8c-2322">Foi corrigido o problema no qual fornecer `--vnets ""` a `ddos-protection update` causava um erro</span><span class="sxs-lookup"><span data-stu-id="69b8c-2322">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="69b8c-2323">Função</span><span class="sxs-lookup"><span data-stu-id="69b8c-2323">Role</span></span>
* <span data-ttu-id="69b8c-2324">[PRETERIDO] O argumento `--password` foi preterido para `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="69b8c-2324">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="69b8c-2325">Como alternativa, use senhas seguras geradas pela CLI</span><span class="sxs-lookup"><span data-stu-id="69b8c-2325">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="69b8c-2326">Segurança</span><span class="sxs-lookup"><span data-stu-id="69b8c-2326">Security</span></span>
* <span data-ttu-id="69b8c-2327">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="69b8c-2327">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-2328">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-2328">Storage</span></span>
* <span data-ttu-id="69b8c-2329">[ALTERAÇÃO SIGNIFICATIVA] O número padrão de resultados de `storage [blob|file|container|share] list` foi alterado para 5.000.</span><span class="sxs-lookup"><span data-stu-id="69b8c-2329">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="69b8c-2330">Use `--num-results *` para o comportamento original de retornar todos os resultados</span><span class="sxs-lookup"><span data-stu-id="69b8c-2330">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="69b8c-2331">Parâmetro `--marker` adicionado a `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2331">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="69b8c-2332">Um marcador de log foi adicionado para a próxima página ao STDERR de `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2332">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="69b8c-2333">O comando `storage blob service-properties update` foi adicionado com suporte para sites estáticos</span><span class="sxs-lookup"><span data-stu-id="69b8c-2333">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="69b8c-2334">VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-2334">VM</span></span>
* <span data-ttu-id="69b8c-2335">`vm [disk|unmanaged-disk]` e `vmss disk` foram alterados para que tenham parâmetros mais consistentes</span><span class="sxs-lookup"><span data-stu-id="69b8c-2335">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="69b8c-2336">Suporte adicionado para referência cruzada de imagem de locatário a `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2336">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="69b8c-2337">O bug de configuração padrão foi corrigido em `vm diagnostics get-default-config --windows-os`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2337">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="69b8c-2338">O argumento `--provision-after-extensions` foi adicionado a `vmss extension set` para definir quais extensões deverão ser provisionadas antes da extensão ser definida</span><span class="sxs-lookup"><span data-stu-id="69b8c-2338">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="69b8c-2339">O argumento `--replica-count` foi adicionado a `sig image-version update` para definir a contagem de replicação padrão</span><span class="sxs-lookup"><span data-stu-id="69b8c-2339">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="69b8c-2340">Foi corrigido o bug com `image create --source` em que o disco do sistema operacional de origem era confundido com uma VM do mesmo nome, mesmo se a ID de recurso completa fosse fornecida</span><span class="sxs-lookup"><span data-stu-id="69b8c-2340">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="69b8c-2341">20 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="69b8c-2341">December 20, 2018</span></span>

<span data-ttu-id="69b8c-2342">Versão 2.0.54</span><span class="sxs-lookup"><span data-stu-id="69b8c-2342">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="69b8c-2343">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-2343">Appservice</span></span>
* <span data-ttu-id="69b8c-2344">Corrigido o problema que causava falha na reimplantação do `webapp up`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2344">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="69b8c-2345">Adicionado suporte para listar e restaurar instantâneos de aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="69b8c-2345">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="69b8c-2346">Adicionado suporte para o sinalizador `--runtime` para aplicativos de funções do Windows</span><span class="sxs-lookup"><span data-stu-id="69b8c-2346">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="69b8c-2347">IoT Central</span><span class="sxs-lookup"><span data-stu-id="69b8c-2347">IoTCentral</span></span>
* <span data-ttu-id="69b8c-2348">Corrigida a chamada à API do comando de atualização</span><span class="sxs-lookup"><span data-stu-id="69b8c-2348">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="69b8c-2349">Função</span><span class="sxs-lookup"><span data-stu-id="69b8c-2349">Role</span></span>
* <span data-ttu-id="69b8c-2350">[ALTERAÇÃO SIGNIFICATIVA]`ad [app|sp] list` alterado para listar somente os 100 primeiros objetos por padrão</span><span class="sxs-lookup"><span data-stu-id="69b8c-2350">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="69b8c-2351">SQL</span><span class="sxs-lookup"><span data-stu-id="69b8c-2351">SQL</span></span>
* <span data-ttu-id="69b8c-2352">Adicionado suporte para ordenação personalizada nas instâncias gerenciadas</span><span class="sxs-lookup"><span data-stu-id="69b8c-2352">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="69b8c-2353">VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-2353">VM</span></span>
* <span data-ttu-id="69b8c-2354">Parâmetro `---os-type` adicionado a `disk create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2354">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="69b8c-2355">18 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="69b8c-2355">December 18, 2018</span></span>

<span data-ttu-id="69b8c-2356">Versão 2.0.53</span><span class="sxs-lookup"><span data-stu-id="69b8c-2356">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="69b8c-2357">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-2357">ACR</span></span>
* <span data-ttu-id="69b8c-2358">Adicionado suporte para importação de imagem de Registros de Contêiner externos</span><span class="sxs-lookup"><span data-stu-id="69b8c-2358">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="69b8c-2359">Simplificado o layout da tabela para a lista de tarefas</span><span class="sxs-lookup"><span data-stu-id="69b8c-2359">Condensed the table layout for task list</span></span>
* <span data-ttu-id="69b8c-2360">Adicionado suporte para URLs do Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="69b8c-2360">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="69b8c-2361">ACS</span><span class="sxs-lookup"><span data-stu-id="69b8c-2361">ACS</span></span>
* <span data-ttu-id="69b8c-2362">Adicionada visualização dos nós virtuais</span><span class="sxs-lookup"><span data-stu-id="69b8c-2362">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="69b8c-2363">Removido “(VISUALIZAÇÃO)” de argumentos do AAD para `aks create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2363">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="69b8c-2364">[PRETERIDO] Comandos `az acs` preteridos.</span><span class="sxs-lookup"><span data-stu-id="69b8c-2364">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="69b8c-2365">O serviço ACS será desativado em 31 de janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="69b8c-2365">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="69b8c-2366">Adicionado suporte da Política de Rede durante a criação de novos clusters AKS</span><span class="sxs-lookup"><span data-stu-id="69b8c-2366">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="69b8c-2367">Removido o requisito do argumento `--nodepool-name` para `aks scale` se houver apenas um pool de nós</span><span class="sxs-lookup"><span data-stu-id="69b8c-2367">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-2368">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-2368">Appservice</span></span>
* <span data-ttu-id="69b8c-2369">Corrigido o problema em que `webapp config container` não honra o parâmetro `--slot`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2369">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="69b8c-2370">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="69b8c-2370">Botservice</span></span>
* <span data-ttu-id="69b8c-2371">Suporte adicionado para análise do arquivo `.bot` ao chamar `bot show`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2371">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="69b8c-2372">Corrigido o bug de provisionamento do AppInsights</span><span class="sxs-lookup"><span data-stu-id="69b8c-2372">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="69b8c-2373">Corrigido o bug de espaço em branco ao lidar com caminhos de arquivo</span><span class="sxs-lookup"><span data-stu-id="69b8c-2373">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="69b8c-2374">Reduzidas as chamadas de rede do Kudu</span><span class="sxs-lookup"><span data-stu-id="69b8c-2374">Reduced Kudu network calls</span></span>
* <span data-ttu-id="69b8c-2375">Melhorias de UX para comandos gerais</span><span class="sxs-lookup"><span data-stu-id="69b8c-2375">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="69b8c-2376">Consumo</span><span class="sxs-lookup"><span data-stu-id="69b8c-2376">Consumption</span></span>
* <span data-ttu-id="69b8c-2377">Corrigidos os bugs da API de orçamento ao mostrar notificações</span><span class="sxs-lookup"><span data-stu-id="69b8c-2377">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="69b8c-2378">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="69b8c-2378">CosmosDB</span></span>
* <span data-ttu-id="69b8c-2379">Suporte adicionado para atualizar a conta de vários mestres para mestre único</span><span class="sxs-lookup"><span data-stu-id="69b8c-2379">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="69b8c-2380">Mapas</span><span class="sxs-lookup"><span data-stu-id="69b8c-2380">Maps</span></span>
* <span data-ttu-id="69b8c-2381">Adicionado suporte ao SKU S1 para `maps account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2381">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-2382">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-2382">Network</span></span>
* <span data-ttu-id="69b8c-2383">Adicionado suporte para `--format` e `--log-version` para `watcher flow-log configure`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2383">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="69b8c-2384">Corrigido o problema com `dns zone update` em que usar "" para limpar a resolução e o registro de redes virtuais não funcionava</span><span class="sxs-lookup"><span data-stu-id="69b8c-2384">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="69b8c-2385">Recurso</span><span class="sxs-lookup"><span data-stu-id="69b8c-2385">Resource</span></span>
* <span data-ttu-id="69b8c-2386">Corrigido o tratamento do parâmetro de escopo para grupos de gerenciamento do `policy assignment [create|list|delete|show|update]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2386">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="69b8c-2387">Adicionado o novo comando `resource wait`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2387">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-2388">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-2388">Storage</span></span>
*  <span data-ttu-id="69b8c-2389">Adicionada a capacidade de atualizar a versão do esquema de log para serviços de armazenamento no `storage logging update`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2389">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="69b8c-2390">VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-2390">VM</span></span>
* <span data-ttu-id="69b8c-2391">Corrigida a falha em `vm identity remove` quando a VM especificada não tem nenhuma identidade de serviço gerenciado atribuída</span><span class="sxs-lookup"><span data-stu-id="69b8c-2391">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="69b8c-2392">4 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="69b8c-2392">December 4, 2018</span></span>

<span data-ttu-id="69b8c-2393">Versão 2.0.52</span><span class="sxs-lookup"><span data-stu-id="69b8c-2393">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="69b8c-2394">Núcleo</span><span class="sxs-lookup"><span data-stu-id="69b8c-2394">Core</span></span>
* <span data-ttu-id="69b8c-2395">Adicionado suporte para provisionamento de recursos de locatários cruzados para a entidade de serviço de multilocatários</span><span class="sxs-lookup"><span data-stu-id="69b8c-2395">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="69b8c-2396">Corrigido o bug onde as ids enviadas por pipe de um comando com a saída tsv eram analisados incorretamente</span><span class="sxs-lookup"><span data-stu-id="69b8c-2396">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-2397">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-2397">Appservice</span></span>
* <span data-ttu-id="69b8c-2398">[VERSÃO PRÉVIA] Adicionado o comando `webapp up` que ajuda a criar e implantar conteúdo em aplicativo</span><span class="sxs-lookup"><span data-stu-id="69b8c-2398">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="69b8c-2399">Corrigido um bug no aplicativo com base em contêiner do Windows devido à alteração de back-end</span><span class="sxs-lookup"><span data-stu-id="69b8c-2399">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-2400">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-2400">Network</span></span>
* <span data-ttu-id="69b8c-2401">Adicionado o argumento `--exclusion` a `application-gateway waf-config set` para dar suporte a exclusões de WAF</span><span class="sxs-lookup"><span data-stu-id="69b8c-2401">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="69b8c-2402">Função</span><span class="sxs-lookup"><span data-stu-id="69b8c-2402">Role</span></span>
* <span data-ttu-id="69b8c-2403">Adicionado suporte para identificadores personalizados para a credencial de senha</span><span class="sxs-lookup"><span data-stu-id="69b8c-2403">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="69b8c-2404">VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-2404">VM</span></span>
* <span data-ttu-id="69b8c-2405">[PRETERIDO] Parâmetro `vm extension [show|wait] --expand` preterido</span><span class="sxs-lookup"><span data-stu-id="69b8c-2405">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="69b8c-2406">Adicionado parâmetro `--force` a `vm restart` para reimplantar as VMs sem resposta</span><span class="sxs-lookup"><span data-stu-id="69b8c-2406">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="69b8c-2407">Alterado `[vm|vmss] create --authentication-type` para aceitar "todos" para criar uma VM com senha e autenticação SSH</span><span class="sxs-lookup"><span data-stu-id="69b8c-2407">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="69b8c-2408">Adicionado parâmetro `image create --os-disk-caching` para definir o cache de disco do sistema operacional para uma imagem</span><span class="sxs-lookup"><span data-stu-id="69b8c-2408">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="69b8c-2409">20 de novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="69b8c-2409">November 20, 2018</span></span>

<span data-ttu-id="69b8c-2410">Versão 2.0.51</span><span class="sxs-lookup"><span data-stu-id="69b8c-2410">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="69b8c-2411">Núcleo</span><span class="sxs-lookup"><span data-stu-id="69b8c-2411">Core</span></span>
* <span data-ttu-id="69b8c-2412">Logon do MSI alterado para não reutilizar o nome da assinatura na identidade</span><span class="sxs-lookup"><span data-stu-id="69b8c-2412">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-2413">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-2413">ACR</span></span>
* <span data-ttu-id="69b8c-2414">Token de contexto adicionado à etapa da tarefa</span><span class="sxs-lookup"><span data-stu-id="69b8c-2414">Added context token to task step</span></span>
* <span data-ttu-id="69b8c-2415">Suporte adicionado para definir segredos na execução do acr para espelhar a tarefa do acr</span><span class="sxs-lookup"><span data-stu-id="69b8c-2415">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="69b8c-2416">Suporte aprimorado para `--top` e `--orderby` para os comandos `show-tags` e `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2416">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-2417">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-2417">Appservice</span></span>
* <span data-ttu-id="69b8c-2418">Tempo limite padrão para a implantação do zip alterado para sondar o status aumentado para 5 minutos, também adicionando uma propriedade de tempo limite para personalizar esse valor</span><span class="sxs-lookup"><span data-stu-id="69b8c-2418">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="69b8c-2419">Padrão `node_version` atualizado.</span><span class="sxs-lookup"><span data-stu-id="69b8c-2419">Updated the default `node_version`.</span></span> <span data-ttu-id="69b8c-2420">Redefinir a ação de troca de slots durante uma troca de duas fases preserva todas as configurações do aplicativo e cadeias de conexão</span><span class="sxs-lookup"><span data-stu-id="69b8c-2420">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="69b8c-2421">Verificação da SKU no lado do cliente removida para o Linux criar o plano do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="69b8c-2421">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="69b8c-2422">Erro corrigido ao tentar obter o status de implantação do zip</span><span class="sxs-lookup"><span data-stu-id="69b8c-2422">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="69b8c-2423">Iot Central</span><span class="sxs-lookup"><span data-stu-id="69b8c-2423">IotCentral</span></span>
* <span data-ttu-id="69b8c-2424">Verificação de disponibilidade do subdomínio adicionada ao criar um aplicativo do IoT Central</span><span class="sxs-lookup"><span data-stu-id="69b8c-2424">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="69b8c-2425">KeyVault</span><span class="sxs-lookup"><span data-stu-id="69b8c-2425">KeyVault</span></span>
* <span data-ttu-id="69b8c-2426">Bug corrigido em que os erros podem ter sido ignorados</span><span class="sxs-lookup"><span data-stu-id="69b8c-2426">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-2427">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-2427">Network</span></span>
* <span data-ttu-id="69b8c-2428">Subcomandos `root-cert` adicionados a `application-gateway` para lidar com os certificados de raiz confiável</span><span class="sxs-lookup"><span data-stu-id="69b8c-2428">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="69b8c-2429">Opções `--min-capacity` e `--custom-error-pages` adicionadas a `application-gateway [create|update]`:</span><span class="sxs-lookup"><span data-stu-id="69b8c-2429">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="69b8c-2430">`--zones` adicionado para suporte da zona de disponibilidade a `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2430">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="69b8c-2431">Argumentos `--file-upload-limit`, `--max-request-body-size` e `--request-body-check` a `application-gateway waf-config set` adicionados</span><span class="sxs-lookup"><span data-stu-id="69b8c-2431">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="69b8c-2432">Rdbms</span><span class="sxs-lookup"><span data-stu-id="69b8c-2432">Rdbms</span></span>
* <span data-ttu-id="69b8c-2433">Comandos vnet do mariadb adicionados</span><span class="sxs-lookup"><span data-stu-id="69b8c-2433">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="69b8c-2434">Rbac</span><span class="sxs-lookup"><span data-stu-id="69b8c-2434">Rbac</span></span>
* <span data-ttu-id="69b8c-2435">Um problema corrigido ao tentar atualizar credenciais inalteradas em `ad app update`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2435">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="69b8c-2436">Avisos de saída adicionados para comunicar alterações de falha em um futuro próximo para `ad [app|sp] list`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2436">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="69b8c-2437">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-2437">Storage</span></span>
* <span data-ttu-id="69b8c-2438">Melhor manipulação de casos incomuns para os comandos da cópia de armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-2438">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="69b8c-2439">Corrigido o problema em que `storage blob copy start-batch` não usava credenciais de logon quando as contas de origem e destino eram iguais</span><span class="sxs-lookup"><span data-stu-id="69b8c-2439">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="69b8c-2440">Bug corrigido com `storage [blob|file] url` em que `sas_token` não foi incorporado na URL</span><span class="sxs-lookup"><span data-stu-id="69b8c-2440">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="69b8c-2441">Aviso de alteração da falha adicionado a `[blob|container] list`: produzirá apenas os primeiros 5.000 resultados por padrão</span><span class="sxs-lookup"><span data-stu-id="69b8c-2441">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="69b8c-2442">VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-2442">VM</span></span>
* <span data-ttu-id="69b8c-2443">Suporte adicionado a `[vm|vmss] create --storage-sku` para especificar a SKU da conta de armazenamento para o SO gerenciado e os discos de dados separadamente</span><span class="sxs-lookup"><span data-stu-id="69b8c-2443">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="69b8c-2444">Parâmetros do nome da versão alterados de `sig image-version` para `--image-version -e`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2444">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="69b8c-2445">Argumento `sig image-version` preterido `--image-version-name`, substituído por `--image-version`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2445">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="69b8c-2446">Suporte adicionado para usar o disco local do SO a `[vm|vmss] create --ephemeral-os-disk`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2446">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="69b8c-2447">Adicionado o suporte ao `--no-wait` para `snapshot create/update`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2447">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="69b8c-2448">Adicionado o comando `snapshot wait`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2448">Added `snapshot wait` command</span></span>
* <span data-ttu-id="69b8c-2449">Suporte adicionado para usar o nome da instância com `[vm|vmss] extension set --extension-instance-name`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2449">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="69b8c-2450">6 de novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="69b8c-2450">November 6, 2018</span></span>

<span data-ttu-id="69b8c-2451">Versão 2.0.50</span><span class="sxs-lookup"><span data-stu-id="69b8c-2451">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="69b8c-2452">Núcleo</span><span class="sxs-lookup"><span data-stu-id="69b8c-2452">Core</span></span>
* <span data-ttu-id="69b8c-2453">Foi adicionado suporte para o serviço principal sn + autenticação do emissor</span><span class="sxs-lookup"><span data-stu-id="69b8c-2453">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-2454">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-2454">ACR</span></span>
* <span data-ttu-id="69b8c-2455">Foi adicionado suporte para eventos de git de solicitação de pull e de confirmação para o gatilho de origem da tarefa</span><span class="sxs-lookup"><span data-stu-id="69b8c-2455">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="69b8c-2456">Alterado para usar o padrão do Dockerfile se ele não for especificado no comando de compilação</span><span class="sxs-lookup"><span data-stu-id="69b8c-2456">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="69b8c-2457">ACS</span><span class="sxs-lookup"><span data-stu-id="69b8c-2457">ACS</span></span>
* <span data-ttu-id="69b8c-2458">[ALTERAÇÃO SIGNIFICATIVA]`enable_cloud_console_aks_browse` foi removido para habilitar 'az aks browse' por padrão</span><span class="sxs-lookup"><span data-stu-id="69b8c-2458">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="69b8c-2459">Supervisor</span><span class="sxs-lookup"><span data-stu-id="69b8c-2459">Advisor</span></span>
* <span data-ttu-id="69b8c-2460">Versão de GA</span><span class="sxs-lookup"><span data-stu-id="69b8c-2460">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="69b8c-2461">AMS</span><span class="sxs-lookup"><span data-stu-id="69b8c-2461">AMS</span></span>
* <span data-ttu-id="69b8c-2462">Novos grupos de comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="69b8c-2462">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="69b8c-2463">Novos comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="69b8c-2463">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="69b8c-2464">Adicionados parâmetros de criptografia com suporte para `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2464">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="69b8c-2465">O suporte adicionado para `ams transform output remove` agora pode ser executado passando o índice de saída a ser removido</span><span class="sxs-lookup"><span data-stu-id="69b8c-2465">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="69b8c-2466">Adicionados os argumentos `--correlation-data` e `--label` ao grupo de comandos `ams job`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2466">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="69b8c-2467">Adicionados os argumentos `--storage-account` e `--container` ao grupo de comandos `ams asset`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2467">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="69b8c-2468">Foram adicionados valores padrões para o horário de expiração (agora +23h) e permissões (Leitura) no comando `ams asset get-sas-url`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2468">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="69b8c-2469">[ALTERAÇÃO SIGNIFICATIVA] O comando `ams streaming locator` foi substituído por `ams streaming-locator`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2469">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="69b8c-2470">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--content-keys` de `ams streaming locator` foi atualizado</span><span class="sxs-lookup"><span data-stu-id="69b8c-2470">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="69b8c-2471">[ALTERAÇÃO SIGNIFICATIVA]`--content-policy-name` foi renomeado como `--content-key-policy-name` no comando `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2471">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="69b8c-2472">[ALTERAÇÃO SIGNIFICATIVA] O comando `ams streaming policy` foi substituído por `ams streaming-policy`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2472">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="69b8c-2473">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--preset-names` foi substituído por `--preset` no grupo de comandos `ams transform`.</span><span class="sxs-lookup"><span data-stu-id="69b8c-2473">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="69b8c-2474">Agora, você só pode definir uma saída/predefinição de cada vez (para adicionar mais, é preciso executar `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="69b8c-2474">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="69b8c-2475">Além disso, você pode definir StandardEncoderPreset personalizado passando o caminho para seu JSON personalizado</span><span class="sxs-lookup"><span data-stu-id="69b8c-2475">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="69b8c-2476">[ALTERAÇÃO SIGNIFICATIVA]`--output-asset-names ` foi renomeado como `--output-assets` no comando `ams job start`.</span><span class="sxs-lookup"><span data-stu-id="69b8c-2476">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="69b8c-2477">Agora, ele aceita uma lista separada por espaços dos ativos no formato 'assetName=label'.</span><span class="sxs-lookup"><span data-stu-id="69b8c-2477">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="69b8c-2478">Um ativo sem rótulo pode ser enviado assim: 'assetName='</span><span class="sxs-lookup"><span data-stu-id="69b8c-2478">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-2479">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-2479">AppService</span></span>
* <span data-ttu-id="69b8c-2480">Um bug no `az webapp config backup update` que impede a configuração de um agendamento de backup foi corrigido, caso ele ainda não tenha sido definido</span><span class="sxs-lookup"><span data-stu-id="69b8c-2480">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="69b8c-2481">Configurar</span><span class="sxs-lookup"><span data-stu-id="69b8c-2481">Configure</span></span>
* <span data-ttu-id="69b8c-2482">O YAML foi adicionado às opções de formato de saída</span><span class="sxs-lookup"><span data-stu-id="69b8c-2482">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="69b8c-2483">Contêiner</span><span class="sxs-lookup"><span data-stu-id="69b8c-2483">Container</span></span>
* <span data-ttu-id="69b8c-2484">Alterado para mostrar a identidade ao exportar um grupo de contêineres para yaml</span><span class="sxs-lookup"><span data-stu-id="69b8c-2484">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="69b8c-2485">EventHub</span><span class="sxs-lookup"><span data-stu-id="69b8c-2485">EventHub</span></span>
* <span data-ttu-id="69b8c-2486">O sinalizador `--enable-kafka` foi adicionado para dar suporte ao Kafka no `eventhub namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2486">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="69b8c-2487">Interativo</span><span class="sxs-lookup"><span data-stu-id="69b8c-2487">Interactive</span></span>
* <span data-ttu-id="69b8c-2488">O interativo agora instala a extensão `interactive` que permite atualizações e suporte mais rápidos</span><span class="sxs-lookup"><span data-stu-id="69b8c-2488">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="69b8c-2489">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="69b8c-2489">Monitor</span></span>
* <span data-ttu-id="69b8c-2490">Foi adicionado suporte para nomes de métricas, que incluem os caracteres barra (/) e ponto (.) para `--condition` em `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2490">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-2491">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-2491">Network</span></span>
* <span data-ttu-id="69b8c-2492">Os nomes de comandos `network interface-endpoint` foram preteridos em benefício de `network private-endpoint`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2492">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="69b8c-2493">Foi corrigido um problema onde um argumento `--peer-circuit` em `express-route peering connection create` não aceitaria uma ID</span><span class="sxs-lookup"><span data-stu-id="69b8c-2493">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="69b8c-2494">Foi corrigido um problema onde `--ip-tags` não funcionava corretamente com `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2494">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="69b8c-2495">Perfil</span><span class="sxs-lookup"><span data-stu-id="69b8c-2495">Profile</span></span>
* <span data-ttu-id="69b8c-2496">`--use-cert-sn-issuer` foi adicionado a `az login` para logon da entidade de serviço com rolagens automáticas de certificado</span><span class="sxs-lookup"><span data-stu-id="69b8c-2496">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="69b8c-2497">RDBMS</span><span class="sxs-lookup"><span data-stu-id="69b8c-2497">RDBMS</span></span>
* <span data-ttu-id="69b8c-2498">Adicionados comandos da réplica mysql</span><span class="sxs-lookup"><span data-stu-id="69b8c-2498">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="69b8c-2499">Recurso</span><span class="sxs-lookup"><span data-stu-id="69b8c-2499">Resource</span></span>
* <span data-ttu-id="69b8c-2500">Adicionado suporte para grupos de gerenciamento e assinaturas aos comandos `policy definition|set-definition`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2500">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="69b8c-2501">Função</span><span class="sxs-lookup"><span data-stu-id="69b8c-2501">Role</span></span>
* <span data-ttu-id="69b8c-2502">Adicionado suporte para gerenciamento de permissões de API, usuário conectado e gerenciamento de senhas dos aplicativos e certificados de credenciais</span><span class="sxs-lookup"><span data-stu-id="69b8c-2502">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="69b8c-2503">`ad sp create-for-rbac` foi alterado para esclarecer a confusão entre o displayName e o nome da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="69b8c-2503">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="69b8c-2504">Suporte adicionado para conceder permissões a aplicativos do AAD</span><span class="sxs-lookup"><span data-stu-id="69b8c-2504">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-2505">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-2505">Storage</span></span>
* <span data-ttu-id="69b8c-2506">Suporte adicionado para se conectar aos serviços de armazenamento somente com SAS e pontos de extremidade (sem um nome de conta ou uma chave), conforme descrito em `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2506">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="69b8c-2507">VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-2507">VM</span></span>
* <span data-ttu-id="69b8c-2508">O argumento `storage-sku` foi adicionado a `image create` para definir o tipo de conta de armazenamento padrão da imagem</span><span class="sxs-lookup"><span data-stu-id="69b8c-2508">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="69b8c-2509">O bug com `vm resize` onde a opção `--no-wait` faz com que o comando falhasse foi corrigido</span><span class="sxs-lookup"><span data-stu-id="69b8c-2509">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="69b8c-2510">O formato de saída da tabela `vm encryption show` para mostrar o status foi alterado</span><span class="sxs-lookup"><span data-stu-id="69b8c-2510">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="69b8c-2511">`vm secret format` foi alterado para exigir a saída json/jsonc.</span><span class="sxs-lookup"><span data-stu-id="69b8c-2511">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="69b8c-2512">Avisa o usuário e assume como padrão a saída json se um formato de saída indesejado for escolhido</span><span class="sxs-lookup"><span data-stu-id="69b8c-2512">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="69b8c-2513">Validação de argumento aprimorado para `vm create --image`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2513">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="69b8c-2514">23 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="69b8c-2514">October 23, 2018</span></span>

<span data-ttu-id="69b8c-2515">Versão 2.0.49</span><span class="sxs-lookup"><span data-stu-id="69b8c-2515">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="69b8c-2516">Núcleo</span><span class="sxs-lookup"><span data-stu-id="69b8c-2516">Core</span></span>
* <span data-ttu-id="69b8c-2517">Corrigido o problema com `--ids` onde `--subscription` teria precedência sobre a assinatura em `--ids`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2517">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="69b8c-2518">Adicionados avisos explícitos quando parâmetros seriam ignorados pelo uso de `--ids`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2518">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-2519">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-2519">ACR</span></span>
* <span data-ttu-id="69b8c-2520">Corrigido um problema de codificação de ACR Build no Python2</span><span class="sxs-lookup"><span data-stu-id="69b8c-2520">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="69b8c-2521">CDN</span><span class="sxs-lookup"><span data-stu-id="69b8c-2521">CDN</span></span>
* <span data-ttu-id="69b8c-2522">[ALTERAÇÃO SIGNIFICATIVA] Alterado o comportamento de armazenamento em cache da cadeia de caracteres de consulta padrão de `cdn endpoint create` para não assumir o padrão "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="69b8c-2522">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="69b8c-2523">Agora, ele é definido pelo serviço</span><span class="sxs-lookup"><span data-stu-id="69b8c-2523">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="69b8c-2524">Contêiner</span><span class="sxs-lookup"><span data-stu-id="69b8c-2524">Container</span></span>
* <span data-ttu-id="69b8c-2525">Adicionado `Private` como um tipo válido para passar para '--ip-address'</span><span class="sxs-lookup"><span data-stu-id="69b8c-2525">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="69b8c-2526">Alterado para permitir o uso somente de ID de sub-rede para configurar uma rede virtual para o grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="69b8c-2526">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="69b8c-2527">Alterado para permitir o uso de nome de rede virtual ou ID de recurso para habilitar o uso de redes virtuais de diferentes grupos de recursos</span><span class="sxs-lookup"><span data-stu-id="69b8c-2527">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="69b8c-2528">Adicionado `--assign-identity` para adicionar uma identidade MSI a um grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="69b8c-2528">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="69b8c-2529">Adicionado `--scope` para criar uma atribuição de função para a identidade MSI atribuída pelo sistema</span><span class="sxs-lookup"><span data-stu-id="69b8c-2529">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="69b8c-2530">Adicionado um aviso ao criar um grupo de contêineres com uma imagem sem um processo de execução longa</span><span class="sxs-lookup"><span data-stu-id="69b8c-2530">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="69b8c-2531">Corrigidos os problemas de saída da tabela para comandos `list` e `show`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2531">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="69b8c-2532">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="69b8c-2532">CosmosDB</span></span>
* <span data-ttu-id="69b8c-2533">Adicionado o suporte `--enable-multiple-write-locations` para `cosmosdb create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2533">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="69b8c-2534">Interativo</span><span class="sxs-lookup"><span data-stu-id="69b8c-2534">Interactive</span></span>
* <span data-ttu-id="69b8c-2535">Alterado para garantir que o parâmetro de assinatura global seja exibido nos parâmetros</span><span class="sxs-lookup"><span data-stu-id="69b8c-2535">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="69b8c-2536">Central da IoT</span><span class="sxs-lookup"><span data-stu-id="69b8c-2536">IoT Central</span></span>
* <span data-ttu-id="69b8c-2537">Adicionadas opções de nome de exibição e modelo para criação de aplicativos de IoT Central</span><span class="sxs-lookup"><span data-stu-id="69b8c-2537">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="69b8c-2538">[ALTERAÇÃO SIGNIFICATIVA] Removido o suporte para a SKU F1; Use a SKU S1</span><span class="sxs-lookup"><span data-stu-id="69b8c-2538">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="69b8c-2539">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="69b8c-2539">Monitor</span></span>
* <span data-ttu-id="69b8c-2540">Alterações para `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="69b8c-2540">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="69b8c-2541">Adicionado suporte para listar todos os eventos no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="69b8c-2541">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="69b8c-2542">Adicionado o parâmetro `--offset` para criar consultas de tempo mais facilmente</span><span class="sxs-lookup"><span data-stu-id="69b8c-2542">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="69b8c-2543">Melhorada a validação para `--start-time` e `--end-time` para usar um intervalo mais amplo de formatos ISO8601 e formatos de data/hora mais amigáveis ao usuário</span><span class="sxs-lookup"><span data-stu-id="69b8c-2543">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="69b8c-2544">Adicionado `--namespace` como alias para a opção preterida `--resource-provider`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2544">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="69b8c-2545">Preterido `--filters` porque não há valores diferentes daqueles com opções fortemente tipadas compatíveis com o serviço</span><span class="sxs-lookup"><span data-stu-id="69b8c-2545">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="69b8c-2546">Alterações para `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="69b8c-2546">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="69b8c-2547">Adicionado o parâmetro `--offset` para criar consultas de tempo mais facilmente</span><span class="sxs-lookup"><span data-stu-id="69b8c-2547">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="69b8c-2548">Melhorada a validação para `--start-time` e `--end-time` para usar um intervalo mais amplo de formatos ISO8601 e formatos de data/hora mais amigáveis ao usuário</span><span class="sxs-lookup"><span data-stu-id="69b8c-2548">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="69b8c-2549">Melhorada a validação para os argumentos `--event-hub` e `--event-hub-rule` para `monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2549">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-2550">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-2550">Network</span></span>
* <span data-ttu-id="69b8c-2551">Adicionados os argumentos `--app-gateway-address-pools` e `--gateway-name` para `nic create`, para dar suporte à adição de pools de endereços de back-end do gateway de aplicativo a um NIC</span><span class="sxs-lookup"><span data-stu-id="69b8c-2551">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="69b8c-2552">Adicionados os argumentos `--app-gateway-address-pools` e `--gateway-name` para `nic ip-config create/update`, para dar suporte à adição de pools de endereços de back-end do gateway de aplicativo a um NIC</span><span class="sxs-lookup"><span data-stu-id="69b8c-2552">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="69b8c-2553">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="69b8c-2553">ServiceBus</span></span>
* <span data-ttu-id="69b8c-2554">Adicionado `migration_state` somente leitura para MigrationConfigProperties para mostrar o atual estado de migração de namespace Standard para Premium do Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="69b8c-2554">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="69b8c-2555">SQL</span><span class="sxs-lookup"><span data-stu-id="69b8c-2555">SQL</span></span>
* <span data-ttu-id="69b8c-2556">Corrigidos `sql failover-group create` e `sql failover-group update` para trabalhar com a política de failover Manual</span><span class="sxs-lookup"><span data-stu-id="69b8c-2556">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-2557">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-2557">Storage</span></span>
* <span data-ttu-id="69b8c-2558">Corrigida a formatação de saída `az storage cors list`, todos os itens mostram a chave correta de "Serviço"</span><span class="sxs-lookup"><span data-stu-id="69b8c-2558">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="69b8c-2559">Adicionado o parâmetro `--bypass-immutability-policy` para a exclusão de contêiner bloqueado pela política de imutabilidade</span><span class="sxs-lookup"><span data-stu-id="69b8c-2559">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="69b8c-2560">VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-2560">VM</span></span>
* <span data-ttu-id="69b8c-2561">Aplicado o modo `None` de armazenamento em cache de disco para as séries Lv/Lv2 de computadores no `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2561">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="69b8c-2562">Atualizada a lista de tamanhos com suporte compatíveis com a aceleração de rede para `vm create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2562">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="69b8c-2563">Adicionado argumentos fortemente tipados para configurações de iops e mbps de ultra ssd para `disk create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2563">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="69b8c-2564">16 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="69b8c-2564">October 16, 2018</span></span>

<span data-ttu-id="69b8c-2565">Versão 2.0.48</span><span class="sxs-lookup"><span data-stu-id="69b8c-2565">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="69b8c-2566">VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-2566">VM</span></span>
* <span data-ttu-id="69b8c-2567">Corrigido o problema do SDK que causava falha durante a instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="69b8c-2567">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="69b8c-2568">9 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="69b8c-2568">October 9, 2018</span></span>

<span data-ttu-id="69b8c-2569">Versão 2.0.47</span><span class="sxs-lookup"><span data-stu-id="69b8c-2569">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="69b8c-2570">Núcleo</span><span class="sxs-lookup"><span data-stu-id="69b8c-2570">Core</span></span>
* <span data-ttu-id="69b8c-2571">Melhoria do tratamento de erro para os erros de "Solicitação Incorreta"</span><span class="sxs-lookup"><span data-stu-id="69b8c-2571">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-2572">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-2572">ACR</span></span>
* <span data-ttu-id="69b8c-2573">Suporte adicionado para o formato de tabela semelhante como cliente do helm</span><span class="sxs-lookup"><span data-stu-id="69b8c-2573">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="69b8c-2574">ACS</span><span class="sxs-lookup"><span data-stu-id="69b8c-2574">ACS</span></span>
* <span data-ttu-id="69b8c-2575">`aks [create|scale] --nodepool-name` adicionado para configurar o nome nodepool, truncado com 12 caracteres, padrão – nodepool1</span><span class="sxs-lookup"><span data-stu-id="69b8c-2575">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="69b8c-2576">Corrigido para voltar para “scp” quando Parimiko falha</span><span class="sxs-lookup"><span data-stu-id="69b8c-2576">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="69b8c-2577">`aks create` alterado para não precisar mais de `--aad-tenant-id`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2577">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="69b8c-2578">Melhoria da mesclagem das credenciais do Kubernetes quando houver entradas duplicadas</span><span class="sxs-lookup"><span data-stu-id="69b8c-2578">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="69b8c-2579">Contêiner</span><span class="sxs-lookup"><span data-stu-id="69b8c-2579">Container</span></span>
* <span data-ttu-id="69b8c-2580">`functionapp create` alterado para dar suporte à criação de um tipo de plano de consumo do Linux com um runtime específico</span><span class="sxs-lookup"><span data-stu-id="69b8c-2580">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="69b8c-2581">[VERSÃO PRÉVIA] Suporte adicionado para hospedar aplicativos Web nos contêineres do Windows</span><span class="sxs-lookup"><span data-stu-id="69b8c-2581">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="69b8c-2582">Hub de evento</span><span class="sxs-lookup"><span data-stu-id="69b8c-2582">Event Hub</span></span>
* <span data-ttu-id="69b8c-2583">Corrigido o comando `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2583">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="69b8c-2584">[ALTERAÇÃO SIGNIFICATIVA]`list` comandos alterados para lidar com os erros de recurso(s) NotFound(404) do modo típico, em vez de mostrar uma lista vazia</span><span class="sxs-lookup"><span data-stu-id="69b8c-2584">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="69b8c-2585">Extensões</span><span class="sxs-lookup"><span data-stu-id="69b8c-2585">Extensions</span></span>
* <span data-ttu-id="69b8c-2586">Corrigido o problema ao tentar adicionar uma extensão já instalada</span><span class="sxs-lookup"><span data-stu-id="69b8c-2586">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="69b8c-2587">HDInsight</span><span class="sxs-lookup"><span data-stu-id="69b8c-2587">HDInsight</span></span>
* <span data-ttu-id="69b8c-2588">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="69b8c-2588">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="69b8c-2589">IoT</span><span class="sxs-lookup"><span data-stu-id="69b8c-2589">IoT</span></span>
* <span data-ttu-id="69b8c-2590">Comando de instalação da extensão adicionado à faixa inicial</span><span class="sxs-lookup"><span data-stu-id="69b8c-2590">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="69b8c-2591">KeyVault</span><span class="sxs-lookup"><span data-stu-id="69b8c-2591">KeyVault</span></span>
* <span data-ttu-id="69b8c-2592">Alterado para restringir os comandos de armazenamento do keyvault ao perfil da API mais recente</span><span class="sxs-lookup"><span data-stu-id="69b8c-2592">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-2593">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-2593">Network</span></span>
* <span data-ttu-id="69b8c-2594">Corrigido `network dns zone create`: O comando terá êxito mesmo se o usuário tiver configurado um local padrão.</span><span class="sxs-lookup"><span data-stu-id="69b8c-2594">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="69b8c-2595">Veja o n° 6052</span><span class="sxs-lookup"><span data-stu-id="69b8c-2595">See #6052</span></span>
* <span data-ttu-id="69b8c-2596">Preterido `--remote-vnet-id` para `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2596">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="69b8c-2597">`--remote-vnet` a `network vnet peering create` adicionados, que aceita um nome ou uma ID</span><span class="sxs-lookup"><span data-stu-id="69b8c-2597">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="69b8c-2598">Suporte adicionado para vários prefixos de sub-rede a `network vnet create` com `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2598">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="69b8c-2599">Suporte adicionado para vários prefixos de sub-rede a `network vnet subnet [create|update]` com `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2599">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="69b8c-2600">Corrigido o problema com `network application-gateway create` que impedia a criação de gateways com a SKU `WAF_v2` ou `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2600">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="69b8c-2601">Argumento de conveniência `--service-endpoint-policy` adicionado a `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2601">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="69b8c-2602">Função</span><span class="sxs-lookup"><span data-stu-id="69b8c-2602">Role</span></span>
* <span data-ttu-id="69b8c-2603">Suporte adicionado para listar os proprietários de aplicativo do Azure AD para `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2603">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="69b8c-2604">Suporte adicionado para listar os proprietários da entidade de serviço do Azure AD para `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2604">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="69b8c-2605">Alterado para garantir que os comandos para criar e atualizar a definição da função aceitem várias configurações de permissão</span><span class="sxs-lookup"><span data-stu-id="69b8c-2605">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="69b8c-2606">`ad sp create-for-rbac` alterado para garantir que a URI da home page sempre seja "https"</span><span class="sxs-lookup"><span data-stu-id="69b8c-2606">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="69b8c-2607">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="69b8c-2607">Service Bus</span></span>
* <span data-ttu-id="69b8c-2608">[ALTERAÇÃO SIGNIFICATIVA]`list` comandos alterados para lidar com os erros de recurso(s) NotFound(404) do modo típico, em vez de mostrar uma lista vazia</span><span class="sxs-lookup"><span data-stu-id="69b8c-2608">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="69b8c-2609">VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-2609">VM</span></span>
* <span data-ttu-id="69b8c-2610">Corrigido o campo `accessSas` vazio em `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2610">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="69b8c-2611">`vmss create` alterado para reservar um intervalo de portas de front-end grande o suficiente para lidar com excesso de provisionamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-2611">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="69b8c-2612">Corrigidos os comandos de atualização para `sig`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2612">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="69b8c-2613">Suporte `--no-wait` adicionado para gerenciar as versões da imagem em `sig`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2613">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="69b8c-2614">`vm list-ip-addresses` alterado para mostrar a zona de disponibilidade dos endereços IP públicos</span><span class="sxs-lookup"><span data-stu-id="69b8c-2614">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="69b8c-2615">`[vm|vmss] disk attach` alterado para definir o LUN padrão do disco para o primeiro ponto disponível</span><span class="sxs-lookup"><span data-stu-id="69b8c-2615">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="69b8c-2616">21 de setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="69b8c-2616">September 21, 2018</span></span>

<span data-ttu-id="69b8c-2617">Versão 2.0.46</span><span class="sxs-lookup"><span data-stu-id="69b8c-2617">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-2618">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-2618">ACR</span></span>
* <span data-ttu-id="69b8c-2619">Adicionados comandos de tarefa de ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-2619">Added ACR Task commands</span></span>
* <span data-ttu-id="69b8c-2620">Adicionado o comando de execução rápido</span><span class="sxs-lookup"><span data-stu-id="69b8c-2620">Added quick run command</span></span>
* <span data-ttu-id="69b8c-2621">Grupo de comandos `build-task` preteridos</span><span class="sxs-lookup"><span data-stu-id="69b8c-2621">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="69b8c-2622">Adicionado o grupo de comando `helm` para dar suporte ao gerenciamento de gráficos Helm com o ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-2622">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="69b8c-2623">Suporte adicionado para criação idempotente para registro gerenciado</span><span class="sxs-lookup"><span data-stu-id="69b8c-2623">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="69b8c-2624">Adicionado um sinalizador de formato no para exibir logs de build</span><span class="sxs-lookup"><span data-stu-id="69b8c-2624">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="69b8c-2625">ACS</span><span class="sxs-lookup"><span data-stu-id="69b8c-2625">ACS</span></span>
* <span data-ttu-id="69b8c-2626">Alterado o comando `install-connector` para definir o FQDN mestre do AKS</span><span class="sxs-lookup"><span data-stu-id="69b8c-2626">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="69b8c-2627">Corrigida a criação de atribuição de função para vnet-subnet-id ao não especificar a entidade de serviço e skip-role-assignment</span><span class="sxs-lookup"><span data-stu-id="69b8c-2627">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-2628">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-2628">AppService</span></span>

* <span data-ttu-id="69b8c-2629">Adicionado suporte para o gerenciamento de operações de WebJobs (contínuos e disparados)</span><span class="sxs-lookup"><span data-stu-id="69b8c-2629">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="69b8c-2630">Suporte de az webapp config set para a propriedade --fts-state property. Adicionado suporte também para az functionapp config set & show</span><span class="sxs-lookup"><span data-stu-id="69b8c-2630">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="69b8c-2631">Adicionado suporte para trazer seu próprio armazenamento para aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="69b8c-2631">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="69b8c-2632">Adicionado suporte para a listar e restaurar aplicativos Web excluídos</span><span class="sxs-lookup"><span data-stu-id="69b8c-2632">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="69b8c-2633">Lote</span><span class="sxs-lookup"><span data-stu-id="69b8c-2633">Batch</span></span>
* <span data-ttu-id="69b8c-2634">Alterada a inclusão de tarefas por meio de `--json-file` para dar suporte à sintaxe AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="69b8c-2634">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="69b8c-2635">Atualizada a documentação de formatos `--json-file` aceitos</span><span class="sxs-lookup"><span data-stu-id="69b8c-2635">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="69b8c-2636">`--max-tasks-per-node-option` foi adicionado a `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2636">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="69b8c-2637">Alterado o comportamento de `batch account` para mostrar as contas atualmente conectadas se nenhuma opção foi especificada</span><span class="sxs-lookup"><span data-stu-id="69b8c-2637">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="69b8c-2638">Lote AI</span><span class="sxs-lookup"><span data-stu-id="69b8c-2638">Batch AI</span></span> 
* <span data-ttu-id="69b8c-2639">Corrigida a falha na criação de conta de armazenamento automática no comando `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2639">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="69b8c-2640">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="69b8c-2640">Cognitive Services</span></span>
* <span data-ttu-id="69b8c-2641">Adicionado o complemento para os argumentos `--sku`, `--kind`, `--location`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2641">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="69b8c-2642">Adicionado o comando `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2642">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="69b8c-2643">Adicionado o comando `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2643">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="69b8c-2644">Adicionado o comando `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2644">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="69b8c-2645">Preterido `cognitiveservices list`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2645">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="69b8c-2646">Alterado `--name` para que seja opcional para `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2646">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="69b8c-2647">Contêiner</span><span class="sxs-lookup"><span data-stu-id="69b8c-2647">Container</span></span>
* <span data-ttu-id="69b8c-2648">Adicionada a capacidade de reiniciar e parar um grupo de contêineres em execução</span><span class="sxs-lookup"><span data-stu-id="69b8c-2648">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="69b8c-2649">Adicionado `--network-profile` para passar em um perfil de rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-2649">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="69b8c-2650">Adicionado `--subnet`, `--vnet_name`, para permitir a criação de grupos de contêineres em uma rede virtual</span><span class="sxs-lookup"><span data-stu-id="69b8c-2650">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="69b8c-2651">Alterada a saída da tabela para mostrar o status do grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="69b8c-2651">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="69b8c-2652">DataLake</span><span class="sxs-lookup"><span data-stu-id="69b8c-2652">Datalake</span></span>
* <span data-ttu-id="69b8c-2653">Comandos adicionados para regras da rede virtual</span><span class="sxs-lookup"><span data-stu-id="69b8c-2653">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="69b8c-2654">Shell interativo</span><span class="sxs-lookup"><span data-stu-id="69b8c-2654">Interactive Shell</span></span>
* <span data-ttu-id="69b8c-2655">Corrigido o erro no Windows em que comandos não são executados corretamente</span><span class="sxs-lookup"><span data-stu-id="69b8c-2655">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="69b8c-2656">Corrigido o problema para carregar o comando no modo interativo que era causado por objetos preteridos</span><span class="sxs-lookup"><span data-stu-id="69b8c-2656">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="69b8c-2657">IoT</span><span class="sxs-lookup"><span data-stu-id="69b8c-2657">IoT</span></span>
* <span data-ttu-id="69b8c-2658">Adicionado suporte para roteamento de Hubs de IoT</span><span class="sxs-lookup"><span data-stu-id="69b8c-2658">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="69b8c-2659">Key Vault</span><span class="sxs-lookup"><span data-stu-id="69b8c-2659">Key Vault</span></span>
* <span data-ttu-id="69b8c-2660">Corrigida a importação de chave do Key Vault para chaves RSA</span><span class="sxs-lookup"><span data-stu-id="69b8c-2660">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-2661">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-2661">Network</span></span>
* <span data-ttu-id="69b8c-2662">Adicionados os comandos `network public-ip prefix` para dar suporte a recursos de prefixos de IP público</span><span class="sxs-lookup"><span data-stu-id="69b8c-2662">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="69b8c-2663">Adicionados os comandos `network service-endpoint` para dar suporte a recursos de política de ponto de extremidade de serviço</span><span class="sxs-lookup"><span data-stu-id="69b8c-2663">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="69b8c-2664">Adicionados os comandos `network lb outbound-rule` para dar suporte à criação de regras de saída do Standard Load Balancer</span><span class="sxs-lookup"><span data-stu-id="69b8c-2664">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="69b8c-2665">Adicionado `--public-ip-prefix` a `network lb frontend-ip create/update` para dar suporte a configurações de IP de front-end usando prefixos de IP público</span><span class="sxs-lookup"><span data-stu-id="69b8c-2665">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="69b8c-2666">Adicionado `--enable-tcp-reset` a `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2666">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="69b8c-2667">Adicionado `--disable-outbound-snat` a `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2667">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="69b8c-2668">Permitido o uso de `network watcher flow-log show/configure` com NSGs clássicos</span><span class="sxs-lookup"><span data-stu-id="69b8c-2668">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="69b8c-2669">Adição do comando `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2669">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="69b8c-2670">Corrigido o comando `network watcher test-connectivity` e adicionadas as propriedades `--method`, `--valid-status-codes` e `--headers`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2670">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="69b8c-2671">`network express-route create/update`: Adicionado o sinalizador `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2671">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="69b8c-2672">`network vnet subnet create/update`: Adicionado suporte para `--delegation`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2672">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="69b8c-2673">Adicionado o comando `network vnet subnet list-available-delegations`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2673">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="69b8c-2674">`network traffic-manager profile create/update`: Adicionado suporte para `--interval`, `--timeout` e `--max-failures` para as opções preteridas de configuração do monitor `--monitor-path`, `--monitor-port` e `--monitor-protocol`, que foram substituídas por `--path`, `--port` e `--protocol`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2674">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="69b8c-2675">`network lb frontend-ip create/update`: Corrigida a lógica para configurar o método de alocação de IP privado. Se um endereço IP privado for fornecido, a alocação será estática. Se nenhum endereço IP privado for fornecido ou uma cadeia de caracteres vazia for fornecida para o endereço IP privado, a alocação será dinâmica.</span><span class="sxs-lookup"><span data-stu-id="69b8c-2675">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="69b8c-2676">`dns record-set * create/update`: Adicionado suporte para `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2676">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="69b8c-2677">Adicionados comandos `network interface-endpoint` para consultar objetos do ponto de extremidade da interface</span><span class="sxs-lookup"><span data-stu-id="69b8c-2677">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="69b8c-2678">Adicionado `network profile show/list/delete` para gerenciamento parcial dos perfis de rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-2678">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="69b8c-2679">Adicionados comandos `network express-route peering connection` para gerenciar conexões de emparelhamento entre as ExpressRoutes</span><span class="sxs-lookup"><span data-stu-id="69b8c-2679">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="69b8c-2680">RDBMS</span><span class="sxs-lookup"><span data-stu-id="69b8c-2680">RDBMS</span></span>
* <span data-ttu-id="69b8c-2681">Adicionado suporte para o serviço MariaDB</span><span class="sxs-lookup"><span data-stu-id="69b8c-2681">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="69b8c-2682">Reserva</span><span class="sxs-lookup"><span data-stu-id="69b8c-2682">Reservation</span></span>
* <span data-ttu-id="69b8c-2683">Adicionado CosmosDB no tipo enumerado de recurso reservado</span><span class="sxs-lookup"><span data-stu-id="69b8c-2683">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="69b8c-2684">Adicionada a propriedade nome no modelo do Patch</span><span class="sxs-lookup"><span data-stu-id="69b8c-2684">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="69b8c-2685">Gerenciar aplicativo</span><span class="sxs-lookup"><span data-stu-id="69b8c-2685">Manage App</span></span>
* <span data-ttu-id="69b8c-2686">Corrigido o bug em `managedapp create --kind MarketPlace` que resultava em falha durante a criação da instância de um aplicativo gerenciado do Marketplace</span><span class="sxs-lookup"><span data-stu-id="69b8c-2686">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="69b8c-2687">Alterados os comandos `feature` para serem restritos somente aos perfis com suporte</span><span class="sxs-lookup"><span data-stu-id="69b8c-2687">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="69b8c-2688">Função</span><span class="sxs-lookup"><span data-stu-id="69b8c-2688">Role</span></span>
* <span data-ttu-id="69b8c-2689">Adicionado suporte para listar membros de grupo de usuários</span><span class="sxs-lookup"><span data-stu-id="69b8c-2689">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="69b8c-2690">SignalR</span><span class="sxs-lookup"><span data-stu-id="69b8c-2690">SignalR</span></span>
* <span data-ttu-id="69b8c-2691">Primeira versão</span><span class="sxs-lookup"><span data-stu-id="69b8c-2691">First release</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-2692">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-2692">Storage</span></span>
* <span data-ttu-id="69b8c-2693">Adicionado o parâmetro `--auth-mode login` para usar as credenciais de login do usuário para autorização de filas e blobs</span><span class="sxs-lookup"><span data-stu-id="69b8c-2693">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="69b8c-2694">Adicionado `storage container immutability-policy/legal-hold` para gerenciar o armazenamento imutável</span><span class="sxs-lookup"><span data-stu-id="69b8c-2694">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="69b8c-2695">VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-2695">VM</span></span>
* <span data-ttu-id="69b8c-2696">Corrigido o problema em que `vm create --generate-ssh-keys` sobrescreve o arquivo de chave privada se o arquivo de chave pública estiver ausente (#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="69b8c-2696">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="69b8c-2697">Adicionado suporte para galeria de imagem compartilhada através de `az sig`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2697">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="69b8c-2698">28 de Agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="69b8c-2698">August 28, 2018</span></span>

<span data-ttu-id="69b8c-2699">Versão 2.0.45</span><span class="sxs-lookup"><span data-stu-id="69b8c-2699">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="69b8c-2700">Núcleo</span><span class="sxs-lookup"><span data-stu-id="69b8c-2700">Core</span></span>

* <span data-ttu-id="69b8c-2701">Corrigido o problema de carregamento de arquivo de configuração vazio</span><span class="sxs-lookup"><span data-stu-id="69b8c-2701">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="69b8c-2702">Adicionado suporte para o perfil `2018-03-01-hybrid` para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="69b8c-2702">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-2703">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-2703">ACR</span></span>

* <span data-ttu-id="69b8c-2704">Adicionada uma solução alternativa para operações de runtime sem solicitações ARM</span><span class="sxs-lookup"><span data-stu-id="69b8c-2704">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="69b8c-2705">Alterado para excluir arquivos de controle de versão (por exemplo, .git, .gitignore) de tar carregados por padrão no comando `build`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2705">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="69b8c-2706">ACS</span><span class="sxs-lookup"><span data-stu-id="69b8c-2706">ACS</span></span>

* <span data-ttu-id="69b8c-2707">Alterado `aks create` para os padrões para VMs `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2707">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="69b8c-2708">Alterado `aks get-credentials` para agora chamar novas APIs para obter credenciais de cluster</span><span class="sxs-lookup"><span data-stu-id="69b8c-2708">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-2709">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-2709">AppService</span></span>

* <span data-ttu-id="69b8c-2710">Adicionado suporte para CORS no functionapp e webapp</span><span class="sxs-lookup"><span data-stu-id="69b8c-2710">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="69b8c-2711">Adicionado suporte a marcas ARM ao criar comandos</span><span class="sxs-lookup"><span data-stu-id="69b8c-2711">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="69b8c-2712">Alterado `[webapp|functionapp] identity show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="69b8c-2712">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="69b8c-2713">Backup</span><span class="sxs-lookup"><span data-stu-id="69b8c-2713">Backup</span></span>

* <span data-ttu-id="69b8c-2714">Alterado `backup vault backup-properties show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="69b8c-2714">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="69b8c-2715">Serviço de Bot</span><span class="sxs-lookup"><span data-stu-id="69b8c-2715">Bot Service</span></span>

* <span data-ttu-id="69b8c-2716">Versão da CLI do serviço de Bot inicial</span><span class="sxs-lookup"><span data-stu-id="69b8c-2716">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="69b8c-2717">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="69b8c-2717">Cognitive Services</span></span>

* <span data-ttu-id="69b8c-2718">Adicionado novo parâmetro `--api-properties,` que é necessário para a criação de alguns dos serviços</span><span class="sxs-lookup"><span data-stu-id="69b8c-2718">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="69b8c-2719">IoT</span><span class="sxs-lookup"><span data-stu-id="69b8c-2719">IoT</span></span>

* <span data-ttu-id="69b8c-2720">Corrigido o problema com a associação de hubs vinculados</span><span class="sxs-lookup"><span data-stu-id="69b8c-2720">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="69b8c-2721">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="69b8c-2721">Monitor</span></span>

* <span data-ttu-id="69b8c-2722">Adicionados comandos `monitor metrics alert` para alertas de métrica quase em tempo real</span><span class="sxs-lookup"><span data-stu-id="69b8c-2722">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="69b8c-2723">Comandos `monitor alert` preteridos</span><span class="sxs-lookup"><span data-stu-id="69b8c-2723">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-2724">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-2724">Network</span></span>

* <span data-ttu-id="69b8c-2725">Alterado `network application-gateway ssl-policy predefined show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="69b8c-2725">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="69b8c-2726">Recurso</span><span class="sxs-lookup"><span data-stu-id="69b8c-2726">Resource</span></span>

* <span data-ttu-id="69b8c-2727">Alterado `provider operation show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="69b8c-2727">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-2728">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-2728">Storage</span></span>

* <span data-ttu-id="69b8c-2729">Alterado `storage share policy show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="69b8c-2729">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="69b8c-2730">VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-2730">VM</span></span>

* <span data-ttu-id="69b8c-2731">Alterado `vm/vmss identity show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="69b8c-2731">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="69b8c-2732">Preterido `--storage-caching` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2732">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="69b8c-2733">14 de agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="69b8c-2733">Auguest 14, 2018</span></span>

<span data-ttu-id="69b8c-2734">Versão 2.0.44</span><span class="sxs-lookup"><span data-stu-id="69b8c-2734">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="69b8c-2735">Núcleo</span><span class="sxs-lookup"><span data-stu-id="69b8c-2735">Core</span></span>

* <span data-ttu-id="69b8c-2736">Corrigida a exibição numérica na saída `table`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2736">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="69b8c-2737">Adicionado o formato de saída YAML</span><span class="sxs-lookup"><span data-stu-id="69b8c-2737">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="69b8c-2738">Telemetria</span><span class="sxs-lookup"><span data-stu-id="69b8c-2738">Telemetry</span></span>

* <span data-ttu-id="69b8c-2739">Melhorias nos relatórios de telemetria</span><span class="sxs-lookup"><span data-stu-id="69b8c-2739">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-2740">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-2740">ACR</span></span>

* <span data-ttu-id="69b8c-2741">Adicionados os comandos `content-trust policy`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2741">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="69b8c-2742">Corrigido o problema onde `.dockerignore` não foi tratado adequadamente</span><span class="sxs-lookup"><span data-stu-id="69b8c-2742">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="69b8c-2743">ACS</span><span class="sxs-lookup"><span data-stu-id="69b8c-2743">ACS</span></span>

* <span data-ttu-id="69b8c-2744">Alterado `az acs/aks install-cli` para instalar em `%USERPROFILE%\.azure-kubectl` no Windows</span><span class="sxs-lookup"><span data-stu-id="69b8c-2744">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="69b8c-2745">Alterado `az aks install-connector` para detectar se o cluster tem RBAC e configurar o conector ACI adequadamente</span><span class="sxs-lookup"><span data-stu-id="69b8c-2745">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="69b8c-2746">Alterado para atribuição de função à sub-rede quando ela é fornecida</span><span class="sxs-lookup"><span data-stu-id="69b8c-2746">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="69b8c-2747">Adicionada uma nova opção para “ignorar a atribuição de função” à sub-rede quando ela é fornecida</span><span class="sxs-lookup"><span data-stu-id="69b8c-2747">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="69b8c-2748">Alterado para ignorar a atribuição de função à sub-rede quando a atribuição já existe</span><span class="sxs-lookup"><span data-stu-id="69b8c-2748">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="69b8c-2749">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-2749">AppService</span></span>

* <span data-ttu-id="69b8c-2750">Corrigido um bug que impede a criação de um aplicativo de funções usando contas de armazenamento em grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="69b8c-2750">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="69b8c-2751">Corrigida uma falha na implantação de zip</span><span class="sxs-lookup"><span data-stu-id="69b8c-2751">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="69b8c-2752">BatchAI</span><span class="sxs-lookup"><span data-stu-id="69b8c-2752">BatchAI</span></span>

* <span data-ttu-id="69b8c-2753">Alterada a saída do agente para criação de conta de armazenamento automática para especificar “ *grupo* de recurso”.</span><span class="sxs-lookup"><span data-stu-id="69b8c-2753">Changed logger output for auto-storage account creation to specifies "resource *group* ".</span></span>        

### <a name="container"></a><span data-ttu-id="69b8c-2754">Contêiner</span><span class="sxs-lookup"><span data-stu-id="69b8c-2754">Container</span></span>

* <span data-ttu-id="69b8c-2755">Adicionado `--secure-environment-variables` para passar as variáveis de ambiente seguras para um contêiner</span><span class="sxs-lookup"><span data-stu-id="69b8c-2755">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="69b8c-2756">IoT</span><span class="sxs-lookup"><span data-stu-id="69b8c-2756">IoT</span></span>

* <span data-ttu-id="69b8c-2757">[ALTERAÇÃO SIGNIFICATIVA] Removidos os comandos preteridos que foram movidos para a extensão iot</span><span class="sxs-lookup"><span data-stu-id="69b8c-2757">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="69b8c-2758">Atualizados os elementos para não presumirem o domínio `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2758">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="69b8c-2759">Central de IoT</span><span class="sxs-lookup"><span data-stu-id="69b8c-2759">Iot Central</span></span>

* <span data-ttu-id="69b8c-2760">Versão inicial do módulo do IoT Central</span><span class="sxs-lookup"><span data-stu-id="69b8c-2760">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="69b8c-2761">KeyVault</span><span class="sxs-lookup"><span data-stu-id="69b8c-2761">KeyVault</span></span>


* <span data-ttu-id="69b8c-2762">Comandos adicionados para gerenciar contas de armazenamento e as definições de sas</span><span class="sxs-lookup"><span data-stu-id="69b8c-2762">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="69b8c-2763">Comandos adicionados para regras de rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-2763">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="69b8c-2764">Adicionado o parâmetro `--id` para operações de certificado, chave e segredo</span><span class="sxs-lookup"><span data-stu-id="69b8c-2764">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="69b8c-2765">Adicionado suporte para a versão de várias APIs de gerenciamento KV</span><span class="sxs-lookup"><span data-stu-id="69b8c-2765">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="69b8c-2766">Adicionado suporte para a versão de várias APIs do plano de dados KV</span><span class="sxs-lookup"><span data-stu-id="69b8c-2766">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="69b8c-2767">Retransmissão</span><span class="sxs-lookup"><span data-stu-id="69b8c-2767">Relay</span></span>

* <span data-ttu-id="69b8c-2768">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="69b8c-2768">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="69b8c-2769">Sql</span><span class="sxs-lookup"><span data-stu-id="69b8c-2769">Sql</span></span>

* <span data-ttu-id="69b8c-2770">Adicionados os comandos `sql failover-group`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2770">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-2771">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-2771">Storage</span></span>

* <span data-ttu-id="69b8c-2772">[ALTERAÇÃO SIGNIFICATIVA] Alterado `storage account show-usage` para exigir o parâmetro `--location` e listará por região</span><span class="sxs-lookup"><span data-stu-id="69b8c-2772">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="69b8c-2773">Alterado o parâmetro `--resource-group` para ser opcional para comandos `storage account`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2773">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="69b8c-2774">Removidos os avisos de “Falha na pré-condição” para as falhas individuais em comandos em lote para uma única mensagem agregada</span><span class="sxs-lookup"><span data-stu-id="69b8c-2774">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="69b8c-2775">Alterados os comandos `[blob|file] delete-batch` para não exibir mais matriz de nulos</span><span class="sxs-lookup"><span data-stu-id="69b8c-2775">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="69b8c-2776">Alterados os comandos `blob [download|upload|delete-batch]` para ler o token de sas da url do contêiner</span><span class="sxs-lookup"><span data-stu-id="69b8c-2776">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="69b8c-2777">VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-2777">VM</span></span>

* <span data-ttu-id="69b8c-2778">Adicionado filtros comuns à `vm list-skus` para facilidade de uso</span><span class="sxs-lookup"><span data-stu-id="69b8c-2778">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="69b8c-2779">31 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="69b8c-2779">July 31, 2018</span></span>

<span data-ttu-id="69b8c-2780">Versão 2.0.43</span><span class="sxs-lookup"><span data-stu-id="69b8c-2780">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-2781">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-2781">ACR</span></span>

* <span data-ttu-id="69b8c-2782">Sinalizador `--with-secure-properties` adicionado ao comando `acr build-task show`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2782">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="69b8c-2783">Adicionado o comando `acr build-task update-build`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2783">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="69b8c-2784">ACS</span><span class="sxs-lookup"><span data-stu-id="69b8c-2784">ACS</span></span>

* <span data-ttu-id="69b8c-2785">Alterado para retornar 0 (êxito) ao terminar `az aks browse` pressionando [Ctrl+C]</span><span class="sxs-lookup"><span data-stu-id="69b8c-2785">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="69b8c-2786">Lote</span><span class="sxs-lookup"><span data-stu-id="69b8c-2786">Batch</span></span>

* <span data-ttu-id="69b8c-2787">Bug corrigido ao mostrar o token AAD no cloudshell</span><span class="sxs-lookup"><span data-stu-id="69b8c-2787">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="69b8c-2788">Contêiner</span><span class="sxs-lookup"><span data-stu-id="69b8c-2788">Container</span></span>

* <span data-ttu-id="69b8c-2789">Requisito removido de `--log-analytics-workspace-key` para o nome ou a ID ao definir assinatura</span><span class="sxs-lookup"><span data-stu-id="69b8c-2789">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-2790">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-2790">Network</span></span>

* <span data-ttu-id="69b8c-2791">Suporte a DNS adicionado a 2017-03-09-profile para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="69b8c-2791">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="69b8c-2792">Recurso</span><span class="sxs-lookup"><span data-stu-id="69b8c-2792">Resource</span></span>

* <span data-ttu-id="69b8c-2793">`--rollback-on-error` a `group deployment create` adicionado para executar uma implantação válida no erro</span><span class="sxs-lookup"><span data-stu-id="69b8c-2793">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="69b8c-2794">Problema corrigido onde `--parameters {}` com `group deployment create` resultou em um erro</span><span class="sxs-lookup"><span data-stu-id="69b8c-2794">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="69b8c-2795">Função</span><span class="sxs-lookup"><span data-stu-id="69b8c-2795">Role</span></span>

* <span data-ttu-id="69b8c-2796">Suporte adicionado para o perfil da pilha 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="69b8c-2796">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="69b8c-2797">Problema corrigido onde os parâmetros de atualização genéricos para `app update` não funcionariam corretamente</span><span class="sxs-lookup"><span data-stu-id="69b8c-2797">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="69b8c-2798">Search</span><span class="sxs-lookup"><span data-stu-id="69b8c-2798">Search</span></span>

* <span data-ttu-id="69b8c-2799">Comandos adicionados para o serviço Azure Search</span><span class="sxs-lookup"><span data-stu-id="69b8c-2799">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="69b8c-2800">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="69b8c-2800">Service Bus</span></span>

* <span data-ttu-id="69b8c-2801">Grupo de comandos de migração adicionados para migrar um namespace do Barramento de Serviço Standard para Premium</span><span class="sxs-lookup"><span data-stu-id="69b8c-2801">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="69b8c-2802">Novas propriedades opcionais adicionadas à fila do Barramento de Serviço e à Assinatura</span><span class="sxs-lookup"><span data-stu-id="69b8c-2802">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="69b8c-2803">`--enable-batched-operations` e `--enable-dead-lettering-on-message-expiration` em `queue`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2803">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="69b8c-2804">`--dead-letter-on-filter-exceptions` em `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2804">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-2805">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-2805">Storage</span></span>

* <span data-ttu-id="69b8c-2806">Suporte adicionado para o download de arquivos grandes usando uma única conexão</span><span class="sxs-lookup"><span data-stu-id="69b8c-2806">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="69b8c-2807">Comandos `show` convertidos que foram perdidos na falha com código de saída 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="69b8c-2807">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="69b8c-2808">VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-2808">VM</span></span>

* <span data-ttu-id="69b8c-2809">Suporte adicionado para listar conjuntos de disponibilidade por assinatura</span><span class="sxs-lookup"><span data-stu-id="69b8c-2809">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="69b8c-2810">Adicionado o suporte para `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2810">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="69b8c-2811">Suporte adicionado para o grupo de segurança do aplicativo ao criar um conjunto de dimensionamento da VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-2811">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="69b8c-2812">[ALTERAÇÃO SIGNIFICATIVA]`[vm|vmss] create`, `[vm|vmss] identity assign` e `[vm|vmss] identity remove` alterados para produzir identidades de usuário atribuídas no formato de dicionário</span><span class="sxs-lookup"><span data-stu-id="69b8c-2812">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="69b8c-2813">18 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="69b8c-2813">July 18, 2018</span></span>

<span data-ttu-id="69b8c-2814">Versão 2.0.42</span><span class="sxs-lookup"><span data-stu-id="69b8c-2814">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="69b8c-2815">Núcleo</span><span class="sxs-lookup"><span data-stu-id="69b8c-2815">Core</span></span>

* <span data-ttu-id="69b8c-2816">Adicionado suporte para logon baseado em navegador, na janela de bash WSL</span><span class="sxs-lookup"><span data-stu-id="69b8c-2816">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="69b8c-2817">O sinalizador `--force-string` foi adicionado a todos os comandos de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="69b8c-2817">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="69b8c-2818">[ALTERAÇÃO SIGNIFICATIVA] Os comandos 'show' foram alterados para registrar mensagens de erro e falha com código de saída 3 quando um recurso está ausente</span><span class="sxs-lookup"><span data-stu-id="69b8c-2818">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-2819">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-2819">ACR</span></span>

* <span data-ttu-id="69b8c-2820">[ALTERAÇÃO SIGNIFICATIVA] '--no-push' foi atualizado para um sinalizador puro no comando 'acr build'</span><span class="sxs-lookup"><span data-stu-id="69b8c-2820">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="69b8c-2821">Foram adicionados os comandos `show` e `update` no grupo `acr repository`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2821">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="69b8c-2822">Foi adicionado o sinalizador `--detail` a `show-manifests` e `show-tags` para mostrar informações mais detalhadas</span><span class="sxs-lookup"><span data-stu-id="69b8c-2822">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="69b8c-2823">Foi adicionado o parâmetro `--image` para dar suporte aos detalhes do build get ou aos logs por meio de uma imagem</span><span class="sxs-lookup"><span data-stu-id="69b8c-2823">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="69b8c-2824">ACS</span><span class="sxs-lookup"><span data-stu-id="69b8c-2824">ACS</span></span>

* <span data-ttu-id="69b8c-2825">`az aks create` foi alterado para excluir o erro se `--max-pods` for menor que 5</span><span class="sxs-lookup"><span data-stu-id="69b8c-2825">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-2826">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-2826">AppService</span></span>

* <span data-ttu-id="69b8c-2827">Suporte adicionado para skus PremiumV2</span><span class="sxs-lookup"><span data-stu-id="69b8c-2827">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="69b8c-2828">Lote</span><span class="sxs-lookup"><span data-stu-id="69b8c-2828">Batch</span></span>

* <span data-ttu-id="69b8c-2829">Corrigido o bug sobre como usar a credencial de token no modo do Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="69b8c-2829">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="69b8c-2830">Alterada a entrada JSON para diferenciar maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="69b8c-2830">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="69b8c-2831">Lote AI</span><span class="sxs-lookup"><span data-stu-id="69b8c-2831">Batch AI</span></span>

* <span data-ttu-id="69b8c-2832">Corrigido o comando `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2832">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="69b8c-2833">Contêiner</span><span class="sxs-lookup"><span data-stu-id="69b8c-2833">Container</span></span>

* <span data-ttu-id="69b8c-2834">Removido o requisito de nome de usuário e senha para os registros não dockerhub</span><span class="sxs-lookup"><span data-stu-id="69b8c-2834">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="69b8c-2835">Correção de erro durante a criação de grupos de contêineres de arquivo yaml</span><span class="sxs-lookup"><span data-stu-id="69b8c-2835">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-2836">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-2836">Network</span></span>

* <span data-ttu-id="69b8c-2837">Adicionado o suporte `--no-wait` para `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2837">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="69b8c-2838">Adicionado `network nic wait`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2838">Added `network nic wait`</span></span>
* <span data-ttu-id="69b8c-2839">Preterido o argumento `--ids` para `network vnet [subnet|peering] list`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2839">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="69b8c-2840">Adicionado o sinalizador `--include-default` para incluir regras de segurança padrão na saída do `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2840">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="69b8c-2841">Recurso</span><span class="sxs-lookup"><span data-stu-id="69b8c-2841">Resource</span></span>

* <span data-ttu-id="69b8c-2842">Adicionado o suporte `--no-wait` para `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2842">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="69b8c-2843">Adicionado o suporte `--no-wait` para `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2843">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="69b8c-2844">Adicionado o comando `deployment wait`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2844">Added `deployment wait` command</span></span>
* <span data-ttu-id="69b8c-2845">Correção do problema em que os comandos de nível de assinatura `az deployment` erroneamente apareceram no perfil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="69b8c-2845">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="69b8c-2846">SQL</span><span class="sxs-lookup"><span data-stu-id="69b8c-2846">SQL</span></span>

* <span data-ttu-id="69b8c-2847">O erro “O nome de grupo de recursos fornecido ... não correspondeu ao nome na Url” foi fixado ao especificar o nome do pool elástico para os comandos `sql db copy` e `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2847">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="69b8c-2848">Permitir a configuração do padrão do SQL Server, executando `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2848">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="69b8c-2849">Os formatadores de tabela foram implementados aos comandos `sql server`, `sql server firewall-rule`, `sql list-usages` e `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2849">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-2850">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-2850">Storage</span></span>

* <span data-ttu-id="69b8c-2851">Adicionada a propriedade `pageRanges` à saída `storage blob show` que será preenchida para blobs de página</span><span class="sxs-lookup"><span data-stu-id="69b8c-2851">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="69b8c-2852">VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-2852">VM</span></span>

* <span data-ttu-id="69b8c-2853">[ALTERAÇÃO SIGNIFICATIVA] Alterado `vmss create` para usar o `Standard_DS1_v2` como o tamanho de instância padrão</span><span class="sxs-lookup"><span data-stu-id="69b8c-2853">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="69b8c-2854">Adicionado o suporte `--no-wait` para `vm extension [set|delete]` e `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2854">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="69b8c-2855">Adicionado `vm extension wait`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2855">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="69b8c-2856">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="69b8c-2856">July 3, 2018</span></span>

<span data-ttu-id="69b8c-2857">Versão 2.0.41</span><span class="sxs-lookup"><span data-stu-id="69b8c-2857">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="69b8c-2858">AKS</span><span class="sxs-lookup"><span data-stu-id="69b8c-2858">AKS</span></span>

* <span data-ttu-id="69b8c-2859">Monitoramento alterado para usar a ID de assinatura</span><span class="sxs-lookup"><span data-stu-id="69b8c-2859">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="69b8c-2860">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="69b8c-2860">July 3, 2018</span></span>

<span data-ttu-id="69b8c-2861">Versão 2.0.40</span><span class="sxs-lookup"><span data-stu-id="69b8c-2861">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="69b8c-2862">Núcleo</span><span class="sxs-lookup"><span data-stu-id="69b8c-2862">Core</span></span>

* <span data-ttu-id="69b8c-2863">Adicionado um novo fluxo de código de autorização para o logon interativo</span><span class="sxs-lookup"><span data-stu-id="69b8c-2863">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-2864">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-2864">ACR</span></span>

* <span data-ttu-id="69b8c-2865">Status da compilação de sondagem adicionado</span><span class="sxs-lookup"><span data-stu-id="69b8c-2865">Added polling build status</span></span>
* <span data-ttu-id="69b8c-2866">Suporte adicionado para valores de enumeração que não diferenciam maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="69b8c-2866">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="69b8c-2867">Parâmetros `--top` e `--orderby` adicionados para `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2867">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="69b8c-2868">ACS</span><span class="sxs-lookup"><span data-stu-id="69b8c-2868">ACS</span></span>

* <span data-ttu-id="69b8c-2869">[ALTERAÇÃO SIGNIFICATIVA] Habilitar controle de acesso baseado em funções do Kubernetes por padrão</span><span class="sxs-lookup"><span data-stu-id="69b8c-2869">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="69b8c-2870">Argumento `--disable-rbac` e preterido `--enable-rbac` adicionados, pois é o padrão agora</span><span class="sxs-lookup"><span data-stu-id="69b8c-2870">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="69b8c-2871">Opções atualizadas do comando `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="69b8c-2871">Updated options for `aks browse` command.</span></span> <span data-ttu-id="69b8c-2872">Suporte `--listen-port` adicionado</span><span class="sxs-lookup"><span data-stu-id="69b8c-2872">Added `--listen-port` support</span></span>
* <span data-ttu-id="69b8c-2873">Atualizado o pacote de gráficos do helm padrão para o comando `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="69b8c-2873">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="69b8c-2874">Usar virtual-kubelet-para-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="69b8c-2874">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="69b8c-2875">Comandos `aks enable-addons` e `aks disable-addons` adicionados para atualizar um cluster existente</span><span class="sxs-lookup"><span data-stu-id="69b8c-2875">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-2876">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-2876">AppService</span></span>

* <span data-ttu-id="69b8c-2877">Suporte adicionado para desabilitar a identidade via `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2877">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="69b8c-2878">Marca `preview` removida para o recurso de Identidade</span><span class="sxs-lookup"><span data-stu-id="69b8c-2878">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="69b8c-2879">Backup</span><span class="sxs-lookup"><span data-stu-id="69b8c-2879">Backup</span></span>

* <span data-ttu-id="69b8c-2880">Definição do módulo atualizada</span><span class="sxs-lookup"><span data-stu-id="69b8c-2880">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="69b8c-2881">BatchAI</span><span class="sxs-lookup"><span data-stu-id="69b8c-2881">BatchAI</span></span>

* <span data-ttu-id="69b8c-2882">Saída da tabela corrigida para comandos `batchai cluster node list` e `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2882">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="69b8c-2883">Nuvem</span><span class="sxs-lookup"><span data-stu-id="69b8c-2883">Cloud</span></span>

* <span data-ttu-id="69b8c-2884">Sufixo do servidor `acr login` adicionado à configuração de nuvem</span><span class="sxs-lookup"><span data-stu-id="69b8c-2884">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="69b8c-2885">Contêiner</span><span class="sxs-lookup"><span data-stu-id="69b8c-2885">Container</span></span>

* <span data-ttu-id="69b8c-2886">`container create` alterado para padrão para a operação de longa execução</span><span class="sxs-lookup"><span data-stu-id="69b8c-2886">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="69b8c-2887">Parâmetros `--log-analytics-workspace` e `--log-analytics-workspace-key` adicionados do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="69b8c-2887">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="69b8c-2888">Parâmetro `--protocol` adicionado para especificar qual protocolo de rede usar</span><span class="sxs-lookup"><span data-stu-id="69b8c-2888">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="69b8c-2889">Extensão</span><span class="sxs-lookup"><span data-stu-id="69b8c-2889">Extension</span></span>

* <span data-ttu-id="69b8c-2890">`extension list-available` alterado para mostrar apenas as extensões compatíveis com a versão da CLI</span><span class="sxs-lookup"><span data-stu-id="69b8c-2890">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-2891">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-2891">Network</span></span>

* <span data-ttu-id="69b8c-2892">Corrigido o problema onde os tipos de registro diferenciam maiúsculas de minúsculas ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="69b8c-2892">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="69b8c-2893">Rdbms</span><span class="sxs-lookup"><span data-stu-id="69b8c-2893">Rdbms</span></span>

* <span data-ttu-id="69b8c-2894">Adicionados os comandos `[postgres|myql] server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2894">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="69b8c-2895">Recurso</span><span class="sxs-lookup"><span data-stu-id="69b8c-2895">Resource</span></span>

* <span data-ttu-id="69b8c-2896">Novo grupo de operação `deployment` adicionado</span><span class="sxs-lookup"><span data-stu-id="69b8c-2896">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="69b8c-2897">VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-2897">VM</span></span>

* <span data-ttu-id="69b8c-2898">Suporte adicionado para remover a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="69b8c-2898">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="69b8c-2899">25 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="69b8c-2899">June 25, 2018</span></span>

<span data-ttu-id="69b8c-2900">Versão 2.0.39</span><span class="sxs-lookup"><span data-stu-id="69b8c-2900">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="69b8c-2901">CLI</span><span class="sxs-lookup"><span data-stu-id="69b8c-2901">CLI</span></span>

* <span data-ttu-id="69b8c-2902">Corte de arquivo atualizado no instalador MSI para corrigir o problema de instalação da extensão</span><span class="sxs-lookup"><span data-stu-id="69b8c-2902">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="69b8c-2903">19 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="69b8c-2903">June 19, 2018</span></span>

<span data-ttu-id="69b8c-2904">Versão 2.0.38</span><span class="sxs-lookup"><span data-stu-id="69b8c-2904">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="69b8c-2905">Núcleo</span><span class="sxs-lookup"><span data-stu-id="69b8c-2905">Core</span></span>

* <span data-ttu-id="69b8c-2906">Suporte global adicionado para `--subscription` a maioria dos comandos</span><span class="sxs-lookup"><span data-stu-id="69b8c-2906">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-2907">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-2907">ACR</span></span>

* <span data-ttu-id="69b8c-2908">`azure-storage-blob` foi adicionado como dependência</span><span class="sxs-lookup"><span data-stu-id="69b8c-2908">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="69b8c-2909">A configuração de CPU padrão foi alterada com `acr build-task create` para usar 2 núcleos</span><span class="sxs-lookup"><span data-stu-id="69b8c-2909">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="69b8c-2910">ACS</span><span class="sxs-lookup"><span data-stu-id="69b8c-2910">ACS</span></span>

* <span data-ttu-id="69b8c-2911">As opções do comando `aks use-dev-spaces` foram atualizadas.</span><span class="sxs-lookup"><span data-stu-id="69b8c-2911">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="69b8c-2912">Suporte `--update` adicionado</span><span class="sxs-lookup"><span data-stu-id="69b8c-2912">Added `--update` support</span></span>
* <span data-ttu-id="69b8c-2913">`aks get-credentials --admin` foi alterado para substituir o contexto do usuário em `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2913">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="69b8c-2914">A propriedade `nodeResourceGroup` somente leitura foi exposta em clusters gerenciados</span><span class="sxs-lookup"><span data-stu-id="69b8c-2914">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="69b8c-2915">O erro de comando `acs browse` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="69b8c-2915">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="69b8c-2916">Foram feitas `--connector-name` opcional para `aks install-connector`, `aks upgrade-connector` e `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2916">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="69b8c-2917">Novas regiões de Instância de Contêiner do Azure foram adicionadas para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2917">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="69b8c-2918">O local normalizado foi adicionado no nome de versão do comando e no nome do nó para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2918">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-2919">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-2919">AppService</span></span>

* <span data-ttu-id="69b8c-2920">Foi adicionado suporte para versões mais recentes do urllib</span><span class="sxs-lookup"><span data-stu-id="69b8c-2920">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="69b8c-2921">Foi adicionado suporte para `functionapp create` para usar o plano de serviço de aplicativo de grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="69b8c-2921">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="69b8c-2922">Lote</span><span class="sxs-lookup"><span data-stu-id="69b8c-2922">Batch</span></span>

* <span data-ttu-id="69b8c-2923">A dependência `azure-batch-extensions` foi removida</span><span class="sxs-lookup"><span data-stu-id="69b8c-2923">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="69b8c-2924">Lote AI</span><span class="sxs-lookup"><span data-stu-id="69b8c-2924">Batch AI</span></span>

* <span data-ttu-id="69b8c-2925">Foi adicionado suporte aos workspaces.</span><span class="sxs-lookup"><span data-stu-id="69b8c-2925">Added support for workspaces.</span></span> <span data-ttu-id="69b8c-2926">Os workspaces permitem agrupar clusters, servidores de arquivos e experimentos, removendo a limitação no número de recursos que podem ser criados</span><span class="sxs-lookup"><span data-stu-id="69b8c-2926">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="69b8c-2927">Foi adicionado suporte para os experimentos.</span><span class="sxs-lookup"><span data-stu-id="69b8c-2927">Added support for experiments.</span></span> <span data-ttu-id="69b8c-2928">Os experimentos permitem agrupar trabalhos em coleções removendo a limitação no número de trabalhos criados</span><span class="sxs-lookup"><span data-stu-id="69b8c-2928">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="69b8c-2929">Foi adicionado suporte para configurar `/dev/shm` para trabalhos em execução em um contêiner de docker</span><span class="sxs-lookup"><span data-stu-id="69b8c-2929">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="69b8c-2930">Foram adicionados os comandos `batchai cluster node exec` e `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="69b8c-2930">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="69b8c-2931">Esses comandos permitem executar qualquer comando diretamente nos nós e fornece a funcionalidade de encaminhamento de porta.</span><span class="sxs-lookup"><span data-stu-id="69b8c-2931">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="69b8c-2932">Foi adicionado suporte a `--ids` para os comandos `batchai`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2932">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="69b8c-2933">[ALTERAÇÃO SIGNIFICATIVA] Todos os clusters e servidores de arquivos devem ser criados nos workspaces</span><span class="sxs-lookup"><span data-stu-id="69b8c-2933">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="69b8c-2934">[ALTERAÇÃO SIGNIFICATIVA] Os trabalhos devem ser criados nas experiências</span><span class="sxs-lookup"><span data-stu-id="69b8c-2934">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="69b8c-2935">[ALTERAÇÃO SIGNIFICATIVA]`--nfs-resource-group` foi removido dos comandos `cluster create` e `job create`.</span><span class="sxs-lookup"><span data-stu-id="69b8c-2935">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="69b8c-2936">Para montar um NFS pertencente a outro workspace/grupo de recursos, forneça a ID de ARM do servidor de arquivos através da opção `--nfs`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2936">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="69b8c-2937">[ALTERAÇÃO SIGNIFICATIVA]`--cluster-resource-group` foi removido do comando `job create`.</span><span class="sxs-lookup"><span data-stu-id="69b8c-2937">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="69b8c-2938">Para enviar um trabalho em um cluster pertencente a outro workspace/grupo de recursos, forneça a ID de ARM do cluster através da opção `--cluster`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2938">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="69b8c-2939">[ALTERAÇÃO SIGNIFICATIVA] O atributo `location` foi removido de trabalhos, cluster e servidores de arquivos.</span><span class="sxs-lookup"><span data-stu-id="69b8c-2939">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="69b8c-2940">Agora, o local é um atributo de um workspace.</span><span class="sxs-lookup"><span data-stu-id="69b8c-2940">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="69b8c-2941">[ALTERAÇÃO SIGNIFICATIVA]`--location` foi removido dos comandos `job create` e `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2941">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="69b8c-2942">[ALTERAÇÃO SIGNIFICATIVA] Os nomes das opções curtas foi alterado para tornar a interface mais consistente:</span><span class="sxs-lookup"><span data-stu-id="69b8c-2942">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="69b8c-2943">[`--config`, `-c`] foi renomeado para [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="69b8c-2943">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="69b8c-2944">[`--cluster`, `-r`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="69b8c-2944">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="69b8c-2945">[`--cluster`, `-n`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="69b8c-2945">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="69b8c-2946">[`--job`, `-n`] foi renomeado para [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="69b8c-2946">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="69b8c-2947">Mapas</span><span class="sxs-lookup"><span data-stu-id="69b8c-2947">Maps</span></span>

* <span data-ttu-id="69b8c-2948">[ALTERAÇÃO SIGNIFICATIVA]`maps account create` foi alterado para exigir a aceitação dos Termos de Serviço pelo prompt interativo ou sinalizador `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2948">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-2949">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-2949">Network</span></span>

* <span data-ttu-id="69b8c-2950">Suporte adicionado para `https` a `network lb probe create` [nº6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="69b8c-2950">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="69b8c-2951">Foi corrigido o problema em que `--endpoint-status` diferenciava maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="69b8c-2951">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="69b8c-2952">#6502</span><span class="sxs-lookup"><span data-stu-id="69b8c-2952">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="69b8c-2953">Reservas</span><span class="sxs-lookup"><span data-stu-id="69b8c-2953">Reservations</span></span>

* <span data-ttu-id="69b8c-2954">[ALTERAÇÃO SIGNIFICATIVA] Foi adicionado o parâmetro `ReservedResourceType` necessário a `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2954">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="69b8c-2955">Parâmetro `Location` adicionado a `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2955">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="69b8c-2956">[ALTERAÇÃO SIGNIFICATIVA]`kind` foi removido de `ReservationProperties`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2956">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="69b8c-2957">[ALTERAÇÃO SIGNIFICATIVA]`capabilities` foi renomeado para `sku_properties` em `Catalog`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2957">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="69b8c-2958">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `size` e `tier` foram removidas de `Catalog`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2958">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="69b8c-2959">Parâmetro `InstanceFlexibility` adicionado a `reservations reservation update`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2959">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="69b8c-2960">Função</span><span class="sxs-lookup"><span data-stu-id="69b8c-2960">Role</span></span>

* <span data-ttu-id="69b8c-2961">Tratamento de erro melhorado</span><span class="sxs-lookup"><span data-stu-id="69b8c-2961">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="69b8c-2962">SQL</span><span class="sxs-lookup"><span data-stu-id="69b8c-2962">SQL</span></span>

* <span data-ttu-id="69b8c-2963">Foi corrigido um erro confuso ao executar `az sql db list-editions` para um local que não está disponível para sua assinatura</span><span class="sxs-lookup"><span data-stu-id="69b8c-2963">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-2964">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-2964">Storage</span></span>

* <span data-ttu-id="69b8c-2965">A saída da tabela foi alterada para `storage blob download` para ser mais legível</span><span class="sxs-lookup"><span data-stu-id="69b8c-2965">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="69b8c-2966">VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-2966">VM</span></span>

* <span data-ttu-id="69b8c-2967">A verificação da refinação do tamanho da VM foi aprimorada para o suporte de rede acelerada em `vm create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2967">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="69b8c-2968">Foi adicionado um aviso para `vmss create` informando que o tamanho padrão da VM será alternado de `Standard_D1_v2` para `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2968">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="69b8c-2969">Foi adicionado `--force-update` a `[vm|vmss] extension set` para atualizar a extensão mesmo quando a configuração não foi alterada</span><span class="sxs-lookup"><span data-stu-id="69b8c-2969">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="69b8c-2970">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="69b8c-2970">June 13, 2018</span></span>

<span data-ttu-id="69b8c-2971">Versão 2.0.37</span><span class="sxs-lookup"><span data-stu-id="69b8c-2971">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="69b8c-2972">Núcleo</span><span class="sxs-lookup"><span data-stu-id="69b8c-2972">Core</span></span>

* <span data-ttu-id="69b8c-2973">A telemetria interativa foi melhorada</span><span class="sxs-lookup"><span data-stu-id="69b8c-2973">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="69b8c-2974">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="69b8c-2974">June 13, 2018</span></span>

<span data-ttu-id="69b8c-2975">Versão 2.0.36</span><span class="sxs-lookup"><span data-stu-id="69b8c-2975">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="69b8c-2976">AKS</span><span class="sxs-lookup"><span data-stu-id="69b8c-2976">AKS</span></span>

* <span data-ttu-id="69b8c-2977">Foram adicionadas opções avançadas de rede para `aks create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2977">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="69b8c-2978">Foram adicionados argumentos para `aks create` para habilitar o monitoramento e roteamento de HTTP</span><span class="sxs-lookup"><span data-stu-id="69b8c-2978">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="69b8c-2979">Adicionado o argumento `--no-ssh-key` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2979">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="69b8c-2980">Adicionado o argumento `--enable-rbac` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2980">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="69b8c-2981">[VERSÃO PRÉVIA] Suporte adicionado para a autenticação do Azure Active Directory no `aks create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2981">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-2982">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-2982">AppService</span></span>

* <span data-ttu-id="69b8c-2983">Foi corrigido um problema com as versões urllib incompatíveis</span><span class="sxs-lookup"><span data-stu-id="69b8c-2983">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="69b8c-2984">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="69b8c-2984">June 5, 2018</span></span>

<span data-ttu-id="69b8c-2985">Versão 2.0.35</span><span class="sxs-lookup"><span data-stu-id="69b8c-2985">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="69b8c-2986">Interativo</span><span class="sxs-lookup"><span data-stu-id="69b8c-2986">Interactive</span></span>

* <span data-ttu-id="69b8c-2987">Foram adicionados limites para as dependências do modo interativo</span><span class="sxs-lookup"><span data-stu-id="69b8c-2987">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="69b8c-2988">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="69b8c-2988">June 5, 2018</span></span>

<span data-ttu-id="69b8c-2989">Versão 2.0.34</span><span class="sxs-lookup"><span data-stu-id="69b8c-2989">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="69b8c-2990">Núcleo</span><span class="sxs-lookup"><span data-stu-id="69b8c-2990">Core</span></span>

* <span data-ttu-id="69b8c-2991">Suporte adicionado para referência de recursos de locatário cruzado</span><span class="sxs-lookup"><span data-stu-id="69b8c-2991">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="69b8c-2992">Melhor confiabilidade de carregamento de telemetria</span><span class="sxs-lookup"><span data-stu-id="69b8c-2992">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-2993">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-2993">ACR</span></span>

* <span data-ttu-id="69b8c-2994">Suporte adicionado para VSTS como um local de origem remota</span><span class="sxs-lookup"><span data-stu-id="69b8c-2994">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="69b8c-2995">Adicionado o comando `acr import`</span><span class="sxs-lookup"><span data-stu-id="69b8c-2995">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="69b8c-2996">AKS</span><span class="sxs-lookup"><span data-stu-id="69b8c-2996">AKS</span></span>

* <span data-ttu-id="69b8c-2997">`aks get-credentials` foi alterado para criar o arquivo de configuração kube com permissões de sistema de arquivos mais seguras</span><span class="sxs-lookup"><span data-stu-id="69b8c-2997">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="69b8c-2998">Lote</span><span class="sxs-lookup"><span data-stu-id="69b8c-2998">Batch</span></span>

* <span data-ttu-id="69b8c-2999">Correção do bug na formatação de tabela da lista de Pool [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="69b8c-2999">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="69b8c-3000">IOT</span><span class="sxs-lookup"><span data-stu-id="69b8c-3000">IOT</span></span>

* <span data-ttu-id="69b8c-3001">Suporte adicionado para a criação de Hubs IoT de Camada Básica</span><span class="sxs-lookup"><span data-stu-id="69b8c-3001">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-3002">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-3002">Network</span></span>

* <span data-ttu-id="69b8c-3003">`network vnet peering` melhorado</span><span class="sxs-lookup"><span data-stu-id="69b8c-3003">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="69b8c-3004">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="69b8c-3004">Policy Insights</span></span>

* <span data-ttu-id="69b8c-3005">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="69b8c-3005">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="69b8c-3006">ARM</span><span class="sxs-lookup"><span data-stu-id="69b8c-3006">ARM</span></span>

* <span data-ttu-id="69b8c-3007">Comandos `account management-group` adicionados.</span><span class="sxs-lookup"><span data-stu-id="69b8c-3007">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="69b8c-3008">SQL</span><span class="sxs-lookup"><span data-stu-id="69b8c-3008">SQL</span></span>

* <span data-ttu-id="69b8c-3009">Novos comandos de instância gerenciada adicionados:</span><span class="sxs-lookup"><span data-stu-id="69b8c-3009">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="69b8c-3010">Novos comandos de banco de dados gerenciado adicionados:</span><span class="sxs-lookup"><span data-stu-id="69b8c-3010">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="69b8c-3011">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-3011">Storage</span></span>

* <span data-ttu-id="69b8c-3012">Mimetypes extra adicionados para json e javascript para ser deduzido de extensões de arquivo</span><span class="sxs-lookup"><span data-stu-id="69b8c-3012">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="69b8c-3013">VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-3013">VM</span></span>

* <span data-ttu-id="69b8c-3014">`vm list-skus` foi alterado para usar colunas fixas e adicionar o aviso de que `Tier` e `Size` serão removidos</span><span class="sxs-lookup"><span data-stu-id="69b8c-3014">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="69b8c-3015">Opção `--accelerated-networking` adicionada a `vm create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3015">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="69b8c-3016">`--tags` foi adicionado a `identity create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3016">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="69b8c-3017">22 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="69b8c-3017">May 22, 2018</span></span>

<span data-ttu-id="69b8c-3018">Versão 2.0.33</span><span class="sxs-lookup"><span data-stu-id="69b8c-3018">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="69b8c-3019">Núcleo</span><span class="sxs-lookup"><span data-stu-id="69b8c-3019">Core</span></span>

* <span data-ttu-id="69b8c-3020">Suporte adicionado para expandir `@` em nomes de arquivos</span><span class="sxs-lookup"><span data-stu-id="69b8c-3020">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="69b8c-3021">ACS</span><span class="sxs-lookup"><span data-stu-id="69b8c-3021">ACS</span></span>

* <span data-ttu-id="69b8c-3022">Novos comandos de espaços de desenvolvimento `aks use-dev-spaces` e `aks remove-dev-spaces` foram adicionados</span><span class="sxs-lookup"><span data-stu-id="69b8c-3022">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="69b8c-3023">Erro de digitação corrigido na mensagem de ajuda</span><span class="sxs-lookup"><span data-stu-id="69b8c-3023">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-3024">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-3024">AppService</span></span>

* <span data-ttu-id="69b8c-3025">Comandos melhorados de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="69b8c-3025">Improved generic update commands</span></span>
* <span data-ttu-id="69b8c-3026">Suporte assíncrono adicionado para `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3026">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="69b8c-3027">Contêiner</span><span class="sxs-lookup"><span data-stu-id="69b8c-3027">Container</span></span>

* <span data-ttu-id="69b8c-3028">Suporte adicionado para a exportação de um grupo de contêiner no formato yaml</span><span class="sxs-lookup"><span data-stu-id="69b8c-3028">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="69b8c-3029">Suporte adicionado para usar um arquivo yaml para criar/atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="69b8c-3029">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="69b8c-3030">Extensão</span><span class="sxs-lookup"><span data-stu-id="69b8c-3030">Extension</span></span>

* <span data-ttu-id="69b8c-3031">Remoção de extensões melhorada</span><span class="sxs-lookup"><span data-stu-id="69b8c-3031">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="69b8c-3032">Interativo</span><span class="sxs-lookup"><span data-stu-id="69b8c-3032">Interactive</span></span>

* <span data-ttu-id="69b8c-3033">Log de alterações alterado para silenciar o analisador para conclusões</span><span class="sxs-lookup"><span data-stu-id="69b8c-3033">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="69b8c-3034">Manipulação aprimorada de caches de ajuda inválida</span><span class="sxs-lookup"><span data-stu-id="69b8c-3034">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="69b8c-3035">KeyVault</span><span class="sxs-lookup"><span data-stu-id="69b8c-3035">KeyVault</span></span>

* <span data-ttu-id="69b8c-3036">Comandos de keyvault corrigidos para trabalhar no cloud shell ou VMs com identidade</span><span class="sxs-lookup"><span data-stu-id="69b8c-3036">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-3037">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-3037">Network</span></span>

* <span data-ttu-id="69b8c-3038">Corrija o problema em que `network watcher show-topology` não funcionará com o nome de rede virtual e/ou sub-rede [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="69b8c-3038">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="69b8c-3039">Corrija o problema onde alguns comandos `network watcher` iriam declarar que o Observador de Rede não está habilitado para regiões quando na verdade é [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="69b8c-3039">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="69b8c-3040">SQL</span><span class="sxs-lookup"><span data-stu-id="69b8c-3040">SQL</span></span>

* <span data-ttu-id="69b8c-3041">[ALTERAÇÃO SIGNIFICATIVA] Objetos de resposta alterados retornados dos comandos `db` e `dw`:</span><span class="sxs-lookup"><span data-stu-id="69b8c-3041">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="69b8c-3042">A propriedade `serviceLevelObjective` foi renomeada para `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3042">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="69b8c-3043">As propriedades `currentServiceObjectiveId` e `requestedServiceObjectiveId` foram removidas</span><span class="sxs-lookup"><span data-stu-id="69b8c-3043">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="69b8c-3044">A propriedade `maxSizeBytes` foi alterada para ser um valor inteiro em vez de uma cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69b8c-3044">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="69b8c-3045">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `db` e `dw` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="69b8c-3045">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="69b8c-3046">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="69b8c-3046">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="69b8c-3047">Para atualizar, use o parâmetro `--service-objective` ou defina a propriedade `sku.name`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3047">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="69b8c-3048">`edition`.</span><span class="sxs-lookup"><span data-stu-id="69b8c-3048">`edition`.</span></span> <span data-ttu-id="69b8c-3049">Para atualizar, use o parâmetro `--edition` ou defina a propriedade `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3049">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="69b8c-3050">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="69b8c-3050">`elasticPoolName`.</span></span> <span data-ttu-id="69b8c-3051">Para atualizar, use o parâmetro `--elastic-pool` ou defina a propriedade `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3051">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="69b8c-3052">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `elastic-pool` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="69b8c-3052">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="69b8c-3053">`edition`.</span><span class="sxs-lookup"><span data-stu-id="69b8c-3053">`edition`.</span></span> <span data-ttu-id="69b8c-3054">Para atualizar, use o parâmetro `--edition`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3054">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="69b8c-3055">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="69b8c-3055">`dtu`.</span></span> <span data-ttu-id="69b8c-3056">Para atualizar, use o parâmetro `--capacity`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3056">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="69b8c-3057">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="69b8c-3057">`databaseDtuMin`.</span></span> <span data-ttu-id="69b8c-3058">Para atualizar, use o parâmetro `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3058">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="69b8c-3059">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="69b8c-3059">`databaseDtuMax`.</span></span> <span data-ttu-id="69b8c-3060">Para atualizar, use o parâmetro `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3060">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="69b8c-3061">Os parâmetros `--family` e `--capacity` foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="69b8c-3061">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="69b8c-3062">Os formatadores de tabela foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="69b8c-3062">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-3063">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-3063">Storage</span></span>

* <span data-ttu-id="69b8c-3064">Complemento adicionado ao argumento `--account-name`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3064">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="69b8c-3065">O problema com `storage entity query` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="69b8c-3065">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="69b8c-3066">VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-3066">VM</span></span>

* <span data-ttu-id="69b8c-3067">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="69b8c-3067">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="69b8c-3068">O mesmo suporte pode ser acessado por meio de `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3068">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="69b8c-3069">Imagem de extensão fixa correspondente em `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3069">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="69b8c-3070">`--boot-diagnostics-storage` foi adicionado a `vm create` para capturar o log de inicialização</span><span class="sxs-lookup"><span data-stu-id="69b8c-3070">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="69b8c-3071">`--license-type` foi adicionado a `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3071">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="69b8c-3072">7 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="69b8c-3072">May 7, 2018</span></span>

<span data-ttu-id="69b8c-3073">Versão 2.0.32</span><span class="sxs-lookup"><span data-stu-id="69b8c-3073">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="69b8c-3074">Núcleo</span><span class="sxs-lookup"><span data-stu-id="69b8c-3074">Core</span></span>

* <span data-ttu-id="69b8c-3075">Foi corrigida uma exceção sem tratamento ao recuperar segredos de uma conta de entidade de serviço com certificado</span><span class="sxs-lookup"><span data-stu-id="69b8c-3075">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="69b8c-3076">Adicionado suporte limitado para argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="69b8c-3076">Added limited support for positional arguments</span></span>
* <span data-ttu-id="69b8c-3077">Corrigir problema no qual `--query` não pôde ser usado com `--ids`.</span><span class="sxs-lookup"><span data-stu-id="69b8c-3077">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="69b8c-3078">#5591</span><span class="sxs-lookup"><span data-stu-id="69b8c-3078">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="69b8c-3079">Foram melhorados os cenários de redirecionamento de comandos ao usar `--ids`.</span><span class="sxs-lookup"><span data-stu-id="69b8c-3079">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="69b8c-3080">Oferece suporte a `-o tsv` com uma consulta especificada ou `-o json` sem especificar uma consulta</span><span class="sxs-lookup"><span data-stu-id="69b8c-3080">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="69b8c-3081">Foram adicionadas sugestões de comando sobre o erro se os usuários cometeram algum erro de digitação em seus comandos</span><span class="sxs-lookup"><span data-stu-id="69b8c-3081">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="69b8c-3082">Erro corrigido quando os usuários digitam `az ''`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3082">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="69b8c-3083">Foram adicionados tipos de recursos personalizados com suporte para módulos de comando e extensões</span><span class="sxs-lookup"><span data-stu-id="69b8c-3083">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-3084">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-3084">ACR</span></span>

* <span data-ttu-id="69b8c-3085">Foram adicionados comandos de compilação de ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-3085">Added ACR Build commands</span></span>
* <span data-ttu-id="69b8c-3086">O recurso aprimorado não encontrou mensagens de erro</span><span class="sxs-lookup"><span data-stu-id="69b8c-3086">Improved resource not found error messages</span></span>
* <span data-ttu-id="69b8c-3087">Desempenho de criação de recurso aprimorado e tratamento de erros</span><span class="sxs-lookup"><span data-stu-id="69b8c-3087">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="69b8c-3088">Logon de acr aprimorado em consoles não padrão e WSL</span><span class="sxs-lookup"><span data-stu-id="69b8c-3088">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="69b8c-3089">Mensagens de erro de comandos de repositório aprimoradas</span><span class="sxs-lookup"><span data-stu-id="69b8c-3089">Improved repository commands error messages</span></span>
* <span data-ttu-id="69b8c-3090">Colunas de tabela e ordenação atualizadas</span><span class="sxs-lookup"><span data-stu-id="69b8c-3090">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="69b8c-3091">ACS</span><span class="sxs-lookup"><span data-stu-id="69b8c-3091">ACS</span></span>

* <span data-ttu-id="69b8c-3092">Foi adicionado um aviso informando que `az aks` é um serviço de versão prévia</span><span class="sxs-lookup"><span data-stu-id="69b8c-3092">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="69b8c-3093">Foi corrigido um problema de permissão em `aks install-connector` quando `--aci-resource-group` não for especificado</span><span class="sxs-lookup"><span data-stu-id="69b8c-3093">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="69b8c-3094">AMS</span><span class="sxs-lookup"><span data-stu-id="69b8c-3094">AMS</span></span>

* <span data-ttu-id="69b8c-3095">Versão inicial — Gerenciar recursos dos Serviços de Mídia do Azure</span><span class="sxs-lookup"><span data-stu-id="69b8c-3095">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-3096">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-3096">Appservice</span></span>

* <span data-ttu-id="69b8c-3097">Correção de bug no `webapp delete` quando `--slot` é fornecido</span><span class="sxs-lookup"><span data-stu-id="69b8c-3097">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="69b8c-3098">`--runtime-version` foi removido de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3098">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="69b8c-3099">Foi adicionado suporte para min\_tls\_versão e https2.0</span><span class="sxs-lookup"><span data-stu-id="69b8c-3099">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="69b8c-3100">Suporte adicionado para vários contêineres</span><span class="sxs-lookup"><span data-stu-id="69b8c-3100">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="69b8c-3101">Lote AI</span><span class="sxs-lookup"><span data-stu-id="69b8c-3101">Batch AI</span></span>

* <span data-ttu-id="69b8c-3102">O `batchai create cluster` foi alterado para respeitar a prioridade de VM configurada no arquivo de configuração do cluster</span><span class="sxs-lookup"><span data-stu-id="69b8c-3102">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="69b8c-3103">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="69b8c-3103">Cognitive Services</span></span>

* <span data-ttu-id="69b8c-3104">Foi corrigido um erro de digitação no exemplo para `cognitiveservices account create`[#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="69b8c-3104">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="69b8c-3105">Consumo</span><span class="sxs-lookup"><span data-stu-id="69b8c-3105">Consumption</span></span>

* <span data-ttu-id="69b8c-3106">Foram adicionados novos comandos para a API de orçamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-3106">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="69b8c-3107">Contêiner</span><span class="sxs-lookup"><span data-stu-id="69b8c-3107">Container</span></span>

* <span data-ttu-id="69b8c-3108">Requisito removido para `--registry-server` e `container create` quando um servidor de registro estiver incluído no nome da imagem</span><span class="sxs-lookup"><span data-stu-id="69b8c-3108">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="69b8c-3109">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="69b8c-3109">Cosmos DB</span></span>

* <span data-ttu-id="69b8c-3110">Introdução ao suporte de rede virtual para a CLI do Azure — Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="69b8c-3110">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="69b8c-3111">DMS</span><span class="sxs-lookup"><span data-stu-id="69b8c-3111">DMS</span></span>

* <span data-ttu-id="69b8c-3112">Versão inicial — Adiciona suporte ao SQL para o cenário de migração do SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="69b8c-3112">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="69b8c-3113">Extensão</span><span class="sxs-lookup"><span data-stu-id="69b8c-3113">Extension</span></span>

* <span data-ttu-id="69b8c-3114">Correção do bug em que os metadados de extensão pararam de ser exibidos</span><span class="sxs-lookup"><span data-stu-id="69b8c-3114">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="69b8c-3115">Interativo</span><span class="sxs-lookup"><span data-stu-id="69b8c-3115">Interactive</span></span>

* <span data-ttu-id="69b8c-3116">Permitir que complementos interativos funcionem com argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="69b8c-3116">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="69b8c-3117">Resultado mais simplificado quando os usuários digitam '\'</span><span class="sxs-lookup"><span data-stu-id="69b8c-3117">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="69b8c-3118">Conclusões corrigidas para parâmetros sem ajuda</span><span class="sxs-lookup"><span data-stu-id="69b8c-3118">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="69b8c-3119">Descrições corrigidas para grupos de comando</span><span class="sxs-lookup"><span data-stu-id="69b8c-3119">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="69b8c-3120">Laboratório</span><span class="sxs-lookup"><span data-stu-id="69b8c-3120">Lab</span></span>

* <span data-ttu-id="69b8c-3121">Regressões corrigidas de conversão de aptidão</span><span class="sxs-lookup"><span data-stu-id="69b8c-3121">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-3122">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-3122">Network</span></span>

* <span data-ttu-id="69b8c-3123">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--ids` removido de:</span><span class="sxs-lookup"><span data-stu-id="69b8c-3123">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="69b8c-3124">Perfil</span><span class="sxs-lookup"><span data-stu-id="69b8c-3124">Profile</span></span>

* <span data-ttu-id="69b8c-3125">Detecção de origem do `disk create` corrigida</span><span class="sxs-lookup"><span data-stu-id="69b8c-3125">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="69b8c-3126">[ALTERAÇÃO SIGNIFICATIVA]`--msi-port` e `--identity-port` removidos porque não são mais usados</span><span class="sxs-lookup"><span data-stu-id="69b8c-3126">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="69b8c-3127">Erro de digitação corrigido no resumo do `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3127">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="69b8c-3128">Redis</span><span class="sxs-lookup"><span data-stu-id="69b8c-3128">Redis</span></span>

* <span data-ttu-id="69b8c-3129">`redis patch-schedule patch-schedule show` preterido em favor de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3129">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="69b8c-3130">`redis list-all` preterido.</span><span class="sxs-lookup"><span data-stu-id="69b8c-3130">Deprecated `redis list-all`.</span></span> <span data-ttu-id="69b8c-3131">Esta funcionalidade foi dobrada em `redis list`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3131">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="69b8c-3132">`redis import-method` preterido em favor de `redis import`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3132">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="69b8c-3133">Foi adicionado suporte a `--ids` para vários comandos</span><span class="sxs-lookup"><span data-stu-id="69b8c-3133">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="69b8c-3134">Função</span><span class="sxs-lookup"><span data-stu-id="69b8c-3134">Role</span></span>

* <span data-ttu-id="69b8c-3135">[ALTERAÇÃO SIGNIFICATIVA] Remoção de `ad sp reset-credentials` preterido</span><span class="sxs-lookup"><span data-stu-id="69b8c-3135">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-3136">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-3136">Storage</span></span>

* <span data-ttu-id="69b8c-3137">Permitir que o token SAS de destino aplique na origem a cópia do blob se a SAS de origem e a chave de conta não forem especificadas</span><span class="sxs-lookup"><span data-stu-id="69b8c-3137">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="69b8c-3138">Exposto -- tempo limite do soquete para carregamentos e downloads de blobs</span><span class="sxs-lookup"><span data-stu-id="69b8c-3138">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="69b8c-3139">Tratar os nomes de blobs que começam com separadores de caminho como caminhos relativos</span><span class="sxs-lookup"><span data-stu-id="69b8c-3139">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="69b8c-3140">Permitir `storage blob copy --source-sas` com a inicialização char de consulta, '?'</span><span class="sxs-lookup"><span data-stu-id="69b8c-3140">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="69b8c-3141">`storage entity query --marker` foi corrigido para aceitar a lista de chaves = valores</span><span class="sxs-lookup"><span data-stu-id="69b8c-3141">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="69b8c-3142">VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-3142">VM</span></span>

* <span data-ttu-id="69b8c-3143">Uma lógica de detecção inválida foi corrigida no URI do blob não gerenciado</span><span class="sxs-lookup"><span data-stu-id="69b8c-3143">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="69b8c-3144">Adicionada criptografia de disco de suporte sem entidades de serviço fornecidas pelo usuário</span><span class="sxs-lookup"><span data-stu-id="69b8c-3144">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="69b8c-3145">[ALTERAÇÃO SIGNIFICATIVA] Não usar a VM 'ManagedIdentityExtension' para suporte de MSI</span><span class="sxs-lookup"><span data-stu-id="69b8c-3145">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="69b8c-3146">Suporte adicionado para a política de remoção em `vmss`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3146">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="69b8c-3147">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--ids` de:</span><span class="sxs-lookup"><span data-stu-id="69b8c-3147">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="69b8c-3148">Foi adicionado suporte do acelerador de gravação</span><span class="sxs-lookup"><span data-stu-id="69b8c-3148">Added write accelerator support</span></span>
* <span data-ttu-id="69b8c-3149">Adicionado `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3149">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="69b8c-3150">`vm diagnostics set` foi corrigido para detectar o tipo de sistema operacional da VM de forma confiável</span><span class="sxs-lookup"><span data-stu-id="69b8c-3150">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="69b8c-3151">`vm resize` foi alterado para verificar se o tamanho solicitado é diferente daquele definido no momento e atualizar somente na alteração</span><span class="sxs-lookup"><span data-stu-id="69b8c-3151">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="69b8c-3152">10 de abril de 2018</span><span class="sxs-lookup"><span data-stu-id="69b8c-3152">April 10, 2018</span></span>

<span data-ttu-id="69b8c-3153">Versão 2.0.31</span><span class="sxs-lookup"><span data-stu-id="69b8c-3153">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-3154">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-3154">ACR</span></span>

* <span data-ttu-id="69b8c-3155">Melhoria do tratamento de erros do fallback do wincred</span><span class="sxs-lookup"><span data-stu-id="69b8c-3155">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="69b8c-3156">ACS</span><span class="sxs-lookup"><span data-stu-id="69b8c-3156">ACS</span></span>

* <span data-ttu-id="69b8c-3157">Alteração da validade de SPNs criados pelo AKS para 5 anos</span><span class="sxs-lookup"><span data-stu-id="69b8c-3157">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-3158">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-3158">Appservice</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="69b8c-3160">Correção da exceção não identificada de planos de webapp inexistentes</span><span class="sxs-lookup"><span data-stu-id="69b8c-3160">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="69b8c-3161">BatchAI</span><span class="sxs-lookup"><span data-stu-id="69b8c-3161">BatchAI</span></span>

* <span data-ttu-id="69b8c-3162">Adição de suporte para a API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="69b8c-3162">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="69b8c-3163">Montagem de nível de trabalho</span><span class="sxs-lookup"><span data-stu-id="69b8c-3163">Job level mounting</span></span>
  - <span data-ttu-id="69b8c-3164">Variáveis de ambiente com valores secretos</span><span class="sxs-lookup"><span data-stu-id="69b8c-3164">Environment variables with secret values</span></span>
  - <span data-ttu-id="69b8c-3165">Configurações de contadores de desempenho</span><span class="sxs-lookup"><span data-stu-id="69b8c-3165">Performance counters settings</span></span>
  - <span data-ttu-id="69b8c-3166">Relatório de segmento de linha específico de trabalho</span><span class="sxs-lookup"><span data-stu-id="69b8c-3166">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="69b8c-3167">Suporte para subpastas na API de arquivos de lista</span><span class="sxs-lookup"><span data-stu-id="69b8c-3167">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="69b8c-3168">Relatório de uso e limites</span><span class="sxs-lookup"><span data-stu-id="69b8c-3168">Usage and limits reporting</span></span>
  - <span data-ttu-id="69b8c-3169">Permitir a especificação do tipo de cache para servidores NFS</span><span class="sxs-lookup"><span data-stu-id="69b8c-3169">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="69b8c-3170">Suporte para imagens personalizadas</span><span class="sxs-lookup"><span data-stu-id="69b8c-3170">Support for custom images</span></span>
  - <span data-ttu-id="69b8c-3171">Adição de suporte para o kit de ferramentas pyTorch</span><span class="sxs-lookup"><span data-stu-id="69b8c-3171">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="69b8c-3172">Adição do comando `job wait`, que permite aguardar a conclusão do trabalho e relata o código de saída de trabalho</span><span class="sxs-lookup"><span data-stu-id="69b8c-3172">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="69b8c-3173">Adição do comando `usage show` para listar o uso e os limites do IA do Lote atual para diferentes regiões</span><span class="sxs-lookup"><span data-stu-id="69b8c-3173">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="69b8c-3174">Há suporte para nuvens nacionais</span><span class="sxs-lookup"><span data-stu-id="69b8c-3174">National clouds are supported</span></span>
* <span data-ttu-id="69b8c-3175">Adição de argumentos de linha de comando do trabalho para montar sistemas de arquivos no nível de trabalho, além de arquivos de configuração</span><span class="sxs-lookup"><span data-stu-id="69b8c-3175">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="69b8c-3176">Adição de mais opções para personalizar clusters — prioridade de VM, sub-rede, contagem inicial de nós para clusters de dimensionamento automático, especificando a imagem personalizada</span><span class="sxs-lookup"><span data-stu-id="69b8c-3176">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="69b8c-3177">Adição de opção de linha de comando para especificar o tipo de cache de NFS gerenciado por IA do Lote</span><span class="sxs-lookup"><span data-stu-id="69b8c-3177">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="69b8c-3178">Simplificação da especificação do sistema de arquivos de montagem nos arquivos de configuração.</span><span class="sxs-lookup"><span data-stu-id="69b8c-3178">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="69b8c-3179">Agora é possível omitir as credenciais do Compartilhamento de arquivos do Azure e Contêineres de Blob do Azure — a CLI preencherá credenciais ausentes usando a chave da conta de armazenamento fornecida por meio dos parâmetros de linha de comando ou especificada por meio da variável de ambiente ou consultará a chave a partir do Armazenamento do Azure (se a conta de armazenamento pertencer à assinatura atual)</span><span class="sxs-lookup"><span data-stu-id="69b8c-3179">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="69b8c-3180">O comando do fluxo de arquivo de trabalho agora é preenchido automaticamente quando o trabalho é concluído (com êxito, com falha, encerrado ou excluído)</span><span class="sxs-lookup"><span data-stu-id="69b8c-3180">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="69b8c-3181">Melhoria da saída de `table` para operações de `show`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3181">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="69b8c-3182">Adição da opção `--use-auto-storage` para a criação de cluster.</span><span class="sxs-lookup"><span data-stu-id="69b8c-3182">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="69b8c-3183">Essa opção simplifica o gerenciamento de contas de armazenamento e a montagem do Compartilhamento de arquivos do Azure e dos Contêineres de Blob do Azure para clusters</span><span class="sxs-lookup"><span data-stu-id="69b8c-3183">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="69b8c-3184">Adição da opção `--generate-ssh-keys` para `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3184">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="69b8c-3185">Adição da capacidade de fornecer a tarefa de configuração de nó por meio da linha de comando</span><span class="sxs-lookup"><span data-stu-id="69b8c-3185">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="69b8c-3186">[ALTERAÇÃO SIGNIFICATIVA] Comandos `job stream-file` e `job list-files` movidos para o grupo `job file`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3186">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="69b8c-3187">[ALTERAÇÃO SIGNIFICATIVA]`--admin-user-name` renomeado para `--user-name` no comando `file-server create` para ser consistente com o comando `cluster create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3187">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="69b8c-3188">Cobrança</span><span class="sxs-lookup"><span data-stu-id="69b8c-3188">Billing</span></span>

* <span data-ttu-id="69b8c-3189">Adição de comandos da conta de registro</span><span class="sxs-lookup"><span data-stu-id="69b8c-3189">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="69b8c-3190">Consumo</span><span class="sxs-lookup"><span data-stu-id="69b8c-3190">Consumption</span></span>

* <span data-ttu-id="69b8c-3191">Adicionados os comandos `marketplace`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3191">Added `marketplace` commands</span></span>
* <span data-ttu-id="69b8c-3192">[ALTERAÇÃO SIGNIFICATIVA]`reservations summaries` renomeado para `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3192">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="69b8c-3193">[ALTERAÇÃO SIGNIFICATIVA]`reservations details` renomeado para `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3193">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="69b8c-3194">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--reservation-order-id` e `--reservation-id` para os comandos `reservation`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3194">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="69b8c-3195">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--grain` para os comandos `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3195">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="69b8c-3196">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--include-meter-details` para os comandos `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3196">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="69b8c-3197">Contêiner</span><span class="sxs-lookup"><span data-stu-id="69b8c-3197">Container</span></span>

* <span data-ttu-id="69b8c-3198">Adição dos parâmetros de montagem de volume do Repositório Git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` e `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3198">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="69b8c-3199">Correção de [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` com falha com --container-name especificado</span><span class="sxs-lookup"><span data-stu-id="69b8c-3199">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="69b8c-3200">Extensão</span><span class="sxs-lookup"><span data-stu-id="69b8c-3200">Extension</span></span>

* <span data-ttu-id="69b8c-3201">Alteração da mensagem de verificação de distribuição para ser de nível de depuração</span><span class="sxs-lookup"><span data-stu-id="69b8c-3201">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="69b8c-3202">Interativo</span><span class="sxs-lookup"><span data-stu-id="69b8c-3202">Interactive</span></span>

* <span data-ttu-id="69b8c-3203">Alteração para interromper as conclusões após comandos não reconhecidos</span><span class="sxs-lookup"><span data-stu-id="69b8c-3203">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="69b8c-3204">Adição de ganchos de eventos antes e depois da criação da subárvore do comando</span><span class="sxs-lookup"><span data-stu-id="69b8c-3204">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="69b8c-3205">Adição de conclusão para parâmetros `--ids`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3205">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-3206">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-3206">Network</span></span>

* <span data-ttu-id="69b8c-3207">Correção de [#5936](https://github.com/Azure/azure-cli/issues/5936): as marcas `application-gateway create` não podiam ser definidas</span><span class="sxs-lookup"><span data-stu-id="69b8c-3207">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="69b8c-3208">Adição do argumento `--auth-certs` para anexar certificados de autenticação para `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="69b8c-3208">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="69b8c-3209">#4910</span><span class="sxs-lookup"><span data-stu-id="69b8c-3209">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="69b8c-3210">Adição dos comandos `ddos-protection` para criar planos de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="69b8c-3210">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="69b8c-3211">Adição de suporte de `--ddos-protection-plan` a `vnet [create|update]` para associar uma VNET a um plano de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="69b8c-3211">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="69b8c-3212">Correção do problema com o sinalizador `--disable-bgp-route-propagation` em `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3212">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="69b8c-3213">Remoção de argumentos fictícios `--public-ip-address-type` e `--subnet-type` para `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3213">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="69b8c-3214">Adição de suporte para registros TXT com sequências de escape RFC 1035 para `network dns zone [import|export]` e `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3214">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="69b8c-3215">Perfil</span><span class="sxs-lookup"><span data-stu-id="69b8c-3215">Profile</span></span>

* <span data-ttu-id="69b8c-3216">Adição de suporte para contas clássicas do Azure em `account list`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3216">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="69b8c-3217">[ALTERAÇÃO SIGNIFICATIVA] Remoção dos argumentos `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3217">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="69b8c-3218">RDBMS</span><span class="sxs-lookup"><span data-stu-id="69b8c-3218">RDBMS</span></span>

* <span data-ttu-id="69b8c-3219">Adicionado o comando `georestore`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3219">Added `georestore` command</span></span>
* <span data-ttu-id="69b8c-3220">Remoção da restrição de tamanho de armazenamento do comando `create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3220">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="69b8c-3221">Recurso</span><span class="sxs-lookup"><span data-stu-id="69b8c-3221">Resource</span></span>

* <span data-ttu-id="69b8c-3222">Adicionado o suporte ao `--metadata` para `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3222">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="69b8c-3223">Adição de suporte para `--metadata`, `--set`, `--add`, `--remove` para `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3223">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="69b8c-3224">SQL</span><span class="sxs-lookup"><span data-stu-id="69b8c-3224">SQL</span></span>

* <span data-ttu-id="69b8c-3225">Adição de `sql elastic-pool op list` e `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3225">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-3226">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-3226">Storage</span></span>

* <span data-ttu-id="69b8c-3227">Melhoria de mensagens de erro para cadeias de conexão malformadas</span><span class="sxs-lookup"><span data-stu-id="69b8c-3227">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="69b8c-3228">VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-3228">VM</span></span>

* <span data-ttu-id="69b8c-3229">Adição de suporte para configurar a contagem de domínios de falha da plataforma para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3229">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="69b8c-3230">Alteração de `vmss create` para balanceador de carga padrão para um conjunto de dimensionamento desabilitado zonal, grande ou de único grupo de posicionamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-3230">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [ALTERAÇÃO SIGNIFICATIVA]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="69b8c-3232">Adição de suporte para a SKU de IP público para `vm create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3232">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="69b8c-3233">Adição dos argumentos `--keyvault` e `--resource-group` para `vm secret format` para oferecer suporte a cenários em que o comando não é capaz de resolver a ID do cofre.</span><span class="sxs-lookup"><span data-stu-id="69b8c-3233">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="69b8c-3234">#5718</span><span class="sxs-lookup"><span data-stu-id="69b8c-3234">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="69b8c-3235">Melhoria de erros de `[vm|vmss create]` quando um local do grupo de recursos não tem suporte de zona</span><span class="sxs-lookup"><span data-stu-id="69b8c-3235">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="69b8c-3236">27 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="69b8c-3236">March 27, 2018</span></span>

<span data-ttu-id="69b8c-3237">Versão 2.0.30</span><span class="sxs-lookup"><span data-stu-id="69b8c-3237">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="69b8c-3238">Núcleo</span><span class="sxs-lookup"><span data-stu-id="69b8c-3238">Core</span></span>

* <span data-ttu-id="69b8c-3239">Mostrar mensagem para extensões marcadas como versão prévia na Ajuda</span><span class="sxs-lookup"><span data-stu-id="69b8c-3239">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="69b8c-3240">ACS</span><span class="sxs-lookup"><span data-stu-id="69b8c-3240">ACS</span></span>

* <span data-ttu-id="69b8c-3241">Corrija o erro de verificação de certificado SSL para `aks install-cli` no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="69b8c-3241">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-3242">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-3242">Appservice</span></span>

* <span data-ttu-id="69b8c-3243">Adição do suporte somente para HTTPS para `webapp update`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3243">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="69b8c-3244">Adição do suporte para os slots `az webapp identity [assign|show]` e `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3244">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="69b8c-3245">Backup</span><span class="sxs-lookup"><span data-stu-id="69b8c-3245">Backup</span></span>

* <span data-ttu-id="69b8c-3246">Adição do novo comando `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="69b8c-3246">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="69b8c-3247">Esse comando pode ser usado para verificar se o backup de uma VM é realizado por qualquer cofre na assinatura</span><span class="sxs-lookup"><span data-stu-id="69b8c-3247">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="69b8c-3248">Habilitação das IDs de objeto do Azure para os parâmetros `--resource-group` e `--vault-name` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="69b8c-3248">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="69b8c-3249">`--name` parâmetros alterados a fim de aceitar o formato de saída dos comandos `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3249">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="69b8c-3250">Contêiner</span><span class="sxs-lookup"><span data-stu-id="69b8c-3250">Container</span></span>

* <span data-ttu-id="69b8c-3251">Adição do comando `container exec`.</span><span class="sxs-lookup"><span data-stu-id="69b8c-3251">Added `container exec` command.</span></span> <span data-ttu-id="69b8c-3252">Executa comandos em um contêiner para um grupo de contêiner em execução</span><span class="sxs-lookup"><span data-stu-id="69b8c-3252">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="69b8c-3253">Permitir a saída da tabela para criar e atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="69b8c-3253">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="69b8c-3254">Extensão</span><span class="sxs-lookup"><span data-stu-id="69b8c-3254">Extension</span></span>

* <span data-ttu-id="69b8c-3255">Mensagem adicionada para `extension add`, se a extensão estiver no modo de versão prévia</span><span class="sxs-lookup"><span data-stu-id="69b8c-3255">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="69b8c-3256">`extension list-available` alterado para mostrar dados de extensão total com `--show-details`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3256">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="69b8c-3257">[ALTERAÇÃO SIGNIFICATIVA]`extension list-available` alterado para mostrar dados de extensão simplificados por padrão</span><span class="sxs-lookup"><span data-stu-id="69b8c-3257">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="69b8c-3258">Interativo</span><span class="sxs-lookup"><span data-stu-id="69b8c-3258">Interactive</span></span>

* <span data-ttu-id="69b8c-3259">Alteração nas conclusões para ativar após a conclusão do carregamento da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="69b8c-3259">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="69b8c-3260">Correção de bug usando o parâmetro `--style`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3260">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="69b8c-3261">Analisador léxico interativo instanciado após a falta do despejo da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="69b8c-3261">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="69b8c-3262">Suporte aprimorado ao completador</span><span class="sxs-lookup"><span data-stu-id="69b8c-3262">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="69b8c-3263">Laboratório</span><span class="sxs-lookup"><span data-stu-id="69b8c-3263">Lab</span></span>

* <span data-ttu-id="69b8c-3264">Correção de bugs com o comando `create environment`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3264">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="69b8c-3265">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="69b8c-3265">Monitor</span></span>

* <span data-ttu-id="69b8c-3266">Adicionado suporte para `--top`, `--orderby` e `--namespace` para `metrics list` [nº5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="69b8c-3266">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="69b8c-3267">Corrigido [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` aceita uma lista separada por espaços de métricas para recuperação</span><span class="sxs-lookup"><span data-stu-id="69b8c-3267">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="69b8c-3268">Suporte adicionado para `--namespace` a `metrics list-definitions` [nº5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="69b8c-3268">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-3269">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-3269">Network</span></span>

* <span data-ttu-id="69b8c-3270">Adição de suporte para zonas DNS privado</span><span class="sxs-lookup"><span data-stu-id="69b8c-3270">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="69b8c-3271">Perfil</span><span class="sxs-lookup"><span data-stu-id="69b8c-3271">Profile</span></span>

* <span data-ttu-id="69b8c-3272">Adição de avisos para `--identity-port` e `--msi-port` para `login`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3272">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="69b8c-3273">RDBMS</span><span class="sxs-lookup"><span data-stu-id="69b8c-3273">RDBMS</span></span>

* <span data-ttu-id="69b8c-3274">Adição de modelo de negócios GA API versão 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="69b8c-3274">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="69b8c-3275">Recurso</span><span class="sxs-lookup"><span data-stu-id="69b8c-3275">Resource</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="69b8c-3277">Função</span><span class="sxs-lookup"><span data-stu-id="69b8c-3277">Role</span></span>

* <span data-ttu-id="69b8c-3278">Adição de suporte para configurações de acesso necessário e clientes nativos para `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3278">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="69b8c-3279">`rbac` comandos alterados para retornar menos de 1000 IDs na resolução do objeto</span><span class="sxs-lookup"><span data-stu-id="69b8c-3279">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="69b8c-3280">Adição de comandos de gerenciamento de credencial `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3280">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="69b8c-3281">[ALTERAÇÃO SIGNIFICATIVA] "Propriedades" removidas da saída `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3281">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="69b8c-3282">Adição de suporte para as permissões `dataActions` e `notDataActions` para `role definition`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3282">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-3283">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-3283">Storage</span></span>

* <span data-ttu-id="69b8c-3284">Correção de problema ao carregar um arquivo com tamanho entre 195 e 200 GB</span><span class="sxs-lookup"><span data-stu-id="69b8c-3284">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="69b8c-3285">Corrigido [#4049](https://github.com/Azure/azure-cli/issues/4049): problemas com o acréscimo de uploads de blob ignorando os parâmetros da condição</span><span class="sxs-lookup"><span data-stu-id="69b8c-3285">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="69b8c-3286">VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-3286">VM</span></span>

* <span data-ttu-id="69b8c-3287">Adição de aviso para `vmss create` para alterações de falha futuras para conjuntos com mais de 100 instâncias</span><span class="sxs-lookup"><span data-stu-id="69b8c-3287">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="69b8c-3288">Adição de suporte com flexibilidade de região para `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3288">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="69b8c-3289">Alteração no modo de exibição de instância de disco para reportar status de criptografia mais adequados</span><span class="sxs-lookup"><span data-stu-id="69b8c-3289">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="69b8c-3290">[ALTERAÇÃO SIGNIFICATIVA]`vm extension delete` alterado para não retornar mais a saída</span><span class="sxs-lookup"><span data-stu-id="69b8c-3290">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="69b8c-3291">13 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="69b8c-3291">March 13, 2018</span></span>

<span data-ttu-id="69b8c-3292">Versão 2.0.29</span><span class="sxs-lookup"><span data-stu-id="69b8c-3292">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-3293">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-3293">ACR</span></span>

* <span data-ttu-id="69b8c-3294">Suporte adicionado do parâmetro `--image` a `repository delete`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3294">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="69b8c-3295">Parâmetros `--manifest` e `--tag` preteridos do comando `repository delete`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3295">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="69b8c-3296">Comando `repository untag` adicionado para remover uma marcação sem excluir dados</span><span class="sxs-lookup"><span data-stu-id="69b8c-3296">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="69b8c-3297">ACS</span><span class="sxs-lookup"><span data-stu-id="69b8c-3297">ACS</span></span>

* <span data-ttu-id="69b8c-3298">Comando `aks upgrade-connector` adicionado para atualizar um conector existente</span><span class="sxs-lookup"><span data-stu-id="69b8c-3298">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="69b8c-3299">Arquivos de configuração `kubectl` alterados para usar um YAML mais legível em bloco</span><span class="sxs-lookup"><span data-stu-id="69b8c-3299">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="69b8c-3300">Supervisor</span><span class="sxs-lookup"><span data-stu-id="69b8c-3300">Advisor</span></span>

* <span data-ttu-id="69b8c-3301">[ALTERAÇÃO SIGNIFICATIVA]`advisor configuration get` renomeado para `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3301">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="69b8c-3302">[ALTERAÇÃO SIGNIFICATIVA]`advisor configuration set` renomeado para `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3302">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="69b8c-3303">[ALTERAÇÃO SIGNIFICATIVA]`advisor recommendation generate` removido</span><span class="sxs-lookup"><span data-stu-id="69b8c-3303">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="69b8c-3304">Parâmetro `--refresh` adicionado a `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3304">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="69b8c-3305">Adicionado o comando `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3305">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-3306">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-3306">Appservice</span></span>

* <span data-ttu-id="69b8c-3307">Preterido `[webapp|functionapp] assign-identity`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3307">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="69b8c-3308">Comandos de identidade gerenciada `webapp identity [assign|show]` e `functionapp identity [assign|show]` adicionados</span><span class="sxs-lookup"><span data-stu-id="69b8c-3308">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="69b8c-3309">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="69b8c-3309">Eventhubs</span></span>

* <span data-ttu-id="69b8c-3310">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="69b8c-3310">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="69b8c-3311">Extensão</span><span class="sxs-lookup"><span data-stu-id="69b8c-3311">Extension</span></span>

* <span data-ttu-id="69b8c-3312">Verificação adicionada para avisar ao usuário se a distribuição usada é diferente da armazenado no arquivo de origem do pacote, pois isso pode levar a erros</span><span class="sxs-lookup"><span data-stu-id="69b8c-3312">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="69b8c-3313">Interativo</span><span class="sxs-lookup"><span data-stu-id="69b8c-3313">Interactive</span></span>

* <span data-ttu-id="69b8c-3314">Corrigido [#5625](https://github.com/Azure/azure-cli/issues/5625): manter histórico em sessões diferentes</span><span class="sxs-lookup"><span data-stu-id="69b8c-3314">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="69b8c-3315">Corrigido [#3016](https://github.com/Azure/azure-cli/issues/3016): histórico não registrado no escopo</span><span class="sxs-lookup"><span data-stu-id="69b8c-3315">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="69b8c-3316">Corrigido [#5688](https://github.com/Azure/azure-cli/issues/5688): as conclusões não aparecerão se o carregamento da tabela de comando encontrar uma exceção</span><span class="sxs-lookup"><span data-stu-id="69b8c-3316">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="69b8c-3317">Medidor de progresso corrigido para operações de longa execução</span><span class="sxs-lookup"><span data-stu-id="69b8c-3317">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="69b8c-3318">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="69b8c-3318">Monitor</span></span>

* <span data-ttu-id="69b8c-3319">Comandos `monitor autoscale-settings` preteridos</span><span class="sxs-lookup"><span data-stu-id="69b8c-3319">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="69b8c-3320">Adicionados os comandos `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3320">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="69b8c-3321">Adicionados os comandos `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3321">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="69b8c-3322">Adicionados os comandos `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3322">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-3323">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-3323">Network</span></span>

* <span data-ttu-id="69b8c-3324">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--tags` removido de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3324">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="69b8c-3325">Valores padrão incorretos removidos dos seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="69b8c-3325">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="69b8c-3326">Comandos `network watcher connection-monitor` adicionados</span><span class="sxs-lookup"><span data-stu-id="69b8c-3326">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="69b8c-3327">Parâmetros `--vnet` e `--subnet` adicionados a `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3327">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="69b8c-3328">Perfil</span><span class="sxs-lookup"><span data-stu-id="69b8c-3328">Profile</span></span>

* <span data-ttu-id="69b8c-3329">Parâmetro `--msi` preterido de `az login`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3329">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="69b8c-3330">Parâmetro `--identity` adicionado de `az login` para substituir `--msi`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3330">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="69b8c-3331">RDBMS</span><span class="sxs-lookup"><span data-stu-id="69b8c-3331">RDBMS</span></span>

* <span data-ttu-id="69b8c-3332">[VISUALIZAÇÃO] Alterado para usar a API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="69b8c-3332">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="69b8c-3333">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="69b8c-3333">Service Bus</span></span>

* <span data-ttu-id="69b8c-3334">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="69b8c-3334">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-3335">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-3335">Storage</span></span>

* <span data-ttu-id="69b8c-3336">[#4971](https://github.com/Azure/azure-cli/issues/4971) corrigido: `storage blob copy` agora dá suporte a outras nuvens do Azure</span><span class="sxs-lookup"><span data-stu-id="69b8c-3336">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="69b8c-3337">Corrigido [#5286](https://github.com/Azure/azure-cli/issues/5286): os comandos em lotes `storage blob [delete-batch|download-batch|upload-batch]` não geram mais um erro após falhas da pré-condição</span><span class="sxs-lookup"><span data-stu-id="69b8c-3337">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="69b8c-3338">VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-3338">VM</span></span>

* <span data-ttu-id="69b8c-3339">Suporte adicionado a `[vm|vmss] create` anexar discos de dados não gerenciados e configurar o cache</span><span class="sxs-lookup"><span data-stu-id="69b8c-3339">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="69b8c-3340">`[vm|vmss] assign-identity` e `[vm|vmss] remove-identity` preteridos</span><span class="sxs-lookup"><span data-stu-id="69b8c-3340">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="69b8c-3341">Comandos `vm identity [assign|remove|show]` e `vmss identity [assign|remove|show]` adicionados para substituir comandos preteridos</span><span class="sxs-lookup"><span data-stu-id="69b8c-3341">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="69b8c-3342">Prioridade padrão alterada em `vmss create` para None</span><span class="sxs-lookup"><span data-stu-id="69b8c-3342">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="69b8c-3343">27 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="69b8c-3343">February 27, 2018</span></span>

<span data-ttu-id="69b8c-3344">Versão 2.0.28</span><span class="sxs-lookup"><span data-stu-id="69b8c-3344">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="69b8c-3345">Núcleo</span><span class="sxs-lookup"><span data-stu-id="69b8c-3345">Core</span></span>

* <span data-ttu-id="69b8c-3346">Corrigido [#5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="69b8c-3346">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="69b8c-3347">Adição de suporte para telemetria de extensão com chaves personalizadas</span><span class="sxs-lookup"><span data-stu-id="69b8c-3347">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="69b8c-3348">Adição de log HTTP em `--debug`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3348">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="69b8c-3349">ACS</span><span class="sxs-lookup"><span data-stu-id="69b8c-3349">ACS</span></span>

* <span data-ttu-id="69b8c-3350">Alteração para usa o gráfico `virtual-kubelet-for-aks` do Helm para `aks install-connector` por padrão</span><span class="sxs-lookup"><span data-stu-id="69b8c-3350">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="69b8c-3351">Problema corrigido: permissão insuficiente para entidades de serviço criarem um grupo de contêiner ACI</span><span class="sxs-lookup"><span data-stu-id="69b8c-3351">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="69b8c-3352">Adição dos parâmetros `--aci-container-group`, `--location` e `--image-tag` ao `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3352">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="69b8c-3353">Remoção do aviso de reprovação de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3353">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-3354">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-3354">Appservice</span></span>

* <span data-ttu-id="69b8c-3355">Atualizações para a nova versão do SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="69b8c-3355">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="69b8c-3356">Correção [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` relatado como SKU inválido</span><span class="sxs-lookup"><span data-stu-id="69b8c-3356">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="69b8c-3357">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="69b8c-3357">Cognitive Services</span></span>

* <span data-ttu-id="69b8c-3358">Atualização do “aviso” ao criar uma nova conta dos Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="69b8c-3358">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="69b8c-3359">Consumo</span><span class="sxs-lookup"><span data-stu-id="69b8c-3359">Consumption</span></span>

* <span data-ttu-id="69b8c-3360">Adição de novos comandos para a API pricesheet</span><span class="sxs-lookup"><span data-stu-id="69b8c-3360">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="69b8c-3361">Atualização dos formatos existentes de Detalhes de uso e Detalhes de reserva</span><span class="sxs-lookup"><span data-stu-id="69b8c-3361">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="69b8c-3362">Contêiner</span><span class="sxs-lookup"><span data-stu-id="69b8c-3362">Container</span></span>

* <span data-ttu-id="69b8c-3363">Adição dos argumentos `--secrets` e `--secrets-mount-path` ao `container create` para usar segredos na ACI</span><span class="sxs-lookup"><span data-stu-id="69b8c-3363">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-3364">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-3364">Network</span></span>

* <span data-ttu-id="69b8c-3365">Corrigido [#5559](https://github.com/Azure/azure-cli/issues/5559): cliente ausente em `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3365">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="69b8c-3366">Recurso</span><span class="sxs-lookup"><span data-stu-id="69b8c-3366">Resource</span></span>

* <span data-ttu-id="69b8c-3367">Alteração do `group deployment export` para exibir um modelo parcial e erros ao falhar</span><span class="sxs-lookup"><span data-stu-id="69b8c-3367">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="69b8c-3368">Função</span><span class="sxs-lookup"><span data-stu-id="69b8c-3368">Role</span></span>

* <span data-ttu-id="69b8c-3369">Adição de `role assignment list-changelogs` para permitir a auditoria das funções da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="69b8c-3369">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="69b8c-3370">SQL</span><span class="sxs-lookup"><span data-stu-id="69b8c-3370">SQL</span></span>

* <span data-ttu-id="69b8c-3371">Adição de suporte para a redundância de zona para os bancos de dados e pools elásticos em criação ou atualização</span><span class="sxs-lookup"><span data-stu-id="69b8c-3371">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-3372">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-3372">Storage</span></span>

* <span data-ttu-id="69b8c-3373">Habilitação de especificação de caminho de destino/prefixo do `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3373">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="69b8c-3374">VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-3374">VM</span></span>

* <span data-ttu-id="69b8c-3375">Adição de suporte para anexar/desanexar discos em uma instância única de VMSS</span><span class="sxs-lookup"><span data-stu-id="69b8c-3375">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="69b8c-3376">13 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="69b8c-3376">February 13, 2018</span></span>

<span data-ttu-id="69b8c-3377">Versão 2.0.27</span><span class="sxs-lookup"><span data-stu-id="69b8c-3377">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="69b8c-3378">Núcleo</span><span class="sxs-lookup"><span data-stu-id="69b8c-3378">Core</span></span>

* <span data-ttu-id="69b8c-3379">Alterada a autenticação para chave tanto na ID de assinatura quanto no nome de logon do MSI</span><span class="sxs-lookup"><span data-stu-id="69b8c-3379">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="69b8c-3380">ACS</span><span class="sxs-lookup"><span data-stu-id="69b8c-3380">ACS</span></span>

* <span data-ttu-id="69b8c-3381">[ALTERAÇÃO SIGNIFICATIVA]`aks get-versions` renomeado para `aks get-upgrades` para fins de precisão</span><span class="sxs-lookup"><span data-stu-id="69b8c-3381">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="69b8c-3382">`aks get-versions` alterado para mostrar versões do Kubernetes disponíveis para `aks create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3382">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="69b8c-3383">Alterados os padrões de `aks create` para permitir que o servidor escolha a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="69b8c-3383">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="69b8c-3384">Atualizadas as mensagens de ajuda sobre a entidade de serviço gerada pelo AKS</span><span class="sxs-lookup"><span data-stu-id="69b8c-3384">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="69b8c-3385">Alterados os tamanhos de nó padrão para `aks create` de “Standard\_D1\_v2” para “Standard\_DS1\_v2”</span><span class="sxs-lookup"><span data-stu-id="69b8c-3385">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="69b8c-3386">Aumentada a confiabilidade ao localizar o pod de painel para `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3386">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="69b8c-3387">`aks get-credentials` corrigido para tratar de erros de Unicode ao carregar arquivos de configuração do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="69b8c-3387">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="69b8c-3388">Adicionada uma mensagem para `az aks install-cli` para ajudar a obter `kubectl` em `$PATH`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3388">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-3389">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-3389">Appservice</span></span>

* <span data-ttu-id="69b8c-3390">Corrigido o problema em que `webapp [backup|restore]` falhou devido a uma referência nula</span><span class="sxs-lookup"><span data-stu-id="69b8c-3390">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="69b8c-3391">Adicionado suporte para planos de serviço de aplicativo padrão por meio de `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3391">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="69b8c-3392">CDN</span><span class="sxs-lookup"><span data-stu-id="69b8c-3392">CDN</span></span>

* <span data-ttu-id="69b8c-3393">Adicionados os comandos `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3393">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="69b8c-3394">Contêiner</span><span class="sxs-lookup"><span data-stu-id="69b8c-3394">Container</span></span>

* <span data-ttu-id="69b8c-3395">Adicionada a opção `--follow` para `az container logs` para logs de streaming</span><span class="sxs-lookup"><span data-stu-id="69b8c-3395">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="69b8c-3396">Adicionado o comando `container attach` que anexa fluxos locais de saída e erro padrão para um contêiner em um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="69b8c-3396">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="69b8c-3397">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="69b8c-3397">CosmosDB</span></span>

* <span data-ttu-id="69b8c-3398">Adicionado suporte para a configuração de recursos</span><span class="sxs-lookup"><span data-stu-id="69b8c-3398">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="69b8c-3399">Extensão</span><span class="sxs-lookup"><span data-stu-id="69b8c-3399">Extension</span></span>

* <span data-ttu-id="69b8c-3400">Adicionado suporte para parâmetro `--pip-proxy` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3400">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="69b8c-3401">Adicionado suporte para argumento `--pip-extra-index-urls` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3401">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="69b8c-3402">Comentários</span><span class="sxs-lookup"><span data-stu-id="69b8c-3402">Feedback</span></span>

* <span data-ttu-id="69b8c-3403">Adicionadas informações de extensão aos dados de telemetria</span><span class="sxs-lookup"><span data-stu-id="69b8c-3403">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="69b8c-3404">Interativo</span><span class="sxs-lookup"><span data-stu-id="69b8c-3404">Interactive</span></span>

* <span data-ttu-id="69b8c-3405">Corrigido o problema em que o usuário é solicitado a fazer logon ao usar o modo interativo no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="69b8c-3405">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="69b8c-3406">Corrigida a regressão com conclusões de parâmetro ausentes</span><span class="sxs-lookup"><span data-stu-id="69b8c-3406">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="69b8c-3407">IoT</span><span class="sxs-lookup"><span data-stu-id="69b8c-3407">IoT</span></span>

* <span data-ttu-id="69b8c-3408">Correção do problema em que `iot dps access policy [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="69b8c-3408">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="69b8c-3409">Correção do problema em que `iot dps linked-hub [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="69b8c-3409">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="69b8c-3410">Adicionado o suporte `--no-wait` para `iot dps access policy [create|update]` e `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3410">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="69b8c-3411">`iot hub create` alterado para permitir a especificação do número de partições</span><span class="sxs-lookup"><span data-stu-id="69b8c-3411">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="69b8c-3412">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="69b8c-3412">Monitor</span></span>

* <span data-ttu-id="69b8c-3413">Corrigido o comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3413">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-3414">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-3414">Network</span></span>

* <span data-ttu-id="69b8c-3415">Corrigida a opção `--tags` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="69b8c-3415">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="69b8c-3416">Perfil</span><span class="sxs-lookup"><span data-stu-id="69b8c-3416">Profile</span></span>

* <span data-ttu-id="69b8c-3417">`az login` habilitado no modo interativo</span><span class="sxs-lookup"><span data-stu-id="69b8c-3417">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="69b8c-3418">Recurso</span><span class="sxs-lookup"><span data-stu-id="69b8c-3418">Resource</span></span>

* <span data-ttu-id="69b8c-3419">`feature show` adicionado novamente</span><span class="sxs-lookup"><span data-stu-id="69b8c-3419">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="69b8c-3420">Função</span><span class="sxs-lookup"><span data-stu-id="69b8c-3420">Role</span></span>

* <span data-ttu-id="69b8c-3421">Adicionado o argumento `--available-to-other-tenants` para `ad app update`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3421">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="69b8c-3422">SQL</span><span class="sxs-lookup"><span data-stu-id="69b8c-3422">SQL</span></span>

* <span data-ttu-id="69b8c-3423">Adicionados os comandos `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3423">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="69b8c-3424">Adicionado `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3424">Added `sql db rename`</span></span>
* <span data-ttu-id="69b8c-3425">Adicionado suporte para o argumento `--ids` para todos os comandos sql</span><span class="sxs-lookup"><span data-stu-id="69b8c-3425">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-3426">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-3426">Storage</span></span>

* <span data-ttu-id="69b8c-3427">Adicionados os comandos `storage blob service-properties delete-policy` e `storage blob undelete` para habilitar a exclusão reversível</span><span class="sxs-lookup"><span data-stu-id="69b8c-3427">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="69b8c-3428">VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-3428">VM</span></span>

* <span data-ttu-id="69b8c-3429">Corrigida uma falha quando a criptografia de VM não pode ser totalmente inicializada</span><span class="sxs-lookup"><span data-stu-id="69b8c-3429">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="69b8c-3430">Adicionada saída de ID de entidade de segurança ao habilitar o MSI</span><span class="sxs-lookup"><span data-stu-id="69b8c-3430">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="69b8c-3431">`vm boot-diagnostics get-boot-log` fixo</span><span class="sxs-lookup"><span data-stu-id="69b8c-3431">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="69b8c-3432">31 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="69b8c-3432">January 31, 2018</span></span>

<span data-ttu-id="69b8c-3433">Versão 2.0.26</span><span class="sxs-lookup"><span data-stu-id="69b8c-3433">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="69b8c-3434">Núcleo</span><span class="sxs-lookup"><span data-stu-id="69b8c-3434">Core</span></span>

* <span data-ttu-id="69b8c-3435">Adicionado suporte para recuperação de token bruto no contexto MSI</span><span class="sxs-lookup"><span data-stu-id="69b8c-3435">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="69b8c-3436">Removida a cadeia de caracteres do indicador de sondagem depois de terminar o LRO no Windows cmd.exe</span><span class="sxs-lookup"><span data-stu-id="69b8c-3436">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="69b8c-3437">Adicionado um aviso que aparece ao usar um padrão configurado que foi alterado para uma entrada de nível de informações.</span><span class="sxs-lookup"><span data-stu-id="69b8c-3437">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="69b8c-3438">Usar `--verbose` para ver</span><span class="sxs-lookup"><span data-stu-id="69b8c-3438">Use `--verbose` to see</span></span>
* <span data-ttu-id="69b8c-3439">Adicionar um indicador de progresso para comandos de espera</span><span class="sxs-lookup"><span data-stu-id="69b8c-3439">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="69b8c-3440">ACS</span><span class="sxs-lookup"><span data-stu-id="69b8c-3440">ACS</span></span>

* <span data-ttu-id="69b8c-3441">Argumento `--disable-browser` esclarecido</span><span class="sxs-lookup"><span data-stu-id="69b8c-3441">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="69b8c-3442">Preenchimento de guia melhorado para argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3442">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-3443">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-3443">Appservice</span></span>

* <span data-ttu-id="69b8c-3444">`webapp log [tail|download]` fixo</span><span class="sxs-lookup"><span data-stu-id="69b8c-3444">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="69b8c-3445">Removida a verificação de `kind` em aplicativos Web e funções</span><span class="sxs-lookup"><span data-stu-id="69b8c-3445">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="69b8c-3446">CDN</span><span class="sxs-lookup"><span data-stu-id="69b8c-3446">CDN</span></span>

* <span data-ttu-id="69b8c-3447">Corrigido o problema de cliente ausente com `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3447">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="69b8c-3448">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="69b8c-3448">CosmosDB</span></span>

* <span data-ttu-id="69b8c-3449">Corrigida a descrição do parâmetro para políticas de failover</span><span class="sxs-lookup"><span data-stu-id="69b8c-3449">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="69b8c-3450">Interativo</span><span class="sxs-lookup"><span data-stu-id="69b8c-3450">Interactive</span></span>

* <span data-ttu-id="69b8c-3451">Corrigido o problema em que as conclusões de opção de comando não aparecem mais</span><span class="sxs-lookup"><span data-stu-id="69b8c-3451">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-3452">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-3452">Network</span></span>

* <span data-ttu-id="69b8c-3453">Adicionada a proteção para `--cert-password` para `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3453">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="69b8c-3454">Corrigido o problema com `application-gateway update` em que `--sku` aplicou um valor padrão de forma errada</span><span class="sxs-lookup"><span data-stu-id="69b8c-3454">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="69b8c-3455">Adicionada proteção para `--shared-key` e `--authorization-key` para `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3455">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="69b8c-3456">Corrigido o problema de cliente ausente com `asg create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3456">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="69b8c-3457">Adicionado o parâmetro `--file-name / -f` para nomes exportados para `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3457">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="69b8c-3458">Os seguintes problemas foram corrigidos com `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="69b8c-3458">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="69b8c-3459">Corrigido o problema em que registros TXT longos foram exportados incorretamente</span><span class="sxs-lookup"><span data-stu-id="69b8c-3459">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="69b8c-3460">Corrigido o problema em que registros TXT entre aspas foram exportados incorretamente sem as aspas com caracteres de escape</span><span class="sxs-lookup"><span data-stu-id="69b8c-3460">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="69b8c-3461">Corrigido o problema em que determinados registros foram importados duas vezes com `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3461">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="69b8c-3462">Restaurados os comandos `vnet-gateway root-cert` e `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3462">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="69b8c-3463">Perfil</span><span class="sxs-lookup"><span data-stu-id="69b8c-3463">Profile</span></span>

* <span data-ttu-id="69b8c-3464">`get-access-token` corrigido para trabalhar em uma VM com identidade</span><span class="sxs-lookup"><span data-stu-id="69b8c-3464">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="69b8c-3465">Recurso</span><span class="sxs-lookup"><span data-stu-id="69b8c-3465">Resource</span></span>

* <span data-ttu-id="69b8c-3466">Corrigido o bug com `deployment [create|validate]` em que um aviso era exibido incorretamente quando um campo ‘tipo’ do modelo continha valores maiúsculos</span><span class="sxs-lookup"><span data-stu-id="69b8c-3466">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-3467">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-3467">Storage</span></span>

* <span data-ttu-id="69b8c-3468">Corrigido o problema com a migração de contas de Armazenamento V1 para Armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="69b8c-3468">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="69b8c-3469">Adicionado o relatório de andamento de todos os comandos de upload/download</span><span class="sxs-lookup"><span data-stu-id="69b8c-3469">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="69b8c-3470">Corrigido o bug que impedia a opção “-n” arg com `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3470">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="69b8c-3471">Adicionada a coluna ‘instantâneo’ à saída de tabela para `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3471">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="69b8c-3472">Corrigidos bugs com vários parâmetros que precisam ser analisados como ints</span><span class="sxs-lookup"><span data-stu-id="69b8c-3472">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="69b8c-3473">VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-3473">VM</span></span>

* <span data-ttu-id="69b8c-3474">Adicionado o comando `vm image accept-terms` para permitir a criação de VMs a partir de imagens com encargos adicionais</span><span class="sxs-lookup"><span data-stu-id="69b8c-3474">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="69b8c-3475">`[vm|vmss create]` corrigido para garantir que comandos possam ser executados sob o proxy com certificados não assinados</span><span class="sxs-lookup"><span data-stu-id="69b8c-3475">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="69b8c-3476">[VERSÃO PRÉVIA] Adicionado suporte para “baixa” prioridade para VMSS</span><span class="sxs-lookup"><span data-stu-id="69b8c-3476">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="69b8c-3477">Adicionada a proteção para `--admin-password` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3477">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="69b8c-3478">17 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="69b8c-3478">January 17, 2018</span></span>

<span data-ttu-id="69b8c-3479">Versão 2.0.25</span><span class="sxs-lookup"><span data-stu-id="69b8c-3479">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-3480">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-3480">ACR</span></span>

* <span data-ttu-id="69b8c-3481">Adicionado fallback de logon de acr em erros de credencial do Windows</span><span class="sxs-lookup"><span data-stu-id="69b8c-3481">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="69b8c-3482">Habilitados os logs de registro</span><span class="sxs-lookup"><span data-stu-id="69b8c-3482">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="69b8c-3483">ACS</span><span class="sxs-lookup"><span data-stu-id="69b8c-3483">ACS</span></span>

* <span data-ttu-id="69b8c-3484">Corrigido o comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3484">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="69b8c-3485">Removido o requisito de função do SPN</span><span class="sxs-lookup"><span data-stu-id="69b8c-3485">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-3486">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-3486">Appservice</span></span>

* <span data-ttu-id="69b8c-3487">Corrigido o bug com `config ssl upload` onde `hosting_environment_profile` era nulo</span><span class="sxs-lookup"><span data-stu-id="69b8c-3487">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="69b8c-3488">Adicionado suporte para URLs personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3488">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="69b8c-3489">Corrigido o suporte de slot para `log tail`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3489">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="69b8c-3490">Backup</span><span class="sxs-lookup"><span data-stu-id="69b8c-3490">Backup</span></span>

* <span data-ttu-id="69b8c-3491">Alterada a opção `--container-name` de `backup item list` para ser opcional</span><span class="sxs-lookup"><span data-stu-id="69b8c-3491">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="69b8c-3492">Adicionadas opções da conta de armazenamento para `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3492">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="69b8c-3493">Corrigido o check-in de local de `backup protection enable-for-vm` para não diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="69b8c-3493">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="69b8c-3494">Corrigido o problema em que os comandos falhavam com um nome de contêiner inválido</span><span class="sxs-lookup"><span data-stu-id="69b8c-3494">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="69b8c-3495">Alterado `backup item list` para incluir o 'Status de Integridade' como padrão</span><span class="sxs-lookup"><span data-stu-id="69b8c-3495">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="69b8c-3496">Lote</span><span class="sxs-lookup"><span data-stu-id="69b8c-3496">Batch</span></span>

* <span data-ttu-id="69b8c-3497">Alterado `batch login` para retornar detalhes de autenticação</span><span class="sxs-lookup"><span data-stu-id="69b8c-3497">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="69b8c-3498">Nuvem</span><span class="sxs-lookup"><span data-stu-id="69b8c-3498">Cloud</span></span>

* <span data-ttu-id="69b8c-3499">Alterado para não exigir pontos de extremidade ao definir `--profile` em uma nuvem</span><span class="sxs-lookup"><span data-stu-id="69b8c-3499">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="69b8c-3500">Consumo</span><span class="sxs-lookup"><span data-stu-id="69b8c-3500">Consumption</span></span>

* <span data-ttu-id="69b8c-3501">Adicionados novos comandos para reservas: `consumption reservations summaries` e `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3501">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="69b8c-3502">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="69b8c-3502">Event Grid</span></span>

* <span data-ttu-id="69b8c-3503">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid topic event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3503">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="69b8c-3504">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid resource event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3504">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="69b8c-3505">[ALTERAÇÃO SIGNIFICATIVA] Comando `eventgrid event-subscription show-endpoint-url` removido.</span><span class="sxs-lookup"><span data-stu-id="69b8c-3505">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="69b8c-3506">Usar `eventgrid event-subscription show --include-full-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3506">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="69b8c-3507">Adicionado o comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3507">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="69b8c-3508">Adicionado o comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3508">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="69b8c-3509">Adicionado o parâmetro `--ids` para comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3509">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="69b8c-3510">Adicionado o suporte de conclusão de guia para nomes de tópico</span><span class="sxs-lookup"><span data-stu-id="69b8c-3510">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="69b8c-3511">Interativo</span><span class="sxs-lookup"><span data-stu-id="69b8c-3511">Interactive</span></span>

* <span data-ttu-id="69b8c-3512">Corrigido o problema em que o modo interativo não funcionava com o Python 2.x</span><span class="sxs-lookup"><span data-stu-id="69b8c-3512">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="69b8c-3513">Corrigidos os erros na inicialização</span><span class="sxs-lookup"><span data-stu-id="69b8c-3513">Fixed errors on startup</span></span>
* <span data-ttu-id="69b8c-3514">Corrigido o problema com alguns comandos que não estavam em execução no modo interativo</span><span class="sxs-lookup"><span data-stu-id="69b8c-3514">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="69b8c-3515">IoT</span><span class="sxs-lookup"><span data-stu-id="69b8c-3515">IoT</span></span>

* <span data-ttu-id="69b8c-3516">Adicionado suporte para o serviço de provisionamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="69b8c-3516">Added support for device provisioning service</span></span>
* <span data-ttu-id="69b8c-3517">Adicionadas mensagens de reprovação em comandos e ajuda de comando</span><span class="sxs-lookup"><span data-stu-id="69b8c-3517">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="69b8c-3518">Adicionada verificação de IoT para informar os usuários da Extensão de IoT</span><span class="sxs-lookup"><span data-stu-id="69b8c-3518">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="69b8c-3519">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="69b8c-3519">Monitor</span></span>

* <span data-ttu-id="69b8c-3520">Adicionado o suporte de configuração de vários diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="69b8c-3520">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="69b8c-3521">Agora o parâmetro `--name` é necessário para `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3521">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="69b8c-3522">Adicionado o comando `monitor diagnostic-settings categories` para obter a categoria de configurações de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="69b8c-3522">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-3523">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-3523">Network</span></span>

* <span data-ttu-id="69b8c-3524">Corrigido o problema ao tentar alterar de/para o modo ativo-em espera com `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3524">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="69b8c-3525">Adicionado o suporte para HTTP2 para `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3525">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="69b8c-3526">Perfil</span><span class="sxs-lookup"><span data-stu-id="69b8c-3526">Profile</span></span>

* <span data-ttu-id="69b8c-3527">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="69b8c-3527">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="69b8c-3528">Função</span><span class="sxs-lookup"><span data-stu-id="69b8c-3528">Role</span></span>

* <span data-ttu-id="69b8c-3529">Adicionado o argumento `--assignee-object-id` para `role assignment create` para ignorar a consulta do gráfico</span><span class="sxs-lookup"><span data-stu-id="69b8c-3529">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="69b8c-3530">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="69b8c-3530">Service Fabric</span></span>

* <span data-ttu-id="69b8c-3531">Adicionados erros detalhados à resposta de validação ao criar cluster</span><span class="sxs-lookup"><span data-stu-id="69b8c-3531">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="69b8c-3532">Corrigido o problema de cliente ausente com vários comandos</span><span class="sxs-lookup"><span data-stu-id="69b8c-3532">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="69b8c-3533">VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-3533">VM</span></span>

* <span data-ttu-id="69b8c-3534">[VERSÃO PRÉVIA] Suporte entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3534">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="69b8c-3535">[ALTERAÇÃO SIGNIFICATIVA] Alterada única zona `vmss` padrão para o balanceador de carga "Padrão"</span><span class="sxs-lookup"><span data-stu-id="69b8c-3535">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="69b8c-3536">[ALTERAÇÃO SIGNIFICATIVA]`externalIdentities` alterado para `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="69b8c-3536">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="69b8c-3537">[VERSÃO PRÉVIA] Adicionado o suporte para a troca de disco do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="69b8c-3537">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="69b8c-3538">Adicionado o suporte para o uso de imagens da VM de outras assinaturas</span><span class="sxs-lookup"><span data-stu-id="69b8c-3538">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="69b8c-3539">Adicionados os argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` e `--plan-publisher` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3539">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="69b8c-3540">Corrigidos os problemas de erro com `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3540">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="69b8c-3541">Corrigido o uso excessivo de recursos causados por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3541">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="69b8c-3542">19 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="69b8c-3542">December 19, 2017</span></span>

<span data-ttu-id="69b8c-3543">Versão 2.0.23</span><span class="sxs-lookup"><span data-stu-id="69b8c-3543">Version 2.0.23</span></span>

* <span data-ttu-id="69b8c-3544">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="69b8c-3544">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="69b8c-3545">Contêiner</span><span class="sxs-lookup"><span data-stu-id="69b8c-3545">Container</span></span>

* <span data-ttu-id="69b8c-3546">Corrigida a ordem incorreta de parâmetros para logs de contêiner</span><span class="sxs-lookup"><span data-stu-id="69b8c-3546">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-3547">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-3547">Network</span></span>

* <span data-ttu-id="69b8c-3548">Adicionado o argumento `--disable-bgp-route-propagation` para `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3548">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="69b8c-3549">Adicionado o argumento `--ip-tags` para `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3549">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-3550">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-3550">Storage</span></span>

* <span data-ttu-id="69b8c-3551">Adicionado suporte para armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="69b8c-3551">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="69b8c-3552">VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-3552">VM</span></span>

* <span data-ttu-id="69b8c-3553">[VERSÃO PRÉVIA] Adicionado suporte para identidades atribuídas a usuários para VMs e VMSSes</span><span class="sxs-lookup"><span data-stu-id="69b8c-3553">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="69b8c-3554">5 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="69b8c-3554">December 5, 2017</span></span>

<span data-ttu-id="69b8c-3555">Versão 2.0.22</span><span class="sxs-lookup"><span data-stu-id="69b8c-3555">Version 2.0.22</span></span>

* <span data-ttu-id="69b8c-3556">Comandos `az component` removidos.</span><span class="sxs-lookup"><span data-stu-id="69b8c-3556">Removed `az component` commands.</span></span> <span data-ttu-id="69b8c-3557">Usar `az extension`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3557">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="69b8c-3558">Núcleo</span><span class="sxs-lookup"><span data-stu-id="69b8c-3558">Core</span></span>
* <span data-ttu-id="69b8c-3559">Modificou o ponto de extremidade de autoridade AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com para login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="69b8c-3559">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="69b8c-3560">Corrigido o problema onde a telemetria reenviaria continuamente</span><span class="sxs-lookup"><span data-stu-id="69b8c-3560">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="69b8c-3561">ACS</span><span class="sxs-lookup"><span data-stu-id="69b8c-3561">ACS</span></span>

* <span data-ttu-id="69b8c-3562">Comandos `aks install-connector` e `aks remove-connector` adicionados</span><span class="sxs-lookup"><span data-stu-id="69b8c-3562">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="69b8c-3563">Relatório de erros aprimorado para `acs create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3563">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="69b8c-3564">Corrigido o uso de `aks get-credentials -f` sem um caminho totalmente qualificado</span><span class="sxs-lookup"><span data-stu-id="69b8c-3564">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="69b8c-3565">Supervisor</span><span class="sxs-lookup"><span data-stu-id="69b8c-3565">Advisor</span></span>

* <span data-ttu-id="69b8c-3566">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="69b8c-3566">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-3567">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-3567">Appservice</span></span>

* <span data-ttu-id="69b8c-3568">Corrigida a geração de nome do certificado com `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3568">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="69b8c-3569">Corrigidos `webapp [list|show]` e `functionapp [list|show]` para exibir os aplicativos corretos</span><span class="sxs-lookup"><span data-stu-id="69b8c-3569">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="69b8c-3570">Valor padrão adicionado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3570">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="69b8c-3571">Consumo</span><span class="sxs-lookup"><span data-stu-id="69b8c-3571">Consumption</span></span>

* <span data-ttu-id="69b8c-3572">Suporte adicionado para a API versão de 30/11/2017</span><span class="sxs-lookup"><span data-stu-id="69b8c-3572">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="69b8c-3573">Contêiner</span><span class="sxs-lookup"><span data-stu-id="69b8c-3573">Container</span></span>

* <span data-ttu-id="69b8c-3574">Corrigida a regressão de portas padrão</span><span class="sxs-lookup"><span data-stu-id="69b8c-3574">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="69b8c-3575">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="69b8c-3575">Monitor</span></span>

* <span data-ttu-id="69b8c-3576">Suporte de várias dimensões adicionado ao comando de métricas</span><span class="sxs-lookup"><span data-stu-id="69b8c-3576">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="69b8c-3577">Recurso</span><span class="sxs-lookup"><span data-stu-id="69b8c-3577">Resource</span></span>

* <span data-ttu-id="69b8c-3578">Adicionado o argumento `--include-response-body` para `resource show`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3578">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="69b8c-3579">Função</span><span class="sxs-lookup"><span data-stu-id="69b8c-3579">Role</span></span>

* <span data-ttu-id="69b8c-3580">Exibição de atribuições padrão adicionada dos administradores "clássicos" para `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3580">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="69b8c-3581">Suporte adicionado a `ad sp reset-credentials` para adicionar as credenciais em vez de substituir</span><span class="sxs-lookup"><span data-stu-id="69b8c-3581">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="69b8c-3582">Relatório de erros aprimorado para `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3582">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="69b8c-3583">SQL</span><span class="sxs-lookup"><span data-stu-id="69b8c-3583">SQL</span></span>

* <span data-ttu-id="69b8c-3584">Comandos `sql db list-usages` e `sql db show-usage` adicionados</span><span class="sxs-lookup"><span data-stu-id="69b8c-3584">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="69b8c-3585">Comandos `sql server conn-policy show` e `sql server conn-policy update` adicionados</span><span class="sxs-lookup"><span data-stu-id="69b8c-3585">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="69b8c-3586">VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-3586">VM</span></span>

* <span data-ttu-id="69b8c-3587">Informações da zona adicionadas a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3587">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="69b8c-3588">14 de novembro de 2017</span><span class="sxs-lookup"><span data-stu-id="69b8c-3588">November 14, 2017</span></span>

<span data-ttu-id="69b8c-3589">Versão 2.0.21</span><span class="sxs-lookup"><span data-stu-id="69b8c-3589">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-3590">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-3590">ACR</span></span>

* <span data-ttu-id="69b8c-3591">Suporte adicionado para criar webhooks em regiões de replicação</span><span class="sxs-lookup"><span data-stu-id="69b8c-3591">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="69b8c-3592">ACS</span><span class="sxs-lookup"><span data-stu-id="69b8c-3592">ACS</span></span>

* <span data-ttu-id="69b8c-3593">Alteradas todas as palavras "agente" para "nó" no AKS</span><span class="sxs-lookup"><span data-stu-id="69b8c-3593">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="69b8c-3594">Opção `--orchestrator-release` preterida para `acs create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3594">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="69b8c-3595">Tamanho alterado da VM padrão do AKS para `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3595">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="69b8c-3596">`az aks browse` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="69b8c-3596">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="69b8c-3597">`az aks get-credentials` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="69b8c-3597">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-3598">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-3598">Appservice</span></span>

* <span data-ttu-id="69b8c-3599">Origem da implantação adicional `config-zip` para webapps e aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="69b8c-3599">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="69b8c-3600">Opção `--docker-container-logging` adicionada a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3600">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="69b8c-3601">Removida a opção `storage` do parâmetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3601">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="69b8c-3602">Mensagens de erro aprimoradas para `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3602">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="69b8c-3603">Suporte adicionado para criar aplicativos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="69b8c-3603">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="69b8c-3604">`list-locations` fixo</span><span class="sxs-lookup"><span data-stu-id="69b8c-3604">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="69b8c-3605">Lote</span><span class="sxs-lookup"><span data-stu-id="69b8c-3605">Batch</span></span>

* <span data-ttu-id="69b8c-3606">Bug corrigido no comando pool create quando uma ID do recurso foi usada com o sinalizador `--image`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3606">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="69b8c-3607">Batchai</span><span class="sxs-lookup"><span data-stu-id="69b8c-3607">Batchai</span></span>

* <span data-ttu-id="69b8c-3608">Opção curta adicionada `-s` para `--vm-size` ao fornecer o tamanho da VM no comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3608">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="69b8c-3609">Nome da conta de armazenamento e argumentos-chave adicionados aos parâmetros `cluster create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3609">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="69b8c-3610">Documentação corrigida para `job list-files` e `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3610">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="69b8c-3611">Opção curta adicionada `-r` para `--cluster-name` ao fornecer o nome do cluster no comando `job create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3611">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="69b8c-3612">Nuvem</span><span class="sxs-lookup"><span data-stu-id="69b8c-3612">Cloud</span></span>

* <span data-ttu-id="69b8c-3613">`cloud [register|update]` alterado para evitar registrar nuvens sem os pontos de extremidade necessários</span><span class="sxs-lookup"><span data-stu-id="69b8c-3613">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="69b8c-3614">Contêiner</span><span class="sxs-lookup"><span data-stu-id="69b8c-3614">Container</span></span>

* <span data-ttu-id="69b8c-3615">Suporte adicionado para abrir várias portas</span><span class="sxs-lookup"><span data-stu-id="69b8c-3615">Added support to open multiple ports</span></span>
* <span data-ttu-id="69b8c-3616">Política de reinicialização do grupo de contêiner adicionada</span><span class="sxs-lookup"><span data-stu-id="69b8c-3616">Added container group restart policy</span></span>
* <span data-ttu-id="69b8c-3617">Suporte adicionado para montar o compartilhamento de Arquivos do Azure como um volume</span><span class="sxs-lookup"><span data-stu-id="69b8c-3617">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="69b8c-3618">Documentos de ajuda atualizados</span><span class="sxs-lookup"><span data-stu-id="69b8c-3618">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="69b8c-3619">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="69b8c-3619">Data Lake Analytics</span></span>

* <span data-ttu-id="69b8c-3620">`[job|account] list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="69b8c-3620">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="69b8c-3621">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="69b8c-3621">Data Lake Store</span></span>

* <span data-ttu-id="69b8c-3622">`account list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="69b8c-3622">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="69b8c-3623">Extensão</span><span class="sxs-lookup"><span data-stu-id="69b8c-3623">Extension</span></span>

* <span data-ttu-id="69b8c-3624">`extension list-available` adicionado para permitir a listagem de extensões oficiais da Microsoft</span><span class="sxs-lookup"><span data-stu-id="69b8c-3624">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="69b8c-3625">`--name` adicionado a `extension [add|update]` para permitir a instalação de extensões por nome</span><span class="sxs-lookup"><span data-stu-id="69b8c-3625">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="69b8c-3626">IoT</span><span class="sxs-lookup"><span data-stu-id="69b8c-3626">IoT</span></span>

* <span data-ttu-id="69b8c-3627">Suporte adicionado para as autoridades de certificação (CA) e cadeias de certificado</span><span class="sxs-lookup"><span data-stu-id="69b8c-3627">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="69b8c-3628">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="69b8c-3628">Monitor</span></span>

* <span data-ttu-id="69b8c-3629">Adicionados os comandos `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3629">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-3630">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-3630">Network</span></span>

* <span data-ttu-id="69b8c-3631">Suporte adicionado para registros DNS da CAA</span><span class="sxs-lookup"><span data-stu-id="69b8c-3631">Added support for CAA DNS records</span></span>
* <span data-ttu-id="69b8c-3632">Problema corrigido onde os pontos de extremidade não podem ser atualizados com `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3632">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="69b8c-3633">Problema corrigido onde `vnet update --dns-servers` não funcionou dependendo de como a VNET foi criada</span><span class="sxs-lookup"><span data-stu-id="69b8c-3633">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="69b8c-3634">Problema corrigido onde os nomes DNS relativos foram importados incorretamente por`dns zone import`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3634">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="69b8c-3635">Reservas</span><span class="sxs-lookup"><span data-stu-id="69b8c-3635">Reservations</span></span>

* <span data-ttu-id="69b8c-3636">Versão prévia inicial</span><span class="sxs-lookup"><span data-stu-id="69b8c-3636">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="69b8c-3637">Recurso</span><span class="sxs-lookup"><span data-stu-id="69b8c-3637">Resource</span></span>

* <span data-ttu-id="69b8c-3638">Suporte adicionado das IDs de recurso ao parâmetro `--resource` e bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="69b8c-3638">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="69b8c-3639">SQL</span><span class="sxs-lookup"><span data-stu-id="69b8c-3639">SQL</span></span>

* <span data-ttu-id="69b8c-3640">Parâmetro `--ignore-missing-vnet-service-endpoint` adicionado a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3640">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-3641">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-3641">Storage</span></span>

* <span data-ttu-id="69b8c-3642">`storage account create` criado ao usar o SKU `Standard_RAGRS` como padrão</span><span class="sxs-lookup"><span data-stu-id="69b8c-3642">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="69b8c-3643">Bugs corrigidos ao lidar com nomes de arquivo/blob que incluem caracteres não ascii</span><span class="sxs-lookup"><span data-stu-id="69b8c-3643">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="69b8c-3644">Bug corrigido que impedia usar `--source-uri` com `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3644">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="69b8c-3645">Comandos adicionados para usar o glob e excluir vários objetos com `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3645">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="69b8c-3646">Problema corrigido ao habilitar métricas com `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3646">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="69b8c-3647">Problema corrigido com arquivos acima de 200 GB ao usar `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3647">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="69b8c-3648">Problema corrigido onde `--bypass` e `--default-action` foram ignorados por `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3648">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="69b8c-3649">VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-3649">VM</span></span>

* <span data-ttu-id="69b8c-3650">Bug corrigido com `vmss create`, que impediu o uso da camada de tamanho `Basic`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3650">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="69b8c-3651">Argumentos `--plan` adicionados a `[vm|vmss] create` para ter imagens personalizadas com informações de cobrança</span><span class="sxs-lookup"><span data-stu-id="69b8c-3651">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="69b8c-3652">Comandos `vm secret `[add|remove|list]\` adicionados</span><span class="sxs-lookup"><span data-stu-id="69b8c-3652">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="69b8c-3653">`vm format-secret` renomeado para `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3653">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="69b8c-3654">Adicionado o argumento `--encrypt format` para `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3654">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="69b8c-3655">24 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="69b8c-3655">October 24, 2017</span></span>

<span data-ttu-id="69b8c-3656">Versão 2.0.20</span><span class="sxs-lookup"><span data-stu-id="69b8c-3656">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="69b8c-3657">Núcleo</span><span class="sxs-lookup"><span data-stu-id="69b8c-3657">Core</span></span>

* <span data-ttu-id="69b8c-3658">Atualizado `2017-03-09-profile` para usar a `MGMT_STORAGE` versão da API`2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3658">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-3659">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-3659">ACR</span></span>

* <span data-ttu-id="69b8c-3660">Gerenciamento de recursos atualizado para apontar para a versão da API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3660">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="69b8c-3661">SKU 'traga seu próprio armazenamento' alterada para Clássico</span><span class="sxs-lookup"><span data-stu-id="69b8c-3661">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="69b8c-3662">SKUs de registro renomeados como Básico, Standard e Premium</span><span class="sxs-lookup"><span data-stu-id="69b8c-3662">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="69b8c-3663">ACS</span><span class="sxs-lookup"><span data-stu-id="69b8c-3663">ACS</span></span>

* <span data-ttu-id="69b8c-3664">[VERSÃO PRÉVIA] Comandos `az aks` adicionados</span><span class="sxs-lookup"><span data-stu-id="69b8c-3664">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="69b8c-3665">Kubernetes `get-credentials` corrigido</span><span class="sxs-lookup"><span data-stu-id="69b8c-3665">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-3666">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-3666">Appservice</span></span>

* <span data-ttu-id="69b8c-3667">Problema corrigido onde os logs `webapp` baixados podem ser inválidos</span><span class="sxs-lookup"><span data-stu-id="69b8c-3667">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="69b8c-3668">Componente</span><span class="sxs-lookup"><span data-stu-id="69b8c-3668">Component</span></span>

* <span data-ttu-id="69b8c-3669">Mensagem de reprovação mais clara adicionada para todos os instaladores e prompt de confirmação</span><span class="sxs-lookup"><span data-stu-id="69b8c-3669">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="69b8c-3670">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="69b8c-3670">Monitor</span></span>

* <span data-ttu-id="69b8c-3671">Adicionados os comandos `action-group`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3671">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="69b8c-3672">Recurso</span><span class="sxs-lookup"><span data-stu-id="69b8c-3672">Resource</span></span>

* <span data-ttu-id="69b8c-3673">Incompatibilidade corrigida com a versão mais recente de dependência msrest em `group export`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3673">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="69b8c-3674">`policy assignment create` corrigido para trabalhar com as definições de política internas e as definições do conjunto de políticas</span><span class="sxs-lookup"><span data-stu-id="69b8c-3674">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="69b8c-3675">VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-3675">VM</span></span>

* <span data-ttu-id="69b8c-3676">Adicionado o argumento `--accelerated-networking` para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3676">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="69b8c-3677">9 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="69b8c-3677">October 9, 2017</span></span>

<span data-ttu-id="69b8c-3678">Versão 2.0.19</span><span class="sxs-lookup"><span data-stu-id="69b8c-3678">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="69b8c-3679">Núcleo</span><span class="sxs-lookup"><span data-stu-id="69b8c-3679">Core</span></span>

* <span data-ttu-id="69b8c-3680">Tratamento de URLs de autoridade do AD FS adicionado com uma barra à direita para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="69b8c-3680">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-3681">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-3681">Appservice</span></span>

* <span data-ttu-id="69b8c-3682">Atualização genérica adicionada com o novo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3682">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="69b8c-3683">Lote</span><span class="sxs-lookup"><span data-stu-id="69b8c-3683">Batch</span></span>

* <span data-ttu-id="69b8c-3684">Atualizado para o SDK do Lote 4.0.0</span><span class="sxs-lookup"><span data-stu-id="69b8c-3684">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="69b8c-3685">A opção `--image` de VirtualMachineConfiguration foi atualizada para dar suporte a referências de imagem ARM além de publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="69b8c-3685">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="69b8c-3686">Suporte adicionado para o novo modelo de extensão da CLI para comandos de Extensões de Lote</span><span class="sxs-lookup"><span data-stu-id="69b8c-3686">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="69b8c-3687">Removeu o suporte de Lote do modelo de componente</span><span class="sxs-lookup"><span data-stu-id="69b8c-3687">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="69b8c-3688">Batchai</span><span class="sxs-lookup"><span data-stu-id="69b8c-3688">Batchai</span></span>

* <span data-ttu-id="69b8c-3689">Versão inicial do módulo de IA de Lote</span><span class="sxs-lookup"><span data-stu-id="69b8c-3689">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="69b8c-3690">Keyvault</span><span class="sxs-lookup"><span data-stu-id="69b8c-3690">Keyvault</span></span>

* <span data-ttu-id="69b8c-3691">Correção do problema de autenticação do Cofre de Chaves ao usar o AD FS no Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="69b8c-3691">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="69b8c-3692">(#4448)</span><span class="sxs-lookup"><span data-stu-id="69b8c-3692">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="69b8c-3693">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-3693">Network</span></span>

* <span data-ttu-id="69b8c-3694">Alterado `--server` argumento de `application-gateway address-pool create` para ser opcional, permitindo pools de endereços vazios</span><span class="sxs-lookup"><span data-stu-id="69b8c-3694">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="69b8c-3695">`traffic-manager` foi atualizado para oferecer suporte aos recursos mais recentes</span><span class="sxs-lookup"><span data-stu-id="69b8c-3695">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="69b8c-3696">Recurso</span><span class="sxs-lookup"><span data-stu-id="69b8c-3696">Resource</span></span>

* <span data-ttu-id="69b8c-3697">Suporte adicionado para `--resource-group/-g` opções do nome do grupo de recursos para `group`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3697">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="69b8c-3698">Comandos adicionados a `account lock` para funcionar com bloqueios no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="69b8c-3698">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="69b8c-3699">Comandos adicionados a `group lock` para funcionar com bloqueios no nível do grupo</span><span class="sxs-lookup"><span data-stu-id="69b8c-3699">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="69b8c-3700">Comandos adicionados a `resource lock` para funcionar com bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="69b8c-3700">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="69b8c-3701">Sql</span><span class="sxs-lookup"><span data-stu-id="69b8c-3701">Sql</span></span>

* <span data-ttu-id="69b8c-3702">Suporte adicionado para SQL TDE (Transparent Data Encryption) e TDE com Traga sua própria chave</span><span class="sxs-lookup"><span data-stu-id="69b8c-3702">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="69b8c-3703">Comando `db list-deleted` e parâmetro `db restore --deleted-time` adicionados, permitindo localizar e restaurar bancos de dados excluídos</span><span class="sxs-lookup"><span data-stu-id="69b8c-3703">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="69b8c-3704">`db op list` e `db op cancel` adicionados, permitindo listar e cancelar operações em andamento no banco de dados</span><span class="sxs-lookup"><span data-stu-id="69b8c-3704">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-3705">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-3705">Storage</span></span>

* <span data-ttu-id="69b8c-3706">Suporte adicionado para instantâneo de compartilhamento de arquivos</span><span class="sxs-lookup"><span data-stu-id="69b8c-3706">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="69b8c-3707">VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-3707">Vm</span></span>

* <span data-ttu-id="69b8c-3708">Correção de um bug em `vm show` onde o uso de `-d` causou uma falha nos endereços IP privados ausentes</span><span class="sxs-lookup"><span data-stu-id="69b8c-3708">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="69b8c-3709">[VERSÃO PRÉVIA] Suporte adicionado para atualização sem interrupção para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3709">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="69b8c-3710">Suporte adicionado para atualizar as configurações de criptografia com `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3710">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="69b8c-3711">Parâmetro `--os-disk-size-gb` adicionado a `vm create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3711">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="69b8c-3712">Parâmetro `--license-type` adicionado ao Windows para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3712">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="69b8c-3713">22 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="69b8c-3713">September 22, 2017</span></span>

<span data-ttu-id="69b8c-3714">Versão 2.0.1.8</span><span class="sxs-lookup"><span data-stu-id="69b8c-3714">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="69b8c-3715">Recurso</span><span class="sxs-lookup"><span data-stu-id="69b8c-3715">Resource</span></span>

* <span data-ttu-id="69b8c-3716">Suporte adicionado para mostrar as definições de políticas internas</span><span class="sxs-lookup"><span data-stu-id="69b8c-3716">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="69b8c-3717">Parâmetro de modo de suporte adicionado para a criação de definições de política</span><span class="sxs-lookup"><span data-stu-id="69b8c-3717">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="69b8c-3718">Suporte adicionado para definições de interface do usuário e modelos em `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3718">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="69b8c-3719">[ALTERAÇÃO SIGNIFICATIVA] Tipo de recurso `managedapp` alterado de `appliances` para `applications` e de `applianceDefinitions` para `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3719">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-3720">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-3720">Network</span></span>

* <span data-ttu-id="69b8c-3721">Suporte adicionado para a zona de disponibilidade para os subcomandos `network lb` e `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3721">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="69b8c-3722">Suporte adicionado ao Emparelhamento IPv6 da Microsoft para `express-route`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3722">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="69b8c-3723">Adicionados `asg` comandos de grupo de segurança do aplicativo</span><span class="sxs-lookup"><span data-stu-id="69b8c-3723">Added `asg` application security group commands</span></span>
* <span data-ttu-id="69b8c-3724">Adicionado o argumento `--application-security-groups` para `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3724">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="69b8c-3725">Adicionados os argumentos `--source-asgs` e `--destination-asgs` para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3725">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="69b8c-3726">Adicionados os argumentos `--ddos-protection` e `--vm-protection` para `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3726">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="69b8c-3727">Adicionados os comandos `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3727">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-3728">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-3728">Storage</span></span>

* <span data-ttu-id="69b8c-3729">Correção do problema onde `storage account network-rule` comandos poderão falhar após a atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="69b8c-3729">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="69b8c-3730">Grade de eventos</span><span class="sxs-lookup"><span data-stu-id="69b8c-3730">Eventgrid</span></span>

* <span data-ttu-id="69b8c-3731">Atualizada SDK Python da Grade de Eventos do Azure para usar a versão de API mais recente "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="69b8c-3731">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="69b8c-3732">SQL</span><span class="sxs-lookup"><span data-stu-id="69b8c-3732">SQL</span></span>

* <span data-ttu-id="69b8c-3733">Alterado o `sql server list` argumento `--resource-group` para ser opcional.</span><span class="sxs-lookup"><span data-stu-id="69b8c-3733">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="69b8c-3734">Se não for especificado, todos os servidores sql na assinatura serão retornados</span><span class="sxs-lookup"><span data-stu-id="69b8c-3734">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="69b8c-3735">Adicionado o `--no-wait` parâmetro para `db [create|copy|restore|update|replica create|create|update]` e `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3735">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="69b8c-3736">Keyvault</span><span class="sxs-lookup"><span data-stu-id="69b8c-3736">Keyvault</span></span>

* <span data-ttu-id="69b8c-3737">Adicionado suporte para comandos Keyvault por trás de um proxy</span><span class="sxs-lookup"><span data-stu-id="69b8c-3737">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="69b8c-3738">VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-3738">VM</span></span>

* <span data-ttu-id="69b8c-3739">Adicionado suporte à zona de disponibilidade para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3739">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="69b8c-3740">Correção do problema onde usar`--app-gateway ID` com `vmss create` poderia causar uma falha</span><span class="sxs-lookup"><span data-stu-id="69b8c-3740">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="69b8c-3741">Adicionado o argumento `--asgs` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3741">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="69b8c-3742">Suporte adicionado para executar comandos em VMs com `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3742">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="69b8c-3743">[VERSÃO PRÉVIA] Adicionado suporte para criptografia de disco VMSS com `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3743">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="69b8c-3744">Suporte adicionado para realizar a manutenção em VMs com `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3744">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="69b8c-3745">ACS</span><span class="sxs-lookup"><span data-stu-id="69b8c-3745">ACS</span></span>

* <span data-ttu-id="69b8c-3746">[VERSÃO PRÉVIA] Adicionado `--orchestrator-release` argumento para `acs create` para regiões de versão prévia do ACS</span><span class="sxs-lookup"><span data-stu-id="69b8c-3746">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-3747">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-3747">Appservice</span></span>

* <span data-ttu-id="69b8c-3748">Adicionada a capacidade para atualizar e mostrar as configurações de autenticação com `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3748">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="69b8c-3749">Backup</span><span class="sxs-lookup"><span data-stu-id="69b8c-3749">Backup</span></span>

* <span data-ttu-id="69b8c-3750">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="69b8c-3750">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="69b8c-3751">11 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="69b8c-3751">September 11, 2017</span></span>

<span data-ttu-id="69b8c-3752">Versão 2.0.17</span><span class="sxs-lookup"><span data-stu-id="69b8c-3752">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="69b8c-3753">Núcleo</span><span class="sxs-lookup"><span data-stu-id="69b8c-3753">Core</span></span>

* <span data-ttu-id="69b8c-3754">Módulo de comando habilitado para definir sua própria ID de correlação na telemetria</span><span class="sxs-lookup"><span data-stu-id="69b8c-3754">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="69b8c-3755">Problema de despejo de JSON corrigido quando a telemetria é definida como modo de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="69b8c-3755">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="69b8c-3756">Acs</span><span class="sxs-lookup"><span data-stu-id="69b8c-3756">Acs</span></span>

* <span data-ttu-id="69b8c-3757">Adicionado o comando `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3757">Added `acs list-locations` command</span></span>
* <span data-ttu-id="69b8c-3758">Fez `ssh-key-file` vir com o valor padrão esperado</span><span class="sxs-lookup"><span data-stu-id="69b8c-3758">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-3759">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-3759">Appservice</span></span>

* <span data-ttu-id="69b8c-3760">Foi incluída a capacidade de criar um aplicativo Web em um grupo de recursos que não seja o plano de serviço ativo</span><span class="sxs-lookup"><span data-stu-id="69b8c-3760">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="69b8c-3761">CDN</span><span class="sxs-lookup"><span data-stu-id="69b8c-3761">CDN</span></span>

* <span data-ttu-id="69b8c-3762">Foi corrigido o bug 'Não é possível interar CustomDomain' para `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3762">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="69b8c-3763">Extensão</span><span class="sxs-lookup"><span data-stu-id="69b8c-3763">Extension</span></span>

* <span data-ttu-id="69b8c-3764">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="69b8c-3764">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="69b8c-3765">Keyvault</span><span class="sxs-lookup"><span data-stu-id="69b8c-3765">Keyvault</span></span>

* <span data-ttu-id="69b8c-3766">Foi corrigido o problema onde permissões diferenciavam maiúsculas de minúsculas para `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3766">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-3767">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-3767">Network</span></span>

* <span data-ttu-id="69b8c-3768">`vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3768">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="69b8c-3769">Foi renomeado o argumento `--private-access-services` para `--service-endpoints` para `vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3769">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="69b8c-3770">Foi adicionado suporte a vários intervalos de IP e intervalos de portas para `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3770">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="69b8c-3771">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3771">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="69b8c-3772">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3772">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="69b8c-3773">Recurso</span><span class="sxs-lookup"><span data-stu-id="69b8c-3773">Resource</span></span>

* <span data-ttu-id="69b8c-3774">Permitir a passagem de definições de parâmetro de políticas de recursos em `policy definition create` e`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3774">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="69b8c-3775">Permitir a passagem de valores de parâmetro para`policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3775">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="69b8c-3776">Permitir a passagem de JSON ou arquivo para todos os parâmetros</span><span class="sxs-lookup"><span data-stu-id="69b8c-3776">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="69b8c-3777">Versão da API incrementada</span><span class="sxs-lookup"><span data-stu-id="69b8c-3777">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="69b8c-3778">SQL</span><span class="sxs-lookup"><span data-stu-id="69b8c-3778">SQL</span></span>

* <span data-ttu-id="69b8c-3779">Adicionados os comandos `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3779">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="69b8c-3780">VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-3780">VM</span></span>

* <span data-ttu-id="69b8c-3781">Corrigido: não atribuir acesso, a menos que `--scope` seja fornecido</span><span class="sxs-lookup"><span data-stu-id="69b8c-3781">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="69b8c-3782">Corrigido: usar a mesma nomenclatura de extensão do que o portal</span><span class="sxs-lookup"><span data-stu-id="69b8c-3782">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="69b8c-3783">Foi removido `subscription` da saída de `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3783">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="69b8c-3784">Corrigido: SKU de armazenamento do `[vm|vmss] create` não é aplicada em discos de dados com uma imagem</span><span class="sxs-lookup"><span data-stu-id="69b8c-3784">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="69b8c-3785">Corrigido: `vm format-secret --secrets` não aceita IDs de separados de nova linha</span><span class="sxs-lookup"><span data-stu-id="69b8c-3785">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="69b8c-3786">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="69b8c-3786">August 31, 2017</span></span>

<span data-ttu-id="69b8c-3787">Versão 2.0.16</span><span class="sxs-lookup"><span data-stu-id="69b8c-3787">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="69b8c-3788">Keyvault</span><span class="sxs-lookup"><span data-stu-id="69b8c-3788">Keyvault</span></span>

* <span data-ttu-id="69b8c-3789">Correção do bug ao tentar resolver automaticamente a codificação secreta com `secret download`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3789">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="69b8c-3790">Sf</span><span class="sxs-lookup"><span data-stu-id="69b8c-3790">Sf</span></span>

* <span data-ttu-id="69b8c-3791">Substituição de todos os comandos em favor da CLI do Service Fabric (sfctl)</span><span class="sxs-lookup"><span data-stu-id="69b8c-3791">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-3792">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-3792">Storage</span></span>

* <span data-ttu-id="69b8c-3793">Correção de problema onde as contas de armazenamento não conseguiam ser criadas em regiões sem suporte ao recurso NetworkACLs</span><span class="sxs-lookup"><span data-stu-id="69b8c-3793">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="69b8c-3794">Determinar o tipo de conteúdo e a codificação do conteúdo durante o upload de arquivo e de blob se nem o tipo de conteúdo nem a codificação de conteúdo forem especificados</span><span class="sxs-lookup"><span data-stu-id="69b8c-3794">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="69b8c-3795">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="69b8c-3795">August 28, 2017</span></span>

<span data-ttu-id="69b8c-3796">Versão 2.0.15</span><span class="sxs-lookup"><span data-stu-id="69b8c-3796">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="69b8c-3797">CLI</span><span class="sxs-lookup"><span data-stu-id="69b8c-3797">CLI</span></span>

* <span data-ttu-id="69b8c-3798">Nota legal adicionada ao `--version`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3798">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="69b8c-3799">ACS</span><span class="sxs-lookup"><span data-stu-id="69b8c-3799">ACS</span></span>

* <span data-ttu-id="69b8c-3800">Corrigidas as regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="69b8c-3800">Corrected preview regions</span></span>
* <span data-ttu-id="69b8c-3801">Corrigida a formatação padrão de `dns_name_prefix`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3801">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="69b8c-3802">Saída de comando ACS otimizada</span><span class="sxs-lookup"><span data-stu-id="69b8c-3802">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-3803">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-3803">Appservice</span></span>

* <span data-ttu-id="69b8c-3804">[ALTERAÇÃO SIGNIFICATIVA] Corrigidas as inconsistências na saída de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3804">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="69b8c-3805">Adicionado um novo alias de `-i` para `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3805">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="69b8c-3806">Exposto `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3806">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="69b8c-3807">Expostos novos argumentos de `az webapp delete` para manter o plano, as métricas ou o registro de DNS do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="69b8c-3807">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="69b8c-3808">Corrigido: detectar as configurações de slot corretamente</span><span class="sxs-lookup"><span data-stu-id="69b8c-3808">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="69b8c-3809">IoT</span><span class="sxs-lookup"><span data-stu-id="69b8c-3809">IoT</span></span>

* <span data-ttu-id="69b8c-3810">Corrigido #3934: a criação de uma política não limpa mais as políticas existentes</span><span class="sxs-lookup"><span data-stu-id="69b8c-3810">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-3811">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-3811">Network</span></span>

* <span data-ttu-id="69b8c-3812">[ALTERAÇÃO SIGNIFICATIVA]`vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3812">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="69b8c-3813">[ALTERAÇÃO SIGNIFICATIVA] Opção `--private-access-services` renomeada como `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3813">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="69b8c-3814">Adicionado suporte para vários  intervalos de IP e portas para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3814">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="69b8c-3815">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3815">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="69b8c-3816">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3816">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="69b8c-3817">Perfil</span><span class="sxs-lookup"><span data-stu-id="69b8c-3817">Profile</span></span>

* <span data-ttu-id="69b8c-3818">`--msi` e `--msi-port` expostos a logon usando a identidade de uma máquina virtual</span><span class="sxs-lookup"><span data-stu-id="69b8c-3818">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="69b8c-3819">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="69b8c-3819">Service Fabric</span></span>

* <span data-ttu-id="69b8c-3820">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="69b8c-3820">Preview release</span></span>
* <span data-ttu-id="69b8c-3821">Simplificadas as regras de registro de usuário/senha para comando</span><span class="sxs-lookup"><span data-stu-id="69b8c-3821">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="69b8c-3822">Corrigido o prompt de senha para o usuário mesmo após a passagem do parâmetro</span><span class="sxs-lookup"><span data-stu-id="69b8c-3822">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="69b8c-3823">Adicionado suporte para `registry_cred` vazio</span><span class="sxs-lookup"><span data-stu-id="69b8c-3823">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-3824">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-3824">Storage</span></span>

* <span data-ttu-id="69b8c-3825">Habilitada a camada de blob de configuração</span><span class="sxs-lookup"><span data-stu-id="69b8c-3825">Enabled setting blob tier</span></span>
* <span data-ttu-id="69b8c-3826">Adicionados os argumentos `--bypass` e `--default-action` ao `storage account [create|update]` para dar suporte ao serviço de túnel</span><span class="sxs-lookup"><span data-stu-id="69b8c-3826">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="69b8c-3827">Comandos adicionados ao `storage account network-rule` para adicionar as regras de rede virtual e regras baseadas em IP</span><span class="sxs-lookup"><span data-stu-id="69b8c-3827">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="69b8c-3828">Habilitada a criptografia de serviço por chave gerenciada de cliente</span><span class="sxs-lookup"><span data-stu-id="69b8c-3828">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="69b8c-3829">[ALTERAÇÃO SIGNIFICATIVA] Opção `--encryption` renomeada como `--encryption-services` para o comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3829">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="69b8c-3830">Correção #4220: `az storage account update encryption` - incompatibilidade de sintaxe</span><span class="sxs-lookup"><span data-stu-id="69b8c-3830">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="69b8c-3831">VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-3831">VM</span></span>

* <span data-ttu-id="69b8c-3832">Corrigido o problema em que informações incorretas extras eram exibidas para `vmss get-instance-view` ao usar `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3832">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="69b8c-3833">Adicionado suporte ao `--lb-sku` para `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="69b8c-3833">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="69b8c-3834">Removidos nomes humanos da lista de bloqueio de nome de administrador para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3834">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="69b8c-3835">Corrigido o problema onde `[vm|vmss] create` geraria um erro se não for possível extrair informações do plano de uma imagem</span><span class="sxs-lookup"><span data-stu-id="69b8c-3835">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="69b8c-3836">Corrigida uma falha ao criar um conjunto de dimensionamento de máquinas virtuais com um balanceamento de carga interno</span><span class="sxs-lookup"><span data-stu-id="69b8c-3836">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="69b8c-3837">Corrigido o problema onde o argumento `--no-wait` não funcionava com `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3837">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="69b8c-3838">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="69b8c-3838">August 15, 2017</span></span>

<span data-ttu-id="69b8c-3839">Versão 2.0.14</span><span class="sxs-lookup"><span data-stu-id="69b8c-3839">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="69b8c-3840">ACS</span><span class="sxs-lookup"><span data-stu-id="69b8c-3840">ACS</span></span>

* <span data-ttu-id="69b8c-3841">Corrigido o número da porta SSH Master0 para kubernetes</span><span class="sxs-lookup"><span data-stu-id="69b8c-3841">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-3842">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-3842">Appservice</span></span>

* <span data-ttu-id="69b8c-3843">Corrigida uma exceção ao criar um novo GIT com base no aplicativo Web Linux</span><span class="sxs-lookup"><span data-stu-id="69b8c-3843">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="69b8c-3844">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="69b8c-3844">Event Grid</span></span>

* <span data-ttu-id="69b8c-3845">Adicionadas dependências SDK</span><span class="sxs-lookup"><span data-stu-id="69b8c-3845">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="69b8c-3846">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="69b8c-3846">August 11, 2017</span></span>

<span data-ttu-id="69b8c-3847">Versão 2.0.13</span><span class="sxs-lookup"><span data-stu-id="69b8c-3847">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="69b8c-3848">ACS</span><span class="sxs-lookup"><span data-stu-id="69b8c-3848">ACS</span></span>

* <span data-ttu-id="69b8c-3849">Adicionadas mais regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="69b8c-3849">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="69b8c-3850">Lote</span><span class="sxs-lookup"><span data-stu-id="69b8c-3850">Batch</span></span>

* <span data-ttu-id="69b8c-3851">Atualizado para o Lote SDK 3.1.0 e Gerenciamento de Lote SDK 4.1.0</span><span class="sxs-lookup"><span data-stu-id="69b8c-3851">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="69b8c-3852">Adicionado um novo comando que mostra as contagens de tarefas de um trabalho</span><span class="sxs-lookup"><span data-stu-id="69b8c-3852">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="69b8c-3853">Corrigido o bug no processamento de URL de SAS do arquivo de recurso</span><span class="sxs-lookup"><span data-stu-id="69b8c-3853">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="69b8c-3854">Ponto de extremidade da conta de lote agora dá suporte ao prefixo opcional “https://”</span><span class="sxs-lookup"><span data-stu-id="69b8c-3854">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="69b8c-3855">Suporte para adicionar listas de mais de 100 tarefas a um trabalho</span><span class="sxs-lookup"><span data-stu-id="69b8c-3855">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="69b8c-3856">Adicionado log de depuração para carregar o módulo do comando de Extensões</span><span class="sxs-lookup"><span data-stu-id="69b8c-3856">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="69b8c-3857">Componente</span><span class="sxs-lookup"><span data-stu-id="69b8c-3857">Component</span></span>

* <span data-ttu-id="69b8c-3858">Aviso de substituição adicionado aos comandos 'az component'</span><span class="sxs-lookup"><span data-stu-id="69b8c-3858">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="69b8c-3859">Contêiner</span><span class="sxs-lookup"><span data-stu-id="69b8c-3859">Container</span></span>

* <span data-ttu-id="69b8c-3860">`create`: corrigido o problema em que o sinal de igual não era permitido dentro de uma variável de ambiente</span><span class="sxs-lookup"><span data-stu-id="69b8c-3860">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="69b8c-3861">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="69b8c-3861">Data Lake Store</span></span>

* <span data-ttu-id="69b8c-3862">Habilitado o controle do andamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-3862">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="69b8c-3863">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="69b8c-3863">Event Grid</span></span>

* <span data-ttu-id="69b8c-3864">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="69b8c-3864">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-3865">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-3865">Network</span></span>

* <span data-ttu-id="69b8c-3866">`lb`: corrigido o problema em que os nomes de recursos filhos específicos não eram resolvidos corretamente quando omitidos</span><span class="sxs-lookup"><span data-stu-id="69b8c-3866">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="69b8c-3867">`application-gateway {subresource} delete`: corrigido o problema em que `--no-wait` não foi liquidado</span><span class="sxs-lookup"><span data-stu-id="69b8c-3867">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="69b8c-3868">`application-gateway http-settings update`: corrigido o problema em que `--connection-draining-timeout` não podia ser desativado</span><span class="sxs-lookup"><span data-stu-id="69b8c-3868">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="69b8c-3869">Corrigido o erro de argumento de palavra-chave inesperado `sa_data_size_kilobyes` com `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3869">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="69b8c-3870">Perfil</span><span class="sxs-lookup"><span data-stu-id="69b8c-3870">Profile</span></span>

* <span data-ttu-id="69b8c-3871">`account list`: adicionado `--refresh` para sincronizar as assinaturas mais recentes do servidor</span><span class="sxs-lookup"><span data-stu-id="69b8c-3871">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-3872">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-3872">Storage</span></span>

* <span data-ttu-id="69b8c-3873">Habilitar atualização de conta de armazenamento com a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="69b8c-3873">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="69b8c-3874">VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-3874">VM</span></span>

* <span data-ttu-id="69b8c-3875">`availability-set`: exposta a contagem de domínios de falha durante a conversão</span><span class="sxs-lookup"><span data-stu-id="69b8c-3875">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="69b8c-3876">Exposto o comando `list-skus`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3876">Exposed `list-skus` command</span></span>
* <span data-ttu-id="69b8c-3877">Suporte para atribuir identidade sem criar atribuições de função</span><span class="sxs-lookup"><span data-stu-id="69b8c-3877">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="69b8c-3878">Aplicar o SKU de armazenamento ao anexar discos de dados</span><span class="sxs-lookup"><span data-stu-id="69b8c-3878">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="69b8c-3879">Removido o nome do disco do sistema operacional padrão e SKU de armazenamento ao usar discos gerenciados</span><span class="sxs-lookup"><span data-stu-id="69b8c-3879">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="69b8c-3880">28 de julho de 2017</span><span class="sxs-lookup"><span data-stu-id="69b8c-3880">July 28, 2017</span></span>

<span data-ttu-id="69b8c-3881">Versão 2.0.12</span><span class="sxs-lookup"><span data-stu-id="69b8c-3881">Version 2.0.12</span></span>

* <span data-ttu-id="69b8c-3882">Adicionado os comandos de contêiner</span><span class="sxs-lookup"><span data-stu-id="69b8c-3882">Added container commands</span></span>
* <span data-ttu-id="69b8c-3883">Adicionados módulos de cobrança e de consumo</span><span class="sxs-lookup"><span data-stu-id="69b8c-3883">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="69b8c-3884">Núcleo</span><span class="sxs-lookup"><span data-stu-id="69b8c-3884">Core</span></span>

* <span data-ttu-id="69b8c-3885">Informações de autenticação de SDK de saída para entidades de serviço com certificados</span><span class="sxs-lookup"><span data-stu-id="69b8c-3885">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="69b8c-3886">Corrigidas as exceções de andamento da implantação</span><span class="sxs-lookup"><span data-stu-id="69b8c-3886">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="69b8c-3887">Usar o ponto de extremidade do ARM da nuvem atual para criar cliente da assinatura</span><span class="sxs-lookup"><span data-stu-id="69b8c-3887">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="69b8c-3888">Melhor manipulação simultânea do arquivo clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="69b8c-3888">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="69b8c-3889">Atualização da ID de solicitação do cliente para cada execução de comando</span><span class="sxs-lookup"><span data-stu-id="69b8c-3889">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="69b8c-3890">Criar clientes de assinatura com o perfil correto do SDK (#3635)</span><span class="sxs-lookup"><span data-stu-id="69b8c-3890">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="69b8c-3891">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="69b8c-3891">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="69b8c-3892">Adicionado suporte para escolher campos de saída da tabela através da consulta JMESpath (#3581)</span><span class="sxs-lookup"><span data-stu-id="69b8c-3892">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="69b8c-3893">Aprimoramento da desativação de áudio de argumentos de análise e da adição do histórico com gestos (#3434)</span><span class="sxs-lookup"><span data-stu-id="69b8c-3893">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="69b8c-3894">Criar clientes de assinatura com o perfil correto do SDK</span><span class="sxs-lookup"><span data-stu-id="69b8c-3894">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="69b8c-3895">Mover todos os arquivos existentes de gravação para a pasta mais recente</span><span class="sxs-lookup"><span data-stu-id="69b8c-3895">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="69b8c-3896">Corrigida a idempotência para a criação de VM/VMSS (#3586)</span><span class="sxs-lookup"><span data-stu-id="69b8c-3896">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="69b8c-3897">Os caminhos de comando não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="69b8c-3897">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="69b8c-3898">Determinados parâmetros do tipo booliano não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="69b8c-3898">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="69b8c-3899">Suporte para logon do ADFS em um servidor local como o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="69b8c-3899">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="69b8c-3900">Corrigidas as gravações simultâneas para clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="69b8c-3900">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="69b8c-3901">ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-3901">ACR</span></span>

* <span data-ttu-id="69b8c-3902">Adicionado o comando `show-usage` para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="69b8c-3902">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="69b8c-3903">Suporte para atualização do SKU para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="69b8c-3903">Support SKU update for managed registries</span></span>
* <span data-ttu-id="69b8c-3904">Adicionados registros gerenciados com o SKU gerenciado</span><span class="sxs-lookup"><span data-stu-id="69b8c-3904">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="69b8c-3905">Adicionados webhooks para registros gerenciados com o módulo de comando de webhook do ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-3905">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="69b8c-3906">Adicionada autenticação do AAD com o comando de logon de ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-3906">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="69b8c-3907">Adicionado comando de exclusão para marcas, manifestos e repositórios do Docker</span><span class="sxs-lookup"><span data-stu-id="69b8c-3907">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="69b8c-3908">ACS</span><span class="sxs-lookup"><span data-stu-id="69b8c-3908">ACS</span></span>

* <span data-ttu-id="69b8c-3909">Suporte para a API versão 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="69b8c-3909">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-3910">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-3910">Appservice</span></span>

* <span data-ttu-id="69b8c-3911">Corrigido o bug onde listar o aplicativo Web Linux não retornava nada</span><span class="sxs-lookup"><span data-stu-id="69b8c-3911">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="69b8c-3912">Suporte para recuperar credenciais de ACR</span><span class="sxs-lookup"><span data-stu-id="69b8c-3912">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="69b8c-3913">Remover todos os comandos em `appservice web`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3913">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="69b8c-3914">Ocultar as senhas de registro do Docker da saída do comando (#3656)</span><span class="sxs-lookup"><span data-stu-id="69b8c-3914">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="69b8c-3915">Verifique se o navegador padrão é usado no macOS sem erros (#3623)</span><span class="sxs-lookup"><span data-stu-id="69b8c-3915">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="69b8c-3916">Aprimorada a Ajuda de `webapp log tail` e `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="69b8c-3916">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="69b8c-3917">Exposto o comando `traffic-routing` para configurar roteamento estático (#3566)</span><span class="sxs-lookup"><span data-stu-id="69b8c-3917">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="69b8c-3918">Adicionadas correções de confiabilidade na configuração de controle do código-fonte (#3245)</span><span class="sxs-lookup"><span data-stu-id="69b8c-3918">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="69b8c-3919">Removido o argumento `--node-version` sem suporte de `webapp config update` para aplicativos Web do Windows.</span><span class="sxs-lookup"><span data-stu-id="69b8c-3919">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="69b8c-3920">Em vez disso, use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3920">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="69b8c-3921">Lote</span><span class="sxs-lookup"><span data-stu-id="69b8c-3921">Batch</span></span>

* <span data-ttu-id="69b8c-3922">Atualizado para o Lote SDK 3.0.0 com suporte para VMs de baixa prioridade em pools</span><span class="sxs-lookup"><span data-stu-id="69b8c-3922">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="69b8c-3923">Opção `pool create` renomeada como `--target-dedicated` para `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3923">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="69b8c-3924">Adicionadas as opções `pool create` e `--target-low-priority-nodes` de `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3924">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="69b8c-3925">CDN</span><span class="sxs-lookup"><span data-stu-id="69b8c-3925">CDN</span></span>

* <span data-ttu-id="69b8c-3926">Uma mensagem de erro mais adequada foi fornecida para `cdn endpoint list` quando o perfil especificado por `--profile-name` não existir</span><span class="sxs-lookup"><span data-stu-id="69b8c-3926">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="69b8c-3927">Nuvem</span><span class="sxs-lookup"><span data-stu-id="69b8c-3927">Cloud</span></span>

* <span data-ttu-id="69b8c-3928">Alterada a versão de API do ponto de extremidade de metadados de nuvem para o formato AAAA-MM-DD</span><span class="sxs-lookup"><span data-stu-id="69b8c-3928">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="69b8c-3929">Ponto de extremidade da galeria não é necessário</span><span class="sxs-lookup"><span data-stu-id="69b8c-3929">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="69b8c-3930">Suporte para registrar a nuvem somente com o ponto de extremidade de gerenciador de recursos do ARM</span><span class="sxs-lookup"><span data-stu-id="69b8c-3930">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="69b8c-3931">Fornecida uma opção para `cloud set` para escolher o perfil ao selecionar a nuvem atual</span><span class="sxs-lookup"><span data-stu-id="69b8c-3931">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="69b8c-3932">Exposto `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3932">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="69b8c-3933">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="69b8c-3933">CosmosDB</span></span>

* <span data-ttu-id="69b8c-3934">Corrigida a permissão para criação de coleção com chave de partição personalizada</span><span class="sxs-lookup"><span data-stu-id="69b8c-3934">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="69b8c-3935">Adicionado suporte para o TTL padrão de coleção</span><span class="sxs-lookup"><span data-stu-id="69b8c-3935">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="69b8c-3936">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="69b8c-3936">Data Lake Analytics</span></span>

* <span data-ttu-id="69b8c-3937">Adicionados comandos para gerenciamento de política de computação sob o título `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3937">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="69b8c-3938">Adicionado `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3938">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="69b8c-3939">Adicionado `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3939">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="69b8c-3940">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="69b8c-3940">Data Lake Store</span></span>

* <span data-ttu-id="69b8c-3941">Adicionado suporte para a rotação de chave de cofre de chaves gerenciado do usuário em `dls account update`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3941">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="69b8c-3942">Atualizada a versão SDK do sistema de arquivos do Data Lake Store subjacente para resolver um problema de desempenho</span><span class="sxs-lookup"><span data-stu-id="69b8c-3942">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="69b8c-3943">Adicionado o comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="69b8c-3943">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="69b8c-3944">Esse comando tenta permitir que um Cofre de Chaves fornecido pelo usuário use a criptografia de dados em uma conta do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="69b8c-3944">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="69b8c-3945">Interativo</span><span class="sxs-lookup"><span data-stu-id="69b8c-3945">Interactive</span></span>

* <span data-ttu-id="69b8c-3946">Melhor tempo de inicialização, usando comandos em cache</span><span class="sxs-lookup"><span data-stu-id="69b8c-3946">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="69b8c-3947">Maior cobertura de teste</span><span class="sxs-lookup"><span data-stu-id="69b8c-3947">Increased test coverage</span></span>
* <span data-ttu-id="69b8c-3948">Aprimorado o gesto “?” para injetar também o próximo comando</span><span class="sxs-lookup"><span data-stu-id="69b8c-3948">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="69b8c-3949">Corrigidos os erros interativos com o perfil 2017-03-09-profile-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="69b8c-3949">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="69b8c-3950">Permitido `--version` como um parâmetro para o modo interativo (#3645)</span><span class="sxs-lookup"><span data-stu-id="69b8c-3950">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="69b8c-3951">Impedir que o modo interativo gere erros de conclusões de validação (#3570)</span><span class="sxs-lookup"><span data-stu-id="69b8c-3951">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="69b8c-3952">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="69b8c-3952">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="69b8c-3953">Adicionado o sinalizador `--progress`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3953">Added `--progress` flag</span></span>
* <span data-ttu-id="69b8c-3954">Removidos `--debug` e `--verbose` de conclusões</span><span class="sxs-lookup"><span data-stu-id="69b8c-3954">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="69b8c-3955">Removido `interactive` de conclusões (#3324)</span><span class="sxs-lookup"><span data-stu-id="69b8c-3955">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="69b8c-3956">IoT</span><span class="sxs-lookup"><span data-stu-id="69b8c-3956">IoT</span></span>

* <span data-ttu-id="69b8c-3957">A criação de uma política não limpa as políticas existentes.</span><span class="sxs-lookup"><span data-stu-id="69b8c-3957">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="69b8c-3958">(#3934)</span><span class="sxs-lookup"><span data-stu-id="69b8c-3958">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="69b8c-3959">Cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="69b8c-3959">Key vault</span></span>

* <span data-ttu-id="69b8c-3960">Comandos adicionados para recursos de recuperação do cofre de chaves:</span><span class="sxs-lookup"><span data-stu-id="69b8c-3960">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="69b8c-3961">Subcomandos `purge`, `recover`, `keyvault list-deleted` de `keyvault`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3961">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="69b8c-3962">Subcomandos `backup`, `restore`, `purge`, `recover`, `list-deleted` de `keyvault secret`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3962">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="69b8c-3963">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault certificate`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3963">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="69b8c-3964">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault key`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3964">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="69b8c-3965">Adicionada a integração do cofre de chaves da entidade de serviço (#3133)</span><span class="sxs-lookup"><span data-stu-id="69b8c-3965">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="69b8c-3966">Atualizado o plano de dados de cofre de chaves para 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="69b8c-3966">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="69b8c-3967">(#3307)</span><span class="sxs-lookup"><span data-stu-id="69b8c-3967">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="69b8c-3968">Laboratório</span><span class="sxs-lookup"><span data-stu-id="69b8c-3968">Lab</span></span>

* <span data-ttu-id="69b8c-3969">Adicionado o suporte para reivindicar qualquer VM no laboratório através de `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3969">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="69b8c-3970">Adicionado o formatador de saída da tabela para `az lab vm list` e `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3970">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="69b8c-3971">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="69b8c-3971">Monitor</span></span>

* <span data-ttu-id="69b8c-3972">Correção para o arquivo de modelo com o comando `monitor autoscale-settings get-parameters-template` (#3349)</span><span class="sxs-lookup"><span data-stu-id="69b8c-3972">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="69b8c-3973">`monitor alert-rule-incidents list` renomeado para `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3973">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="69b8c-3974">`monitor alert-rule-incidents show` renomeado para `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3974">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="69b8c-3975">`monitor metric-defintions list` renomeado para `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3975">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="69b8c-3976">`monitor alert-rules` renomeado para `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3976">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="69b8c-3977">Alterado `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="69b8c-3977">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="69b8c-3978">Os subcomandos `condition` e `action` não aceitarão mais JSON</span><span class="sxs-lookup"><span data-stu-id="69b8c-3978">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="69b8c-3979">Adicionar vários parâmetros para simplificar o processo de criação de regra</span><span class="sxs-lookup"><span data-stu-id="69b8c-3979">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="69b8c-3980">`location` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="69b8c-3980">`location` no longer required</span></span>
  * <span data-ttu-id="69b8c-3981">Adicionar nome e o suporte a ID de destino</span><span class="sxs-lookup"><span data-stu-id="69b8c-3981">Add name and ID support for target</span></span>
  * <span data-ttu-id="69b8c-3982">Remover `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3982">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="69b8c-3983">Renomear `is-enabled` para `enabled` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="69b8c-3983">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="69b8c-3984">Padrões de `description` agora baseados na condição fornecida</span><span class="sxs-lookup"><span data-stu-id="69b8c-3984">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="69b8c-3985">Adicionar exemplos para ajudar a esclarecer o novo formato</span><span class="sxs-lookup"><span data-stu-id="69b8c-3985">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="69b8c-3986">Suporte para nomes ou IDs para comandos `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3986">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="69b8c-3987">Exemplos e argumentos de conveniência adicionados ao `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3987">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-3988">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-3988">Network</span></span>

* <span data-ttu-id="69b8c-3989">Adicionado o comando `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3989">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="69b8c-3990">Adicionado argumento `--private-access-services` para `vnet subnet create` e `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3990">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="69b8c-3991">Corrigido o problema onde `application-gateway redirect-config create` falhava</span><span class="sxs-lookup"><span data-stu-id="69b8c-3991">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="69b8c-3992">Corrigido o problema onde `application-gateway redirect-config update` com `--no-wait` não funcionava</span><span class="sxs-lookup"><span data-stu-id="69b8c-3992">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="69b8c-3993">Corrigido o bug ao usar o argumento `--servers` com `application-gateway address-pool create` e `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3993">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="69b8c-3994">Adicionados os comandos `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3994">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="69b8c-3995">Adicionados os comandos para `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3995">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="69b8c-3996">Adicionados os argumentos para `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3996">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="69b8c-3997">Adicionados os argumentos para `application-gateway http-settings create` e `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3997">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="69b8c-3998">Adicionados os argumentos para `application-gateway url-path-map create` e `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3998">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="69b8c-3999">Adicionado o argumento `--redirect-config` para `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-3999">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="69b8c-4000">Adicionado o suporte ao `--no-wait` para `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="69b8c-4000">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="69b8c-4001">Adicionados os argumentos para `application-gateway probe create` e `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="69b8c-4001">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="69b8c-4002">Adicionado o argumento `--redirect-config` para `application-gateway rule create` e `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="69b8c-4002">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="69b8c-4003">Adicionado o suporte ao `--accelerated-networking` para `nic create` e `nic update`</span><span class="sxs-lookup"><span data-stu-id="69b8c-4003">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="69b8c-4004">Removido o argumento `--internal-dns-name-suffix` de `nic create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-4004">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="69b8c-4005">Adicionado o suporte ao `--dns-servers` para `nic update` e `nic create`: Adicionar suporte para --dns-servers</span><span class="sxs-lookup"><span data-stu-id="69b8c-4005">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="69b8c-4006">Corrigido o bug onde `local-gateway create` ignorava `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="69b8c-4006">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="69b8c-4007">Adicionado o suporte ao `--dns-servers` para `vnet update`</span><span class="sxs-lookup"><span data-stu-id="69b8c-4007">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="69b8c-4008">Corrigido o bug ao criar um emparelhamento sem filtragem de rotas com `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-4008">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="69b8c-4009">Corrigido o bug onde os argumentos `--provider` e `--bandwidth` não funcionavam com `express-route update`</span><span class="sxs-lookup"><span data-stu-id="69b8c-4009">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="69b8c-4010">Corrigido o bug com a lógica padrão de `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="69b8c-4010">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="69b8c-4011">Aprimorada a formatação de saída para `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="69b8c-4011">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="69b8c-4012">Usar IP de front-end padrão para `application-gateway http-listener create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="69b8c-4012">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="69b8c-4013">Usar o pool padrão de endereços, configurações de HTTP e o ouvinte HTTP para `application-gateway rule create`, se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="69b8c-4013">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="69b8c-4014">Usar IP de front-end e pool de back-end padrão para `lb rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="69b8c-4014">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="69b8c-4015">Usar IP de front-end padrão para `lb inbound-nat-rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="69b8c-4015">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="69b8c-4016">Perfil</span><span class="sxs-lookup"><span data-stu-id="69b8c-4016">Profile</span></span>

* <span data-ttu-id="69b8c-4017">Suporte a logon em uma VM com uma identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="69b8c-4017">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="69b8c-4018">Suporte a saída para `account show` em formato de arquivo de autenticação do SDK</span><span class="sxs-lookup"><span data-stu-id="69b8c-4018">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="69b8c-4019">Mostrar avisos de código obsoleto ao usar o “modo de exibição expandido”</span><span class="sxs-lookup"><span data-stu-id="69b8c-4019">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="69b8c-4020">Adicionado o comando `get-access-token` para fornecer o token bruto do AAD</span><span class="sxs-lookup"><span data-stu-id="69b8c-4020">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="69b8c-4021">Suporte a logon com uma conta de usuário sem nenhuma assinatura associada</span><span class="sxs-lookup"><span data-stu-id="69b8c-4021">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="69b8c-4022">RDBMS</span><span class="sxs-lookup"><span data-stu-id="69b8c-4022">RDBMS</span></span>

* <span data-ttu-id="69b8c-4023">Suporte para listar servidores em uma assinatura (#3417)</span><span class="sxs-lookup"><span data-stu-id="69b8c-4023">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="69b8c-4024">Corrigido o `%s` não processado devido à ausência de `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="69b8c-4024">Fixed `%s` not processed because of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="69b8c-4025">Corrigido o mapa do código-fonte do documento e adicionada a tarefa CI para verificação (#3361)</span><span class="sxs-lookup"><span data-stu-id="69b8c-4025">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="69b8c-4026">Corrigida a ajuda de MySQL e PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="69b8c-4026">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="69b8c-4027">Recurso</span><span class="sxs-lookup"><span data-stu-id="69b8c-4027">Resource</span></span>

* <span data-ttu-id="69b8c-4028">Aprimorados os prompts para parâmetros ausentes para `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-4028">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="69b8c-4029">Aprimorada a análise da sintaxe `--parameters KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="69b8c-4029">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="69b8c-4030">Corrigidos os problemas onde os arquivos de parâmetros `group deployment create` não eram mais reconhecidos usando a sintaxe `@<file>`</span><span class="sxs-lookup"><span data-stu-id="69b8c-4030">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="69b8c-4031">Suporte do argumento `--ids` para os comandos `resource` e `managedapp`</span><span class="sxs-lookup"><span data-stu-id="69b8c-4031">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="69b8c-4032">Corrigidas algumas mensagens de erro e análise (#3584)</span><span class="sxs-lookup"><span data-stu-id="69b8c-4032">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="69b8c-4033">Corrigida a análise de `--resource-type` para o comando `lock` aceitar `<resource-namespace>` e `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="69b8c-4033">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="69b8c-4034">Adicionados parâmetros de verificação para modelos de link do modelo (#3629)</span><span class="sxs-lookup"><span data-stu-id="69b8c-4034">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="69b8c-4035">Adicionado suporte para especificar parâmetros de implantação usando a sintaxe `KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="69b8c-4035">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="69b8c-4036">Função</span><span class="sxs-lookup"><span data-stu-id="69b8c-4036">Role</span></span>

* <span data-ttu-id="69b8c-4037">Suporte à saída no formato de arquivo de autenticação do SDK para `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="69b8c-4037">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="69b8c-4038">Limpar as atribuições de função e aplicativos relacionados ao AAD ao excluir uma entidade de serviço (#3610)</span><span class="sxs-lookup"><span data-stu-id="69b8c-4038">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="69b8c-4039">Incluir o formato de hora nos argumentos `app create` e descrições `--start-date` e `--end-date`</span><span class="sxs-lookup"><span data-stu-id="69b8c-4039">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="69b8c-4040">Mostrar avisos de código obsoleto ao usar `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="69b8c-4040">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="69b8c-4041">Adicionada a integração do cofre de chaves para os comandos `create-for-rbac` e `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="69b8c-4041">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="69b8c-4042">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="69b8c-4042">Service Fabric</span></span>
* <span data-ttu-id="69b8c-4043">Corrigido um problema com arquivos grandes em aplicativos que eram truncados ao serem carregados (#3666)</span><span class="sxs-lookup"><span data-stu-id="69b8c-4043">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="69b8c-4044">Adicionados testes para os comandos do Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="69b8c-4044">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="69b8c-4045">Corrigidos vários comandos do Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="69b8c-4045">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="69b8c-4046">SQL</span><span class="sxs-lookup"><span data-stu-id="69b8c-4046">SQL</span></span>

* <span data-ttu-id="69b8c-4047">Removido o parâmetro `sql server create` `--identity` desfeito</span><span class="sxs-lookup"><span data-stu-id="69b8c-4047">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="69b8c-4048">Remover os valores de senha da saída dos comandos `sql server create` e `sql server update`</span><span class="sxs-lookup"><span data-stu-id="69b8c-4048">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="69b8c-4049">Adicionados os comandos para `sql db list-editions` e `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="69b8c-4049">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-4050">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-4050">Storage</span></span>

* <span data-ttu-id="69b8c-4051">Removida a opção `--marker` dos comandos `storage blob list`, `storage container list`, e `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="69b8c-4051">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="69b8c-4052">Habilitado a criação de uma conta de armazenamento somente para https</span><span class="sxs-lookup"><span data-stu-id="69b8c-4052">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="69b8c-4053">Atualizadas as métricas de armazenamento, registro em log e os comandos do CORS (#3495)</span><span class="sxs-lookup"><span data-stu-id="69b8c-4053">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="69b8c-4054">Mensagem de exceção reformulada do ADD do CORS adicionar (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="69b8c-4054">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="69b8c-4055">Convertido o gerador para uma lista no modo de simulação de comando do lote de download (#3592)</span><span class="sxs-lookup"><span data-stu-id="69b8c-4055">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="69b8c-4056">Corrigido o problema de simulação do lote de download de blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="69b8c-4056">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="69b8c-4057">VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-4057">VM</span></span>

* <span data-ttu-id="69b8c-4058">Suporte para configuração de NSG</span><span class="sxs-lookup"><span data-stu-id="69b8c-4058">Support configuring nsg</span></span>
* <span data-ttu-id="69b8c-4059">Corrigido o bug onde o servidor DNS não era configurado corretamente</span><span class="sxs-lookup"><span data-stu-id="69b8c-4059">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="69b8c-4060">Suporte às identidades de serviço gerenciado</span><span class="sxs-lookup"><span data-stu-id="69b8c-4060">Support managed service identities</span></span>
* <span data-ttu-id="69b8c-4061">Corrigido o problema onde `cmss create` com um balanceador de carga existente exigia `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="69b8c-4061">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="69b8c-4062">Os discos de dados criados com LUN do `vm image create` agora começam com 0</span><span class="sxs-lookup"><span data-stu-id="69b8c-4062">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="69b8c-4063">10 de maio de 2017</span><span class="sxs-lookup"><span data-stu-id="69b8c-4063">May 10, 2017</span></span>

<span data-ttu-id="69b8c-4064">Versão 2.0.6</span><span class="sxs-lookup"><span data-stu-id="69b8c-4064">Version 2.0.6</span></span>

* <span data-ttu-id="69b8c-4065">Renomeação do DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="69b8c-4065">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="69b8c-4066">Adição do RDBMS (MySQL, Postgres)</span><span class="sxs-lookup"><span data-stu-id="69b8c-4066">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="69b8c-4067">Inclusão dos módulos Data Lake Analytics e Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="69b8c-4067">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="69b8c-4068">Inclusão do módulo Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="69b8c-4068">Include Cognitive Services module</span></span>
* <span data-ttu-id="69b8c-4069">Inclusão do módulo Service Fabric</span><span class="sxs-lookup"><span data-stu-id="69b8c-4069">Include Service Fabric module</span></span>
* <span data-ttu-id="69b8c-4070">Inclusão do módulo Interativo (renomeação de az-shell)</span><span class="sxs-lookup"><span data-stu-id="69b8c-4070">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="69b8c-4071">Adição de suporte para comandos CDN</span><span class="sxs-lookup"><span data-stu-id="69b8c-4071">Add support for CDN commands</span></span>
* <span data-ttu-id="69b8c-4072">Remoção do módulo Contêiner</span><span class="sxs-lookup"><span data-stu-id="69b8c-4072">Remove Container module</span></span>
* <span data-ttu-id="69b8c-4073">Adição de “az -v” como atalho para “az --version” ([nº 2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4073">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="69b8c-4074">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4074">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="69b8c-4075">Núcleo</span><span class="sxs-lookup"><span data-stu-id="69b8c-4075">Core</span></span>

* <span data-ttu-id="69b8c-4076">núcleo: captura de exceções causadas por um provedor não registrado e seu registro automático</span><span class="sxs-lookup"><span data-stu-id="69b8c-4076">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="69b8c-4077">desempenho: persistência do cache de tokens do ADAL na memória até o encerramento do processo ([nº 2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4077">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="69b8c-4078">Correção de bytes retornados da impressão digital hexadecimal -o tsv ([nº 3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4078">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="69b8c-4079">Melhoria do download do Certificado do Key Vault e da integração de SP do AAD ([nº 3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4079">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="69b8c-4080">Adição da localização do Python a “az —version” ([nº 2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4080">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="69b8c-4081">logon: suporte ao logon quando não há nenhuma assinatura ([nº 2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4081">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="69b8c-4082">núcleo: correção de uma falha ao fazer logon usando uma entidade de serviço duas vezes ([nº 2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4082">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="69b8c-4083">núcleo: permitir que o caminho do arquivo accessTokens.json seja configurável por meio de uma variável de ambiente ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4083">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="69b8c-4084">núcleo: permitir que padrões configurados sejam aplicados em argumentos opcionais ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4084">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="69b8c-4085">núcleo: desempenho aprimorado</span><span class="sxs-lookup"><span data-stu-id="69b8c-4085">core: Improved performance</span></span>
* <span data-ttu-id="69b8c-4086">núcleo: certificados de AC personalizados – suporte à configuração da variável de ambiente REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="69b8c-4086">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="69b8c-4087">núcleo: configuração na nuvem – uso do ponto de extremidade do “Resource Manager” caso o ponto de extremidade de “Gerenciamento” não esteja definido</span><span class="sxs-lookup"><span data-stu-id="69b8c-4087">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="69b8c-4088">ACS</span><span class="sxs-lookup"><span data-stu-id="69b8c-4088">ACS</span></span>

* <span data-ttu-id="69b8c-4089">correção da contagem mestre e de agente para ser inteiro em vez de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69b8c-4089">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="69b8c-4090">exposição de “az acs create --no-wait” e “az acs wait” para a criação assíncrona</span><span class="sxs-lookup"><span data-stu-id="69b8c-4090">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="69b8c-4091">exposição de “az acs create --validate” para validações de simulação</span><span class="sxs-lookup"><span data-stu-id="69b8c-4091">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="69b8c-4092">remoção do perfil do Windows antes da chamada PUT ao comando scale ([nº 2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4092">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-4093">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-4093">AppService</span></span>

* <span data-ttu-id="69b8c-4094">functionapp: adição de suportes completos a functionapp, incluindo create, show, list, delete, hostname, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="69b8c-4094">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="69b8c-4095">Adição do VSTS (Team Services) como uma opção de entrega contínua a “appservice web source-control config”</span><span class="sxs-lookup"><span data-stu-id="69b8c-4095">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="69b8c-4096">Criação de “az webapp” para substituição de “az appservice web” (para compatibilidade com versões anteriores, “az appservice web” permanecerá por duas versões)</span><span class="sxs-lookup"><span data-stu-id="69b8c-4096">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="69b8c-4097">Exposição de argumentos para configurar a implantação e as “pilhas em runtime” em webapp create</span><span class="sxs-lookup"><span data-stu-id="69b8c-4097">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="69b8c-4098">Exposição de “webapp list-runtimes”</span><span class="sxs-lookup"><span data-stu-id="69b8c-4098">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="69b8c-4099">suporte à configuração de cadeias de conexão ([nº 2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4099">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="69b8c-4100">suporte à permuta de slots com visualização</span><span class="sxs-lookup"><span data-stu-id="69b8c-4100">support slot swap with preview</span></span>
* <span data-ttu-id="69b8c-4101">Correção de erros em comandos appservice ([nº 2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4101">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="69b8c-4102">Uso do grupo de recursos do plano do serviço de aplicativo para operações de certificado ([nº 2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4102">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="69b8c-4103">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="69b8c-4103">CosmosDB</span></span>

* <span data-ttu-id="69b8c-4104">Renomeação do módulo DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="69b8c-4104">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="69b8c-4105">Adição de suporte para APIs do plano de dados do DocumentDB: gerenciamento de banco de dados e de coleção</span><span class="sxs-lookup"><span data-stu-id="69b8c-4105">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="69b8c-4106">Adição de suporte para habilitar o failover automático em contas de banco de dados</span><span class="sxs-lookup"><span data-stu-id="69b8c-4106">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="69b8c-4107">Adição de suporte para nova política de consistência ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="69b8c-4107">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="69b8c-4108">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="69b8c-4108">Data Lake Analytics</span></span>

* <span data-ttu-id="69b8c-4109">Correção de um bug em que a filtragem no resultado e no estado das listas de trabalho gera um erro</span><span class="sxs-lookup"><span data-stu-id="69b8c-4109">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="69b8c-4110">Adição de suporte para o novo tipo de item de catálogo: pacote.</span><span class="sxs-lookup"><span data-stu-id="69b8c-4110">Add support for new catalog item type: package.</span></span> <span data-ttu-id="69b8c-4111">acessado por meio de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="69b8c-4111">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="69b8c-4112">Possibilidade de listar os seguintes itens de catálogo no banco de dados (sem a necessidade de especificação de esquema):</span><span class="sxs-lookup"><span data-stu-id="69b8c-4112">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="69b8c-4113">Tabela</span><span class="sxs-lookup"><span data-stu-id="69b8c-4113">Table</span></span>
  * <span data-ttu-id="69b8c-4114">Função com valor de tabela</span><span class="sxs-lookup"><span data-stu-id="69b8c-4114">Table valued function</span></span>
  * <span data-ttu-id="69b8c-4115">Visualizar</span><span class="sxs-lookup"><span data-stu-id="69b8c-4115">View</span></span>
  * <span data-ttu-id="69b8c-4116">Estatísticas de Tabela.</span><span class="sxs-lookup"><span data-stu-id="69b8c-4116">Table Statistics.</span></span> <span data-ttu-id="69b8c-4117">Isso também pode ser listado com um esquema, mas sem a especificação de um nome de tabela</span><span class="sxs-lookup"><span data-stu-id="69b8c-4117">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="69b8c-4118">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="69b8c-4118">Data Lake Store</span></span>

* <span data-ttu-id="69b8c-4119">Atualização da versão do SDK do sistema de arquivos subjacente, que fornece melhor suporte para lidar com cenários de limitação do servidor</span><span class="sxs-lookup"><span data-stu-id="69b8c-4119">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="69b8c-4120">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4120">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="69b8c-4121">Ausência de ajuda para mostrar o acesso.</span><span class="sxs-lookup"><span data-stu-id="69b8c-4121">missed help for access show.</span></span> <span data-ttu-id="69b8c-4122">Adição em andamento.</span><span class="sxs-lookup"><span data-stu-id="69b8c-4122">adding it.</span></span> <span data-ttu-id="69b8c-4123">([nº 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4123">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="69b8c-4124">Localizar</span><span class="sxs-lookup"><span data-stu-id="69b8c-4124">Find</span></span>

* <span data-ttu-id="69b8c-4125">melhoria dos resultados da pesquisa e permissão de controle de versão do índice de pesquisa</span><span class="sxs-lookup"><span data-stu-id="69b8c-4125">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="69b8c-4126">KeyVault</span><span class="sxs-lookup"><span data-stu-id="69b8c-4126">KeyVault</span></span>

* <span data-ttu-id="69b8c-4127">BC:`az keyvault certificate download` alteração de -e da cadeia de caracteres ou do binário para PEM ou DER a fim de representar melhor as opções</span><span class="sxs-lookup"><span data-stu-id="69b8c-4127">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="69b8c-4128">BC: remoção de --expires e --not-before de `keyvault certificate create`, pois estes parâmetros não têm suporte no serviço</span><span class="sxs-lookup"><span data-stu-id="69b8c-4128">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="69b8c-4129">Adição do parâmetro --validity a `keyvault certificate create` para substituir seletivamente o valor em --policy</span><span class="sxs-lookup"><span data-stu-id="69b8c-4129">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="69b8c-4130">Correção do problema em `keyvault certificate get-default-policy`, em que “expires” e “not_before” eram expostos, ao contrário de “validity_in_months”</span><span class="sxs-lookup"><span data-stu-id="69b8c-4130">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="69b8c-4131">Correção do cofre de chaves para importação de PEM e PFX ([nº 2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4131">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="69b8c-4132">Laboratório</span><span class="sxs-lookup"><span data-stu-id="69b8c-4132">Lab</span></span>

* <span data-ttu-id="69b8c-4133">Adição dos comandos create, show, delete e list ao ambiente do laboratório</span><span class="sxs-lookup"><span data-stu-id="69b8c-4133">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="69b8c-4134">Adição dos comandos show e list para exibir modelos ARM no laboratório</span><span class="sxs-lookup"><span data-stu-id="69b8c-4134">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="69b8c-4135">Adição do sinalizador --environment a `az lab vm list` para filtrar as VMs por ambiente no laboratório</span><span class="sxs-lookup"><span data-stu-id="69b8c-4135">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="69b8c-4136">Adição do comando de conveniência `az lab formula export-artifacts` para exportar o scaffold de artefato em uma fórmula do Laboratório</span><span class="sxs-lookup"><span data-stu-id="69b8c-4136">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="69b8c-4137">Adição de comandos para gerenciar segredos em um Laboratório</span><span class="sxs-lookup"><span data-stu-id="69b8c-4137">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="69b8c-4138">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="69b8c-4138">Monitor</span></span>

* <span data-ttu-id="69b8c-4139">Correção de bug: modelagem de `--actions` de `az alert-rules create` para consumir a cadeia de caracteres JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4139">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="69b8c-4140">Correção de bug – as configurações de diagnóstico criam, mas não aceitam logs e métrica de comandos show ([nº 2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4140">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="69b8c-4141">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-4141">Network</span></span>

* <span data-ttu-id="69b8c-4142">Adição do comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="69b8c-4142">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="69b8c-4143">Adição de suporte para o parâmetro `--filters` de `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-4143">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="69b8c-4144">Adição de suporte para drenagem de conexão do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="69b8c-4144">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="69b8c-4145">Adição de suporte para a configuração do conjunto de regras WAF do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="69b8c-4145">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="69b8c-4146">Adição de suporte para filtros de rota e regras do ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="69b8c-4146">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="69b8c-4147">Adição de suporte para o roteamento geográfico do Gerenciador de Tráfego</span><span class="sxs-lookup"><span data-stu-id="69b8c-4147">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="69b8c-4148">Adição de suporte para seletores de tráfego baseados em política da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="69b8c-4148">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="69b8c-4149">Adição de suporte para políticas IPsec da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="69b8c-4149">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="69b8c-4150">Correção de um bug com `vpn-connection create` ao usar os parâmetros `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="69b8c-4150">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="69b8c-4151">Adição de suporte para gateways de VNet ativos/ativos</span><span class="sxs-lookup"><span data-stu-id="69b8c-4151">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="69b8c-4152">Remoção de valores nulos na saída de comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="69b8c-4152">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="69b8c-4153">BC: corrigido um bug na saída de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-4153">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="69b8c-4154">Correção de um bug em que o argumento “--key-length” de “vpn-connection create” não é analisado corretamente</span><span class="sxs-lookup"><span data-stu-id="69b8c-4154">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="69b8c-4155">Correção de um bug em `dns zone import`, em que os registros não são importados corretamente</span><span class="sxs-lookup"><span data-stu-id="69b8c-4155">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="69b8c-4156">Correção de um bug em que `traffic-manager endpoint update` não funciona</span><span class="sxs-lookup"><span data-stu-id="69b8c-4156">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="69b8c-4157">Adição de comandos de visualização “network watcher”</span><span class="sxs-lookup"><span data-stu-id="69b8c-4157">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="69b8c-4158">Perfil</span><span class="sxs-lookup"><span data-stu-id="69b8c-4158">Profile</span></span>

* <span data-ttu-id="69b8c-4159">Suporte ao logon quando não há nenhuma assinatura encontrada ([nº 2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4159">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="69b8c-4160">Suporte ao nome curto do parâmetro em az account set --subscription ([nº 2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4160">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="69b8c-4161">Redis</span><span class="sxs-lookup"><span data-stu-id="69b8c-4161">Redis</span></span>

* <span data-ttu-id="69b8c-4162">Adição do comando update que também adiciona a capacidade de dimensionar o Cache Redis</span><span class="sxs-lookup"><span data-stu-id="69b8c-4162">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="69b8c-4163">Preterição do comando “update-settings”</span><span class="sxs-lookup"><span data-stu-id="69b8c-4163">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="69b8c-4164">Recurso</span><span class="sxs-lookup"><span data-stu-id="69b8c-4164">Resource</span></span>

* <span data-ttu-id="69b8c-4165">Adição dos comandos de definição managedapp e managedapp ([nº 2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4165">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="69b8c-4166">Suporte aos comandos “provider operation” ([nº 2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4166">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="69b8c-4167">Suporte à criação de recurso genérico ([nº 2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4167">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="69b8c-4168">Correção da análise de recurso e da pesquisa de versão de API.</span><span class="sxs-lookup"><span data-stu-id="69b8c-4168">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="69b8c-4169">([nº 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4169">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="69b8c-4170">Adição de documentos a az lock update.</span><span class="sxs-lookup"><span data-stu-id="69b8c-4170">Add docs for az lock update.</span></span> <span data-ttu-id="69b8c-4171">([nº 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4171">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="69b8c-4172">Erro ao tentar listar recursos de um grupo que não existe.</span><span class="sxs-lookup"><span data-stu-id="69b8c-4172">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="69b8c-4173">([nº 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4173">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="69b8c-4174">[Computação] Correção de problemas com a atualização do conjunto de disponibilidade da VMSS e da VM.</span><span class="sxs-lookup"><span data-stu-id="69b8c-4174">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="69b8c-4175">([nº 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4175">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="69b8c-4176">Correção de lock create e delete se parent-resource-path é None ([nº 2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4176">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="69b8c-4177">Função</span><span class="sxs-lookup"><span data-stu-id="69b8c-4177">Role</span></span>

* <span data-ttu-id="69b8c-4178">create-for-rbac: garantia de que a data de término do SP não excederá a data de validade do certificado ([nº 2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4178">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="69b8c-4179">RBAC: adição de suporte completo a “ad group” ([nº 2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4179">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="69b8c-4180">função: correção de problemas na atualização de definição de função ([nº 2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4180">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="69b8c-4181">create-for-rbac: garantia de que a senha fornecida pelo usuário é coletada</span><span class="sxs-lookup"><span data-stu-id="69b8c-4181">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="69b8c-4182">SQL</span><span class="sxs-lookup"><span data-stu-id="69b8c-4182">SQL</span></span>

* <span data-ttu-id="69b8c-4183">Adição dos comandos az sql server list-usages e az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="69b8c-4183">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="69b8c-4184">SQL – capacidade de se conectar diretamente ao provedor de recursos ([nº 2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4184">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="69b8c-4185">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-4185">Storage</span></span>

* <span data-ttu-id="69b8c-4186">Localização padrão da localização do grupo de recursos de `storage account create`</span><span class="sxs-lookup"><span data-stu-id="69b8c-4186">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="69b8c-4187">Adição de suporte para cópia incremental de blob</span><span class="sxs-lookup"><span data-stu-id="69b8c-4187">Add support for incremental blob copy</span></span>
* <span data-ttu-id="69b8c-4188">Adição de suporte para upload de blobs de blocos grandes</span><span class="sxs-lookup"><span data-stu-id="69b8c-4188">Add support for large block blob upload</span></span>
* <span data-ttu-id="69b8c-4189">Alteração do tamanho do bloco para 100MB quando o arquivo a ser carregado é maior que 200GB</span><span class="sxs-lookup"><span data-stu-id="69b8c-4189">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="69b8c-4190">VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-4190">VM</span></span>

* <span data-ttu-id="69b8c-4191">avail-set: as contagens de domínio de UD e FD agora são opcionais</span><span class="sxs-lookup"><span data-stu-id="69b8c-4191">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="69b8c-4192">observação: em comandos da VM em nuvens soberanas, evite recursos relacionados ao disco gerenciado, incluindo os seguintes:</span><span class="sxs-lookup"><span data-stu-id="69b8c-4192">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="69b8c-4193">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="69b8c-4193">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="69b8c-4194">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="69b8c-4194">az vm/vmss disk</span></span>
  3. <span data-ttu-id="69b8c-4195">Em “az vm/vmss create”, use “—use-unmanaged-disk” para evitar o disco gerenciado Outros comandos deverão funcionar</span><span class="sxs-lookup"><span data-stu-id="69b8c-4195">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="69b8c-4196">VM/VMSS: melhoria do texto de aviso ao gerar pares de chaves SSH</span><span class="sxs-lookup"><span data-stu-id="69b8c-4196">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="69b8c-4197">VM/VMSS: suporte à criação com base em uma imagem do Marketplace que exige informações de plano ([nº 1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4197">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="69b8c-4198">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="69b8c-4198">April 3, 2017</span></span>

<span data-ttu-id="69b8c-4199">Versão 2.0.2</span><span class="sxs-lookup"><span data-stu-id="69b8c-4199">Version 2.0.2</span></span>

<span data-ttu-id="69b8c-4200">Lançamos os componentes ACR, Batch, KeyVault, e SQL nessa versão</span><span class="sxs-lookup"><span data-stu-id="69b8c-4200">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="69b8c-4201">Núcleo</span><span class="sxs-lookup"><span data-stu-id="69b8c-4201">Core</span></span>

* <span data-ttu-id="69b8c-4202">Adicionar módulos acr, laboratório, monitor e localizar à lista padrão</span><span class="sxs-lookup"><span data-stu-id="69b8c-4202">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="69b8c-4203">Logon: ignorar locatário errado ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4203">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="69b8c-4204">logon: definir assinatura padrão como um com o estado de "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4204">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="69b8c-4205">Adicionar comandos de espera e suporte --no-wait para mais comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4205">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="69b8c-4206">núcleo: suporte a logon usando a entidade de serviço com um certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4206">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="69b8c-4207">Adicione solicitação para parâmetros de modelo ausentes.</span><span class="sxs-lookup"><span data-stu-id="69b8c-4207">Add prompting for missing template parameters.</span></span> <span data-ttu-id="69b8c-4208">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4208">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="69b8c-4209">Suporte à definição de valores padrão para os argumentos comuns como grupo de recursos padrão, Web padrão, vm padrão</span><span class="sxs-lookup"><span data-stu-id="69b8c-4209">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="69b8c-4210">Suporte a logon para um locatário específico</span><span class="sxs-lookup"><span data-stu-id="69b8c-4210">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="69b8c-4211">ACS</span><span class="sxs-lookup"><span data-stu-id="69b8c-4211">ACS</span></span>

* <span data-ttu-id="69b8c-4212">[ACS] Adicionar suporte para configurar um cluster do ACS padrão ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4212">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="69b8c-4213">Adicione suporte para solicitação de senha de chave ssh.</span><span class="sxs-lookup"><span data-stu-id="69b8c-4213">Add support for ssh key password prompting.</span></span> <span data-ttu-id="69b8c-4214">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4214">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="69b8c-4215">Adicione suporte para clusters do windows.</span><span class="sxs-lookup"><span data-stu-id="69b8c-4215">Add support for windows clusters.</span></span> <span data-ttu-id="69b8c-4216">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4216">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="69b8c-4217">Alterne da função Proprietário para Colaborador.</span><span class="sxs-lookup"><span data-stu-id="69b8c-4217">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="69b8c-4218">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4218">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="69b8c-4219">AppService</span><span class="sxs-lookup"><span data-stu-id="69b8c-4219">AppService</span></span>

* <span data-ttu-id="69b8c-4220">AppService: suporte para obter o endereço ip externo usado para registros de DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4220">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="69b8c-4221">AppService: suporte à associação de certificados curinga ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4221">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="69b8c-4222">AppService: lista de suporte à publicação de perfis ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4222">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="69b8c-4223">AppService - Aciona a sincronização de controle de origem após a configuração ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4223">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="69b8c-4224">DataLake</span><span class="sxs-lookup"><span data-stu-id="69b8c-4224">DataLake</span></span>

* <span data-ttu-id="69b8c-4225">Versão inicial do módulo do Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="69b8c-4225">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="69b8c-4226">Versão inicial do módulo do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="69b8c-4226">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="69b8c-4227">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="69b8c-4227">DocuemntDB</span></span>

* <span data-ttu-id="69b8c-4228">DocumentDB: adicionado suporte para a listagem de cadeias de conexão ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4228">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="69b8c-4229">VM</span><span class="sxs-lookup"><span data-stu-id="69b8c-4229">VM</span></span>

* <span data-ttu-id="69b8c-4230">[Compute] Adicionar suporte a AppGateway para criar o conjunto de dimensionamento de máquinas virtuais ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4230">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="69b8c-4231">[VM/VMSS] Suporte aprimorado ao cache de disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4231">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="69b8c-4232">VM/VMSS: incorporar a lógica de validação de credenciais usada pelo portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4232">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="69b8c-4233">Adicionar comandos de espera e suporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4233">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="69b8c-4234">Conjunto de dimensionamento de máquinas virtuais: suporte à \* para listar a exibição de instâncias em vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4234">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="69b8c-4235">Adicionar: segredos da VM e do conjunto de dimensionamento de máquinas virtuais ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4235">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="69b8c-4236">Permitir a criação de VMs com VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="69b8c-4236">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="69b8c-4237">27 de fevereiro de 2017</span><span class="sxs-lookup"><span data-stu-id="69b8c-4237">February 27, 2017</span></span>

<span data-ttu-id="69b8c-4238">Versão 2.0.0</span><span class="sxs-lookup"><span data-stu-id="69b8c-4238">Version 2.0.0</span></span>

<span data-ttu-id="69b8c-4239">Esta versão da CLI do Azure 2.0 é a primeira versão "Amplamente Disponível". A disponibilidade geral se aplica a estes módulos de comando:</span><span class="sxs-lookup"><span data-stu-id="69b8c-4239">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="69b8c-4240">Serviço de Contêiner (acs)</span><span class="sxs-lookup"><span data-stu-id="69b8c-4240">Container Service (acs)</span></span>
- <span data-ttu-id="69b8c-4241">Computação (incluindo Gerenciador de Recursos, VM, conjunto de dimensionamento de máquinas virtuais, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="69b8c-4241">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="69b8c-4242">Rede</span><span class="sxs-lookup"><span data-stu-id="69b8c-4242">Networking</span></span>
- <span data-ttu-id="69b8c-4243">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="69b8c-4243">Storage</span></span>

<span data-ttu-id="69b8c-4244">Esses módulos de comando podem ser usados na produção e têm suporte do SLA padrão da Microsoft. Você pode abrir problemas diretamente com o suporte da Microsoft ou em nossa [lista de problemas do github](https://github.com/azure/azure-cli/issues/). Faça perguntas no [StackOverflow usando a marca azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contate a equipe de produto em [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) Forneça comentários na linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="69b8c-4244">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="69b8c-4245">Os comandos nesses módulos são estáveis e a sintaxe não deve ser alterada em versões futuras dessa versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="69b8c-4245">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="69b8c-4246">Para verificar a versão da CLI, use `az --version` A saída lista a versão da CLI (2.0.0 nessa versão), os módulos de comando individuais, as versões do Python e GCC que você está usando</span><span class="sxs-lookup"><span data-stu-id="69b8c-4246">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="69b8c-4247">Alguns dos módulos de comando têm um sufixo "b *n* " ou "rc *n* ". Esses módulos de comando ainda estão em versão prévia e estarão disponíveis no futuro</span><span class="sxs-lookup"><span data-stu-id="69b8c-4247">Some of the command modules have a "b *n* " or "rc *n* " postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="69b8c-4248">Também temos compilações de versão prévia noturnas da CLI. Para obter informações, consulte essas instruções sobre [como obter as compilações diárias](https://github.com/Azure/azure-cli#nightly-builds) e essas instruções sobre [configuração do desenvolvedor e código de contribuição](https://github.com/Azure/azure-cli#developer-setup)</span><span class="sxs-lookup"><span data-stu-id="69b8c-4248">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="69b8c-4249">Você pode relatar problemas com as compilações de visualização diárias das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="69b8c-4249">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="69b8c-4250">Relatar problemas na [lista de problemas do github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="69b8c-4250">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="69b8c-4251">Entre em contato com a equipe do produto no endereço [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="69b8c-4251">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="69b8c-4252">Forneça comentários a partir da linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="69b8c-4252">Provide feedback from the command line with the `az feedback` command</span></span>

# <a name="beta-release-notes"></a>[<span data-ttu-id="69b8c-4253">Notas sobre a versão beta</span><span class="sxs-lookup"><span data-stu-id="69b8c-4253">Beta release notes</span></span>](#tab/azure-cli-beta)

<span data-ttu-id="69b8c-4254">A versão beta da CLI do Azure é uma migração do método de autenticação da plataforma AAD (v 1.0) para a [plataforma de Identidade da Microsoft (v 2.0)](/azure/active-directory/develop/v2-overview).</span><span class="sxs-lookup"><span data-stu-id="69b8c-4254">The Azure CLI beta release is a migration from the authentican method of AAD platform (v1.0) to [Microsoft Identity platform (v2.0)](/azure/active-directory/develop/v2-overview).</span></span>

## <a name="june-23-2020"></a><span data-ttu-id="69b8c-4255">23 de junho de 2020</span><span class="sxs-lookup"><span data-stu-id="69b8c-4255">June 23, 2020</span></span>

### <a name="things-to-know-about-the-new-azure-cli-beta-release"></a><span data-ttu-id="69b8c-4256">O que você precisa saber sobre a nova versão beta da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="69b8c-4256">Things to know about the new Azure CLI beta release</span></span>

-   <span data-ttu-id="69b8c-4257">A versão beta da CLI do Azure dá suporte a todos os comandos da CLI que você encontrará na versão lançada atual.</span><span class="sxs-lookup"><span data-stu-id="69b8c-4257">The beta version of the Azure CLI supports all CLI commands that you will find in the current released version.</span></span>
-   <span data-ttu-id="69b8c-4258">Fazer logon novamente é necessário após a instalação da versão beta.</span><span class="sxs-lookup"><span data-stu-id="69b8c-4258">Relogin is required after install the beta version.</span></span>
-   <span data-ttu-id="69b8c-4259">A versão beta dá suporte apenas à plataforma Windows.</span><span class="sxs-lookup"><span data-stu-id="69b8c-4259">The beta release only supports the Windows platform.</span></span>
-   <span data-ttu-id="69b8c-4260">Não há suporte para o Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="69b8c-4260">The Azure Stack is not supported.</span></span>
-   <span data-ttu-id="69b8c-4261">Não há suporte para o parâmetro `--use-cert-sn-issuer` ao usar a chave de entidade de serviço para se autenticar.</span><span class="sxs-lookup"><span data-stu-id="69b8c-4261">`--use-cert-sn-issuer` parameter is not supported when using service principal key to authenticate.</span></span>
-   <span data-ttu-id="69b8c-4262">Não há suporte para ignorar a verificação SSL por meio do ambiente `ADAL_PYTHON_SSL_NO_VERIFY`.</span><span class="sxs-lookup"><span data-stu-id="69b8c-4262">Skip SSL verification via environment `ADAL_PYTHON_SSL_NO_VERIFY` is not supported.</span></span>

<span data-ttu-id="69b8c-4263">Se você encontrar problemas com a versão beta, a equipe de engenharia da CLI do Azure ficará feliz por receber seus comentários no [GitHub](https://github.com/Azure/azure-cli/issues/new/choose).</span><span class="sxs-lookup"><span data-stu-id="69b8c-4263">If you find any issues in the beta release, the Azure CLI engineering team welcomes your comments on [GitHub](https://github.com/Azure/azure-cli/issues/new/choose).</span></span>

---
