---
title: Notas de versão da CLI do Azure
description: Saiba mais sobre as últimas atualizações da CLI do Azure
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 11/09/2020
ms.topic: article
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 02a7cf83bbd3de7dba69a75eeff0d6676d1e0952
ms.sourcegitcommit: 133d53a85073e3ce526a3de8de668e7bca79f48e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/11/2020
ms.locfileid: "94484002"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="3c5b0-103">Notas de versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="3c5b0-103">Azure CLI release notes</span></span>

# <a name="current-release-notes"></a>[<span data-ttu-id="3c5b0-104">Notas sobre a versão atuais</span><span class="sxs-lookup"><span data-stu-id="3c5b0-104">Current release notes</span></span>](#tab/azure-cli)

## <a name="november-09-2020"></a><span data-ttu-id="3c5b0-105">9 de novembro de 2020</span><span class="sxs-lookup"><span data-stu-id="3c5b0-105">November 09, 2020</span></span>

<span data-ttu-id="3c5b0-106">Versão 2.14.2</span><span class="sxs-lookup"><span data-stu-id="3c5b0-106">Version 2.14.2</span></span>

### <a name="app-service"></a><span data-ttu-id="3c5b0-107">Serviço de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-107">App Service</span></span>

* <span data-ttu-id="3c5b0-108">Correção nº 15604, nº 15605: adicionar suporte ao Dotnet5</span><span class="sxs-lookup"><span data-stu-id="3c5b0-108">Fix #15604, #15605: Add Dotnet5 support</span></span>

## <a name="november-06-2020"></a><span data-ttu-id="3c5b0-109">6 de novembro de 2020</span><span class="sxs-lookup"><span data-stu-id="3c5b0-109">November 06, 2020</span></span>

<span data-ttu-id="3c5b0-110">Versão 2.14.1</span><span class="sxs-lookup"><span data-stu-id="3c5b0-110">Version 2.14.1</span></span>

### <a name="arm"></a><span data-ttu-id="3c5b0-111">ARM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-111">ARM</span></span>

* <span data-ttu-id="3c5b0-112">Hotfix: adicionar suporte de cadeia de caracteres com várias linhas do TS para entradas de modelo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-112">Hotfix: Add TS multiline string support for template inputs</span></span>

## <a name="october-27-2020"></a><span data-ttu-id="3c5b0-113">27 de outubro de 2020</span><span class="sxs-lookup"><span data-stu-id="3c5b0-113">October 27, 2020</span></span>

<span data-ttu-id="3c5b0-114">Versão 2.14.0</span><span class="sxs-lookup"><span data-stu-id="3c5b0-114">Version 2.14.0</span></span>

### <a name="aks"></a><span data-ttu-id="3c5b0-115">AKS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-115">AKS</span></span>

* <span data-ttu-id="3c5b0-116">Adição de suporte a PPG</span><span class="sxs-lookup"><span data-stu-id="3c5b0-116">Add PPG support</span></span>
* <span data-ttu-id="3c5b0-117">Atualização do tempo limite máximo Standard Load Balancer para 100 minutos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-117">Update max standard load balancer timeout to 100 minutes</span></span>

### <a name="apim"></a><span data-ttu-id="3c5b0-118">APIM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-118">APIM</span></span>

* <span data-ttu-id="3c5b0-119">Correção de um problema com a criação da instância da camada de consumo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-119">Fix issue with creating consumption tier instance</span></span>

### <a name="app-config"></a><span data-ttu-id="3c5b0-120">Configuração do Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-120">App Config</span></span>

* <span data-ttu-id="3c5b0-121">Correção da consulta de pares chave-valor por rótulos separados por vírgula</span><span class="sxs-lookup"><span data-stu-id="3c5b0-121">Fix querying key-values by comma separated labels</span></span>

### <a name="app-service"></a><span data-ttu-id="3c5b0-122">Serviço de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-122">App Service</span></span>

* <span data-ttu-id="3c5b0-123">Correção de bug: falha no comando az webapp up quando o usuário não tem permissões de gravação no diretório pai do projeto</span><span class="sxs-lookup"><span data-stu-id="3c5b0-123">Bugfix: az webapp up fails when user doesn't have write permissions to project's parent directory</span></span>
* <span data-ttu-id="3c5b0-124">Correção nº 13777: Correção para remover caracteres de escape do XML</span><span class="sxs-lookup"><span data-stu-id="3c5b0-124">Fix #13777: Fix to remove escape chars from XML</span></span>
* <span data-ttu-id="3c5b0-125">Correção nº 15441: falha no comando az webapp create-remote-connection com AttributeError: o objeto 'Thread' não tem nenhum atributo 'isAlive'</span><span class="sxs-lookup"><span data-stu-id="3c5b0-125">Fix #15441: az webapp create-remote-connection fails with AttributeError: 'Thread' object has no attribute 'isAlive'</span></span>
* <span data-ttu-id="3c5b0-126">[ALTERAÇÃO DA FALHA] az webapp up: adição de parâmetros opcionais (sistema operacional e runtime) e atualização de runtimes</span><span class="sxs-lookup"><span data-stu-id="3c5b0-126">[BREAKING CHANGE] az webapp up: add optional params (os & runtime) and updated runtimes</span></span>

### <a name="arm"></a><span data-ttu-id="3c5b0-127">ARM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-127">ARM</span></span>

* <span data-ttu-id="3c5b0-128">Migração para GA de comandos What-If de implantação de modelo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-128">Make template deployment What-If commands GA</span></span>
* <span data-ttu-id="3c5b0-129">[ALTERAÇÃO DA FALHA] Adição da confirmação do usuário ao comando az ts create</span><span class="sxs-lookup"><span data-stu-id="3c5b0-129">[BREAKING CHANGE] Add user confirmation for az ts create</span></span>
* <span data-ttu-id="3c5b0-130">Correção dos dados retornados na marcação de vários recursos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-130">Fix the returned data when tagging multiple resources</span></span>

### <a name="backup"></a><span data-ttu-id="3c5b0-131">Backup</span><span class="sxs-lookup"><span data-stu-id="3c5b0-131">Backup</span></span>

* <span data-ttu-id="3c5b0-132">`az backup policy create`: adição de suporte para criação da política de backup de IaaSVM por meio da CLI</span><span class="sxs-lookup"><span data-stu-id="3c5b0-132">`az backup policy create`: Add support for IaaSVM backup policy creation from CLI</span></span>
* <span data-ttu-id="3c5b0-133">Aumento do limite de proteção da VM de 100 para 1.000</span><span class="sxs-lookup"><span data-stu-id="3c5b0-133">Increasing VM protection limit from 100 to 1000</span></span>

### <a name="compute"></a><span data-ttu-id="3c5b0-134">Computação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-134">Compute</span></span>

* <span data-ttu-id="3c5b0-135">sig image-definition create: add --features</span><span class="sxs-lookup"><span data-stu-id="3c5b0-135">sig image-definition create: add --features</span></span>
* <span data-ttu-id="3c5b0-136">Nova versão de API de gallery_images 2020-09-30</span><span class="sxs-lookup"><span data-stu-id="3c5b0-136">New API version of gallery_images 2020-09-30</span></span>
* <span data-ttu-id="3c5b0-137">`az vm update / az sig image-version update`: suporte à atualização da versão de VM/imagem mesmo quando ela usa uma imagem entre locatários</span><span class="sxs-lookup"><span data-stu-id="3c5b0-137">`az vm update / az sig image-version update`: Support update vm/image-version even it uses a cross tenant image</span></span>
* <span data-ttu-id="3c5b0-138">Remoção da validação de SKUs de host de VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-138">Remove validation of vm host SKUs</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="3c5b0-139">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="3c5b0-139">Cosmos DB</span></span>

* <span data-ttu-id="3c5b0-140">`az cosmosdb create/update`: aprimoramento da mensagem de erro da entrada incorreta de --locations</span><span class="sxs-lookup"><span data-stu-id="3c5b0-140">`az cosmosdb create/update`: Improve error message from incorrect --locations input</span></span>
* <span data-ttu-id="3c5b0-141">`az cosmosdb sql container create/update`: adição do parâmetro --analytical-storage-ttl</span><span class="sxs-lookup"><span data-stu-id="3c5b0-141">`az cosmosdb sql container create/update`: Add --analytical-storage-ttl parameter</span></span>

### <a name="hdinsight"></a><span data-ttu-id="3c5b0-142">HDInsight</span><span class="sxs-lookup"><span data-stu-id="3c5b0-142">HDInsight</span></span>

* <span data-ttu-id="3c5b0-143">[ALTERAÇÃO DA FALHA] az hdinsight create: remoção de dois parâmetros: --public-network-access-type e --outbound-public-network-access-type</span><span class="sxs-lookup"><span data-stu-id="3c5b0-143">[BREAKING CHANGE] az hdinsight create: remove two parameters: --public-network-access-type and  --outbound-public-network-access-type</span></span>

### <a name="iot-central"></a><span data-ttu-id="3c5b0-144">Central da IoT</span><span class="sxs-lookup"><span data-stu-id="3c5b0-144">IoT Central</span></span>

* <span data-ttu-id="3c5b0-145">Remoção do aviso de versão prévia, pois ela já está em GA</span><span class="sxs-lookup"><span data-stu-id="3c5b0-145">Remove preview warning since it is already GAed</span></span>

### <a name="key-vault"></a><span data-ttu-id="3c5b0-146">Key Vault</span><span class="sxs-lookup"><span data-stu-id="3c5b0-146">Key Vault</span></span>

* <span data-ttu-id="3c5b0-147">Invalidação de `--enable-soft-delete false` na criação ou na atualização de cofres</span><span class="sxs-lookup"><span data-stu-id="3c5b0-147">Invalidate `--enable-soft-delete false` while creating or updating vaults</span></span>
* <span data-ttu-id="3c5b0-148">Alteração para que `--bypass` e `--default-action` trabalhem em conjunto com parâmetros da ACL de rede na criação de cofres</span><span class="sxs-lookup"><span data-stu-id="3c5b0-148">Make `--bypass` and `--default-action` work together with network acl parameters while creating vaults</span></span>

### <a name="misc"></a><span data-ttu-id="3c5b0-149">Diversos.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-149">Misc.</span></span>

* <span data-ttu-id="3c5b0-150">Adição de bash-completion a Dockerfile</span><span class="sxs-lookup"><span data-stu-id="3c5b0-150">Add bash-completion to Dockerfile</span></span>

### <a name="rdbms"></a><span data-ttu-id="3c5b0-151">RDBMS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-151">RDBMS</span></span>

* <span data-ttu-id="3c5b0-152">Adição do comando list-SKUS, de transformadores de tabela e do contexto local para o Postgres, o MySQL e o MariaDB – Servidor Único</span><span class="sxs-lookup"><span data-stu-id="3c5b0-152">Add List-SKUS Command, Table Transformers, Local Context for Postgres, MySQL, Mariadb Single Server</span></span>
* <span data-ttu-id="3c5b0-153">[ALTERAÇÃO DA FALHA] Atualizações de nomes de parâmetros.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-153">[BREAKING CHANGE] Parameter name updates.</span></span> <span data-ttu-id="3c5b0-154">Aprimoramentos no plano de gerenciamento para o MySQL e o PostgreSQL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-154">Improvements to Management Plane for MySQL and PostgreSQL</span></span>
* <span data-ttu-id="3c5b0-155">`az postgres|mariadb|mysql server create`: atualização da experiência de criação para o Postgres, o MySQL e o MariaDB: novos campos na saída e introdução de novos valores para o parâmetro `--public` no comando create (tudo, <IP>, <IPRange>, 0.0.0.0)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-155">`az postgres|mariadb|mysql server create` : Update create experience for Postgres, MySQL and MariaDB - new fields in the output , Introduce new values for `--public` parameter in create command (all,<IP>,<IPRange>,0.0.0.0)</span></span>

### <a name="signalr"></a><span data-ttu-id="3c5b0-156">SignalR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-156">SignalR</span></span>

* <span data-ttu-id="3c5b0-157">`az signalr create`: adição da nova opção `--enable-messaging-logs` para controlar o serviço na geração de logs de mensagens ou não</span><span class="sxs-lookup"><span data-stu-id="3c5b0-157">`az signalr create`: Add new option `--enable-messaging-logs` for controling service generate messaging logs or not</span></span>
* <span data-ttu-id="3c5b0-158">`az signalr update`: adição da nova opção `--enable-messaging-logs` para controlar o serviço na geração de logs de mensagens ou não</span><span class="sxs-lookup"><span data-stu-id="3c5b0-158">`az signalr update`: Add new option `--enable-messaging-logs` for controling service generate messaging logs or not</span></span>

### <a name="sql"></a><span data-ttu-id="3c5b0-159">SQL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-159">SQL</span></span>

* <span data-ttu-id="3c5b0-160">[ALTERAÇÃO DA FALHA] Correção da resposta do nome de parâmetro de redundância do armazenamento de backup e do valor para a MI</span><span class="sxs-lookup"><span data-stu-id="3c5b0-160">[BREAKING CHANGE] Fix response for backup storage redundancy param name and value for MI</span></span>
* <span data-ttu-id="3c5b0-161">`az sql db audit-policy show`: extensão para mostrar a política de auditoria do banco de dados, incluindo os dados de LA e EH</span><span class="sxs-lookup"><span data-stu-id="3c5b0-161">`az sql db audit-policy show`: extend to show database's audit policy including LA and EH data</span></span>
* <span data-ttu-id="3c5b0-162">`az sql db audit-policy update`: extensão para permitir a atualização de LA e EH juntamente com a política de auditoria do banco de dados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-162">`az sql db audit-policy update`: extend to allow LA and EH update along with database's audit policy</span></span>
* <span data-ttu-id="3c5b0-163">`az sql db audit-policy wait`: colocação da CLI em um estado de espera até que uma condição da política de auditoria do banco de dados seja atendida.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-163">`az sql db audit-policy wait`: place the CLI in a waiting state until a condition of the database's audit policy is met.</span></span>
* <span data-ttu-id="3c5b0-164">`az sql server audit-policy show`: extensão para mostrar a política de auditoria do servidor, incluindo os dados de LA e EH</span><span class="sxs-lookup"><span data-stu-id="3c5b0-164">`az sql server audit-policy show`: extend to show servers's audit policy including LA and EH data</span></span>
* <span data-ttu-id="3c5b0-165">`az sql server audit-policy update`: extensão para permitir a atualização de LA e EH juntamente com a política de auditoria do servidor</span><span class="sxs-lookup"><span data-stu-id="3c5b0-165">`az sql server audit-policy update`: extend to allow LA and EH update along with server's audit policy</span></span>
* <span data-ttu-id="3c5b0-166">`az sql server audit-policy wait`: colocação da CLI em um estado de espera até que uma condição da política de auditoria do servidor seja atendida.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-166">`az sql server audit-policy wait`: place the CLI in a waiting state until a condition of the server's audit policy is met.</span></span>
* <span data-ttu-id="3c5b0-167">Adição de suporte somente ao AAD para Servidores e Instâncias Gerenciadas de SQL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-167">Add AAD-only Support for SQL Managed Instances and Servers</span></span>
* <span data-ttu-id="3c5b0-168">`az sql db replica create`: adição do argumento --partner-database</span><span class="sxs-lookup"><span data-stu-id="3c5b0-168">`az sql db replica create`: Add --partner-database argument</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-169">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-169">Storage</span></span>

* <span data-ttu-id="3c5b0-170">Correção nº 15111: falha no comando `az storage logging update` sem argumento opcional</span><span class="sxs-lookup"><span data-stu-id="3c5b0-170">Fix #15111: `az storage logging update` fails without optional argument</span></span>
* <span data-ttu-id="3c5b0-171">Correção de bug no uso do comando set-tier com o logon da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="3c5b0-171">Fix bug when using set-tier command with service principal login</span></span>
* <span data-ttu-id="3c5b0-172">Atualização da versão do data lake do arquivo para 2020-02-10</span><span class="sxs-lookup"><span data-stu-id="3c5b0-172">Upgrade version for file datalake to 2020-02-10</span></span>
* <span data-ttu-id="3c5b0-173">`az storage queue list`: suporte a Track2</span><span class="sxs-lookup"><span data-stu-id="3c5b0-173">`az storage queue list`: Track2 supported</span></span>
* <span data-ttu-id="3c5b0-174">`az storage fs access`: suporte ao gerenciamento de ACLs de maneira recursiva</span><span class="sxs-lookup"><span data-stu-id="3c5b0-174">`az storage fs access`: Support managing ACLs recursively</span></span>

### <a name="synapse"></a><span data-ttu-id="3c5b0-175">Synapse</span><span class="sxs-lookup"><span data-stu-id="3c5b0-175">Synapse</span></span>

* <span data-ttu-id="3c5b0-176">adição de cmdlets relacionados a pipeline, serviço vinculado, gatilho, notebook, fluxo de dados e conjunto de dados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-176">Add pipeline, linked service, trigger, notebook, data flow and dataset related cmdlets</span></span>

## <a name="october-13-2020"></a><span data-ttu-id="3c5b0-177">13 de outubro de 2020</span><span class="sxs-lookup"><span data-stu-id="3c5b0-177">October 13, 2020</span></span>

<span data-ttu-id="3c5b0-178">Versão 2.13.0</span><span class="sxs-lookup"><span data-stu-id="3c5b0-178">Version 2.13.0</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-179">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-179">ACR</span></span>

* <span data-ttu-id="3c5b0-180">`az acr helm`: atualizar a URL de substituição</span><span class="sxs-lookup"><span data-stu-id="3c5b0-180">`az acr helm`: Update deprecation url</span></span>
* <span data-ttu-id="3c5b0-181">Adicionar alterações de logtemplate e systemtask para Tarefas do ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-181">Add logtemplate and systemtask changes for ACR Tasks</span></span>

### <a name="aks"></a><span data-ttu-id="3c5b0-182">AKS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-182">AKS</span></span>

* <span data-ttu-id="3c5b0-183">Dar suporte ao nó virtual com o comando aks create: `az aks create --enable-addons virtual-node`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-183">Support virtual-node with aks create: `az aks create --enable-addons virtual-node`</span></span>
* <span data-ttu-id="3c5b0-184">Adicionar a única opção de imagem de nó para a CLI</span><span class="sxs-lookup"><span data-stu-id="3c5b0-184">Add node image only option for CLI</span></span>
* <span data-ttu-id="3c5b0-185">Esperar que o complemento kube-dashboard seja desabilitado por padrão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-185">Expect kube-dashboard addon be disabled by default</span></span>
* <span data-ttu-id="3c5b0-186">`az aks create/update`: adicionar suporte ao LicenseType para o Windows</span><span class="sxs-lookup"><span data-stu-id="3c5b0-186">`az aks create/update`: Add LicenseType support for Windows</span></span>
* <span data-ttu-id="3c5b0-187">Dar suporte para adicionar pools de nós spot</span><span class="sxs-lookup"><span data-stu-id="3c5b0-187">Support add Spot node pool</span></span>
* <span data-ttu-id="3c5b0-188">Respeitar os nomes de complementos definidos na CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="3c5b0-188">Honor addon names defined in Azure CLI</span></span>

### <a name="ams"></a><span data-ttu-id="3c5b0-189">AMS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-189">AMS</span></span>

* <span data-ttu-id="3c5b0-190">Correção nº 14687: o grupo de recursos e o nome da conta misturados no comando "az ams streaming-endpoint show"</span><span class="sxs-lookup"><span data-stu-id="3c5b0-190">Fix #14687: Mixed resource group and account name in command "az ams streaming-endpoint show"</span></span>

### <a name="app-config"></a><span data-ttu-id="3c5b0-191">Configuração do Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-191">App Config</span></span>

* <span data-ttu-id="3c5b0-192">Corrigir o bug de teste</span><span class="sxs-lookup"><span data-stu-id="3c5b0-192">Fix test bug</span></span>
* <span data-ttu-id="3c5b0-193">Dar suporte à autenticação do AAD para operações de dados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-193">Support AAD auth for data operations</span></span>

### <a name="app-service"></a><span data-ttu-id="3c5b0-194">Serviço de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-194">App Service</span></span>

* <span data-ttu-id="3c5b0-195">`az functionapp deployment source config-zip`: correção de um problema em que o config-zip poderia gerar uma exceção em caso de sucesso no consumo em Linux</span><span class="sxs-lookup"><span data-stu-id="3c5b0-195">`az functionapp deployment source config-zip`: Fixed an issue where config-zip could throw an exception on success on linux consumption</span></span>
* <span data-ttu-id="3c5b0-196">Bugfix: mensagens de erro aprimoradas para comandos webapp</span><span class="sxs-lookup"><span data-stu-id="3c5b0-196">Bugfix: Better error messages for webapp commands</span></span>
* <span data-ttu-id="3c5b0-197">`az appservice domain create, show-terms`: adicionar a capacidade de criar um domínio do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-197">`az appservice domain create, show-terms`: Add ability to create app service domain</span></span>
* <span data-ttu-id="3c5b0-198">`az functionapp create`: o sinalizador de visualização do Java 11 foi removido durante a criação de um aplicativo de funções</span><span class="sxs-lookup"><span data-stu-id="3c5b0-198">`az functionapp create`: Removed the preview flag from Java 11 when creating a new function app</span></span>
* <span data-ttu-id="3c5b0-199">[ALTERAÇÃO DA FALHA] az webapp create e az webapp up – Atualizar runtimes de webapp disponíveis</span><span class="sxs-lookup"><span data-stu-id="3c5b0-199">[BREAKING CHANGE] az webapp create, az webapp up - Update available webapp runtimes</span></span>

### <a name="arm"></a><span data-ttu-id="3c5b0-200">ARM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-200">ARM</span></span>

* <span data-ttu-id="3c5b0-201">`az ts`: adicionar novos comandos para especificações de modelo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-201">`az ts`: Add new commands for template specs</span></span>
* <span data-ttu-id="3c5b0-202">`az deployment`: adicionar suporte para --template-spec -s</span><span class="sxs-lookup"><span data-stu-id="3c5b0-202">`az deployment` : Add support for --template-spec -s</span></span>

### <a name="compute"></a><span data-ttu-id="3c5b0-203">Computação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-203">Compute</span></span>

* <span data-ttu-id="3c5b0-204">Corrigir a limitação de contagem FD de criação de grupos de hosts</span><span class="sxs-lookup"><span data-stu-id="3c5b0-204">Fix host group creation FD count limitation</span></span>
* <span data-ttu-id="3c5b0-205">Adicionar um novo comando para dar suporte à atualização de extensões para VMSS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-205">Add new command to support upgrading extensions for VMSS</span></span>
* <span data-ttu-id="3c5b0-206">Não há problemas na correção da referência da imagem</span><span class="sxs-lookup"><span data-stu-id="3c5b0-206">Fix the image reference is missing issue</span></span>

### <a name="hdinsight"></a><span data-ttu-id="3c5b0-207">HDInsight</span><span class="sxs-lookup"><span data-stu-id="3c5b0-207">HDInsight</span></span>

* <span data-ttu-id="3c5b0-208">`az hdinsight create`: adicionar informações preteridas para os argumentos --public-networrk-access-type e --outbound-public-network-access-type</span><span class="sxs-lookup"><span data-stu-id="3c5b0-208">`az hdinsight create`: add deprecate information for argument --public-networrk-access-type and --outbound-public-network-access-type</span></span>
* <span data-ttu-id="3c5b0-209">`az hdinsight create`: adicionar informações preteridas para os argumentos `--public-networrk-access-type` e `--outbound-public-network-access-type`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-209">`az hdinsight create`: add deprecate information for argument `--public-networrk-access-type` and `--outbound-public-network-access-type`</span></span>
* <span data-ttu-id="3c5b0-210">`az hdinsight create`: adicionar o parâmetro `--idbroker` para dar suporte ao cliente a fim de criar um cluster ESP com o Agente de IDs do HDInsight</span><span class="sxs-lookup"><span data-stu-id="3c5b0-210">`az hdinsight create`:  add parameter `--idbroker` to support customer to create ESP cluster with HDInsight Id Broker</span></span>

### <a name="iot-central"></a><span data-ttu-id="3c5b0-211">Central da IoT</span><span class="sxs-lookup"><span data-stu-id="3c5b0-211">IoT Central</span></span>

* <span data-ttu-id="3c5b0-212">Remover o módulo de comando 'az iotcentral' preterido</span><span class="sxs-lookup"><span data-stu-id="3c5b0-212">Remove deprecated 'az iotcentral' command module</span></span>

### <a name="key-vault"></a><span data-ttu-id="3c5b0-213">Key Vault</span><span class="sxs-lookup"><span data-stu-id="3c5b0-213">Key Vault</span></span>

* <span data-ttu-id="3c5b0-214">Dar suporte à `--hsm-name` para `az keyvault key encrypt/decrypt`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-214">Support `--hsm-name` for `az keyvault key encrypt/decrypt`</span></span>

### <a name="lab"></a><span data-ttu-id="3c5b0-215">Laboratório</span><span class="sxs-lookup"><span data-stu-id="3c5b0-215">Lab</span></span>

* <span data-ttu-id="3c5b0-216">Correção nº 14127: `__init__()` precisa de um argumento posicional, porém dois foram fornecidos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-216">Fix #14127: `__init__()` takes 1 positional argument but 2 were given</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-217">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-217">Network</span></span>

* <span data-ttu-id="3c5b0-218">`az network application-gateway ssl-cert show`: adicionar um exemplo para demonstrar o formato do certificado e buscar informações</span><span class="sxs-lookup"><span data-stu-id="3c5b0-218">`az network application-gateway ssl-cert show`: Add example to demonstrate certificate format and fetch information</span></span>
* <span data-ttu-id="3c5b0-219">`az network application-gateway rule`: dar suporte a --priority option</span><span class="sxs-lookup"><span data-stu-id="3c5b0-219">`az network application-gateway rule`: Support --priority option</span></span>
* <span data-ttu-id="3c5b0-220">`az network application-gateway create`: corrigir um bug que não pode ser criado sem um IP especificado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-220">`az network application-gateway create`: Fix bug that cannot create without public IP sepcified</span></span>
* <span data-ttu-id="3c5b0-221">`az network application-gateway waf-policy managed-rule rule-set add`: expor o erro do servidor ao usuário para fornecer uma mensagem de dica mais intuitiva.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-221">`az network application-gateway waf-policy managed-rule rule-set add`: Expose server error to user to give more intuitive hint message.</span></span>
* <span data-ttu-id="3c5b0-222">`az network application-gateway waf-policy managed-rule rule-set update`: dar suporte para alterar a versão do tipo de conjunto de regras.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-222">`az network application-gateway waf-policy managed-rule rule-set update`: Support to change rule set type version.</span></span>

### <a name="rdbms"></a><span data-ttu-id="3c5b0-223">RDBMS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-223">RDBMS</span></span>

* <span data-ttu-id="3c5b0-224">Bugfix: az postgres flexible-server create. Remover a versão de API codificada do cliente de rede.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-224">Bugfix: az postgres flexible-server create Remove hardcoded API version from network client.</span></span>

### <a name="role"></a><span data-ttu-id="3c5b0-225">Função</span><span class="sxs-lookup"><span data-stu-id="3c5b0-225">Role</span></span>

* <span data-ttu-id="3c5b0-226">Correção nº 15278: `az role assignment list/delete`: proibir argumentos de cadeias de caracteres vazias</span><span class="sxs-lookup"><span data-stu-id="3c5b0-226">Fix #15278: `az role assignment list/delete`: Forbid empty string arguments</span></span>

### <a name="sql"></a><span data-ttu-id="3c5b0-227">SQL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-227">SQL</span></span>

* <span data-ttu-id="3c5b0-228">`az sql midb log-replay`: dar suporte para serviços de reprodução de log em um banco de dados gerenciado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-228">`az sql midb log-replay`: Support for log replay service on managed database</span></span>
* <span data-ttu-id="3c5b0-229">Ignorar a formatação de maiúsculas/minúsculas dos caracteres para o valor de parâmetro de redundância de armazenamento de backup para uma instância gerenciada</span><span class="sxs-lookup"><span data-stu-id="3c5b0-229">Ignore character casing for backup storage redundancy param value for managed instance</span></span>
* <span data-ttu-id="3c5b0-230">[ALTERAÇÃO DA FALHA] az sql db create: adicionar o parâmetro --backup-storage-redundancy. Adicionar um aviso para o bsr/bsr == Geo não especificado.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-230">[BREAKING CHANGE] az sql db create: Add --backup-storage-redundancy parameter; add warning for unspecified bsr/bsr == Geo.</span></span>

### <a name="sql-vm"></a><span data-ttu-id="3c5b0-231">SQL VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-231">SQL VM</span></span>

* <span data-ttu-id="3c5b0-232">`az sql vm show`: adicionar opções de configuração ao sinalizador --expand</span><span class="sxs-lookup"><span data-stu-id="3c5b0-232">`az sql vm show`: Add configuration options to --expand flag</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-233">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-233">Storage</span></span>

* <span data-ttu-id="3c5b0-234">[ALTERAÇÃO DA FALHA] `az storage blob copy start`: corrigir o problema de formato para `--destination-if-modified-since` e `--destination-if-unmodified-since`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-234">[BREAKING CHANGE] `az storage blob copy start`: Fix format issue for `--destination-if-modified-since` and `--destination-if-unmodified-since`</span></span>
* <span data-ttu-id="3c5b0-235">[ALTERAÇÃO DA FALHA] `az storage blob incremental-copy start`: corrigir o problema de formato para `--destination-if-modified-since` e `--destination-if-unmodified-since`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-235">[BREAKING CHANGE] `az storage blob incremental-copy start`: Fix format issue for `--destination-if-modified-since` and `--destination-if-unmodified-since`</span></span>
* <span data-ttu-id="3c5b0-236">`az storage fs`: corrigir um problema de cadeia de conexão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-236">`az storage fs`: Fix connection string issue</span></span>
* <span data-ttu-id="3c5b0-237">`az storage share-rm`: camada de acesso da versão de GA</span><span class="sxs-lookup"><span data-stu-id="3c5b0-237">`az storage share-rm`: GA release access tier</span></span>
* <span data-ttu-id="3c5b0-238">`az storage container-rm`: adicionar um novo grupo de comandos com o objetivo de usar o provedor de recursos Microsoft.Storage para operações de gerenciamento de contêineres.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-238">`az storage container-rm`: Add a new command group to use the Microsoft.Storage resource provider for container management operations.</span></span>

## <a name="september-29-2020"></a><span data-ttu-id="3c5b0-239">29 de setembro de 2020</span><span class="sxs-lookup"><span data-stu-id="3c5b0-239">September 29, 2020</span></span>

<span data-ttu-id="3c5b0-240">Versão 2.12.1</span><span class="sxs-lookup"><span data-stu-id="3c5b0-240">Version 2.12.1</span></span>

### <a name="rdbms"></a><span data-ttu-id="3c5b0-241">RDBMS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-241">RDBMS</span></span>

* <span data-ttu-id="3c5b0-242">Hotfix: `az postgres flexible-server create`: Atualizar o VnetName para excluir o nome do servidor e atualizar a região padrão para MySQL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-242">Hotfix: `az postgres flexible-server create` : Update VnetName to exclude servername and update default region for MySQL</span></span>

## <a name="september-22-2020"></a><span data-ttu-id="3c5b0-243">22 de setembro de 2020</span><span class="sxs-lookup"><span data-stu-id="3c5b0-243">September 22, 2020</span></span>

<span data-ttu-id="3c5b0-244">Versão 2.12.0</span><span class="sxs-lookup"><span data-stu-id="3c5b0-244">Version 2.12.0</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-245">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-245">ACR</span></span>

* <span data-ttu-id="3c5b0-246">Correção nº 14811: adicionar suporte para substituição dockerignore</span><span class="sxs-lookup"><span data-stu-id="3c5b0-246">Fix #14811 Add support for dockerignore override</span></span>

### <a name="aks"></a><span data-ttu-id="3c5b0-247">AKS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-247">AKS</span></span>

* <span data-ttu-id="3c5b0-248">A CLI deve tolerar kubeconfig vazio</span><span class="sxs-lookup"><span data-stu-id="3c5b0-248">CLI should tolerate empty kubeconfig</span></span>
* <span data-ttu-id="3c5b0-249">CORREÇÃO nº 12871: az aks enable-addons: o exemplo de ajuda gerada automaticamente está errado para a opção virtual-node</span><span class="sxs-lookup"><span data-stu-id="3c5b0-249">FIX #12871: az aks enable-addons: Autogenerated help example is wrong for vitual-node option</span></span>
* <span data-ttu-id="3c5b0-250">Remover ações do conector do aci herdado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-250">Remove legacy aci connector actions</span></span>
* <span data-ttu-id="3c5b0-251">Dar suporte ao complemento do Azure Policy em azure-cli</span><span class="sxs-lookup"><span data-stu-id="3c5b0-251">Support azure policy addon in azure-cli</span></span>
* <span data-ttu-id="3c5b0-252">Corrigir o problema de diferenciação de maiúsculas e minúsculas do complemento do painel do AKS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-252">Fix case sensitive issue for AKS dashboard addon</span></span>
* <span data-ttu-id="3c5b0-253">Atualizar mgmt-containerservice para a versão 9.4.0 e habilitar a API 09-01</span><span class="sxs-lookup"><span data-stu-id="3c5b0-253">Update mgmt-containerservice to 9.4.0 and enable 09-01 API</span></span>

### <a name="apim"></a><span data-ttu-id="3c5b0-254">APIM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-254">APIM</span></span>

* <span data-ttu-id="3c5b0-255">Dar suporte aos comandos de entidade product/productapi/namedValue e a versão do SDK bump &&</span><span class="sxs-lookup"><span data-stu-id="3c5b0-255">Support product / productapi / namedValue entity commands && bump sdk version</span></span>

### <a name="app-config"></a><span data-ttu-id="3c5b0-256">Configuração do Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-256">App Config</span></span>

* <span data-ttu-id="3c5b0-257">Dar suporte para habilitar/desabilitar PublicNetworkAccess para armazenamentos existentes</span><span class="sxs-lookup"><span data-stu-id="3c5b0-257">Support enabling/disabling PublicNetworkAccess for existing stores</span></span>

### <a name="app-service"></a><span data-ttu-id="3c5b0-258">Serviço de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-258">App Service</span></span>

* <span data-ttu-id="3c5b0-259">Adicionar suporte para o tipo de preço Premium V3</span><span class="sxs-lookup"><span data-stu-id="3c5b0-259">Add support for Premium V3 pricing tier</span></span>
* <span data-ttu-id="3c5b0-260">Correção nº12653: az webapp log config --application-logging false não o desativa</span><span class="sxs-lookup"><span data-stu-id="3c5b0-260">Fix #12653: az webapp log config --application-logging false doesn't turn it off</span></span>
* <span data-ttu-id="3c5b0-261">Correção nº 14684: a remoção de access-restriction por endereço IP não funcionava; nº 13837-az webapp create – Exemplo para diferentes RSgroups para Plan e WebApp</span><span class="sxs-lookup"><span data-stu-id="3c5b0-261">Fix #14684: access-restriction remove by ip address does not work; #13837-az webapp create - Example for different RSgroups for Plan and WebApp</span></span>
* <span data-ttu-id="3c5b0-262">functionapp: Adicionar suporte para manipuladores personalizados.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-262">functionapp: Add support for custom handlers.</span></span> <span data-ttu-id="3c5b0-263">PowerShell 6.2 preterido.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-263">Deprecated Powershell 6.2.</span></span>
* <span data-ttu-id="3c5b0-264">functionapp: Correção do problema em que a configuração do aplicativo estava sendo definida incorretamente para imagens personalizadas do Linux</span><span class="sxs-lookup"><span data-stu-id="3c5b0-264">functionapp: Fix issue where app setting was being incorrectly set for linux custom images</span></span>

### <a name="arm"></a><span data-ttu-id="3c5b0-265">ARM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-265">ARM</span></span>

* <span data-ttu-id="3c5b0-266">`az deployment group/sub/mg/tenant what-if`: Mostrar alterações de recurso "Ignorar" por último</span><span class="sxs-lookup"><span data-stu-id="3c5b0-266">`az deployment group/sub/mg/tenant what-if`: Show "Ignore" resource changes last</span></span>

### <a name="compute"></a><span data-ttu-id="3c5b0-267">Computação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-267">Compute</span></span>

* <span data-ttu-id="3c5b0-268">Adicionar novo license_type na criação/atualização de VM: RHEL_BYOS, SLES_BYOS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-268">Add new license_type in vm create/update: RHEL_BYOS, SLES_BYOS</span></span>
* <span data-ttu-id="3c5b0-269">Atualizar a API do disco para a versão 2020-06-30</span><span class="sxs-lookup"><span data-stu-id="3c5b0-269">Upgrade disk API version to 2020-06-30</span></span>
* <span data-ttu-id="3c5b0-270">criação do disco: add --logical-sector-size, --tier</span><span class="sxs-lookup"><span data-stu-id="3c5b0-270">disk create: add --logical-sector-size, --tier</span></span>
* <span data-ttu-id="3c5b0-271">atualização do disco: Suporte a --disk-iops-read-only, --disk-mbps-read-only, --max-shares</span><span class="sxs-lookup"><span data-stu-id="3c5b0-271">disk update: Support --disk-iops-read-only, --disk-mbps-read-only, --max-shares</span></span>
* <span data-ttu-id="3c5b0-272">Novo comando disk-encryption-set list-associated-resources</span><span class="sxs-lookup"><span data-stu-id="3c5b0-272">New command disk-encryption-set list-associated-resources</span></span>
* <span data-ttu-id="3c5b0-273">Habilitação de vm boot-diagnostics: --storage se torna opcional</span><span class="sxs-lookup"><span data-stu-id="3c5b0-273">vm boot-diagnostics enable: --storage becomes optional</span></span>
* <span data-ttu-id="3c5b0-274">Novo comando: vm boot-diagnostics get-boot-log-uris</span><span class="sxs-lookup"><span data-stu-id="3c5b0-274">New command: vm boot-diagnostics get-boot-log-uris</span></span>
* <span data-ttu-id="3c5b0-275">vm boot-diagnostics get-boot-log: suporte ao armazenamento gerenciado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-275">vm boot-diagnostics get-boot-log: support managed storage</span></span>

### <a name="config"></a><span data-ttu-id="3c5b0-276">Config</span><span class="sxs-lookup"><span data-stu-id="3c5b0-276">Config</span></span>

* <span data-ttu-id="3c5b0-277">Renomear local-context para configurar param-persist</span><span class="sxs-lookup"><span data-stu-id="3c5b0-277">Rename local-context to config param-persist</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="3c5b0-278">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="3c5b0-278">Cosmos DB</span></span>

* <span data-ttu-id="3c5b0-279">Dar suporte a APIs de Migração para o recurso de taxa de transferência para o recurso de dimensionamento automático no CosmosDB</span><span class="sxs-lookup"><span data-stu-id="3c5b0-279">Support for Migration APIs for Throughput resource for Autoscale feature in CosmosDB</span></span>

### <a name="eventhub"></a><span data-ttu-id="3c5b0-280">Eventhub</span><span class="sxs-lookup"><span data-stu-id="3c5b0-280">Eventhub</span></span>

<span data-ttu-id="3c5b0-281">Adição de comandos de cluster e do parâmetro trusted_service_access_enabled para Networkruleset</span><span class="sxs-lookup"><span data-stu-id="3c5b0-281">Added Cluster commands and trusted_service_access_enabled parameter for Networkruleset</span></span>

### <a name="extension"></a><span data-ttu-id="3c5b0-282">Extensão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-282">Extension</span></span>

* <span data-ttu-id="3c5b0-283">`az extension add`: adicionar a opção `--upgrade` para atualizar a extensão, se ela já estiver instalada</span><span class="sxs-lookup"><span data-stu-id="3c5b0-283">`az extension add`: Add `--upgrade` option to update the extension if already installed</span></span>
* <span data-ttu-id="3c5b0-284">Ativar a instalação dinâmica por padrão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-284">Turn on dynamic install by default</span></span>

### <a name="iot"></a><span data-ttu-id="3c5b0-285">IoT</span><span class="sxs-lookup"><span data-stu-id="3c5b0-285">IoT</span></span>

* <span data-ttu-id="3c5b0-286">Versão mínima do TLS habilitada na criação do Hub IoT</span><span class="sxs-lookup"><span data-stu-id="3c5b0-286">Enabled minimum TLS version on IoT Hub Create</span></span>

### <a name="iot-central"></a><span data-ttu-id="3c5b0-287">IoT Central</span><span class="sxs-lookup"><span data-stu-id="3c5b0-287">IoT Central</span></span>

* <span data-ttu-id="3c5b0-288">A operação de exclusão de aplicativo agora é uma operação de execução prolongada</span><span class="sxs-lookup"><span data-stu-id="3c5b0-288">App delete operation is now long running operation</span></span>

### <a name="iot-hub"></a><span data-ttu-id="3c5b0-289">Hub IoT</span><span class="sxs-lookup"><span data-stu-id="3c5b0-289">Iot Hub</span></span>

* <span data-ttu-id="3c5b0-290">Comando 'show-connection-string' preterido</span><span class="sxs-lookup"><span data-stu-id="3c5b0-290">Deprecated 'show-connection-string' command</span></span>

### <a name="key-vault"></a><span data-ttu-id="3c5b0-291">Key Vault</span><span class="sxs-lookup"><span data-stu-id="3c5b0-291">Key Vault</span></span>

* <span data-ttu-id="3c5b0-292">Versão prévia pública do HSM gerenciado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-292">Managed HSM public preview</span></span>
* <span data-ttu-id="3c5b0-293">Corrigir o problema em que `--maxresults` não entrou em vigor durante a listagem de recursos ou versões de recursos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-293">Fix the issue that `--maxresults` does not take effect while listing resources or resource versions</span></span>

### <a name="kusto"></a><span data-ttu-id="3c5b0-294">Kusto</span><span class="sxs-lookup"><span data-stu-id="3c5b0-294">Kusto</span></span>

* <span data-ttu-id="3c5b0-295">Adicionar mensagem de substituição</span><span class="sxs-lookup"><span data-stu-id="3c5b0-295">Add deprecating message</span></span>

### <a name="monitor"></a><span data-ttu-id="3c5b0-296">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-296">Monitor</span></span>

* <span data-ttu-id="3c5b0-297">`az monitor log-analytics workspace linked-storage`: expor a mensagem de erro detalhada aos clientes</span><span class="sxs-lookup"><span data-stu-id="3c5b0-297">`az monitor log-analytics workspace linked-storage`: expose detailed error message to customers</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-298">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-298">Network</span></span>

* <span data-ttu-id="3c5b0-299">`az network vnet subnet`: dar suporte a --disable-private-endpoint-network-policies e --disable-private-link-service-network-policies</span><span class="sxs-lookup"><span data-stu-id="3c5b0-299">`az network vnet subnet`: Support --disable-private-endpoint-network-policies and --disable-private-link-service-network-policies</span></span>
* <span data-ttu-id="3c5b0-300">Corrigir o bug durante a atualização do log de fluxos quando a subpropriedade network_watcher_flow_analytics_configuration for None</span><span class="sxs-lookup"><span data-stu-id="3c5b0-300">Fix bug while updateing flow-log when its subproperty network_watcher_flow_analytics_configuration is None</span></span>
* <span data-ttu-id="3c5b0-301">Elevação da API para a versão 2020-06-01</span><span class="sxs-lookup"><span data-stu-id="3c5b0-301">API version bump to 2020-06-01</span></span>
* <span data-ttu-id="3c5b0-302">Dar suporte --tcp-port-behavior durante a definição da configuração do TCP de um Monitor da Conexão V2</span><span class="sxs-lookup"><span data-stu-id="3c5b0-302">Support --tcp-port-behavior while configuring a TCP configuration of a Connection Monitor V2</span></span>
* <span data-ttu-id="3c5b0-303">Dar suporte a mais tipos e ao nível de cobertura durante a criação do ponto de extremidade do Monitor da Conexão v2</span><span class="sxs-lookup"><span data-stu-id="3c5b0-303">Support more types and coverage level while creating Endpoint of Connection Monitor V2</span></span>
* <span data-ttu-id="3c5b0-304">Dar suporte a --host-subnet para criar o VirtualHub abaixo como VirtualRouter</span><span class="sxs-lookup"><span data-stu-id="3c5b0-304">Support --host-subnet to create VirtualHub underneath as VirtualRouter</span></span>

### <a name="rdbms"></a><span data-ttu-id="3c5b0-305">RDBMS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-305">RDBMS</span></span>

* <span data-ttu-id="3c5b0-306">Atualizações do Plano de Gerenciamento para PostgreSQL e MySQL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-306">Management Plane updates for PostgreSQL and MySQL</span></span>

### <a name="role"></a><span data-ttu-id="3c5b0-307">Função</span><span class="sxs-lookup"><span data-stu-id="3c5b0-307">Role</span></span>

* <span data-ttu-id="3c5b0-308">`az role assignment create/update`: dar suporte a `--description`, `--condition` e `--condition-version`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-308">`az role assignment create/update`: Support `--description`, `--condition` and `--condition-version`</span></span>
* <span data-ttu-id="3c5b0-309">`az ad app permission delete`: dar suporte a `--api-permissions` para excluir o `ResourceAccess` específico</span><span class="sxs-lookup"><span data-stu-id="3c5b0-309">`az ad app permission delete`: Support `--api-permissions` to delete specific `ResourceAccess`</span></span>

### <a name="service-fabric"></a><span data-ttu-id="3c5b0-310">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="3c5b0-310">Service Fabric</span></span>

* <span data-ttu-id="3c5b0-311">Adicionar comandos de tipo de nó e cluster gerenciado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-311">Add managed cluster and node type commands</span></span>

### <a name="sql"></a><span data-ttu-id="3c5b0-312">SQL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-312">SQL</span></span>

* <span data-ttu-id="3c5b0-313">Atualizar azure-mgmt-sql para 0.20.0</span><span class="sxs-lookup"><span data-stu-id="3c5b0-313">Upgrade azure-mgmt-sql to 0.20.0</span></span>
* <span data-ttu-id="3c5b0-314">Adicionar parâmetro opcional de redundância de armazenamento de backup ao cmdlet MI create</span><span class="sxs-lookup"><span data-stu-id="3c5b0-314">Add backup storage redundancy optional parameter to MI create cmdlet</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-315">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-315">Storage</span></span>

* <span data-ttu-id="3c5b0-316">`az storage share-rm stats`: obter os bytes de uso dos dados armazenados no compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-316">`az storage share-rm stats`: Get the usage bytes of the data stored on the share.</span></span>
* <span data-ttu-id="3c5b0-317">PITR de blob de armazenamento de versão GA</span><span class="sxs-lookup"><span data-stu-id="3c5b0-317">GA release storage blob PITR</span></span>
* <span data-ttu-id="3c5b0-318">`az storage blob query`: dar suporte à Aceleração de Consulta do Armazenamento do Azure</span><span class="sxs-lookup"><span data-stu-id="3c5b0-318">`az storage blob query`: Support Azure Storage Query Acceleration</span></span>
* <span data-ttu-id="3c5b0-319">Dar suporte à exclusão reversível para o compartilhamento de arquivo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-319">Support Soft Delete for file share</span></span>
* <span data-ttu-id="3c5b0-320">`az storage copy`: adicionar suporte a credenciais de conta e substituir `--source-local-path`, `--destination-local-path`, `--destination-account-name`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-320">`az storage copy`: Add account credentials support and deprecate `--source-local-path`, `--destination-local-path`, `--destination-account-name`</span></span>
* <span data-ttu-id="3c5b0-321">`az storage account blob-service-properties update`: adicionar suporte à política de retenção de exclusão de contêiner</span><span class="sxs-lookup"><span data-stu-id="3c5b0-321">`az storage account blob-service-properties update`: Add container delete retention policy support</span></span>

### <a name="synapse"></a><span data-ttu-id="3c5b0-322">Synapse</span><span class="sxs-lookup"><span data-stu-id="3c5b0-322">Synapse</span></span>

* <span data-ttu-id="3c5b0-323">Correção de erro de digitação no exemplo de criação e exclusão de atribuição de função do az synapse</span><span class="sxs-lookup"><span data-stu-id="3c5b0-323">Fixed typo in example of az synapse role assignment create and delete</span></span>

## <a name="august-28-2020"></a><span data-ttu-id="3c5b0-324">28 de agosto de 2020</span><span class="sxs-lookup"><span data-stu-id="3c5b0-324">August 28, 2020</span></span>

<span data-ttu-id="3c5b0-325">Versão 2.11.1</span><span class="sxs-lookup"><span data-stu-id="3c5b0-325">Version 2.11.1</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-326">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-326">ACR</span></span>

* <span data-ttu-id="3c5b0-327">Adição de camada isolada ao pool de agentes</span><span class="sxs-lookup"><span data-stu-id="3c5b0-327">Add Isolated Tier to Agent Pool</span></span>
* <span data-ttu-id="3c5b0-328">Adição de contexto de origem do artefato de OCI</span><span class="sxs-lookup"><span data-stu-id="3c5b0-328">Add OCI Artifact Source Context</span></span>

### <a name="aks"></a><span data-ttu-id="3c5b0-329">AKS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-329">AKS</span></span>

* <span data-ttu-id="3c5b0-330">Correção de um problema de criação do cluster do AKS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-330">Fix aks cluster create issue</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="3c5b0-331">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-331">Cognitive Services</span></span>

* <span data-ttu-id="3c5b0-332">[ALTERAÇÃO DA FALHA] Mostrar um termo legal adicional para determinadas APIs</span><span class="sxs-lookup"><span data-stu-id="3c5b0-332">[BREAKING CHANGE] Show additional legal term for certain APIs</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-333">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-333">Network</span></span>

* <span data-ttu-id="3c5b0-334">[ALTERAÇÃO DA FALHA] Permitir a criação de IP público e IP privado ao criar um Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-334">[BREAKING CHANGE] Allow to create both public and private IP while creating an Application Gateway</span></span>
* <span data-ttu-id="3c5b0-335">`az network list-service-tags`: adição de detalhes sobre o uso de parâmetro de localização para a mensagem de ajuda</span><span class="sxs-lookup"><span data-stu-id="3c5b0-335">`az network list-service-tags`: add details on location parameter use to the help message</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-336">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-336">Storage</span></span>

* <span data-ttu-id="3c5b0-337">`az storage blob list`: suporte OU propriedades com a nova versão de API</span><span class="sxs-lookup"><span data-stu-id="3c5b0-337">`az storage blob list`: Support OR properties with new api version</span></span>

## <a name="august-25-2020"></a><span data-ttu-id="3c5b0-338">25 de agosto de 2020</span><span class="sxs-lookup"><span data-stu-id="3c5b0-338">August 25, 2020</span></span>

<span data-ttu-id="3c5b0-339">Versão 2.11.0</span><span class="sxs-lookup"><span data-stu-id="3c5b0-339">Version 2.11.0</span></span>

### <a name="aks"></a><span data-ttu-id="3c5b0-340">AKS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-340">AKS</span></span>

* <span data-ttu-id="3c5b0-341">Remoção da marca de visualização do complemento de Nó Virtual</span><span class="sxs-lookup"><span data-stu-id="3c5b0-341">Remove preview tag from Virtual Node add-on</span></span>
* <span data-ttu-id="3c5b0-342">Adição do argumento CMK do AKS na criação do cluster</span><span class="sxs-lookup"><span data-stu-id="3c5b0-342">Add AKS CMK argument in cluster creation</span></span>
* <span data-ttu-id="3c5b0-343">Definição do perfil de rede durante o uso do balanceador de carga básico.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-343">Set network profile when using basic load balancer.</span></span>
* <span data-ttu-id="3c5b0-344">Remoção da validação máxima de pods da CLI e permissão para que a simulação lide com ela</span><span class="sxs-lookup"><span data-stu-id="3c5b0-344">Remove max pods validation from CLI and let preflight handle it</span></span>
* <span data-ttu-id="3c5b0-345">Correção de complementos disponíveis na mensagem de ajuda em `az aks create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-345">Fixing add-ons available in the help message in `az aks create`</span></span>
* <span data-ttu-id="3c5b0-346">Introdução de suporte para o perfil de dimensionamento automático do cluster na CLI principal</span><span class="sxs-lookup"><span data-stu-id="3c5b0-346">Bring in support for cluster autoscaler profile in core CLI</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-347">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-347">AppService</span></span>

* <span data-ttu-id="3c5b0-348">`az webapp`: adição do comando list-instances</span><span class="sxs-lookup"><span data-stu-id="3c5b0-348">`az webapp`: Add list-instances command</span></span>
* <span data-ttu-id="3c5b0-349">`az webapp ssh`: adição do parâmetro --instance para se conectar a uma instância específica</span><span class="sxs-lookup"><span data-stu-id="3c5b0-349">`az webapp ssh`: Add --instance parameter to connect to a specific instance</span></span>
* <span data-ttu-id="3c5b0-350">`az webapp create-remote-connection`: adição do parâmetro --instance para se conectar a uma instância específica</span><span class="sxs-lookup"><span data-stu-id="3c5b0-350">`az webapp create-remote-connection`: Add --instance parameter to connect to a specific instance</span></span>
* <span data-ttu-id="3c5b0-351">Correção nº 14758: erros de az webapp create durante a criação de um aplicativo do Windows com --runtime dotnetcore</span><span class="sxs-lookup"><span data-stu-id="3c5b0-351">Fix #14758: az webapp create errors when creating windows app with --runtime dotnetcore</span></span>
* <span data-ttu-id="3c5b0-352">Correção nº 14701: implementação de functionapp create --assign-identity</span><span class="sxs-lookup"><span data-stu-id="3c5b0-352">Fix #14701: Implement functionapp create --assign-identity</span></span>
* <span data-ttu-id="3c5b0-353">Correção nº 11244: `az webapp auth update`: adição do parâmetro opcional para atualizar client-secret-certificate-thumbprint</span><span class="sxs-lookup"><span data-stu-id="3c5b0-353">Fix #11244: `az webapp auth update`: Add optional parameter to update client-secret-certificate-thumbprint</span></span>
* <span data-ttu-id="3c5b0-354">`az functionapp keys`: comandos adicionados que permitem aos usuários gerenciar as chaves do aplicativo de funções</span><span class="sxs-lookup"><span data-stu-id="3c5b0-354">`az functionapp keys`: Added commands that allow users to manage their function app keys</span></span>
* <span data-ttu-id="3c5b0-355">`az functionapp function`: comandos adicionados que permitem aos usuários gerenciar as funções individuais</span><span class="sxs-lookup"><span data-stu-id="3c5b0-355">`az functionapp function`: Added commands that allow users to manage their individual functions</span></span>
* <span data-ttu-id="3c5b0-356">`az functionapp function keys`: comandos adicionados que permitem aos usuários gerenciar as chaves de função</span><span class="sxs-lookup"><span data-stu-id="3c5b0-356">`az functionapp function keys`: Added commands that allow users to manage their function keys</span></span>
* <span data-ttu-id="3c5b0-357">Correção nº14788: az webapp create não obtém o webapp correto quando os nomes são substrings</span><span class="sxs-lookup"><span data-stu-id="3c5b0-357">Fix #14788: az webapp create not getting correct webapp when names are substrings</span></span>
* <span data-ttu-id="3c5b0-358">`az functionapp create`: capacidade removida para criar funções 2.x em regiões que não têm compatibilidade</span><span class="sxs-lookup"><span data-stu-id="3c5b0-358">`az functionapp create`: Removed ability to create 2.x Functions in regions that don't support it</span></span>

### <a name="arm"></a><span data-ttu-id="3c5b0-359">ARM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-359">ARM</span></span>

* <span data-ttu-id="3c5b0-360">`az resource list`: extensão dos dados retornados de `createdTime`, `changedTime` e `provisioningState`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-360">`az resource list`: Extend the return data of `createdTime`, `changedTime` and `provisioningState`</span></span>
* <span data-ttu-id="3c5b0-361">`az resource`: adição do parâmetro `--latest-include-preview` para dar suporte ao uso da api-version mais recente se ela for versão prévia</span><span class="sxs-lookup"><span data-stu-id="3c5b0-361">`az resource`: Add parameter `--latest-include-preview` to support using the latest api-version whether this version is preview</span></span>

### <a name="aro"></a><span data-ttu-id="3c5b0-362">ARO</span><span class="sxs-lookup"><span data-stu-id="3c5b0-362">ARO</span></span>

* <span data-ttu-id="3c5b0-363">Aprimoramentos da CLI, incluindo permissões de verificação da tabela de rotas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-363">CLI enhancements, including route table checking permissions</span></span>

### <a name="cloud"></a><span data-ttu-id="3c5b0-364">Nuvem</span><span class="sxs-lookup"><span data-stu-id="3c5b0-364">Cloud</span></span>

* <span data-ttu-id="3c5b0-365">`az cloud register`: correção do registro de nuvens com um arquivo de configuração</span><span class="sxs-lookup"><span data-stu-id="3c5b0-365">`az cloud register`: Fix registering clouds with a config file</span></span>

### <a name="compute"></a><span data-ttu-id="3c5b0-366">Computação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-366">Compute</span></span>

* <span data-ttu-id="3c5b0-367">Atualização de SKUs de VM compatíveis com rede acelerada</span><span class="sxs-lookup"><span data-stu-id="3c5b0-367">Update VM SKUs that support accelerated networking</span></span>
* <span data-ttu-id="3c5b0-368">`az vm create`: aplicação automática de patches no convidado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-368">`az vm create`: Automatic in-guest patching</span></span>
* <span data-ttu-id="3c5b0-369">`az image builder create`: adição de --vm-size, --os-disk-size, --vnet, --subnet</span><span class="sxs-lookup"><span data-stu-id="3c5b0-369">`az image builder create`: Add --vm-size, --os-disk-size, --vnet, --subnet</span></span>
* <span data-ttu-id="3c5b0-370">Novo comando az vm assess-patches</span><span class="sxs-lookup"><span data-stu-id="3c5b0-370">New command az vm assess-patches</span></span>

### <a name="container"></a><span data-ttu-id="3c5b0-371">Contêiner</span><span class="sxs-lookup"><span data-stu-id="3c5b0-371">Container</span></span>

* <span data-ttu-id="3c5b0-372">Correção nº 6235: atualização do texto de ajuda para o parâmetro de portas na criação do contêiner</span><span class="sxs-lookup"><span data-stu-id="3c5b0-372">Fix #6235: Update help text for ports parameter in container create</span></span>

### <a name="datalake-store"></a><span data-ttu-id="3c5b0-373">Datalake Store</span><span class="sxs-lookup"><span data-stu-id="3c5b0-373">Datalake Store</span></span>

* <span data-ttu-id="3c5b0-374">Correção do problema nº 14545 para a operação de ingresso no data lake</span><span class="sxs-lookup"><span data-stu-id="3c5b0-374">Fix issue #14545 for data lake join operation</span></span>

### <a name="eventhub"></a><span data-ttu-id="3c5b0-375">EventHub</span><span class="sxs-lookup"><span data-stu-id="3c5b0-375">EventHub</span></span>

* <span data-ttu-id="3c5b0-376">`az eventhubs eventhub create/update`: alterar a documentação de destination_name</span><span class="sxs-lookup"><span data-stu-id="3c5b0-376">`az eventhubs eventhub create/update`: Change documentation of destination_name</span></span>

### <a name="extension"></a><span data-ttu-id="3c5b0-377">Extensão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-377">Extension</span></span>

* <span data-ttu-id="3c5b0-378">Adição do comando `az extension list-versions` para listar todas as versões disponíveis de uma extensão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-378">Add `az extension list-versions` command to list all available versions of an extension</span></span>

### <a name="hdinsight"></a><span data-ttu-id="3c5b0-379">HDInsight</span><span class="sxs-lookup"><span data-stu-id="3c5b0-379">HDInsight</span></span>

* <span data-ttu-id="3c5b0-380">Suporte à criação de cluster com configuração de dimensionamento automático e suporte ao gerenciamento de configuração de dimensionamento automático</span><span class="sxs-lookup"><span data-stu-id="3c5b0-380">Support creating cluster with autoscale configuration and Support managing autoscale configuration</span></span>
* <span data-ttu-id="3c5b0-381">Suporte à criação de cluster com criptografia no host</span><span class="sxs-lookup"><span data-stu-id="3c5b0-381">Support creating cluster with encryption at host</span></span>

### <a name="iotcentral"></a><span data-ttu-id="3c5b0-382">IoT Central</span><span class="sxs-lookup"><span data-stu-id="3c5b0-382">IoTCentral</span></span>

* <span data-ttu-id="3c5b0-383">Aprimoramentos na documentação da CLI</span><span class="sxs-lookup"><span data-stu-id="3c5b0-383">CLI documentation improvements</span></span>

### <a name="monitor"></a><span data-ttu-id="3c5b0-384">Monitor</span><span class="sxs-lookup"><span data-stu-id="3c5b0-384">Monitor</span></span>

* <span data-ttu-id="3c5b0-385">`az monitor metrics alert create`: suporte a RG e Sub como os valores de escopo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-385">`az monitor metrics alert create`: support RG and Sub as the scope values</span></span>

### <a name="netappfiles"></a><span data-ttu-id="3c5b0-386">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="3c5b0-386">NetAppFiles</span></span>

* <span data-ttu-id="3c5b0-387">[ALTERAÇÃO DA FALHA] az netappfiles snapshot create: file-system-id removido dos parâmetros</span><span class="sxs-lookup"><span data-stu-id="3c5b0-387">[BREAKING CHANGE] az netappfiles snapshot create: Removed file-system-id from parameters</span></span>
* <span data-ttu-id="3c5b0-388">[ALTERAÇÃO DA FALHA] az netappfiles snapshot show: o instantâneo não tem mais o parâmetro file-system-id</span><span class="sxs-lookup"><span data-stu-id="3c5b0-388">[BREAKING CHANGE] az netappfiles snapshot show: Snapshot no longer has parameter file-system-id</span></span>
* <span data-ttu-id="3c5b0-389">`az netappfiles account`: Model ActiveDirectory tem um novo parâmetro backup_operators</span><span class="sxs-lookup"><span data-stu-id="3c5b0-389">`az netappfiles account`: Model ActiveDirectory has a new parameter backup_operators</span></span>
* <span data-ttu-id="3c5b0-390">`az netappfiles volume show`: Model dataProtection tem um novo parâmetro snapshot</span><span class="sxs-lookup"><span data-stu-id="3c5b0-390">`az netappfiles volume show`: Model dataProtection has a new parameter snapshot</span></span>
* <span data-ttu-id="3c5b0-391">`az netappfiles volume show`: Model Volume tem um novo parâmetro snapshot_directory_visible</span><span class="sxs-lookup"><span data-stu-id="3c5b0-391">`az netappfiles volume show`: Model Volume has a new parameter snapshot_directory_visible</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-392">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-392">Network</span></span>

* <span data-ttu-id="3c5b0-393">`az network dns export`: exportação do FQDN para o tipo MX, PTR, NS e SRV em vez do caminho relativo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-393">`az network dns export`: export FQDN for MX, PTR, NS and SRV type instead of relative path</span></span>
* <span data-ttu-id="3c5b0-394">Suporte ao link privado para discos gerenciados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-394">Support private link for managed disks</span></span>
* <span data-ttu-id="3c5b0-395">`az network application-gateway auth-cert show`: adição de exemplo para demonstrar o formato do certificado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-395">`az network application-gateway auth-cert show`: Add example to demonstrate certificate format</span></span>
* <span data-ttu-id="3c5b0-396">`az network private-endpoint-connection`: suporte à configuração de aplicativos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-396">`az network private-endpoint-connection`: support app configuration</span></span>

### <a name="rbac"></a><span data-ttu-id="3c5b0-397">RBAC</span><span class="sxs-lookup"><span data-stu-id="3c5b0-397">RBAC</span></span>

* <span data-ttu-id="3c5b0-398">`az ad group create`: suporte à especificação da descrição durante a criação de um grupo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-398">`az ad group create`: support specify description when creating a group</span></span>
* <span data-ttu-id="3c5b0-399">`az role definition create`: impressão de mensagem legível em vez de exceção quando assignableScope for uma matriz vazia</span><span class="sxs-lookup"><span data-stu-id="3c5b0-399">`az role definition create`: print human readable message instead of exception when assignableScope is an empty array</span></span>
* <span data-ttu-id="3c5b0-400">[ALTERAÇÃO DA FALHA] `az ad sp create-for-rbac`: alteração da permissão padrão do certificado criado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-400">[BREAKING CHANGE] `az ad sp create-for-rbac`: change default permission of created certificate</span></span>

### <a name="sql"></a><span data-ttu-id="3c5b0-401">SQL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-401">SQL</span></span>

* <span data-ttu-id="3c5b0-402">`az sql server audit-policy`: adição de suporte à auditoria do SQL Server</span><span class="sxs-lookup"><span data-stu-id="3c5b0-402">`az sql server audit-policy`: Add sql server auditing support</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-403">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-403">Storage</span></span>

* <span data-ttu-id="3c5b0-404">`az storage blob copy start-batch`: correção nº 6018 para --source-sas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-404">`az storage blob copy start-batch`: Fix #6018 for --source-sas</span></span>
* <span data-ttu-id="3c5b0-405">`az storage account or-policy`: suporte à política de replicação de objeto de conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-405">`az storage account or-policy`: Support storage account object replication policy</span></span>
* <span data-ttu-id="3c5b0-406">Correção do problema nº 14083 para atualizar a versão do pacote do azure-multiapi-storage para o problema do pacote e suporte da versão à nova API</span><span class="sxs-lookup"><span data-stu-id="3c5b0-406">Fix issue #14083 to upgrade azure-multiapi-storage package version for package issue and new api version support</span></span>
* <span data-ttu-id="3c5b0-407">`az storage blob generate-sas`: adição de exemplos para --ip e refinamento da mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="3c5b0-407">`az storage blob generate-sas`: add examples for --ip  and refine error message</span></span>
* <span data-ttu-id="3c5b0-408">`az storage blob list`: correção do problema de next_marker</span><span class="sxs-lookup"><span data-stu-id="3c5b0-408">`az storage blob list`: Fix next_marker issue</span></span>

### <a name="synapse"></a><span data-ttu-id="3c5b0-409">Synapse</span><span class="sxs-lookup"><span data-stu-id="3c5b0-409">Synapse</span></span>

* <span data-ttu-id="3c5b0-410">Adição de cmdlets relacionados a workspace, sparkpool e sqlpool</span><span class="sxs-lookup"><span data-stu-id="3c5b0-410">Add workspace, sparkpool, sqlpool related cmdlets</span></span>
* <span data-ttu-id="3c5b0-411">Adição de comandos relacionados a spark job com base no track2 sdk</span><span class="sxs-lookup"><span data-stu-id="3c5b0-411">Add spark job releated commands based on track2 sdk</span></span>
* <span data-ttu-id="3c5b0-412">Adição de comandos relacionados ao recurso accesscontrol com base no track2 sdk</span><span class="sxs-lookup"><span data-stu-id="3c5b0-412">Add accesscontrol feature related commands based on track2 sdk</span></span>

### <a name="upgrade"></a><span data-ttu-id="3c5b0-413">Atualizar</span><span class="sxs-lookup"><span data-stu-id="3c5b0-413">Upgrade</span></span>

* <span data-ttu-id="3c5b0-414">Adição do comando `az upgrade` para atualizar a CLI do Azure e as extensões</span><span class="sxs-lookup"><span data-stu-id="3c5b0-414">Add `az upgrade` command to upgrade azure cli and extensions</span></span>

## <a name="august-11-2020"></a><span data-ttu-id="3c5b0-415">11 de agosto de 2020</span><span class="sxs-lookup"><span data-stu-id="3c5b0-415">August 11, 2020</span></span>

<span data-ttu-id="3c5b0-416">Versão 2.10.1</span><span class="sxs-lookup"><span data-stu-id="3c5b0-416">Version 2.10.1</span></span>

### <a name="app-service"></a><span data-ttu-id="3c5b0-417">Serviço de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-417">App Service</span></span>

* <span data-ttu-id="3c5b0-418">Correção nº 9887 webapp e functionapp, dar suporte à atribuição/remoção de identidade gerenciada pelo usuário</span><span class="sxs-lookup"><span data-stu-id="3c5b0-418">Fix #9887 webapp and functionapp, support assigning/removing user managed identity</span></span>
* <span data-ttu-id="3c5b0-419">Correção nº 1382, 14055: atualizar mensagens de erro para az webapp create e az webapp config container set</span><span class="sxs-lookup"><span data-stu-id="3c5b0-419">Fix #1382, #14055: Update error messages for az webapp create and az webapp config container set</span></span>
* <span data-ttu-id="3c5b0-420">`az webapp up`: corrigir a lógica de seleção padrão do ASP quando o parâmetro --plan não é fornecido</span><span class="sxs-lookup"><span data-stu-id="3c5b0-420">`az webapp up`: Fix default ASP selection logic when --plan parameter is not provided</span></span>

### <a name="appconfig"></a><span data-ttu-id="3c5b0-421">AppConfig</span><span class="sxs-lookup"><span data-stu-id="3c5b0-421">AppConfig</span></span>

* <span data-ttu-id="3c5b0-422">Dar suporte para habilitar/desabilitar PublicNetworkAccess durante a criação da loja</span><span class="sxs-lookup"><span data-stu-id="3c5b0-422">Support enabling/disabling PublicNetworkAccess during store creation</span></span>

### <a name="compute"></a><span data-ttu-id="3c5b0-423">Computação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-423">Compute</span></span>

* <span data-ttu-id="3c5b0-424">Dar suporte à associação de disco e instantâneo com um recurso de acesso a disco</span><span class="sxs-lookup"><span data-stu-id="3c5b0-424">Support associating disk and snapshot with a disk-access resource</span></span>

### <a name="lab"></a><span data-ttu-id="3c5b0-425">Laboratório</span><span class="sxs-lookup"><span data-stu-id="3c5b0-425">Lab</span></span>

* <span data-ttu-id="3c5b0-426">Correção do problema nº 7904: bug de validação de data na criação de VM do laboratório</span><span class="sxs-lookup"><span data-stu-id="3c5b0-426">Fix for issue #7904 date validation bug in lab vm creation</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-427">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-427">Storage</span></span>

* <span data-ttu-id="3c5b0-428">`az storage blob upload-batch`: correção do problema nº 14660 com argumentos não posicionais</span><span class="sxs-lookup"><span data-stu-id="3c5b0-428">`az storage blob upload-batch`: Fix issue #14660 with unpositional arguments</span></span>

## <a name="august-04-2020"></a><span data-ttu-id="3c5b0-429">04 de agosto de 2020</span><span class="sxs-lookup"><span data-stu-id="3c5b0-429">August 04, 2020</span></span>

<span data-ttu-id="3c5b0-430">Versão 2.10.0</span><span class="sxs-lookup"><span data-stu-id="3c5b0-430">Version 2.10.0</span></span>

### <a name="aks"></a><span data-ttu-id="3c5b0-431">AKS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-431">AKS</span></span>

* <span data-ttu-id="3c5b0-432">`az aks update`: Alteração do argumento --enable-aad para migrar um cluster não AAD habilitado para RBAC para um cluster AAD gerenciado por AKS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-432">`az aks update`: Change --enable-aad argument to migrate a RBAC-enabled non-AAD cluster to a AKS-managed AAD cluster</span></span>
* <span data-ttu-id="3c5b0-433">`az aks install-cli`: Adição de argumentos --kubelogin-version e --kubelogin-install-location para instalar o kubelogin</span><span class="sxs-lookup"><span data-stu-id="3c5b0-433">`az aks install-cli`: Add --kubelogin-version and --kubelogin-install-location arguments to install kubelogin</span></span>
* <span data-ttu-id="3c5b0-434">Adição do comando az aks nodepool get-upgrades</span><span class="sxs-lookup"><span data-stu-id="3c5b0-434">Add az aks nodepool get-upgrades command</span></span>

### <a name="ams"></a><span data-ttu-id="3c5b0-435">AMS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-435">AMS</span></span>

* <span data-ttu-id="3c5b0-436">Correção nº 14021: az ams account sp não é idempotente</span><span class="sxs-lookup"><span data-stu-id="3c5b0-436">Fix #14021: az ams account sp is not idempotent</span></span>

### <a name="apim"></a><span data-ttu-id="3c5b0-437">APIM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-437">APIM</span></span>

* <span data-ttu-id="3c5b0-438">importação da API de APIM: suporte à importação de API e aprimoramento de outros comandos da CLI de nível da API</span><span class="sxs-lookup"><span data-stu-id="3c5b0-438">apim api import: support API import and enchance other api level cli commands</span></span>

### <a name="app-service"></a><span data-ttu-id="3c5b0-439">Serviço de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-439">App Service</span></span>

* <span data-ttu-id="3c5b0-440">Correção nº 13035: Adição de validação para az webapp config access-restriction para evitar a adição de duplicatas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-440">Fix #13035: Add validation for az webapp config access-restriction to avoid adding duplicates</span></span>

### <a name="appconfig"></a><span data-ttu-id="3c5b0-441">AppConfig</span><span class="sxs-lookup"><span data-stu-id="3c5b0-441">AppConfig</span></span>

* <span data-ttu-id="3c5b0-442">Adoção de SKU padrão se não for especificado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-442">Default to standard sku if not specified</span></span>
* <span data-ttu-id="3c5b0-443">[ALTERAÇÃO SIGNIFICATIVA] Configurações de suporte com tipo de conteúdo JSON</span><span class="sxs-lookup"><span data-stu-id="3c5b0-443">[BREAKING CHANGE] Support settings with JSON content type</span></span>

### <a name="arm"></a><span data-ttu-id="3c5b0-444">ARM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-444">ARM</span></span>

* <span data-ttu-id="3c5b0-445">`az resource tag`: Correção do bug de marcação managedApp e alguns problemas de teste relacionados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-445">`az resource tag`: Fix the bug of managedApp tagging and some related test issues</span></span>
* <span data-ttu-id="3c5b0-446">`az deployment mg/tenant what-if`: Adição de suporte ao grupo de gerenciamento e à implantação de nível de locatário What-If</span><span class="sxs-lookup"><span data-stu-id="3c5b0-446">`az deployment mg/tenant what-if`: Add support to management group and tenant level deployment What-If</span></span>
* <span data-ttu-id="3c5b0-447">`az deployment mg/tenant create`: Adição do parâmetro --confirm-with-what-if/-c.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-447">`az deployment mg/tenant create`: Add --confirm-with-what-if/-c parameter.</span></span>
* <span data-ttu-id="3c5b0-448">`az deployment mg/tenant create`: Adição do parâmetro --what-if-result-format/-r.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-448">`az deployment mg/tenant create`: Add --what-if-result-format/-r parameter.</span></span>
* <span data-ttu-id="3c5b0-449">`az deployment mg/tenant create`: adicionar parâmetro --what-if-exclude-change-types/-x.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-449">`az deployment mg/tenant create`: Add --what-if-exclude-change-types/-x parameter.</span></span>
* <span data-ttu-id="3c5b0-450">`az tag`: az tag support para parâmetro ID de recurso</span><span class="sxs-lookup"><span data-stu-id="3c5b0-450">`az tag`: az tag support for resource id parameter</span></span>

### <a name="backup"></a><span data-ttu-id="3c5b0-451">Backup</span><span class="sxs-lookup"><span data-stu-id="3c5b0-451">Backup</span></span>

* <span data-ttu-id="3c5b0-452">Disparar a descoberta de contêiner/item AFS somente quando necessário</span><span class="sxs-lookup"><span data-stu-id="3c5b0-452">Trigger AFS container/item discovery only when needed</span></span>

### <a name="cdn"></a><span data-ttu-id="3c5b0-453">CDN</span><span class="sxs-lookup"><span data-stu-id="3c5b0-453">CDN</span></span>

* <span data-ttu-id="3c5b0-454">Adicionar campos de link privado à origem</span><span class="sxs-lookup"><span data-stu-id="3c5b0-454">Add private link fields to origin</span></span>

### <a name="compute"></a><span data-ttu-id="3c5b0-455">Computação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-455">Compute</span></span>

* <span data-ttu-id="3c5b0-456">`az vm/vmss create`: Selecione um nome de usuário válido para usuário se o nome de usuário padrão for inválido</span><span class="sxs-lookup"><span data-stu-id="3c5b0-456">`az vm/vmss create`: Select a valid username for user if the default username is invalid</span></span>
* <span data-ttu-id="3c5b0-457">`az vm update`: suporte à imagem entre locatários</span><span class="sxs-lookup"><span data-stu-id="3c5b0-457">`az vm update`: support cross tenant image</span></span>
* <span data-ttu-id="3c5b0-458">`az disk-access`: Adicionar novo grupo de comandos para operar o recurso de acesso ao disco</span><span class="sxs-lookup"><span data-stu-id="3c5b0-458">`az disk-access`: Add new command group to operate disk access resource</span></span>
* <span data-ttu-id="3c5b0-459">Suporte ao posicionamento automático do grupo de hosts dedicado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-459">Support dedicated host group automatic placement</span></span>
* <span data-ttu-id="3c5b0-460">Suporte a PPG e SPG no modo de orquestração de VMSS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-460">Support ppg and spg in VMSS orchestration mode</span></span>

### <a name="config"></a><span data-ttu-id="3c5b0-461">Config</span><span class="sxs-lookup"><span data-stu-id="3c5b0-461">Config</span></span>

* <span data-ttu-id="3c5b0-462">`az config`: Adição do novo módulo de comando `config`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-462">`az config`: Add new `config` command module</span></span>

### <a name="extension"></a><span data-ttu-id="3c5b0-463">Extensão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-463">Extension</span></span>

* <span data-ttu-id="3c5b0-464">Suporte à instalação automática de uma extensão se a extensão de um comando não estiver instalada</span><span class="sxs-lookup"><span data-stu-id="3c5b0-464">Support automatically installing an extension if the extension of a command is not installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="3c5b0-465">HDInsight</span><span class="sxs-lookup"><span data-stu-id="3c5b0-465">HDInsight</span></span>

* <span data-ttu-id="3c5b0-466">Adição de três parâmetros ao comando `az hdinsight create` para compatibilidade com o link privado e o recurso de criptografia em trânsito:</span><span class="sxs-lookup"><span data-stu-id="3c5b0-466">Add 3 parameters to the command `az hdinsight create` to support private link and encryption in transit feature:</span></span>

### <a name="iot-hub"></a><span data-ttu-id="3c5b0-467">Hub IoT</span><span class="sxs-lookup"><span data-stu-id="3c5b0-467">Iot Hub</span></span>

* <span data-ttu-id="3c5b0-468">Correção nº 7792: A criação do Hub IoT não é idempotente</span><span class="sxs-lookup"><span data-stu-id="3c5b0-468">Fix #7792: IoT Hub Create is not idempotent</span></span>

### <a name="iot-central"></a><span data-ttu-id="3c5b0-469">Central da IoT</span><span class="sxs-lookup"><span data-stu-id="3c5b0-469">IoT Central</span></span>

* <span data-ttu-id="3c5b0-470">Adição de lista de opções de parâmetros para IoT Central</span><span class="sxs-lookup"><span data-stu-id="3c5b0-470">Add paramater option list for iot central</span></span>

### <a name="keyvault"></a><span data-ttu-id="3c5b0-471">KeyVault</span><span class="sxs-lookup"><span data-stu-id="3c5b0-471">KeyVault</span></span>

* <span data-ttu-id="3c5b0-472">`az keyvault key encrypt/decrypt`: adição de parâmetro `--data-type` para especificar explicitamente o tipo de dado original</span><span class="sxs-lookup"><span data-stu-id="3c5b0-472">`az keyvault key encrypt/decrypt`: add parameter `--data-type` for explicitly specifing the type of original data</span></span>

### <a name="monitor"></a><span data-ttu-id="3c5b0-473">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-473">Monitor</span></span>

* <span data-ttu-id="3c5b0-474">`az monitor log-analytics workspace data-export`: suporte ao namespace do hub de eventos como o destino.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-474">`az monitor log-analytics workspace data-export`: support event hub namespace as the destination.</span></span>
* <span data-ttu-id="3c5b0-475">`az monitor autoscale`: suporte a namespace e dimensões para --condition</span><span class="sxs-lookup"><span data-stu-id="3c5b0-475">`az monitor autoscale`: support namespace and dimensions for --condition</span></span>

### <a name="netappfiles"></a><span data-ttu-id="3c5b0-476">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="3c5b0-476">NetAppFiles</span></span>

* <span data-ttu-id="3c5b0-477">`az volume revert`:  Adição de Reversão de Volume para reverter um volume para um de seus instantâneos.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-477">`az volume revert`:  Add Volume Revert to revert a volume to one of its snapshots.</span></span>
* <span data-ttu-id="3c5b0-478">[ALTERAÇÃO SIGNIFICATIVA] Remoção de `az netappfiles mount-target`.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-478">[BREAKING CHANGE] Remove `az netappfiles mount-target`.</span></span>
* <span data-ttu-id="3c5b0-479">`az volume show`: Adição de site para Propriedades do Active Directory</span><span class="sxs-lookup"><span data-stu-id="3c5b0-479">`az volume show`: Add site to Active Directory Properties</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-480">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-480">Network</span></span>

* <span data-ttu-id="3c5b0-481">`az application-gateway private-link add`: suporte para especificar uma sub-rede existente por ID</span><span class="sxs-lookup"><span data-stu-id="3c5b0-481">`az application-gateway private-link add`: support to specify an existing subnet by ID</span></span>
* <span data-ttu-id="3c5b0-482">`az network application-gateway waf-policy create`: versão e tipo de suporte</span><span class="sxs-lookup"><span data-stu-id="3c5b0-482">`az network application-gateway waf-policy create`: support version and type</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-483">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-483">Storage</span></span>

* <span data-ttu-id="3c5b0-484">Correção nº 10302: Suporte à estimativa de tipo de conteúdo ao sincronizar arquivos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-484">Fix #10302: Support guess content-type when synchronizing files</span></span>
* <span data-ttu-id="3c5b0-485">`az storage blob lease`: Aplicação de nova versão de API para operações de concessão de blob</span><span class="sxs-lookup"><span data-stu-id="3c5b0-485">`az storage blob lease`: Apply new api version for blob lease operations</span></span>
* <span data-ttu-id="3c5b0-486">`az storage fs access`: Suporte a credencial do AAD no gerenciamento de controle de acesso para conta do ADLS Gen2</span><span class="sxs-lookup"><span data-stu-id="3c5b0-486">`az storage fs access`: Support AAD credential in managing access control for ADLS Gen2 account</span></span>
* <span data-ttu-id="3c5b0-487">`az storage share-rm create/update`: adição de --access-tier para dar suporte à camada de acesso</span><span class="sxs-lookup"><span data-stu-id="3c5b0-487">`az storage share-rm create/update`: add --access-tier to support access tier</span></span>

## <a name="july-16-2020"></a><span data-ttu-id="3c5b0-488">16 de julho de 2020</span><span class="sxs-lookup"><span data-stu-id="3c5b0-488">July 16, 2020</span></span>

<span data-ttu-id="3c5b0-489">Versão 2.9.1</span><span class="sxs-lookup"><span data-stu-id="3c5b0-489">Version 2.9.1</span></span>

### <a name="aks"></a><span data-ttu-id="3c5b0-490">AKS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-490">AKS</span></span>

* <span data-ttu-id="3c5b0-491">Remove a configuração explícita de VMSS no comando de exemplo do Windows, pois ele agora é padrão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-491">Remove explicit setting of VMSS in Windows example command since it is now default</span></span>

### <a name="iot"></a><span data-ttu-id="3c5b0-492">IoT</span><span class="sxs-lookup"><span data-stu-id="3c5b0-492">IoT</span></span>

* <span data-ttu-id="3c5b0-493">[ALTERAÇÃO DA FALHA] `az iot pnp`: Remove comandos de versão prévia do IoT PNP da CLI principal</span><span class="sxs-lookup"><span data-stu-id="3c5b0-493">[BREAKING CHANGE] `az iot pnp`: Remove IoT PNP preview commands from core CLI</span></span>

### <a name="rest"></a><span data-ttu-id="3c5b0-494">REST</span><span class="sxs-lookup"><span data-stu-id="3c5b0-494">REST</span></span>

* <span data-ttu-id="3c5b0-495">Correção nº14152: `az rest`: aceita URLs do ARM sem a ID de assinatura</span><span class="sxs-lookup"><span data-stu-id="3c5b0-495">Fix #14152: `az rest`: Accept ARM URLs without subscription ID</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-496">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-496">Storage</span></span>

* <span data-ttu-id="3c5b0-497">Correção nº 14138: torna algumas permissões opcionais</span><span class="sxs-lookup"><span data-stu-id="3c5b0-497">Fix #14138: Make some permissions optional</span></span>

## <a name="july-14-2020"></a><span data-ttu-id="3c5b0-498">14 de julho de 2020</span><span class="sxs-lookup"><span data-stu-id="3c5b0-498">July 14, 2020</span></span>

<span data-ttu-id="3c5b0-499">Versão 2.9.0</span><span class="sxs-lookup"><span data-stu-id="3c5b0-499">Version 2.9.0</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-500">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-500">ACR</span></span>

* <span data-ttu-id="3c5b0-501">Manipular o link do artefato de log do Registro para os logs de fluxo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-501">Handle log artifact link from Registry to stream logs</span></span>
* <span data-ttu-id="3c5b0-502">Substituir comandos helm2</span><span class="sxs-lookup"><span data-stu-id="3c5b0-502">Deprecate helm2 commands</span></span>

### <a name="aks"></a><span data-ttu-id="3c5b0-503">AKS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-503">AKS</span></span>

* <span data-ttu-id="3c5b0-504">`az aks create`: adiciona o argumento --enable-aad</span><span class="sxs-lookup"><span data-stu-id="3c5b0-504">`az aks create`: add --enable-aad argument</span></span>
* <span data-ttu-id="3c5b0-505">`az aks update`: adiciona o argumento --enable-aad</span><span class="sxs-lookup"><span data-stu-id="3c5b0-505">`az aks update`: add --enable-aad argument</span></span>

### <a name="apim"></a><span data-ttu-id="3c5b0-506">APIM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-506">APIM</span></span>

* <span data-ttu-id="3c5b0-507">Comandos az apim api gerais adicionados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-507">Added general az apim api commands</span></span>

### <a name="appconfig"></a><span data-ttu-id="3c5b0-508">AppConfig</span><span class="sxs-lookup"><span data-stu-id="3c5b0-508">AppConfig</span></span>

* <span data-ttu-id="3c5b0-509">Adicionar exemplo para usar --fields na revisão do appconfig</span><span class="sxs-lookup"><span data-stu-id="3c5b0-509">Add example for using --fields in appconfig revision</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-510">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-510">AppService</span></span>

* <span data-ttu-id="3c5b0-511">`az functionapp create`: Suporte para Java 11 e PowerShell 7 adicionado.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-511">`az functionapp create`: Added support for Java 11 and Powershell 7.</span></span> <span data-ttu-id="3c5b0-512">Suporte à API de pilhas adicionado.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-512">Added Stacks API Support.</span></span>
* <span data-ttu-id="3c5b0-513">Correção nº 14208 falha na criação de um aplicativo com vários contêineres</span><span class="sxs-lookup"><span data-stu-id="3c5b0-513">Fix #14208 multi-container app creation fails</span></span>
* <span data-ttu-id="3c5b0-514">Corrige az webapp create – usa pilhas de runtime embutidas em código</span><span class="sxs-lookup"><span data-stu-id="3c5b0-514">Fix az webapp create - use hardcoded runtime stacks</span></span>

### <a name="arm"></a><span data-ttu-id="3c5b0-515">ARM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-515">ARM</span></span>

* <span data-ttu-id="3c5b0-516">`az resource tag`: corrige o problema de marcar recursos com o tipo de recurso `Microsoft.ContainerInstance/containerGroups`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-516">`az resource tag`: Fix the problem of tagging resources with resource type `Microsoft.ContainerInstance/containerGroups`</span></span>

### <a name="compute"></a><span data-ttu-id="3c5b0-517">Computação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-517">Compute</span></span>

* <span data-ttu-id="3c5b0-518">Avançar os discos de versão 2020-05-01, computação 2020-06-01</span><span class="sxs-lookup"><span data-stu-id="3c5b0-518">Bump version disks 2020-05-01, compute 2020-06-01</span></span>
* <span data-ttu-id="3c5b0-519">Criptografia dupla do conjunto de criptografia de disco</span><span class="sxs-lookup"><span data-stu-id="3c5b0-519">Double encryption of disk encryption set</span></span>
* <span data-ttu-id="3c5b0-520">`az vmss update`: dá suporte à especificação de imagem entre locatários.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-520">`az vmss update`: support specify cross tenant image.</span></span>
* <span data-ttu-id="3c5b0-521">`az sig image-version create`: dá suporte à especificação de imagem entre locatários.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-521">`az sig image-version create`: support specify cross tenant image.</span></span>
* <span data-ttu-id="3c5b0-522">vm/vmss create: Criptografia de cache e dados em trânsito para discos do sistema operacional/de dados e discos temporários para VM e VMSS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-522">vm/vmss create: Encryption of cache & data-in-transit for OS/Data disks and temp disks for VM & VMSS</span></span>
* <span data-ttu-id="3c5b0-523">Adicionar operação de remoção simulada para VM e VMSS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-523">Add simulate-eviction operation for VM and VMSS</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="3c5b0-524">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="3c5b0-524">CosmosDB</span></span>

* <span data-ttu-id="3c5b0-525">Recursos recentes: Autoscale, IpRules, EnableFreeTier e EnableAnalyticalStorage</span><span class="sxs-lookup"><span data-stu-id="3c5b0-525">Recent features: Autoscale, IpRules, EnableFreeTier and EnableAnalyticalStorage</span></span>

### <a name="eventgrid"></a><span data-ttu-id="3c5b0-526">EventGrid</span><span class="sxs-lookup"><span data-stu-id="3c5b0-526">EventGrid</span></span>

* <span data-ttu-id="3c5b0-527">Adicionar suporte de CLI para 2020-04-01-preview e marcar a versão prévia dos recursos com is_Preview=True</span><span class="sxs-lookup"><span data-stu-id="3c5b0-527">Add CLI support for 2020-04-01-preview and mark preview features with is_Preview=True</span></span>

### <a name="find"></a><span data-ttu-id="3c5b0-528">Localizar</span><span class="sxs-lookup"><span data-stu-id="3c5b0-528">Find</span></span>

* <span data-ttu-id="3c5b0-529">Correção nº 14094 az find Corrige consultas que falhavam quando não estavam conectadas e quando a telemetria estava desabilitada</span><span class="sxs-lookup"><span data-stu-id="3c5b0-529">Fix #14094 az find Fix Queries failing when not logged in and when telemetry is disabled</span></span>

### <a name="hdinsight"></a><span data-ttu-id="3c5b0-530">HDInsight</span><span class="sxs-lookup"><span data-stu-id="3c5b0-530">HDInsight</span></span>

* <span data-ttu-id="3c5b0-531">Adicionar dois comandos para dar suporte ao recurso de reinicialização do nó do hdinsight</span><span class="sxs-lookup"><span data-stu-id="3c5b0-531">Add two commands to support hdinsight node reboot feature</span></span>

### <a name="monitor"></a><span data-ttu-id="3c5b0-532">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-532">Monitor</span></span>

* <span data-ttu-id="3c5b0-533">Remover sinalizador de visualização para comandos no workspace do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="3c5b0-533">Remove preview flag for commands under Log Analytics workspace</span></span>
* <span data-ttu-id="3c5b0-534">`az monitor diagnostic-settings subscription`: Dar suporte às configurações de diagnóstico para a assinatura</span><span class="sxs-lookup"><span data-stu-id="3c5b0-534">`az monitor diagnostic-settings subscription`: Support diagnositc settings for subscription</span></span>
* <span data-ttu-id="3c5b0-535">`az monitor metrics`: dá suporte para ', ' e '|' no nome da métrica</span><span class="sxs-lookup"><span data-stu-id="3c5b0-535">`az monitor metrics`: support ',' and '|' in metric name</span></span>
* <span data-ttu-id="3c5b0-536">`az monitor log-analytics workspace data-export`: suporte à exportação de dados do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="3c5b0-536">`az monitor log-analytics workspace data-export`: support log analytics data export</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-537">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-537">Network</span></span>

* <span data-ttu-id="3c5b0-538">`az network application-gateway frontend-ip update`: Substituir o parâmetro --public-ip-address</span><span class="sxs-lookup"><span data-stu-id="3c5b0-538">`az network application-gateway frontend-ip update`: Deprecating the --public-ip-address parameter</span></span>
* <span data-ttu-id="3c5b0-539">Avançar azure-mgmt-network para 11.0.0</span><span class="sxs-lookup"><span data-stu-id="3c5b0-539">Bump azure-mgmt-network to 11.0.0</span></span>
* <span data-ttu-id="3c5b0-540">`az network express-route gateway connection`: dá suporte à configuração de roteamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-540">`az network express-route gateway connection`: support routing configuration</span></span>
* <span data-ttu-id="3c5b0-541">`az network virtual-appliance`: dá suporte à solução de virtualização de rede do Azure.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-541">`az network virtual-appliance`: Support Azure network virtual appliance.</span></span>
* <span data-ttu-id="3c5b0-542">Recurso de link privado de suporte do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-542">Application Gateway support private link feature</span></span>

### <a name="policyinsights"></a><span data-ttu-id="3c5b0-543">PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="3c5b0-543">PolicyInsights</span></span>

* <span data-ttu-id="3c5b0-544">`az policy state`: adiciona o comando trigger-scan para disparar avaliações de conformidade de política</span><span class="sxs-lookup"><span data-stu-id="3c5b0-544">`az policy state`: add trigger-scan command to trigger policy compliance evaluations</span></span>
* <span data-ttu-id="3c5b0-545">`az policy state list`: expõe versões de entidades de política em cada registro de conformidade</span><span class="sxs-lookup"><span data-stu-id="3c5b0-545">`az policy state list`: expose versions of policy entities in each compliance record</span></span>

### <a name="profile"></a><span data-ttu-id="3c5b0-546">Perfil</span><span class="sxs-lookup"><span data-stu-id="3c5b0-546">Profile</span></span>

* <span data-ttu-id="3c5b0-547">`az account get-access-token`: Mostra expiresOn para Identidade Gerenciada</span><span class="sxs-lookup"><span data-stu-id="3c5b0-547">`az account get-access-token`: Show expiresOn for Managed Identity</span></span>

### <a name="rdbms"></a><span data-ttu-id="3c5b0-548">RDBMS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-548">RDBMS</span></span>

* <span data-ttu-id="3c5b0-549">Dar suporte à versão mínima do TLS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-549">Support Minimum TLS version</span></span>
* <span data-ttu-id="3c5b0-550">Adicionar criptografia de infraestrutura para o Azure Postgres e MySQL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-550">Add Infrastructure Encryption for Azure Postgres and MySQL</span></span>

### <a name="security"></a><span data-ttu-id="3c5b0-551">Segurança</span><span class="sxs-lookup"><span data-stu-id="3c5b0-551">Security</span></span>

* <span data-ttu-id="3c5b0-552">Adicionar comandos allowed_connections</span><span class="sxs-lookup"><span data-stu-id="3c5b0-552">Add allowed_connections commands</span></span>
* <span data-ttu-id="3c5b0-553">Adicionar comandos hardeningss da rede adaptável</span><span class="sxs-lookup"><span data-stu-id="3c5b0-553">Add Adaptive network hardeningss commands</span></span>
* <span data-ttu-id="3c5b0-554">Adicionar comandos adaptive_application_controls</span><span class="sxs-lookup"><span data-stu-id="3c5b0-554">Add adaptive_application_controls commands</span></span>
* <span data-ttu-id="3c5b0-555">Adição de az security iot-solution/ iot-alerts/iot-recommendations/iot-analytics REST à CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="3c5b0-555">Addition of az security iot-solution/ iot-alerts/iot-recommendations/iot-analytics REST to Azure CLI</span></span>
* <span data-ttu-id="3c5b0-556">Adicionar CLI de conformidade regulatória</span><span class="sxs-lookup"><span data-stu-id="3c5b0-556">Add regulatory compliance CLI</span></span>

### <a name="signalr"></a><span data-ttu-id="3c5b0-557">SignalR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-557">SignalR</span></span>

* <span data-ttu-id="3c5b0-558">Adicionar recursos, incluindo o gerenciamento de conexões de ponto de extremidade privado, regras de rede e upstream</span><span class="sxs-lookup"><span data-stu-id="3c5b0-558">Add features including managing private endpoint connections, network rules and upstream</span></span>

### <a name="sql"></a><span data-ttu-id="3c5b0-559">SQL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-559">SQL</span></span>

* <span data-ttu-id="3c5b0-560">`az sql mi create`, `az sql mi update`: adiciona o parâmetro `--tags` para dar suporte à marcação de recursos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-560">`az sql mi create`, `az sql mi update`: Add `--tags` parameter to support resource tagging</span></span>
* <span data-ttu-id="3c5b0-561">`az sql mi failover`: dá suporte ao failover de um ponto primário ou secundário</span><span class="sxs-lookup"><span data-stu-id="3c5b0-561">`az sql mi failover`: Support failover from primary or secondary point</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-562">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-562">Storage</span></span>

* <span data-ttu-id="3c5b0-563">`az storage account create/update`: adiciona --allow-blob-public-access para permitir ou não permitir acesso público para blob e contêineres</span><span class="sxs-lookup"><span data-stu-id="3c5b0-563">`az storage account create/update`: Add --allow-blob-public-access to allow or disallow public access for blob and containers</span></span>
* <span data-ttu-id="3c5b0-564">`az storage account create/update`: adiciona `--min-tls-version` para dar suporte à definição da versão mínima do TLS a ser permitida em solicitações de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-564">`az storage account create/update`: Add `--min-tls-version` to support setting the minimum TLS version to be permitted on requests to storage.</span></span>
* <span data-ttu-id="3c5b0-565">Remover credencial de token de check-in</span><span class="sxs-lookup"><span data-stu-id="3c5b0-565">Remove check in token credential</span></span>
* <span data-ttu-id="3c5b0-566">Corrigir o nome da conta de armazenamento em exemplos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-566">Fix the storage account name in examples</span></span>

### <a name="webapp"></a><span data-ttu-id="3c5b0-567">Webapp</span><span class="sxs-lookup"><span data-stu-id="3c5b0-567">Webapp</span></span>

* <span data-ttu-id="3c5b0-568">Bugfix: az webapp log deployment show – retorna logs de implantação em vez de metadados de log</span><span class="sxs-lookup"><span data-stu-id="3c5b0-568">Bugfix: az webapp log deployment show - return deployment logs instead of log metadata</span></span>
* <span data-ttu-id="3c5b0-569">Bugfix: az webapp vnet-integration add – corrige o tratamento de erro se o nome da VNet é inadequado, dá suporte à ID do recurso da vnet</span><span class="sxs-lookup"><span data-stu-id="3c5b0-569">Bugfix: az webapp vnet-integration add - fix error handling if bad vnet name, support vnet resource ID</span></span>

## <a name="june-23-2020"></a><span data-ttu-id="3c5b0-570">23 de junho de 2020</span><span class="sxs-lookup"><span data-stu-id="3c5b0-570">June 23, 2020</span></span>

<span data-ttu-id="3c5b0-571">Versão 2.8.0</span><span class="sxs-lookup"><span data-stu-id="3c5b0-571">Version 2.8.0</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-572">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-572">ACR</span></span>

* <span data-ttu-id="3c5b0-573">Adicionar suporte para desabilitar roteamento/ponto de extremidade da região</span><span class="sxs-lookup"><span data-stu-id="3c5b0-573">Add support for region endpoint disable / routing disable</span></span>
* <span data-ttu-id="3c5b0-574">[ALTERAÇÃO DA FALHA] `az acr login --expose-token` não aceita nome de usuário e senha</span><span class="sxs-lookup"><span data-stu-id="3c5b0-574">[BREAKING CHANGE] `az acr login --expose-token` does not accept username and password</span></span>

### <a name="acs"></a><span data-ttu-id="3c5b0-575">ACS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-575">ACS</span></span>

* <span data-ttu-id="3c5b0-576">Remover o cluster privado e a API 2019-10-27-preview</span><span class="sxs-lookup"><span data-stu-id="3c5b0-576">Remove private cluster and 2019-10-27-preview API</span></span>

### <a name="aks"></a><span data-ttu-id="3c5b0-577">AKS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-577">AKS</span></span>

* <span data-ttu-id="3c5b0-578">Suporte a --yes para az aks upgrade</span><span class="sxs-lookup"><span data-stu-id="3c5b0-578">Support --yes for az aks upgrade</span></span>
* <span data-ttu-id="3c5b0-579">Reverter "alteração da sku de vm padrão para Standard_D2s_v3 (#13541)"</span><span class="sxs-lookup"><span data-stu-id="3c5b0-579">Revert "change default vm sku to Standard_D2s_v3 (#13541)"</span></span>
* <span data-ttu-id="3c5b0-580">Adicionar "az aks update --uptime-sla"</span><span class="sxs-lookup"><span data-stu-id="3c5b0-580">Add "az aks update --uptime-sla"</span></span>
* <span data-ttu-id="3c5b0-581">Corrigir erro de digitação no comando az aks update</span><span class="sxs-lookup"><span data-stu-id="3c5b0-581">Fix typo in az aks update command</span></span>
* <span data-ttu-id="3c5b0-582">Alteração para dar suporte ao pool de agentes do nó 0 e bloquear a escala manual do pool habilitado para CAS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-582">Change to support 0 node agent pool and block manual scale for CAS enabled pool</span></span>
* <span data-ttu-id="3c5b0-583">Corrigir erro de digitação em VirtualMachineScaleSets e atualizar referências a versões do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="3c5b0-583">Fix typo on VirtualMachineScaleSets and update references to Kubernetes versions</span></span>

### <a name="ams"></a><span data-ttu-id="3c5b0-584">AMS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-584">AMS</span></span>

* <span data-ttu-id="3c5b0-585">ALTERAR o texto da ajuda do parâmetro "--expiry".</span><span class="sxs-lookup"><span data-stu-id="3c5b0-585">CHANGE help text for "--expiry" parameter.</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-586">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-586">AppService</span></span>

* <span data-ttu-id="3c5b0-587">`az webapp log deployment show`: mostrar o log de implantação mais recente ou os logs de uma implantação específica se a ID da implantação for especificada</span><span class="sxs-lookup"><span data-stu-id="3c5b0-587">`az webapp log deployment show`: Show the latest deployment log, or the deployment logs of a specific deployment if deployment-id is specified</span></span>
* <span data-ttu-id="3c5b0-588">`az webapp log deployment list`: lista de logs de implantação disponíveis</span><span class="sxs-lookup"><span data-stu-id="3c5b0-588">`az webapp log deployment list`: List of deployment logs available</span></span>
* <span data-ttu-id="3c5b0-589">Correção: erro de superfície quando um nome de webapp inválido é fornecido</span><span class="sxs-lookup"><span data-stu-id="3c5b0-589">Fix: Surface error when invalid webapp name provided</span></span>
* <span data-ttu-id="3c5b0-590">Correção #13261: az webapp list-runtimes usa a lista estática até que a nova API de Pilhas Disponíveis esteja disponível</span><span class="sxs-lookup"><span data-stu-id="3c5b0-590">Fix #13261 az webapp list-runtimes use static list until new Available Stacks API is available</span></span>
* <span data-ttu-id="3c5b0-591">`az appservice ase create`: correção na criação do problema #13361</span><span class="sxs-lookup"><span data-stu-id="3c5b0-591">`az appservice ase create`: Fix create issue #13361</span></span>
* <span data-ttu-id="3c5b0-592">`az appservice ase list-addresses`: correção na alteração do SDK #13140.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-592">`az appservice ase list-addresses`: Fix change of SDK #13140.</span></span>
* <span data-ttu-id="3c5b0-593">Correção da criação de webapp/slot para Contêineres do Windows</span><span class="sxs-lookup"><span data-stu-id="3c5b0-593">Fix webapp/slot creation for Windows Containers</span></span>
* <span data-ttu-id="3c5b0-594">`az webapp auth update`: adicionar parâmetro opcional para atualizar a versão do runtime</span><span class="sxs-lookup"><span data-stu-id="3c5b0-594">`az webapp auth update`: Add optional parameter to update runtime-version</span></span>
* <span data-ttu-id="3c5b0-595">Suporte para listar, excluir, aprovar e rejeitar conexão de ponto de extremidade privado para webapp na CLI</span><span class="sxs-lookup"><span data-stu-id="3c5b0-595">Support list, delete, approve and reject private endpoint connection for webapp in CLI</span></span>
* <span data-ttu-id="3c5b0-596">Correção #13888: adicionar suporte para WebApps Estáticos: comandos get, list, create</span><span class="sxs-lookup"><span data-stu-id="3c5b0-596">Fix #13888 : Add support for Static WebApps: get, list, create commands</span></span>
* <span data-ttu-id="3c5b0-597">Mensagens de erro aprimoradas para Conexão de Túnel SSH</span><span class="sxs-lookup"><span data-stu-id="3c5b0-597">Improved error messages for SSH Tunnel Connection</span></span>

### <a name="arm"></a><span data-ttu-id="3c5b0-598">ARM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-598">ARM</span></span>

* <span data-ttu-id="3c5b0-599">`az tag`: adicionar exemplos para -h</span><span class="sxs-lookup"><span data-stu-id="3c5b0-599">`az tag`: Add examples for -h</span></span>
* <span data-ttu-id="3c5b0-600">`az deployment group/sub what-if`: adicionar parâmetro --exclude-change-types/-x.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-600">`az deployment group/sub what-if`: Add --exclude-change-types/-x parameter.</span></span>
* <span data-ttu-id="3c5b0-601">`az deployment group/sub/mg/tenant create`: adicionar parâmetro --what-if-exclude-change-types/-x.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-601">`az deployment group/sub/mg/tenant create`: Add --what-if-exclude-change-types/-x parameter.</span></span>
* <span data-ttu-id="3c5b0-602">`az deployment group/sub/mg/tenant validate`: mostrar mensagens de erro em um formato melhor.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-602">`az deployment group/sub/mg/tenant validate`: Show error messages in a better format.</span></span>
* <span data-ttu-id="3c5b0-603">`az group export`: adicionar novos parâmetros `--skip-resource-name-params` e `--skip-all-params` para dar suporte para ignorar parametrização</span><span class="sxs-lookup"><span data-stu-id="3c5b0-603">`az group export`: Add new parameters `--skip-resource-name-params` and `--skip-all-params` to support skip parameterization</span></span>
* <span data-ttu-id="3c5b0-604">Adicionar az feature unregister api</span><span class="sxs-lookup"><span data-stu-id="3c5b0-604">Add az feature unregister api</span></span>

### <a name="aro"></a><span data-ttu-id="3c5b0-605">ARO</span><span class="sxs-lookup"><span data-stu-id="3c5b0-605">ARO</span></span>

* <span data-ttu-id="3c5b0-606">Adicionar Public e Private aos parâmetros para obter ajuda com a visibilidade de entrada/apiserver</span><span class="sxs-lookup"><span data-stu-id="3c5b0-606">Add Public, Private to params for help with ingress/apiserver visibility</span></span>

### <a name="batch"></a><span data-ttu-id="3c5b0-607">Lote</span><span class="sxs-lookup"><span data-stu-id="3c5b0-607">Batch</span></span>

* <span data-ttu-id="3c5b0-608">`az batch account create`: adicionar novo parâmetro `--public-network-access`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-608">`az batch account create`: Add new parameter `--public-network-access`</span></span>
* <span data-ttu-id="3c5b0-609">`az batch account create`: adicionar novo parâmetro `--identity-type`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-609">`az batch account create`: Add new parameter `--identity-type`</span></span>
* <span data-ttu-id="3c5b0-610">`az batch account set`: adicionar novo parâmetro `--identity-type`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-610">`az batch account set`: Add new parameter `--identity-type`</span></span>
* <span data-ttu-id="3c5b0-611">[ALTERAÇÃO SIGNIFICATIVA] az batch pool create: ao criar um pool usando uma imagem personalizada, a propriedade --image agora pode se referir apenas a uma imagem da Galeria de Imagens Compartilhadas.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-611">[BREAKING CHANGE] az batch pool create: When creating a pool using a custom image, the --image property of can now only refer to a Shared Image Gallery image.</span></span>
* <span data-ttu-id="3c5b0-612">[ALTERAÇÃO SIGNIFICATIVA] az batch pool create: ao criar um pool com a opção --json-file e especificar uma networkConfiguration, a propriedade publicIPs foi movida para uma nova propriedade publicIPAddressConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-612">[BREAKING CHANGE] az batch pool create: When creating a pool with --json-file option and specifying a networkConfiguration, the publicIPs property has moved in to a new property publicIPAddressConfiguration.</span></span> <span data-ttu-id="3c5b0-613">Essa nova propriedade também dá suporte a uma nova propriedade ipAddressProvisioningType, que especifica como o pool deve alocar os IPs, e a uma propriedade publicIPs, que permite a configuração de uma lista de recursos de PublicIP a serem usados caso ipAddressProvisioningType seja definido como UserManaged</span><span class="sxs-lookup"><span data-stu-id="3c5b0-613">This new property also supports a new ipAddressProvisioningType property which specifies how the pool should allocate IP's and a publicIPs property which allows for configuration of a list of PublicIP resources to use in the case ipAddressProvisioningType is set to UserManaged</span></span>
* <span data-ttu-id="3c5b0-614">`az network private-link-resource`: adicionar suporte para o recurso Microsoft.Batch batchAccount</span><span class="sxs-lookup"><span data-stu-id="3c5b0-614">`az network private-link-resource`: Add support for the Microsoft.Batch batchAccount resource</span></span>
* <span data-ttu-id="3c5b0-615">`az network private-endpoint-connection`: adicionar suporte para o recurso Microsoft.Batch batchAccount</span><span class="sxs-lookup"><span data-stu-id="3c5b0-615">`az network private-endpoint-connection`: Add support for the Microsoft.Batch batchAccount resource</span></span>

### <a name="cdn"></a><span data-ttu-id="3c5b0-616">CDN</span><span class="sxs-lookup"><span data-stu-id="3c5b0-616">CDN</span></span>

* <span data-ttu-id="3c5b0-617">`az cdn custom-domain enable-https`: adicionar suporte para BYOC.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-617">`az cdn custom-domain enable-https`: Add BYOC support.</span></span>
* <span data-ttu-id="3c5b0-618">`az cdn custom-domain enable-https`: corrigir a habilitação de HTTPS personalizado com certificados gerenciados da CDN para os SKUs Standard_Verizon e Standard_Microsoft.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-618">`az cdn custom-domain enable-https`: Fix enabling custom HTTPS with CDN managed certificates for Standard_Verizon and Standard_Microsoft SKUs.</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="3c5b0-619">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-619">Cognitive Services</span></span>

* <span data-ttu-id="3c5b0-620">[ALTERAÇÃO DA FALHA] `az cognitiveservices account` agora, há uma estrutura unificada para todos os comandos.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-620">[BREAKING CHANGE] `az cognitiveservices account` now have a unified structure for all commands.</span></span>
* <span data-ttu-id="3c5b0-621">`az cognitiveservices account identity`: adicionar gerenciamento de identidades para os Serviços Cognitivos.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-621">`az cognitiveservices account identity`: Add identity management for Cognitive Services.</span></span>

### <a name="compute"></a><span data-ttu-id="3c5b0-622">Computação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-622">Compute</span></span>

* <span data-ttu-id="3c5b0-623">`az image builder`: atualização da versão da API para 2020-02-14</span><span class="sxs-lookup"><span data-stu-id="3c5b0-623">`az image builder`: Upgrade API version to 2020-02-14</span></span>
* <span data-ttu-id="3c5b0-624">`az image builder create`: adicionar `--identity` para dar suporte à configuração de identidade</span><span class="sxs-lookup"><span data-stu-id="3c5b0-624">`az image builder create`: Add `--identity` to support identity configuration</span></span>
* <span data-ttu-id="3c5b0-625">`az image builder customizer add`: suporte para o personalizador de atualização do Windows</span><span class="sxs-lookup"><span data-stu-id="3c5b0-625">`az image builder customizer add`: Support Windows update customizer</span></span>
* <span data-ttu-id="3c5b0-626">Novo comando `az image builder cancel`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-626">New command `az image builder cancel`</span></span>
* <span data-ttu-id="3c5b0-627">Mostrar um aviso quando um usuário implanta um VMSS fixado a uma versão de uma imagem específica em vez da mais recente</span><span class="sxs-lookup"><span data-stu-id="3c5b0-627">Show a warning when a user deploys a VMSS pinned to a specific image version rather than latest</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="3c5b0-628">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="3c5b0-628">Cosmos DB</span></span>

* <span data-ttu-id="3c5b0-629">`az cosmosdb`: adicionar o comando exists ao banco de dados e aos grupos de contêineres</span><span class="sxs-lookup"><span data-stu-id="3c5b0-629">`az cosmosdb`: Add exists command to database and container groups</span></span>
* <span data-ttu-id="3c5b0-630">Permitir a criação de coleções fixas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-630">Allow creating fixed collections</span></span>

### <a name="eventhub"></a><span data-ttu-id="3c5b0-631">EventHub</span><span class="sxs-lookup"><span data-stu-id="3c5b0-631">EventHub</span></span>

* <span data-ttu-id="3c5b0-632">`az eventhubs namespace create`: adicionar parâmetros de identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="3c5b0-632">`az eventhubs namespace create` : Add managed identity parameters</span></span>

### <a name="extension"></a><span data-ttu-id="3c5b0-633">Extensão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-633">Extension</span></span>

* <span data-ttu-id="3c5b0-634">Adicionar --version para dar suporte à instalação de uma versão específica</span><span class="sxs-lookup"><span data-stu-id="3c5b0-634">Add --version to support to install from a specific version</span></span>
* <span data-ttu-id="3c5b0-635">Habilitar as extensões da CLI a incluírem pacotes no namespace 'azure'</span><span class="sxs-lookup"><span data-stu-id="3c5b0-635">Enable CLI extensions to include packages in the 'azure' namespace</span></span>

### <a name="iot-hub"></a><span data-ttu-id="3c5b0-636">Hub IoT</span><span class="sxs-lookup"><span data-stu-id="3c5b0-636">Iot Hub</span></span>

* <span data-ttu-id="3c5b0-637">[ALTERAÇÃO SIGNIFICATIVA] az iot hub job: remover comandos de trabalho preteridos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-637">[BREAKING CHANGE] az iot hub job: Remove deprecated job commands</span></span>

### <a name="keyvault"></a><span data-ttu-id="3c5b0-638">KeyVault</span><span class="sxs-lookup"><span data-stu-id="3c5b0-638">KeyVault</span></span>

* <span data-ttu-id="3c5b0-639">`az keyvault key import`: dá suporte à importação de cadeias de caracteres por meio de dois novos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-639">`az keyvault key import`: Supports importing from strings via two new parameters.</span></span>
* <span data-ttu-id="3c5b0-640">Suporte à criptografia e descriptografia de cadeias de caracteres/bytes com chaves armazenadas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-640">Support string/bytes encryption and decryption with stored keys</span></span>

### <a name="monitor"></a><span data-ttu-id="3c5b0-641">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-641">Monitor</span></span>

* <span data-ttu-id="3c5b0-642">Suporte para não aguardar a criação do cluster</span><span class="sxs-lookup"><span data-stu-id="3c5b0-642">Support no wait for cluster creation</span></span>
* <span data-ttu-id="3c5b0-643">`az monitor log-analytics workspace saved-search`: suporte para novos comandos para a pesquisa salva</span><span class="sxs-lookup"><span data-stu-id="3c5b0-643">`az monitor log-analytics workspace saved-search`: Support new commands for saved search</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-644">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-644">Network</span></span>

* <span data-ttu-id="3c5b0-645">`az network application-gateway address-pool update`: refinar a mensagem de ajuda e adicionar exemplos.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-645">`az network application-gateway address-pool update`: Refine help message and add examples.</span></span>
* <span data-ttu-id="3c5b0-646">`az network vnet create`: suporte para o argumento --nsg</span><span class="sxs-lookup"><span data-stu-id="3c5b0-646">`az network vnet create`: Support --nsg argument</span></span>
* <span data-ttu-id="3c5b0-647">`az network lb address-pool`: suporte para criar o pool de back-end de lb com endereço de back-end.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-647">`az network lb address-pool`: Support create lb backend pool with backend address.</span></span>
* <span data-ttu-id="3c5b0-648">`az network application-gateway address-pool`: correção para o argumento --add</span><span class="sxs-lookup"><span data-stu-id="3c5b0-648">`az network application-gateway address-pool`: Fix for --add argument</span></span>

### <a name="rbac"></a><span data-ttu-id="3c5b0-649">RBAC</span><span class="sxs-lookup"><span data-stu-id="3c5b0-649">RBAC</span></span>

* <span data-ttu-id="3c5b0-650">`az ad sp create-for-rabc`: suporte para nome com espaço, barra e barra invertida</span><span class="sxs-lookup"><span data-stu-id="3c5b0-650">`az ad sp create-for-rabc`: Support name with space, slash and back slash</span></span>
* <span data-ttu-id="3c5b0-651">`az ad sp create-for-rbac`: refinar mensagem de erro quando o usuário especifica um escopo inválido</span><span class="sxs-lookup"><span data-stu-id="3c5b0-651">`az ad sp create-for-rbac`: Refine error message when user specify an invalid scope</span></span>

### <a name="security"></a><span data-ttu-id="3c5b0-652">Segurança</span><span class="sxs-lookup"><span data-stu-id="3c5b0-652">Security</span></span>

* <span data-ttu-id="3c5b0-653">Adicionar comandos de avaliação de segurança</span><span class="sxs-lookup"><span data-stu-id="3c5b0-653">Add security assessment commands</span></span>

### <a name="sql"></a><span data-ttu-id="3c5b0-654">SQL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-654">SQL</span></span>

* <span data-ttu-id="3c5b0-655">`az sql db ltr-policy/ltr-backup`: atualizar/mostrar política de retenção de longo prazo, mostrar/excluir backups de retenção de longo prazo, restaurar backup de retenção de longo prazo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-655">`az sql db ltr-policy/ltr-backup`: update/show long term retention policy, show/delete long term retention backups, restore long term retention backup</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-656">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-656">Storage</span></span>

* <span data-ttu-id="3c5b0-657">Corrigir problema de autenticação para dar suporte a get token para --subscription</span><span class="sxs-lookup"><span data-stu-id="3c5b0-657">Fix authentication issue to support get token for --subscription</span></span>
* <span data-ttu-id="3c5b0-658">`az storage remove`: correção do problema #13459 para gerar exceção para a falha da operação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-658">`az storage remove`: Fix issue #13459 to raise exception for operation failure</span></span>
* <span data-ttu-id="3c5b0-659">Correção dos problemas #13012, #13632 e #13657 para remover argumentos não utilizados para comandos relacionados à geração de SAS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-659">Fix issues #13012, #13632 and #13657 to remove unused arguments for generate-sas related commands</span></span>
* <span data-ttu-id="3c5b0-660">`az storage logging update`: adicionar verificação da versão de log</span><span class="sxs-lookup"><span data-stu-id="3c5b0-660">`az storage logging update`: Add check for logging version</span></span>
* <span data-ttu-id="3c5b0-661">`az storage blob show`: adicionar mais propriedades para o blob com o SDK da faixa 2</span><span class="sxs-lookup"><span data-stu-id="3c5b0-661">`az storage blob show`: Add more properties for blob with track 2 SDK</span></span>
* <span data-ttu-id="3c5b0-662">Correção #13708: refinar a mensagem de aviso para a credencial</span><span class="sxs-lookup"><span data-stu-id="3c5b0-662">Fix #13708: Refine warning message for credential</span></span>
* <span data-ttu-id="3c5b0-663">`az storage share-rm create/update`: adicionar suporte para protocolo NFS e squash raiz</span><span class="sxs-lookup"><span data-stu-id="3c5b0-663">`az storage share-rm create/update`: Add NFS protocol and root squash support</span></span>
* <span data-ttu-id="3c5b0-664">`az storage account create`: adicionar suporte para criptografia dupla</span><span class="sxs-lookup"><span data-stu-id="3c5b0-664">`az storage account create`: Add support for double encryption</span></span>
* <span data-ttu-id="3c5b0-665">[ALTERAÇÃO DA FALHA] `az storage blob/container/file/share/table/queue generate-sas`: tornar --expiry e --permissions obrigatórios</span><span class="sxs-lookup"><span data-stu-id="3c5b0-665">[BREAKING CHANGE] `az storage blob/container/file/share/table/queue generate-sas`: make --expiry and --permissions required</span></span>
* <span data-ttu-id="3c5b0-666">`az storage blob set-tier`: migrar para a Faixa 2 para dar suporte à definição da prioridade de reidratação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-666">`az storage blob set-tier`: Migrate to Track 2 to support setting rehydrate priority</span></span>

## <a name="june-02-2020"></a><span data-ttu-id="3c5b0-667">02 de Junho de 2020</span><span class="sxs-lookup"><span data-stu-id="3c5b0-667">June 02, 2020</span></span>

<span data-ttu-id="3c5b0-668">Versão 2.7.0</span><span class="sxs-lookup"><span data-stu-id="3c5b0-668">Version 2.7.0</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-669">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-669">ACR</span></span>

* <span data-ttu-id="3c5b0-670">Correção de um erro de digitação em uma mensagem de erro de criação de token</span><span class="sxs-lookup"><span data-stu-id="3c5b0-670">Fix a typo in an error message of token creation</span></span>

### <a name="aks"></a><span data-ttu-id="3c5b0-671">AKS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-671">AKS</span></span>

* <span data-ttu-id="3c5b0-672">Alteração da sku de vm padrão para Standard_D2s_v3</span><span class="sxs-lookup"><span data-stu-id="3c5b0-672">Change default vm sku to Standard_D2s_v3</span></span>
* <span data-ttu-id="3c5b0-673">Correção da criação de atribuição de função para sub-rede personalizada MSI cluster Plus</span><span class="sxs-lookup"><span data-stu-id="3c5b0-673">Fix creating role assignment for MSI clsuter plus custom subnet</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-674">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-674">AppService</span></span>

* <span data-ttu-id="3c5b0-675">A correção #12739 az appservice list-locations retorna alguns locais inválidos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-675">Fix #12739 az appservice list-locations returns some invalid locations</span></span>

### <a name="arm"></a><span data-ttu-id="3c5b0-676">ARM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-676">ARM</span></span>

* <span data-ttu-id="3c5b0-677">`az deployment`: Correção do problema #13159 de mensagem incorreta do JSON após a remoção de comentários e a compactação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-677">`az deployment`: Fix issue #13159 of incorrect message of JSON after removing comments and compressing</span></span>
* <span data-ttu-id="3c5b0-678">`az resource tag`: Correção do problema #13255 de marcação de recursos com o tipo de recurso `Microsoft.ContainerRegistry/registries/webhooks`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-678">`az resource tag`: Fix issue #13255 of tagging resources with resource type `Microsoft.ContainerRegistry/registries/webhooks`</span></span>
* <span data-ttu-id="3c5b0-679">Melhoria dos exemplos do módulo de recursos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-679">Improve the examples for the resource module</span></span>

### <a name="aro"></a><span data-ttu-id="3c5b0-680">ARO</span><span class="sxs-lookup"><span data-stu-id="3c5b0-680">ARO</span></span>

* <span data-ttu-id="3c5b0-681">Alteração do CLIError para corrigir o sinalizador para --worker-vm-disk-size-gb</span><span class="sxs-lookup"><span data-stu-id="3c5b0-681">Change CLIError to correct flag for --worker-vm-disk-size-gb</span></span>

### <a name="eventhub"></a><span data-ttu-id="3c5b0-682">EventHub</span><span class="sxs-lookup"><span data-stu-id="3c5b0-682">EventHub</span></span>

* <span data-ttu-id="3c5b0-683">Correção do problema #12406 Argumento --capture-interval não atualiza o "intervalInSeconds"</span><span class="sxs-lookup"><span data-stu-id="3c5b0-683">Fix for issue #12406 Argument --capture-interval does not update the "intervalInSeconds"</span></span>

### <a name="hdinsight"></a><span data-ttu-id="3c5b0-684">HDInsight</span><span class="sxs-lookup"><span data-stu-id="3c5b0-684">HDInsight</span></span>

* <span data-ttu-id="3c5b0-685">Alteração de get_json_object para shell_safe_json_parse</span><span class="sxs-lookup"><span data-stu-id="3c5b0-685">Change get_json_object to shell_safe_json_parse</span></span>

### <a name="monitor"></a><span data-ttu-id="3c5b0-686">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-686">Monitor</span></span>

* <span data-ttu-id="3c5b0-687">`az monitor metrics alert`: ajuste de várias mensagens de ajuda</span><span class="sxs-lookup"><span data-stu-id="3c5b0-687">`az monitor metrics alert`: refine several help messages</span></span>
* <span data-ttu-id="3c5b0-688">`az monitor diagnostic-settings create`: suporte ao argumento --export-to-resource-specific</span><span class="sxs-lookup"><span data-stu-id="3c5b0-688">`az monitor diagnostic-settings create`: support --export-to-resource-specific argument</span></span>
* <span data-ttu-id="3c5b0-689">Suporte para recuperar o workspace de LA</span><span class="sxs-lookup"><span data-stu-id="3c5b0-689">Support LA workspace recover</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-690">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-690">Network</span></span>

* <span data-ttu-id="3c5b0-691">`az network dns zone`: suporte – caractere</span><span class="sxs-lookup"><span data-stu-id="3c5b0-691">`az network dns zone`: support - character</span></span>
* <span data-ttu-id="3c5b0-692">`az network vpn-connection ipsec-policy`: alteração do --sa-lifetime e do --sa-max-size para valores maiores no exemplo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-692">`az network vpn-connection ipsec-policy`: change the --sa-lifetime and --sa-max-size to larger values in example</span></span>
* <span data-ttu-id="3c5b0-693">Aumento da rede para 2020-04-01</span><span class="sxs-lookup"><span data-stu-id="3c5b0-693">Bump network to 2020-04-01</span></span>
* <span data-ttu-id="3c5b0-694">`az network private-endpoint-connection`: suporte à grade de eventos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-694">`az network private-endpoint-connection`: support event grid</span></span>
* <span data-ttu-id="3c5b0-695">`az network express-route list-route-tables`: correção do bug que faz não ser possível listar rotas como tabela</span><span class="sxs-lookup"><span data-stu-id="3c5b0-695">`az network express-route list-route-tables`: fix bug that cannot list routes as table</span></span>

### <a name="packaging"></a><span data-ttu-id="3c5b0-696">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-696">Packaging</span></span>

* <span data-ttu-id="3c5b0-697">Adição do Pacote Focal do Ubuntu</span><span class="sxs-lookup"><span data-stu-id="3c5b0-697">Add Ubuntu Focal Package</span></span>

### <a name="rbac"></a><span data-ttu-id="3c5b0-698">RBAC</span><span class="sxs-lookup"><span data-stu-id="3c5b0-698">RBAC</span></span>

* <span data-ttu-id="3c5b0-699">`az ad sp credential reset`: modificar a geração de credenciais para evitar caracteres especiais problemáticos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-699">`az ad sp credential reset`: modify credential generation to avoid troublesome special characters</span></span>

### <a name="redis"></a><span data-ttu-id="3c5b0-700">Redis</span><span class="sxs-lookup"><span data-stu-id="3c5b0-700">Redis</span></span>

* <span data-ttu-id="3c5b0-701">Correção #13529: alteração da documentação do parâmetro enable_non_ssl_port</span><span class="sxs-lookup"><span data-stu-id="3c5b0-701">Fix #13529: Change documentation of parameter enable_non_ssl_port</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-702">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-702">Storage</span></span>

* <span data-ttu-id="3c5b0-703">`az storage copy`: adição do parâmetro `--follow-symlinks` para dar suporte ao symlinks</span><span class="sxs-lookup"><span data-stu-id="3c5b0-703">`az storage copy`: Add parameter `--follow-symlinks` to support symlinks</span></span>
* <span data-ttu-id="3c5b0-704">Habilitar contexto local para a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-704">Enable local context for storage account</span></span>
* <span data-ttu-id="3c5b0-705">`az storage logging`: Correção do problema #11969 para ajustar a mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="3c5b0-705">`az storage logging`: Fix issue #11969 to refine error message</span></span>

## <a name="may-19-2020"></a><span data-ttu-id="3c5b0-706">19 de maio de 2020</span><span class="sxs-lookup"><span data-stu-id="3c5b0-706">May 19, 2020</span></span>

<span data-ttu-id="3c5b0-707">Versão 2.6.0</span><span class="sxs-lookup"><span data-stu-id="3c5b0-707">Version 2.6.0</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-708">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-708">ACR</span></span>

* <span data-ttu-id="3c5b0-709">Adiciona tempo limite padrão de 5 minutos para solicitações ao ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-709">Add default timeout of 5 minutes for any requests to ACR</span></span>
* <span data-ttu-id="3c5b0-710">Suporte para desabilitar o acesso à redes públicas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-710">Support disable public network access</span></span>
* <span data-ttu-id="3c5b0-711">`az acr token create`: expõe o argumento --days</span><span class="sxs-lookup"><span data-stu-id="3c5b0-711">`az acr token create`: expose --days argument</span></span>
* <span data-ttu-id="3c5b0-712">`az acr import`: aceita valores do argumento --source que contêm logon no nome do servidor por meio da correção final do cliente</span><span class="sxs-lookup"><span data-stu-id="3c5b0-712">`az acr import`: accept --source argument values which contain login in server name through client end correction</span></span>

### <a name="acs"></a><span data-ttu-id="3c5b0-713">ACS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-713">ACS</span></span>

* <span data-ttu-id="3c5b0-714">Correção de bug: remover limpeza de campos para campos que não existem mais</span><span class="sxs-lookup"><span data-stu-id="3c5b0-714">Bug fix: remove fields cleanup for fields that no longer exist</span></span>

### <a name="aks"></a><span data-ttu-id="3c5b0-715">AKS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-715">AKS</span></span>

* <span data-ttu-id="3c5b0-716">Atualiza o tempo de atividade do contexto de ajuda de comando do SLA</span><span class="sxs-lookup"><span data-stu-id="3c5b0-716">Update uptime-sla command help context</span></span>
* <span data-ttu-id="3c5b0-717">Remove a verificação do intervalo para a atualização da contagem de minutos do dimensionador automático</span><span class="sxs-lookup"><span data-stu-id="3c5b0-717">Remove range check for updating min count for autoscaler</span></span>
* <span data-ttu-id="3c5b0-718">Corrige o problema que fazia com que a CLI falhasse quando o usuário especificava apenas a senha do Windows</span><span class="sxs-lookup"><span data-stu-id="3c5b0-718">Fix that cli doe not fail when user only specifies Windows password</span></span>

### <a name="ams"></a><span data-ttu-id="3c5b0-719">AMS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-719">AMS</span></span>

* <span data-ttu-id="3c5b0-720">`az ams transform create`: Adiciona a capacidade de criar uma transformação com um FaceDetector predefinido</span><span class="sxs-lookup"><span data-stu-id="3c5b0-720">`az ams transform create`: Add ability to create a transform with a FaceDetector preset</span></span>
* <span data-ttu-id="3c5b0-721">`az ams content-key-policy create`: Adiciona a capacidade de criar uma política de chave de conteúdo do FairPlay com uma configuração de aluguel offline</span><span class="sxs-lookup"><span data-stu-id="3c5b0-721">`az ams content-key-policy create` : Add ability to create a FairPlay content key policy with an offline rental configuration</span></span>

### <a name="appconfig"></a><span data-ttu-id="3c5b0-722">AppConfig</span><span class="sxs-lookup"><span data-stu-id="3c5b0-722">AppConfig</span></span>

* <span data-ttu-id="3c5b0-723">Correção de bug para valores de chave da lista com campos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-723">Bug fix for list key values with fields</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-724">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-724">AppService</span></span>

* <span data-ttu-id="3c5b0-725">`az functionapp create`: AzureWebJobsDashboard será definido somente se AppInsights estiver desabilitado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-725">`az functionapp create`: AzureWebJobsDashboard will only be set if AppInsights is disabled</span></span>
* <span data-ttu-id="3c5b0-726">Correção #10664 – Integração VNet – Problema de Verificação de Localização e Correção #13257-AZ Web App falha quando o RG precisar ser criado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-726">Fix #10664- VNet Integration - Location Check Issue & fix #13257- az webapp up failing when RG needs to be created</span></span>
* <span data-ttu-id="3c5b0-727">`az webapp|functionapp config ssl import`: Pesquisa o cofre de chaves em grupos de recursos na assinatura e aprimora a ajuda e os exemplos.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-727">`az webapp|functionapp config ssl import`: Lookup key vault across resources groups in subscription and improve help and examples.</span></span>
* <span data-ttu-id="3c5b0-728">Integra o contexto local para o serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-728">Onboard local context for app service</span></span>

### <a name="arm"></a><span data-ttu-id="3c5b0-729">ARM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-729">ARM</span></span>

* <span data-ttu-id="3c5b0-730">`az deployment`: Corrige o problema que faz com que o templateLink não seja retornado ao implantar ou validar o template-uri</span><span class="sxs-lookup"><span data-stu-id="3c5b0-730">`az deployment`: Fix the problem that the templateLink will not be returned when deploying or validating template-uri</span></span>
* <span data-ttu-id="3c5b0-731">`az deployment`: Corrige o problema que faz com que implantação/validação não dê suporte ao caractere codificado especialmente</span><span class="sxs-lookup"><span data-stu-id="3c5b0-731">`az deployment`: Fix the problem that deployment/validate does not support specially encoded character</span></span>
* <span data-ttu-id="3c5b0-732">`az deployment sub/group what-if`: Corrige o alinhamento de matriz e o tratamento de erro</span><span class="sxs-lookup"><span data-stu-id="3c5b0-732">`az deployment sub/group what-if`: Fix array alignment and error handling</span></span>
* <span data-ttu-id="3c5b0-733">`az deployment operation`: Modifica as informações preteridas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-733">`az deployment operation`: Modify the deprecate information</span></span>

### <a name="aro"></a><span data-ttu-id="3c5b0-734">ARO</span><span class="sxs-lookup"><span data-stu-id="3c5b0-734">ARO</span></span>

* <span data-ttu-id="3c5b0-735">Adiciona exemplos para az aro create, list, list-credentials, show, delete</span><span class="sxs-lookup"><span data-stu-id="3c5b0-735">Add examples to az aro create, list, list-credentials, show, delete</span></span>
* <span data-ttu-id="3c5b0-736">Adiciona a função generate_random_id</span><span class="sxs-lookup"><span data-stu-id="3c5b0-736">Add generate_random_id function</span></span>

### <a name="backup"></a><span data-ttu-id="3c5b0-737">Backup</span><span class="sxs-lookup"><span data-stu-id="3c5b0-737">Backup</span></span>

* <span data-ttu-id="3c5b0-738">Permite FriendlyName ao habilitar proteção para o comando AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="3c5b0-738">Allow FriendlyName in enable protection for AzureFileShare command</span></span>
* <span data-ttu-id="3c5b0-739">Correção do comando restore-disks da IaasVM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-739">Fix in IaasVM restore-disks Command</span></span>
* <span data-ttu-id="3c5b0-740">Adiciona o BackupManagementType "MAB" ao comando item list</span><span class="sxs-lookup"><span data-stu-id="3c5b0-740">Add "MAB" BackupManagementType to item list command</span></span>
* <span data-ttu-id="3c5b0-741">Adiciona suporte para a repetição de tentativas de atualização da política para itens com falha.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-741">Add support for retrying policy update for failed items.</span></span>
* <span data-ttu-id="3c5b0-742">Adiciona a funcionalidade de Retomada de Proteção para as Máquinas Virtuais do Azure</span><span class="sxs-lookup"><span data-stu-id="3c5b0-742">Add Resume Protection functionality for Azure Virtual Machine</span></span>
* <span data-ttu-id="3c5b0-743">Adiciona suporte para especificar o ResourceGroup para armazenar instantRP durante a Criação ou Modificação de Política</span><span class="sxs-lookup"><span data-stu-id="3c5b0-743">Add support to specify ResourceGroup for storing instantRP during Create or Modify Policy</span></span>

### <a name="ci"></a><span data-ttu-id="3c5b0-744">CI</span><span class="sxs-lookup"><span data-stu-id="3c5b0-744">CI</span></span>

* <span data-ttu-id="3c5b0-745">Suporte para flake8 3.8.0</span><span class="sxs-lookup"><span data-stu-id="3c5b0-745">Support flake8 3.8.0</span></span>

### <a name="compute"></a><span data-ttu-id="3c5b0-746">Computação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-746">Compute</span></span>

* <span data-ttu-id="3c5b0-747">Novo comando az vm auto-shutdown</span><span class="sxs-lookup"><span data-stu-id="3c5b0-747">New command az vm auto-shutdown</span></span>
* <span data-ttu-id="3c5b0-748">`az vm list-skus`: Atualização do comportamento --zone, retorna SKUs de todos os tipos agora</span><span class="sxs-lookup"><span data-stu-id="3c5b0-748">`az vm list-skus`: Update --zone behavior, return all type skus now</span></span>

### <a name="core"></a><span data-ttu-id="3c5b0-749">Núcleo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-749">Core</span></span>

* <span data-ttu-id="3c5b0-750">Atualiza o status de ativado/desativado do contexto local para o nível de usuário global</span><span class="sxs-lookup"><span data-stu-id="3c5b0-750">Update local context on/off status to global user level</span></span>

### <a name="extension"></a><span data-ttu-id="3c5b0-751">Extensão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-751">Extension</span></span>

* <span data-ttu-id="3c5b0-752">`az extension add`: Adiciona --system para habilitar a instalação de extensões em um caminho do sistema</span><span class="sxs-lookup"><span data-stu-id="3c5b0-752">`az extension add`: Add --system to enable installing extensions in a system path</span></span>
* <span data-ttu-id="3c5b0-753">Suporte para .egg-info para armazenar metadados de extensão de tipo de roda</span><span class="sxs-lookup"><span data-stu-id="3c5b0-753">Support .egg-info to store wheel type extension metadata</span></span>

### <a name="iot"></a><span data-ttu-id="3c5b0-754">IoT</span><span class="sxs-lookup"><span data-stu-id="3c5b0-754">IoT</span></span>

* <span data-ttu-id="3c5b0-755">`az iot`: Atualiza a mensagem de reconhecimento de extensão da primeira execução do módulo de comando IoT para a ID precisa e moderna não preterida `azure-iot`.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-755">`az iot`: Update the IoT command module first run extension awareness message to the accurate, non-deprecated modern Id `azure-iot`.</span></span>

### <a name="iot-hub"></a><span data-ttu-id="3c5b0-756">Hub IoT</span><span class="sxs-lookup"><span data-stu-id="3c5b0-756">IoT Hub</span></span>

* <span data-ttu-id="3c5b0-757">Suporte para comandos de isolamento de rede e API 2020-03-01</span><span class="sxs-lookup"><span data-stu-id="3c5b0-757">Support for 2020-03-01 API and Network Isolation commands</span></span>

### <a name="netappfiles"></a><span data-ttu-id="3c5b0-758">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="3c5b0-758">NetAppFiles</span></span>

* <span data-ttu-id="3c5b0-759">`az volume create`: Adiciona snapshot-id como um parâmetro para criar volume – isso permitirá que os usuários criem um volume por meio de um instantâneo existente.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-759">`az volume create`: Adds snapshot-id as a parameter to create volume this will allow users to create a volume from existing snapshot.</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-760">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-760">Network</span></span>

* <span data-ttu-id="3c5b0-761">Corrige o valor TTL alterado não destinado ao DNS add-record</span><span class="sxs-lookup"><span data-stu-id="3c5b0-761">Fix ttl value changed unintended for dns add-record</span></span>
* <span data-ttu-id="3c5b0-762">`az network public-ip create`: Informa os clientes sobre futuras alterações da falha</span><span class="sxs-lookup"><span data-stu-id="3c5b0-762">`az network public-ip create`: Inform customers of a coming breaking change</span></span>
* <span data-ttu-id="3c5b0-763">Suporte para comandos genéricos para cenários de link privado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-763">Support generic commands for private link scenario</span></span>
* <span data-ttu-id="3c5b0-764">`az network private-endpoint-connection`: suporte a tipos mysql, postgres e mariadb</span><span class="sxs-lookup"><span data-stu-id="3c5b0-764">`az network private-endpoint-connection`: Support mysql, postgres and mariadb types</span></span>
* <span data-ttu-id="3c5b0-765">`az network private-endpoint-connection`: Suporte para tipos cosmosdb</span><span class="sxs-lookup"><span data-stu-id="3c5b0-765">`az network private-endpoint-connection`: Support cosmosdb types</span></span>
* <span data-ttu-id="3c5b0-766">`az network private-endpoint`: pretere --group-ids e redireciona para --group-id</span><span class="sxs-lookup"><span data-stu-id="3c5b0-766">`az network private-endpoint`: deprecate --group-ids and redirect to --group-id</span></span>

### <a name="output"></a><span data-ttu-id="3c5b0-767">Saída</span><span class="sxs-lookup"><span data-stu-id="3c5b0-767">Output</span></span>

* <span data-ttu-id="3c5b0-768">Mostra instruções de atualização em localizar, comentários e --help</span><span class="sxs-lookup"><span data-stu-id="3c5b0-768">Show update instruction in find, feedback and --help</span></span>

### <a name="packaging"></a><span data-ttu-id="3c5b0-769">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-769">Packaging</span></span>

* <span data-ttu-id="3c5b0-770">Cria pacotes MSI/Homebrew com dependências resolvidas de requirements.txt</span><span class="sxs-lookup"><span data-stu-id="3c5b0-770">Build MSI/Homebrew packages with dependecies resolved from requirements.txt</span></span>

### <a name="rbac"></a><span data-ttu-id="3c5b0-771">RBAC</span><span class="sxs-lookup"><span data-stu-id="3c5b0-771">RBAC</span></span>

* <span data-ttu-id="3c5b0-772">`az ad sp credential reset`: corrige a geração de credenciais fracas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-772">`az ad sp credential reset`: fix weak credential generation</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-773">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-773">Storage</span></span>

* <span data-ttu-id="3c5b0-774">`az storage account file-service-properties update/show`: Adiciona suporte a propriedades de arquivo para a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-774">`az storage account file-service-properties update/show`: Add File Properties Support for Storage Account</span></span>
* <span data-ttu-id="3c5b0-775">`az storage container create`: Correção #13373 ao adicionar o validador para acesso público</span><span class="sxs-lookup"><span data-stu-id="3c5b0-775">`az storage container create`: Fix #13373 by adding validator for public access</span></span>
* <span data-ttu-id="3c5b0-776">Adiciona suporte a ADLS Gen2 track2</span><span class="sxs-lookup"><span data-stu-id="3c5b0-776">Add ADLS Gen2 track2 support</span></span>
* <span data-ttu-id="3c5b0-777">`az storage blob sync`: Dar suporte à `--connection-string`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-777">`az storage blob sync`: Support `--connection-string`</span></span>
* <span data-ttu-id="3c5b0-778">`az storage blob sync`: Corrige a mensagem de erro incorreta quando azcopy não consegue encontrar o local de instalação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-778">`az storage blob sync`: Fix the incorrect error message when azcopy cannot find the installation location</span></span>

## <a name="april-30-2020"></a><span data-ttu-id="3c5b0-779">30 de abril de 2020</span><span class="sxs-lookup"><span data-stu-id="3c5b0-779">April 30, 2020</span></span>

<span data-ttu-id="3c5b0-780">Versão 2.5.1</span><span class="sxs-lookup"><span data-stu-id="3c5b0-780">Version 2.5.1</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-781">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-781">ACR</span></span>

* <span data-ttu-id="3c5b0-782">`az acr check-health`: correção de "DOCKER_PULL_ERROR" no Windows</span><span class="sxs-lookup"><span data-stu-id="3c5b0-782">`az acr check-health`: Fix "DOCKER_PULL_ERROR" on Windows</span></span>

### <a name="compute"></a><span data-ttu-id="3c5b0-783">Computação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-783">Compute</span></span>

* <span data-ttu-id="3c5b0-784">`az vm list-ip-addresses`: Tratamento de erros</span><span class="sxs-lookup"><span data-stu-id="3c5b0-784">`az vm list-ip-addresses`: Error handling</span></span>
* <span data-ttu-id="3c5b0-785">Correção de um bug de criação de VM caso endpoint_vm_image_alias_doc não estivesse definido no perfil de nuvem</span><span class="sxs-lookup"><span data-stu-id="3c5b0-785">Fix a bug of vm create if endpoint_vm_image_alias_doc is not set in cloud profile</span></span>
* <span data-ttu-id="3c5b0-786">`az vmss create`: adição de --os-disk-size-gb</span><span class="sxs-lookup"><span data-stu-id="3c5b0-786">`az vmss create`: Add --os-disk-size-gb</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="3c5b0-787">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="3c5b0-787">Cosmos DB</span></span>

* <span data-ttu-id="3c5b0-788">`az cosmosdb create/update`: adição de suporte a --enable-public-network</span><span class="sxs-lookup"><span data-stu-id="3c5b0-788">`az cosmosdb create/update`: add --enable-public-network support</span></span>

### <a name="extension"></a><span data-ttu-id="3c5b0-789">Extensão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-789">Extension</span></span>

* <span data-ttu-id="3c5b0-790">Correção do carregamento de metadados errados para a extensão de tipo roda</span><span class="sxs-lookup"><span data-stu-id="3c5b0-790">Fix loading wrong metadata for wheel type extension</span></span>

### <a name="packaging"></a><span data-ttu-id="3c5b0-791">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-791">Packaging</span></span>

* <span data-ttu-id="3c5b0-792">Adição de script az para Git Bash/Cygwin no Windows</span><span class="sxs-lookup"><span data-stu-id="3c5b0-792">Add az script for Git Bash/Cygwin on Windows</span></span>

### <a name="sql"></a><span data-ttu-id="3c5b0-793">SQL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-793">SQL</span></span>

* <span data-ttu-id="3c5b0-794">`az sql instance-pool`: adição de grupo de comando de pools de instância</span><span class="sxs-lookup"><span data-stu-id="3c5b0-794">`az sql instance-pool`: Add instance pools command group</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-795">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-795">Storage</span></span>

* <span data-ttu-id="3c5b0-796">Atualização do pacote azure-multiapi-storage para 0.3.0</span><span class="sxs-lookup"><span data-stu-id="3c5b0-796">Upgrade package azure-multiapi-storage to 0.3.0</span></span>
* <span data-ttu-id="3c5b0-797">Dá suporte ao GZRS para a criação e atualização da conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-797">Support GZRS for storage account creation and update</span></span>
* <span data-ttu-id="3c5b0-798">`az storage account failover`: adição de suporte para failover da conta de armazenamento de GRS/GZRS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-798">`az storage account failover`: Add support for grs/gzrs storage account failover</span></span>
* <span data-ttu-id="3c5b0-799">`az storage blob upload`: adição do parâmetro --encryption-scope para dar suporte à especificação da informação do escopo da criptografia</span><span class="sxs-lookup"><span data-stu-id="3c5b0-799">`az storage blob upload`: Add --encryption-scope parameter to support specifying encryption scope information</span></span>

## <a name="april-28-2020"></a><span data-ttu-id="3c5b0-800">28 de abril de 2020</span><span class="sxs-lookup"><span data-stu-id="3c5b0-800">April 28, 2020</span></span>

<span data-ttu-id="3c5b0-801">Versão 2.5.0</span><span class="sxs-lookup"><span data-stu-id="3c5b0-801">Version 2.5.0</span></span>

### <a name="acs"></a><span data-ttu-id="3c5b0-802">ACS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-802">ACS</span></span>

* <span data-ttu-id="3c5b0-803">[ALTERAÇÃO SIGNIFICATIVA] az openshift create: remove o parâmetro --vnet-peer.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-803">[BREAKING CHANGE] az openshift create: remove --vnet-peer parameter.</span></span>
* <span data-ttu-id="3c5b0-804">`az openshift create`: adição de sinalizadores para dar suporte a clusters privados.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-804">`az openshift create`: add flags to support private cluster.</span></span>
* <span data-ttu-id="3c5b0-805">`az openshift`: atualização para a versão `2019-10-27-preview` da API.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-805">`az openshift`: upgrade to `2019-10-27-preview` API version.</span></span>
* <span data-ttu-id="3c5b0-806">`az openshift`: adição do comando `update`.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-806">`az openshift`: add `update` command.</span></span>

### <a name="aks"></a><span data-ttu-id="3c5b0-807">AKS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-807">AKS</span></span>

* <span data-ttu-id="3c5b0-808">`az aks create`: adição do suporte para Windows</span><span class="sxs-lookup"><span data-stu-id="3c5b0-808">`az aks create`: Add support for Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-809">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-809">AppService</span></span>

* <span data-ttu-id="3c5b0-810">`az webapp deployment source config-zip`: remoção da suspensão após request.get()</span><span class="sxs-lookup"><span data-stu-id="3c5b0-810">`az webapp deployment source config-zip`: remove sleep after request.get()</span></span>

### <a name="arm"></a><span data-ttu-id="3c5b0-811">ARM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-811">ARM</span></span>

* <span data-ttu-id="3c5b0-812">Adição de comandos What-If de implantação de modelo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-812">Add template deployment What-If commands</span></span>

### <a name="aro"></a><span data-ttu-id="3c5b0-813">ARO</span><span class="sxs-lookup"><span data-stu-id="3c5b0-813">ARO</span></span>

* <span data-ttu-id="3c5b0-814">`az aro`: correção da saída da tabela</span><span class="sxs-lookup"><span data-stu-id="3c5b0-814">`az aro`: Fix table output</span></span>

### <a name="ci"></a><span data-ttu-id="3c5b0-815">CI</span><span class="sxs-lookup"><span data-stu-id="3c5b0-815">CI</span></span>

* <span data-ttu-id="3c5b0-816">Integração do pytest e preterição do nose para o teste de automação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-816">Onboard pytest and deprecate nose for Automation Test</span></span>

### <a name="compute"></a><span data-ttu-id="3c5b0-817">Computação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-817">Compute</span></span>

* <span data-ttu-id="3c5b0-818">`az vmss disk detach`: correção do problema de NoneType do disco de dados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-818">`az vmss disk detach`: fix data disk NoneType issue</span></span>
* <span data-ttu-id="3c5b0-819">`az vm availability-set list`: suporte à exibição da lista de VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-819">`az vm availability-set list`: Support showing VM list</span></span>
* <span data-ttu-id="3c5b0-820">`az vm list-skus`: correção do problema de exibição do formato de tabela</span><span class="sxs-lookup"><span data-stu-id="3c5b0-820">`az vm list-skus`: Fix display problem of table format</span></span>

### <a name="keyvault"></a><span data-ttu-id="3c5b0-821">KeyVault</span><span class="sxs-lookup"><span data-stu-id="3c5b0-821">KeyVault</span></span>

* <span data-ttu-id="3c5b0-822">Adição de novo parâmetro `--enable-rbac-authorization` durante a criação ou atualização</span><span class="sxs-lookup"><span data-stu-id="3c5b0-822">Add new parameter `--enable-rbac-authorization` during creating or updating</span></span>

### <a name="monitor"></a><span data-ttu-id="3c5b0-823">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-823">Monitor</span></span>

* <span data-ttu-id="3c5b0-824">Suporte aos recursos de CMK do cluster de LA</span><span class="sxs-lookup"><span data-stu-id="3c5b0-824">Support LA cluster CMK features</span></span>
* <span data-ttu-id="3c5b0-825">`az monitor log-analytics workspace linked-storage`: dá suporte aos recursos BYOS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-825">`az monitor log-analytics workspace linked-storage`: supports BYOS features</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-826">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-826">Network</span></span>

* <span data-ttu-id="3c5b0-827">`az network security-partner`: suporte para provedor de segurança de parceiros</span><span class="sxs-lookup"><span data-stu-id="3c5b0-827">`az network security-partner`: support security partner provider</span></span>

### <a name="privatedns"></a><span data-ttu-id="3c5b0-828">Privatedns</span><span class="sxs-lookup"><span data-stu-id="3c5b0-828">Privatedns</span></span>

* <span data-ttu-id="3c5b0-829">Adição do recurso na zona DNS privada para importar o arquivo da zona de exportação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-829">Add feature in private DNS zone to import export zone file</span></span>

## <a name="april-21-2020"></a><span data-ttu-id="3c5b0-830">21 de abril de 2020</span><span class="sxs-lookup"><span data-stu-id="3c5b0-830">April 21, 2020</span></span>

<span data-ttu-id="3c5b0-831">Versão 2.4.0</span><span class="sxs-lookup"><span data-stu-id="3c5b0-831">Version 2.4.0</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-832">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-832">ACR</span></span>

* <span data-ttu-id="3c5b0-833">`az acr run --cmd`: desabilitar a substituição do diretório de trabalho</span><span class="sxs-lookup"><span data-stu-id="3c5b0-833">`az acr run --cmd`: disable working directory override</span></span>
* <span data-ttu-id="3c5b0-834">Suporte ao ponto de extremidade dos dados dedicados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-834">Support dedicated data endpoint</span></span>

### <a name="aks"></a><span data-ttu-id="3c5b0-835">AKS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-835">AKS</span></span>

* <span data-ttu-id="3c5b0-836">`az aks list -o table` deve mostrar privateFqdn como fqdn para clusters privados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-836">`az aks list -o table` should show privateFqdn as fqdn for private clusters</span></span>
* <span data-ttu-id="3c5b0-837">Adicionar --uptime-sla</span><span class="sxs-lookup"><span data-stu-id="3c5b0-837">Add --uptime-sla</span></span>
* <span data-ttu-id="3c5b0-838">Atualizar pacote containerservice</span><span class="sxs-lookup"><span data-stu-id="3c5b0-838">Update containerservice package</span></span>
* <span data-ttu-id="3c5b0-839">Adicionar suporte ao IP público do nó</span><span class="sxs-lookup"><span data-stu-id="3c5b0-839">Add node public IP support</span></span>
* <span data-ttu-id="3c5b0-840">Corrigir erros de digitação no comando de ajuda</span><span class="sxs-lookup"><span data-stu-id="3c5b0-840">Fix typo in the help command</span></span>

### <a name="appconfig"></a><span data-ttu-id="3c5b0-841">AppConfig</span><span class="sxs-lookup"><span data-stu-id="3c5b0-841">AppConfig</span></span>

* <span data-ttu-id="3c5b0-842">Resolver referência do cofre de chaves para os comandos kv list e export</span><span class="sxs-lookup"><span data-stu-id="3c5b0-842">Resolve key vault reference for kv list and export commands</span></span>
* <span data-ttu-id="3c5b0-843">Correção de bug para valores de chave da lista</span><span class="sxs-lookup"><span data-stu-id="3c5b0-843">Bug fix for list key values</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-844">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-844">AppService</span></span>

* <span data-ttu-id="3c5b0-845">`az functionapp create`: mudou a maneira como o linuxFxVersion estava sendo definido para os aplicativos de funções dotnet linux.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-845">`az functionapp create`: Changed the way linuxFxVersion was being set for dotnet linux function apps.</span></span> <span data-ttu-id="3c5b0-846">Isso deve corrigir um bug que estava impedindo a criação de aplicativos de consumo em dotnet linux</span><span class="sxs-lookup"><span data-stu-id="3c5b0-846">This should fix a bug that was preventing dotnet linux consumption apps from being created</span></span>
* <span data-ttu-id="3c5b0-847">[ALTERAÇÃO DA FALHA] `az webapp create`: correção para manter o AppSettings existente com o az webapp create</span><span class="sxs-lookup"><span data-stu-id="3c5b0-847">[BREAKING CHANGE] `az webapp create`: fix to keep existing AppSettings with az webapp create</span></span>
* <span data-ttu-id="3c5b0-848">[ALTERAÇÃO DA FALHA] `az webapp up`: correção para criar o RG para o comando az webapp up ao usar o sinalizador -g</span><span class="sxs-lookup"><span data-stu-id="3c5b0-848">[BREAKING CHANGE] `az webapp up`: fix to create RG for az webapp up command when using -g flag</span></span>
* <span data-ttu-id="3c5b0-849">[ALTERAÇÃO DA FALHA] `az webapp config`: correção para mostrar valores de saída não JSON com o az webapp config connection-string list</span><span class="sxs-lookup"><span data-stu-id="3c5b0-849">[BREAKING CHANGE] `az webapp config`: fix to show values for non-JSON output with az webapp config connection-string list</span></span>

### <a name="arm"></a><span data-ttu-id="3c5b0-850">ARM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-850">ARM</span></span>

* <span data-ttu-id="3c5b0-851">`az deployment create/validate`: adicionar o parâmetro `--no-prompt` para dar suporte à ação de ignorar o prompt de parâmetros ausentes para o modelo do Resource Manager</span><span class="sxs-lookup"><span data-stu-id="3c5b0-851">`az deployment create/validate`: Add parameter `--no-prompt` to support skipping the prompt of missing parameters for ARM template</span></span>
* <span data-ttu-id="3c5b0-852">`az deployment group/mg/sub/tenant validate`: dar suporte aos comentários no arquivo de parâmetro de implantação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-852">`az deployment group/mg/sub/tenant validate`: Support comments in deployment parameter file</span></span>
* <span data-ttu-id="3c5b0-853">`az deployment`: remover `is_preview` para o parâmetro `--handle-extended-json-format`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-853">`az deployment`: Remove `is_preview` for parameter `--handle-extended-json-format`</span></span>
* <span data-ttu-id="3c5b0-854">`az deployment group/mg/sub/tenant cancel`: dar suporte para cancelar a implantação do modelo do Resource Manager</span><span class="sxs-lookup"><span data-stu-id="3c5b0-854">`az deployment group/mg/sub/tenant cancel`: Support cancel deployment for ARM template</span></span>
* <span data-ttu-id="3c5b0-855">`az deployment group/mg/sub/tenant validate`: melhorar a mensagem de erro quando a verificação de implantação falhar</span><span class="sxs-lookup"><span data-stu-id="3c5b0-855">`az deployment group/mg/sub/tenant validate`: Improve the error message when deployment verification fails</span></span>
* <span data-ttu-id="3c5b0-856">`az deployment-scripts`: adicionar novos comandos para DeploymentScripts</span><span class="sxs-lookup"><span data-stu-id="3c5b0-856">`az deployment-scripts`: Add new commands for DeploymentScripts</span></span>
* <span data-ttu-id="3c5b0-857">`az resource tag`: adicionar o parâmetro `--is-incremental` para dar suporte à adição de marcas ao recurso de maneira incremental</span><span class="sxs-lookup"><span data-stu-id="3c5b0-857">`az resource tag`: Add parameter `--is-incremental` to support adding tags to resource incrementally</span></span>

### <a name="aro"></a><span data-ttu-id="3c5b0-858">ARO</span><span class="sxs-lookup"><span data-stu-id="3c5b0-858">ARO</span></span>

* <span data-ttu-id="3c5b0-859">`az aro`:  adicionar módulo de comando aro do Azure RedHat OpenShift V4</span><span class="sxs-lookup"><span data-stu-id="3c5b0-859">`az aro`:  Add Azure RedHat OpenShift V4 aro command module</span></span>

### <a name="batch"></a><span data-ttu-id="3c5b0-860">Lote</span><span class="sxs-lookup"><span data-stu-id="3c5b0-860">Batch</span></span>

* <span data-ttu-id="3c5b0-861">Atualizar a API do Lote</span><span class="sxs-lookup"><span data-stu-id="3c5b0-861">Update Batch API</span></span>

### <a name="compute"></a><span data-ttu-id="3c5b0-862">Computação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-862">Compute</span></span>

* <span data-ttu-id="3c5b0-863">`az sig image-version create`: adicionar o tipo da conta de armazenamento Premium_LRS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-863">`az sig image-version create`: Add storage account type Premium_LRS</span></span>
* <span data-ttu-id="3c5b0-864">`az vmss update`: corrigir problema de atualização de notificação de término</span><span class="sxs-lookup"><span data-stu-id="3c5b0-864">`az vmss update`: Fix terminate notification update issue</span></span>
* <span data-ttu-id="3c5b0-865">`az vm/vmss create`: adicionar suporte para a versão de imagem especializada</span><span class="sxs-lookup"><span data-stu-id="3c5b0-865">`az vm/vmss create`: Add support for specialized image version</span></span>
* <span data-ttu-id="3c5b0-866">Versão da API SIG 2019-12-01</span><span class="sxs-lookup"><span data-stu-id="3c5b0-866">SIG API Version 2019-12-01</span></span>
* <span data-ttu-id="3c5b0-867">`az sig image-version create`: Adicionar --target-region-encryption</span><span class="sxs-lookup"><span data-stu-id="3c5b0-867">`az sig image-version create`: Add --target-region-encryption</span></span>
* <span data-ttu-id="3c5b0-868">Os testes de correção falham quando executados em série, pois o nome do keyvault está duplicado no cache global na memória</span><span class="sxs-lookup"><span data-stu-id="3c5b0-868">Fix tests fail when running in serial due to keyvault name is duplicated in global in-momery cache</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="3c5b0-869">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="3c5b0-869">CosmosDB</span></span>

* <span data-ttu-id="3c5b0-870">Dar suporte à `az cosmosdb private-link-resource/private-endpoint-connection`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-870">Support `az cosmosdb private-link-resource/private-endpoint-connection`</span></span>

### <a name="iot-central"></a><span data-ttu-id="3c5b0-871">Central da IoT</span><span class="sxs-lookup"><span data-stu-id="3c5b0-871">IoT Central</span></span>

* <span data-ttu-id="3c5b0-872">Preterir `az iotcentral`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-872">Deprecate `az iotcentral`</span></span>
* <span data-ttu-id="3c5b0-873">Adicionar o módulo de comando `az iot central`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-873">Add `az iot central` command module</span></span>

### <a name="monitor"></a><span data-ttu-id="3c5b0-874">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-874">Monitor</span></span>

* <span data-ttu-id="3c5b0-875">Dar suporte ao cenário de link privado para monitoramento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-875">Support private link scenario for monitor</span></span>
* <span data-ttu-id="3c5b0-876">Corrigir a maneira incorreta de simulação em test_monitor_general_operations.py</span><span class="sxs-lookup"><span data-stu-id="3c5b0-876">Fix wrong mocking way in test_monitor_general_operations.py</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-877">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-877">Network</span></span>

* <span data-ttu-id="3c5b0-878">Preterir o sku para o comando de atualização de ip público</span><span class="sxs-lookup"><span data-stu-id="3c5b0-878">Deprecate sku for public ip update command</span></span>
* <span data-ttu-id="3c5b0-879">`az network private-endpoint`: dar suporte ao grupo de zona dns privada</span><span class="sxs-lookup"><span data-stu-id="3c5b0-879">`az network private-endpoint`: Support private dns zone group</span></span>
* <span data-ttu-id="3c5b0-880">Habilitar o recurso de contexto local para o parâmetro vnet/sub-rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-880">Enable local context feature for vnet/subnet parameter</span></span>
* <span data-ttu-id="3c5b0-881">Corrigir o exemplo de uso incorreto em test_nw_flow_log_delete</span><span class="sxs-lookup"><span data-stu-id="3c5b0-881">Fix wrong usage example in test_nw_flow_log_delete</span></span>

### <a name="packaging"></a><span data-ttu-id="3c5b0-882">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-882">Packaging</span></span>

* <span data-ttu-id="3c5b0-883">Descartar o suporte para o pacote Ubuntu/Disco</span><span class="sxs-lookup"><span data-stu-id="3c5b0-883">Drop support for Ubuntu/Disco package</span></span>

### <a name="rbac"></a><span data-ttu-id="3c5b0-884">RBAC</span><span class="sxs-lookup"><span data-stu-id="3c5b0-884">RBAC</span></span>

* <span data-ttu-id="3c5b0-885">`az ad app create/update`: dar suporte a --optional-claims como um parâmetro</span><span class="sxs-lookup"><span data-stu-id="3c5b0-885">`az ad app create/update`: support --optional-claims as a parameter</span></span>

### <a name="rdbms"></a><span data-ttu-id="3c5b0-886">RDBMS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-886">RDBMS</span></span>

* <span data-ttu-id="3c5b0-887">Adicionar comandos do administrador do Azure Active Directory para PostgreSQL e MySQL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-887">Add Azure active directory administrator commands for PostgreSQL and MySQL</span></span>

### <a name="service-fabric"></a><span data-ttu-id="3c5b0-888">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="3c5b0-888">Service Fabric</span></span>

* <span data-ttu-id="3c5b0-889">Correção nº 12891: `az sf application update --application-parameters` remove parâmetros antigos que não estão na solicitação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-889">Fix #12891: `az sf application update --application-parameters` removes old parameters that are not in the request</span></span>
* <span data-ttu-id="3c5b0-890">Correção nº 12470 az sf create cluster, corrigir bugs na atualização de durabilidade e confiabilidade e encontrar vmss corretamente por meio do código, dado um nome de tipo de nó</span><span class="sxs-lookup"><span data-stu-id="3c5b0-890">Fix #12470 az sf create cluster, fix bugs in update durability and reliability and find vmss correctly through the code given a node type name</span></span>

### <a name="sql"></a><span data-ttu-id="3c5b0-891">SQL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-891">SQL</span></span>

* <span data-ttu-id="3c5b0-892">Adicionar `az sql mi op list`, `az sql mi op get`, `az sql mi op cancel`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-892">Add `az sql mi op list`, `az sql mi op get`, `az sql mi op cancel`</span></span>
* <span data-ttu-id="3c5b0-893">`az sql midb`: atualizar/mostrar política de retenção de longo prazo, mostrar/excluir backups de retenção de longo prazo, restaurar backup de retenção de longo prazo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-893">`az sql midb`: update/show long term retention policy,  show/delete long term retention backups, restore long term retention backup</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-894">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-894">Storage</span></span>

* <span data-ttu-id="3c5b0-895">Atualizar azure-mgmt-storage para 9.0.0</span><span class="sxs-lookup"><span data-stu-id="3c5b0-895">Upgrade azure-mgmt-storage to 9.0.0</span></span>
* <span data-ttu-id="3c5b0-896">`az storage logging off`: dar suporte à desativação do registro em log de uma conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-896">`az storage logging off`: Support turning off logging for a storage account</span></span>
* <span data-ttu-id="3c5b0-897">`az storage account update`: habilitar rotação automática de chave para CMK</span><span class="sxs-lookup"><span data-stu-id="3c5b0-897">`az storage account update`: Enable key auto-rotated for CMK</span></span>
* <span data-ttu-id="3c5b0-898">`az storage account encryption-scope create/update/list/show`: adicionar suporte para personalizar o escopo de criptografia</span><span class="sxs-lookup"><span data-stu-id="3c5b0-898">`az storage account encryption-scope create/update/list/show`: Add support to customize encryption scope</span></span>
* <span data-ttu-id="3c5b0-899">`az storage container create`: adicionar --default-encryption-scope e --deny-encryption-scope-override a fim de definir o escopo de criptografia para o nível de contêiner</span><span class="sxs-lookup"><span data-stu-id="3c5b0-899">`az storage container create`: Add --default-encryption-scope and --deny-encryption-scope-override to set encryption scope for container level</span></span>

### <a name="survey"></a><span data-ttu-id="3c5b0-900">Pesquisa</span><span class="sxs-lookup"><span data-stu-id="3c5b0-900">Survey</span></span>

* <span data-ttu-id="3c5b0-901">Adicionar opção para desligar o link de pesquisa</span><span class="sxs-lookup"><span data-stu-id="3c5b0-901">Add switch to turn off survey link</span></span>

## <a name="april-01-2020"></a><span data-ttu-id="3c5b0-902">1º de abril de 2020</span><span class="sxs-lookup"><span data-stu-id="3c5b0-902">April 01, 2020</span></span>

<span data-ttu-id="3c5b0-903">Versão 2.3.1</span><span class="sxs-lookup"><span data-stu-id="3c5b0-903">Version 2.3.1</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-904">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-904">ACR</span></span>

* <span data-ttu-id="3c5b0-905">Corrigir a versão errada do azure-mgmt-containerregistry para Linux</span><span class="sxs-lookup"><span data-stu-id="3c5b0-905">Fix wrong version of azure-mgmt-containerregistry for Linux</span></span>

### <a name="profile"></a><span data-ttu-id="3c5b0-906">Perfil</span><span class="sxs-lookup"><span data-stu-id="3c5b0-906">Profile</span></span>

* <span data-ttu-id="3c5b0-907">az login: Corrigir falha de logon com perfis de nuvem diferentes de `latest`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-907">az login: Fix login failure with cloud profiles other than `latest`</span></span>

## <a name="march-31-2020"></a><span data-ttu-id="3c5b0-908">31 de março de 2020</span><span class="sxs-lookup"><span data-stu-id="3c5b0-908">March 31, 2020</span></span>

<span data-ttu-id="3c5b0-909">Versão 2.3.0</span><span class="sxs-lookup"><span data-stu-id="3c5b0-909">Version 2.3.0</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-910">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-910">ACR</span></span>

* <span data-ttu-id="3c5b0-911">'az acr task update': exceção de ponteiro nulo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-911">'az acr task update': null pointer exception</span></span>
* <span data-ttu-id="3c5b0-912">`az acr import`: Modificar a mensagem de ajuda e de erro para esclarecer o uso de --source e --registry</span><span class="sxs-lookup"><span data-stu-id="3c5b0-912">`az acr import`: Modify help and error message to clarify the usage of --source and --registry</span></span>
* <span data-ttu-id="3c5b0-913">Adicionar um validador para o argumento 'registry_name'</span><span class="sxs-lookup"><span data-stu-id="3c5b0-913">Add a validator for argument 'registry_name'</span></span>
* <span data-ttu-id="3c5b0-914">`az acr login`: remover o sinalizador de visualização em '--expose-token'</span><span class="sxs-lookup"><span data-stu-id="3c5b0-914">`az acr login`:Remove the preview flag on '--expose-token'</span></span>
* <span data-ttu-id="3c5b0-915">O parâmetro de branch 'az acr task create/update' de [ALTERAÇÃO SIGNIFICATIVA] foi removido</span><span class="sxs-lookup"><span data-stu-id="3c5b0-915">[BREAKING CHANGE] 'az acr task create/update' Branch parameter is removed</span></span>
* <span data-ttu-id="3c5b0-916">O cliente 'az acr task update' agora pode atualizar o contexto, o token do git e/ou os gatilhos individualmente</span><span class="sxs-lookup"><span data-stu-id="3c5b0-916">'az acr task update' Customer now can update context, git-token, and or triggers individually</span></span>
* <span data-ttu-id="3c5b0-917">'az acr agentpool': novo recurso</span><span class="sxs-lookup"><span data-stu-id="3c5b0-917">'az acr agentpool': new feature</span></span>

### <a name="aks"></a><span data-ttu-id="3c5b0-918">AKS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-918">AKS</span></span>

* <span data-ttu-id="3c5b0-919">Corrigir apiServerAccessProfile ao atualizar --api-server-authorized-ip-ranges</span><span class="sxs-lookup"><span data-stu-id="3c5b0-919">Fix apiServerAccessProfile when updating --api-server-authorized-ip-ranges</span></span>
* <span data-ttu-id="3c5b0-920">aks update: Substituir IPs de saída por valores de entrada ao atualizar</span><span class="sxs-lookup"><span data-stu-id="3c5b0-920">aks update: Override outbound IPs with input values when update</span></span>
* <span data-ttu-id="3c5b0-921">Não criar SPN para clusters MSI e dar suporte à anexação de ACR a clusters MSI</span><span class="sxs-lookup"><span data-stu-id="3c5b0-921">Do not create SPN for MSI clusters and support attach acr to MSI clusters</span></span>

### <a name="ams"></a><span data-ttu-id="3c5b0-922">AMS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-922">AMS</span></span>

* <span data-ttu-id="3c5b0-923">Correção nº. 12469: a adição da política de chave de conteúdo Fairplay falha devido a problemas com o parâmetro 'ask'</span><span class="sxs-lookup"><span data-stu-id="3c5b0-923">Fix #12469: adding Fairplay content-key-policy fails due to problems with 'ask' parameter</span></span>

### <a name="appconfig"></a><span data-ttu-id="3c5b0-924">AppConfig</span><span class="sxs-lookup"><span data-stu-id="3c5b0-924">AppConfig</span></span>

* <span data-ttu-id="3c5b0-925">Adicionar --skip-keyvault a kv export</span><span class="sxs-lookup"><span data-stu-id="3c5b0-925">Add --skip-keyvault for kv export</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-926">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-926">AppService</span></span>

* <span data-ttu-id="3c5b0-927">Correção nº 12509: remover a marca para az webapp up por padrão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-927">Fix #12509: Remove the tag to az webapp up by default</span></span>
* <span data-ttu-id="3c5b0-928">az functionapp create: o menu de ajuda de --runtime-version foi atualizado e um aviso foi adicionado quando o usuário especifica --runtime-version para dotnet</span><span class="sxs-lookup"><span data-stu-id="3c5b0-928">az functionapp create: Updated --runtime-version help menu and added warning when user specifies --runtime-version for dotnet</span></span>
* <span data-ttu-id="3c5b0-929">az functionapp create: atualizado o modo como o javaVersion estava sendo definido para aplicativos de funções do Windows</span><span class="sxs-lookup"><span data-stu-id="3c5b0-929">az functionapp create: Updated the way javaVersion was being set for Windows function apps</span></span>

### <a name="arm"></a><span data-ttu-id="3c5b0-930">ARM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-930">ARM</span></span>

* <span data-ttu-id="3c5b0-931">az deployment create/validate: usar --handle-extended-json-format por padrão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-931">az deployment create/validate: Use --handle-extended-json-format by default</span></span>
* <span data-ttu-id="3c5b0-932">az lock create: adicionar exemplos de criação de subrecurso na documentação da ajuda</span><span class="sxs-lookup"><span data-stu-id="3c5b0-932">az lock create: Add examples of creating subresource in the help documentation</span></span>
* <span data-ttu-id="3c5b0-933">az deployment {group/mg/sub/tenant} list: dar suporte à filtragem de provisioningState</span><span class="sxs-lookup"><span data-stu-id="3c5b0-933">az deployment {group/mg/sub/tenant} list: Support provisioningState filtering</span></span>
* <span data-ttu-id="3c5b0-934">az deployment: corrigir o bug de análise para o comentário no último argumento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-934">az deployment: Fix the parse bug for comment under the last argument</span></span>

### <a name="backup"></a><span data-ttu-id="3c5b0-935">Backup</span><span class="sxs-lookup"><span data-stu-id="3c5b0-935">Backup</span></span>

* <span data-ttu-id="3c5b0-936">Adicionadas várias funcionalidades de restauração de arquivo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-936">Added multiple files restore capabilities</span></span>
* <span data-ttu-id="3c5b0-937">Adicionado suporte para backup somente de discos do SO</span><span class="sxs-lookup"><span data-stu-id="3c5b0-937">Added support for Backing up OS Disks only</span></span>
* <span data-ttu-id="3c5b0-938">Adicionado o parâmetro restore-as-unmanaged-disk para especificar a restauração não gerenciada</span><span class="sxs-lookup"><span data-stu-id="3c5b0-938">Added restore-as-unmanaged-disk parameter to specify unmanaged restore</span></span>

### <a name="compute"></a><span data-ttu-id="3c5b0-939">Computação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-939">Compute</span></span>

* <span data-ttu-id="3c5b0-940">az vm create: adicionar opção NONE de --nsg-rule</span><span class="sxs-lookup"><span data-stu-id="3c5b0-940">az vm create: Add NONE option of --nsg-rule</span></span>
* <span data-ttu-id="3c5b0-941">az vmss create/update: remover a marca de visualização de reparos automáticos do vmss</span><span class="sxs-lookup"><span data-stu-id="3c5b0-941">az vmss create/update: remove vmss automatic repairs preview tag</span></span>
* <span data-ttu-id="3c5b0-942">az vm update: dar suporte a --workspace</span><span class="sxs-lookup"><span data-stu-id="3c5b0-942">az vm update: Support --workspace</span></span>
* <span data-ttu-id="3c5b0-943">Corrigir um bug no código de inicialização de VirtualMachineScaleSetExtension</span><span class="sxs-lookup"><span data-stu-id="3c5b0-943">Fix a bug in VirtualMachineScaleSetExtension initialization code</span></span>
* <span data-ttu-id="3c5b0-944">Atualizar a versão do VMAccessAgent para 2.4</span><span class="sxs-lookup"><span data-stu-id="3c5b0-944">Upgrade VMAccessAgent version to 2.4</span></span>
* <span data-ttu-id="3c5b0-945">az vmss set-orchestration-service-state: dar suporte para o estado de definição do serviço de orquestração do vmss</span><span class="sxs-lookup"><span data-stu-id="3c5b0-945">az vmss set-orchestration-service-state: support vmss set orchestration service state</span></span>
* <span data-ttu-id="3c5b0-946">Atualizar a API do disco para a versão 2019-11-01</span><span class="sxs-lookup"><span data-stu-id="3c5b0-946">Upgrade disk API version to 2019-11-01</span></span>
* <span data-ttu-id="3c5b0-947">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun</span><span class="sxs-lookup"><span data-stu-id="3c5b0-947">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="3c5b0-948">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="3c5b0-948">Cosmos DB</span></span>

* <span data-ttu-id="3c5b0-949">Corrigir a ausência da opção --type para redirecionamentos de preterimento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-949">Fix missing --type option for deprecation redirections</span></span>

### <a name="docker"></a><span data-ttu-id="3c5b0-950">Docker</span><span class="sxs-lookup"><span data-stu-id="3c5b0-950">Docker</span></span>

* <span data-ttu-id="3c5b0-951">Atualizar para Alpine 3.11 e Python 3.6.10</span><span class="sxs-lookup"><span data-stu-id="3c5b0-951">Update to Alpine 3.11 and Python 3.6.10</span></span>

### <a name="extension"></a><span data-ttu-id="3c5b0-952">Extensão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-952">Extension</span></span>

* <span data-ttu-id="3c5b0-953">Permitir carregar extensões no caminho do sistema por meio de pacotes</span><span class="sxs-lookup"><span data-stu-id="3c5b0-953">Allow to load extensions in the system path via packages</span></span>

### <a name="hdinsight"></a><span data-ttu-id="3c5b0-954">HDInsight</span><span class="sxs-lookup"><span data-stu-id="3c5b0-954">HDInsight</span></span>

* <span data-ttu-id="3c5b0-955">(az hdinsight create:) dar suporte à especificação da versão de TLS mínima pelos clientes usando o parâmetro `--minimal-tls-version`.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-955">(az hdinsight create:) Support customers specify minimal supported tls version by using parameter `--minimal-tls-version`.</span></span> <span data-ttu-id="3c5b0-956">O valor permitido é 1.0,1.1,1.2</span><span class="sxs-lookup"><span data-stu-id="3c5b0-956">The allowed value is 1.0,1.1,1.2</span></span>

### <a name="iot"></a><span data-ttu-id="3c5b0-957">IoT</span><span class="sxs-lookup"><span data-stu-id="3c5b0-957">IoT</span></span>

* <span data-ttu-id="3c5b0-958">Adicionar codeowner</span><span class="sxs-lookup"><span data-stu-id="3c5b0-958">Add codeowner</span></span>
* <span data-ttu-id="3c5b0-959">az iot hub create : alterar o SKU padrão de F1 para S1</span><span class="sxs-lookup"><span data-stu-id="3c5b0-959">az iot hub create : Change default sku to S1 from F1</span></span>
* <span data-ttu-id="3c5b0-960">iot hub: dar suporte a IotHub no perfil de 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="3c5b0-960">iot hub: Support IotHub in the profile of 2019-03-01-hybrid</span></span>

### <a name="iotcentral"></a><span data-ttu-id="3c5b0-961">IoT Central</span><span class="sxs-lookup"><span data-stu-id="3c5b0-961">IoTCentral</span></span>

* <span data-ttu-id="3c5b0-962">Atualizar detalhes do erro, atualizar modelo de aplicativo padrão e a mensagem de aviso</span><span class="sxs-lookup"><span data-stu-id="3c5b0-962">Update error details, update default application template and prompt message</span></span>

### <a name="keyvault"></a><span data-ttu-id="3c5b0-963">KeyVault</span><span class="sxs-lookup"><span data-stu-id="3c5b0-963">KeyVault</span></span>

* <span data-ttu-id="3c5b0-964">Suporte para backup/restauração de certificado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-964">Support certificate backup/restore</span></span>
* <span data-ttu-id="3c5b0-965">keyvault create/update: Suporte a --retention-days</span><span class="sxs-lookup"><span data-stu-id="3c5b0-965">keyvault create/update: Support --retention-days</span></span>
* <span data-ttu-id="3c5b0-966">Não exibir mais chaves/segredos gerenciados durante a listagem</span><span class="sxs-lookup"><span data-stu-id="3c5b0-966">No longer display managed keys/secrets while listing</span></span>
* <span data-ttu-id="3c5b0-967">az keyvault create: suporte a `--network-acls`, `--network-acls-ips` e `--network-acls-vnets` para especificar regras de rede ao criar o cofre</span><span class="sxs-lookup"><span data-stu-id="3c5b0-967">az keyvault create: support `--network-acls`, `--network-acls-ips` and `--network-acls-vnets` for specifying network rules while creating vault</span></span>

### <a name="lock"></a><span data-ttu-id="3c5b0-968">Bloqueio</span><span class="sxs-lookup"><span data-stu-id="3c5b0-968">Lock</span></span>

* <span data-ttu-id="3c5b0-969">az lock delete fix bug: az lock delete não funciona no Microsoft.DocumentDB</span><span class="sxs-lookup"><span data-stu-id="3c5b0-969">az lock delete fix bug: az lock delete does not work on Microsoft.DocumentDB</span></span>

### <a name="monitor"></a><span data-ttu-id="3c5b0-970">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-970">Monitor</span></span>

* <span data-ttu-id="3c5b0-971">az monitor clone: suporte a regras de métrica de clone de um recurso para outro</span><span class="sxs-lookup"><span data-stu-id="3c5b0-971">az monitor clone: support clone metric rules from one resource to another</span></span>
* <span data-ttu-id="3c5b0-972">Corrigir IcM179210086: não é possível criar um alerta de métrica personalizado para a métrica de Application Insights</span><span class="sxs-lookup"><span data-stu-id="3c5b0-972">Fix IcM179210086: unable to create custom metric alert for their Application Insights metric</span></span>

### <a name="netappfiles"></a><span data-ttu-id="3c5b0-973">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="3c5b0-973">NetAppFiles</span></span>

* <span data-ttu-id="3c5b0-974">az volume create: permitir volumes de proteção de dados adicionando operações de replicação: approve, suspend, resume, status, remove</span><span class="sxs-lookup"><span data-stu-id="3c5b0-974">az volume create: Allow data protection volumes adding replication operations: approve, suspend, resume, status, remove</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-975">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-975">Network</span></span>

* <span data-ttu-id="3c5b0-976">az network application-gateway waf-policy managed-rule rule-set add: dar suporte a Microsoft_BotManagerRuleSet</span><span class="sxs-lookup"><span data-stu-id="3c5b0-976">az network application-gateway waf-policy managed-rule rule-set add: support Microsoft_BotManagerRuleSet</span></span>
* <span data-ttu-id="3c5b0-977">network watcher flow-log show: corrigir informações erradas em preterimento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-977">network watcher flow-log show: fix wrong deprecating info</span></span>
* <span data-ttu-id="3c5b0-978">dar suporte a nomes de host no ouvinte do gateway de aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-978">support host names in application gateway listener</span></span>
* <span data-ttu-id="3c5b0-979">az network nat gateway: dar suporte para criar um recurso vazio sem IP público nem prefixo de IP público</span><span class="sxs-lookup"><span data-stu-id="3c5b0-979">az network nat gateway: support create empty resource without public ip or public ip prefix</span></span>
* <span data-ttu-id="3c5b0-980">Dar suporte à geração de gateway de VPN</span><span class="sxs-lookup"><span data-stu-id="3c5b0-980">Support vpn gateway generation</span></span>
* <span data-ttu-id="3c5b0-981">Dar suporte a `--if-none-match` em `az network dns record-set {} add-record`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-981">Support `--if-none-match` in `az network dns record-set {} add-record`</span></span>

### <a name="packaging"></a><span data-ttu-id="3c5b0-982">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-982">Packaging</span></span>

* <span data-ttu-id="3c5b0-983">Remover o suporte ao Python 3.5</span><span class="sxs-lookup"><span data-stu-id="3c5b0-983">Drop support for python 3.5</span></span>

### <a name="profile"></a><span data-ttu-id="3c5b0-984">Perfil</span><span class="sxs-lookup"><span data-stu-id="3c5b0-984">Profile</span></span>

* <span data-ttu-id="3c5b0-985">az login: Mostrar aviso para erro de MFA</span><span class="sxs-lookup"><span data-stu-id="3c5b0-985">az login: Show warning for MFA error</span></span>

### <a name="rdbms"></a><span data-ttu-id="3c5b0-986">RDBMS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-986">RDBMS</span></span>

* <span data-ttu-id="3c5b0-987">Adicionar comandos de gerenciamento de chaves de criptografia de dados do servidor para PostgreSQL e MySQL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-987">Add server data encryption key management commands for PostgreSQL and MySQL</span></span>

## <a name="march-10-2020"></a><span data-ttu-id="3c5b0-988">10 de março de 2020</span><span class="sxs-lookup"><span data-stu-id="3c5b0-988">March 10, 2020</span></span>

<span data-ttu-id="3c5b0-989">Versão 2.2.0</span><span class="sxs-lookup"><span data-stu-id="3c5b0-989">Version 2.2.0</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-990">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-990">ACR</span></span>

* <span data-ttu-id="3c5b0-991">Correção: `az acr login` gerava erro incorretamente</span><span class="sxs-lookup"><span data-stu-id="3c5b0-991">Fix: `az acr login` wrongly raise error</span></span>
* <span data-ttu-id="3c5b0-992">Adicionou o novo comando `az acr helm install-cli`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-992">Add new command `az acr helm install-cli`</span></span>
* <span data-ttu-id="3c5b0-993">Adicionou link privado e suporte do CMK</span><span class="sxs-lookup"><span data-stu-id="3c5b0-993">Add private link and CMK support</span></span>
* <span data-ttu-id="3c5b0-994">Adicionou o comando 'private-link-resource list'</span><span class="sxs-lookup"><span data-stu-id="3c5b0-994">add 'private-link-resource list' command</span></span>

### <a name="aks"></a><span data-ttu-id="3c5b0-995">AKS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-995">AKS</span></span>

* <span data-ttu-id="3c5b0-996">correção da busca do AKS no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="3c5b0-996">fix the aks browse in cloud shell</span></span>
* <span data-ttu-id="3c5b0-997">az aks: correção dos erros de complemento de monitoramento e de agentpool NoneType</span><span class="sxs-lookup"><span data-stu-id="3c5b0-997">az aks: Fix monitoring addon and agentpool NoneType errors</span></span>
* <span data-ttu-id="3c5b0-998">Adicionou --nodepool-tags ao pool de nós ao criar o cluster do Kubernetes do Azure</span><span class="sxs-lookup"><span data-stu-id="3c5b0-998">Add --nodepool-tags to node pool when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="3c5b0-999">Adicionou --tags ao adicionar ou atualizar um pool de nós para o cluster</span><span class="sxs-lookup"><span data-stu-id="3c5b0-999">Add --tags when adding or updating a nodepool to cluster</span></span>
* <span data-ttu-id="3c5b0-1000">AKS create: adicionou `--enable-private-cluster`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1000">aks create: add `--enable-private-cluster`</span></span>
* <span data-ttu-id="3c5b0-1001">Adicionou --nodepool-labels ao criar o cluster do Kubernetes do Azure</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1001">add --nodepool-labels when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="3c5b0-1002">Adicionou --labels ao adicionar um novo pool de nós ao cluster do Kubernetes do Azure</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1002">add --labels when adding a new nodepool to azure kubernetes cluster</span></span>
* <span data-ttu-id="3c5b0-1003">Adicionou / ausente na URL do painel</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1003">add missing / in the dashboard url</span></span>
* <span data-ttu-id="3c5b0-1004">Suporte para criar clusters do AKS habilitando identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1004">Support create aks clusters enabling managed identity</span></span>
* <span data-ttu-id="3c5b0-1005">az aks: validou o plug-in de rede como "Azure" ou "Kubenet"</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1005">az aks: Validate network plugin to be either "azure" or "kubenet"</span></span>
* <span data-ttu-id="3c5b0-1006">az aks: adicionou suporte da chave da sessão do AAD</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1006">az aks: Add aad session key support</span></span>
* <span data-ttu-id="3c5b0-1007">[ALTERAÇÃO SIGNIFICATIVA] AZ AKS: suporte para alterações de MSI para GF e BF para omsagent (Monitoramento de contêiner) (#1)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1007">[BREAKING CHANGE] az aks: support msi changes for GF and BF for omsagent (Container monitoring)(#1)</span></span>
* <span data-ttu-id="3c5b0-1008">az aks use-dev-spaces: adicionou a opção de tipo de ponto de extremidade ao comando use-dev-spaces para personalizar o ponto de extremidade criado em um controlador Azure Dev Spaces</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1008">az aks use-dev-spaces: Adding endpoint type option to the use-dev-spaces command to customize the endpoint created on an Azure Dev Spaces controller</span></span>

### <a name="appconfig"></a><span data-ttu-id="3c5b0-1009">AppConfig</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1009">AppConfig</span></span>

* <span data-ttu-id="3c5b0-1010">Desbloqueou usando "KV set" para adicionar o recurso e a referência do keyvault...</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1010">Unblock using "kv set" to add keyvault reference and feature …</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-1011">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1011">AppService</span></span>

* <span data-ttu-id="3c5b0-1012">az webapp create: correção do problema ao executar o comando com --runtime</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1012">az webapp create : Fix issue when running the command with --runtime</span></span>
* <span data-ttu-id="3c5b0-1013">az functionapp deployment source config-zip: adicionou uma mensagem de erro se o grupo de recursos ou o nome da função forem inválidos/não existirem</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1013">az functionapp deployment source config-zip: Add an error message if resource group or function name are invalid/don't exist</span></span>
* <span data-ttu-id="3c5b0-1014">functionapp create: correção da mensagem de aviso que aparece com `functionapp create` hoje, que cita um sinalizador de `--functions_version`, mas usa erroneamente `_` em vez de `-` no nome do sinalizador</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1014">functionapp create: Fix the warning message that appears with `functionapp create` today which cites a `--functions_version` flag but erroneously uses a `_` instead of a `-` in the flag name</span></span>
* <span data-ttu-id="3c5b0-1015">az functionapp create: atualizou o modo como linuxFxVersion e o nome da imagem de contêiner eram definidos para aplicativos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1015">az functionapp create: Updated the way linuxFxVersion and container image name were being set for linux function apps</span></span>
* <span data-ttu-id="3c5b0-1016">az functionapp deployment source config-zip: correção de um problema causado pelas configurações do aplicativo que alterava a condição de corrida durante a implantação do zip, provocando erros 5xx durante a implantação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1016">az functionapp deployment source config-zip: Fix an issue caused by app settings change racing condition during zip deploy, giving 5xx errors during deployment</span></span>
* <span data-ttu-id="3c5b0-1017">Correção #5720946: AZ WebApp backup falha ao definir o nome</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1017">Fix #5720946: az webapp backup fails to set name</span></span>

### <a name="arm"></a><span data-ttu-id="3c5b0-1018">ARM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1018">ARM</span></span>

* <span data-ttu-id="3c5b0-1019">az resource: aprimorou os exemplos do módulo de recurso</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1019">az resource: Improve the examples of the resource module</span></span>
* <span data-ttu-id="3c5b0-1020">az policy assignment list: suporte à listagem de atribuições de política no escopo do Grupo de Gerenciamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1020">az policy assignment list: Support listing policy assignments at Management Group scope</span></span>
* <span data-ttu-id="3c5b0-1021">Adicionou `az deployment group` e `az deployment operation group` para a implantação de modelos nos grupos de recursos.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1021">Add `az deployment group` and `az deployment operation group` for template deployment at resource groups.</span></span> <span data-ttu-id="3c5b0-1022">Esta é uma duplicata de `az group deployment` e `az group deployment operation`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1022">This is a duplicate of `az group deployment` and `az group deployment operation`</span></span>
* <span data-ttu-id="3c5b0-1023">Adicionou `az deployment sub` e `az deployment operation sub` para a implantação de modelos no escopo da assinatura.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1023">Add `az deployment sub` and `az deployment operation sub` for template deployment at subscription scope.</span></span> <span data-ttu-id="3c5b0-1024">Esta é uma duplicata de `az deployment` e `az deployment operation`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1024">This is a duplicate of `az deployment` and `az deployment operation`</span></span>
* <span data-ttu-id="3c5b0-1025">Adicionou `az deployment mg` e `az deployment operation mg` para implantação de modelos nos grupos de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1025">Add `az deployment mg` and `az deployment operation mg` for template deployment at management groups</span></span>
* <span data-ttu-id="3c5b0-1026">Adicionou `az deployment tenant` e `az deployment operation tenant` para implantação de modelos no escopo do locatário.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1026">Add `az deployment tenant` and `az deployment operation tenant` for template deployment at tenant scope</span></span>
* <span data-ttu-id="3c5b0-1027">az policy assignment create: adicionou descrição ao parâmetro `--location`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1027">az policy assignment create: Add a description to the `--location` parameter</span></span>
* <span data-ttu-id="3c5b0-1028">az group deployment create: adicionou o parâmetro `--aux-tenants` para dar suporte a locatários cruzados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1028">az group deployment create: Add parameter `--aux-tenants` to support cross tenants</span></span>

### <a name="cdn"></a><span data-ttu-id="3c5b0-1029">CDN</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1029">CDN</span></span>

* <span data-ttu-id="3c5b0-1030">Adicionou comandos do WAF da CDN</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1030">Add CDN WAF commands</span></span>

### <a name="compute"></a><span data-ttu-id="3c5b0-1031">Computação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1031">Compute</span></span>

* <span data-ttu-id="3c5b0-1032">az sig image-version: adicionar --data-snapshot-luns</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1032">az sig image-version: add --data-snapshot-luns</span></span>
* <span data-ttu-id="3c5b0-1033">AZ PPG show: adicionou --outlocation-status para habilitar a busca do status de colocalização de todos os recursos no grupo de posicionamento por proximidade</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1033">az ppg show: add --colocation-status to enable fetching the colocation status of all the resources in the proximity placement group</span></span>
* <span data-ttu-id="3c5b0-1034">az vmss create/update: suporte a reparos automáticos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1034">az vmss create/update: support automatic repairs</span></span>
* <span data-ttu-id="3c5b0-1035">[ALTERAÇÃO SIGNIFICATIVA] modelo de imagem AZ: renomear modelo para builder</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1035">[BREAKING CHANGE] az image template: rename template to builder</span></span>
* <span data-ttu-id="3c5b0-1036">AZ Image Builder Create: adicionou --Image-template</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1036">az image builder create: add --image-template</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="3c5b0-1037">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1037">Cosmos DB</span></span>

* <span data-ttu-id="3c5b0-1038">Adicionou procedimento armazenado do SQL, UDF e disparar cmdlets</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1038">Add Sql stored procedure, udf and trigger cmdlets</span></span>
* <span data-ttu-id="3c5b0-1039">az cosmosdb create: adicionou --key-uri para dar suporte à adição de informações de criptografia do cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1039">az cosmosdb create: add --key-uri to support adding key vault encryption information</span></span>

### <a name="keyvault"></a><span data-ttu-id="3c5b0-1040">KeyVault</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1040">KeyVault</span></span>

* <span data-ttu-id="3c5b0-1041">keyvault create: habilitou a exclusão reversível por padrão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1041">keyvault create: enable soft-delete by default</span></span>

### <a name="monitor"></a><span data-ttu-id="3c5b0-1042">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1042">Monitor</span></span>

* <span data-ttu-id="3c5b0-1043">az monitor metrics alert create: suporte a `~` em `--condition`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1043">az monitor metrics alert create: support `~` in `--condition`</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-1044">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1044">Network</span></span>

* <span data-ttu-id="3c5b0-1045">az network application-gateway rewrite-rule create: suporte à configuração de URL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1045">az network application-gateway rewrite-rule create: support url configuration</span></span>
* <span data-ttu-id="3c5b0-1046">az network dns zone import: --zone-name não diferenciará maiúsculas de minúsculas no futuro</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1046">az network dns zone import: --zone-name will be case insensitive in the future</span></span>
* <span data-ttu-id="3c5b0-1047">az network private-endpoint/private-link-service: removeu rótulo de visualização</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1047">az network private-endpoint/private-link-service: remove preview label</span></span>
* <span data-ttu-id="3c5b0-1048">az network bastion: suporte a bastions</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1048">az network bastion: support bastion</span></span>
* <span data-ttu-id="3c5b0-1049">az network vnet list-available-ips: dar suporte à lista de IPs disponíveis em uma vnet</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1049">az network vnet list-available-ips: support list available ips in a vnet</span></span>
* <span data-ttu-id="3c5b0-1050">az network watcher flow-log create/list/delete/update: adicionou novos comandos para gerenciar o log de fluxo do Inspetor e expor o --local para identificá-lo explicitamente</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1050">az network watcher flow-log create/list/delete/update: add new commands to manage watcher flow log and exposing --location to identify watcher explicitly</span></span>
* <span data-ttu-id="3c5b0-1051">az network watcher flow-log configure: preterido</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1051">az network watcher flow-log configure: deprecated</span></span>
* <span data-ttu-id="3c5b0-1052">az network watcher flow-log show: dá suporte a --location e --name para obter o resultado formatado por ARM, saída formatada antiga preterida</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1052">az network watcher flow-log show: support --location and --name to get ARM-formatted result, deprecated old formatted output</span></span>

### <a name="policy"></a><span data-ttu-id="3c5b0-1053">Política</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1053">Policy</span></span>

* <span data-ttu-id="3c5b0-1054">az policy assignment create: correção do bug que gerou automaticamente o nome da atribuição de política, que excede o limite</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1054">az policy assignment create: Fix the bug that automatically generated name of policy assignment exceeds the limit</span></span>

### <a name="rbac"></a><span data-ttu-id="3c5b0-1055">RBAC</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1055">RBAC</span></span>

* <span data-ttu-id="3c5b0-1056">az ad group show: correção do valor --group, que é tratado como um problema de regex</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1056">az ad group show: fix --group value treated as regex problem</span></span>

### <a name="rdbms"></a><span data-ttu-id="3c5b0-1057">RDBMS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1057">RDBMS</span></span>

* <span data-ttu-id="3c5b0-1058">Trocou a versão do zure-mgmt-rdbms SDK para 2.0.0</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1058">Bump the azure-mgmt-rdbms SDK version to 2.0.0</span></span>
* <span data-ttu-id="3c5b0-1059">az postgres private-endpoint-connection: gerenciou conexões de ponto de extremidade privado do Postgres</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1059">az postgres private-endpoint-connection: manage postgres private endpoint connections</span></span>
* <span data-ttu-id="3c5b0-1060">az postgres private-link-resource: gerenciou recursos de link privado do Postgres</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1060">az postgres private-link-resource: manage postgres private link resources</span></span>
* <span data-ttu-id="3c5b0-1061">az mysql private-endpoint-connection: gerenciar conexões de ponto de extremidade privado do MySQL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1061">az mysql private-endpoint-connection: manage mysql private endpoint connections</span></span>
* <span data-ttu-id="3c5b0-1062">az mysql private-link-resource: gerenciou recursos de link privado do MySQL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1062">az mysql private-link-resource: manage mysql private link resources</span></span>
* <span data-ttu-id="3c5b0-1063">az mariadb private-endpoint-connection: gerenciou conexões de ponto de extremidade privado do MariaDB</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1063">az mariadb private-endpoint-connection: manage mariadb private endpoint connections</span></span>
* <span data-ttu-id="3c5b0-1064">az mariadb private-link-resource: gerenciou recursos de link privado do MariaDB</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1064">az mariadb private-link-resource: manage mariadb private link resources</span></span>
* <span data-ttu-id="3c5b0-1065">Atualizando testes de ponto de extremidade privado do RDBMS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1065">Updating RDBMS Private Endpoint Tests</span></span>

### <a name="sql"></a><span data-ttu-id="3c5b0-1066">SQL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1066">SQL</span></span>

* <span data-ttu-id="3c5b0-1067">Sql midb Add: list-deleted, show-deleted, update-retention, show-retention</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1067">Sql midb Add: list-deleted, show-deleted, update-retention, show-retention</span></span>
* <span data-ttu-id="3c5b0-1068">(sql server create:) adicionou o sinalizador ' habilitar '/' desabilitar ' opcional public-network-access ao SQL Server create</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1068">(sql server create:) Add optional public-network-access 'Enable'/'Disable' flag to sql server create</span></span>
* <span data-ttu-id="3c5b0-1069">(sql server update:) fez algumas alterações voltadas para o cliente</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1069">(sql server update:) make some customer-facing change</span></span>
* <span data-ttu-id="3c5b0-1070">adicionou a propriedade minimal_tls_version para o banco de BD de MI e SQL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1070">Add minimal_tls_version property for MI and SQL DB</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-1071">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1071">Storage</span></span>

* <span data-ttu-id="3c5b0-1072">az storage blob delete-batch: sinalizador `--dryrun` de comportamento inadequado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1072">az storage blob delete-batch: Misbehaving `--dryrun` flag</span></span>
* <span data-ttu-id="3c5b0-1073">az storage account network-rule add (correção de bug): a operação de adição deve ser idempotente</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1073">az storage account network-rule add (bug fix): add operation should be idempotent</span></span>
* <span data-ttu-id="3c5b0-1074">az storage account create/update: Adicionou suporte de preferência de roteamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1074">az storage account create/update: Add Routing Preference support</span></span>
* <span data-ttu-id="3c5b0-1075">Atualizou a versão do azure-mgmt-storage para 8.0.0</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1075">Upgrade azure-mgmt-storage version to 8.0.0</span></span>
* <span data-ttu-id="3c5b0-1076">az storage container immutability create: adicionou o parâmetro --allow-protected-append-write</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1076">az storage container immutability create: add --allow-protected-append-write parameter</span></span>
* <span data-ttu-id="3c5b0-1077">az storage account private-link-resource list: Adicionou suporte para lista de recursos de link privado para a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1077">az storage account private-link-resource list: Add support to list private link resources for storage account</span></span>
* <span data-ttu-id="3c5b0-1078">az storage account private-endpoint-connection approve/reject/show/delete: Suporte para gerenciar conexões de ponto de extremidade privado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1078">az storage account private-endpoint-connection approve/reject/show/delete: Support to manage private endpoint connections</span></span>
* <span data-ttu-id="3c5b0-1079">az storage account blob-service-properties update: adicionou --enable-restore-policy e --restore-days</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1079">az storage account blob-service-properties update: add --enable-restore-policy and --restore-days</span></span>
* <span data-ttu-id="3c5b0-1080">az storage blob restore: adicionou suporte para restaurar intervalos de blob</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1080">az storage blob restore: Add support to restore blob ranges</span></span>

## <a name="february-18-2020"></a><span data-ttu-id="3c5b0-1081">18 de fevereiro de 2020</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1081">February 18, 2020</span></span>

<span data-ttu-id="3c5b0-1082">Versão 2.1.0</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1082">Version 2.1.0</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-1083">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1083">ACR</span></span>

* <span data-ttu-id="3c5b0-1084">Adicionar um novo argumento `--expose-token` a `az acr login`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1084">Add a new argument `--expose-token` for `az acr login`</span></span>
* <span data-ttu-id="3c5b0-1085">Corrigir a saída incorreta de `az acr task identity show -n Name -r Registry -o table`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1085">Fix the incorrect output of `az acr task identity show -n Name -r Registry -o table`</span></span>
* <span data-ttu-id="3c5b0-1086">az acr login: Gerar CLIError se erros forem retornados pelo comando docker</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1086">az acr login: Throw a CLIError if there are errors returned by docker command</span></span>

### <a name="acs"></a><span data-ttu-id="3c5b0-1087">ACS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1087">ACS</span></span>

* <span data-ttu-id="3c5b0-1088">aks create/update: adicionar a validação `--vnet-subnet-id`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1088">aks create/update: add `--vnet-subnet-id` validation</span></span>

### <a name="aladdin"></a><span data-ttu-id="3c5b0-1089">Aladdin</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1089">Aladdin</span></span>

* <span data-ttu-id="3c5b0-1090">Analisar os exemplos gerados no _help.py do comando</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1090">Parse generated examples into commands' _help.py</span></span>

### <a name="ams"></a><span data-ttu-id="3c5b0-1091">AMS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1091">AMS</span></span>

* <span data-ttu-id="3c5b0-1092">az ams já está em GA</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1092">az ams is GA now</span></span>

### <a name="appconfig"></a><span data-ttu-id="3c5b0-1093">AppConfig</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1093">AppConfig</span></span>

* <span data-ttu-id="3c5b0-1094">Revisar a mensagem de ajuda para excluir o filtro de chave/rótulo não compatível</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1094">Revise help message to exclude unsupported key/label filter</span></span>
* <span data-ttu-id="3c5b0-1095">Remover a marca de versão prévia da maioria dos comandos que excluem a identidade gerenciada e têm sinalizadores</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1095">Remove preview tag for most commands excluding managed identity and feature flags</span></span>
* <span data-ttu-id="3c5b0-1096">Adicionar a chave gerenciada do cliente ao atualizar os repositórios</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1096">Add customer managed key when updating stores</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-1097">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1097">AppService</span></span>

* <span data-ttu-id="3c5b0-1098">az webapp list-runtimes: Corrigir o bug de list-runtimes</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1098">az webapp list-runtimes: Fix the bug for list-runtimes</span></span>
* <span data-ttu-id="3c5b0-1099">Adicionar az webapp|functionapp config ssl create</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1099">Add az webapp|functionapp config ssl create</span></span>
* <span data-ttu-id="3c5b0-1100">Adicionar compatibilidade com aplicativos de funções v3 e nó 12</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1100">Add support for v3 function apps and node 12</span></span>

### <a name="arm"></a><span data-ttu-id="3c5b0-1101">ARM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1101">ARM</span></span>

* <span data-ttu-id="3c5b0-1102">az policy assignment create: Corrigir a mensagem de erro quando o parâmetro `--policy` for inválido</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1102">az policy assignment create: Fix the error message when the `--policy` parameter is invalid</span></span>
* <span data-ttu-id="3c5b0-1103">az group deployment create: Corrigir o erro "stat: o caminho é muito longo para o Windows" ao usar o arquivo grande parameters.json</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1103">az group deployment create: Fix "stat: path too long for Windows" error when using large parameters.json file</span></span>

### <a name="backup"></a><span data-ttu-id="3c5b0-1104">Backup</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1104">Backup</span></span>

* <span data-ttu-id="3c5b0-1105">Corrigir o fluxo de recuperação de nível de item no OLR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1105">Fix for item level recovery flow in OLR</span></span>
* <span data-ttu-id="3c5b0-1106">Adicionar compatibilidade com restauração como arquivo aos bancos de dados SQL e SAP</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1106">Add restore as files support for SQL and SAP Databases</span></span>

### <a name="compute"></a><span data-ttu-id="3c5b0-1107">Computação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1107">Compute</span></span>

* <span data-ttu-id="3c5b0-1108">vm/vmss/availability-set update: adicionar --ppg para permitir a atualização de ProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1108">vm/vmss/availability-set update: add --ppg to allowing updating ProximityPlacementGroup</span></span>
* <span data-ttu-id="3c5b0-1109">vmss create: adicionar --data-disk-iops e --data-disk-mbps</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1109">vmss create: add --data-disk-iops and --data-disk-mbps</span></span>
* <span data-ttu-id="3c5b0-1110">az vm host: remover a marca de versão prévia de `vm host` e `vm host group`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1110">az vm host: remove preview tag for `vm host` and `vm host group`</span></span>
* <span data-ttu-id="3c5b0-1111">[ALTERAÇÃO SIGNIFICATIVA] Correção nº 10.728: `az vm create`: criar uma sub-rede automaticamente quando a vnet for especificada e não houver uma sub-rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1111">[BREAKING CHANGE] Fix #10728: `az vm create`: create subnet automatically if vnet is specified and subnet not exists</span></span>
* <span data-ttu-id="3c5b0-1112">Aumentar a robustez da lista de imagens de VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1112">Increase robustness of vm image list</span></span>

### <a name="eventhub"></a><span data-ttu-id="3c5b0-1113">Eventhub</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1113">Eventhub</span></span>

* <span data-ttu-id="3c5b0-1114">Compatibilidade com o Azure Stack para o perfil 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1114">Azure Stack support for 2019-03-01-hybrid profile</span></span>

### <a name="keyvault"></a><span data-ttu-id="3c5b0-1115">KeyVault</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1115">KeyVault</span></span>

* <span data-ttu-id="3c5b0-1116">az keyvault key create: adicionar um novo valor `import` ao parâmetro `--ops`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1116">az keyvault key create: add a new value `import` for parameter `--ops`</span></span>
* <span data-ttu-id="3c5b0-1117">az keyvault key list-versions: compatibilidade com o parâmetro `--id` para especificar chaves</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1117">az keyvault key list-versions: support parameter `--id` for specifying keys</span></span>
* <span data-ttu-id="3c5b0-1118">Compatibilidade com conexões de ponto de extremidade privado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1118">Support private endpoint connections</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-1119">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1119">Network</span></span>

* <span data-ttu-id="3c5b0-1120">Avançar para azure-mgmt-network 9.0.0</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1120">Bump to azure-mgmt-network 9.0.0</span></span>
* <span data-ttu-id="3c5b0-1121">az network private-link-service update/create: dá suporte a --enable-proxy-protocol</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1121">az network private-link-service update/create: support --enable-proxy-protocol</span></span>
* <span data-ttu-id="3c5b0-1122">Adicionar o recurso de Monitor de conexão V2</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1122">Add connection Monitor V2 feature</span></span>

### <a name="packaging"></a><span data-ttu-id="3c5b0-1123">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1123">Packaging</span></span>

* <span data-ttu-id="3c5b0-1124">[ALTERAÇÃO SIGNIFICATIVA] Fim da compatibilidade com o Python 2.7</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1124">[BREAKING CHANGE] Drop support for Python 2.7</span></span>

### <a name="profile"></a><span data-ttu-id="3c5b0-1125">Perfil</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1125">Profile</span></span>

* <span data-ttu-id="3c5b0-1126">Visualização: Adicionar novos atributos `homeTenantId` e `managedByTenants` às contas de assinatura.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1126">Preview: Add new attributes `homeTenantId` and `managedByTenants` to subscription accounts.</span></span> <span data-ttu-id="3c5b0-1127">Executar `az login` novamente para as alterações entrarem em vigor</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1127">Please re-run `az login` for the changes to take effect</span></span>
* <span data-ttu-id="3c5b0-1128">az login: Mostrar um aviso quando uma assinatura estiver listada de mais de um locatário e definir a primeira como padrão.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1128">az login: Show a warning when a subscription is listed from more than one tenants and default to the first one.</span></span> <span data-ttu-id="3c5b0-1129">Para selecionar um locatário específico ao acessar essa assinatura, inclua `--tenant` em `az login`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1129">To select a specific tenant when accessing this subscription, please include `--tenant` in `az login`</span></span>

### <a name="role"></a><span data-ttu-id="3c5b0-1130">Função</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1130">Role</span></span>

* <span data-ttu-id="3c5b0-1131">az role assignment create: Corrigir o erro em que atribuir uma função a uma entidade de serviço pelo nome de exibição gera um HTTP 400</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1131">az role assignment create: Fix the error that assigning a role to a service principal by display name yields a HTTP 400</span></span>

### <a name="sql"></a><span data-ttu-id="3c5b0-1132">SQL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1132">SQL</span></span>

* <span data-ttu-id="3c5b0-1133">Atualizar o cmdlet da Instância Gerenciada do SQL `az sql mi update` com dois novos parâmetros: nível e família</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1133">Update SQL Managed Instance cmdlet `az sql mi update` with two new parameters: tier and family</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-1134">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1134">Storage</span></span>

* <span data-ttu-id="3c5b0-1135">[ALTERAÇÃO DA FALHA] `az storage account create`: Alterar o tipo de conta de armazenamento padrão para StorageV2</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1135">[BREAKING CHANGE] `az storage account create`: Change default storage account kind to StorageV2</span></span>

## <a name="february-04-2020"></a><span data-ttu-id="3c5b0-1136">4 de fevereiro de 2020</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1136">February 04, 2020</span></span>

<span data-ttu-id="3c5b0-1137">Versão 2.0.81</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1137">Version 2.0.81</span></span>

### <a name="acs"></a><span data-ttu-id="3c5b0-1138">ACS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1138">ACS</span></span>

* <span data-ttu-id="3c5b0-1139">Adicionar suporte para definir portas alocadas de saída e tempos limite ociosos no balanceador de carga standard</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1139">Add support to set outbound allocated ports and idle timeouts on standard load balancer</span></span>
* <span data-ttu-id="3c5b0-1140">Atualizar para a versão da API 2019-11-01</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1140">Update to API Version 2019-11-01</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-1141">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1141">ACR</span></span>

* <span data-ttu-id="3c5b0-1142">A [ALTERAÇÃO DA FALHA] `az acr delete` será exibida</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1142">[BREAKING CHANGE] `az acr delete` will prompt</span></span>
* <span data-ttu-id="3c5b0-1143">A [ALTERAÇÃO SIGNIFICATIVA] 'az acr task delete’ será exibida</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1143">[BREAKING CHANGE] 'az acr task delete' will prompt</span></span>
* <span data-ttu-id="3c5b0-1144">Adicionar um novo grupo de comandos ‘az acr taskrun show/list/delete’ para o gerenciamento de taskrun</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1144">Add a new command group 'az acr taskrun show/list/delete' for taskrun management</span></span>

### <a name="aks"></a><span data-ttu-id="3c5b0-1145">AKS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1145">AKS</span></span>

* <span data-ttu-id="3c5b0-1146">Cada cluster obtém uma entidade de serviço separada para aprimorar o isolamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1146">Each cluster gets a separate service principal to improve isolation</span></span>

### <a name="appconfig"></a><span data-ttu-id="3c5b0-1147">AppConfig</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1147">AppConfig</span></span>

* <span data-ttu-id="3c5b0-1148">Dar suporte à importação/exportação de referências keyvault de/a appservice</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1148">Support import/export of keyvault references from/to appservice</span></span>
* <span data-ttu-id="3c5b0-1149">Dar suporte à importação/exportação de todos os rótulos de appconfig para appconfig</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1149">Support import/export of all labels from appconfig to appconfig</span></span>
* <span data-ttu-id="3c5b0-1150">Validar nomes de chave e recursos antes de configurar e importar</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1150">Validate key and feature names before setting and importing</span></span>
* <span data-ttu-id="3c5b0-1151">Exponha a modificação do sku para o repositório de configurações.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1151">Expose sku modification for configuration store.</span></span>
* <span data-ttu-id="3c5b0-1152">Adicione o grupo de comandos à identidade gerenciada.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1152">Add command group for managed identity.</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-1153">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1153">AppService</span></span>

* <span data-ttu-id="3c5b0-1154">Azure Stack: comandos de superfície no perfil de 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1154">Azure Stack: surface commands under the profile of 2019-03-01-hybrid</span></span>
* <span data-ttu-id="3c5b0-1155">functionapp: adicionar a capacidade de criar aplicativos de funções Java no Linux</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1155">functionapp: Add ability to create Java function apps in Linux</span></span>

### <a name="arm"></a><span data-ttu-id="3c5b0-1156">ARM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1156">ARM</span></span>

* <span data-ttu-id="3c5b0-1157">Correção de problema nº 10246: `az resource tag` falha quando o parâmetro `--ids` passado é a ID do grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1157">Fix issue #10246: `az resource tag` crashes when the parameter `--ids` passed in is resource group ID</span></span>
* <span data-ttu-id="3c5b0-1158">Correção de problema nº 11658: o comando `az group export` não é compatível com os parâmetros `--query` e `--output`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1158">Fix issue #11658: `az group export` command does not support `--query` and `--output` parameters</span></span>
* <span data-ttu-id="3c5b0-1159">Correção de problema nº 10279: O código de saída `az group deployment validate` é 0 quando a verificação falha</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1159">Fix issue #10279: The exit code of `az group deployment validate` is 0 when the verification fails</span></span>
* <span data-ttu-id="3c5b0-1160">Correção de problema nº 9916: aprimorar a mensagem de erro do conflito entre a marca e outras condições de filtro para o comando `az resource list`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1160">Fix issue #9916: Improve the error message of the conflict between tag and other filter conditions for `az resource list` command</span></span>
* <span data-ttu-id="3c5b0-1161">Adicionar novo parâmetro `--managed-by` para dar suporte à adição de informações managedBy para o comando `az group create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1161">Add new parameter `--managed-by` to support adding managedBy information for command `az group create`</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="3c5b0-1162">Red Hat OpenShift no Azure</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1162">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="3c5b0-1163">Adicionar o subgrupo `monitor` para gerenciar o monitoramento do Log Analytics no cluster do Red Hat OpensShift no Azure</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1163">Add `monitor` subgroup to manage Log Analytics monitoring in Azure Red Hat OpensShift cluster</span></span>

### <a name="botservice"></a><span data-ttu-id="3c5b0-1164">BotService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1164">BotService</span></span>

* <span data-ttu-id="3c5b0-1165">Correção de problema nº 11697: `az bot create` não é idempotente</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1165">Fix issue #11697: `az bot create` is not idempotent</span></span>
* <span data-ttu-id="3c5b0-1166">Alterar testes de correção de nomes para serem executados somente em modo Ao vivo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1166">Change name-correcting tests to run in Live-mode only</span></span>

### <a name="cdn"></a><span data-ttu-id="3c5b0-1167">CDN</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1167">CDN</span></span>

* <span data-ttu-id="3c5b0-1168">Adicionar suporte ao recurso rulesEngine</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1168">Add support for rulesEngine feature</span></span>
* <span data-ttu-id="3c5b0-1169">Adicionar o novo grupo de comandos ‘cdn endpoint rule’ para gerenciar regras</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1169">Add new commands group 'cdn endpoint rule' to manage rules</span></span>
* <span data-ttu-id="3c5b0-1170">Atualizar a versão azure-mgmt-cdn para a 4.0.0 para usar a versão da API 2019-04-15</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1170">Update azure-mgmt-cdn version to 4.0.0 to use api version 2019-04-15</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="3c5b0-1171">Gerenciador de Implantação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1171">Deployment Manager</span></span>

* <span data-ttu-id="3c5b0-1172">Adicione a operação de lista para todos os recursos.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1172">Add list operation for all resources.</span></span>
* <span data-ttu-id="3c5b0-1173">Aprimore o recurso de etapa do novo tipo de etapa.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1173">Enhance step resource for new step type.</span></span>
* <span data-ttu-id="3c5b0-1174">Atualize o pacote azure-mgmt-deploymentmanager para usar a versão 0.2.0.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1174">Update azure-mgmt-deploymentmanager package to use version 0.2.0.</span></span>

### <a name="iot"></a><span data-ttu-id="3c5b0-1175">IoT</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1175">IoT</span></span>

* <span data-ttu-id="3c5b0-1176">Substitua os comandos ‘IoT hub Job’.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1176">Deprecate 'IoT hub Job' commands.</span></span>

### <a name="iot-central"></a><span data-ttu-id="3c5b0-1177">Central da IoT</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1177">IoT Central</span></span>

* <span data-ttu-id="3c5b0-1178">Dê suporte à atualização/criação de aplicativos com o novo nome do SKU ST0, ST1, ST2.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1178">Support app creation/update with the new sku name ST0, ST1, ST2.</span></span>

### <a name="key-vault"></a><span data-ttu-id="3c5b0-1179">Key Vault</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1179">Key Vault</span></span>

* <span data-ttu-id="3c5b0-1180">Adicione um novo comando `az keyvault key download` para baixar chaves.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1180">Add a new command `az keyvault key download` for downloading keys.</span></span>

### <a name="misc"></a><span data-ttu-id="3c5b0-1181">Diversos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1181">Misc</span></span>

* <span data-ttu-id="3c5b0-1182">Correção nº 6371: dar suporte à conclusão da variável de nome de arquivo e de ambiente em Bash</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1182">Fix #6371: Support filename and environment variable completion in Bash</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-1183">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1183">Network</span></span>

* <span data-ttu-id="3c5b0-1184">Correção nº 2092: az network dns record-set add/remove: adicione um aviso quando record-set não é encontrado.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1184">Fix #2092: az network dns record-set add/remove: add warning when record-set is not found.</span></span> <span data-ttu-id="3c5b0-1185">No futuro, haverá suporte para um argumento extra para confirmar essa criação automática.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1185">In the future, an extra argument will be supported to confirm this auto creation.</span></span>

### <a name="policy"></a><span data-ttu-id="3c5b0-1186">Política</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1186">Policy</span></span>

* <span data-ttu-id="3c5b0-1187">Adicionar o novo comando `az policy metadata` para recuperar recursos avançados de metadados de política</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1187">Add new command `az policy metadata` to retrieve rich policy metadata resources</span></span>
* <span data-ttu-id="3c5b0-1188">`az policy remediation create`: Especifique se a conformidade deve ser reavaliada antes da correção com o parâmetro `--resource-discovery-mode`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1188">`az policy remediation create`: Specify whether compliance should be re-evaluated prior to remediation with the `--resource-discovery-mode` parameter</span></span>

### <a name="profile"></a><span data-ttu-id="3c5b0-1189">Perfil</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1189">Profile</span></span>

* <span data-ttu-id="3c5b0-1190">`az account get-access-token`: Adicionar parâmetro `--tenant` para adquirir o token do locatário diretamente, sem a necessidade de especificar uma assinatura</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1190">`az account get-access-token`: Add `--tenant` parameter to acquire token for the tenant directly, needless to specify a subscription</span></span>

### <a name="rbac"></a><span data-ttu-id="3c5b0-1191">RBAC</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1191">RBAC</span></span>

* <span data-ttu-id="3c5b0-1192">[ALTERAÇÃO SIGNIFICATIVA] Correção nº 11883: `az role assignment create`: o escopo vazio exibirá erro</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1192">[BREAKING CHANGE] Fix #11883: `az role assignment create`: empty scope will prompt error</span></span>

### <a name="security"></a><span data-ttu-id="3c5b0-1193">Segurança</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1193">Security</span></span>

* <span data-ttu-id="3c5b0-1194">Adicione novos comandos `az atp show` e `az atp update` para exibir e gerenciar configurações avançadas de proteção contra ameaças para contas de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1194">Add new commands `az atp show` and `az atp update` to view and manage advanced threat protection settings for storage accounts.</span></span>

### <a name="sql"></a><span data-ttu-id="3c5b0-1195">SQL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1195">SQL</span></span>

* <span data-ttu-id="3c5b0-1196">`sql dw create`: substitua os parâmetros `--zone-redundant` e `--read-replica-count`.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1196">`sql dw create`: deprecate `--zone-redundant` and `--read-replica-count` parameters.</span></span> <span data-ttu-id="3c5b0-1197">Esses parâmetros não se aplicam ao DataWarehouse.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1197">These parameters do not apply to DataWarehouse.</span></span>
* <span data-ttu-id="3c5b0-1198">[ALTERAÇÃO DA FALHA] `az sql db create`: Remova "WideWorldImportersStd" e "WideWorldImportersFull" como valores permitidos documentados para "az sql db create --sample-name".</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1198">[BREAKING CHANGE] `az sql db create`: Remove "WideWorldImportersStd" and "WideWorldImportersFull" as documented allowed values for "az sql db create --sample-name".</span></span> <span data-ttu-id="3c5b0-1199">Esses bancos de dados de exemplo sempre farão a criação falhar.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1199">These sample databases would always cause creation to fail.</span></span>
* <span data-ttu-id="3c5b0-1200">Adicione os novos comandos `sql db classification show/list/update/delete` e `sql db classification recommendation list/enable/disable` para gerenciar classificações de confidencialidade para bancos de dados SQL.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1200">Add New commands `sql db classification show/list/update/delete` and `sql db classification recommendation list/enable/disable` to manage sensitivity classifications for SQL databases.</span></span>
* <span data-ttu-id="3c5b0-1201">`az sql db audit-policy`: Correção para ações e grupos de auditoria vazios</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1201">`az sql db audit-policy`: Fix for empty audit actions and groups</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-1202">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1202">Storage</span></span>

* <span data-ttu-id="3c5b0-1203">Adicione um novo grupo de comandos `az storage share-rm` para usar o provedor de recursos Microsoft.Storage para operações de gerenciamento de compartilhamento de arquivo do Azure.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1203">Add a new command group `az storage share-rm` to use the Microsoft.Storage resource provider for Azure file share management operations.</span></span>
* <span data-ttu-id="3c5b0-1204">Correção de problema nº 11415: erro de permissão para `az storage blob update`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1204">Fix issue #11415: permission error for `az storage blob update`</span></span>
* <span data-ttu-id="3c5b0-1205">Integre Azcopy 10.3.3 e dê suporte a Win32.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1205">Integrate Azcopy 10.3.3 and support Win32.</span></span>
* <span data-ttu-id="3c5b0-1206">`az storage copy`: Adicione os parâmetros `--include-path`, `--include-pattern`, `--exclude-path` e `--exclude-pattern`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1206">`az storage copy`: Add `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="3c5b0-1207">`az storage remove`: Altere os parâmetros `--inlcude` e `--exclude` para os parâmetros `--include-path`, `--include-pattern`, `--exclude-path` e `--exclude-pattern`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1207">`az storage remove`: Change `--inlcude` and `--exclude` parameters to `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="3c5b0-1208">`az storage sync`: Adicione os parâmetros `--include-pattern`, `--exclude-path` e `--exclude-pattern`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1208">`az storage sync`: Add `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>

### <a name="servicefabric"></a><span data-ttu-id="3c5b0-1209">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1209">ServiceFabric</span></span>

* <span data-ttu-id="3c5b0-1210">Adicione novos comandos para gerenciar o aplicativo e os serviços.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1210">Add new commands to manage appliaction and services.</span></span>

## <a name="january-13-2020"></a><span data-ttu-id="3c5b0-1211">13 de janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1211">January 13, 2020</span></span>

<span data-ttu-id="3c5b0-1212">Versão 2.0.80</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1212">Version 2.0.80</span></span>

### <a name="compute"></a><span data-ttu-id="3c5b0-1213">Computação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1213">Compute</span></span>

* <span data-ttu-id="3c5b0-1214">atualização do disco: Adicionar --disk-encryption-set e --encryption-type</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1214">disk update: Add --disk-encryption-set and --encryption-type</span></span>
* <span data-ttu-id="3c5b0-1215">criação/atualização do instantâneo: Adicionar --disk-encryption-set e --encryption-type</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1215">snapshot create/update: Add --disk-encryption-set and --encryption-type</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-1216">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1216">Storage</span></span>

* <span data-ttu-id="3c5b0-1217">Atualizar a versão do azure-mgmt-storage para 7.1.0</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1217">Upgrade azure-mgmt-storage version to 7.1.0</span></span>
* <span data-ttu-id="3c5b0-1218">`az storage account create`: Adicionar `--encryption-key-type-for-table` e `--encryption-key-type-for-queue` para dar suporte ao Serviço de Criptografia de Tabela e de Fila</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1218">`az storage account create`: Add `--encryption-key-type-for-table` and `--encryption-key-type-for-queue` to support Table and Queue Encryption Service</span></span>

## <a name="january-07-2020"></a><span data-ttu-id="3c5b0-1219">07 de janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1219">January 07, 2020</span></span>

<span data-ttu-id="3c5b0-1220">Versão 2.0.79</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1220">Version 2.0.79</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-1221">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1221">ACR</span></span>

* <span data-ttu-id="3c5b0-1222">[ALTERAÇÃO SIGNIFICATIVA] Remover o parâmetro '--os' para 'acr build', 'acr task create/update', 'acr run' e 'acr pack'.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1222">[BREAKING CHANGE] Remove '--os' parameter for 'acr build', 'acr task create/update', 'acr run', and 'acr pack'.</span></span> <span data-ttu-id="3c5b0-1223">Em vez disso, use '--platform'.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1223">Use '--platform' instead.</span></span>

### <a name="appconfig"></a><span data-ttu-id="3c5b0-1224">AppConfig</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1224">AppConfig</span></span>

* <span data-ttu-id="3c5b0-1225">Adicionar suporte para importar/exportar sinalizadores de recurso</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1225">Add support for importing/exporting feature flags</span></span>
* <span data-ttu-id="3c5b0-1226">Adicione o novo comando 'az appconfig kv set-keyvault' para criar a referência do keyvault</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1226">Add new command 'az appconfig kv set-keyvault' for creating keyvault reference</span></span>
* <span data-ttu-id="3c5b0-1227">Suporte a várias convenções de nomenclatura ao exportar os sinalizadores de recurso para o arquivo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1227">Support various naming conventions when exporting feature flags to file</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-1228">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1228">AppService</span></span>

* <span data-ttu-id="3c5b0-1229">Corrigir o problema #7154: Atualizar a documentação para o comando <> para usar acentos grave em vez de aspas simples</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1229">Fix issue #7154: Updating documentation for command <> to use back ticks instead of single quotes</span></span>
* <span data-ttu-id="3c5b0-1230">Corrigir o problema #11287: webapp up: Por padrão, faça o aplicativo criado usando 'should be 'SSL enabled'</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1230">Fix issue #11287: webapp up: By default make the app created using up 'should be 'SSL enabled'</span></span>
* <span data-ttu-id="3c5b0-1231">Corrigir o problema #11592: Adicionar o sinalizador az webapp up para sites HTML estáticos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1231">Fix issue #11592: Add az webapp up flag for html static sites</span></span>

### <a name="arm"></a><span data-ttu-id="3c5b0-1232">ARM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1232">ARM</span></span>

* <span data-ttu-id="3c5b0-1233">Corrigir `az resource tag`: As marcas do Cofre dos Serviços de Recuperação não podem ser atualizadas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1233">Fix `az resource tag`: Recovery Services Vault tags cannot be updated</span></span>

### <a name="backup"></a><span data-ttu-id="3c5b0-1234">Backup</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1234">Backup</span></span>

* <span data-ttu-id="3c5b0-1235">Novo comando 'backup protection undelete' adicionado para habilitar o recurso de exclusão reversível para carga de trabalho IaasVM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1235">Added new command 'backup protection undelete' to enable soft-delete feature for IaasVM workload</span></span>
* <span data-ttu-id="3c5b0-1236">Novo parâmetro '--soft-delete-feature-state' adicionado para definir o comando propriedades do backup</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1236">Added new parameter '--soft-delete-feature-state' to set backup-properties command</span></span>
* <span data-ttu-id="3c5b0-1237">Suporte de exclusão de disco adicionado para carga de trabalho IaasVM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1237">Added disk exclusion support for IaasVM workload</span></span>

### <a name="compute"></a><span data-ttu-id="3c5b0-1238">Computação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1238">Compute</span></span>

* <span data-ttu-id="3c5b0-1239">Corrigir a falha `vm create` no perfil do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1239">Fix `vm create` failure in Azure Stack profile.</span></span>
* <span data-ttu-id="3c5b0-1240">parte final/listar definições de métricas de monitor de vm: suporte a métricas de consulta e definições de lista para uma vm.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1240">vm monitor metrics tail/list-definitions: support query metric and list definitions for a vm.</span></span>
* <span data-ttu-id="3c5b0-1241">Adicionar nova ação de comando de reaplicação para az vm</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1241">Add new reapply command action for az vm</span></span>

### <a name="hdinsight"></a><span data-ttu-id="3c5b0-1242">HDInsight</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1242">HDInsight</span></span>

* <span data-ttu-id="3c5b0-1243">Suporte para criar um cluster Kafka com o Proxy REST do Kafka</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1243">Support for creating a Kafka cluster with Kafka Rest Proxy</span></span>
* <span data-ttu-id="3c5b0-1244">Atualizar azure-mgmt-hdinsight para 1.3.0</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1244">Upgrade azure-mgmt-hdinsight to 1.3.0</span></span>

### <a name="misc"></a><span data-ttu-id="3c5b0-1245">Diversos.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1245">Misc.</span></span>

* <span data-ttu-id="3c5b0-1246">Adicionar comando de visualização `az version show` para mostrar as versões dos módulos e das extensões da CLI do Azure no formato JSON por padrão ou no formato configurado por --output</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1246">Add preview command `az version show` to show the versions of Azure CLI modules and extensions in JSON format by default or format configured by --output</span></span>

### <a name="event-hubs"></a><span data-ttu-id="3c5b0-1247">Hubs de Eventos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1247">Event Hubs</span></span>

* <span data-ttu-id="3c5b0-1248">[ALTERAÇÃO SIGNIFICATIVA] Remover a opção de status 'ReceiveDisabled' do comando 'az eventhubs eventhub update' e 'az eventhubs eventhub create'.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1248">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az eventhubs eventhub update' and 'az eventhubs eventhub create'.</span></span> <span data-ttu-id="3c5b0-1249">Essa opção não é válida para entidades do Hub de Eventos.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1249">This option is not valid for Event Hub entities.</span></span>

### <a name="service-bus"></a><span data-ttu-id="3c5b0-1250">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1250">Service Bus</span></span>

* <span data-ttu-id="3c5b0-1251">[ALTERAÇÃO SIGNIFICATIVA] Remover a opção de status 'ReceiveDisabled' do comando 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create' e 'az servicebus queue update'.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1251">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create', and 'az servicebus queue update'.</span></span> <span data-ttu-id="3c5b0-1252">Essa opção não é válida para tópicos e filas do Barramento de Serviço.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1252">This option is not valid for Service Bus topics and queues.</span></span>

### <a name="rbac"></a><span data-ttu-id="3c5b0-1253">RBAC</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1253">RBAC</span></span>

* <span data-ttu-id="3c5b0-1254">Correção #11712: `az ad app/sp show` não devolve o código de saída 3 quando o aplicativo ou a entidade de serviço não existir</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1254">Fix #11712: `az ad app/sp show` does not return exit code 3 when the application or service principal does not exist</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-1255">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1255">Storage</span></span>

* <span data-ttu-id="3c5b0-1256">`az storage account create`: Remover o sinalizador de visualização do parâmetro --enable-hierarchical-namespace</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1256">`az storage account create`: Remove preview flag for --enable-hierarchical-namespace parameter</span></span>
* <span data-ttu-id="3c5b0-1257">Atualizar a versão azure-mgmt-storage para 7.0.0 para usar a versão de API 2019-06-01</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1257">Update azure-mgmt-storage version to 7.0.0 to use api version 2019-06-01</span></span>
* <span data-ttu-id="3c5b0-1258">Adicionar novos parâmetros `--enable-delete-retention` e `--delete-retention-days` para dar suporte ao gerenciamento da política de retenção de exclusão para a conta de armazenamento blob-service-properties.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1258">Add new parameters `--enable-delete-retention` and `--delete-retention-days` to support managing delete retention policy for storage account blob-service-properties.</span></span>

## <a name="december-17-2019"></a><span data-ttu-id="3c5b0-1259">17 de dezembro de 2019</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1259">December 17, 2019</span></span>

<span data-ttu-id="3c5b0-1260">2.0.78</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1260">2.0.78</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-1261">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1261">ACR</span></span>

* <span data-ttu-id="3c5b0-1262">Contexto local de suporte adicionado na execução da tarefa acr</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1262">Added support Local context in acr task run</span></span>

### <a name="acs"></a><span data-ttu-id="3c5b0-1263">ACS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1263">ACS</span></span>

* <span data-ttu-id="3c5b0-1264">[ALTERAÇÃO SIGNIFICATIVA]criar az openshift: renomear `--workspace-resource-id` para `--workspace-id`.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1264">[BREAKING CHANGE]az openshift create: rename `--workspace-resource-id` to `--workspace-id`.</span></span>

### <a name="ams"></a><span data-ttu-id="3c5b0-1265">AMS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1265">AMS</span></span>

* <span data-ttu-id="3c5b0-1266">Comandos de exibição atualizados para devolver 3 quando o recurso não for encontrado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1266">Updated show commands to return 3 when resource not found</span></span>

### <a name="appconfig"></a><span data-ttu-id="3c5b0-1267">AppConfig</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1267">AppConfig</span></span>

* <span data-ttu-id="3c5b0-1268">Bug corrigido ao acrescentar a versão de API à URL de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1268">Fixed bug when appending api-version to request url.</span></span> <span data-ttu-id="3c5b0-1269">A solução existente não funciona com a paginação.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1269">The existing solution doesn't work with pagination.</span></span>
* <span data-ttu-id="3c5b0-1270">Suporte adicionado para a exibição de idiomas além do inglês, pois nosso serviço de back-end é compatível com unicode para globalização.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1270">Added support for showing languages besides English as our backend service support unicode for globalization.</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-1271">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1271">AppService</span></span>

* <span data-ttu-id="3c5b0-1272">Problema corrigido nº 11217: webapp: o upload ssl de configuração do az webapp deve ser compatível com o parâmetro do slot</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1272">Fixed issue #11217: webapp: az webapp config ssl upload should support slot parameter</span></span>
* <span data-ttu-id="3c5b0-1273">Problema corrigido nº 10965: Erro: O nome não pode estar vazio.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1273">Fixed issue #10965: Error: Name cannot be empty.</span></span> <span data-ttu-id="3c5b0-1274">Permitir remoção por ip_address e sub-rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1274">Allow remove by ip_address and subnet</span></span>
* <span data-ttu-id="3c5b0-1275">Suporte adicionado para importar certificados do Key Vault `az webapp config ssl import`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1275">Added support for importing certificates from Key Vault `az webapp config ssl import`</span></span>

### <a name="arm"></a><span data-ttu-id="3c5b0-1276">ARM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1276">ARM</span></span>

* <span data-ttu-id="3c5b0-1277">Pacote azure-mgmt-resource atualizado para usar 6.0.0</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1277">Updated azure-mgmt-resource package to use 6.0.0</span></span>
* <span data-ttu-id="3c5b0-1278">Suporte entre locatários para o comando `az group deployment create` adicionando o novo parâmetro `--aux-subs`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1278">Cross Tenant Support for `az group deployment create` command by adding new parameter `--aux-subs`</span></span>
* <span data-ttu-id="3c5b0-1279">Novo parâmetro `--metadata` adicionado para dar suporte à adição de informações de metadados para definições de conjunto de políticas.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1279">Added new parameter `--metadata` to support adding metadata information for policy set definitions.</span></span>

### <a name="backup"></a><span data-ttu-id="3c5b0-1280">Backup</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1280">Backup</span></span>

* <span data-ttu-id="3c5b0-1281">Suporte de backup adicionado para carga de trabalho SQL e SAP Hana.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1281">Added Backup support for SQL and SAP Hana workload.</span></span>

### <a name="botservice"></a><span data-ttu-id="3c5b0-1282">BotService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1282">BotService</span></span>

* <span data-ttu-id="3c5b0-1283">[ALTERAÇÃO SIGNIFICATIVA] Remover o sinalizador '--version ' do comando de visualização 'az bot create'.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1283">[Breaking change] Remove '--version' flag from preview command 'az bot create'.</span></span> <span data-ttu-id="3c5b0-1284">Somente os bots do SDK v4 são compatíveis.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1284">Only v4 SDK bots are supported.</span></span>
* <span data-ttu-id="3c5b0-1285">Verificação de disponibilidade de nome adicionada para 'az bot create'.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1285">Added name availability check for 'az bot create'.</span></span>
* <span data-ttu-id="3c5b0-1286">Suporte adicionado para atualizar a URL do ícone para um bot por meio de 'az bot update'.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1286">Added support for updating the icon URL for a bot via 'az bot update'.</span></span>
* <span data-ttu-id="3c5b0-1287">Suporte adicionado para atualizar um canal Direct Line por meio de 'az bot directline update'.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1287">Added support for updating a Direct Line channel via 'az bot directline update'.</span></span>
* <span data-ttu-id="3c5b0-1288">Suporte ao sinalizador '--enable-enhanced-auth' adicionado para 'az bot directline create'.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1288">Added '--enable-enhanced-auth' flag support to 'az bot directline create'.</span></span>
* <span data-ttu-id="3c5b0-1289">Os seguintes grupos de comandos estão em GA e não estão em versão prévia: 'az bot authsetting'.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1289">The following command groups are GA and not in preview: 'az bot authsetting'.</span></span>
* <span data-ttu-id="3c5b0-1290">Os seguintes comandos em 'az bot' estão em GA e não na versão prévia: 'criar', 'preparar-implantar', 'mostrar', 'excluir', 'atualizar'.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1290">The following commands in 'az bot' are GA and not in preview: 'create', 'prepare-deploy', 'show', 'delete', 'update'.</span></span>
* <span data-ttu-id="3c5b0-1291">Correção do valor 'az bot prepare-deploy' alterando '--proj-file-path ' para letras minúsculas (por exemplo, "Test. csproj" para "Test. csproj").</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1291">Fixed 'az bot prepare-deploy' changing '--proj-file-path' value to lower case (e.g. "Test.csproj" to "test.csproj").</span></span>

### <a name="compute"></a><span data-ttu-id="3c5b0-1292">Computação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1292">Compute</span></span>

* <span data-ttu-id="3c5b0-1293">Criar/atualizar vmss: --scale-in-policy adicionado, que decide quais máquinas virtuais são escolhidas para remoção quando um VMSS é dimensionado.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1293">vmss create/update: Added --scale-in-policy, which decides which virtual machines are chosen for removal when a VMSS is scaled-in.</span></span>
* <span data-ttu-id="3c5b0-1294">atualização de vm/vmss: --priority adicionado.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1294">vm/vmss update: Added --priority.</span></span>
* <span data-ttu-id="3c5b0-1295">atualização de vm/vmss: --max-price adicionado.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1295">vm/vmss update: Added --max-price.</span></span>
* <span data-ttu-id="3c5b0-1296">Grupo de comandos do conjunto de criptografia de disco adicionado (criar, mostrar, atualizar, excluir e listar).</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1296">Added disk-encryption-set command group (create, show, update, delete, list).</span></span>
* <span data-ttu-id="3c5b0-1297">criação de disco: --encryption-type e --disk-encryption-set adicionados.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1297">disk create: Added --encryption-type and --disk-encryption-set.</span></span>
* <span data-ttu-id="3c5b0-1298">vm/vmss create: --os-disk-encryption-set e --data-disk-encryption-sets adicionados.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1298">vm/vmss create: Added --os-disk-encryption-set and --data-disk-encryption-sets.</span></span>

### <a name="core"></a><span data-ttu-id="3c5b0-1299">Núcleo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1299">Core</span></span>

* <span data-ttu-id="3c5b0-1300">Suporte para Python 3.4 removido</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1300">Removed support for Python 3.4</span></span>
* <span data-ttu-id="3c5b0-1301">Pesquisa de funções de plug-in em vários comandos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1301">Plug in HaTS survey in multiple commands</span></span>

### <a name="dls"></a><span data-ttu-id="3c5b0-1302">DLS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1302">DLS</span></span>

* <span data-ttu-id="3c5b0-1303">Versão atualizada do SDK do ADLS (0.0.48).</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1303">Updated ADLS sdk version (0.0.48).</span></span>

### <a name="install"></a><span data-ttu-id="3c5b0-1304">Instalar</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1304">Install</span></span>

* <span data-ttu-id="3c5b0-1305">Instalar suporte de script Python 3.8</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1305">Install script support python 3.8</span></span>

### <a name="iot"></a><span data-ttu-id="3c5b0-1306">IOT</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1306">IOT</span></span>

* <span data-ttu-id="3c5b0-1307">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro--failover-region removido de failover manual.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1307">[BREAKING CHANGE] Removed --failover-region parameter from manual-failover.</span></span> <span data-ttu-id="3c5b0-1308">Agora ele fará failover para a região secundária emparelhada atribuída geograficamente.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1308">Now it will failover to assigned geo-paired secondary region.</span></span>

### <a name="key-vault"></a><span data-ttu-id="3c5b0-1309">Key Vault</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1309">Key Vault</span></span>

* <span data-ttu-id="3c5b0-1310">Nº 8095 corrigido: `az keyvault storage remove`: melhorar a mensagem de ajuda</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1310">Fixed #8095: `az keyvault storage remove`: improve the help message</span></span>
* <span data-ttu-id="3c5b0-1311">Nº 8921 corrigido: `az keyvault key/secret/certificate list/list-deleted/list-versions`: corrigir o bug de validação no parâmetro `--maxresults`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1311">Fixed #8921: `az keyvault key/secret/certificate list/list-deleted/list-versions`: fix the validation bug on parameter `--maxresults`</span></span>
* <span data-ttu-id="3c5b0-1312">Nº 10512 corrigido: `az keyvault set-policy`: melhorar a mensagem de erro quando nenhuma das `--object-id`, `--spn` ou `--upn` for especificada</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1312">Fixed #10512: `az keyvault set-policy`: improve the error message when none of `--object-id`, `--spn` or `--upn` is specified</span></span>
* <span data-ttu-id="3c5b0-1313">Nº 10846 corrigido: `az keyvault secret show-deleted`: quando `--id` for especificado, `--name/-n` não será necessário</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1313">Fixed #10846: `az keyvault secret show-deleted`: when `--id` is specified, `--name/-n` is not required</span></span>
* <span data-ttu-id="3c5b0-1314">Nº 11084 corrigido: `az keyvault secret download`: melhorar a mensagem de ajuda do parâmetro `--encoding`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1314">Fixed #11084: `az keyvault secret download`: improve the help message of parameter `--encoding`</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-1315">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1315">Network</span></span>

* <span data-ttu-id="3c5b0-1316">Investigação de gateway de aplicativo de rede az: Suporte --port option adicionado para especificar uma porta para sondar servidores de back-end ao criar e atualizar</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1316">az network application-gateway probe: Added support --port option to specify a port for probing backend servers when create and update</span></span>
* <span data-ttu-id="3c5b0-1317">az network application-gateway url-path-map create/update: correção de bug para `--waf-policy`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1317">az network application-gateway url-path-map create/update: bug fix for `--waf-policy`</span></span>
* <span data-ttu-id="3c5b0-1318">az network application-gateway: Suporte `--rewrite-rule-set` adicionado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1318">az network application-gateway: Added support `--rewrite-rule-set`</span></span>
* <span data-ttu-id="3c5b0-1319">az network list-service-aliases: Foram adicionados aliases de serviço da lista de suporte que podem ser usados para políticas de ponto de extremidade de serviço</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1319">az network list-service-aliases: Added support list service aliases which can be used for Service Endpoint Policies</span></span>
* <span data-ttu-id="3c5b0-1320">importar zona dns da rede az: Suporte adicionado. @ no nome do registro</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1320">az network dns zone import: Added support .@ in record name</span></span>

### <a name="packaging"></a><span data-ttu-id="3c5b0-1321">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1321">Packaging</span></span>

* <span data-ttu-id="3c5b0-1322">Compilações de back edge adicionadas para instalação de pip</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1322">Added back edge builds for pip install</span></span>
* <span data-ttu-id="3c5b0-1323">Pacote eoan do Ubuntu adicionado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1323">Added Ubuntu eoan package</span></span>

### <a name="policy"></a><span data-ttu-id="3c5b0-1324">Política</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1324">Policy</span></span>

* <span data-ttu-id="3c5b0-1325">Inclusão de compatibilidade com a API de Política, versão de 01/09/2019.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1325">Added support for Policy API version 2019-09-01.</span></span>
* <span data-ttu-id="3c5b0-1326">az policy set-definition: Agrupamento de suporte adicionado nas definições do conjunto de políticas com `--definition-groups` parâmetro</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1326">az policy set-definition: Added support grouping within policy set definitions with `--definition-groups` parameter</span></span>

### <a name="redis"></a><span data-ttu-id="3c5b0-1327">Redis</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1327">Redis</span></span>

* <span data-ttu-id="3c5b0-1328">Adicionado o parâmetro de visualização `--replicas-per-master` ao comando `az redis create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1328">Added preview param `--replicas-per-master` to `az redis create` command</span></span>
* <span data-ttu-id="3c5b0-1329">Azure-MGMT-Redis adicionado do 6.0.0 para o 7.0.0rc1</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1329">Updated azure-mgmt-redis from 6.0.0 to 7.0.0rc1</span></span>

### <a name="servicefabric"></a><span data-ttu-id="3c5b0-1330">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1330">ServiceFabric</span></span>

* <span data-ttu-id="3c5b0-1331">Corrigido em nó-tipo adicionar lógica, incluindo #10963: A adição do novo tipo de nó com nível de durabilidade Gold sempre gerará erro da CLI</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1331">Fixed in node-type add logic including #10963: Adding new node type with durability level Gold will always throw CLI error</span></span>
* <span data-ttu-id="3c5b0-1332">Versão do ServiceFabricNodeVmExt atualizada para 1.1 no modelo de criação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1332">Updated ServiceFabricNodeVmExt version to 1.1 in creation template</span></span>

### <a name="sql"></a><span data-ttu-id="3c5b0-1333">SQL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1333">SQL</span></span>

* <span data-ttu-id="3c5b0-1334">Adicionados os parâmetros "--read-scale" e "--read-replicas" aos comandos criar e atualizar do BD SQL para dar suporte ao gerenciamento de escala de leitura.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1334">Added "--read-scale" and "--read-replicas" parameters to sql db create and update commands, to support read scale management.</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-1335">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1335">Storage</span></span>

* <span data-ttu-id="3c5b0-1336">Propriedade de compartilhamentos de arquivos grandes da versão GA para o comando criar e atualizar da conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1336">GA Release Large File Shares property for storage account create and update command</span></span>
* <span data-ttu-id="3c5b0-1337">Suporte ao token SAS de delegação de usuário da versão GA</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1337">GA Release User Delegation SAS token Support</span></span>
* <span data-ttu-id="3c5b0-1338">Novos comandos adicionados `az storage account blob-service-properties show` e `az storage account blob-service-properties update --enable-change-feed` para gerenciar Propriedades do serviço blob para a conta de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1338">Added new commands `az storage account blob-service-properties show` and `az storage account blob-service-properties update --enable-change-feed` to manage blob service properties for storage account.</span></span>
* <span data-ttu-id="3c5b0-1339">[PRÓXIMA ALTERAÇÃO DA FALHA] `az storage copy`: `*` não há mais suporte para o caractere de como um curinga na URL, mas novos parâmetros--include-pattern e --exclude-pattern serão adicionados com suporte a curinga `*`.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1339">[COMING BREAKING CHANGE] `az storage copy`: `*` character is no longer supported as a wildcard in URL, but new parameters --include-pattern and --exclude-pattern will be added with `*` wildcard support.</span></span>
* <span data-ttu-id="3c5b0-1340">Problema corrigido nº 11043: Suporte adicionado para remover contêiner/compartilhamento inteiro no comando `az storage remove`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1340">Fixed issue #11043: Added support to remove whole container/share in `az storage remove` command</span></span>

## <a name="november-26-2019"></a><span data-ttu-id="3c5b0-1341">26 de novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1341">November 26, 2019</span></span>

<span data-ttu-id="3c5b0-1342">Versão 2.0.77</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1342">Version 2.0.77</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-1343">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1343">ACR</span></span>

* <span data-ttu-id="3c5b0-1344">Parâmetro `--branch` preterido da criação/atualização da tarefa ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1344">Deprecated parameter `--branch` from acr task create/update</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="3c5b0-1345">Red Hat OpenShift no Azure</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1345">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="3c5b0-1346">Sinalizador `--workspace-resource-id` adicionado para permitir a criação do cluster do Red Hat OpenShift no Azure com monitoramento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1346">Added `--workspace-resource-id` flag to allow creation of Azure Red Hat Openshift cluster with monitoring</span></span>
* <span data-ttu-id="3c5b0-1347">`monitor_profile` adicionado para criar o cluster do Red Hat OpenShift no Azure com monitoramento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1347">Added `monitor_profile` to create Azure Red Hat OpenShift cluster with monitoring</span></span>

### <a name="aks"></a><span data-ttu-id="3c5b0-1348">AKS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1348">AKS</span></span>

* <span data-ttu-id="3c5b0-1349">Operação de rotação de certificado de cluster de suporte adicionada usando "az aks rotate-certs".</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1349">Added support cluster certificate rotation operation using "az aks rotate-certs".</span></span>

### <a name="appconfig"></a><span data-ttu-id="3c5b0-1350">AppConfig</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1350">AppConfig</span></span>

* <span data-ttu-id="3c5b0-1351">Suporte adicionado para usar ":" para o separador `as az appconfig kv import`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1351">Added support for using ":" for `as az appconfig kv import` separator</span></span>
* <span data-ttu-id="3c5b0-1352">Problema corrigido para listar valores de chave com vários rótulos incluindo o rótulo nulo.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1352">Fixed issue for listing key values with multiple labels including null label.</span></span> 
* <span data-ttu-id="3c5b0-1353">SDK do plano de gerenciamento atualizado, azure-mgmt-appconfiguration, para a versão 0.3.0.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1353">Updated management plane sdk, azure-mgmt-appconfiguration, to version 0.3.0.</span></span> 

### <a name="appservice"></a><span data-ttu-id="3c5b0-1354">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1354">AppService</span></span>

* <span data-ttu-id="3c5b0-1355">Problema corrigido nº 11100: AttributeError para az webapp up ao criar o plano de serviço</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1355">Fixed issue #11100: AttributeError for az webapp up when create service plan</span></span>
* <span data-ttu-id="3c5b0-1356">az webapp up: Forçar a criação ou a implantação em um site para linguagens com suporte, nenhum padrão usado.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1356">az webapp up: Forcing the creation or deployment to a site for supported languages, no defaults used.</span></span>
* <span data-ttu-id="3c5b0-1357">Suporte adicionado para o Ambiente do Serviço de Aplicativo: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1357">Added support for App Service Environment: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span></span>

### <a name="backup"></a><span data-ttu-id="3c5b0-1358">Backup</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1358">Backup</span></span>

* <span data-ttu-id="3c5b0-1359">Problema corrigido em list-associated-items da política de backup az.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1359">Fixed issue in az backup policy list-associated-items.</span></span> <span data-ttu-id="3c5b0-1360">Parâmetro BackupManagementType opcional adicionado.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1360">Added optional BackupManagementType parameter.</span></span>

### <a name="compute"></a><span data-ttu-id="3c5b0-1361">Computação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1361">Compute</span></span>

* <span data-ttu-id="3c5b0-1362">Versão de API de computação, discos e instantâneos atualizados para 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1362">Upgraded API version of compute, disks, snapshots to 2019-07-01</span></span>
* <span data-ttu-id="3c5b0-1363">vmss create: melhoria para --orchestration-mode</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1363">vmss create: Improvement for --orchestration-mode</span></span>
* <span data-ttu-id="3c5b0-1364">sig image-definition create: --os-state adicionado para permitir a especificação se as máquinas virtuais criadas nessa imagem são 'Generalizadas' ou 'Especializadas'</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1364">sig image-definition create: Added --os-state to allow specifying whether the virtual machines created under this image are 'Generalized' or 'Specialized'</span></span>
* <span data-ttu-id="3c5b0-1365">sig image-definition create: --hyper-v-generation adicionado para permitir a especificação da geração do hipervisor</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1365">sig image-definition create: Added --hyper-v-generation to allow specifying the hypervisor generation</span></span>
* <span data-ttu-id="3c5b0-1366">sig image-version create: --os-snapshot e --data-snapshots de suporte adicionados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1366">sig image-version create: Added support --os-snapshot and --data-snapshots</span></span>
* <span data-ttu-id="3c5b0-1367">image create: --data-disk-caching adicionado para permitir a especificação da configuração de cache de discos de dados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1367">image create: Added --data-disk-caching to allow specifying caching setting of data disks</span></span>
* <span data-ttu-id="3c5b0-1368">SDK de computação do Python atualizado para 10.0.0</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1368">Upgraded Python Compute SDK to 10.0.0</span></span>
* <span data-ttu-id="3c5b0-1369">vm/vmss create: 'Spot' adicionado à propriedade de enumeração 'Priority'</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1369">vm/vmss create: Added 'Spot' to 'Priority' enum property</span></span>
* <span data-ttu-id="3c5b0-1370">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro '--max-billing' renomeado para '--max-price', para a VM e o VMSS, a fim de que seja consistente com os cmdlets do Swagger e do PowerShell</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1370">[Breaking change] Renamed '--max-billing' parameter to '--max-price', for both VM and VMSS, to be consistent with Swagger and Powershell cmdlets</span></span>
* <span data-ttu-id="3c5b0-1371">vm monitor log show: suporte adicionado para consultar o log pelo workspace do Log Analytics vinculado.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1371">vm monitor log show: Added support for querying log over linked log analytics workspace.</span></span>

### <a name="iot"></a><span data-ttu-id="3c5b0-1372">IOT</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1372">IOT</span></span>

* <span data-ttu-id="3c5b0-1373">Correção nº 2531: argumentos de conveniência adicionados para a atualização do hub.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1373">Fix #2531: Added convenience arguments for hub update.</span></span>
* <span data-ttu-id="3c5b0-1374">Correção nº 8323: parâmetros ausentes adicionados para criar o ponto de extremidade personalizado de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1374">Fix #8323: Added missing parameters to create storage custom endpoint.</span></span>
* <span data-ttu-id="3c5b0-1375">Corrigir bug de regressão: as alterações que substituem o ponto de extremidade de armazenamento padrão foram revertidas.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1375">Fix regression bug: Reverted the changes which overrides the default storage endpoint.</span></span>

### <a name="key-vault"></a><span data-ttu-id="3c5b0-1376">Key Vault</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1376">Key Vault</span></span>

* <span data-ttu-id="3c5b0-1377">Correção nº 11121: ao usar `az keyvault certificate list`, passar `--include-pending` agora não exige um valor de `true` ou `false`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1377">Fixed #11121: When using `az keyvault certificate list`, passing `--include-pending` now doesn't require a value of `true` or `false`</span></span>

### <a name="netappfiles"></a><span data-ttu-id="3c5b0-1378">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1378">NetAppFiles</span></span>

* <span data-ttu-id="3c5b0-1379">azure-mgmt-netapp atualizado para 0.7.0 que inclui algumas propriedades de volume adicionais associadas a operações de replicação futuras</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1379">Upgraded azure-mgmt-netapp to 0.7.0 which includes some additional volume properties associated with upcoming replication operations</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-1380">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1380">Network</span></span>

* <span data-ttu-id="3c5b0-1381">application-gateway waf-config: preterido</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1381">application-gateway waf-config: deprecated</span></span>
* <span data-ttu-id="3c5b0-1382">application-gateway waf-policy: subgrupo managed-rules adicionado para gerenciar os conjuntos de regras e regras de exclusão gerenciados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1382">application-gateway waf-policy: Added subgroup managed-rules to manage managed rule sets and exclusion rules</span></span>
* <span data-ttu-id="3c5b0-1383">application-gateway waf-policy: subgrupo policy-setting adicionado para gerenciar a configuração global de um waf-policy</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1383">application-gateway waf-policy: Added subgroup policy-setting to manage global configuration of a waf-policy</span></span>
* <span data-ttu-id="3c5b0-1384">[ALTERAÇÃO SIGNIFICATIVA] application-gateway waf-policy: subgrupo rule renomeado para custom-rule</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1384">[BREAKING CHANGE] application-gateway waf-policy: Renamed subgroup rule to custom-rule</span></span>
* <span data-ttu-id="3c5b0-1385">application-gateway http-listener: --firewall-policy adicionado durante a criação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1385">application-gateway http-listener: Added --firewall-policy when create</span></span>
* <span data-ttu-id="3c5b0-1386">application-gateway url-path-map rule: --firewall-policy adicionado durante a criação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1386">application-gateway url-path-map rule: Added --firewall-policy when create</span></span>

### <a name="packaging"></a><span data-ttu-id="3c5b0-1387">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1387">Packaging</span></span>

* <span data-ttu-id="3c5b0-1388">Wrapper az reescrito no Python</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1388">Rewrote the az wrapper in Python</span></span>
* <span data-ttu-id="3c5b0-1389">Suporte adicionado para Python 3.8</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1389">Added support for Python 3.8</span></span>
* <span data-ttu-id="3c5b0-1390">Alterado para Python 3 para o pacote RPM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1390">Changed to Python 3 for RPM package</span></span>

### <a name="profile"></a><span data-ttu-id="3c5b0-1391">Perfil</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1391">Profile</span></span>

* <span data-ttu-id="3c5b0-1392">Erro aperfeiçoado ao executar `az login -u {} -p {}` com a conta Microsoft</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1392">Polished error when running `az login -u {} -p {}` with Microsoft account</span></span>
* <span data-ttu-id="3c5b0-1393">`SSLError` aperfeiçoado ao executar `az login` atrás de um proxy com o certificado raiz autoassinado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1393">Polished `SSLError` when running `az login` behind a proxy with self-signed root certificate</span></span>
* <span data-ttu-id="3c5b0-1394">Correção nº 10578: `az login` trava quando mais de uma instância é iniciada ao mesmo tempo no Windows ou WSL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1394">Fixed #10578: `az login` hangs when more than one instances are launched at the same time on Windows or WSL</span></span>
* <span data-ttu-id="3c5b0-1395">Correção nº 11059: `az login --allow-no-subscriptions` falhará se houver assinaturas no locatário</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1395">Fixed #11059: `az login --allow-no-subscriptions` fails if there are subscriptions in the tenant</span></span>
* <span data-ttu-id="3c5b0-1396">Correção nº 11238: após renomear uma assinatura, fazer logon com a MSI fará a mesma assinatura aparecer duas vezes</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1396">Fixed #11238: After renaming a subscription, logging in with MSI will result in the same subscription appearing twice</span></span>

### <a name="rbac"></a><span data-ttu-id="3c5b0-1397">RBAC</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1397">RBAC</span></span>

* <span data-ttu-id="3c5b0-1398">Correção nº 10996: erro aperfeiçoado para `--force-change-password-next-login` em `az ad user update` quando `--password` não for especificado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1398">Fixed #10996: Polish error for `--force-change-password-next-login` in `az ad user update` when `--password` is not specified</span></span>

### <a name="redis"></a><span data-ttu-id="3c5b0-1399">Redis</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1399">Redis</span></span>

* <span data-ttu-id="3c5b0-1400">Correção nº 2902: evite definir configurações de memória ao atualizar o cache do SKU básico</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1400">Fixed #2902: Avoid setting memory configs while updating Basic SKU cache</span></span>

### <a name="reservations"></a><span data-ttu-id="3c5b0-1401">Reservas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1401">Reservations</span></span>

* <span data-ttu-id="3c5b0-1402">Versão do SDK atualizada para 0.6.0</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1402">Upgraded SDK Version to 0.6.0</span></span>
* <span data-ttu-id="3c5b0-1403">Informações de detalhes do plano de cobrança atualizadas após chamar Get-Gatalogs</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1403">Added billingplan details info after calling Get-Gatalogs</span></span>
* <span data-ttu-id="3c5b0-1404">Novo comando `az reservations reservation-order calculate` adicionado para calcular o preço de uma reserva</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1404">Added new command `az reservations reservation-order calculate` to calculate the price for a reservation</span></span>
* <span data-ttu-id="3c5b0-1405">Novo comando `az reservations reservation-order purchase` adicionado para comprar uma nova reserva</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1405">Added new command `az reservations reservation-order purchase` to purchase a new reservation</span></span>

### <a name="rest"></a><span data-ttu-id="3c5b0-1406">Rest</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1406">Rest</span></span>
* <span data-ttu-id="3c5b0-1407">`az rest` alterado para GA</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1407">Changed `az rest` to GA</span></span>

### <a name="sql"></a><span data-ttu-id="3c5b0-1408">SQL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1408">SQL</span></span>

* <span data-ttu-id="3c5b0-1409">azure-mgmt-sql atualizado para 0.15.0.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1409">Updated azure-mgmt-sql to version 0.15.0.</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-1410">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1410">Storage</span></span>

* <span data-ttu-id="3c5b0-1411">storage account create: --enable-hierarchical-namespace adicionado para dar suporte à semântica do sistema de arquivos no serviço Blob.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1411">storage account create: Added --enable-hierarchical-namespace to support filesystem semantics in blob service.</span></span>
* <span data-ttu-id="3c5b0-1412">Exceção não relacionada removida da mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1412">Removed unrelated exception from error message</span></span>
* <span data-ttu-id="3c5b0-1413">Problemas corrigidos com a mensagem de erro incorreta "Você não tem as permissões necessárias para executar essa operação."</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1413">Fixed issues with incorrect error message "You do not have the required permissions needed to perform this operation."</span></span> <span data-ttu-id="3c5b0-1414">quando bloqueado pelas regras de rede ou AuthenticationFailed.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1414">when blocked by network rules or AuthenticationFailed.</span></span>

## <a name="november-4-2019"></a><span data-ttu-id="3c5b0-1415">4 de novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1415">November 4, 2019</span></span>

<span data-ttu-id="3c5b0-1416">Versão 2.0.76</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1416">Version 2.0.76</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-1417">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1417">ACR</span></span>

* <span data-ttu-id="3c5b0-1418">O parâmetro de versão prévia `--pack-image-tag` foi adicionado ao comando `az acr pack build`.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1418">Added a preview parameter `--pack-image-tag` to command `az acr pack build`.</span></span>
* <span data-ttu-id="3c5b0-1419">Suporte adicionado para habilitar a auditoria na criação de um registro</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1419">Added support for enabling auditing on creating a registry</span></span>
* <span data-ttu-id="3c5b0-1420">Suporte adicionado para o RBAC com escopo de repositório</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1420">Added support for Repository-scoped RBAC</span></span>

### <a name="aks"></a><span data-ttu-id="3c5b0-1421">AKS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1421">AKS</span></span>

* <span data-ttu-id="3c5b0-1422">`--enable-cluster-autoscaler`, `--min-count` e `--max-count` foram adicionados ao comando `az aks create`, que habilita o dimensionamento automático do cluster para o pool de nós.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1422">Added `--enable-cluster-autoscaler`, `--min-count` and `--max-count` to the `az aks create` command, which enables cluster autoscaler for the node pool.</span></span>
* <span data-ttu-id="3c5b0-1423">Foram adicionados os sinalizadores acima, bem como `--update-cluster-autoscaler` e `--disable-cluster-autoscaler` ao comando `az aks update`, permitindo atualizações do cluster de dimensionamento automático.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1423">Added the above flags as well as `--update-cluster-autoscaler` and `--disable-cluster-autoscaler` to the `az aks update` command, allowing updates to cluster autoscaler.</span></span>

### <a name="appconfig"></a><span data-ttu-id="3c5b0-1424">AppConfig</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1424">AppConfig</span></span>

* <span data-ttu-id="3c5b0-1425">O grupo de comandos do recurso AppConfig foi adicionado para gerenciar os sinalizadores de recurso armazenados em uma Configuração de Aplicativos.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1425">Added appconfig feature command group to manage feature flags stored in an App Configuration.</span></span>
* <span data-ttu-id="3c5b0-1426">Foi corrigido um bug secundário do comando de exportação para arquivo appconfig kv.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1426">Fixed minor bug for appconfig kv export to file command.</span></span> <span data-ttu-id="3c5b0-1427">Foi interrompida a leitura de conteúdo do arquivo de destino durante a exportação.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1427">Stop reading dest file contents during export.</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-1428">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1428">AppService</span></span>

* <span data-ttu-id="3c5b0-1429">`az appservice plan create`: Foi adicionado o suporte para definir 'persitecalling' no comando appservice plan create.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1429">`az appservice plan create`: Added support to set 'persitescaling' on appservice plan create.</span></span>
* <span data-ttu-id="3c5b0-1430">Foi corrigido um problema em que a operação webapp config ssl bind estava removendo as marcas existentes do recurso</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1430">Fixed an issue where webapp config ssl bind operation was removing existing tags from the resource</span></span>
* <span data-ttu-id="3c5b0-1431">Foi adicionado o sinalizador `--build-remote` para `az functionapp deployment source config-zip` para dar suporte à ação de build remoto durante a implantação do aplicativo de funções.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1431">Added `--build-remote` flag for `az functionapp deployment source config-zip` to support remote build action during function app deployment.</span></span>
* <span data-ttu-id="3c5b0-1432">Foi alterada a versão do nó padrão em aplicativos de funções para ~10 para Windows</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1432">Changed default node version on function apps to ~10 for Windows</span></span>
* <span data-ttu-id="3c5b0-1433">A propriedade `--runtime-version` foi adicionada a `az functionapp create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1433">Added `--runtime-version` property to `az functionapp create`</span></span>

### <a name="arm"></a><span data-ttu-id="3c5b0-1434">ARM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1434">ARM</span></span>

* <span data-ttu-id="3c5b0-1435">`az deployment/group deployment validate`: Foi adicionado o parâmetro `--handle-extended-json-format` para dar suporte a várias linhas e comentários no modelo JSON durante a implantação.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1435">`az deployment/group deployment validate`: Added `--handle-extended-json-format` parameter to support multiline and comments in json template when deployment.</span></span>
* <span data-ttu-id="3c5b0-1436">O azure-mgmt-resource passou a usar a 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1436">Bumped azure-mgmt-resource to 2019-07-01</span></span>

### <a name="backup"></a><span data-ttu-id="3c5b0-1437">Backup</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1437">Backup</span></span>

* <span data-ttu-id="3c5b0-1438">Foi adicionado o suporte de backup aos Arquivos do Azure</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1438">Added AzureFiles backup support</span></span>

### <a name="compute"></a><span data-ttu-id="3c5b0-1439">Computação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1439">Compute</span></span>

* <span data-ttu-id="3c5b0-1440">`az vm create`: foi adicionado um aviso ao especificar a rede acelerada e um adaptador de rede existente juntos.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1440">`az vm create`: Added warning when specifying accelerated networking and an existing NIC together.</span></span>
* <span data-ttu-id="3c5b0-1441">`az vm create`: foi adicionado `--vmss` para especificar um conjunto de dimensionamento de máquinas virtuais existente ao qual a máquina virtual deve ser atribuída.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1441">`az vm create`: Added `--vmss` to specify an existing virtual machine scale set that the virtual machine should be assigned to.</span></span>
* <span data-ttu-id="3c5b0-1442">`az vm/vmss create`: foi adicionada uma cópia local do arquivo de alias de imagem para que ele possa ser acessado em um ambiente de rede restrita.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1442">`az vm/vmss create`: Added a local copy of image alias file so that it can be accessed in a restricted network environment.</span></span>
* <span data-ttu-id="3c5b0-1443">`az vmss create`: foi adicionado `--orchestration-mode` para especificar como as máquinas virtuais são gerenciadas pelo conjunto de dimensionamento.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1443">`az vmss create`: Added `--orchestration-mode` to specify how virtual machines are managed by the scale set.</span></span>
* <span data-ttu-id="3c5b0-1444">`az vm/vmss update`: foi adicionado `--ultra-ssd-enabled` para permitir a atualização da configuração de SSD Ultra.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1444">`az vm/vmss update`: Added `--ultra-ssd-enabled` to allow updating ultra SSD setting.</span></span>
* <span data-ttu-id="3c5b0-1445">[ALTERAÇÃO DA FALHA] `az vm extension set`: foi corrigido o bug em que os usuários não podiam definir uma extensão em uma VM com `--ids`.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1445">[BREAKING CHANGE] `az vm extension set`: Fixed bug where users could not set an extension on a VM with `--ids`.</span></span>
* <span data-ttu-id="3c5b0-1446">Foram adicionados os novos comandos `az vm image terms accept/cancel/show` para gerenciar os termos de imagem do Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1446">Added new commands `az vm image terms accept/cancel/show` to manage Azure Marketplace image terms.</span></span>
* <span data-ttu-id="3c5b0-1447">O VMAccessForLinux foi atualizado para a versão 1.5</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1447">Updated VMAccessForLinux to version 1.5</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="3c5b0-1448">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1448">CosmosDB</span></span>

* <span data-ttu-id="3c5b0-1449">[ALTERAÇÃO DA FALHA] `az sql container create`: `--partition-key-path` foi alterado para parâmetro obrigatório</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1449">[BREAKING CHANGE] `az sql container create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="3c5b0-1450">[ALTERAÇÃO DA FALHA] `az gremlin graph create`: `--partition-key-path` foi alterado para parâmetro obrigatório</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1450">[BREAKING CHANGE] `az gremlin graph create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="3c5b0-1451">`az sql container create`: Adição de `--unique-key-policy` e `--conflict-resolution-policy`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1451">`az sql container create`: Added `--unique-key-policy` and `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="3c5b0-1452">`az sql container create/update`: o esquema padrão `--idx` foi atualizado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1452">`az sql container create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="3c5b0-1453">`gremlin graph create`: Adicionado `--conflict-resolution-policy`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1453">`gremlin graph create`: Added `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="3c5b0-1454">`gremlin graph create/update`: o esquema padrão `--idx` foi atualizado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1454">`gremlin graph create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="3c5b0-1455">Erro de digitação corrigido na mensagem de ajuda</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1455">Fixed typo in help message</span></span>
* <span data-ttu-id="3c5b0-1456">banco de dados: Foram adicionadas informações sobre preteridos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1456">database: Added deprecation information</span></span>
* <span data-ttu-id="3c5b0-1457">coleção: Foram adicionadas informações sobre preteridos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1457">collection: Added deprecation information</span></span>

### <a name="iot"></a><span data-ttu-id="3c5b0-1458">IoT</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1458">IoT</span></span>

* <span data-ttu-id="3c5b0-1459">Um novo tipo de fonte de roteamento foi adicionado: DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1459">Added new routing source type: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="3c5b0-1460">Foi corrigido o erro de recursos ausentes no `az iot hub create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1460">Fixed missing features in `az iot hub create`</span></span>

### <a name="key-vault"></a><span data-ttu-id="3c5b0-1461">Key Vault</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1461">Key Vault</span></span>

* <span data-ttu-id="3c5b0-1462">Foi corrigido um erro inesperado quando o arquivo de certificado não existe</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1462">Fixed an unexpected error when certificate file does not exist</span></span>
* <span data-ttu-id="3c5b0-1463">Foi corrigido o problema em que o `az keyvault recover/purge` não funcionava</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1463">Fixed `az keyvault recover/purge` not working</span></span>

### <a name="netappfiles"></a><span data-ttu-id="3c5b0-1464">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1464">NetAppFiles</span></span>

* <span data-ttu-id="3c5b0-1465">O azure-mgmt-netapp foi atualizado para 0.6.0 para usar a versão da API 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1465">Upgraded azure-mgmt-netapp to 0.6.0 to use API version 2019-07-01.</span></span> <span data-ttu-id="3c5b0-1466">Essa nova versão da API inclui:</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1466">This new API version includes:</span></span>

    - <span data-ttu-id="3c5b0-1467">A criação de volume `--protocol-types` agora aceita "NFSv4.1" não "NFSv4"</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1467">Volume creation `--protocol-types` accepts now "NFSv4.1" not "NFSv4"</span></span>
    - <span data-ttu-id="3c5b0-1468">A propriedade da política de exportação de volume agora é chamada 'nfsv41' não 'nfsv4'</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1468">Volume export policy property now named 'nfsv41' not 'nfsv4'</span></span>
    - <span data-ttu-id="3c5b0-1469">O volume `--creation-token` foi renomeado para `--file-path`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1469">Volume `--creation-token` renamed to `--file-path`</span></span>
    - <span data-ttu-id="3c5b0-1470">A data de criação do instantâneo agora é chamada apenas de 'criação'</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1470">Snapshot creation date now named just 'created'</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-1471">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1471">Network</span></span>

* <span data-ttu-id="3c5b0-1472">`az network private-dns link vnet create/update`: suporte à vinculação de rede virtual entre locatários.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1472">`az network private-dns link vnet create/update`: Support cross-tenant virtual network linking.</span></span>
* <span data-ttu-id="3c5b0-1473">[ALTERAÇÃO DA FALHA] `az network vnet subnet list`: `--resource-group` e `--vnet-name` foram alterados para serem obrigatórios agora.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1473">[BREAKING CHANGE] `az network vnet subnet list`: Changed `--resource-group` and `--vnet-name` to be required now.</span></span>
* <span data-ttu-id="3c5b0-1474">`az network public-ip prefix create`: Suporte adicionado para especificar a versão do endereço IP (IPv4, IPv6) durante a criação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1474">`az network public-ip prefix create`: Added support to specify IP address version (IPv4, IPv6) when creation</span></span>
* <span data-ttu-id="3c5b0-1475">O azure-mgmt-network foi atualizado para 7.0.0 e a api-version para 2019-09-01</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1475">Bumped azure-mgmt-network to 7.0.0 and api-version to 2019-09-01</span></span>
* <span data-ttu-id="3c5b0-1476">`az network vrouter`: Suporte adicionado para o novo roteador virtual de serviço e o emparelhamento do roteador virtual</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1476">`az network vrouter`: Added support for new service virtual router and virtual router peering</span></span>
* <span data-ttu-id="3c5b0-1477">`az network express-route gateway connection`: Adicionado o suporte para `--internet-security`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1477">`az network express-route gateway connection`: Added support for `--internet-security`</span></span>

### <a name="profile"></a><span data-ttu-id="3c5b0-1478">Perfil</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1478">Profile</span></span>

* <span data-ttu-id="3c5b0-1479">Foi corrigido o problema em que o `az account get-access-token --resource-type ms-graph` não funcionava</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1479">Fixed `az account get-access-token --resource-type ms-graph` not working</span></span>
* <span data-ttu-id="3c5b0-1480">O aviso foi removido de `az login`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1480">Removed warning from `az login`</span></span>

### <a name="rbac"></a><span data-ttu-id="3c5b0-1481">RBAC</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1481">RBAC</span></span>

* <span data-ttu-id="3c5b0-1482">Foi corrigido o problema em que o `az ad app update --id {} --display-name {}` não funcionava</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1482">Fixed `az ad app update --id {} --display-name {}` doesn't work</span></span>

### <a name="servicefabric"></a><span data-ttu-id="3c5b0-1483">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1483">ServiceFabric</span></span>

* <span data-ttu-id="3c5b0-1484">`az sf cluster create`: foi corrigido um problema que ocorria ao modificar o VMSS de computação do template.json do Linux e do Windows, do Service Fabric, de discos Standard para discos gerenciados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1484">`az sf cluster create`: Fixed an issue by modifying service fabric linux and windows template.json compute vmss from standard to managed disks</span></span>

### <a name="sql"></a><span data-ttu-id="3c5b0-1485">SQL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1485">SQL</span></span>

* <span data-ttu-id="3c5b0-1486">Os parâmetros `--compute-model`, `--auto-pause-delay` e `--min-capacity` foram adicionados para dar suporte a operações CRUD para a nova oferta de Banco de Dados SQL: Modelo de computação sem servidor.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1486">Added `--compute-model`, `--auto-pause-delay`, and `--min-capacity` parameters to support CRUD operations for new SQL Database offering: Serverless compute model.</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-1487">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1487">Storage</span></span>

* <span data-ttu-id="3c5b0-1488">`az storage account create/update`: Foram adicionados o parâmetro --enable-files-adds e o grupo Argumentos de Propriedades do Azure Active Directory para dar suporte à Autenticação do Serviço de Domínio do Active Directory do Arquivos do Azure</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1488">`az storage account create/update`: Added --enable-files-adds parameter and Azure Active Directory Properties Argument group to support Azure Files Active Directory Domain Service Authentication</span></span>
* <span data-ttu-id="3c5b0-1489">O `az storage account keys list/renew` foi expandido para dar suporte à listagem ou à regeneração de chaves Kerberos da conta de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1489">Expanded `az storage account keys list/renew` to support listing or regenerating Kerberos keys of storage account.</span></span>

## <a name="october-15-2019"></a><span data-ttu-id="3c5b0-1490">15 de outubro de 2019</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1490">October 15, 2019</span></span>

<span data-ttu-id="3c5b0-1491">Versão 2.0.75</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1491">Version 2.0.75</span></span>

### <a name="aks"></a><span data-ttu-id="3c5b0-1492">AKS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1492">AKS</span></span>

* <span data-ttu-id="3c5b0-1493">Alteração do valor padrão `--load-balancer-sku` para `standard` se for compatível com a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1493">Changed `--load-balancer-sku` default value to `standard` if supported by the kubernetes version</span></span>
* <span data-ttu-id="3c5b0-1494">Alteração do valor padrão `--vm-set-type` para `virtualmachinescalesets` se for compatível com a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1494">Changed `--vm-set-type` default value to `virtualmachinescalesets` if supported by the kubernetes version</span></span>

### <a name="ams"></a><span data-ttu-id="3c5b0-1495">AMS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1495">AMS</span></span>

* <span data-ttu-id="3c5b0-1496">[ALTERAÇÃO SIGNIFICATIVA] Alteração do nome de `job start` para `job create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1496">[BREAKING CHANGE] Changed the name of `job start` to `job create`</span></span>
* <span data-ttu-id="3c5b0-1497">[ALTERAÇÃO SIGNIFICATIVA] Alteração do parâmetro `--ask` de `content-key-policy create` para usar uma cadeia de 32 caracteres hexadecimais em vez do UTF8</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1497">[BREAKING CHANGE] Changed the `--ask` parameter of `content-key-policy create` to use a 32-character hex string instead of UTF8</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-1498">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1498">AppService</span></span>

* <span data-ttu-id="3c5b0-1499">Adição dos comandos `webapp config access-restriction show|set|add|remove`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1499">Added commands `webapp config access-restriction show|set|add|remove`</span></span>
* <span data-ttu-id="3c5b0-1500">Adição de um melhor tratamento de erro a `webapp up`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1500">Added better error handling to `webapp up`</span></span>
* <span data-ttu-id="3c5b0-1501">Adição de suporte do SKU `Isolated` para `appservice plan update`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1501">Added support for `Isolated` SKU to `appservice plan update`</span></span>

### <a name="arm"></a><span data-ttu-id="3c5b0-1502">ARM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1502">ARM</span></span>

* <span data-ttu-id="3c5b0-1503">Adição do parâmetro `--handle-extended-json-format``deployment create` para dar suporte a várias linhas e a comentários no modelo json</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1503">Added `--handle-extended-json-format` parameter `deployment create` to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="3c5b0-1504">Computação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1504">Compute</span></span>

* <span data-ttu-id="3c5b0-1505">Parâmetro `--enable-agent` adicionado a `vm create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1505">Added `--enable-agent` parameter to `vm create`</span></span>
* <span data-ttu-id="3c5b0-1506">Alteração de `vm create` para usar um SKU de IP público padrão automaticamente ao usar zonas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1506">Changed `vm create` to use standard public IP SKU automatically when using zones</span></span>
* <span data-ttu-id="3c5b0-1507">Alteração de `vm create` para criar automaticamente um nome de computador válido para uma VM, caso nenhum tenha sido fornecido</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1507">Changed `vm create` to automatically create a valid computer name for a VM if none is provided</span></span>
* <span data-ttu-id="3c5b0-1508">Adição do parâmetro `--computer-name-prefix` a `vmss create` para dar suporte ao prefixo de nome de computador personalizado de máquinas virtuais no VMSS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1508">Added `--computer-name-prefix` parameter to `vmss create` to support custom computer name prefix of virtual machines in the VMSS</span></span>
* <span data-ttu-id="3c5b0-1509">Adicione o parâmetro `--workspace` a `vm create` para habilitar o workspace de análise de logs automaticamente</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1509">Add `--workspace` parameter to `vm create` to enable log analytics workspace automatically</span></span>
* <span data-ttu-id="3c5b0-1510">Versão de API de galerias atualizadas para 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1510">Updated galleries API version to 2019-07-01</span></span>

### <a name="core"></a><span data-ttu-id="3c5b0-1511">Núcleo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1511">Core</span></span>

* <span data-ttu-id="3c5b0-1512">Adição da verificação de sintaxe para o parâmetro `--set` no comando de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1512">Added syntax check for `--set` parameter in generic update command</span></span>

### <a name="iot"></a><span data-ttu-id="3c5b0-1513">IoT</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1513">IoT</span></span>

* <span data-ttu-id="3c5b0-1514">Correção de um problema em que o `iot hub show` retornaria incorretamente um erro com "recurso não encontrado"</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1514">Fixed an issue where `iot hub show` would incorrectly error with "resource not found"</span></span>

### <a name="monitor"></a><span data-ttu-id="3c5b0-1515">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1515">Monitor</span></span>

* <span data-ttu-id="3c5b0-1516">Adição de suporte para CRUD a `monitor log-analytics workspace`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1516">Added support for CRUD to `monitor log-analytics workspace`</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-1517">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1517">Network</span></span>

* <span data-ttu-id="3c5b0-1518">Adição de suporte para vinculação virtual entre locatários para `network private-dns link vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1518">Added support for cross-tenant virtual linking to `network private-dns link vnet [create|update]`</span></span>
* <span data-ttu-id="3c5b0-1519">[ALTERAÇÃO SIGNIFICATIVA] Alteração de `network vnet subnet list` para exigir os parâmetros `--resource-group` e `--vnet-name`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1519">[BREAKING CHANGE] Changed `network vnet subnet list` to require `--resource-group` and `--vnet-name` parameters</span></span>

### <a name="sql"></a><span data-ttu-id="3c5b0-1520">SQL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1520">SQL</span></span>

* <span data-ttu-id="3c5b0-1521">Adição de comandos a `sql mi ad-admin` que dão suporte à configuração de um administrador do AAD em instâncias gerenciadas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1521">Added commands to `sql mi ad-admin` that support setting an AAD administrator on managed instances</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-1522">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1522">Storage</span></span>

* <span data-ttu-id="3c5b0-1523">Adição do parâmetro `--preserve-s2s-access-tier``storage copy` para preservar a camada de acesso durante a cópia do serviço para serviço</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1523">Added `--preserve-s2s-access-tier` parameter `storage copy` to preserve access tier during service to service copy</span></span>
* <span data-ttu-id="3c5b0-1524">Adição do parâmetro `--enable-large-file-share` a `storage account [create|update]` para dar suporte a compartilhamentos de arquivos grandes para a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1524">Added `--enable-large-file-share` parameter to `storage account [create|update]` to support large file shares for storage account</span></span>

## <a name="september-24-2019"></a><span data-ttu-id="3c5b0-1525">24 de setembro de 2019</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1525">September 24, 2019</span></span>

<span data-ttu-id="3c5b0-1526">Versão 2.0.74</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1526">Version 2.0.74</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-1527">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1527">ACR</span></span>

* <span data-ttu-id="3c5b0-1528">Inclusão de um parâmetro `--type` obrigatório em `acr config retention update`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1528">Added a required `--type` parameter to `acr config retention update`</span></span>
* <span data-ttu-id="3c5b0-1529">[ALTERAÇÃO SIGNIFICATIVA] O parâmetro renomeado `--name -n` foi alterado para `--registry -r ` para o grupo de comando `acr config`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1529">[BREAKING CHANGE] Renamed parameter `--name -n` changed to `--registry -r ` for `acr config` command group</span></span>

### <a name="aks"></a><span data-ttu-id="3c5b0-1530">AKS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1530">AKS</span></span>

* <span data-ttu-id="3c5b0-1531">Inclusão do parâmetro `--load-balancer-sku` no comando `aks create`, o que permite criar um cluster do AKS com SLB</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1531">Added `--load-balancer-sku` parameter to `aks create` command, which allows for creating AKS cluster with SLB</span></span>
* <span data-ttu-id="3c5b0-1532">Inclusão dos parâmetros `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` e `--load-balancer-outbound-ip-prefixes` nos comandos `aks [create|update]`, o que permite atualizar o perfil do balanceador de carga de um cluster do AKS com SLB</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1532">Added `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` and `--load-balancer-outbound-ip-prefixes` parameters to `aks [create|update]` commands, which allow for updating load balancer profile of an AKS cluster with SLB</span></span>
* <span data-ttu-id="3c5b0-1533">Inclusão do parâmetro `--vm-set-type` no comando `aks create`, o que permite especificar os tipos de VM de um cluster do AKS (vmas ou vmss)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1533">Added `--vm-set-type` parameter to `aks create` command, which allows to specify vm types of an AKS Cluster (vmas or vmss)</span></span>

### <a name="arm"></a><span data-ttu-id="3c5b0-1534">ARM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1534">ARM</span></span>

* <span data-ttu-id="3c5b0-1535">Inclusão do parâmetro `--handle-extended-json-format` no comando `group deployment create` para compatibilidade com várias linhas e comentários no modelo JSON</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1535">Added `--handle-extended-json-format` parameter to `group deployment create` command to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="3c5b0-1536">Computação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1536">Compute</span></span>

* <span data-ttu-id="3c5b0-1537">Inclusão do parâmetro `--terminate-notification-time` nos comandos `vmss [create|update]` para compatibilidade com a capacidade de configurar o encerramento de eventos agendados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1537">Added `--terminate-notification-time` parameter to `vmss [create|update]` commands to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="3c5b0-1538">Inclusão do parâmetro `--enable-terminate-notification` no comando `vmss update` para compatibilidade com a capacidade de configurar o encerramento de eventos agendados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1538">Added `--enable-terminate-notification` parameter to `vmss update` command to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="3c5b0-1539">Inclusão dos parâmetros `--priority,`, `--eviction-policy,` e `--max-billing` nos comandos `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1539">Added `--priority,` `--eviction-policy,` `--max-billing` parameters to `[vm|vmss] create` commands</span></span>
* <span data-ttu-id="3c5b0-1540">Alteração de `disk create` para permitir a especificação do tamanho exato do carregamento de disco</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1540">Changed `disk create` to allow specifying the exact size of the disk upload</span></span>
* <span data-ttu-id="3c5b0-1541">Inclusão de compatibilidade com instantâneos incrementais para discos gerenciados para `snapshot create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1541">Added support for incremental snapshots for managed disks to `snapshot create`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="3c5b0-1542">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1542">Cosmos DB</span></span>

* <span data-ttu-id="3c5b0-1543">Inclusão do parâmetro `--type <key-type>` no comando `cosmosdb keys list` para mostrar a chave, as chaves somente leitura ou cadeias de conexão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1543">Added `--type <key-type>` parameter to `cosmosdb keys list` command to show key, read only keys or connection strings</span></span>
* <span data-ttu-id="3c5b0-1544">Adicionado o comando `cosmosdb keys regenerate`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1544">Added `cosmosdb keys regenerate` command</span></span>
* <span data-ttu-id="3c5b0-1545">[PRETERIDO] Comandos `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` e `cosmosdb list-read-only-keys` preteridos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1545">[DEPRECATED] Deprecated `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` and `cosmosdb list-read-only-keys` commands</span></span>

### <a name="eventgrid"></a><span data-ttu-id="3c5b0-1546">EventGrid</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1546">EventGrid</span></span>

* <span data-ttu-id="3c5b0-1547">Correção do texto de ajuda do ponto de extremidade para fazer referência ao parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1547">Fixed the endpoint help text to refer to the right parameter</span></span>

### <a name="key-vault"></a><span data-ttu-id="3c5b0-1548">Key Vault</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1548">Key Vault</span></span>

* <span data-ttu-id="3c5b0-1549">Correção do problema em que fazer logon com um locatário (`login -t`) poderia causar uma falha no `keyvault create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1549">Fixed issue where logging in with a tenant (`login -t`) could cause `keyvault create` to fail</span></span>

### <a name="monitor"></a><span data-ttu-id="3c5b0-1550">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1550">Monitor</span></span>

* <span data-ttu-id="3c5b0-1551">Correção do problema em que o caractere `:` não era permitido no argumento `--condition` para `monitor metrics alert create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1551">Fixed issue where `:` character was not allowed in `--condition` argument to `monitor metrics alert create`</span></span>

### <a name="policy"></a><span data-ttu-id="3c5b0-1552">Política</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1552">Policy</span></span>

* <span data-ttu-id="3c5b0-1553">Inclusão de compatibilidade com a API de Política, versão de 01/06/2019</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1553">Added support for Policy API version 2019-06-01</span></span>
* <span data-ttu-id="3c5b0-1554">Inclusão do parâmetro `--enforcement-mode` no comando `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1554">Added `--enforcement-mode` parameter to `policy assignment create` command</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-1555">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1555">Storage</span></span>

* <span data-ttu-id="3c5b0-1556">Inclusão do parâmetro `--blob-type` no comando `az storage copy`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1556">Added `--blob-type` parameter to `az storage copy` command</span></span>

## <a name="september-10-2019"></a><span data-ttu-id="3c5b0-1557">10 de setembro de 2019</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1557">September 10, 2019</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-1558">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1558">ACR</span></span>

* <span data-ttu-id="3c5b0-1559">Adição do grupo de comandos `acr config retention` para configurar a política de retenção</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1559">Added command group `acr config retention` to configure retention policy</span></span>

### <a name="aks"></a><span data-ttu-id="3c5b0-1560">AKS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1560">AKS</span></span>

* <span data-ttu-id="3c5b0-1561">Adição de suporte para integração do ACR com os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1561">Added support for ACR integration with the following commands:</span></span>
  * <span data-ttu-id="3c5b0-1562">Adição do parâmetro `--attach-acr` a `aks [create|update]` para anexar um ACR a um cluster do AKS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1562">Added `--attach-acr` parameter to `aks [create|update]` to attach an ACR to an AKS cluster</span></span>
  * <span data-ttu-id="3c5b0-1563">Adição do parâmetro `--detach-acr` a `aks update` para desanexar o ACR de um cluster do AKS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1563">Added `--detach-acr` parameter to `aks update` to detach the ACR from an AKS cluster</span></span>

### <a name="arm"></a><span data-ttu-id="3c5b0-1564">ARM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1564">ARM</span></span>

* <span data-ttu-id="3c5b0-1565">Atualização para uso da versão de API 2019-05-10</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1565">Updated to use API version 2019-05-10</span></span>

### <a name="batch"></a><span data-ttu-id="3c5b0-1566">Lote</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1566">Batch</span></span>

* <span data-ttu-id="3c5b0-1567">Adição de novas definições de configuração JSON de `--json-file` para `batch pool create`:</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1567">Added new JSON configuration settings to `--json-file` for `batch pool create`:</span></span>
  * <span data-ttu-id="3c5b0-1568">Adição de `MountConfigurations` para montagens do sistema de arquivos (confira https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body para obter detalhes)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1568">Added `MountConfigurations` for file system mounts (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
  * <span data-ttu-id="3c5b0-1569">Adição da propriedade opcional `publicIPs` a `NetworkConfiguration` para IPs públicos em pools (confira https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body para obter detalhes)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1569">Added optional property `publicIPs` on `NetworkConfiguration` for public IPs on pools (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
* <span data-ttu-id="3c5b0-1570">Adição de suporte para galerias de imagens compartilhadas a `--image`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1570">Added support for shared image galleries to `--image`</span></span>
* <span data-ttu-id="3c5b0-1571">[ALTERAÇÃO SIGNIFICATIVA] Alteração do valor padrão de `--start-task-wait-for-success` em `batch pool create` para `true`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1571">[BREAKING CHANGE] Changed default value of `--start-task-wait-for-success` on `batch pool create` to be `true`</span></span>
* <span data-ttu-id="3c5b0-1572">[ALTERAÇÃO SIGNIFICATIVA] Alteração do valor padrão de `Scope` em `AutoUserSpecification` para sempre ser Pool (anteriormente, `Task` em nós do Windows e `Pool` em nós do Linux)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1572">[BREAKING CHANGE] Changed default value for `Scope` on `AutoUserSpecification` to always be Pool (was `Task` on Windows nodes, `Pool` on Linux nodes)</span></span>
  * <span data-ttu-id="3c5b0-1573">Esse argumento só pode ser definido em uma configuração JSON com `--json-file`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1573">This argument can only be set from a JSON configuration with `--json-file`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="3c5b0-1574">HDInsight</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1574">HDInsight</span></span>

* <span data-ttu-id="3c5b0-1575">Versão de GA</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1575">GA release</span></span>
* <span data-ttu-id="3c5b0-1576">[ALTERAÇÃO SIGNIFICATIVA] Alteração do parâmetro `--workernode-count/-c` de `az hdinsight resize` para ser obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1576">[BREAKING CHANGE] Changed parameter `--workernode-count/-c` of `az hdinsight resize` to be required.</span></span>

### <a name="key-vault"></a><span data-ttu-id="3c5b0-1577">Key Vault</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1577">Key Vault</span></span>

* <span data-ttu-id="3c5b0-1578">Correção do problema em que as sub-redes não podiam ser excluídas das regras da rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1578">Fixed issue where subnets couldn't be deleted from network rules</span></span>
* <span data-ttu-id="3c5b0-1579">Correção do problema em que sub-redes e endereços IP duplicados podiam ser adicionados às regras da rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1579">Fixed issue where duplicated subnets and IP addresses could be added to network rules</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-1580">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1580">Network</span></span>

* <span data-ttu-id="3c5b0-1581">Adição do parâmetro `--interval` a `network watcher flow-log` para definir o valor do intervalo de análise de tráfego</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1581">Added `--interval` parameter to `network watcher flow-log` to set traffic analysis interval value</span></span>
* <span data-ttu-id="3c5b0-1582">Adição de `network application-gateway identity` para gerenciar a identidade do gateway</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1582">Added `network application-gateway identity` to manage gateway identity</span></span>
* <span data-ttu-id="3c5b0-1583">Adição de suporte para definir a ID do Key Vault como `network application-gateway ssl-cert`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1583">Added support for setting Key Vault ID to `network application-gateway ssl-cert`</span></span>
* <span data-ttu-id="3c5b0-1584">Adicionado `network express-route peering peer-connection [show|list]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1584">Added `network express-route peering peer-connection [show|list]`</span></span>

### <a name="policy"></a><span data-ttu-id="3c5b0-1585">Política</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1585">Policy</span></span>

* <span data-ttu-id="3c5b0-1586">Atualização para uso da versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1586">Updated to use API version 2019-01-01</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="3c5b0-1587">27 de agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1587">August 27, 2019</span></span>

<span data-ttu-id="3c5b0-1588">Versão 2.0.72</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1588">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-1589">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1589">ACR</span></span>

* <span data-ttu-id="3c5b0-1590">[ALTERAÇÃO SIGNIFICATIVA] Remoção da compatibilidade com o SKU `classic`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1590">[BREAKING CHANGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="3c5b0-1591">Gerenciamento de API</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1591">API Management</span></span>

* <span data-ttu-id="3c5b0-1592">[VERSÃO PRÉVIA] Adição do grupo de comandos `apim`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1592">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-1593">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1593">AppService</span></span>

* <span data-ttu-id="3c5b0-1594">Correção do problema com o comando `webapp webjob continuous start` ao especificar um slot</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1594">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="3c5b0-1595">Alteração de `webapp up` para detectar a pasta `env` e removê-la do arquivo usado para implantação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1595">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="3c5b0-1596">Keyvault</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1596">Keyvault</span></span>

* <span data-ttu-id="3c5b0-1597">Correção de um bug no `keyvault secret set` que ignorava o argumento `--expires`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1597">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-1598">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1598">Network</span></span>

* <span data-ttu-id="3c5b0-1599">Adição de suporte para endereços IPv6 a argumentos `--private-ip-address-version`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1599">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="3c5b0-1600">Adição de novos comandos `network private-endpoint [create|update|list-types]` para o gerenciamento de ponto de extremidade privado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1600">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="3c5b0-1601">Adição do grupo de comandos `network private-link-service`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1601">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="3c5b0-1602">Adicionados os argumentos `--private-endpoint-network-policies` e `--private-link-service-network-policies` para `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1602">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="3c5b0-1603">RBAC</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1603">RBAC</span></span>

* <span data-ttu-id="3c5b0-1604">Correção de um problema com `ad app update --homepage` em que a página inicial não era atualizada</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1604">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="3c5b0-1605">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1605">ServiceFabric</span></span>

* <span data-ttu-id="3c5b0-1606">Adição de suporte para nomes de Key Vault grafados com maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1606">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="3c5b0-1607">Correção de um problema ao usar certificados no Key Vault</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1607">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="3c5b0-1608">Correção de um problema com o uso de arquivos de certificado PFX</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1608">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="3c5b0-1609">Correção de um problema com `sf cluster certificate add` quando o grupo de recursos do Key Vault não era especificado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1609">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="3c5b0-1610">Correção de um problema em que `sf cluster set` não funcionava</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1610">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="3c5b0-1611">SignalR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1611">SignalR</span></span>

* <span data-ttu-id="3c5b0-1612">Novos comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1612">Added new commands:</span></span>
  * <span data-ttu-id="3c5b0-1613">`signalr cors`: gerenciar CORS do SignalR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1613">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="3c5b0-1614">`signalr restart`: reiniciar um serviço do SignalR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1614">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="3c5b0-1615">`signalr update`: atualizar um serviço do SignalR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1615">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="3c5b0-1616">Adicionado o argumento `--service-mode` para `signalr create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1616">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-1617">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1617">Storage</span></span>

* <span data-ttu-id="3c5b0-1618">Adicionado o comando `storage account revoke-delegation-keys`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1618">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="3c5b0-1619">13 de agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1619">August 13, 2019</span></span>

<span data-ttu-id="3c5b0-1620">Versão 2.0.71</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1620">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-1621">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1621">AppService</span></span>

* <span data-ttu-id="3c5b0-1622">Um problema de falha de slots com os comandos `webapp webjob continuous` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1622">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="3c5b0-1623">BotService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1623">BotService</span></span>

* <span data-ttu-id="3c5b0-1624">[ALTERAÇÃO SIGNIFICATIVA] O suporte para a criação de bots SDK v3 foi removido</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1624">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="3c5b0-1625">CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1625">CognitiveServices</span></span>

* <span data-ttu-id="3c5b0-1626">Adicionados os comandos `cognitiveservices account network-rule`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1626">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="3c5b0-1627">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1627">Cosmos DB</span></span>

* <span data-ttu-id="3c5b0-1628">Removido o aviso ao atualizar vários locais de gravação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1628">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="3c5b0-1629">Foram adicionados os comandos CRUD para o CosmosDB SQL, MongoDB, Cassandra, Gremlin e Recursos de tabela e taxa de transferência do recurso</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1629">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="3c5b0-1630">HDInsight</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1630">HDInsight</span></span>

<span data-ttu-id="3c5b0-1631">Esta versão contém um grande número de alterações da falha.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1631">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="3c5b0-1632">[ALTERAÇÃO SIGNIFICATIVA] Parâmetros renomeados para `hdinsight create`:</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1632">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="3c5b0-1633">`--storage-default-container` renomeado para `--storage-container`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1633">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="3c5b0-1634">`--storage-default-filesystem` renomeado para `--storage-filesystem`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1634">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="3c5b0-1635">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--name` de `application create` foi alterado para representar o nome do aplicativo em vez do nome do cluster</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1635">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="3c5b0-1636">O argumento `--cluster-name` foi adicionado a `application create` para substituir a funcionalidade `--name` antiga</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1636">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="3c5b0-1637">[ALTERAÇÃO SIGNIFICATIVA] Parâmetros renomeados para `application create`:</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1637">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="3c5b0-1638">`--application-type` renomeado para `--type`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1638">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="3c5b0-1639">`--marketplace-identifier` renomeado para `--marketplace-id`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1639">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="3c5b0-1640">`--https-endpoint-access-mode` renomeado para `--access-mode`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1640">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="3c5b0-1641">Renomeado de `--https-endpoint-destination-port` para `--destination-port`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1641">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="3c5b0-1642">[ALTERAÇÃO SIGNIFICATIVA] Parâmetros removidos para `application create`:</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1642">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="3c5b0-1643">[ALTERAÇÃO DA FALHA] Renomeado de `--target-instance-count` para `--workernode-count` para `hdinsight resize`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1643">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="3c5b0-1644">[ALTERAÇÃO SIGNIFICATIVA] Todos os comandos no grupo `hdinsight script-action` foram alterados para usar o parâmetro `--name` como o nome da ação de script.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1644">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="3c5b0-1645">O argumento `--cluster-name` foi adicionado a todos os comandos `hdinsight script-action` para substituir a funcionalidade `--name` antiga</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1645">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="3c5b0-1646">[ALTERAÇÃO SIGNIFICATIVA] Renomeado de `--script-execution-id` para `--execution-id` para todos os comandos `hdinsight script-action`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1646">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="3c5b0-1647">[ALTERAÇÃO SIGNIFICATIVA]`hdinsight script-action show` renomeado para `hdinsight script-action show-execution-details`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1647">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="3c5b0-1648">[ALTERAÇÃO DA FALHA] Os parâmetros foram alterados para `hdinsight script-action execute --roles` para serem separados por espaços em vez de separados por vírgula</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1648">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="3c5b0-1649">[ALTERAÇÃO SIGNIFICATIVA] O parâmetro `--persisted` de `hdinsight script-action list` foi removido</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1649">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="3c5b0-1650">O parâmetro `hdinsight create --cluster-configurations` foi alterado para aceitar um caminho para um arquivo JSON local ou uma cadeia de caracteres JSON</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1650">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="3c5b0-1651">Adicionado o comando `hdinsight script-action list-execution-history`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1651">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="3c5b0-1652">Alterado `hdinsight monitor enable --workspace` para aceitar uma ID do workspace ou nome do workspace do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1652">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="3c5b0-1653">O argumento `hdinsight monitor enable --primary-key`, que será necessário caso uma ID do workspace seja fornecida como o parâmetro, foi adicionado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1653">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="3c5b0-1654">Foram adicionados mais exemplos e atualização das descrições das mensagens de erro</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1654">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="3c5b0-1655">Interativo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1655">Interactive</span></span>

* <span data-ttu-id="3c5b0-1656">Um erro no carregamento foi corrigido</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1656">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="3c5b0-1657">Kubernetes</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1657">Kubernetes</span></span>

* <span data-ttu-id="3c5b0-1658">Alterado para usar `https` se a porta do contêiner do painel estiver usando `https`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1658">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-1659">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1659">Network</span></span>

* <span data-ttu-id="3c5b0-1660">O argumento `--yes` foi adicionado a `network dns record-set cname delete`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1660">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="3c5b0-1661">Perfil</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1661">Profile</span></span>

* <span data-ttu-id="3c5b0-1662">O argumento `--resource-type` foi adicionado a `account get-access-token` para obter tokens de acesso de recurso</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1662">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="3c5b0-1663">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1663">ServiceFabric</span></span>

* <span data-ttu-id="3c5b0-1664">Todas as versões de sistema operacional com suporte para criação do cluster sf foram adicionadas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1664">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="3c5b0-1665">Foi corrigido o bug de validação do certificado primário</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1665">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-1666">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1666">Storage</span></span>

* <span data-ttu-id="3c5b0-1667">Adicionado o comando `storage copy`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1667">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="3c5b0-1668">30 de julho de 2019</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1668">July 30, 2019</span></span>

<span data-ttu-id="3c5b0-1669">Versão 2.0.70</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1669">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-1670">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1670">ACR</span></span>

* <span data-ttu-id="3c5b0-1671">Corrigido o problema #9952 (uma regressão no comando `acr pack build`)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1671">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="3c5b0-1672">Removido o nome da imagem do construtor padrão em `acr pack build`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1672">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-1673">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1673">Appservice</span></span>

* <span data-ttu-id="3c5b0-1674">Alterado `webapp config ssl` para mostrar uma mensagem se um recurso não for encontrado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1674">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="3c5b0-1675">Corrigido o problema em que `functionapp create` não aceita o tipo de conta de armazenamento `Standard_RAGRS`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1675">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="3c5b0-1676">Corrigido um problema em que `webapp up` falharia se fosse executado usando versões mais antigas do Python</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1676">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-1677">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1677">Network</span></span>

* <span data-ttu-id="3c5b0-1678">Removido parâmetro inválido `--ids` de `network nic ip-config add` (corrige o #9861)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1678">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="3c5b0-1679">Corrige o #9604.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1679">Fixes #9604.</span></span> <span data-ttu-id="3c5b0-1680">Adicionado o parâmetro `--root-certs` ao `network application-gateway http-settings [create|update]` para dar suporte a certificados raiz confiáveis associados ao usuário.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1680">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="3c5b0-1681">Fixado argumento `--subscription` para `network dns record-set ns create` (#9965)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1681">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="3c5b0-1682">RBAC</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1682">RBAC</span></span>

* <span data-ttu-id="3c5b0-1683">Adicionado o comando `user update`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1683">Added `user update` command</span></span>
* <span data-ttu-id="3c5b0-1684">[PRETERIDO] Preterido `--upn-or-object-id` de comandos relacionados ao usuário</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1684">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="3c5b0-1685">Usar argumento de substituição `--id`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1685">Use replacement argument `--id`</span></span>
* <span data-ttu-id="3c5b0-1686">Adicionado argumento `--id` para comandos relacionados ao usuário</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1686">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="3c5b0-1687">SQL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1687">SQL</span></span>

* <span data-ttu-id="3c5b0-1688">Adicionados comandos de gerenciamento para chaves de instância gerenciada e protetor de TDE</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1688">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-1689">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1689">Storage</span></span>

* <span data-ttu-id="3c5b0-1690">Adicionado o comando `storage remove`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1690">Added `storage remove` command</span></span>
* <span data-ttu-id="3c5b0-1691">Corrigido um problema com `storage blob update`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1691">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="3c5b0-1692">VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1692">VM</span></span>

* <span data-ttu-id="3c5b0-1693">Alterado `list-skus` para usar versão de API mais recente a fim de externar detalhes de zona</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1693">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="3c5b0-1694">Alterado o padrão de `--single-placement-group` para `false` para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1694">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="3c5b0-1695">Adicionada a capacidade de selecionar SKUs de armazenamento ZRS para `[snapshot|disk] create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1695">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="3c5b0-1696">Adicionado novo grupo de comandos `vm host` para dar suporte a hosts dedicados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1696">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="3c5b0-1697">Adicionados parâmetros `--host` e `--host-group` em `vm create` para definir o host dedicado da VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1697">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="3c5b0-1698">16 de julho de 2019</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1698">July 16, 2019</span></span>

<span data-ttu-id="3c5b0-1699">Versão 2.0.69</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1699">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-1700">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1700">Appservice</span></span>

* <span data-ttu-id="3c5b0-1701">Os comandos `webapp identity` foram alterados para retornar uma mensagem de erro apropriada se o nome do aplicativo ou ResourceGroupName for inválido</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1701">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="3c5b0-1702">`webapp list` corrigido para retornar o valor correto para numberOfSites se nenhum ResourceGroup foi fornecido</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1702">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="3c5b0-1703">Corrigidos os efeitos colaterais de `appservice plan create` e `webapp create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1703">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="3c5b0-1704">Núcleo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1704">Core</span></span>

* <span data-ttu-id="3c5b0-1705">Corrigido um problema em que `--subscription` aparecia apesar de não ser aplicável</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1705">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="3c5b0-1706">Lote</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1706">Batch</span></span>

* <span data-ttu-id="3c5b0-1707">[ALTERAÇÃO SIGNIFICATIVA]`batch pool node-agent-skus list` foi substituído por `batch pool supported-images list`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1707">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="3c5b0-1708">Adicionado suporte para regras de segurança bloqueando o acesso de rede a um pool com base na porta de origem do tráfego ao usar a opção `--json-file` de `batch pool create network`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1708">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="3c5b0-1709">Suporte adicionado para executar a tarefa no diretório de trabalho de contêiner ou no diretório de trabalho de tarefa em lotes ao usar a opção `--json-file` de `batch task create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1709">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="3c5b0-1710">Corrigido o erro na opção `--application-package-references` de `batch pool create` em que ela funcionaria apenas com padrões</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1710">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="3c5b0-1711">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1711">Eventhubs</span></span>

* <span data-ttu-id="3c5b0-1712">Adicionada validação para o parâmetro `--rights` dos comandos `authorizationrule`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1712">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="3c5b0-1713">RDBMS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1713">RDBMS</span></span>

* <span data-ttu-id="3c5b0-1714">Adicionado um parâmetro opcional para especificar a réplica de SKU para criar o comando de réplica</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1714">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="3c5b0-1715">Corrigido o problema com a falha no teste de CI com a criação de réplica de MySQL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1715">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="3c5b0-1716">Retransmissão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1716">Relay</span></span>

* <span data-ttu-id="3c5b0-1717">Corrigido o problema com a conexão híbrida quando a autorização do cliente desabilitava [#8775](https://github.com/azure/azure-cli/issues/8775)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1717">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="3c5b0-1718">Parâmetro `--requires-transport-security` adicionado a `relay wcfrelay create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1718">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="3c5b0-1719">Barramento de serviço</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1719">Servicebus</span></span>

* <span data-ttu-id="3c5b0-1720">Adicionada validação para o parâmetro `--rights` dos comandos `authorizationrule`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1720">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-1721">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1721">Storage</span></span>

* <span data-ttu-id="3c5b0-1722">Habilitar AADDS de arquivos para atualização da conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1722">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="3c5b0-1723">Problema corrigido `storage blob service-properties update --set`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1723">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="3c5b0-1724">2 de julho de 2019</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1724">July 2, 2019</span></span>

<span data-ttu-id="3c5b0-1725">Versão 2.0.68</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1725">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="3c5b0-1726">Núcleo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1726">Core</span></span>

* <span data-ttu-id="3c5b0-1727">Agora, os módulos de comando são consolidados em um único Python distribuível.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1727">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="3c5b0-1728">Isso substitui o uso direto de muitos pacotes `azure-cli-` no PyPI.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1728">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="3c5b0-1729">Assim, o tamanho da instalação será reduzido e apenas os usuários que tiverem instalado diretamente por meio do `pip` serão afetados.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1729">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-1730">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1730">ACR</span></span>

* <span data-ttu-id="3c5b0-1731">Foi adicionado o suporte para gatilhos de temporizador para tarefa</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1731">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-1732">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1732">Appservice</span></span>

* <span data-ttu-id="3c5b0-1733">O `functionapp create` foi alterado para habilitar o Application Insights por padrão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1733">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="3c5b0-1734">[ALTERAÇÃO SIGNIFICATIVA] Foi removido o comando `functionapp devops-build` preterido.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1734">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="3c5b0-1735">Agora, use o novo comando `az functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1735">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="3c5b0-1736">Foi adicionado o suporte ao plano de aplicativo de funções Consumo em Linux ao `functionapp deployment config-zip`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1736">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="3c5b0-1737">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1737">Cosmos DB</span></span>

* <span data-ttu-id="3c5b0-1738">Foi adicionado o suporte para desabilitar a TTL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1738">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="3c5b0-1739">DLS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1739">DLS</span></span>

* <span data-ttu-id="3c5b0-1740">Versão atualizada do ADLS (0.0.45)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1740">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="3c5b0-1741">Comentários</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1741">Feedback</span></span>

* <span data-ttu-id="3c5b0-1742">Ao relatar um comando de extensão com falha, agora, o `az feedback` tenta abrir o navegador na URL do projeto/repositório da extensão por meio do índice</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1742">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="3c5b0-1743">HDInsight</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1743">HDInsight</span></span>

* <span data-ttu-id="3c5b0-1744">[ALTERAÇÃO SIGNIFICATIVA] O nome do grupo de comandos `oms` foi alterado para `monitor`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1744">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="3c5b0-1745">[ALTERAÇÃO SIGNIFICATIVA]`--http-password/-p` tornou-se um parâmetro obrigatório</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1745">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="3c5b0-1746">Foram adicionados preenchedores para o preenchedor dos parâmetros `--cluster-admin-account` e `cluster-users-group-dns`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1746">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="3c5b0-1747">O parâmetro `cluster-users-group-dns` foi alterado para ser obrigatório quando `—esp` estiver presente</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1747">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="3c5b0-1748">Foi adicionado um tempo limite para todos os preenchedores automáticos de argumento existentes</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1748">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="3c5b0-1749">Foi adicionado um tempo limite para transformar o nome do recurso na ID de recurso</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1749">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="3c5b0-1750">Os preenchedores automáticos foram alterados para selecionar recursos de qualquer grupo de recursos.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1750">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="3c5b0-1751">Pode ser um grupo de recursos diferente daquele especificado com `-g`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1751">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="3c5b0-1752">Foi adicionado o suporte para os parâmetros `--sub-domain-suffix` e `--disable_gateway_auth` no comando `hdinsight application create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1752">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="3c5b0-1753">Serviços gerenciados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1753">Managed Services</span></span>

* <span data-ttu-id="3c5b0-1754">Introdução ao módulo de comando de serviço gerenciado em versão prévia</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1754">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="3c5b0-1755">Perfil</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1755">Profile</span></span>
* <span data-ttu-id="3c5b0-1756">Suprimir o argumento `--subscription` para o comando de logoff</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1756">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="3c5b0-1757">RBAC</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1757">RBAC</span></span>

* <span data-ttu-id="3c5b0-1758">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--password` foi removido de `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1758">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="3c5b0-1759">Foi adicionado o parâmetro `--assignee-principal-type` ao comando `create` para evitar falhas intermitentes causadas pela latência de replicação do servidor do AAD Graph</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1759">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="3c5b0-1760">Foi corrigida uma falha em `ad signed-in-user` ao listar objetos de propriedade</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1760">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="3c5b0-1761">Foi corrigido um problema em que o `ad sp` não localizava o aplicativo certo de uma entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1761">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="3c5b0-1762">RDBMS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1762">RDBMS</span></span>

* <span data-ttu-id="3c5b0-1763">Foi adicionado o suporte à replicação para o MariaDB</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1763">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="3c5b0-1764">SQL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1764">SQL</span></span>

* <span data-ttu-id="3c5b0-1765">Valores permitidos documentados para `sql db create --sample-name`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1765">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-1766">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1766">Storage</span></span>

* <span data-ttu-id="3c5b0-1767">Foi adicionado o suporte ao token SAS de delegação de usuário com `--as-user` para `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1767">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="3c5b0-1768">Foi adicionado o suporte ao token SAS de delegação de usuário com `--as-user` para `storage container generate-sas`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1768">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="3c5b0-1769">VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1769">VM</span></span>

* <span data-ttu-id="3c5b0-1770">Foi corrigido o bug em que o `vmss create` retornava uma mensagem de erro quando era executado com `--no-wait`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1770">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="3c5b0-1771">Foi removida a validação do lado do cliente de `vmss create --single-placement-group`.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1771">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="3c5b0-1772">Não falha quando `--single-placement-group` é definido como `true` e `--instance-count` é maior que 100 ou quando são especificadas zonas de disponibilidade, mas deixa essa validação para o serviço de computação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1772">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="3c5b0-1773">Foi corrigido o bug em que o `[vm|vmss] extension image list` falhava quando era usado com `--latest`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1773">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="3c5b0-1774">18 de junho de 2019</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1774">June 18, 2019</span></span>

<span data-ttu-id="3c5b0-1775">Versão 2.0.67</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1775">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="3c5b0-1776">Núcleo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1776">Core</span></span>

<span data-ttu-id="3c5b0-1777">Esta versão apresenta uma nova marca [Versão prévia] para comunicar com mais clareza aos clientes quando um comando, um grupo de comandos ou um argumento está no status de versão prévia.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1777">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="3c5b0-1778">Anteriormente, essa informação era transmitida no texto de ajuda ou, implicitamente, pelo número da versão do módulo de comando.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1778">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="3c5b0-1779">A CLI removerá os números de versão dos pacotes individuais no futuro.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1779">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="3c5b0-1780">Se um comando estiver em versão prévia, todos os seus argumentos também estarão.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1780">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="3c5b0-1781">Se um grupo de comandos for rotulado com o status de versão prévia, então todos os seus comandos e argumentos também serão considerados em versão prévia.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1781">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="3c5b0-1782">Como resultado dessa alteração, diversos grupos de comandos podem parecer surgir "de repente" com o status de versão prévia com esta liberação.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1782">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="3c5b0-1783">O que realmente aconteceu é que a maioria dos pacotes já estava com status de versão prévia, mas estão sendo consideradas GA com esta liberação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1783">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-1784">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1784">ACR</span></span>
* <span data-ttu-id="3c5b0-1785">Adicionado o comando 'acr check-health'</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1785">Added 'acr check-health' command</span></span>
* <span data-ttu-id="3c5b0-1786">Melhorado o tratamento de erro para tokens do AAD e para recuperar comandos externos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1786">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="3c5b0-1787">ACS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1787">ACS</span></span>
* <span data-ttu-id="3c5b0-1788">Comandos preteridos do ACS agora ficam ocultos da exibição da ajuda</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1788">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="3c5b0-1789">AMS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1789">AMS</span></span>
* <span data-ttu-id="3c5b0-1790">[ALTERAÇÃO SIGNIFICATIVA] Alterada para retornar cadeias de caracteres de tempo da ISO 8601 para archive-window-length e key-frame-interval-duration</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1790">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-1791">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1791">AppService</span></span>
* <span data-ttu-id="3c5b0-1792">Adicionado roteamento com base no local para `webapp deleted list` e `webapp deleted restore`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1792">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="3c5b0-1793">Corrigido problema em que a URL de destino registrada do webapp ("Não é possível iniciar o aplicativo em...") não era clicável no Azure Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1793">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="3c5b0-1794">Corrigido um problema em que a criação de aplicativos com algumas SKUs falhava com um erro de AlwaysOn</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1794">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="3c5b0-1795">Adicionada a pré-validação para o `[appservice|webapp] create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1795">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="3c5b0-1796">Corrigido o `[webapp|functionapp] traffic-routing` para usar o actionHostName correto</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1796">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="3c5b0-1797">Adicionado o suporte de slot para comandos `functionapp`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1797">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="3c5b0-1798">Lote</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1798">Batch</span></span>
* <span data-ttu-id="3c5b0-1799">Corrigida a regressão de autenticação do AAD causada pela geração de relatórios de erros superagressiva para autenticação de chave compartilhada</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1799">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="3c5b0-1800">BatchAI</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1800">BatchAI</span></span>
* <span data-ttu-id="3c5b0-1801">Agora os comandos do BatchAI estão preteridos e ocultos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1801">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="3c5b0-1802">BotService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1802">BotService</span></span>
* <span data-ttu-id="3c5b0-1803">Adição das mensagens de aviso "suporte descontinuado"/"modo de manutenção" para os comandos compatíveis com a v3 do SDK</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1803">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="3c5b0-1804">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1804">CosmosDB</span></span>
* <span data-ttu-id="3c5b0-1805">[PRETERIDO] Preterido o comando `cosmosdb list-keys`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1805">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="3c5b0-1806">Adicionado o comando `cosmosdb keys list` – substitui o `cosmosdb list-keys`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1806">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="3c5b0-1807">`cosmsodb create/update`: Adicionado novo formato para --location a fim de permitir a configuração da propriedade "isZoneRedundant".</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1807">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="3c5b0-1808">Formato antigo preterido</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1808">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="3c5b0-1809">EventGrid</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1809">EventGrid</span></span>
* <span data-ttu-id="3c5b0-1810">Adicionados comandos do `eventgrid domain` para operações de CRUD no domínio</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1810">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="3c5b0-1811">Adicionados comandos do `eventgrid domain topic` para operações de CRUD nos tópicos do domínio</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1811">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="3c5b0-1812">Adicionado argumento do `--odata-query` ao `eventgrid [topic|event-subscription] list` para filtrar os resultados usando a sintaxe do OData</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1812">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="3c5b0-1813">`event-subscription create/update`: Adicionado o servicebusqueue como novos valores para o parâmetro `--endpoint-type`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1813">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="3c5b0-1814">[ALTERAÇÃO SIGNIFICATIVA] Removido o suporte para `--included-event-types All` com `eventgrid event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1814">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="3c5b0-1815">HDInsight</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1815">HDInsight</span></span>
* <span data-ttu-id="3c5b0-1816">Adicionado suporte para o parâmetro `--ssh-public-key` no comando `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1816">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="3c5b0-1817">IoT</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1817">IoT</span></span>
* <span data-ttu-id="3c5b0-1818">Adicionado suporte para regenerar as chaves da política de autorização</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1818">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="3c5b0-1819">Adicionados SDK e suporte para o serviço de provisionamento de repositórios do DigitalTwin</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1819">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-1820">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1820">Network</span></span>
* <span data-ttu-id="3c5b0-1821">Adicionado suporte de zona para o Gateway da NAT</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1821">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="3c5b0-1822">Adicionado o comando `network list-service-tags`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1822">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="3c5b0-1823">Corrigido o problema com o `dns zone import` em que os usuários não conseguiam importar registros do curinga A</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1823">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="3c5b0-1824">Corrigido o problema com o `watcher flow-log configure` em que o registro de fluxo não podia ser habilitado em determinadas regiões</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1824">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="3c5b0-1825">Recurso</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1825">Resource</span></span>
* <span data-ttu-id="3c5b0-1826">Adicionado o comando do `az rest` para fazer chamadas REST</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1826">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="3c5b0-1827">Corrigido o erro ao usar o `policy assignment list` com um grupo de recursos ou o nível de assinatura `--scope`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1827">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="3c5b0-1828">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1828">ServiceBus</span></span>
* <span data-ttu-id="3c5b0-1829">Corrigido o problema com o `servicebus topic create --max-size`[nº9319](https://github.com/azure/azure-cli/issues/9319)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1829">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="3c5b0-1830">SQL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1830">SQL</span></span>
* <span data-ttu-id="3c5b0-1831">Alterado o `--location` para ser opcional para `sql [server|mi] create` – usa o local do grupo de recursos se não especificado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1831">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="3c5b0-1832">Corrigido o erro "objeto 'NoneType' não é iterável" para `sql db list-editions --available`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1832">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="3c5b0-1833">SQLVm</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1833">SQLVm</span></span>
* <span data-ttu-id="3c5b0-1834">[ALTERAÇÃO DA FALHA] Alterado `sql vm create` para exigir o parâmetro `--license-type`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1834">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="3c5b0-1835">Alterado para permitir a configuração da SKU da imagem do SQL ao criar ou atualizar uma VM do SQL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1835">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-1836">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1836">Storage</span></span>
* <span data-ttu-id="3c5b0-1837">Corrigido o problema com a chave de conta ignorada para `storage container generate-sas`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1837">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="3c5b0-1838">Corrigido o problema com o `storage blob sync` no Linux</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1838">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="3c5b0-1839">VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1839">VM</span></span>
* <span data-ttu-id="3c5b0-1840">[VERSÃO PRÉVIA] Adicionados os comandos `vm image template` para criar imagens de VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1840">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="3c5b0-1841">4 de junho de 2019</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1841">June 4, 2019</span></span>

<span data-ttu-id="3c5b0-1842">Versão 2.0.66</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1842">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="3c5b0-1843">Núcleo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1843">Core</span></span>
* <span data-ttu-id="3c5b0-1844">Foi corrigido o bug em que os comandos falhavam quando `--output yaml` era usado com `--query`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1844">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-1845">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1845">ACR</span></span>
* <span data-ttu-id="3c5b0-1846">Foi adicionado o grupo de comando 'pack acr' para a criação de Tarefas de build rápida usando Buildpacks.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1846">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="3c5b0-1847">ACS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1847">ACS</span></span>
* <span data-ttu-id="3c5b0-1848">Permitir a opção de habilitar/desabilitar o complemento kube-dashboard do AKS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1848">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="3c5b0-1849">Imprimir uma mensagem amigável quando a assinatura não estiver na lista de permissões para usar o Red Hat OpenShift no Azure</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1849">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="3c5b0-1850">Lote</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1850">Batch</span></span>
* <span data-ttu-id="3c5b0-1851">Melhoria no tratamento de erro quando você não está conectado a uma conta \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1851">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="3c5b0-1852">IoT</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1852">IoT</span></span>
* <span data-ttu-id="3c5b0-1853">Foi adicionado o suporte para failover manual</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1853">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-1854">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1854">Network</span></span>
* <span data-ttu-id="3c5b0-1855">Foram adicionados os comandos `network application-gateway waf-policy` para oferecer suporte às regras de WAF personalizadas.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1855">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="3c5b0-1856">Adicionados os argumentos `--waf-policy` e `--max-capacity` para `network application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1856">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="3c5b0-1857">Recurso</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1857">Resource</span></span>
* <span data-ttu-id="3c5b0-1858">Melhoria da mensagem de erro do `deployment create` quando não há nenhum TTY disponível</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1858">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="3c5b0-1859">Função</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1859">Role</span></span>
* <span data-ttu-id="3c5b0-1860">O texto da Ajuda foi atualizado.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1860">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="3c5b0-1861">Computação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1861">Compute</span></span>
* <span data-ttu-id="3c5b0-1862">Foi adicionado o suporte para `vm create` para as VMs de uma imagem gerenciada com LUNs de disco de dados que não começam em 0 ou que ignoram números</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1862">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="3c5b0-1863">21 de maio de 2019</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1863">May 21, 2019</span></span>

<span data-ttu-id="3c5b0-1864">Versão 2.0.65</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1864">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="3c5b0-1865">Núcleo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1865">Core</span></span>
* <span data-ttu-id="3c5b0-1866">Foram adicionados comentários melhores para erros de autenticação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1866">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="3c5b0-1867">Corrigido um problema em que a CLI carregava extensões que não eram compatíveis com a versão do núcleo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1867">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="3c5b0-1868">Corrigido um problema com a inicialização quando `clouds.config` está corrompido</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1868">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-1869">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1869">ACR</span></span>
* <span data-ttu-id="3c5b0-1870">Foi adicionado suporte das Identidades Gerenciadas para Tarefas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1870">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="3c5b0-1871">ACS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1871">ACS</span></span>
* <span data-ttu-id="3c5b0-1872">Corrigido o comando `openshift create` quando usado com o cliente AAD do consumidor</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1872">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-1873">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1873">AppService</span></span>
* <span data-ttu-id="3c5b0-1874">[PRETERIDO] Preterido o comando `functionapp devops-build` – Será removido na próxima versão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1874">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="3c5b0-1875">`functionapp devops-pipeline` foi alterado para buscar o log de build do Azure DevOps no modo detalhado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1875">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="3c5b0-1876">[ALTERAÇÃO SIGNIFICATIVA] O sinalizador `--use_local_settings` foi removido do comando `functionapp devops-pipeline` – não estava operacional</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1876">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="3c5b0-1877">`webapp up` foi alterado para retornar uma saída JSON se `--logs` não for usado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1877">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="3c5b0-1878">Foi adicionado suporte para escrever recursos padrão para a configuração local de `webapp up`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1878">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="3c5b0-1879">Foi adicionado suporte para `webapp up` reimplantar um aplicativo sem usar o argumento `--location`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1879">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="3c5b0-1880">Corrigido um problema em que o valor do SKU gratuito não funcionava na criação do ASP do SKU gratuito do Linux</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1880">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="3c5b0-1881">BotService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1881">BotService</span></span>
* <span data-ttu-id="3c5b0-1882">Alterado para permitir todas as capitalizações para parâmetros `--lang` em todos os comandos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1882">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="3c5b0-1883">Descrição atualizada do módulo de comando</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1883">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="3c5b0-1884">Consumo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1884">Consumption</span></span>
* <span data-ttu-id="3c5b0-1885">O parâmetro obrigatório ausente foi adicionado para executar `consumption usage list --billing-period-name`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1885">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="3c5b0-1886">IoT</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1886">IoT</span></span>
* <span data-ttu-id="3c5b0-1887">Suporte adicionado para listar todas as chaves</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1887">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-1888">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1888">Network</span></span>
* [ALTERAÇÃO SIGNIFICATIVA]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="3c5b0-1890">O argumento `--nat-gateway` foi adicionado a `network vnet subnet [create|update]` para anexar a um gateway NAT</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1890">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="3c5b0-1891">Corrigido o problema de `dns zone import`, em que os nomes de registro não correspondiam ao tipo de registro</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1891">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="3c5b0-1892">RDBMS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1892">RDBMS</span></span>
* <span data-ttu-id="3c5b0-1893">Suporte a postgres e mysql adicionado para replicação geográfica</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1893">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="3c5b0-1894">RBAC</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1894">RBAC</span></span>
* <span data-ttu-id="3c5b0-1895">Adição de suporte do escopo de grupo de gerenciamento a `role assignment`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1895">Added support for management group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-1896">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1896">Storage</span></span>
* <span data-ttu-id="3c5b0-1897">`storage blob sync`: adicionar um comando de sincronização ao armazenamento de blobs</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1897">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="3c5b0-1898">Computação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1898">Compute</span></span>
* <span data-ttu-id="3c5b0-1899">`--computer-name` foi adicionado a `vm create` para configurar o nome do computador da VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1899">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="3c5b0-1900">`--ssh-key-value` foi renomeado para `--ssh-key-values` para `[vm|vmss] create` – Agora, pode aceitar vários valores de chave pública ou caminhos ssh</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1900">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="3c5b0-1901">__Observação__ : Isso **não** é uma alteração da falha – `--ssh-key-value` será analisado corretamente, pois corresponde somente a `--ssh-key-values`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1901">__Note__ : This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="3c5b0-1902">O argumento `--type` de `ppg create` foi alterado para ser opcional</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1902">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="3c5b0-1903">6 de maio de 2019</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1903">May 6, 2019</span></span>

<span data-ttu-id="3c5b0-1904">Versão 2.0.64</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1904">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="3c5b0-1905">ACS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1905">ACS</span></span>
* <span data-ttu-id="3c5b0-1906">[ALTERAÇÃO SIGNIFICATIVA] O sinalizador `--fqdn` foi removido dos comandos `openshift`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1906">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="3c5b0-1907">Alterado para usar a versão da API do Red Hat OpenShift no Azure em disponibilidade geral</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1907">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="3c5b0-1908">O sinalizador `customer-admin-group-id` foi adicionado a `openshift create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1908">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="3c5b0-1909">[GA] `(PREVIEW)` foi removido da opção `aks create``--network-policy`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1909">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-1910">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1910">Appservice</span></span>
* <span data-ttu-id="3c5b0-1911">[PRETERIDO] O comando `functionapp devops-build` foi preterido</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1911">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="3c5b0-1912">Renomeado para `functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1912">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="3c5b0-1913">Corrigido ao obter o nome de usuário correto para cloudshell que estava causando a falha em `webapp up`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1913">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="3c5b0-1914">Documentação `appservice plan --sku` atualizada para refletir o appserviceplans com suporte</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1914">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="3c5b0-1915">Adicionado argumentos opcionais para o grupo de recursos e plano a `webapp up`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1915">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="3c5b0-1916">Adicionado suporte a `webapp ssh` para respeitar a variável de ambiente `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1916">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="3c5b0-1917">Adicionado suporte `appserviceplan create` para a SKU gratuita do Linux</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1917">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="3c5b0-1918">Alterado `webapp up` para ter uma suspensão de 30 segundos depois de definir appsetting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` para lidar com a inicialização a frio kudu</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1918">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="3c5b0-1919">Adicionado suporte para runtime `powershell` a `functionapp create` no Windows</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1919">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="3c5b0-1920">Adicionado o comando `create-remote-connection`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1920">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="3c5b0-1921">Lote</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1921">Batch</span></span>
* <span data-ttu-id="3c5b0-1922">Corrigido o bug no validador para as opções `--application-package-references`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1922">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="3c5b0-1923">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1923">Botservice</span></span>
* <span data-ttu-id="3c5b0-1924">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v4 -k webapp` foi alterado para criar um Bot de Aplicativo Web vazio por padrão (ou seja, nenhum bot será implantado no Serviço de Aplicativo)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1924">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="3c5b0-1925">O sinalizador `--echo` foi adicionado ao `bot create` para usar o comportamento antigo com `-v v4`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1925">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="3c5b0-1926">[ALTERAÇÃO SIGNIFICATIVA] O valor padrão de `--version` foi alterado para `v4`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1926">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="3c5b0-1927">__OBSERVAÇÃO:__ `bot prepare-publish` ainda usa o padrão antigo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1927">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="3c5b0-1928">[ALTERAÇÃO SIGNIFICATIVA]`--lang` foi alterado para não definir mais `Csharp` como padrão.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1928">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="3c5b0-1929">Se o comando exigir `--lang` e ele não for fornecido, o comando será um erro</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1929">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="3c5b0-1930">[ALTERAÇÃO SIGNIFICATIVA] Os argumentos `--appid` e `--password` foram alterados para `bot create` ser obrigatório e agora podem ser criados por meio de `ad app create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1930">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="3c5b0-1931">Foi adicionada validação a `--appid` e `--password`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1931">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="3c5b0-1932">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v4` foi alterado para não criar ou usar uma Conta de Armazenamento ou o Application Insights</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1932">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="3c5b0-1933">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v3` foi alterado para exigir uma região em que o Application Insights está disponível</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1933">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="3c5b0-1934">[ALTERAÇÃO SIGNIFICATIVA] O `bot update` foi alterado para afetar somente as propriedades específicas de um bot</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1934">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="3c5b0-1935">[ALTERAÇÃO SIGNIFICATIVA] Os sinalizadores `--lang` foram alterados para aceitar `Javascript` em vez de `Node`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1935">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="3c5b0-1936">[ALTERAÇÃO SIGNIFICATIVA] O `Node` foi removido como um valor `--lang` permitido</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1936">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="3c5b0-1937">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v4 -k webapp` foi alterado para não definir mais `SCM_DO_BUILD_DURING_DEPLOYMENT` como verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1937">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="3c5b0-1938">Todas as implantações por meio do Kudu atuarão de acordo com o comportamento padrão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1938">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="3c5b0-1939">O `bot download` foi alterado para os bots sem arquivos `.bot` para criar o arquivo de configuração específico a um idioma com os valores das Configurações de Aplicativo do bot</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1939">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="3c5b0-1940">Adicionado o suporte `Typescript` para `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1940">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="3c5b0-1941">Uma mensagem de aviso foi adicionada a `bot prepare-deploy` para os bots `Javascript` e `Typescript` para quando `--code-dir` não contiver `package.json`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1941">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="3c5b0-1942">O `bot prepare-deploy` foi alterado para retornar `true`, se bem-sucedido</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1942">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="3c5b0-1943">O log detalhado foi adicionado a `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1943">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="3c5b0-1944">Mais regiões disponíveis do Application Insights foram adicionadas ao `az bot create -v v3`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1944">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="3c5b0-1945">Configurar</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1945">Configure</span></span>
* <span data-ttu-id="3c5b0-1946">Adicionado suporte para configurações de valor padrão do argumento baseado em pasta</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1946">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="3c5b0-1947">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1947">Eventhubs</span></span>
* <span data-ttu-id="3c5b0-1948">Adicionados os comandos `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1948">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="3c5b0-1949">O argumento `--default-action` foi adicionado às regras de rede de `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1949">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-1950">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1950">Network</span></span>
* <span data-ttu-id="3c5b0-1951">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--cache` foi substituído por `--defer` para `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1951">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="3c5b0-1952">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1952">Policy Insights</span></span>
* <span data-ttu-id="3c5b0-1953">Suporte adicionado a `--expand PolicyEvaluationDetails` para detalhes de avaliação de política de consulta no recurso</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1953">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="3c5b0-1954">Função</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1954">Role</span></span>
* <span data-ttu-id="3c5b0-1955">[PRETERIDO] Alterado argumento ocultar '--password' `create-for-rbac` - suporte será removido em maio de 2019</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1955">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="3c5b0-1956">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1956">Service Bus</span></span>
* <span data-ttu-id="3c5b0-1957">Adicionados os comandos `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1957">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="3c5b0-1958">O argumento `--default-action` foi adicionado às regras de rede de `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1958">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="3c5b0-1959">`topic [create|update]` foi fixado para permitir suporte a `--max-size` para valores de 10, 20, 40 e 80 GB com a SKU Premium</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1959">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="3c5b0-1960">SQL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1960">SQL</span></span>
* <span data-ttu-id="3c5b0-1961">Adicionados os comandos `sql virtual-cluster [list|show|delete]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1961">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="3c5b0-1962">VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1962">VM</span></span>
* <span data-ttu-id="3c5b0-1963">O `--protect-from-scale-in` e o `--protect-from-scale-set-actions` foram adicionados a `vmss update` para habilitar atualizações à política de proteção das instâncias de VM VMSS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1963">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="3c5b0-1964">Adicionado a `--instance-id` e `vmss update` para habilitar atualização genérica das instâncias de VM VMSS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1964">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="3c5b0-1965">`--instance-id` foi adicionado a `vmss wait`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1965">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="3c5b0-1966">Adição do novo grupo de comandos `ppg` para gerenciar Grupos de Posicionamento de Proximidade</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1966">Added new `ppg` command group for managing Proximity Placement Groups</span></span>
* <span data-ttu-id="3c5b0-1967">Adicionado a `--ppg`, `[vm|vmss] create` e `vm availability-set create` para gerenciar PPGs</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1967">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="3c5b0-1968">Parâmetro `--hyper-v-generation` adicionado a `image create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1968">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="3c5b0-1969">23 de abril de 2019</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1969">April 23, 2019</span></span>

<span data-ttu-id="3c5b0-1970">Versão 2.0.63</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1970">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="3c5b0-1971">ACS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1971">ACS</span></span>
* <span data-ttu-id="3c5b0-1972">Alterado `aks get-credentials` para solicitar substituição dos valores duplicados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1972">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="3c5b0-1973">Removido `(PREVIEW)` dos comandos de espaços de desenvolvimento "aks use-dev-espaces" e "aks remove-dev-espaces"</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1973">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="3c5b0-1974">AMS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1974">AMS</span></span>
* <span data-ttu-id="3c5b0-1975">Corrigido o bug com a atualização de filtros de conta e de ativo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1975">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-1976">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1976">AppService</span></span>
* <span data-ttu-id="3c5b0-1977">Adicionado suporte para o ASE e o tempo limite para `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1977">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="3c5b0-1978">Adicionado suporte para o estabelecimento de CI CD em um pipeline do Azure DevOps de um repositório do Github para aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1978">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="3c5b0-1979">Adicionado argumento `--github-pat` a `functionapp devops-build create` para aceitar o token de acesso pessoal do Github</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1979">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="3c5b0-1980">Adicionado argumento `--github-repository` a `functionapp devops-build create` para aceitar o repositório Github que contém um código-fonte functionapp</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1980">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="3c5b0-1981">Problema corrigido em que `az webapp up --logs` estava falhando com um erro e atualização da versão .NETCORE padrão para 2.1</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1981">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="3c5b0-1982">Configurações de functionapp desnecessárias removidas durante a criação de um aplicativo de funções com plano de consumo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1982">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="3c5b0-1983">Alterado `webapp up` para que a cadeia de caracteres padrão asp agora acrescente o número no final para criar um novo ASP com base nas opções de SKU</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1983">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="3c5b0-1984">Adicionado `-b` como uma opção a `webapp up` para iniciar o aplicativo no navegador</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1984">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="3c5b0-1985">Alterado `webapp deployment source config zip` para lidar com a variável de ambiente `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1985">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="3c5b0-1986">Gerenciador de Implantação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1986">Deployment Manager</span></span>
* <span data-ttu-id="3c5b0-1987">[VERSÃO PRÉVIA] Criar e gerenciar artefatos que dão suporte a distribuições</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1987">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="3c5b0-1988">Laboratório</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1988">Lab</span></span>
* <span data-ttu-id="3c5b0-1989">Corrigido o bug que causa uma saída inicial</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1989">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-1990">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1990">Network</span></span>
* <span data-ttu-id="3c5b0-1991">Adicionada delegação de servidor de nome automática a `dns zone create` no pai durante a criação da zona filho</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1991">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="3c5b0-1992">Recurso</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1992">Resource</span></span>
* <span data-ttu-id="3c5b0-1993">[PRETERIDO] Argumentos `--link-id`, `--target-id` e `--filter-string` preteridos de `resource link`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1993">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="3c5b0-1994">Use os argumentos `--link`, `--target` e `--filter`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1994">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="3c5b0-1995">Corrigido o problema em que os comandos `resource link [create|update]` não funcionavam</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1995">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="3c5b0-1996">Corrigido um problema em que a exclusão usando uma ID de recurso poderia causar falha no erro</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1996">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="3c5b0-1997">SQL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1997">SQL</span></span>
* <span data-ttu-id="3c5b0-1998">Adicionado suporte para fuso horário personalizado nas instâncias gerenciadas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1998">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="3c5b0-1999">Alterado para permitir que o nome do pool Elástico seja usado com `sql db update`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-1999">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="3c5b0-2000">Adicionado o suporte `--no-wait` para `sql server [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2000">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="3c5b0-2001">Adicionado o comando `sql server wait`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2001">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-2002">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2002">Storage</span></span>
* <span data-ttu-id="3c5b0-2003">Corrigido o problema com tokens SAS com codificação dupla em `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2003">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="3c5b0-2004">VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2004">VM</span></span>
* <span data-ttu-id="3c5b0-2005">Adicionado sinalizador `--skip-shutdown` a `vm|vmss stop` para desligar as VMs sem o desligamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2005">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="3c5b0-2006">Adicionado argumento `--storage-account-type` a `sig image-version create` para definir o tipo de conta do perfil de publicação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2006">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="3c5b0-2007">Adicionado argumento `--target-regions` a `sig image-version create` para permitir definir os tipos de conta de armazenamento específico da região</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2007">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="3c5b0-2008">9 de abril de 2019</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2008">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="3c5b0-2009">Núcleo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2009">Core</span></span>
* <span data-ttu-id="3c5b0-2010">Correção do problema em que algumas extensões mostraram uma versão do `Unknown` e não podiam ser atualizadas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2010">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-2011">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2011">ACR</span></span>
* <span data-ttu-id="3c5b0-2012">Adição de suporte para execução de uma imagem sem contexto</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2012">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="3c5b0-2013">AMS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2013">AMS</span></span>
* [PRETERIDO]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [ALTERAÇÃO SIGNIFICATIVA]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="3c5b0-2016">Adição de suporte para novos parâmetros de criptografia em `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2016">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="3c5b0-2017">Adição de novo parâmetro `--filters` a `ams streaming-locator create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2017">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-2018">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2018">AppService</span></span>
* <span data-ttu-id="3c5b0-2019">Adicionado o suporte `--logs` para `webapp up`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2019">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="3c5b0-2020">Correção de problemas do comando `functionapp devops-build create` de geração de `azure-pipelines.yml`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2020">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="3c5b0-2021">Melhoria do tratamento de erros e indicadores `unctionapp devops-build create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2021">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="3c5b0-2022">[ALTERAÇÃO SIGNIFICATIVA] Remoção do sinalizador `--local-git` para o comando `devops-build`; a detecção de git local e a manipulação são obrigatórias para a criação de pipelines do Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2022">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="3c5b0-2023">Adição de suporte para a criação de planos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2023">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="3c5b0-2024">Adição da capacidade de trocar um plano sob um aplicativo de funções usando `functionapp update --plan`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2024">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="3c5b0-2025">Adição de suporte para configurações de expansão de plano Premium do Azure Functions</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2025">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="3c5b0-2026">CDN</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2026">CDN</span></span>
* <span data-ttu-id="3c5b0-2027">Adição de suporte para `Microsoft_Standard` e `Standard_ChinaCdn`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2027">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="3c5b0-2028">Comentários</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2028">Feedback</span></span>
* <span data-ttu-id="3c5b0-2029">Alteração de `feedback` para mostrar metadados em comandos executados recentemente</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2029">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="3c5b0-2030">Alteração de `feedback` para solicitar o auxílio do usuário no processo de criação de problema abrindo um navegador e usando um modelo de problema</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2030">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="3c5b0-2031">Alteração do `feedback` para imprimir o corpo do problema ao executar com '--verbose'</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2031">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="3c5b0-2032">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2032">Monitor</span></span>
* <span data-ttu-id="3c5b0-2033">Correção de um problema em que “count” não era um valor permitido com `metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2033">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="3c5b0-2034">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2034">Network</span></span>
* <span data-ttu-id="3c5b0-2035">Correção do formato de tabela que não estava sendo exibido com `vnet-gateway list-bgp-peer-status`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2035">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="3c5b0-2036">Adição dos comandos `list-request-headers` e `list-response-headers` para `application-gateway rewrite-rule`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2036">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="3c5b0-2037">Adição do comando `list-server-variables` para `application-gateway rewrite-rule condition`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2037">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="3c5b0-2038">Correção de um problema em que a atualização do estado do link em uma porta express-route geraria uma exceção de atributo desconhecido `express-route port update`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2038">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="3c5b0-2039">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2039">PrivateDNS</span></span>
* <span data-ttu-id="3c5b0-2040">Adição de `network private-dns` para zonas de DNS privado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2040">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="3c5b0-2041">Recurso</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2041">Resource</span></span>
* <span data-ttu-id="3c5b0-2042">Correção do problema com `deployment create` e `group deployment create`, em que um arquivo de parâmetros com um conjunto vazio de parâmetros não funcionaria</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2042">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="3c5b0-2043">Função</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2043">Role</span></span>
* <span data-ttu-id="3c5b0-2044">Correção de `create-for-rbac` para lidar corretamente com `--years`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2044">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="3c5b0-2045">[ALTERAÇÃO SIGNIFICATIVA] Alteração de `role assignment delete` para solicitar ao excluir todas as atribuições na assinatura incondicionalmente</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2045">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="3c5b0-2046">SQL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2046">SQL</span></span>
* <span data-ttu-id="3c5b0-2047">Atualização de `sql mi [create|update]` com as propriedades proxyOverride e publicDataEndpointEnabled</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2047">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-2048">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2048">Storage</span></span>
* <span data-ttu-id="3c5b0-2049">[ALTERAÇÃO SIGNIFICATIVA] Remoção do resultado de `storage blob delete`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2049">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="3c5b0-2050">Adição de `--full-uri` a `storage blob generate-sas` para criar o URI completo para o blob com SAS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2050">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="3c5b0-2051">Adição de `--file-snapshot` a `storage file copy start` para copiar arquivo do instantâneo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2051">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="3c5b0-2052">Alteração de `storage blob copy cancel` para mostrar apenas o erro em vez da exceção para NoPendingCopyOperation</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2052">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="3c5b0-2053">26 de março de 2019</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2053">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="3c5b0-2054">Núcleo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2054">Core</span></span>
* <span data-ttu-id="3c5b0-2055">Correção de problemas com incompatibilidade da extensão de desenvolvimento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2055">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="3c5b0-2056">Agora o tratamento de erros encaminha os clientes para a página de problemas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2056">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="3c5b0-2057">Nuvem</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2057">Cloud</span></span>
* <span data-ttu-id="3c5b0-2058">Erro de “assinatura não encontrada” corrigido em `cloud set`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2058">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-2059">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2059">ACR</span></span>
* <span data-ttu-id="3c5b0-2060">Corrigidas fontes redundantes na importação de imagem.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2060">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="3c5b0-2061">`--auth-mode` adicionado aos comandos `acr build`, `acr run`, `acr task create` e `acr task update`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2061">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="3c5b0-2062">Grupo de comandos “acr task credential” adicionado para gerenciar as credenciais de uma Tarefa</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2062">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="3c5b0-2063">“--no-wait” adicionado ao comando `acr build`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2063">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-2064">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2064">AppService</span></span>
* <span data-ttu-id="3c5b0-2065">Bug corrigido onde `webapp up` não estava lidando corretamente com a execução do diretório vazio ou do cenário de código desconhecido</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2065">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="3c5b0-2066">Bug corrigido onde os slots não funcionavam para `[webapp|functionapp] config ssl bind`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2066">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="3c5b0-2067">Serviço de BOT</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2067">BOT Service</span></span>
* <span data-ttu-id="3c5b0-2068">`bot prepare-deploy` adicionado para se preparar para a implantação de bots via `webapp`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2068">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="3c5b0-2069">`bot create --kind registration` alterado para mostrar a senha se ela não for fornecida</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2069">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="3c5b0-2070">[ALTERAÇÃO SIGNIFICATIVA]`--endpoint` alterado em `bot create --kind registration` como padrão para uma cadeia de caracteres vazia, em vez de ser requerido</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2070">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="3c5b0-2071">Adicionado `SCM_DO_BUILD_DURING_DEPLOYMENT` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2071">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="3c5b0-2072">CDN</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2072">CDN</span></span>
* <span data-ttu-id="3c5b0-2073">Adicionado o suporte ao `--no-wait` para `cdn endpoint [create|update|start|stop|delete|load|purge]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2073">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* [ALTERAÇÃO SIGNIFICATIVA]: `cdn endpoint create` alterado para o comportamento de cache da cadeia de consulta padrão.
[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour. <span data-ttu-id="3c5b0-2075">Não há mais padrão para "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2075">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="3c5b0-2076">Agora, ele é definido pelo serviço</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2076">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="3c5b0-2077">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2077">Cosmosdb</span></span>
* <span data-ttu-id="3c5b0-2078">Suporte adicionado para `--enable-multiple-write-locations` na atualização da conta</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2078">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="3c5b0-2079">O subgrupo `network-rule` foi adicionado com os comandos `add`, `remove` e `list` para gerenciar as regras de VNET de uma conta do Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2079">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="3c5b0-2080">Interativo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2080">Interactive</span></span>
* <span data-ttu-id="3c5b0-2081">Incompatibilidade corrigida com a extensão Interativa instalada por meio do azdev</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2081">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="3c5b0-2082">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2082">Monitor</span></span>
* <span data-ttu-id="3c5b0-2083">Alterado para permitir o valor de dimensão `*` para `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2083">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-2084">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2084">Network</span></span>
* <span data-ttu-id="3c5b0-2085">Grupo de comandos `rewrite-rule` adicionado em `application-gateway`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2085">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="3c5b0-2086">Perfil</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2086">Profile</span></span>
* <span data-ttu-id="3c5b0-2087">Suporte de conta no nível do locatário para a identidade de serviço gerenciado adicionado em `login`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2087">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="3c5b0-2088">Postgres</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2088">Postgres</span></span> 
* <span data-ttu-id="3c5b0-2089">Adicionados os comandos postgresql `replica` e `restart server`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2089">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="3c5b0-2090">Alterado para obter o local padrão do grupo de recursos quando não fornecido para criar servidores e adicionar validação para os dias de retenção</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2090">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="3c5b0-2091">Recurso</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2091">Resource</span></span>
* <span data-ttu-id="3c5b0-2092">Saída da tabela aperfeiçoada para `deployment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2092">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="3c5b0-2093">Corrigido o problema com `deployment [create|validate]` onde o tipo secureObject não era reconhecido</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2093">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="3c5b0-2094">Grafo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2094">Graph</span></span>
* <span data-ttu-id="3c5b0-2095">Adicionado o suporte ao `--end-date` para `ad [app|sp] credential reset`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2095">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="3c5b0-2096">Suporte adicionado para acrescentar permissões com `ad app permission add`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2096">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="3c5b0-2097">Bug corrigido com `ad app permission list` quando não havia nenhuma permissão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2097">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="3c5b0-2098">`ad sp delete` alterado para ignorar a exclusão da atribuição de função se a conta atual não tem nenhuma assinatura</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2098">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="3c5b0-2099">`ad app create` alterado para `--identifier-uris` passar para lista vazia como padrão se não fornecido</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2099">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-2100">armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2100">storage</span></span>
* <span data-ttu-id="3c5b0-2101">`--snapshot` adicionado a `storage file download-batch` para baixar de um instantâneo de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2101">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="3c5b0-2102">Barra de progresso `storage blob [download-batch|upload-batch]` alterada para ser menos detalhada e indicar o blob atual</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2102">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="3c5b0-2103">Problema corrigido com `storage account update` ao atualizar os parâmetros de criptografia</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2103">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="3c5b0-2104">Problema corrigido onde `storage blob show` falharia ao usar o oauth (`--auth-mode=login`)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2104">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="3c5b0-2105">VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2105">VM</span></span>
* <span data-ttu-id="3c5b0-2106">Adicionado o comando `image update`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2106">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="3c5b0-2107">12 de março de 2019</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2107">March 12, 2019</span></span>

<span data-ttu-id="3c5b0-2108">Versão 2.0.60</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2108">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="3c5b0-2109">Núcleo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2109">Core</span></span>

* <span data-ttu-id="3c5b0-2110">Foi corrigido um erro incorreto no `cloud set` sobre assinatura não encontrada.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2110">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-2111">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2111">ACR</span></span>

* <span data-ttu-id="3c5b0-2112">Corrigidas fontes redundantes na importação de imagem.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2112">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="3c5b0-2113">ACS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2113">ACS</span></span>

* <span data-ttu-id="3c5b0-2114">Alteração para ignorar o parâmetro `--listen-address` para `aks browse` se ele não for compatível com kubectl</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2114">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="3c5b0-2115">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2115">AppService</span></span>

* <span data-ttu-id="3c5b0-2116">Adicionado `[webapp|functionapp] deployment list-publishing-credentials` para obter a URL de publicação do Kudu e suas credenciais.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2116">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="3c5b0-2117">Removida a instrução de impressão errônea de `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2117">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="3c5b0-2118">Corrigido `functionapp` para definir a imagem correta do runtime nos planos do Serviço de Aplicativo no Linux.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2118">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="3c5b0-2119">Removida a marca de versão prévia do `webapp up` e adicionadas melhorias ao comando.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2119">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="3c5b0-2120">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2120">Botservice</span></span>

* <span data-ttu-id="3c5b0-2121">Adicionado `SCM_DO_BUILD_DURING_DEPLOYMENT` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2121">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="3c5b0-2122">Adicionados `Microsoft-BotFramework-AppId` e `Microsoft-BotFramework-AppPassword` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2122">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="3c5b0-2123">Removidas as aspas simples da saída de comando `bot publish`, no final de `bot create`.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2123">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="3c5b0-2124">Alterado `bot publish` para que seja assíncrono.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2124">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="3c5b0-2125">Contêiner</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2125">Container</span></span>

* <span data-ttu-id="3c5b0-2126">Adicionado o argumento `--no-wait` para `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2126">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="3c5b0-2127">EventHub</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2127">EventHub</span></span>

* <span data-ttu-id="3c5b0-2128">Adicionado o sinalizador `--skip-empty-archives` a `eventhub create|update` para dar suporte a arquivos vazios na captura.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2128">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="3c5b0-2129">Localizar</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2129">Find</span></span>

* <span data-ttu-id="3c5b0-2130">Atualização de funcionalidade principal</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2130">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="3c5b0-2131">HDInsight</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2131">HDInsight</span></span>

* <span data-ttu-id="3c5b0-2132">Adicionado o parâmetro `--storage-account-managed-identity` a `hdinsight create` para oferecer suporte ao MSI do ADLS Gen2.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2132">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-2133">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2133">Network</span></span>

* <span data-ttu-id="3c5b0-2134">Corrigido o problema com `vpn-connection update`, onde a atualização de uma conexão VPN entre gateways em assinaturas diferentes falharia.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2134">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="3c5b0-2135">Rdbms</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2135">Rdbms</span></span>

* <span data-ttu-id="3c5b0-2136">Correções secundárias para obter a localização padrão do grupo de recursos, quando não fornecida, para criar servidores e adicionar validação nos dias de retenção.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2136">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="3c5b0-2137">Função</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2137">Role</span></span>

* <span data-ttu-id="3c5b0-2138">Corrigido `role definition update` para usar ID a fim de resolver a definição corretamente.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2138">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="3c5b0-2139">Alterado `ad app credential reset` para remover a suposição de que a entidade de serviço do aplicativo já existe.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2139">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="3c5b0-2140">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2140">Service Fabric</span></span>

* <span data-ttu-id="3c5b0-2141">Corrigido o problema com o fato de `sf cluster list` não ser iterável.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2141">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="3c5b0-2142">26 de fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2142">February 26, 2019</span></span>

<span data-ttu-id="3c5b0-2143">Versão 2.0.59</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2143">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="3c5b0-2144">Núcleo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2144">Core</span></span>

* <span data-ttu-id="3c5b0-2145">Corrigido o problema onde algumas instâncias usando `--subscription NAME` produziriam uma exceção</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2145">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-2146">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2146">ACR</span></span>

* <span data-ttu-id="3c5b0-2147">Parâmetro `--target` adicionado para os comandos `acr build`, `acr task create` e `acr task update`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2147">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="3c5b0-2148">Melhor tratamento de erros para os comandos de execução quando não conectado ao Azure</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2148">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="3c5b0-2149">ACS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2149">ACS</span></span>

* <span data-ttu-id="3c5b0-2150">Opção `--listen-address` adicionada a `aks port-forward`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2150">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-2151">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2151">AppService</span></span>

* <span data-ttu-id="3c5b0-2152">Adicionado o comando `functionapp devops-build`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2152">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="3c5b0-2153">Lote</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2153">Batch</span></span>
* <span data-ttu-id="3c5b0-2154">[ALTERAÇÃO SIGNIFICATIVA] Comando `batch pool upgrade os` removido</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2154">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="3c5b0-2155">[ALTERAÇÃO SIGNIFICATIVA] Propriedade `Pacakges` removida das respostas `Application`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2155">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="3c5b0-2156">Comando `batch application package list` adicionado para listar os pacotes de um aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2156">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="3c5b0-2157">[ALTERAÇÃO SIGNIFICATIVA]`--application-id` alterado para `--application-name` em todos os comandos `batch application`,</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2157">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="3c5b0-2158">O argumento `--json-file` foi adicionado aos comandos para a solicitação de resposta da API bruta</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2158">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="3c5b0-2159">Validação atualizada para incluir automaticamente `https://` em todos os pontos de extremidade, se ausente</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2159">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="3c5b0-2160">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2160">CosmosDB</span></span>

* <span data-ttu-id="3c5b0-2161">O subgrupo `network-rule` foi adicionado com os comandos `add`, `remove` e `list` para gerenciar as regras de VNET de uma conta do Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2161">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="3c5b0-2162">Kusto</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2162">Kusto</span></span>

* <span data-ttu-id="3c5b0-2163">[ALTERAÇÃO SIGNIFICATIVA] Os tipos `hot_cache_period` e `soft_delete_period` foram alterados do banco de dados para o formato de duração ISO8601</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2163">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-2164">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2164">Network</span></span>

* <span data-ttu-id="3c5b0-2165">Adicionado o argumento `--express-route-gateway-bypass` para `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2165">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="3c5b0-2166">Foram adicionados os grupos de comando a partir das extensões `express-route`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2166">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="3c5b0-2167">Os grupos de comando `express-route gateway` e `express-route port` foram adicionados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2167">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="3c5b0-2168">Adicionado o argumento `--legacy-mode` para `express-route peering [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2168">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="3c5b0-2169">Os argumentos `--allow-classic-operations` e `--express-route-port` foram adicionados a `express-route [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2169">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="3c5b0-2170">Adicionado o argumento `--gateway-default-site` para `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2170">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="3c5b0-2171">Os comandos `ipsec-policy` foram adicionados a `vnet-gateway`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2171">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="3c5b0-2172">Recurso</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2172">Resource</span></span>

* <span data-ttu-id="3c5b0-2173">Foi corrigido o problema com `deployment create` em que o campo do tipo diferencia letras maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2173">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="3c5b0-2174">Foi adicionado o suporte para arquivo de parâmetros de URI a `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2174">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="3c5b0-2175">Foi adicionado o suporte para parâmetros de URI e definições a `policy set-definition update`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2175">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="3c5b0-2176">Foi corrigido o tratamento de parâmetros e regras para `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2176">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="3c5b0-2177">Foi corrigido o problema com `resource show/update/delete/tag/invoke-action` em que as IDs de assinatura cruzada não respeitaram corretamente a ID da assinatura</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2177">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="3c5b0-2178">Função</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2178">Role</span></span>

* <span data-ttu-id="3c5b0-2179">Foi adicionado o suporte para as funções do aplicativo a `ad app [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2179">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="3c5b0-2180">VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2180">VM</span></span>

* <span data-ttu-id="3c5b0-2181">Foi corrigido o problema com `vm create where ` – a rede acelerada não foi habilitada por padrão no Ubuntu 18.0</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2181">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="3c5b0-2182">12 de fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2182">February 12, 2019</span></span>

<span data-ttu-id="3c5b0-2183">Versão 2.0.58</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2183">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="3c5b0-2184">Núcleo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2184">Core</span></span>

* <span data-ttu-id="3c5b0-2185">`az --version` agora exibe uma notificação se você tiver pacotes para atualização</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2185">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="3c5b0-2186">A regressão em que `--ids` não pode ser usado com a saída JSON foi corrigida</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2186">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-2187">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2187">ACR</span></span>
* <span data-ttu-id="3c5b0-2188">[ALTERAÇÃO SIGNIFICATIVA] O grupo de comandos `acr build-task` foi removido</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2188">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="3c5b0-2189">[ALTERAÇÃO SIGNIFICATIVA] As opções `--tag` e `--manifest` de `acr repository delete` foram removidas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2189">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="3c5b0-2190">ACS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2190">ACS</span></span>
* <span data-ttu-id="3c5b0-2191">Suporte adicionado a `aks [enable-addons|disable-addons]` para nomes que não diferenciam maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2191">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="3c5b0-2192">Suporte adicionado para a operação de atualização do Azure Active Directory usando `aks update-credentials --reset-aad`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2192">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="3c5b0-2193">Um esclarecimento informando que `--output` é ignorado para `aks get-credentials` foi adicionado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2193">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="3c5b0-2194">AMS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2194">AMS</span></span>
* <span data-ttu-id="3c5b0-2195">Adicionados os comandos `ams streaming-endpoint [start | stop | create | update] wait`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2195">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="3c5b0-2196">Adicionados os comandos `ams live-event [create | start | stop | reset] wait`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2196">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-2197">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2197">Appservice</span></span>
* <span data-ttu-id="3c5b0-2198">Foi adicionada a capacidade de criar e configurar funções usando contêineres de ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2198">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="3c5b0-2199">Suporte adicionado para a atualização das configurações de aplicativos Web por meio de JSON</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2199">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="3c5b0-2200">A ajuda foi aprimorada para `appservice-plan-update`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2200">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="3c5b0-2201">Suporte adicionado para o App Insights para auxiliar na criação de aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2201">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="3c5b0-2202">Os problemas com o SSH do aplicativo Web foram corrigidos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2202">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="3c5b0-2203">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2203">Botservice</span></span>
* <span data-ttu-id="3c5b0-2204">A experiência do usuário para `bot publish` foi aprimorada</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2204">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="3c5b0-2205">Foram adicionados avisos de tempos limite ao executar `npm install` durante `az bot publish`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2205">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="3c5b0-2206">O caractere inválido `.` de `--name` em `az bot create` foi removido</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2206">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="3c5b0-2207">Alteração para interromper a geração aleatória de nomes de recursos durante a criação do Armazenamento do Azure, Plano do Serviço de Aplicativo, Aplicativo Web/de funções e Application Insights</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2207">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="3c5b0-2208">[PRETERIDO] O argumento `--proj-name` foi preterido em favor de `--proj-file-path`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2208">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="3c5b0-2209">`az bot publish` foi alterado para remover arquivos de implantação do Node.js do IIS buscados, caso eles já não existissem</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2209">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="3c5b0-2210">Foi adicionado o argumento `--keep-node-modules` para `az bot publish` para não excluir a pasta `node_modules` no Serviço de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2210">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="3c5b0-2211">O par chave-valor `"publishCommand"` foi adicionado à saída de `az bot create` durante a criação de uma função do Azure ou bot de aplicativo Web</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2211">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="3c5b0-2212">O valor de `"publishCommand"` é um comando `az bot publish` que é automaticamente preenchido com os parâmetros necessários para publicar o bot recém-criado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2212">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="3c5b0-2213">O `"WEBSITE_NODE_DEFAULT_VERSION"` foi atualizado no modelo do ARM para que os bots de SDK v4 usem 10.14.1 em vez de 8.9.4</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2213">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="3c5b0-2214">Key Vault</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2214">Key Vault</span></span>
* <span data-ttu-id="3c5b0-2215">Foi corrigido o problema com `keyvault secret backup`, em que alguns usuários recebiam um erro `unexpected_keyword` ao usar `--id`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2215">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="3c5b0-2216">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2216">Monitor</span></span>
* <span data-ttu-id="3c5b0-2217">`monitor metrics alert [create|update]` foi alterado para permitir o valor dimensional `*`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2217">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-2218">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2218">Network</span></span>
* <span data-ttu-id="3c5b0-2219">`dns zone export` foi alterado para garantir que CNAMEs exportados fossem FQDNs</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2219">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="3c5b0-2220">O parâmetro `--gateway-name` foi adicionado a `nic ip-config address-pool [add|remove]` para dar suporte a pools de endereços de back-end de gateway de aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2220">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="3c5b0-2221">Os argumentos `--traffic-analytics` e `--workspace` foram adicionados a `network watcher flow-log configure` para dar suporte à análise de tráfego por meio de um espaço de trabalho do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2221">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="3c5b0-2222">`--idle-timeout` e `--floating-ip` foram adicionados a `lb inbound-nat-pool [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2222">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="3c5b0-2223">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2223">Policy Insights</span></span>
* <span data-ttu-id="3c5b0-2224">Os comandos `policy remediation` foram adicionados para dar suporte a recursos de correção de política de recursos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2224">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="3c5b0-2225">RDBMS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2225">RDBMS</span></span>
* <span data-ttu-id="3c5b0-2226">A mensagem e os parâmetros de comando de ajuda foram aprimorados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2226">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="3c5b0-2227">Redis</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2227">Redis</span></span>
* <span data-ttu-id="3c5b0-2228">Foram adicionados comandos para gerenciar regras de firewall (criar, atualizar, excluir, mostrar, listar)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2228">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="3c5b0-2229">Foram adicionados comandos para gerenciar links do servidor (criar, excluir, mostrar, listar)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2229">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="3c5b0-2230">Foram adicionados comandos para gerenciar o agendamento de patches (criar, atualizar, excluir, mostrar)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2230">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="3c5b0-2231">Suporte adicionado para Zonas de Disponibilidade e versão mínima de TLS para criar Redis</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2231">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="3c5b0-2232">[ALTERAÇÃO SIGNIFICATIVA] Os comandos `redis update-settings` e `redis list-all` foram removidos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2232">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="3c5b0-2233">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro para `redis create`: “configurações de locatário” não é aceito no formato chave[=valor]</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2233">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="3c5b0-2234">[PRETERIDO] Uma mensagem de aviso foi adicionada para preterir o comando `redis import-method`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2234">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="3c5b0-2235">Função</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2235">Role</span></span>
* <span data-ttu-id="3c5b0-2236">[ALTERAÇÃO SIGNIFICATIVA] O comando `az identity` foi movido dos comandos `vm` para esta localização</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2236">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="3c5b0-2237">SQL VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2237">SQL VM</span></span>
* <span data-ttu-id="3c5b0-2238">[PRETERIDO] O argumento `--boostrap-acc-pwd` foi preterido devido a um erro de digitação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2238">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="3c5b0-2239">VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2239">VM</span></span>
* <span data-ttu-id="3c5b0-2240">`vm list-skus` foi alterado para permitir o uso de `--all` no lugar de `--all true`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2240">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="3c5b0-2241">Adicionado `vmss run-command [invoke | list | show]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2241">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="3c5b0-2242">Foi corrigido o bug em que `vmss encryption enable` falhava se fosse executado anteriormente</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2242">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="3c5b0-2243">[ALTERAÇÃO SIGNIFICATIVA] O comando `az identity` foi movido para os comandos `role`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2243">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="3c5b0-2244">31 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2244">January 31, 2019</span></span>

<span data-ttu-id="3c5b0-2245">Versão 2.0.57</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2245">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="3c5b0-2246">Núcleo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2246">Core</span></span>

* <span data-ttu-id="3c5b0-2247">Hotfix para o [problema 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2247">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="3c5b0-2248">28 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2248">January 28, 2019</span></span>

<span data-ttu-id="3c5b0-2249">Versão 2.0.56</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2249">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-2250">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2250">ACR</span></span>
* <span data-ttu-id="3c5b0-2251">Suporte adicionado para regras de rede virtual/IP</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2251">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="3c5b0-2252">ACS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2252">ACS</span></span>
* <span data-ttu-id="3c5b0-2253">Adicionada visualização dos nós virtuais</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2253">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="3c5b0-2254">Comandos do OpenShift gerenciado foram adicionados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2254">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="3c5b0-2255">Suporte adicionado para operações de atualização da entidade de serviço com `aks update-credentials -reset-service-principal`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2255">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="3c5b0-2256">AMS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2256">AMS</span></span>
* <span data-ttu-id="3c5b0-2257">[ALTERAÇÃO SIGNIFICATIVA]`ams asset get-streaming-locators` renomeado para `ams asset list-streaming-locators`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2257">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="3c5b0-2258">[ALTERAÇÃO SIGNIFICATIVA]`ams streaming-locator get-content-keys` renomeado para `ams streaming-locator list-content-keys`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2258">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-2259">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2259">Appservice</span></span>
* <span data-ttu-id="3c5b0-2260">Suporte adicionado para o App Insights no `functionapp create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2260">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="3c5b0-2261">Suporte adicionado para a criação do plano de serviço de aplicativo (incluindo Elástico Premium) para Aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2261">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="3c5b0-2262">Foram corrigidos os problemas com de configuração de aplicativo com os planos Elástico Premium</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2262">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="3c5b0-2263">Contêiner</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2263">Container</span></span>
* <span data-ttu-id="3c5b0-2264">Adicionado o comando `container start`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2264">Added `container start` command</span></span>
* <span data-ttu-id="3c5b0-2265">Alteração para permitir o uso de valores decimais para CPU durante a criação do contêiner</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2265">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="3c5b0-2266">EventGrid</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2266">EventGrid</span></span>
* <span data-ttu-id="3c5b0-2267">Parâmetro `--deadletter-endpoint` adicionado a `event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2267">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="3c5b0-2268">Storagequeue e hybridconnection foram adicionados como novos valores para 'event-subscription [create|update] --endpoint-type\`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2268">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="3c5b0-2269">Os parâmetros `--max-delivery-attempts` e `--event-ttl` foram adicionados a `event-subscription create` para especificar a política de repetição para eventos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2269">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="3c5b0-2270">Uma mensagem de aviso foi adicionada a `event-subscription [create|update]` quando o webhook como destino for usado para uma assinatura de evento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2270">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="3c5b0-2271">O parâmetro source-resource-id foi adicionado para todos os comandos relacionados a eventos e marcar todos os outros parâmetros relacionados ao recurso de origem como preteridos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2271">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="3c5b0-2272">HDInsight</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2272">HDInsight</span></span>
* <span data-ttu-id="3c5b0-2273">[ALTERAÇÃO SIGNIFICATIVA] Os parâmetros `--virtual-network` e `--subnet-name` de `hdinsight [application] create` foram removidos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2273">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="3c5b0-2274">[ALTERAÇÃO SIGNIFICATIVA]`hdinsight create --storage-account` foi alterado para aceitar o nome ou ID da conta de armazenamento, em vez de pontos de extremidade de blob</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2274">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="3c5b0-2275">Parâmetros `--vnet-name` e `--subnet-name` adicionados a `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2275">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="3c5b0-2276">Suporte adicionado para a criptografia de disco e Enterprise Security Package ao `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2276">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="3c5b0-2277">Adicionado o comando `hdinsight rotate-disk-encryption-key`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2277">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="3c5b0-2278">Adicionado o comando `hdinsight update`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2278">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="3c5b0-2279">IoT</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2279">IoT</span></span>
* <span data-ttu-id="3c5b0-2280">O formato de codificação foi adicionado ao comando routing-endpoint</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2280">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="3c5b0-2281">Kusto</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2281">Kusto</span></span>
* <span data-ttu-id="3c5b0-2282">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2282">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="3c5b0-2283">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2283">Monitor</span></span>
* <span data-ttu-id="3c5b0-2284">A comparação de ID foi alterada para diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2284">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="3c5b0-2285">Perfil</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2285">Profile</span></span>
* <span data-ttu-id="3c5b0-2286">A conta de nível de locatário foi habilitada para a identidade de serviço gerenciada de `login`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2286">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-2287">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2287">Network</span></span>
* <span data-ttu-id="3c5b0-2288">Foi corrigido o problema com `express-route update`: em que o argumento `--bandwidth` era ignorado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2288">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="3c5b0-2289">Foi corrigido o problema com `ddos-protection update` em que definir a compreensão levava ao rastreamento de pilha</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2289">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="3c5b0-2290">Recurso</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2290">Resource</span></span>
* <span data-ttu-id="3c5b0-2291">Suporte adicionado para o arquivo de parâmetros de URI à `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2291">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="3c5b0-2292">Suporte adicionado para a identidade gerenciada à `policy assignment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2292">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="3c5b0-2293">Máquina virtual SQL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2293">SQL Virtual Machine</span></span>
* <span data-ttu-id="3c5b0-2294">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2294">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-2295">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2295">Storage</span></span>
* <span data-ttu-id="3c5b0-2296">Alteração na correção para atualizar apenas as propriedades que são alteradas no mesmo objeto</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2296">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="3c5b0-2297">#8021 foi corrigido, dados binários são codificados em base 64 quando retornados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2297">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="3c5b0-2298">VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2298">VM</span></span>
* <span data-ttu-id="3c5b0-2299">Alteração de `vm encryption enable` para validar o cofre de chaves de criptografia de disco e se esse cofre de chaves de criptografia de chave existe</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2299">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="3c5b0-2300">O sinalizador `--force` foi adicionado a `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2300">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="3c5b0-2301">15 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2301">January 15, 2019</span></span>

<span data-ttu-id="3c5b0-2302">Versão 2.0.55</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2302">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-2303">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2303">ACR</span></span>
* <span data-ttu-id="3c5b0-2304">Alteração para permitir forçar o envio por push de um gráfico Helm que não existe</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2304">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="3c5b0-2305">Alteração para permitir operações de runtime sem solicitações ARM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2305">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="3c5b0-2306">[PRETERIDO] O parâmetro `--resource-group` foi preterido nos comandos:</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2306">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="3c5b0-2307">ACS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2307">ACS</span></span>
* <span data-ttu-id="3c5b0-2308">Suporte adicionado para novas regiões ACI</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2308">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-2309">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2309">Appservice</span></span>
* <span data-ttu-id="3c5b0-2310">Foi corrigido o problema com o carregamento de certificados para aplicativos que são hospedados em um ASE, em que o RG do ASE e o RG do aplicativo são diferentes</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2310">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="3c5b0-2311">Alteração de `webapp up` para usar a SKU P1V1 como padrão para Linux</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2311">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="3c5b0-2312">`[webapp|functionapp] deployment source config-zip` foi corrigido para mostrar a mensagem de erro adequada quando uma implantação falhar</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2312">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="3c5b0-2313">Adicionado o comando `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2313">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="3c5b0-2314">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2314">Botservice</span></span>
* <span data-ttu-id="3c5b0-2315">Atualizações de status de implantação foram adicionadas a `bot create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2315">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="3c5b0-2316">Configurar</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2316">Configure</span></span>
* <span data-ttu-id="3c5b0-2317">`none` foi adicionado como um formato de saída configurável</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2317">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="3c5b0-2318">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2318">CosmosDB</span></span>
* <span data-ttu-id="3c5b0-2319">Suporte adicionado para criar o banco de dados com taxa de transferência compartilhada</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2319">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="3c5b0-2320">HDInsight</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2320">HDInsight</span></span>
* <span data-ttu-id="3c5b0-2321">Foram adicionados comandos para o gerenciamento de aplicativos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2321">Added commands for managing applications</span></span>
* <span data-ttu-id="3c5b0-2322">Foram adicionados comandos para o gerenciamento de ações de script</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2322">Added commands for managing script actions</span></span>
* <span data-ttu-id="3c5b0-2323">Foram adicionados comandos para o gerenciamento do Operations Management Suite (OMS)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2323">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="3c5b0-2324">Suporte adicionado para listar a utilização regional ao `hdinsight list-usage`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2324">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="3c5b0-2325">[ALTERAÇÃO SIGNIFICATIVA] O tipo de cluster padrão de `hdinsight create` foi removido</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2325">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-2326">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2326">Network</span></span>
* <span data-ttu-id="3c5b0-2327">Adicionados os argumentos `--custom-headers` e `--status-code-ranges` para `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2327">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="3c5b0-2328">Novos tipos de roteamento foram adicionados: Subrede e múltiplos valores</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2328">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="3c5b0-2329">Adicionados os argumentos `--custom-headers` e `--subnets` para `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2329">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="3c5b0-2330">Foi corrigido o problema no qual fornecer `--vnets ""` a `ddos-protection update` causava um erro</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2330">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="3c5b0-2331">Função</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2331">Role</span></span>
* <span data-ttu-id="3c5b0-2332">[PRETERIDO] O argumento `--password` foi preterido para `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2332">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="3c5b0-2333">Como alternativa, use senhas seguras geradas pela CLI</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2333">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="3c5b0-2334">Segurança</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2334">Security</span></span>
* <span data-ttu-id="3c5b0-2335">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2335">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-2336">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2336">Storage</span></span>
* <span data-ttu-id="3c5b0-2337">[ALTERAÇÃO SIGNIFICATIVA] O número padrão de resultados de `storage [blob|file|container|share] list` foi alterado para 5.000.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2337">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="3c5b0-2338">Use `--num-results *` para o comportamento original de retornar todos os resultados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2338">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="3c5b0-2339">Parâmetro `--marker` adicionado a `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2339">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="3c5b0-2340">Um marcador de log foi adicionado para a próxima página ao STDERR de `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2340">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="3c5b0-2341">O comando `storage blob service-properties update` foi adicionado com suporte para sites estáticos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2341">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="3c5b0-2342">VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2342">VM</span></span>
* <span data-ttu-id="3c5b0-2343">`vm [disk|unmanaged-disk]` e `vmss disk` foram alterados para que tenham parâmetros mais consistentes</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2343">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="3c5b0-2344">Suporte adicionado para referência cruzada de imagem de locatário a `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2344">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="3c5b0-2345">O bug de configuração padrão foi corrigido em `vm diagnostics get-default-config --windows-os`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2345">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="3c5b0-2346">O argumento `--provision-after-extensions` foi adicionado a `vmss extension set` para definir quais extensões deverão ser provisionadas antes da extensão ser definida</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2346">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="3c5b0-2347">O argumento `--replica-count` foi adicionado a `sig image-version update` para definir a contagem de replicação padrão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2347">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="3c5b0-2348">Foi corrigido o bug com `image create --source` em que o disco do sistema operacional de origem era confundido com uma VM do mesmo nome, mesmo se a ID de recurso completa fosse fornecida</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2348">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="3c5b0-2349">20 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2349">December 20, 2018</span></span>

<span data-ttu-id="3c5b0-2350">Versão 2.0.54</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2350">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="3c5b0-2351">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2351">Appservice</span></span>
* <span data-ttu-id="3c5b0-2352">Corrigido o problema que causava falha na reimplantação do `webapp up`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2352">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="3c5b0-2353">Adicionado suporte para listar e restaurar instantâneos de aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2353">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="3c5b0-2354">Adicionado suporte para o sinalizador `--runtime` para aplicativos de funções do Windows</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2354">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="3c5b0-2355">IoT Central</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2355">IoTCentral</span></span>
* <span data-ttu-id="3c5b0-2356">Corrigida a chamada à API do comando de atualização</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2356">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="3c5b0-2357">Função</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2357">Role</span></span>
* <span data-ttu-id="3c5b0-2358">[ALTERAÇÃO SIGNIFICATIVA]`ad [app|sp] list` alterado para listar somente os 100 primeiros objetos por padrão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2358">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="3c5b0-2359">SQL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2359">SQL</span></span>
* <span data-ttu-id="3c5b0-2360">Adicionado suporte para ordenação personalizada nas instâncias gerenciadas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2360">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="3c5b0-2361">VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2361">VM</span></span>
* <span data-ttu-id="3c5b0-2362">Parâmetro `---os-type` adicionado a `disk create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2362">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="3c5b0-2363">18 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2363">December 18, 2018</span></span>

<span data-ttu-id="3c5b0-2364">Versão 2.0.53</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2364">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="3c5b0-2365">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2365">ACR</span></span>
* <span data-ttu-id="3c5b0-2366">Adicionado suporte para importação de imagem de Registros de Contêiner externos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2366">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="3c5b0-2367">Simplificado o layout da tabela para a lista de tarefas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2367">Condensed the table layout for task list</span></span>
* <span data-ttu-id="3c5b0-2368">Adicionado suporte para URLs do Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2368">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="3c5b0-2369">ACS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2369">ACS</span></span>
* <span data-ttu-id="3c5b0-2370">Adicionada visualização dos nós virtuais</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2370">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="3c5b0-2371">Removido “(VISUALIZAÇÃO)” de argumentos do AAD para `aks create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2371">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="3c5b0-2372">[PRETERIDO] Comandos `az acs` preteridos.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2372">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="3c5b0-2373">O serviço ACS será desativado em 31 de janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2373">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="3c5b0-2374">Adicionado suporte da Política de Rede durante a criação de novos clusters AKS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2374">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="3c5b0-2375">Removido o requisito do argumento `--nodepool-name` para `aks scale` se houver apenas um pool de nós</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2375">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-2376">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2376">Appservice</span></span>
* <span data-ttu-id="3c5b0-2377">Corrigido o problema em que `webapp config container` não honra o parâmetro `--slot`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2377">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="3c5b0-2378">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2378">Botservice</span></span>
* <span data-ttu-id="3c5b0-2379">Suporte adicionado para análise do arquivo `.bot` ao chamar `bot show`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2379">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="3c5b0-2380">Corrigido o bug de provisionamento do AppInsights</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2380">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="3c5b0-2381">Corrigido o bug de espaço em branco ao lidar com caminhos de arquivo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2381">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="3c5b0-2382">Reduzidas as chamadas de rede do Kudu</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2382">Reduced Kudu network calls</span></span>
* <span data-ttu-id="3c5b0-2383">Melhorias de UX para comandos gerais</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2383">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="3c5b0-2384">Consumo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2384">Consumption</span></span>
* <span data-ttu-id="3c5b0-2385">Corrigidos os bugs da API de orçamento ao mostrar notificações</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2385">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="3c5b0-2386">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2386">CosmosDB</span></span>
* <span data-ttu-id="3c5b0-2387">Suporte adicionado para atualizar a conta de vários mestres para mestre único</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2387">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="3c5b0-2388">Mapas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2388">Maps</span></span>
* <span data-ttu-id="3c5b0-2389">Adicionado suporte ao SKU S1 para `maps account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2389">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-2390">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2390">Network</span></span>
* <span data-ttu-id="3c5b0-2391">Adicionado suporte para `--format` e `--log-version` para `watcher flow-log configure`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2391">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="3c5b0-2392">Corrigido o problema com `dns zone update` em que usar "" para limpar a resolução e o registro de redes virtuais não funcionava</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2392">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="3c5b0-2393">Recurso</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2393">Resource</span></span>
* <span data-ttu-id="3c5b0-2394">Corrigido o tratamento do parâmetro de escopo para grupos de gerenciamento do `policy assignment [create|list|delete|show|update]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2394">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="3c5b0-2395">Adicionado o novo comando `resource wait`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2395">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-2396">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2396">Storage</span></span>
*  <span data-ttu-id="3c5b0-2397">Adicionada a capacidade de atualizar a versão do esquema de log para serviços de armazenamento no `storage logging update`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2397">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="3c5b0-2398">VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2398">VM</span></span>
* <span data-ttu-id="3c5b0-2399">Corrigida a falha em `vm identity remove` quando a VM especificada não tem nenhuma identidade de serviço gerenciado atribuída</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2399">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="3c5b0-2400">4 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2400">December 4, 2018</span></span>

<span data-ttu-id="3c5b0-2401">Versão 2.0.52</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2401">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="3c5b0-2402">Núcleo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2402">Core</span></span>
* <span data-ttu-id="3c5b0-2403">Adicionado suporte para provisionamento de recursos de locatários cruzados para a entidade de serviço de multilocatários</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2403">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="3c5b0-2404">Corrigido o bug onde as ids enviadas por pipe de um comando com a saída tsv eram analisados incorretamente</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2404">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-2405">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2405">Appservice</span></span>
* <span data-ttu-id="3c5b0-2406">[VERSÃO PRÉVIA] Adicionado o comando `webapp up` que ajuda a criar e implantar conteúdo em aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2406">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="3c5b0-2407">Corrigido um bug no aplicativo com base em contêiner do Windows devido à alteração de back-end</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2407">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-2408">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2408">Network</span></span>
* <span data-ttu-id="3c5b0-2409">Adicionado o argumento `--exclusion` a `application-gateway waf-config set` para dar suporte a exclusões de WAF</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2409">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="3c5b0-2410">Função</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2410">Role</span></span>
* <span data-ttu-id="3c5b0-2411">Adicionado suporte para identificadores personalizados para a credencial de senha</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2411">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="3c5b0-2412">VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2412">VM</span></span>
* <span data-ttu-id="3c5b0-2413">[PRETERIDO] Parâmetro `vm extension [show|wait] --expand` preterido</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2413">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="3c5b0-2414">Adicionado parâmetro `--force` a `vm restart` para reimplantar as VMs sem resposta</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2414">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="3c5b0-2415">Alterado `[vm|vmss] create --authentication-type` para aceitar "todos" para criar uma VM com senha e autenticação SSH</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2415">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="3c5b0-2416">Adicionado parâmetro `image create --os-disk-caching` para definir o cache de disco do sistema operacional para uma imagem</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2416">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="3c5b0-2417">20 de novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2417">November 20, 2018</span></span>

<span data-ttu-id="3c5b0-2418">Versão 2.0.51</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2418">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="3c5b0-2419">Núcleo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2419">Core</span></span>
* <span data-ttu-id="3c5b0-2420">Logon do MSI alterado para não reutilizar o nome da assinatura na identidade</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2420">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-2421">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2421">ACR</span></span>
* <span data-ttu-id="3c5b0-2422">Token de contexto adicionado à etapa da tarefa</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2422">Added context token to task step</span></span>
* <span data-ttu-id="3c5b0-2423">Suporte adicionado para definir segredos na execução do acr para espelhar a tarefa do acr</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2423">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="3c5b0-2424">Suporte aprimorado para `--top` e `--orderby` para os comandos `show-tags` e `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2424">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-2425">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2425">Appservice</span></span>
* <span data-ttu-id="3c5b0-2426">Tempo limite padrão para a implantação do zip alterado para sondar o status aumentado para 5 minutos, também adicionando uma propriedade de tempo limite para personalizar esse valor</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2426">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="3c5b0-2427">Padrão `node_version` atualizado.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2427">Updated the default `node_version`.</span></span> <span data-ttu-id="3c5b0-2428">Redefinir a ação de troca de slots durante uma troca de duas fases preserva todas as configurações do aplicativo e cadeias de conexão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2428">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="3c5b0-2429">Verificação da SKU no lado do cliente removida para o Linux criar o plano do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2429">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="3c5b0-2430">Erro corrigido ao tentar obter o status de implantação do zip</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2430">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="3c5b0-2431">Iot Central</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2431">IotCentral</span></span>
* <span data-ttu-id="3c5b0-2432">Verificação de disponibilidade do subdomínio adicionada ao criar um aplicativo do IoT Central</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2432">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="3c5b0-2433">KeyVault</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2433">KeyVault</span></span>
* <span data-ttu-id="3c5b0-2434">Bug corrigido em que os erros podem ter sido ignorados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2434">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-2435">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2435">Network</span></span>
* <span data-ttu-id="3c5b0-2436">Subcomandos `root-cert` adicionados a `application-gateway` para lidar com os certificados de raiz confiável</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2436">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="3c5b0-2437">Opções `--min-capacity` e `--custom-error-pages` adicionadas a `application-gateway [create|update]`:</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2437">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="3c5b0-2438">`--zones` adicionado para suporte da zona de disponibilidade a `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2438">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="3c5b0-2439">Argumentos `--file-upload-limit`, `--max-request-body-size` e `--request-body-check` a `application-gateway waf-config set` adicionados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2439">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="3c5b0-2440">Rdbms</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2440">Rdbms</span></span>
* <span data-ttu-id="3c5b0-2441">Comandos vnet do mariadb adicionados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2441">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="3c5b0-2442">Rbac</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2442">Rbac</span></span>
* <span data-ttu-id="3c5b0-2443">Um problema corrigido ao tentar atualizar credenciais inalteradas em `ad app update`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2443">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="3c5b0-2444">Avisos de saída adicionados para comunicar alterações de falha em um futuro próximo para `ad [app|sp] list`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2444">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="3c5b0-2445">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2445">Storage</span></span>
* <span data-ttu-id="3c5b0-2446">Melhor manipulação de casos incomuns para os comandos da cópia de armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2446">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="3c5b0-2447">Corrigido o problema em que `storage blob copy start-batch` não usava credenciais de logon quando as contas de origem e destino eram iguais</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2447">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="3c5b0-2448">Bug corrigido com `storage [blob|file] url` em que `sas_token` não foi incorporado na URL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2448">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="3c5b0-2449">Aviso de alteração da falha adicionado a `[blob|container] list`: produzirá apenas os primeiros 5.000 resultados por padrão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2449">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="3c5b0-2450">VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2450">VM</span></span>
* <span data-ttu-id="3c5b0-2451">Suporte adicionado a `[vm|vmss] create --storage-sku` para especificar a SKU da conta de armazenamento para o SO gerenciado e os discos de dados separadamente</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2451">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="3c5b0-2452">Parâmetros do nome da versão alterados de `sig image-version` para `--image-version -e`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2452">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="3c5b0-2453">Argumento `sig image-version` preterido `--image-version-name`, substituído por `--image-version`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2453">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="3c5b0-2454">Suporte adicionado para usar o disco local do SO a `[vm|vmss] create --ephemeral-os-disk`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2454">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="3c5b0-2455">Adicionado o suporte ao `--no-wait` para `snapshot create/update`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2455">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="3c5b0-2456">Adicionado o comando `snapshot wait`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2456">Added `snapshot wait` command</span></span>
* <span data-ttu-id="3c5b0-2457">Suporte adicionado para usar o nome da instância com `[vm|vmss] extension set --extension-instance-name`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2457">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="3c5b0-2458">6 de novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2458">November 6, 2018</span></span>

<span data-ttu-id="3c5b0-2459">Versão 2.0.50</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2459">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="3c5b0-2460">Núcleo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2460">Core</span></span>
* <span data-ttu-id="3c5b0-2461">Foi adicionado suporte para o serviço principal sn + autenticação do emissor</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2461">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-2462">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2462">ACR</span></span>
* <span data-ttu-id="3c5b0-2463">Foi adicionado suporte para eventos de git de solicitação de pull e de confirmação para o gatilho de origem da tarefa</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2463">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="3c5b0-2464">Alterado para usar o padrão do Dockerfile se ele não for especificado no comando de compilação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2464">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="3c5b0-2465">ACS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2465">ACS</span></span>
* <span data-ttu-id="3c5b0-2466">[ALTERAÇÃO SIGNIFICATIVA]`enable_cloud_console_aks_browse` foi removido para habilitar 'az aks browse' por padrão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2466">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="3c5b0-2467">Supervisor</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2467">Advisor</span></span>
* <span data-ttu-id="3c5b0-2468">Versão de GA</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2468">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="3c5b0-2469">AMS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2469">AMS</span></span>
* <span data-ttu-id="3c5b0-2470">Novos grupos de comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2470">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="3c5b0-2471">Novos comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2471">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="3c5b0-2472">Adicionados parâmetros de criptografia com suporte para `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2472">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="3c5b0-2473">O suporte adicionado para `ams transform output remove` agora pode ser executado passando o índice de saída a ser removido</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2473">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="3c5b0-2474">Adicionados os argumentos `--correlation-data` e `--label` ao grupo de comandos `ams job`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2474">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="3c5b0-2475">Adicionados os argumentos `--storage-account` e `--container` ao grupo de comandos `ams asset`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2475">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="3c5b0-2476">Foram adicionados valores padrões para o horário de expiração (agora +23h) e permissões (Leitura) no comando `ams asset get-sas-url`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2476">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="3c5b0-2477">[ALTERAÇÃO SIGNIFICATIVA] O comando `ams streaming locator` foi substituído por `ams streaming-locator`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2477">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="3c5b0-2478">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--content-keys` de `ams streaming locator` foi atualizado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2478">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="3c5b0-2479">[ALTERAÇÃO SIGNIFICATIVA]`--content-policy-name` foi renomeado como `--content-key-policy-name` no comando `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2479">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="3c5b0-2480">[ALTERAÇÃO SIGNIFICATIVA] O comando `ams streaming policy` foi substituído por `ams streaming-policy`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2480">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="3c5b0-2481">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--preset-names` foi substituído por `--preset` no grupo de comandos `ams transform`.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2481">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="3c5b0-2482">Agora, você só pode definir uma saída/predefinição de cada vez (para adicionar mais, é preciso executar `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2482">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="3c5b0-2483">Além disso, você pode definir StandardEncoderPreset personalizado passando o caminho para seu JSON personalizado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2483">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="3c5b0-2484">[ALTERAÇÃO SIGNIFICATIVA]`--output-asset-names ` foi renomeado como `--output-assets` no comando `ams job start`.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2484">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="3c5b0-2485">Agora, ele aceita uma lista separada por espaços dos ativos no formato 'assetName=label'.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2485">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="3c5b0-2486">Um ativo sem rótulo pode ser enviado assim: 'assetName='</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2486">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-2487">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2487">AppService</span></span>
* <span data-ttu-id="3c5b0-2488">Um bug no `az webapp config backup update` que impede a configuração de um agendamento de backup foi corrigido, caso ele ainda não tenha sido definido</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2488">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="3c5b0-2489">Configurar</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2489">Configure</span></span>
* <span data-ttu-id="3c5b0-2490">O YAML foi adicionado às opções de formato de saída</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2490">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="3c5b0-2491">Contêiner</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2491">Container</span></span>
* <span data-ttu-id="3c5b0-2492">Alterado para mostrar a identidade ao exportar um grupo de contêineres para yaml</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2492">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="3c5b0-2493">EventHub</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2493">EventHub</span></span>
* <span data-ttu-id="3c5b0-2494">O sinalizador `--enable-kafka` foi adicionado para dar suporte ao Kafka no `eventhub namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2494">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="3c5b0-2495">Interativo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2495">Interactive</span></span>
* <span data-ttu-id="3c5b0-2496">O interativo agora instala a extensão `interactive` que permite atualizações e suporte mais rápidos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2496">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="3c5b0-2497">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2497">Monitor</span></span>
* <span data-ttu-id="3c5b0-2498">Foi adicionado suporte para nomes de métricas, que incluem os caracteres barra (/) e ponto (.) para `--condition` em `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2498">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-2499">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2499">Network</span></span>
* <span data-ttu-id="3c5b0-2500">Os nomes de comandos `network interface-endpoint` foram preteridos em benefício de `network private-endpoint`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2500">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="3c5b0-2501">Foi corrigido um problema onde um argumento `--peer-circuit` em `express-route peering connection create` não aceitaria uma ID</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2501">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="3c5b0-2502">Foi corrigido um problema onde `--ip-tags` não funcionava corretamente com `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2502">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="3c5b0-2503">Perfil</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2503">Profile</span></span>
* <span data-ttu-id="3c5b0-2504">`--use-cert-sn-issuer` foi adicionado a `az login` para logon da entidade de serviço com rolagens automáticas de certificado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2504">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="3c5b0-2505">RDBMS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2505">RDBMS</span></span>
* <span data-ttu-id="3c5b0-2506">Adicionados comandos da réplica mysql</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2506">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="3c5b0-2507">Recurso</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2507">Resource</span></span>
* <span data-ttu-id="3c5b0-2508">Adicionado suporte para grupos de gerenciamento e assinaturas aos comandos `policy definition|set-definition`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2508">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="3c5b0-2509">Função</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2509">Role</span></span>
* <span data-ttu-id="3c5b0-2510">Adicionado suporte para gerenciamento de permissões de API, usuário conectado e gerenciamento de senhas dos aplicativos e certificados de credenciais</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2510">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="3c5b0-2511">`ad sp create-for-rbac` foi alterado para esclarecer a confusão entre o displayName e o nome da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2511">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="3c5b0-2512">Suporte adicionado para conceder permissões a aplicativos do AAD</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2512">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-2513">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2513">Storage</span></span>
* <span data-ttu-id="3c5b0-2514">Suporte adicionado para se conectar aos serviços de armazenamento somente com SAS e pontos de extremidade (sem um nome de conta ou uma chave), conforme descrito em `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2514">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="3c5b0-2515">VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2515">VM</span></span>
* <span data-ttu-id="3c5b0-2516">O argumento `storage-sku` foi adicionado a `image create` para definir o tipo de conta de armazenamento padrão da imagem</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2516">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="3c5b0-2517">O bug com `vm resize` onde a opção `--no-wait` faz com que o comando falhasse foi corrigido</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2517">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="3c5b0-2518">O formato de saída da tabela `vm encryption show` para mostrar o status foi alterado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2518">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="3c5b0-2519">`vm secret format` foi alterado para exigir a saída json/jsonc.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2519">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="3c5b0-2520">Avisa o usuário e assume como padrão a saída json se um formato de saída indesejado for escolhido</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2520">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="3c5b0-2521">Validação de argumento aprimorado para `vm create --image`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2521">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="3c5b0-2522">23 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2522">October 23, 2018</span></span>

<span data-ttu-id="3c5b0-2523">Versão 2.0.49</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2523">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="3c5b0-2524">Núcleo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2524">Core</span></span>
* <span data-ttu-id="3c5b0-2525">Corrigido o problema com `--ids` onde `--subscription` teria precedência sobre a assinatura em `--ids`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2525">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="3c5b0-2526">Adicionados avisos explícitos quando parâmetros seriam ignorados pelo uso de `--ids`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2526">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-2527">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2527">ACR</span></span>
* <span data-ttu-id="3c5b0-2528">Corrigido um problema de codificação de ACR Build no Python2</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2528">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="3c5b0-2529">CDN</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2529">CDN</span></span>
* <span data-ttu-id="3c5b0-2530">[ALTERAÇÃO SIGNIFICATIVA] Alterado o comportamento de armazenamento em cache da cadeia de caracteres de consulta padrão de `cdn endpoint create` para não assumir o padrão "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2530">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="3c5b0-2531">Agora, ele é definido pelo serviço</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2531">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="3c5b0-2532">Contêiner</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2532">Container</span></span>
* <span data-ttu-id="3c5b0-2533">Adicionado `Private` como um tipo válido para passar para '--ip-address'</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2533">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="3c5b0-2534">Alterado para permitir o uso somente de ID de sub-rede para configurar uma rede virtual para o grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2534">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="3c5b0-2535">Alterado para permitir o uso de nome de rede virtual ou ID de recurso para habilitar o uso de redes virtuais de diferentes grupos de recursos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2535">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="3c5b0-2536">Adicionado `--assign-identity` para adicionar uma identidade MSI a um grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2536">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="3c5b0-2537">Adicionado `--scope` para criar uma atribuição de função para a identidade MSI atribuída pelo sistema</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2537">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="3c5b0-2538">Adicionado um aviso ao criar um grupo de contêineres com uma imagem sem um processo de execução longa</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2538">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="3c5b0-2539">Corrigidos os problemas de saída da tabela para comandos `list` e `show`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2539">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="3c5b0-2540">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2540">CosmosDB</span></span>
* <span data-ttu-id="3c5b0-2541">Adicionado o suporte `--enable-multiple-write-locations` para `cosmosdb create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2541">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="3c5b0-2542">Interativo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2542">Interactive</span></span>
* <span data-ttu-id="3c5b0-2543">Alterado para garantir que o parâmetro de assinatura global seja exibido nos parâmetros</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2543">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="3c5b0-2544">Central da IoT</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2544">IoT Central</span></span>
* <span data-ttu-id="3c5b0-2545">Adicionadas opções de nome de exibição e modelo para criação de aplicativos de IoT Central</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2545">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="3c5b0-2546">[ALTERAÇÃO SIGNIFICATIVA] Removido o suporte para a SKU F1; Use a SKU S1</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2546">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="3c5b0-2547">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2547">Monitor</span></span>
* <span data-ttu-id="3c5b0-2548">Alterações para `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2548">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="3c5b0-2549">Adicionado suporte para listar todos os eventos no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2549">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="3c5b0-2550">Adicionado o parâmetro `--offset` para criar consultas de tempo mais facilmente</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2550">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="3c5b0-2551">Melhorada a validação para `--start-time` e `--end-time` para usar um intervalo mais amplo de formatos ISO8601 e formatos de data/hora mais amigáveis ao usuário</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2551">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="3c5b0-2552">Adicionado `--namespace` como alias para a opção preterida `--resource-provider`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2552">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="3c5b0-2553">Preterido `--filters` porque não há valores diferentes daqueles com opções fortemente tipadas compatíveis com o serviço</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2553">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="3c5b0-2554">Alterações para `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2554">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="3c5b0-2555">Adicionado o parâmetro `--offset` para criar consultas de tempo mais facilmente</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2555">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="3c5b0-2556">Melhorada a validação para `--start-time` e `--end-time` para usar um intervalo mais amplo de formatos ISO8601 e formatos de data/hora mais amigáveis ao usuário</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2556">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="3c5b0-2557">Melhorada a validação para os argumentos `--event-hub` e `--event-hub-rule` para `monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2557">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-2558">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2558">Network</span></span>
* <span data-ttu-id="3c5b0-2559">Adicionados os argumentos `--app-gateway-address-pools` e `--gateway-name` para `nic create`, para dar suporte à adição de pools de endereços de back-end do gateway de aplicativo a um NIC</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2559">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="3c5b0-2560">Adicionados os argumentos `--app-gateway-address-pools` e `--gateway-name` para `nic ip-config create/update`, para dar suporte à adição de pools de endereços de back-end do gateway de aplicativo a um NIC</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2560">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="3c5b0-2561">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2561">ServiceBus</span></span>
* <span data-ttu-id="3c5b0-2562">Adicionado `migration_state` somente leitura para MigrationConfigProperties para mostrar o atual estado de migração de namespace Standard para Premium do Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2562">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="3c5b0-2563">SQL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2563">SQL</span></span>
* <span data-ttu-id="3c5b0-2564">Corrigidos `sql failover-group create` e `sql failover-group update` para trabalhar com a política de failover Manual</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2564">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-2565">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2565">Storage</span></span>
* <span data-ttu-id="3c5b0-2566">Corrigida a formatação de saída `az storage cors list`, todos os itens mostram a chave correta de "Serviço"</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2566">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="3c5b0-2567">Adicionado o parâmetro `--bypass-immutability-policy` para a exclusão de contêiner bloqueado pela política de imutabilidade</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2567">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="3c5b0-2568">VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2568">VM</span></span>
* <span data-ttu-id="3c5b0-2569">Aplicado o modo `None` de armazenamento em cache de disco para as séries Lv/Lv2 de computadores no `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2569">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="3c5b0-2570">Atualizada a lista de tamanhos com suporte compatíveis com a aceleração de rede para `vm create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2570">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="3c5b0-2571">Adicionado argumentos fortemente tipados para configurações de iops e mbps de ultra ssd para `disk create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2571">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="3c5b0-2572">16 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2572">October 16, 2018</span></span>

<span data-ttu-id="3c5b0-2573">Versão 2.0.48</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2573">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="3c5b0-2574">VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2574">VM</span></span>
* <span data-ttu-id="3c5b0-2575">Corrigido o problema do SDK que causava falha durante a instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2575">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="3c5b0-2576">9 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2576">October 9, 2018</span></span>

<span data-ttu-id="3c5b0-2577">Versão 2.0.47</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2577">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="3c5b0-2578">Núcleo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2578">Core</span></span>
* <span data-ttu-id="3c5b0-2579">Melhoria do tratamento de erro para os erros de "Solicitação Incorreta"</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2579">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-2580">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2580">ACR</span></span>
* <span data-ttu-id="3c5b0-2581">Suporte adicionado para o formato de tabela semelhante como cliente do helm</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2581">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="3c5b0-2582">ACS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2582">ACS</span></span>
* <span data-ttu-id="3c5b0-2583">`aks [create|scale] --nodepool-name` adicionado para configurar o nome nodepool, truncado com 12 caracteres, padrão – nodepool1</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2583">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="3c5b0-2584">Corrigido para voltar para “scp” quando Parimiko falha</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2584">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="3c5b0-2585">`aks create` alterado para não precisar mais de `--aad-tenant-id`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2585">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="3c5b0-2586">Melhoria da mesclagem das credenciais do Kubernetes quando houver entradas duplicadas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2586">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="3c5b0-2587">Contêiner</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2587">Container</span></span>
* <span data-ttu-id="3c5b0-2588">`functionapp create` alterado para dar suporte à criação de um tipo de plano de consumo do Linux com um runtime específico</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2588">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="3c5b0-2589">[VERSÃO PRÉVIA] Suporte adicionado para hospedar aplicativos Web nos contêineres do Windows</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2589">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="3c5b0-2590">Hub de evento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2590">Event Hub</span></span>
* <span data-ttu-id="3c5b0-2591">Corrigido o comando `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2591">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="3c5b0-2592">[ALTERAÇÃO SIGNIFICATIVA]`list` comandos alterados para lidar com os erros de recurso(s) NotFound(404) do modo típico, em vez de mostrar uma lista vazia</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2592">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="3c5b0-2593">Extensões</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2593">Extensions</span></span>
* <span data-ttu-id="3c5b0-2594">Corrigido o problema ao tentar adicionar uma extensão já instalada</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2594">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="3c5b0-2595">HDInsight</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2595">HDInsight</span></span>
* <span data-ttu-id="3c5b0-2596">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2596">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="3c5b0-2597">IoT</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2597">IoT</span></span>
* <span data-ttu-id="3c5b0-2598">Comando de instalação da extensão adicionado à faixa inicial</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2598">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="3c5b0-2599">KeyVault</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2599">KeyVault</span></span>
* <span data-ttu-id="3c5b0-2600">Alterado para restringir os comandos de armazenamento do keyvault ao perfil da API mais recente</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2600">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-2601">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2601">Network</span></span>
* <span data-ttu-id="3c5b0-2602">Corrigido `network dns zone create`: O comando terá êxito mesmo se o usuário tiver configurado um local padrão.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2602">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="3c5b0-2603">Veja o n° 6052</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2603">See #6052</span></span>
* <span data-ttu-id="3c5b0-2604">Preterido `--remote-vnet-id` para `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2604">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="3c5b0-2605">`--remote-vnet` a `network vnet peering create` adicionados, que aceita um nome ou uma ID</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2605">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="3c5b0-2606">Suporte adicionado para vários prefixos de sub-rede a `network vnet create` com `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2606">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="3c5b0-2607">Suporte adicionado para vários prefixos de sub-rede a `network vnet subnet [create|update]` com `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2607">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="3c5b0-2608">Corrigido o problema com `network application-gateway create` que impedia a criação de gateways com a SKU `WAF_v2` ou `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2608">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="3c5b0-2609">Argumento de conveniência `--service-endpoint-policy` adicionado a `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2609">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="3c5b0-2610">Função</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2610">Role</span></span>
* <span data-ttu-id="3c5b0-2611">Suporte adicionado para listar os proprietários de aplicativo do Azure AD para `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2611">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="3c5b0-2612">Suporte adicionado para listar os proprietários da entidade de serviço do Azure AD para `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2612">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="3c5b0-2613">Alterado para garantir que os comandos para criar e atualizar a definição da função aceitem várias configurações de permissão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2613">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="3c5b0-2614">`ad sp create-for-rbac` alterado para garantir que a URI da home page sempre seja "https"</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2614">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="3c5b0-2615">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2615">Service Bus</span></span>
* <span data-ttu-id="3c5b0-2616">[ALTERAÇÃO SIGNIFICATIVA]`list` comandos alterados para lidar com os erros de recurso(s) NotFound(404) do modo típico, em vez de mostrar uma lista vazia</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2616">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="3c5b0-2617">VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2617">VM</span></span>
* <span data-ttu-id="3c5b0-2618">Corrigido o campo `accessSas` vazio em `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2618">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="3c5b0-2619">`vmss create` alterado para reservar um intervalo de portas de front-end grande o suficiente para lidar com excesso de provisionamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2619">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="3c5b0-2620">Corrigidos os comandos de atualização para `sig`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2620">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="3c5b0-2621">Suporte `--no-wait` adicionado para gerenciar as versões da imagem em `sig`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2621">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="3c5b0-2622">`vm list-ip-addresses` alterado para mostrar a zona de disponibilidade dos endereços IP públicos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2622">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="3c5b0-2623">`[vm|vmss] disk attach` alterado para definir o LUN padrão do disco para o primeiro ponto disponível</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2623">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="3c5b0-2624">21 de setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2624">September 21, 2018</span></span>

<span data-ttu-id="3c5b0-2625">Versão 2.0.46</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2625">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-2626">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2626">ACR</span></span>
* <span data-ttu-id="3c5b0-2627">Adicionados comandos de tarefa de ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2627">Added ACR Task commands</span></span>
* <span data-ttu-id="3c5b0-2628">Adicionado o comando de execução rápido</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2628">Added quick run command</span></span>
* <span data-ttu-id="3c5b0-2629">Grupo de comandos `build-task` preteridos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2629">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="3c5b0-2630">Adicionado o grupo de comando `helm` para dar suporte ao gerenciamento de gráficos Helm com o ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2630">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="3c5b0-2631">Suporte adicionado para criação idempotente para registro gerenciado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2631">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="3c5b0-2632">Adicionado um sinalizador de formato no para exibir logs de build</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2632">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="3c5b0-2633">ACS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2633">ACS</span></span>
* <span data-ttu-id="3c5b0-2634">Alterado o comando `install-connector` para definir o FQDN mestre do AKS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2634">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="3c5b0-2635">Corrigida a criação de atribuição de função para vnet-subnet-id ao não especificar a entidade de serviço e skip-role-assignment</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2635">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-2636">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2636">AppService</span></span>

* <span data-ttu-id="3c5b0-2637">Adicionado suporte para o gerenciamento de operações de WebJobs (contínuos e disparados)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2637">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="3c5b0-2638">Suporte de az webapp config set para a propriedade --fts-state property. Adicionado suporte também para az functionapp config set & show</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2638">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="3c5b0-2639">Adicionado suporte para trazer seu próprio armazenamento para aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2639">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="3c5b0-2640">Adicionado suporte para a listar e restaurar aplicativos Web excluídos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2640">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="3c5b0-2641">Lote</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2641">Batch</span></span>
* <span data-ttu-id="3c5b0-2642">Alterada a inclusão de tarefas por meio de `--json-file` para dar suporte à sintaxe AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2642">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="3c5b0-2643">Atualizada a documentação de formatos `--json-file` aceitos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2643">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="3c5b0-2644">`--max-tasks-per-node-option` foi adicionado a `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2644">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="3c5b0-2645">Alterado o comportamento de `batch account` para mostrar as contas atualmente conectadas se nenhuma opção foi especificada</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2645">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="3c5b0-2646">Lote AI</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2646">Batch AI</span></span> 
* <span data-ttu-id="3c5b0-2647">Corrigida a falha na criação de conta de armazenamento automática no comando `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2647">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="3c5b0-2648">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2648">Cognitive Services</span></span>
* <span data-ttu-id="3c5b0-2649">Adicionado o complemento para os argumentos `--sku`, `--kind`, `--location`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2649">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="3c5b0-2650">Adicionado o comando `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2650">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="3c5b0-2651">Adicionado o comando `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2651">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="3c5b0-2652">Adicionado o comando `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2652">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="3c5b0-2653">Preterido `cognitiveservices list`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2653">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="3c5b0-2654">Alterado `--name` para que seja opcional para `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2654">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="3c5b0-2655">Contêiner</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2655">Container</span></span>
* <span data-ttu-id="3c5b0-2656">Adicionada a capacidade de reiniciar e parar um grupo de contêineres em execução</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2656">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="3c5b0-2657">Adicionado `--network-profile` para passar em um perfil de rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2657">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="3c5b0-2658">Adicionado `--subnet`, `--vnet_name`, para permitir a criação de grupos de contêineres em uma rede virtual</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2658">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="3c5b0-2659">Alterada a saída da tabela para mostrar o status do grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2659">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="3c5b0-2660">DataLake</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2660">Datalake</span></span>
* <span data-ttu-id="3c5b0-2661">Comandos adicionados para regras da rede virtual</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2661">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="3c5b0-2662">Shell interativo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2662">Interactive Shell</span></span>
* <span data-ttu-id="3c5b0-2663">Corrigido o erro no Windows em que comandos não são executados corretamente</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2663">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="3c5b0-2664">Corrigido o problema para carregar o comando no modo interativo que era causado por objetos preteridos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2664">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="3c5b0-2665">IoT</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2665">IoT</span></span>
* <span data-ttu-id="3c5b0-2666">Adicionado suporte para roteamento de Hubs de IoT</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2666">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="3c5b0-2667">Key Vault</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2667">Key Vault</span></span>
* <span data-ttu-id="3c5b0-2668">Corrigida a importação de chave do Key Vault para chaves RSA</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2668">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-2669">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2669">Network</span></span>
* <span data-ttu-id="3c5b0-2670">Adicionados os comandos `network public-ip prefix` para dar suporte a recursos de prefixos de IP público</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2670">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="3c5b0-2671">Adicionados os comandos `network service-endpoint` para dar suporte a recursos de política de ponto de extremidade de serviço</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2671">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="3c5b0-2672">Adicionados os comandos `network lb outbound-rule` para dar suporte à criação de regras de saída do Standard Load Balancer</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2672">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="3c5b0-2673">Adicionado `--public-ip-prefix` a `network lb frontend-ip create/update` para dar suporte a configurações de IP de front-end usando prefixos de IP público</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2673">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="3c5b0-2674">Adicionado `--enable-tcp-reset` a `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2674">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="3c5b0-2675">Adicionado `--disable-outbound-snat` a `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2675">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="3c5b0-2676">Permitido o uso de `network watcher flow-log show/configure` com NSGs clássicos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2676">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="3c5b0-2677">Adição do comando `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2677">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="3c5b0-2678">Corrigido o comando `network watcher test-connectivity` e adicionadas as propriedades `--method`, `--valid-status-codes` e `--headers`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2678">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="3c5b0-2679">`network express-route create/update`: Adicionado o sinalizador `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2679">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="3c5b0-2680">`network vnet subnet create/update`: Adicionado suporte para `--delegation`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2680">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="3c5b0-2681">Adicionado o comando `network vnet subnet list-available-delegations`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2681">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="3c5b0-2682">`network traffic-manager profile create/update`: Adicionado suporte para `--interval`, `--timeout` e `--max-failures` para as opções preteridas de configuração do monitor `--monitor-path`, `--monitor-port` e `--monitor-protocol`, que foram substituídas por `--path`, `--port` e `--protocol`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2682">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="3c5b0-2683">`network lb frontend-ip create/update`: Corrigida a lógica para configurar o método de alocação de IP privado. Se um endereço IP privado for fornecido, a alocação será estática. Se nenhum endereço IP privado for fornecido ou uma cadeia de caracteres vazia for fornecida para o endereço IP privado, a alocação será dinâmica.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2683">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="3c5b0-2684">`dns record-set * create/update`: Adicionado suporte para `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2684">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="3c5b0-2685">Adicionados comandos `network interface-endpoint` para consultar objetos do ponto de extremidade da interface</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2685">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="3c5b0-2686">Adicionado `network profile show/list/delete` para gerenciamento parcial dos perfis de rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2686">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="3c5b0-2687">Adicionados comandos `network express-route peering connection` para gerenciar conexões de emparelhamento entre as ExpressRoutes</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2687">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="3c5b0-2688">RDBMS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2688">RDBMS</span></span>
* <span data-ttu-id="3c5b0-2689">Adicionado suporte para o serviço MariaDB</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2689">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="3c5b0-2690">Reserva</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2690">Reservation</span></span>
* <span data-ttu-id="3c5b0-2691">Adicionado CosmosDB no tipo enumerado de recurso reservado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2691">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="3c5b0-2692">Adicionada a propriedade nome no modelo do Patch</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2692">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="3c5b0-2693">Gerenciar aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2693">Manage App</span></span>
* <span data-ttu-id="3c5b0-2694">Corrigido o bug em `managedapp create --kind MarketPlace` que resultava em falha durante a criação da instância de um aplicativo gerenciado do Marketplace</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2694">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="3c5b0-2695">Alterados os comandos `feature` para serem restritos somente aos perfis com suporte</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2695">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="3c5b0-2696">Função</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2696">Role</span></span>
* <span data-ttu-id="3c5b0-2697">Adicionado suporte para listar membros de grupo de usuários</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2697">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="3c5b0-2698">SignalR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2698">SignalR</span></span>
* <span data-ttu-id="3c5b0-2699">Primeira versão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2699">First release</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-2700">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2700">Storage</span></span>
* <span data-ttu-id="3c5b0-2701">Adicionado o parâmetro `--auth-mode login` para usar as credenciais de login do usuário para autorização de filas e blobs</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2701">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="3c5b0-2702">Adicionado `storage container immutability-policy/legal-hold` para gerenciar o armazenamento imutável</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2702">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="3c5b0-2703">VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2703">VM</span></span>
* <span data-ttu-id="3c5b0-2704">Corrigido o problema em que `vm create --generate-ssh-keys` sobrescreve o arquivo de chave privada se o arquivo de chave pública estiver ausente (#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2704">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="3c5b0-2705">Adicionado suporte para galeria de imagem compartilhada através de `az sig`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2705">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="3c5b0-2706">28 de Agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2706">August 28, 2018</span></span>

<span data-ttu-id="3c5b0-2707">Versão 2.0.45</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2707">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="3c5b0-2708">Núcleo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2708">Core</span></span>

* <span data-ttu-id="3c5b0-2709">Corrigido o problema de carregamento de arquivo de configuração vazio</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2709">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="3c5b0-2710">Adicionado suporte para o perfil `2018-03-01-hybrid` para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2710">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-2711">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2711">ACR</span></span>

* <span data-ttu-id="3c5b0-2712">Adicionada uma solução alternativa para operações de runtime sem solicitações ARM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2712">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="3c5b0-2713">Alterado para excluir arquivos de controle de versão (por exemplo, .git, .gitignore) de tar carregados por padrão no comando `build`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2713">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="3c5b0-2714">ACS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2714">ACS</span></span>

* <span data-ttu-id="3c5b0-2715">Alterado `aks create` para os padrões para VMs `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2715">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="3c5b0-2716">Alterado `aks get-credentials` para agora chamar novas APIs para obter credenciais de cluster</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2716">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-2717">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2717">AppService</span></span>

* <span data-ttu-id="3c5b0-2718">Adicionado suporte para CORS no functionapp e webapp</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2718">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="3c5b0-2719">Adicionado suporte a marcas ARM ao criar comandos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2719">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="3c5b0-2720">Alterado `[webapp|functionapp] identity show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2720">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="3c5b0-2721">Backup</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2721">Backup</span></span>

* <span data-ttu-id="3c5b0-2722">Alterado `backup vault backup-properties show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2722">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="3c5b0-2723">Serviço de Bot</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2723">Bot Service</span></span>

* <span data-ttu-id="3c5b0-2724">Versão da CLI do serviço de Bot inicial</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2724">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="3c5b0-2725">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2725">Cognitive Services</span></span>

* <span data-ttu-id="3c5b0-2726">Adicionado novo parâmetro `--api-properties,` que é necessário para a criação de alguns dos serviços</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2726">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="3c5b0-2727">IoT</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2727">IoT</span></span>

* <span data-ttu-id="3c5b0-2728">Corrigido o problema com a associação de hubs vinculados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2728">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="3c5b0-2729">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2729">Monitor</span></span>

* <span data-ttu-id="3c5b0-2730">Adicionados comandos `monitor metrics alert` para alertas de métrica quase em tempo real</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2730">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="3c5b0-2731">Comandos `monitor alert` preteridos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2731">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-2732">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2732">Network</span></span>

* <span data-ttu-id="3c5b0-2733">Alterado `network application-gateway ssl-policy predefined show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2733">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="3c5b0-2734">Recurso</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2734">Resource</span></span>

* <span data-ttu-id="3c5b0-2735">Alterado `provider operation show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2735">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-2736">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2736">Storage</span></span>

* <span data-ttu-id="3c5b0-2737">Alterado `storage share policy show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2737">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="3c5b0-2738">VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2738">VM</span></span>

* <span data-ttu-id="3c5b0-2739">Alterado `vm/vmss identity show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2739">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="3c5b0-2740">Preterido `--storage-caching` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2740">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="3c5b0-2741">14 de agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2741">Auguest 14, 2018</span></span>

<span data-ttu-id="3c5b0-2742">Versão 2.0.44</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2742">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="3c5b0-2743">Núcleo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2743">Core</span></span>

* <span data-ttu-id="3c5b0-2744">Corrigida a exibição numérica na saída `table`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2744">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="3c5b0-2745">Adicionado o formato de saída YAML</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2745">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="3c5b0-2746">Telemetria</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2746">Telemetry</span></span>

* <span data-ttu-id="3c5b0-2747">Melhorias nos relatórios de telemetria</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2747">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-2748">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2748">ACR</span></span>

* <span data-ttu-id="3c5b0-2749">Adicionados os comandos `content-trust policy`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2749">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="3c5b0-2750">Corrigido o problema onde `.dockerignore` não foi tratado adequadamente</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2750">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="3c5b0-2751">ACS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2751">ACS</span></span>

* <span data-ttu-id="3c5b0-2752">Alterado `az acs/aks install-cli` para instalar em `%USERPROFILE%\.azure-kubectl` no Windows</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2752">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="3c5b0-2753">Alterado `az aks install-connector` para detectar se o cluster tem RBAC e configurar o conector ACI adequadamente</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2753">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="3c5b0-2754">Alterado para atribuição de função à sub-rede quando ela é fornecida</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2754">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="3c5b0-2755">Adicionada uma nova opção para “ignorar a atribuição de função” à sub-rede quando ela é fornecida</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2755">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="3c5b0-2756">Alterado para ignorar a atribuição de função à sub-rede quando a atribuição já existe</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2756">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="3c5b0-2757">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2757">AppService</span></span>

* <span data-ttu-id="3c5b0-2758">Corrigido um bug que impede a criação de um aplicativo de funções usando contas de armazenamento em grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2758">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="3c5b0-2759">Corrigida uma falha na implantação de zip</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2759">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="3c5b0-2760">BatchAI</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2760">BatchAI</span></span>

* <span data-ttu-id="3c5b0-2761">Alterada a saída do agente para criação de conta de armazenamento automática para especificar “ *grupo* de recurso”.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2761">Changed logger output for auto-storage account creation to specifies "resource *group* ".</span></span>        

### <a name="container"></a><span data-ttu-id="3c5b0-2762">Contêiner</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2762">Container</span></span>

* <span data-ttu-id="3c5b0-2763">Adicionado `--secure-environment-variables` para passar as variáveis de ambiente seguras para um contêiner</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2763">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="3c5b0-2764">IoT</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2764">IoT</span></span>

* <span data-ttu-id="3c5b0-2765">[ALTERAÇÃO SIGNIFICATIVA] Removidos os comandos preteridos que foram movidos para a extensão iot</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2765">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="3c5b0-2766">Atualizados os elementos para não presumirem o domínio `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2766">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="3c5b0-2767">Central de IoT</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2767">Iot Central</span></span>

* <span data-ttu-id="3c5b0-2768">Versão inicial do módulo do IoT Central</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2768">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="3c5b0-2769">KeyVault</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2769">KeyVault</span></span>


* <span data-ttu-id="3c5b0-2770">Comandos adicionados para gerenciar contas de armazenamento e as definições de sas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2770">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="3c5b0-2771">Comandos adicionados para regras de rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2771">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="3c5b0-2772">Adicionado o parâmetro `--id` para operações de certificado, chave e segredo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2772">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="3c5b0-2773">Adicionado suporte para a versão de várias APIs de gerenciamento KV</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2773">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="3c5b0-2774">Adicionado suporte para a versão de várias APIs do plano de dados KV</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2774">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="3c5b0-2775">Retransmissão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2775">Relay</span></span>

* <span data-ttu-id="3c5b0-2776">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2776">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="3c5b0-2777">Sql</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2777">Sql</span></span>

* <span data-ttu-id="3c5b0-2778">Adicionados os comandos `sql failover-group`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2778">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-2779">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2779">Storage</span></span>

* <span data-ttu-id="3c5b0-2780">[ALTERAÇÃO SIGNIFICATIVA] Alterado `storage account show-usage` para exigir o parâmetro `--location` e listará por região</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2780">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="3c5b0-2781">Alterado o parâmetro `--resource-group` para ser opcional para comandos `storage account`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2781">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="3c5b0-2782">Removidos os avisos de “Falha na pré-condição” para as falhas individuais em comandos em lote para uma única mensagem agregada</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2782">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="3c5b0-2783">Alterados os comandos `[blob|file] delete-batch` para não exibir mais matriz de nulos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2783">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="3c5b0-2784">Alterados os comandos `blob [download|upload|delete-batch]` para ler o token de sas da url do contêiner</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2784">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="3c5b0-2785">VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2785">VM</span></span>

* <span data-ttu-id="3c5b0-2786">Adicionado filtros comuns à `vm list-skus` para facilidade de uso</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2786">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="3c5b0-2787">31 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2787">July 31, 2018</span></span>

<span data-ttu-id="3c5b0-2788">Versão 2.0.43</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2788">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-2789">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2789">ACR</span></span>

* <span data-ttu-id="3c5b0-2790">Sinalizador `--with-secure-properties` adicionado ao comando `acr build-task show`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2790">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="3c5b0-2791">Adicionado o comando `acr build-task update-build`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2791">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="3c5b0-2792">ACS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2792">ACS</span></span>

* <span data-ttu-id="3c5b0-2793">Alterado para retornar 0 (êxito) ao terminar `az aks browse` pressionando [Ctrl+C]</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2793">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="3c5b0-2794">Lote</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2794">Batch</span></span>

* <span data-ttu-id="3c5b0-2795">Bug corrigido ao mostrar o token AAD no cloudshell</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2795">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="3c5b0-2796">Contêiner</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2796">Container</span></span>

* <span data-ttu-id="3c5b0-2797">Requisito removido de `--log-analytics-workspace-key` para o nome ou a ID ao definir assinatura</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2797">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-2798">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2798">Network</span></span>

* <span data-ttu-id="3c5b0-2799">Suporte a DNS adicionado a 2017-03-09-profile para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2799">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="3c5b0-2800">Recurso</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2800">Resource</span></span>

* <span data-ttu-id="3c5b0-2801">`--rollback-on-error` a `group deployment create` adicionado para executar uma implantação válida no erro</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2801">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="3c5b0-2802">Problema corrigido onde `--parameters {}` com `group deployment create` resultou em um erro</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2802">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="3c5b0-2803">Função</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2803">Role</span></span>

* <span data-ttu-id="3c5b0-2804">Suporte adicionado para o perfil da pilha 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2804">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="3c5b0-2805">Problema corrigido onde os parâmetros de atualização genéricos para `app update` não funcionariam corretamente</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2805">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="3c5b0-2806">Search</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2806">Search</span></span>

* <span data-ttu-id="3c5b0-2807">Comandos adicionados para o serviço Azure Search</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2807">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="3c5b0-2808">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2808">Service Bus</span></span>

* <span data-ttu-id="3c5b0-2809">Grupo de comandos de migração adicionados para migrar um namespace do Barramento de Serviço Standard para Premium</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2809">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="3c5b0-2810">Novas propriedades opcionais adicionadas à fila do Barramento de Serviço e à Assinatura</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2810">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="3c5b0-2811">`--enable-batched-operations` e `--enable-dead-lettering-on-message-expiration` em `queue`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2811">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="3c5b0-2812">`--dead-letter-on-filter-exceptions` em `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2812">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-2813">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2813">Storage</span></span>

* <span data-ttu-id="3c5b0-2814">Suporte adicionado para o download de arquivos grandes usando uma única conexão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2814">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="3c5b0-2815">Comandos `show` convertidos que foram perdidos na falha com código de saída 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2815">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="3c5b0-2816">VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2816">VM</span></span>

* <span data-ttu-id="3c5b0-2817">Suporte adicionado para listar conjuntos de disponibilidade por assinatura</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2817">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="3c5b0-2818">Adicionado o suporte para `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2818">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="3c5b0-2819">Suporte adicionado para o grupo de segurança do aplicativo ao criar um conjunto de dimensionamento da VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2819">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="3c5b0-2820">[ALTERAÇÃO SIGNIFICATIVA]`[vm|vmss] create`, `[vm|vmss] identity assign` e `[vm|vmss] identity remove` alterados para produzir identidades de usuário atribuídas no formato de dicionário</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2820">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="3c5b0-2821">18 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2821">July 18, 2018</span></span>

<span data-ttu-id="3c5b0-2822">Versão 2.0.42</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2822">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="3c5b0-2823">Núcleo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2823">Core</span></span>

* <span data-ttu-id="3c5b0-2824">Adicionado suporte para logon baseado em navegador, na janela de bash WSL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2824">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="3c5b0-2825">O sinalizador `--force-string` foi adicionado a todos os comandos de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2825">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="3c5b0-2826">[ALTERAÇÃO SIGNIFICATIVA] Os comandos 'show' foram alterados para registrar mensagens de erro e falha com código de saída 3 quando um recurso está ausente</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2826">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-2827">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2827">ACR</span></span>

* <span data-ttu-id="3c5b0-2828">[ALTERAÇÃO SIGNIFICATIVA] '--no-push' foi atualizado para um sinalizador puro no comando 'acr build'</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2828">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="3c5b0-2829">Foram adicionados os comandos `show` e `update` no grupo `acr repository`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2829">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="3c5b0-2830">Foi adicionado o sinalizador `--detail` a `show-manifests` e `show-tags` para mostrar informações mais detalhadas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2830">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="3c5b0-2831">Foi adicionado o parâmetro `--image` para dar suporte aos detalhes do build get ou aos logs por meio de uma imagem</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2831">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="3c5b0-2832">ACS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2832">ACS</span></span>

* <span data-ttu-id="3c5b0-2833">`az aks create` foi alterado para excluir o erro se `--max-pods` for menor que 5</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2833">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-2834">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2834">AppService</span></span>

* <span data-ttu-id="3c5b0-2835">Suporte adicionado para skus PremiumV2</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2835">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="3c5b0-2836">Lote</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2836">Batch</span></span>

* <span data-ttu-id="3c5b0-2837">Corrigido o bug sobre como usar a credencial de token no modo do Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2837">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="3c5b0-2838">Alterada a entrada JSON para diferenciar maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2838">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="3c5b0-2839">Lote AI</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2839">Batch AI</span></span>

* <span data-ttu-id="3c5b0-2840">Corrigido o comando `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2840">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="3c5b0-2841">Contêiner</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2841">Container</span></span>

* <span data-ttu-id="3c5b0-2842">Removido o requisito de nome de usuário e senha para os registros não dockerhub</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2842">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="3c5b0-2843">Correção de erro durante a criação de grupos de contêineres de arquivo yaml</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2843">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-2844">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2844">Network</span></span>

* <span data-ttu-id="3c5b0-2845">Adicionado o suporte `--no-wait` para `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2845">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="3c5b0-2846">Adicionado `network nic wait`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2846">Added `network nic wait`</span></span>
* <span data-ttu-id="3c5b0-2847">Preterido o argumento `--ids` para `network vnet [subnet|peering] list`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2847">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="3c5b0-2848">Adicionado o sinalizador `--include-default` para incluir regras de segurança padrão na saída do `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2848">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="3c5b0-2849">Recurso</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2849">Resource</span></span>

* <span data-ttu-id="3c5b0-2850">Adicionado o suporte `--no-wait` para `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2850">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="3c5b0-2851">Adicionado o suporte `--no-wait` para `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2851">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="3c5b0-2852">Adicionado o comando `deployment wait`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2852">Added `deployment wait` command</span></span>
* <span data-ttu-id="3c5b0-2853">Correção do problema em que os comandos de nível de assinatura `az deployment` erroneamente apareceram no perfil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2853">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="3c5b0-2854">SQL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2854">SQL</span></span>

* <span data-ttu-id="3c5b0-2855">O erro “O nome de grupo de recursos fornecido ... não correspondeu ao nome na Url” foi fixado ao especificar o nome do pool elástico para os comandos `sql db copy` e `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2855">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="3c5b0-2856">Permitir a configuração do padrão do SQL Server, executando `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2856">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="3c5b0-2857">Os formatadores de tabela foram implementados aos comandos `sql server`, `sql server firewall-rule`, `sql list-usages` e `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2857">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-2858">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2858">Storage</span></span>

* <span data-ttu-id="3c5b0-2859">Adicionada a propriedade `pageRanges` à saída `storage blob show` que será preenchida para blobs de página</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2859">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="3c5b0-2860">VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2860">VM</span></span>

* <span data-ttu-id="3c5b0-2861">[ALTERAÇÃO SIGNIFICATIVA] Alterado `vmss create` para usar o `Standard_DS1_v2` como o tamanho de instância padrão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2861">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="3c5b0-2862">Adicionado o suporte `--no-wait` para `vm extension [set|delete]` e `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2862">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="3c5b0-2863">Adicionado `vm extension wait`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2863">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="3c5b0-2864">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2864">July 3, 2018</span></span>

<span data-ttu-id="3c5b0-2865">Versão 2.0.41</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2865">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="3c5b0-2866">AKS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2866">AKS</span></span>

* <span data-ttu-id="3c5b0-2867">Monitoramento alterado para usar a ID de assinatura</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2867">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="3c5b0-2868">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2868">July 3, 2018</span></span>

<span data-ttu-id="3c5b0-2869">Versão 2.0.40</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2869">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="3c5b0-2870">Núcleo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2870">Core</span></span>

* <span data-ttu-id="3c5b0-2871">Adicionado um novo fluxo de código de autorização para o logon interativo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2871">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-2872">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2872">ACR</span></span>

* <span data-ttu-id="3c5b0-2873">Status da compilação de sondagem adicionado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2873">Added polling build status</span></span>
* <span data-ttu-id="3c5b0-2874">Suporte adicionado para valores de enumeração que não diferenciam maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2874">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="3c5b0-2875">Parâmetros `--top` e `--orderby` adicionados para `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2875">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="3c5b0-2876">ACS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2876">ACS</span></span>

* <span data-ttu-id="3c5b0-2877">[ALTERAÇÃO SIGNIFICATIVA] Habilitar controle de acesso baseado em funções do Kubernetes por padrão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2877">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="3c5b0-2878">Argumento `--disable-rbac` e preterido `--enable-rbac` adicionados, pois é o padrão agora</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2878">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="3c5b0-2879">Opções atualizadas do comando `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2879">Updated options for `aks browse` command.</span></span> <span data-ttu-id="3c5b0-2880">Suporte `--listen-port` adicionado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2880">Added `--listen-port` support</span></span>
* <span data-ttu-id="3c5b0-2881">Atualizado o pacote de gráficos do helm padrão para o comando `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2881">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="3c5b0-2882">Usar virtual-kubelet-para-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2882">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="3c5b0-2883">Comandos `aks enable-addons` e `aks disable-addons` adicionados para atualizar um cluster existente</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2883">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-2884">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2884">AppService</span></span>

* <span data-ttu-id="3c5b0-2885">Suporte adicionado para desabilitar a identidade via `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2885">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="3c5b0-2886">Marca `preview` removida para o recurso de Identidade</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2886">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="3c5b0-2887">Backup</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2887">Backup</span></span>

* <span data-ttu-id="3c5b0-2888">Definição do módulo atualizada</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2888">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="3c5b0-2889">BatchAI</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2889">BatchAI</span></span>

* <span data-ttu-id="3c5b0-2890">Saída da tabela corrigida para comandos `batchai cluster node list` e `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2890">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="3c5b0-2891">Nuvem</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2891">Cloud</span></span>

* <span data-ttu-id="3c5b0-2892">Sufixo do servidor `acr login` adicionado à configuração de nuvem</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2892">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="3c5b0-2893">Contêiner</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2893">Container</span></span>

* <span data-ttu-id="3c5b0-2894">`container create` alterado para padrão para a operação de longa execução</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2894">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="3c5b0-2895">Parâmetros `--log-analytics-workspace` e `--log-analytics-workspace-key` adicionados do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2895">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="3c5b0-2896">Parâmetro `--protocol` adicionado para especificar qual protocolo de rede usar</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2896">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="3c5b0-2897">Extensão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2897">Extension</span></span>

* <span data-ttu-id="3c5b0-2898">`extension list-available` alterado para mostrar apenas as extensões compatíveis com a versão da CLI</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2898">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-2899">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2899">Network</span></span>

* <span data-ttu-id="3c5b0-2900">Corrigido o problema onde os tipos de registro diferenciam maiúsculas de minúsculas ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2900">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="3c5b0-2901">Rdbms</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2901">Rdbms</span></span>

* <span data-ttu-id="3c5b0-2902">Adicionados os comandos `[postgres|myql] server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2902">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="3c5b0-2903">Recurso</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2903">Resource</span></span>

* <span data-ttu-id="3c5b0-2904">Novo grupo de operação `deployment` adicionado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2904">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="3c5b0-2905">VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2905">VM</span></span>

* <span data-ttu-id="3c5b0-2906">Suporte adicionado para remover a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2906">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="3c5b0-2907">25 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2907">June 25, 2018</span></span>

<span data-ttu-id="3c5b0-2908">Versão 2.0.39</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2908">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="3c5b0-2909">CLI</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2909">CLI</span></span>

* <span data-ttu-id="3c5b0-2910">Corte de arquivo atualizado no instalador MSI para corrigir o problema de instalação da extensão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2910">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="3c5b0-2911">19 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2911">June 19, 2018</span></span>

<span data-ttu-id="3c5b0-2912">Versão 2.0.38</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2912">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="3c5b0-2913">Núcleo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2913">Core</span></span>

* <span data-ttu-id="3c5b0-2914">Suporte global adicionado para `--subscription` a maioria dos comandos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2914">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-2915">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2915">ACR</span></span>

* <span data-ttu-id="3c5b0-2916">`azure-storage-blob` foi adicionado como dependência</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2916">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="3c5b0-2917">A configuração de CPU padrão foi alterada com `acr build-task create` para usar 2 núcleos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2917">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="3c5b0-2918">ACS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2918">ACS</span></span>

* <span data-ttu-id="3c5b0-2919">As opções do comando `aks use-dev-spaces` foram atualizadas.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2919">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="3c5b0-2920">Suporte `--update` adicionado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2920">Added `--update` support</span></span>
* <span data-ttu-id="3c5b0-2921">`aks get-credentials --admin` foi alterado para substituir o contexto do usuário em `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2921">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="3c5b0-2922">A propriedade `nodeResourceGroup` somente leitura foi exposta em clusters gerenciados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2922">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="3c5b0-2923">O erro de comando `acs browse` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2923">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="3c5b0-2924">Foram feitas `--connector-name` opcional para `aks install-connector`, `aks upgrade-connector` e `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2924">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="3c5b0-2925">Novas regiões de Instância de Contêiner do Azure foram adicionadas para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2925">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="3c5b0-2926">O local normalizado foi adicionado no nome de versão do comando e no nome do nó para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2926">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-2927">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2927">AppService</span></span>

* <span data-ttu-id="3c5b0-2928">Foi adicionado suporte para versões mais recentes do urllib</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2928">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="3c5b0-2929">Foi adicionado suporte para `functionapp create` para usar o plano de serviço de aplicativo de grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2929">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="3c5b0-2930">Lote</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2930">Batch</span></span>

* <span data-ttu-id="3c5b0-2931">A dependência `azure-batch-extensions` foi removida</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2931">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="3c5b0-2932">Lote AI</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2932">Batch AI</span></span>

* <span data-ttu-id="3c5b0-2933">Foi adicionado suporte aos workspaces.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2933">Added support for workspaces.</span></span> <span data-ttu-id="3c5b0-2934">Os workspaces permitem agrupar clusters, servidores de arquivos e experimentos, removendo a limitação no número de recursos que podem ser criados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2934">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="3c5b0-2935">Foi adicionado suporte para os experimentos.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2935">Added support for experiments.</span></span> <span data-ttu-id="3c5b0-2936">Os experimentos permitem agrupar trabalhos em coleções removendo a limitação no número de trabalhos criados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2936">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="3c5b0-2937">Foi adicionado suporte para configurar `/dev/shm` para trabalhos em execução em um contêiner de docker</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2937">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="3c5b0-2938">Foram adicionados os comandos `batchai cluster node exec` e `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2938">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="3c5b0-2939">Esses comandos permitem executar qualquer comando diretamente nos nós e fornece a funcionalidade de encaminhamento de porta.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2939">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="3c5b0-2940">Foi adicionado suporte a `--ids` para os comandos `batchai`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2940">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="3c5b0-2941">[ALTERAÇÃO SIGNIFICATIVA] Todos os clusters e servidores de arquivos devem ser criados nos workspaces</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2941">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="3c5b0-2942">[ALTERAÇÃO SIGNIFICATIVA] Os trabalhos devem ser criados nas experiências</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2942">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="3c5b0-2943">[ALTERAÇÃO SIGNIFICATIVA]`--nfs-resource-group` foi removido dos comandos `cluster create` e `job create`.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2943">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="3c5b0-2944">Para montar um NFS pertencente a outro workspace/grupo de recursos, forneça a ID de ARM do servidor de arquivos através da opção `--nfs`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2944">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="3c5b0-2945">[ALTERAÇÃO SIGNIFICATIVA]`--cluster-resource-group` foi removido do comando `job create`.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2945">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="3c5b0-2946">Para enviar um trabalho em um cluster pertencente a outro workspace/grupo de recursos, forneça a ID de ARM do cluster através da opção `--cluster`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2946">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="3c5b0-2947">[ALTERAÇÃO SIGNIFICATIVA] O atributo `location` foi removido de trabalhos, cluster e servidores de arquivos.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2947">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="3c5b0-2948">Agora, o local é um atributo de um workspace.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2948">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="3c5b0-2949">[ALTERAÇÃO SIGNIFICATIVA]`--location` foi removido dos comandos `job create` e `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2949">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="3c5b0-2950">[ALTERAÇÃO SIGNIFICATIVA] Os nomes das opções curtas foi alterado para tornar a interface mais consistente:</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2950">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="3c5b0-2951">[`--config`, `-c`] foi renomeado para [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2951">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="3c5b0-2952">[`--cluster`, `-r`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2952">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="3c5b0-2953">[`--cluster`, `-n`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2953">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="3c5b0-2954">[`--job`, `-n`] foi renomeado para [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2954">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="3c5b0-2955">Mapas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2955">Maps</span></span>

* <span data-ttu-id="3c5b0-2956">[ALTERAÇÃO SIGNIFICATIVA]`maps account create` foi alterado para exigir a aceitação dos Termos de Serviço pelo prompt interativo ou sinalizador `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2956">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-2957">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2957">Network</span></span>

* <span data-ttu-id="3c5b0-2958">Suporte adicionado para `https` a `network lb probe create` [nº6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2958">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="3c5b0-2959">Foi corrigido o problema em que `--endpoint-status` diferenciava maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2959">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="3c5b0-2960">#6502</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2960">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="3c5b0-2961">Reservas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2961">Reservations</span></span>

* <span data-ttu-id="3c5b0-2962">[ALTERAÇÃO SIGNIFICATIVA] Foi adicionado o parâmetro `ReservedResourceType` necessário a `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2962">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="3c5b0-2963">Parâmetro `Location` adicionado a `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2963">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="3c5b0-2964">[ALTERAÇÃO SIGNIFICATIVA]`kind` foi removido de `ReservationProperties`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2964">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="3c5b0-2965">[ALTERAÇÃO SIGNIFICATIVA]`capabilities` foi renomeado para `sku_properties` em `Catalog`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2965">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="3c5b0-2966">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `size` e `tier` foram removidas de `Catalog`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2966">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="3c5b0-2967">Parâmetro `InstanceFlexibility` adicionado a `reservations reservation update`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2967">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="3c5b0-2968">Função</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2968">Role</span></span>

* <span data-ttu-id="3c5b0-2969">Tratamento de erro melhorado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2969">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="3c5b0-2970">SQL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2970">SQL</span></span>

* <span data-ttu-id="3c5b0-2971">Foi corrigido um erro confuso ao executar `az sql db list-editions` para um local que não está disponível para sua assinatura</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2971">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-2972">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2972">Storage</span></span>

* <span data-ttu-id="3c5b0-2973">A saída da tabela foi alterada para `storage blob download` para ser mais legível</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2973">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="3c5b0-2974">VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2974">VM</span></span>

* <span data-ttu-id="3c5b0-2975">A verificação da refinação do tamanho da VM foi aprimorada para o suporte de rede acelerada em `vm create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2975">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="3c5b0-2976">Foi adicionado um aviso para `vmss create` informando que o tamanho padrão da VM será alternado de `Standard_D1_v2` para `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2976">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="3c5b0-2977">Foi adicionado `--force-update` a `[vm|vmss] extension set` para atualizar a extensão mesmo quando a configuração não foi alterada</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2977">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="3c5b0-2978">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2978">June 13, 2018</span></span>

<span data-ttu-id="3c5b0-2979">Versão 2.0.37</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2979">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="3c5b0-2980">Núcleo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2980">Core</span></span>

* <span data-ttu-id="3c5b0-2981">A telemetria interativa foi melhorada</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2981">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="3c5b0-2982">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2982">June 13, 2018</span></span>

<span data-ttu-id="3c5b0-2983">Versão 2.0.36</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2983">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="3c5b0-2984">AKS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2984">AKS</span></span>

* <span data-ttu-id="3c5b0-2985">Foram adicionadas opções avançadas de rede para `aks create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2985">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="3c5b0-2986">Foram adicionados argumentos para `aks create` para habilitar o monitoramento e roteamento de HTTP</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2986">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="3c5b0-2987">Adicionado o argumento `--no-ssh-key` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2987">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="3c5b0-2988">Adicionado o argumento `--enable-rbac` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2988">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="3c5b0-2989">[VERSÃO PRÉVIA] Suporte adicionado para a autenticação do Azure Active Directory no `aks create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2989">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-2990">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2990">AppService</span></span>

* <span data-ttu-id="3c5b0-2991">Foi corrigido um problema com as versões urllib incompatíveis</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2991">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="3c5b0-2992">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2992">June 5, 2018</span></span>

<span data-ttu-id="3c5b0-2993">Versão 2.0.35</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2993">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="3c5b0-2994">Interativo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2994">Interactive</span></span>

* <span data-ttu-id="3c5b0-2995">Foram adicionados limites para as dependências do modo interativo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2995">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="3c5b0-2996">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2996">June 5, 2018</span></span>

<span data-ttu-id="3c5b0-2997">Versão 2.0.34</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2997">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="3c5b0-2998">Núcleo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2998">Core</span></span>

* <span data-ttu-id="3c5b0-2999">Suporte adicionado para referência de recursos de locatário cruzado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-2999">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="3c5b0-3000">Melhor confiabilidade de carregamento de telemetria</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3000">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-3001">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3001">ACR</span></span>

* <span data-ttu-id="3c5b0-3002">Suporte adicionado para VSTS como um local de origem remota</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3002">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="3c5b0-3003">Adicionado o comando `acr import`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3003">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="3c5b0-3004">AKS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3004">AKS</span></span>

* <span data-ttu-id="3c5b0-3005">`aks get-credentials` foi alterado para criar o arquivo de configuração kube com permissões de sistema de arquivos mais seguras</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3005">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="3c5b0-3006">Lote</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3006">Batch</span></span>

* <span data-ttu-id="3c5b0-3007">Correção do bug na formatação de tabela da lista de Pool [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3007">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="3c5b0-3008">IOT</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3008">IOT</span></span>

* <span data-ttu-id="3c5b0-3009">Suporte adicionado para a criação de Hubs IoT de Camada Básica</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3009">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-3010">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3010">Network</span></span>

* <span data-ttu-id="3c5b0-3011">`network vnet peering` melhorado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3011">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="3c5b0-3012">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3012">Policy Insights</span></span>

* <span data-ttu-id="3c5b0-3013">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3013">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="3c5b0-3014">ARM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3014">ARM</span></span>

* <span data-ttu-id="3c5b0-3015">Comandos `account management-group` adicionados.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3015">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="3c5b0-3016">SQL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3016">SQL</span></span>

* <span data-ttu-id="3c5b0-3017">Novos comandos de instância gerenciada adicionados:</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3017">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="3c5b0-3018">Novos comandos de banco de dados gerenciado adicionados:</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3018">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="3c5b0-3019">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3019">Storage</span></span>

* <span data-ttu-id="3c5b0-3020">Mimetypes extra adicionados para json e javascript para ser deduzido de extensões de arquivo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3020">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="3c5b0-3021">VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3021">VM</span></span>

* <span data-ttu-id="3c5b0-3022">`vm list-skus` foi alterado para usar colunas fixas e adicionar o aviso de que `Tier` e `Size` serão removidos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3022">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="3c5b0-3023">Opção `--accelerated-networking` adicionada a `vm create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3023">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="3c5b0-3024">`--tags` foi adicionado a `identity create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3024">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="3c5b0-3025">22 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3025">May 22, 2018</span></span>

<span data-ttu-id="3c5b0-3026">Versão 2.0.33</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3026">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="3c5b0-3027">Núcleo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3027">Core</span></span>

* <span data-ttu-id="3c5b0-3028">Suporte adicionado para expandir `@` em nomes de arquivos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3028">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="3c5b0-3029">ACS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3029">ACS</span></span>

* <span data-ttu-id="3c5b0-3030">Novos comandos de espaços de desenvolvimento `aks use-dev-spaces` e `aks remove-dev-spaces` foram adicionados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3030">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="3c5b0-3031">Erro de digitação corrigido na mensagem de ajuda</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3031">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-3032">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3032">AppService</span></span>

* <span data-ttu-id="3c5b0-3033">Comandos melhorados de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3033">Improved generic update commands</span></span>
* <span data-ttu-id="3c5b0-3034">Suporte assíncrono adicionado para `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3034">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="3c5b0-3035">Contêiner</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3035">Container</span></span>

* <span data-ttu-id="3c5b0-3036">Suporte adicionado para a exportação de um grupo de contêiner no formato yaml</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3036">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="3c5b0-3037">Suporte adicionado para usar um arquivo yaml para criar/atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3037">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="3c5b0-3038">Extensão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3038">Extension</span></span>

* <span data-ttu-id="3c5b0-3039">Remoção de extensões melhorada</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3039">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="3c5b0-3040">Interativo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3040">Interactive</span></span>

* <span data-ttu-id="3c5b0-3041">Log de alterações alterado para silenciar o analisador para conclusões</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3041">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="3c5b0-3042">Manipulação aprimorada de caches de ajuda inválida</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3042">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="3c5b0-3043">KeyVault</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3043">KeyVault</span></span>

* <span data-ttu-id="3c5b0-3044">Comandos de keyvault corrigidos para trabalhar no cloud shell ou VMs com identidade</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3044">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-3045">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3045">Network</span></span>

* <span data-ttu-id="3c5b0-3046">Corrija o problema em que `network watcher show-topology` não funcionará com o nome de rede virtual e/ou sub-rede [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3046">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="3c5b0-3047">Corrija o problema onde alguns comandos `network watcher` iriam declarar que o Observador de Rede não está habilitado para regiões quando na verdade é [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3047">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="3c5b0-3048">SQL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3048">SQL</span></span>

* <span data-ttu-id="3c5b0-3049">[ALTERAÇÃO SIGNIFICATIVA] Objetos de resposta alterados retornados dos comandos `db` e `dw`:</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3049">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="3c5b0-3050">A propriedade `serviceLevelObjective` foi renomeada para `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3050">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="3c5b0-3051">As propriedades `currentServiceObjectiveId` e `requestedServiceObjectiveId` foram removidas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3051">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="3c5b0-3052">A propriedade `maxSizeBytes` foi alterada para ser um valor inteiro em vez de uma cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3052">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="3c5b0-3053">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `db` e `dw` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3053">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="3c5b0-3054">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3054">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="3c5b0-3055">Para atualizar, use o parâmetro `--service-objective` ou defina a propriedade `sku.name`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3055">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="3c5b0-3056">`edition`.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3056">`edition`.</span></span> <span data-ttu-id="3c5b0-3057">Para atualizar, use o parâmetro `--edition` ou defina a propriedade `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3057">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="3c5b0-3058">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3058">`elasticPoolName`.</span></span> <span data-ttu-id="3c5b0-3059">Para atualizar, use o parâmetro `--elastic-pool` ou defina a propriedade `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3059">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="3c5b0-3060">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `elastic-pool` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3060">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="3c5b0-3061">`edition`.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3061">`edition`.</span></span> <span data-ttu-id="3c5b0-3062">Para atualizar, use o parâmetro `--edition`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3062">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="3c5b0-3063">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3063">`dtu`.</span></span> <span data-ttu-id="3c5b0-3064">Para atualizar, use o parâmetro `--capacity`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3064">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="3c5b0-3065">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3065">`databaseDtuMin`.</span></span> <span data-ttu-id="3c5b0-3066">Para atualizar, use o parâmetro `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3066">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="3c5b0-3067">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3067">`databaseDtuMax`.</span></span> <span data-ttu-id="3c5b0-3068">Para atualizar, use o parâmetro `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3068">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="3c5b0-3069">Os parâmetros `--family` e `--capacity` foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3069">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="3c5b0-3070">Os formatadores de tabela foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3070">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-3071">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3071">Storage</span></span>

* <span data-ttu-id="3c5b0-3072">Complemento adicionado ao argumento `--account-name`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3072">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="3c5b0-3073">O problema com `storage entity query` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3073">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="3c5b0-3074">VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3074">VM</span></span>

* <span data-ttu-id="3c5b0-3075">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3075">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="3c5b0-3076">O mesmo suporte pode ser acessado por meio de `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3076">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="3c5b0-3077">Imagem de extensão fixa correspondente em `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3077">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="3c5b0-3078">`--boot-diagnostics-storage` foi adicionado a `vm create` para capturar o log de inicialização</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3078">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="3c5b0-3079">`--license-type` foi adicionado a `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3079">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="3c5b0-3080">7 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3080">May 7, 2018</span></span>

<span data-ttu-id="3c5b0-3081">Versão 2.0.32</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3081">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="3c5b0-3082">Núcleo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3082">Core</span></span>

* <span data-ttu-id="3c5b0-3083">Foi corrigida uma exceção sem tratamento ao recuperar segredos de uma conta de entidade de serviço com certificado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3083">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="3c5b0-3084">Adicionado suporte limitado para argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3084">Added limited support for positional arguments</span></span>
* <span data-ttu-id="3c5b0-3085">Corrigir problema no qual `--query` não pôde ser usado com `--ids`.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3085">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="3c5b0-3086">#5591</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3086">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="3c5b0-3087">Foram melhorados os cenários de redirecionamento de comandos ao usar `--ids`.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3087">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="3c5b0-3088">Oferece suporte a `-o tsv` com uma consulta especificada ou `-o json` sem especificar uma consulta</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3088">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="3c5b0-3089">Foram adicionadas sugestões de comando sobre o erro se os usuários cometeram algum erro de digitação em seus comandos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3089">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="3c5b0-3090">Erro corrigido quando os usuários digitam `az ''`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3090">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="3c5b0-3091">Foram adicionados tipos de recursos personalizados com suporte para módulos de comando e extensões</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3091">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-3092">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3092">ACR</span></span>

* <span data-ttu-id="3c5b0-3093">Foram adicionados comandos de compilação de ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3093">Added ACR Build commands</span></span>
* <span data-ttu-id="3c5b0-3094">O recurso aprimorado não encontrou mensagens de erro</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3094">Improved resource not found error messages</span></span>
* <span data-ttu-id="3c5b0-3095">Desempenho de criação de recurso aprimorado e tratamento de erros</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3095">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="3c5b0-3096">Logon de acr aprimorado em consoles não padrão e WSL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3096">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="3c5b0-3097">Mensagens de erro de comandos de repositório aprimoradas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3097">Improved repository commands error messages</span></span>
* <span data-ttu-id="3c5b0-3098">Colunas de tabela e ordenação atualizadas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3098">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="3c5b0-3099">ACS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3099">ACS</span></span>

* <span data-ttu-id="3c5b0-3100">Foi adicionado um aviso informando que `az aks` é um serviço de versão prévia</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3100">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="3c5b0-3101">Foi corrigido um problema de permissão em `aks install-connector` quando `--aci-resource-group` não for especificado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3101">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="3c5b0-3102">AMS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3102">AMS</span></span>

* <span data-ttu-id="3c5b0-3103">Versão inicial — Gerenciar recursos dos Serviços de Mídia do Azure</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3103">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-3104">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3104">Appservice</span></span>

* <span data-ttu-id="3c5b0-3105">Correção de bug no `webapp delete` quando `--slot` é fornecido</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3105">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="3c5b0-3106">`--runtime-version` foi removido de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3106">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="3c5b0-3107">Foi adicionado suporte para min\_tls\_versão e https2.0</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3107">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="3c5b0-3108">Suporte adicionado para vários contêineres</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3108">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="3c5b0-3109">Lote AI</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3109">Batch AI</span></span>

* <span data-ttu-id="3c5b0-3110">O `batchai create cluster` foi alterado para respeitar a prioridade de VM configurada no arquivo de configuração do cluster</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3110">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="3c5b0-3111">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3111">Cognitive Services</span></span>

* <span data-ttu-id="3c5b0-3112">Foi corrigido um erro de digitação no exemplo para `cognitiveservices account create`[#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3112">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="3c5b0-3113">Consumo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3113">Consumption</span></span>

* <span data-ttu-id="3c5b0-3114">Foram adicionados novos comandos para a API de orçamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3114">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="3c5b0-3115">Contêiner</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3115">Container</span></span>

* <span data-ttu-id="3c5b0-3116">Requisito removido para `--registry-server` e `container create` quando um servidor de registro estiver incluído no nome da imagem</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3116">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="3c5b0-3117">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3117">Cosmos DB</span></span>

* <span data-ttu-id="3c5b0-3118">Introdução ao suporte de rede virtual para a CLI do Azure — Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3118">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="3c5b0-3119">DMS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3119">DMS</span></span>

* <span data-ttu-id="3c5b0-3120">Versão inicial — Adiciona suporte ao SQL para o cenário de migração do SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3120">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="3c5b0-3121">Extensão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3121">Extension</span></span>

* <span data-ttu-id="3c5b0-3122">Correção do bug em que os metadados de extensão pararam de ser exibidos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3122">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="3c5b0-3123">Interativo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3123">Interactive</span></span>

* <span data-ttu-id="3c5b0-3124">Permitir que complementos interativos funcionem com argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3124">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="3c5b0-3125">Resultado mais simplificado quando os usuários digitam '\'</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3125">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="3c5b0-3126">Conclusões corrigidas para parâmetros sem ajuda</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3126">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="3c5b0-3127">Descrições corrigidas para grupos de comando</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3127">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="3c5b0-3128">Laboratório</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3128">Lab</span></span>

* <span data-ttu-id="3c5b0-3129">Regressões corrigidas de conversão de aptidão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3129">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-3130">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3130">Network</span></span>

* <span data-ttu-id="3c5b0-3131">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--ids` removido de:</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3131">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="3c5b0-3132">Perfil</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3132">Profile</span></span>

* <span data-ttu-id="3c5b0-3133">Detecção de origem do `disk create` corrigida</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3133">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="3c5b0-3134">[ALTERAÇÃO SIGNIFICATIVA]`--msi-port` e `--identity-port` removidos porque não são mais usados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3134">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="3c5b0-3135">Erro de digitação corrigido no resumo do `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3135">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="3c5b0-3136">Redis</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3136">Redis</span></span>

* <span data-ttu-id="3c5b0-3137">`redis patch-schedule patch-schedule show` preterido em favor de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3137">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="3c5b0-3138">`redis list-all` preterido.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3138">Deprecated `redis list-all`.</span></span> <span data-ttu-id="3c5b0-3139">Esta funcionalidade foi dobrada em `redis list`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3139">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="3c5b0-3140">`redis import-method` preterido em favor de `redis import`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3140">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="3c5b0-3141">Foi adicionado suporte a `--ids` para vários comandos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3141">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="3c5b0-3142">Função</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3142">Role</span></span>

* <span data-ttu-id="3c5b0-3143">[ALTERAÇÃO SIGNIFICATIVA] Remoção de `ad sp reset-credentials` preterido</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3143">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-3144">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3144">Storage</span></span>

* <span data-ttu-id="3c5b0-3145">Permitir que o token SAS de destino aplique na origem a cópia do blob se a SAS de origem e a chave de conta não forem especificadas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3145">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="3c5b0-3146">Exposto -- tempo limite do soquete para carregamentos e downloads de blobs</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3146">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="3c5b0-3147">Tratar os nomes de blobs que começam com separadores de caminho como caminhos relativos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3147">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="3c5b0-3148">Permitir `storage blob copy --source-sas` com a inicialização char de consulta, '?'</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3148">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="3c5b0-3149">`storage entity query --marker` foi corrigido para aceitar a lista de chaves = valores</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3149">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="3c5b0-3150">VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3150">VM</span></span>

* <span data-ttu-id="3c5b0-3151">Uma lógica de detecção inválida foi corrigida no URI do blob não gerenciado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3151">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="3c5b0-3152">Adicionada criptografia de disco de suporte sem entidades de serviço fornecidas pelo usuário</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3152">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="3c5b0-3153">[ALTERAÇÃO SIGNIFICATIVA] Não usar a VM 'ManagedIdentityExtension' para suporte de MSI</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3153">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="3c5b0-3154">Suporte adicionado para a política de remoção em `vmss`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3154">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="3c5b0-3155">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--ids` de:</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3155">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="3c5b0-3156">Foi adicionado suporte do acelerador de gravação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3156">Added write accelerator support</span></span>
* <span data-ttu-id="3c5b0-3157">Adicionado `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3157">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="3c5b0-3158">`vm diagnostics set` foi corrigido para detectar o tipo de sistema operacional da VM de forma confiável</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3158">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="3c5b0-3159">`vm resize` foi alterado para verificar se o tamanho solicitado é diferente daquele definido no momento e atualizar somente na alteração</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3159">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="3c5b0-3160">10 de abril de 2018</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3160">April 10, 2018</span></span>

<span data-ttu-id="3c5b0-3161">Versão 2.0.31</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3161">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-3162">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3162">ACR</span></span>

* <span data-ttu-id="3c5b0-3163">Melhoria do tratamento de erros do fallback do wincred</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3163">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="3c5b0-3164">ACS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3164">ACS</span></span>

* <span data-ttu-id="3c5b0-3165">Alteração da validade de SPNs criados pelo AKS para 5 anos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3165">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-3166">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3166">Appservice</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="3c5b0-3168">Correção da exceção não identificada de planos de webapp inexistentes</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3168">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="3c5b0-3169">BatchAI</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3169">BatchAI</span></span>

* <span data-ttu-id="3c5b0-3170">Adição de suporte para a API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3170">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="3c5b0-3171">Montagem de nível de trabalho</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3171">Job level mounting</span></span>
  - <span data-ttu-id="3c5b0-3172">Variáveis de ambiente com valores secretos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3172">Environment variables with secret values</span></span>
  - <span data-ttu-id="3c5b0-3173">Configurações de contadores de desempenho</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3173">Performance counters settings</span></span>
  - <span data-ttu-id="3c5b0-3174">Relatório de segmento de linha específico de trabalho</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3174">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="3c5b0-3175">Suporte para subpastas na API de arquivos de lista</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3175">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="3c5b0-3176">Relatório de uso e limites</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3176">Usage and limits reporting</span></span>
  - <span data-ttu-id="3c5b0-3177">Permitir a especificação do tipo de cache para servidores NFS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3177">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="3c5b0-3178">Suporte para imagens personalizadas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3178">Support for custom images</span></span>
  - <span data-ttu-id="3c5b0-3179">Adição de suporte para o kit de ferramentas pyTorch</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3179">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="3c5b0-3180">Adição do comando `job wait`, que permite aguardar a conclusão do trabalho e relata o código de saída de trabalho</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3180">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="3c5b0-3181">Adição do comando `usage show` para listar o uso e os limites do IA do Lote atual para diferentes regiões</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3181">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="3c5b0-3182">Há suporte para nuvens nacionais</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3182">National clouds are supported</span></span>
* <span data-ttu-id="3c5b0-3183">Adição de argumentos de linha de comando do trabalho para montar sistemas de arquivos no nível de trabalho, além de arquivos de configuração</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3183">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="3c5b0-3184">Adição de mais opções para personalizar clusters — prioridade de VM, sub-rede, contagem inicial de nós para clusters de dimensionamento automático, especificando a imagem personalizada</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3184">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="3c5b0-3185">Adição de opção de linha de comando para especificar o tipo de cache de NFS gerenciado por IA do Lote</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3185">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="3c5b0-3186">Simplificação da especificação do sistema de arquivos de montagem nos arquivos de configuração.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3186">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="3c5b0-3187">Agora é possível omitir as credenciais do Compartilhamento de arquivos do Azure e Contêineres de Blob do Azure — a CLI preencherá credenciais ausentes usando a chave da conta de armazenamento fornecida por meio dos parâmetros de linha de comando ou especificada por meio da variável de ambiente ou consultará a chave a partir do Armazenamento do Azure (se a conta de armazenamento pertencer à assinatura atual)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3187">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="3c5b0-3188">O comando do fluxo de arquivo de trabalho agora é preenchido automaticamente quando o trabalho é concluído (com êxito, com falha, encerrado ou excluído)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3188">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="3c5b0-3189">Melhoria da saída de `table` para operações de `show`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3189">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="3c5b0-3190">Adição da opção `--use-auto-storage` para a criação de cluster.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3190">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="3c5b0-3191">Essa opção simplifica o gerenciamento de contas de armazenamento e a montagem do Compartilhamento de arquivos do Azure e dos Contêineres de Blob do Azure para clusters</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3191">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="3c5b0-3192">Adição da opção `--generate-ssh-keys` para `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3192">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="3c5b0-3193">Adição da capacidade de fornecer a tarefa de configuração de nó por meio da linha de comando</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3193">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="3c5b0-3194">[ALTERAÇÃO SIGNIFICATIVA] Comandos `job stream-file` e `job list-files` movidos para o grupo `job file`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3194">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="3c5b0-3195">[ALTERAÇÃO SIGNIFICATIVA]`--admin-user-name` renomeado para `--user-name` no comando `file-server create` para ser consistente com o comando `cluster create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3195">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="3c5b0-3196">Cobrança</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3196">Billing</span></span>

* <span data-ttu-id="3c5b0-3197">Adição de comandos da conta de registro</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3197">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="3c5b0-3198">Consumo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3198">Consumption</span></span>

* <span data-ttu-id="3c5b0-3199">Adicionados os comandos `marketplace`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3199">Added `marketplace` commands</span></span>
* <span data-ttu-id="3c5b0-3200">[ALTERAÇÃO SIGNIFICATIVA]`reservations summaries` renomeado para `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3200">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="3c5b0-3201">[ALTERAÇÃO SIGNIFICATIVA]`reservations details` renomeado para `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3201">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="3c5b0-3202">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--reservation-order-id` e `--reservation-id` para os comandos `reservation`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3202">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="3c5b0-3203">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--grain` para os comandos `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3203">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="3c5b0-3204">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--include-meter-details` para os comandos `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3204">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="3c5b0-3205">Contêiner</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3205">Container</span></span>

* <span data-ttu-id="3c5b0-3206">Adição dos parâmetros de montagem de volume do Repositório Git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` e `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3206">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="3c5b0-3207">Correção de [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` com falha com --container-name especificado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3207">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="3c5b0-3208">Extensão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3208">Extension</span></span>

* <span data-ttu-id="3c5b0-3209">Alteração da mensagem de verificação de distribuição para ser de nível de depuração</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3209">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="3c5b0-3210">Interativo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3210">Interactive</span></span>

* <span data-ttu-id="3c5b0-3211">Alteração para interromper as conclusões após comandos não reconhecidos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3211">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="3c5b0-3212">Adição de ganchos de eventos antes e depois da criação da subárvore do comando</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3212">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="3c5b0-3213">Adição de conclusão para parâmetros `--ids`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3213">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-3214">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3214">Network</span></span>

* <span data-ttu-id="3c5b0-3215">Correção de [#5936](https://github.com/Azure/azure-cli/issues/5936): as marcas `application-gateway create` não podiam ser definidas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3215">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="3c5b0-3216">Adição do argumento `--auth-certs` para anexar certificados de autenticação para `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3216">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="3c5b0-3217">#4910</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3217">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="3c5b0-3218">Adição dos comandos `ddos-protection` para criar planos de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3218">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="3c5b0-3219">Adição de suporte de `--ddos-protection-plan` a `vnet [create|update]` para associar uma VNET a um plano de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3219">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="3c5b0-3220">Correção do problema com o sinalizador `--disable-bgp-route-propagation` em `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3220">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="3c5b0-3221">Remoção de argumentos fictícios `--public-ip-address-type` e `--subnet-type` para `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3221">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="3c5b0-3222">Adição de suporte para registros TXT com sequências de escape RFC 1035 para `network dns zone [import|export]` e `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3222">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="3c5b0-3223">Perfil</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3223">Profile</span></span>

* <span data-ttu-id="3c5b0-3224">Adição de suporte para contas clássicas do Azure em `account list`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3224">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="3c5b0-3225">[ALTERAÇÃO SIGNIFICATIVA] Remoção dos argumentos `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3225">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="3c5b0-3226">RDBMS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3226">RDBMS</span></span>

* <span data-ttu-id="3c5b0-3227">Adicionado o comando `georestore`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3227">Added `georestore` command</span></span>
* <span data-ttu-id="3c5b0-3228">Remoção da restrição de tamanho de armazenamento do comando `create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3228">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="3c5b0-3229">Recurso</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3229">Resource</span></span>

* <span data-ttu-id="3c5b0-3230">Adicionado o suporte ao `--metadata` para `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3230">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="3c5b0-3231">Adição de suporte para `--metadata`, `--set`, `--add`, `--remove` para `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3231">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="3c5b0-3232">SQL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3232">SQL</span></span>

* <span data-ttu-id="3c5b0-3233">Adição de `sql elastic-pool op list` e `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3233">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-3234">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3234">Storage</span></span>

* <span data-ttu-id="3c5b0-3235">Melhoria de mensagens de erro para cadeias de conexão malformadas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3235">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="3c5b0-3236">VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3236">VM</span></span>

* <span data-ttu-id="3c5b0-3237">Adição de suporte para configurar a contagem de domínios de falha da plataforma para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3237">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="3c5b0-3238">Alteração de `vmss create` para balanceador de carga padrão para um conjunto de dimensionamento desabilitado zonal, grande ou de único grupo de posicionamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3238">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [ALTERAÇÃO SIGNIFICATIVA]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="3c5b0-3240">Adição de suporte para a SKU de IP público para `vm create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3240">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="3c5b0-3241">Adição dos argumentos `--keyvault` e `--resource-group` para `vm secret format` para oferecer suporte a cenários em que o comando não é capaz de resolver a ID do cofre.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3241">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="3c5b0-3242">#5718</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3242">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="3c5b0-3243">Melhoria de erros de `[vm|vmss create]` quando um local do grupo de recursos não tem suporte de zona</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3243">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="3c5b0-3244">27 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3244">March 27, 2018</span></span>

<span data-ttu-id="3c5b0-3245">Versão 2.0.30</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3245">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="3c5b0-3246">Núcleo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3246">Core</span></span>

* <span data-ttu-id="3c5b0-3247">Mostrar mensagem para extensões marcadas como versão prévia na Ajuda</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3247">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="3c5b0-3248">ACS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3248">ACS</span></span>

* <span data-ttu-id="3c5b0-3249">Corrija o erro de verificação de certificado SSL para `aks install-cli` no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3249">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-3250">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3250">Appservice</span></span>

* <span data-ttu-id="3c5b0-3251">Adição do suporte somente para HTTPS para `webapp update`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3251">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="3c5b0-3252">Adição do suporte para os slots `az webapp identity [assign|show]` e `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3252">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="3c5b0-3253">Backup</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3253">Backup</span></span>

* <span data-ttu-id="3c5b0-3254">Adição do novo comando `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3254">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="3c5b0-3255">Esse comando pode ser usado para verificar se o backup de uma VM é realizado por qualquer cofre na assinatura</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3255">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="3c5b0-3256">Habilitação das IDs de objeto do Azure para os parâmetros `--resource-group` e `--vault-name` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3256">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="3c5b0-3257">`--name` parâmetros alterados a fim de aceitar o formato de saída dos comandos `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3257">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="3c5b0-3258">Contêiner</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3258">Container</span></span>

* <span data-ttu-id="3c5b0-3259">Adição do comando `container exec`.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3259">Added `container exec` command.</span></span> <span data-ttu-id="3c5b0-3260">Executa comandos em um contêiner para um grupo de contêiner em execução</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3260">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="3c5b0-3261">Permitir a saída da tabela para criar e atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3261">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="3c5b0-3262">Extensão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3262">Extension</span></span>

* <span data-ttu-id="3c5b0-3263">Mensagem adicionada para `extension add`, se a extensão estiver no modo de versão prévia</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3263">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="3c5b0-3264">`extension list-available` alterado para mostrar dados de extensão total com `--show-details`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3264">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="3c5b0-3265">[ALTERAÇÃO SIGNIFICATIVA]`extension list-available` alterado para mostrar dados de extensão simplificados por padrão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3265">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="3c5b0-3266">Interativo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3266">Interactive</span></span>

* <span data-ttu-id="3c5b0-3267">Alteração nas conclusões para ativar após a conclusão do carregamento da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3267">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="3c5b0-3268">Correção de bug usando o parâmetro `--style`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3268">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="3c5b0-3269">Analisador léxico interativo instanciado após a falta do despejo da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3269">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="3c5b0-3270">Suporte aprimorado ao completador</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3270">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="3c5b0-3271">Laboratório</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3271">Lab</span></span>

* <span data-ttu-id="3c5b0-3272">Correção de bugs com o comando `create environment`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3272">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="3c5b0-3273">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3273">Monitor</span></span>

* <span data-ttu-id="3c5b0-3274">Adicionado suporte para `--top`, `--orderby` e `--namespace` para `metrics list` [nº5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3274">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="3c5b0-3275">Corrigido [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` aceita uma lista separada por espaços de métricas para recuperação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3275">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="3c5b0-3276">Suporte adicionado para `--namespace` a `metrics list-definitions` [nº5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3276">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-3277">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3277">Network</span></span>

* <span data-ttu-id="3c5b0-3278">Adição de suporte para zonas DNS privado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3278">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="3c5b0-3279">Perfil</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3279">Profile</span></span>

* <span data-ttu-id="3c5b0-3280">Adição de avisos para `--identity-port` e `--msi-port` para `login`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3280">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="3c5b0-3281">RDBMS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3281">RDBMS</span></span>

* <span data-ttu-id="3c5b0-3282">Adição de modelo de negócios GA API versão 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3282">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="3c5b0-3283">Recurso</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3283">Resource</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="3c5b0-3285">Função</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3285">Role</span></span>

* <span data-ttu-id="3c5b0-3286">Adição de suporte para configurações de acesso necessário e clientes nativos para `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3286">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="3c5b0-3287">`rbac` comandos alterados para retornar menos de 1000 IDs na resolução do objeto</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3287">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="3c5b0-3288">Adição de comandos de gerenciamento de credencial `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3288">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="3c5b0-3289">[ALTERAÇÃO SIGNIFICATIVA] "Propriedades" removidas da saída `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3289">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="3c5b0-3290">Adição de suporte para as permissões `dataActions` e `notDataActions` para `role definition`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3290">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-3291">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3291">Storage</span></span>

* <span data-ttu-id="3c5b0-3292">Correção de problema ao carregar um arquivo com tamanho entre 195 e 200 GB</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3292">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="3c5b0-3293">Corrigido [#4049](https://github.com/Azure/azure-cli/issues/4049): problemas com o acréscimo de uploads de blob ignorando os parâmetros da condição</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3293">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="3c5b0-3294">VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3294">VM</span></span>

* <span data-ttu-id="3c5b0-3295">Adição de aviso para `vmss create` para alterações de falha futuras para conjuntos com mais de 100 instâncias</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3295">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="3c5b0-3296">Adição de suporte com flexibilidade de região para `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3296">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="3c5b0-3297">Alteração no modo de exibição de instância de disco para reportar status de criptografia mais adequados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3297">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="3c5b0-3298">[ALTERAÇÃO SIGNIFICATIVA]`vm extension delete` alterado para não retornar mais a saída</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3298">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="3c5b0-3299">13 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3299">March 13, 2018</span></span>

<span data-ttu-id="3c5b0-3300">Versão 2.0.29</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3300">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-3301">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3301">ACR</span></span>

* <span data-ttu-id="3c5b0-3302">Suporte adicionado do parâmetro `--image` a `repository delete`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3302">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="3c5b0-3303">Parâmetros `--manifest` e `--tag` preteridos do comando `repository delete`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3303">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="3c5b0-3304">Comando `repository untag` adicionado para remover uma marcação sem excluir dados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3304">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="3c5b0-3305">ACS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3305">ACS</span></span>

* <span data-ttu-id="3c5b0-3306">Comando `aks upgrade-connector` adicionado para atualizar um conector existente</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3306">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="3c5b0-3307">Arquivos de configuração `kubectl` alterados para usar um YAML mais legível em bloco</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3307">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="3c5b0-3308">Supervisor</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3308">Advisor</span></span>

* <span data-ttu-id="3c5b0-3309">[ALTERAÇÃO SIGNIFICATIVA]`advisor configuration get` renomeado para `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3309">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="3c5b0-3310">[ALTERAÇÃO SIGNIFICATIVA]`advisor configuration set` renomeado para `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3310">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="3c5b0-3311">[ALTERAÇÃO SIGNIFICATIVA]`advisor recommendation generate` removido</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3311">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="3c5b0-3312">Parâmetro `--refresh` adicionado a `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3312">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="3c5b0-3313">Adicionado o comando `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3313">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-3314">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3314">Appservice</span></span>

* <span data-ttu-id="3c5b0-3315">Preterido `[webapp|functionapp] assign-identity`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3315">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="3c5b0-3316">Comandos de identidade gerenciada `webapp identity [assign|show]` e `functionapp identity [assign|show]` adicionados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3316">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="3c5b0-3317">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3317">Eventhubs</span></span>

* <span data-ttu-id="3c5b0-3318">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3318">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="3c5b0-3319">Extensão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3319">Extension</span></span>

* <span data-ttu-id="3c5b0-3320">Verificação adicionada para avisar ao usuário se a distribuição usada é diferente da armazenado no arquivo de origem do pacote, pois isso pode levar a erros</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3320">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="3c5b0-3321">Interativo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3321">Interactive</span></span>

* <span data-ttu-id="3c5b0-3322">Corrigido [#5625](https://github.com/Azure/azure-cli/issues/5625): manter histórico em sessões diferentes</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3322">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="3c5b0-3323">Corrigido [#3016](https://github.com/Azure/azure-cli/issues/3016): histórico não registrado no escopo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3323">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="3c5b0-3324">Corrigido [#5688](https://github.com/Azure/azure-cli/issues/5688): as conclusões não aparecerão se o carregamento da tabela de comando encontrar uma exceção</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3324">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="3c5b0-3325">Medidor de progresso corrigido para operações de longa execução</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3325">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="3c5b0-3326">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3326">Monitor</span></span>

* <span data-ttu-id="3c5b0-3327">Comandos `monitor autoscale-settings` preteridos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3327">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="3c5b0-3328">Adicionados os comandos `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3328">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="3c5b0-3329">Adicionados os comandos `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3329">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="3c5b0-3330">Adicionados os comandos `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3330">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-3331">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3331">Network</span></span>

* <span data-ttu-id="3c5b0-3332">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--tags` removido de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3332">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="3c5b0-3333">Valores padrão incorretos removidos dos seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3333">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="3c5b0-3334">Comandos `network watcher connection-monitor` adicionados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3334">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="3c5b0-3335">Parâmetros `--vnet` e `--subnet` adicionados a `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3335">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="3c5b0-3336">Perfil</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3336">Profile</span></span>

* <span data-ttu-id="3c5b0-3337">Parâmetro `--msi` preterido de `az login`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3337">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="3c5b0-3338">Parâmetro `--identity` adicionado de `az login` para substituir `--msi`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3338">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="3c5b0-3339">RDBMS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3339">RDBMS</span></span>

* <span data-ttu-id="3c5b0-3340">[VISUALIZAÇÃO] Alterado para usar a API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3340">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="3c5b0-3341">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3341">Service Bus</span></span>

* <span data-ttu-id="3c5b0-3342">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3342">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-3343">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3343">Storage</span></span>

* <span data-ttu-id="3c5b0-3344">[#4971](https://github.com/Azure/azure-cli/issues/4971) corrigido: `storage blob copy` agora dá suporte a outras nuvens do Azure</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3344">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="3c5b0-3345">Corrigido [#5286](https://github.com/Azure/azure-cli/issues/5286): os comandos em lotes `storage blob [delete-batch|download-batch|upload-batch]` não geram mais um erro após falhas da pré-condição</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3345">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="3c5b0-3346">VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3346">VM</span></span>

* <span data-ttu-id="3c5b0-3347">Suporte adicionado a `[vm|vmss] create` anexar discos de dados não gerenciados e configurar o cache</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3347">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="3c5b0-3348">`[vm|vmss] assign-identity` e `[vm|vmss] remove-identity` preteridos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3348">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="3c5b0-3349">Comandos `vm identity [assign|remove|show]` e `vmss identity [assign|remove|show]` adicionados para substituir comandos preteridos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3349">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="3c5b0-3350">Prioridade padrão alterada em `vmss create` para None</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3350">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="3c5b0-3351">27 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3351">February 27, 2018</span></span>

<span data-ttu-id="3c5b0-3352">Versão 2.0.28</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3352">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="3c5b0-3353">Núcleo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3353">Core</span></span>

* <span data-ttu-id="3c5b0-3354">Corrigido [#5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3354">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="3c5b0-3355">Adição de suporte para telemetria de extensão com chaves personalizadas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3355">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="3c5b0-3356">Adição de log HTTP em `--debug`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3356">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="3c5b0-3357">ACS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3357">ACS</span></span>

* <span data-ttu-id="3c5b0-3358">Alteração para usa o gráfico `virtual-kubelet-for-aks` do Helm para `aks install-connector` por padrão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3358">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="3c5b0-3359">Problema corrigido: permissão insuficiente para entidades de serviço criarem um grupo de contêiner ACI</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3359">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="3c5b0-3360">Adição dos parâmetros `--aci-container-group`, `--location` e `--image-tag` ao `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3360">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="3c5b0-3361">Remoção do aviso de reprovação de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3361">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-3362">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3362">Appservice</span></span>

* <span data-ttu-id="3c5b0-3363">Atualizações para a nova versão do SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3363">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="3c5b0-3364">Correção [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` relatado como SKU inválido</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3364">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="3c5b0-3365">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3365">Cognitive Services</span></span>

* <span data-ttu-id="3c5b0-3366">Atualização do “aviso” ao criar uma nova conta dos Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3366">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="3c5b0-3367">Consumo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3367">Consumption</span></span>

* <span data-ttu-id="3c5b0-3368">Adição de novos comandos para a API pricesheet</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3368">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="3c5b0-3369">Atualização dos formatos existentes de Detalhes de uso e Detalhes de reserva</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3369">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="3c5b0-3370">Contêiner</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3370">Container</span></span>

* <span data-ttu-id="3c5b0-3371">Adição dos argumentos `--secrets` e `--secrets-mount-path` ao `container create` para usar segredos na ACI</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3371">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-3372">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3372">Network</span></span>

* <span data-ttu-id="3c5b0-3373">Corrigido [#5559](https://github.com/Azure/azure-cli/issues/5559): cliente ausente em `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3373">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="3c5b0-3374">Recurso</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3374">Resource</span></span>

* <span data-ttu-id="3c5b0-3375">Alteração do `group deployment export` para exibir um modelo parcial e erros ao falhar</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3375">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="3c5b0-3376">Função</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3376">Role</span></span>

* <span data-ttu-id="3c5b0-3377">Adição de `role assignment list-changelogs` para permitir a auditoria das funções da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3377">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="3c5b0-3378">SQL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3378">SQL</span></span>

* <span data-ttu-id="3c5b0-3379">Adição de suporte para a redundância de zona para os bancos de dados e pools elásticos em criação ou atualização</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3379">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-3380">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3380">Storage</span></span>

* <span data-ttu-id="3c5b0-3381">Habilitação de especificação de caminho de destino/prefixo do `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3381">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="3c5b0-3382">VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3382">VM</span></span>

* <span data-ttu-id="3c5b0-3383">Adição de suporte para anexar/desanexar discos em uma instância única de VMSS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3383">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="3c5b0-3384">13 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3384">February 13, 2018</span></span>

<span data-ttu-id="3c5b0-3385">Versão 2.0.27</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3385">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="3c5b0-3386">Núcleo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3386">Core</span></span>

* <span data-ttu-id="3c5b0-3387">Alterada a autenticação para chave tanto na ID de assinatura quanto no nome de logon do MSI</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3387">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="3c5b0-3388">ACS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3388">ACS</span></span>

* <span data-ttu-id="3c5b0-3389">[ALTERAÇÃO SIGNIFICATIVA]`aks get-versions` renomeado para `aks get-upgrades` para fins de precisão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3389">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="3c5b0-3390">`aks get-versions` alterado para mostrar versões do Kubernetes disponíveis para `aks create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3390">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="3c5b0-3391">Alterados os padrões de `aks create` para permitir que o servidor escolha a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3391">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="3c5b0-3392">Atualizadas as mensagens de ajuda sobre a entidade de serviço gerada pelo AKS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3392">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="3c5b0-3393">Alterados os tamanhos de nó padrão para `aks create` de “Standard\_D1\_v2” para “Standard\_DS1\_v2”</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3393">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="3c5b0-3394">Aumentada a confiabilidade ao localizar o pod de painel para `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3394">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="3c5b0-3395">`aks get-credentials` corrigido para tratar de erros de Unicode ao carregar arquivos de configuração do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3395">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="3c5b0-3396">Adicionada uma mensagem para `az aks install-cli` para ajudar a obter `kubectl` em `$PATH`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3396">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-3397">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3397">Appservice</span></span>

* <span data-ttu-id="3c5b0-3398">Corrigido o problema em que `webapp [backup|restore]` falhou devido a uma referência nula</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3398">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="3c5b0-3399">Adicionado suporte para planos de serviço de aplicativo padrão por meio de `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3399">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="3c5b0-3400">CDN</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3400">CDN</span></span>

* <span data-ttu-id="3c5b0-3401">Adicionados os comandos `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3401">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="3c5b0-3402">Contêiner</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3402">Container</span></span>

* <span data-ttu-id="3c5b0-3403">Adicionada a opção `--follow` para `az container logs` para logs de streaming</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3403">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="3c5b0-3404">Adicionado o comando `container attach` que anexa fluxos locais de saída e erro padrão para um contêiner em um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3404">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="3c5b0-3405">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3405">CosmosDB</span></span>

* <span data-ttu-id="3c5b0-3406">Adicionado suporte para a configuração de recursos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3406">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="3c5b0-3407">Extensão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3407">Extension</span></span>

* <span data-ttu-id="3c5b0-3408">Adicionado suporte para parâmetro `--pip-proxy` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3408">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="3c5b0-3409">Adicionado suporte para argumento `--pip-extra-index-urls` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3409">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="3c5b0-3410">Comentários</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3410">Feedback</span></span>

* <span data-ttu-id="3c5b0-3411">Adicionadas informações de extensão aos dados de telemetria</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3411">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="3c5b0-3412">Interativo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3412">Interactive</span></span>

* <span data-ttu-id="3c5b0-3413">Corrigido o problema em que o usuário é solicitado a fazer logon ao usar o modo interativo no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3413">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="3c5b0-3414">Corrigida a regressão com conclusões de parâmetro ausentes</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3414">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="3c5b0-3415">IoT</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3415">IoT</span></span>

* <span data-ttu-id="3c5b0-3416">Correção do problema em que `iot dps access policy [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3416">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="3c5b0-3417">Correção do problema em que `iot dps linked-hub [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3417">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="3c5b0-3418">Adicionado o suporte `--no-wait` para `iot dps access policy [create|update]` e `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3418">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="3c5b0-3419">`iot hub create` alterado para permitir a especificação do número de partições</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3419">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="3c5b0-3420">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3420">Monitor</span></span>

* <span data-ttu-id="3c5b0-3421">Corrigido o comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3421">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-3422">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3422">Network</span></span>

* <span data-ttu-id="3c5b0-3423">Corrigida a opção `--tags` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3423">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="3c5b0-3424">Perfil</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3424">Profile</span></span>

* <span data-ttu-id="3c5b0-3425">`az login` habilitado no modo interativo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3425">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="3c5b0-3426">Recurso</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3426">Resource</span></span>

* <span data-ttu-id="3c5b0-3427">`feature show` adicionado novamente</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3427">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="3c5b0-3428">Função</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3428">Role</span></span>

* <span data-ttu-id="3c5b0-3429">Adicionado o argumento `--available-to-other-tenants` para `ad app update`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3429">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="3c5b0-3430">SQL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3430">SQL</span></span>

* <span data-ttu-id="3c5b0-3431">Adicionados os comandos `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3431">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="3c5b0-3432">Adicionado `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3432">Added `sql db rename`</span></span>
* <span data-ttu-id="3c5b0-3433">Adicionado suporte para o argumento `--ids` para todos os comandos sql</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3433">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-3434">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3434">Storage</span></span>

* <span data-ttu-id="3c5b0-3435">Adicionados os comandos `storage blob service-properties delete-policy` e `storage blob undelete` para habilitar a exclusão reversível</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3435">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="3c5b0-3436">VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3436">VM</span></span>

* <span data-ttu-id="3c5b0-3437">Corrigida uma falha quando a criptografia de VM não pode ser totalmente inicializada</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3437">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="3c5b0-3438">Adicionada saída de ID de entidade de segurança ao habilitar o MSI</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3438">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="3c5b0-3439">`vm boot-diagnostics get-boot-log` fixo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3439">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="3c5b0-3440">31 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3440">January 31, 2018</span></span>

<span data-ttu-id="3c5b0-3441">Versão 2.0.26</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3441">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="3c5b0-3442">Núcleo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3442">Core</span></span>

* <span data-ttu-id="3c5b0-3443">Adicionado suporte para recuperação de token bruto no contexto MSI</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3443">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="3c5b0-3444">Removida a cadeia de caracteres do indicador de sondagem depois de terminar o LRO no Windows cmd.exe</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3444">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="3c5b0-3445">Adicionado um aviso que aparece ao usar um padrão configurado que foi alterado para uma entrada de nível de informações.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3445">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="3c5b0-3446">Usar `--verbose` para ver</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3446">Use `--verbose` to see</span></span>
* <span data-ttu-id="3c5b0-3447">Adicionar um indicador de progresso para comandos de espera</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3447">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="3c5b0-3448">ACS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3448">ACS</span></span>

* <span data-ttu-id="3c5b0-3449">Argumento `--disable-browser` esclarecido</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3449">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="3c5b0-3450">Preenchimento de guia melhorado para argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3450">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-3451">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3451">Appservice</span></span>

* <span data-ttu-id="3c5b0-3452">`webapp log [tail|download]` fixo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3452">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="3c5b0-3453">Removida a verificação de `kind` em aplicativos Web e funções</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3453">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="3c5b0-3454">CDN</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3454">CDN</span></span>

* <span data-ttu-id="3c5b0-3455">Corrigido o problema de cliente ausente com `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3455">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="3c5b0-3456">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3456">CosmosDB</span></span>

* <span data-ttu-id="3c5b0-3457">Corrigida a descrição do parâmetro para políticas de failover</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3457">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="3c5b0-3458">Interativo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3458">Interactive</span></span>

* <span data-ttu-id="3c5b0-3459">Corrigido o problema em que as conclusões de opção de comando não aparecem mais</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3459">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-3460">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3460">Network</span></span>

* <span data-ttu-id="3c5b0-3461">Adicionada a proteção para `--cert-password` para `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3461">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="3c5b0-3462">Corrigido o problema com `application-gateway update` em que `--sku` aplicou um valor padrão de forma errada</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3462">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="3c5b0-3463">Adicionada proteção para `--shared-key` e `--authorization-key` para `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3463">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="3c5b0-3464">Corrigido o problema de cliente ausente com `asg create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3464">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="3c5b0-3465">Adicionado o parâmetro `--file-name / -f` para nomes exportados para `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3465">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="3c5b0-3466">Os seguintes problemas foram corrigidos com `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3466">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="3c5b0-3467">Corrigido o problema em que registros TXT longos foram exportados incorretamente</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3467">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="3c5b0-3468">Corrigido o problema em que registros TXT entre aspas foram exportados incorretamente sem as aspas com caracteres de escape</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3468">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="3c5b0-3469">Corrigido o problema em que determinados registros foram importados duas vezes com `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3469">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="3c5b0-3470">Restaurados os comandos `vnet-gateway root-cert` e `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3470">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="3c5b0-3471">Perfil</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3471">Profile</span></span>

* <span data-ttu-id="3c5b0-3472">`get-access-token` corrigido para trabalhar em uma VM com identidade</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3472">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="3c5b0-3473">Recurso</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3473">Resource</span></span>

* <span data-ttu-id="3c5b0-3474">Corrigido o bug com `deployment [create|validate]` em que um aviso era exibido incorretamente quando um campo ‘tipo’ do modelo continha valores maiúsculos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3474">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-3475">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3475">Storage</span></span>

* <span data-ttu-id="3c5b0-3476">Corrigido o problema com a migração de contas de Armazenamento V1 para Armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3476">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="3c5b0-3477">Adicionado o relatório de andamento de todos os comandos de upload/download</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3477">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="3c5b0-3478">Corrigido o bug que impedia a opção “-n” arg com `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3478">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="3c5b0-3479">Adicionada a coluna ‘instantâneo’ à saída de tabela para `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3479">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="3c5b0-3480">Corrigidos bugs com vários parâmetros que precisam ser analisados como ints</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3480">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="3c5b0-3481">VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3481">VM</span></span>

* <span data-ttu-id="3c5b0-3482">Adicionado o comando `vm image accept-terms` para permitir a criação de VMs a partir de imagens com encargos adicionais</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3482">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="3c5b0-3483">`[vm|vmss create]` corrigido para garantir que comandos possam ser executados sob o proxy com certificados não assinados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3483">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="3c5b0-3484">[VERSÃO PRÉVIA] Adicionado suporte para “baixa” prioridade para VMSS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3484">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="3c5b0-3485">Adicionada a proteção para `--admin-password` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3485">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="3c5b0-3486">17 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3486">January 17, 2018</span></span>

<span data-ttu-id="3c5b0-3487">Versão 2.0.25</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3487">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-3488">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3488">ACR</span></span>

* <span data-ttu-id="3c5b0-3489">Adicionado fallback de logon de acr em erros de credencial do Windows</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3489">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="3c5b0-3490">Habilitados os logs de registro</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3490">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="3c5b0-3491">ACS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3491">ACS</span></span>

* <span data-ttu-id="3c5b0-3492">Corrigido o comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3492">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="3c5b0-3493">Removido o requisito de função do SPN</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3493">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-3494">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3494">Appservice</span></span>

* <span data-ttu-id="3c5b0-3495">Corrigido o bug com `config ssl upload` onde `hosting_environment_profile` era nulo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3495">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="3c5b0-3496">Adicionado suporte para URLs personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3496">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="3c5b0-3497">Corrigido o suporte de slot para `log tail`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3497">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="3c5b0-3498">Backup</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3498">Backup</span></span>

* <span data-ttu-id="3c5b0-3499">Alterada a opção `--container-name` de `backup item list` para ser opcional</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3499">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="3c5b0-3500">Adicionadas opções da conta de armazenamento para `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3500">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="3c5b0-3501">Corrigido o check-in de local de `backup protection enable-for-vm` para não diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3501">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="3c5b0-3502">Corrigido o problema em que os comandos falhavam com um nome de contêiner inválido</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3502">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="3c5b0-3503">Alterado `backup item list` para incluir o 'Status de Integridade' como padrão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3503">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="3c5b0-3504">Lote</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3504">Batch</span></span>

* <span data-ttu-id="3c5b0-3505">Alterado `batch login` para retornar detalhes de autenticação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3505">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="3c5b0-3506">Nuvem</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3506">Cloud</span></span>

* <span data-ttu-id="3c5b0-3507">Alterado para não exigir pontos de extremidade ao definir `--profile` em uma nuvem</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3507">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="3c5b0-3508">Consumo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3508">Consumption</span></span>

* <span data-ttu-id="3c5b0-3509">Adicionados novos comandos para reservas: `consumption reservations summaries` e `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3509">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="3c5b0-3510">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3510">Event Grid</span></span>

* <span data-ttu-id="3c5b0-3511">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid topic event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3511">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="3c5b0-3512">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid resource event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3512">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="3c5b0-3513">[ALTERAÇÃO SIGNIFICATIVA] Comando `eventgrid event-subscription show-endpoint-url` removido.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3513">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="3c5b0-3514">Usar `eventgrid event-subscription show --include-full-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3514">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="3c5b0-3515">Adicionado o comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3515">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="3c5b0-3516">Adicionado o comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3516">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="3c5b0-3517">Adicionado o parâmetro `--ids` para comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3517">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="3c5b0-3518">Adicionado o suporte de conclusão de guia para nomes de tópico</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3518">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="3c5b0-3519">Interativo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3519">Interactive</span></span>

* <span data-ttu-id="3c5b0-3520">Corrigido o problema em que o modo interativo não funcionava com o Python 2.x</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3520">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="3c5b0-3521">Corrigidos os erros na inicialização</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3521">Fixed errors on startup</span></span>
* <span data-ttu-id="3c5b0-3522">Corrigido o problema com alguns comandos que não estavam em execução no modo interativo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3522">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="3c5b0-3523">IoT</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3523">IoT</span></span>

* <span data-ttu-id="3c5b0-3524">Adicionado suporte para o serviço de provisionamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3524">Added support for device provisioning service</span></span>
* <span data-ttu-id="3c5b0-3525">Adicionadas mensagens de reprovação em comandos e ajuda de comando</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3525">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="3c5b0-3526">Adicionada verificação de IoT para informar os usuários da Extensão de IoT</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3526">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="3c5b0-3527">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3527">Monitor</span></span>

* <span data-ttu-id="3c5b0-3528">Adicionado o suporte de configuração de vários diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3528">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="3c5b0-3529">Agora o parâmetro `--name` é necessário para `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3529">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="3c5b0-3530">Adicionado o comando `monitor diagnostic-settings categories` para obter a categoria de configurações de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3530">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-3531">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3531">Network</span></span>

* <span data-ttu-id="3c5b0-3532">Corrigido o problema ao tentar alterar de/para o modo ativo-em espera com `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3532">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="3c5b0-3533">Adicionado o suporte para HTTP2 para `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3533">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="3c5b0-3534">Perfil</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3534">Profile</span></span>

* <span data-ttu-id="3c5b0-3535">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3535">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="3c5b0-3536">Função</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3536">Role</span></span>

* <span data-ttu-id="3c5b0-3537">Adicionado o argumento `--assignee-object-id` para `role assignment create` para ignorar a consulta do gráfico</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3537">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="3c5b0-3538">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3538">Service Fabric</span></span>

* <span data-ttu-id="3c5b0-3539">Adicionados erros detalhados à resposta de validação ao criar cluster</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3539">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="3c5b0-3540">Corrigido o problema de cliente ausente com vários comandos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3540">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="3c5b0-3541">VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3541">VM</span></span>

* <span data-ttu-id="3c5b0-3542">[VERSÃO PRÉVIA] Suporte entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3542">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="3c5b0-3543">[ALTERAÇÃO SIGNIFICATIVA] Alterada única zona `vmss` padrão para o balanceador de carga "Padrão"</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3543">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="3c5b0-3544">[ALTERAÇÃO SIGNIFICATIVA]`externalIdentities` alterado para `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3544">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="3c5b0-3545">[VERSÃO PRÉVIA] Adicionado o suporte para a troca de disco do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3545">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="3c5b0-3546">Adicionado o suporte para o uso de imagens da VM de outras assinaturas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3546">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="3c5b0-3547">Adicionados os argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` e `--plan-publisher` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3547">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="3c5b0-3548">Corrigidos os problemas de erro com `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3548">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="3c5b0-3549">Corrigido o uso excessivo de recursos causados por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3549">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="3c5b0-3550">19 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3550">December 19, 2017</span></span>

<span data-ttu-id="3c5b0-3551">Versão 2.0.23</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3551">Version 2.0.23</span></span>

* <span data-ttu-id="3c5b0-3552">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3552">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="3c5b0-3553">Contêiner</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3553">Container</span></span>

* <span data-ttu-id="3c5b0-3554">Corrigida a ordem incorreta de parâmetros para logs de contêiner</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3554">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-3555">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3555">Network</span></span>

* <span data-ttu-id="3c5b0-3556">Adicionado o argumento `--disable-bgp-route-propagation` para `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3556">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="3c5b0-3557">Adicionado o argumento `--ip-tags` para `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3557">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-3558">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3558">Storage</span></span>

* <span data-ttu-id="3c5b0-3559">Adicionado suporte para armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3559">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="3c5b0-3560">VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3560">VM</span></span>

* <span data-ttu-id="3c5b0-3561">[VERSÃO PRÉVIA] Adicionado suporte para identidades atribuídas a usuários para VMs e VMSSes</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3561">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="3c5b0-3562">5 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3562">December 5, 2017</span></span>

<span data-ttu-id="3c5b0-3563">Versão 2.0.22</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3563">Version 2.0.22</span></span>

* <span data-ttu-id="3c5b0-3564">Comandos `az component` removidos.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3564">Removed `az component` commands.</span></span> <span data-ttu-id="3c5b0-3565">Usar `az extension`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3565">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="3c5b0-3566">Núcleo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3566">Core</span></span>
* <span data-ttu-id="3c5b0-3567">Modificou o ponto de extremidade de autoridade AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com para login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3567">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="3c5b0-3568">Corrigido o problema onde a telemetria reenviaria continuamente</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3568">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="3c5b0-3569">ACS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3569">ACS</span></span>

* <span data-ttu-id="3c5b0-3570">Comandos `aks install-connector` e `aks remove-connector` adicionados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3570">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="3c5b0-3571">Relatório de erros aprimorado para `acs create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3571">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="3c5b0-3572">Corrigido o uso de `aks get-credentials -f` sem um caminho totalmente qualificado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3572">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="3c5b0-3573">Supervisor</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3573">Advisor</span></span>

* <span data-ttu-id="3c5b0-3574">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3574">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-3575">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3575">Appservice</span></span>

* <span data-ttu-id="3c5b0-3576">Corrigida a geração de nome do certificado com `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3576">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="3c5b0-3577">Corrigidos `webapp [list|show]` e `functionapp [list|show]` para exibir os aplicativos corretos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3577">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="3c5b0-3578">Valor padrão adicionado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3578">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="3c5b0-3579">Consumo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3579">Consumption</span></span>

* <span data-ttu-id="3c5b0-3580">Suporte adicionado para a API versão de 30/11/2017</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3580">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="3c5b0-3581">Contêiner</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3581">Container</span></span>

* <span data-ttu-id="3c5b0-3582">Corrigida a regressão de portas padrão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3582">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="3c5b0-3583">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3583">Monitor</span></span>

* <span data-ttu-id="3c5b0-3584">Suporte de várias dimensões adicionado ao comando de métricas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3584">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="3c5b0-3585">Recurso</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3585">Resource</span></span>

* <span data-ttu-id="3c5b0-3586">Adicionado o argumento `--include-response-body` para `resource show`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3586">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="3c5b0-3587">Função</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3587">Role</span></span>

* <span data-ttu-id="3c5b0-3588">Exibição de atribuições padrão adicionada dos administradores "clássicos" para `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3588">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="3c5b0-3589">Suporte adicionado a `ad sp reset-credentials` para adicionar as credenciais em vez de substituir</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3589">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="3c5b0-3590">Relatório de erros aprimorado para `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3590">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="3c5b0-3591">SQL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3591">SQL</span></span>

* <span data-ttu-id="3c5b0-3592">Comandos `sql db list-usages` e `sql db show-usage` adicionados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3592">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="3c5b0-3593">Comandos `sql server conn-policy show` e `sql server conn-policy update` adicionados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3593">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="3c5b0-3594">VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3594">VM</span></span>

* <span data-ttu-id="3c5b0-3595">Informações da zona adicionadas a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3595">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="3c5b0-3596">14 de novembro de 2017</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3596">November 14, 2017</span></span>

<span data-ttu-id="3c5b0-3597">Versão 2.0.21</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3597">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-3598">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3598">ACR</span></span>

* <span data-ttu-id="3c5b0-3599">Suporte adicionado para criar webhooks em regiões de replicação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3599">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="3c5b0-3600">ACS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3600">ACS</span></span>

* <span data-ttu-id="3c5b0-3601">Alteradas todas as palavras "agente" para "nó" no AKS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3601">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="3c5b0-3602">Opção `--orchestrator-release` preterida para `acs create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3602">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="3c5b0-3603">Tamanho alterado da VM padrão do AKS para `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3603">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="3c5b0-3604">`az aks browse` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3604">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="3c5b0-3605">`az aks get-credentials` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3605">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-3606">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3606">Appservice</span></span>

* <span data-ttu-id="3c5b0-3607">Origem da implantação adicional `config-zip` para webapps e aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3607">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="3c5b0-3608">Opção `--docker-container-logging` adicionada a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3608">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="3c5b0-3609">Removida a opção `storage` do parâmetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3609">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="3c5b0-3610">Mensagens de erro aprimoradas para `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3610">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="3c5b0-3611">Suporte adicionado para criar aplicativos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3611">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="3c5b0-3612">`list-locations` fixo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3612">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="3c5b0-3613">Lote</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3613">Batch</span></span>

* <span data-ttu-id="3c5b0-3614">Bug corrigido no comando pool create quando uma ID do recurso foi usada com o sinalizador `--image`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3614">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="3c5b0-3615">Batchai</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3615">Batchai</span></span>

* <span data-ttu-id="3c5b0-3616">Opção curta adicionada `-s` para `--vm-size` ao fornecer o tamanho da VM no comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3616">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="3c5b0-3617">Nome da conta de armazenamento e argumentos-chave adicionados aos parâmetros `cluster create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3617">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="3c5b0-3618">Documentação corrigida para `job list-files` e `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3618">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="3c5b0-3619">Opção curta adicionada `-r` para `--cluster-name` ao fornecer o nome do cluster no comando `job create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3619">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="3c5b0-3620">Nuvem</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3620">Cloud</span></span>

* <span data-ttu-id="3c5b0-3621">`cloud [register|update]` alterado para evitar registrar nuvens sem os pontos de extremidade necessários</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3621">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="3c5b0-3622">Contêiner</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3622">Container</span></span>

* <span data-ttu-id="3c5b0-3623">Suporte adicionado para abrir várias portas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3623">Added support to open multiple ports</span></span>
* <span data-ttu-id="3c5b0-3624">Política de reinicialização do grupo de contêiner adicionada</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3624">Added container group restart policy</span></span>
* <span data-ttu-id="3c5b0-3625">Suporte adicionado para montar o compartilhamento de Arquivos do Azure como um volume</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3625">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="3c5b0-3626">Documentos de ajuda atualizados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3626">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="3c5b0-3627">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3627">Data Lake Analytics</span></span>

* <span data-ttu-id="3c5b0-3628">`[job|account] list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3628">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="3c5b0-3629">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3629">Data Lake Store</span></span>

* <span data-ttu-id="3c5b0-3630">`account list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3630">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="3c5b0-3631">Extensão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3631">Extension</span></span>

* <span data-ttu-id="3c5b0-3632">`extension list-available` adicionado para permitir a listagem de extensões oficiais da Microsoft</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3632">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="3c5b0-3633">`--name` adicionado a `extension [add|update]` para permitir a instalação de extensões por nome</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3633">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="3c5b0-3634">IoT</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3634">IoT</span></span>

* <span data-ttu-id="3c5b0-3635">Suporte adicionado para as autoridades de certificação (CA) e cadeias de certificado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3635">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="3c5b0-3636">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3636">Monitor</span></span>

* <span data-ttu-id="3c5b0-3637">Adicionados os comandos `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3637">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-3638">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3638">Network</span></span>

* <span data-ttu-id="3c5b0-3639">Suporte adicionado para registros DNS da CAA</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3639">Added support for CAA DNS records</span></span>
* <span data-ttu-id="3c5b0-3640">Problema corrigido onde os pontos de extremidade não podem ser atualizados com `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3640">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="3c5b0-3641">Problema corrigido onde `vnet update --dns-servers` não funcionou dependendo de como a VNET foi criada</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3641">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="3c5b0-3642">Problema corrigido onde os nomes DNS relativos foram importados incorretamente por`dns zone import`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3642">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="3c5b0-3643">Reservas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3643">Reservations</span></span>

* <span data-ttu-id="3c5b0-3644">Versão prévia inicial</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3644">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="3c5b0-3645">Recurso</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3645">Resource</span></span>

* <span data-ttu-id="3c5b0-3646">Suporte adicionado das IDs de recurso ao parâmetro `--resource` e bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3646">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="3c5b0-3647">SQL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3647">SQL</span></span>

* <span data-ttu-id="3c5b0-3648">Parâmetro `--ignore-missing-vnet-service-endpoint` adicionado a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3648">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-3649">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3649">Storage</span></span>

* <span data-ttu-id="3c5b0-3650">`storage account create` criado ao usar o SKU `Standard_RAGRS` como padrão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3650">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="3c5b0-3651">Bugs corrigidos ao lidar com nomes de arquivo/blob que incluem caracteres não ascii</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3651">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="3c5b0-3652">Bug corrigido que impedia usar `--source-uri` com `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3652">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="3c5b0-3653">Comandos adicionados para usar o glob e excluir vários objetos com `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3653">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="3c5b0-3654">Problema corrigido ao habilitar métricas com `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3654">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="3c5b0-3655">Problema corrigido com arquivos acima de 200 GB ao usar `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3655">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="3c5b0-3656">Problema corrigido onde `--bypass` e `--default-action` foram ignorados por `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3656">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="3c5b0-3657">VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3657">VM</span></span>

* <span data-ttu-id="3c5b0-3658">Bug corrigido com `vmss create`, que impediu o uso da camada de tamanho `Basic`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3658">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="3c5b0-3659">Argumentos `--plan` adicionados a `[vm|vmss] create` para ter imagens personalizadas com informações de cobrança</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3659">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="3c5b0-3660">Comandos `vm secret `[add|remove|list]\` adicionados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3660">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="3c5b0-3661">`vm format-secret` renomeado para `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3661">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="3c5b0-3662">Adicionado o argumento `--encrypt format` para `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3662">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="3c5b0-3663">24 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3663">October 24, 2017</span></span>

<span data-ttu-id="3c5b0-3664">Versão 2.0.20</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3664">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="3c5b0-3665">Núcleo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3665">Core</span></span>

* <span data-ttu-id="3c5b0-3666">Atualizado `2017-03-09-profile` para usar a `MGMT_STORAGE` versão da API`2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3666">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-3667">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3667">ACR</span></span>

* <span data-ttu-id="3c5b0-3668">Gerenciamento de recursos atualizado para apontar para a versão da API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3668">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="3c5b0-3669">SKU 'traga seu próprio armazenamento' alterada para Clássico</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3669">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="3c5b0-3670">SKUs de registro renomeados como Básico, Standard e Premium</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3670">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="3c5b0-3671">ACS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3671">ACS</span></span>

* <span data-ttu-id="3c5b0-3672">[VERSÃO PRÉVIA] Comandos `az aks` adicionados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3672">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="3c5b0-3673">Kubernetes `get-credentials` corrigido</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3673">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-3674">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3674">Appservice</span></span>

* <span data-ttu-id="3c5b0-3675">Problema corrigido onde os logs `webapp` baixados podem ser inválidos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3675">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="3c5b0-3676">Componente</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3676">Component</span></span>

* <span data-ttu-id="3c5b0-3677">Mensagem de reprovação mais clara adicionada para todos os instaladores e prompt de confirmação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3677">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="3c5b0-3678">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3678">Monitor</span></span>

* <span data-ttu-id="3c5b0-3679">Adicionados os comandos `action-group`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3679">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="3c5b0-3680">Recurso</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3680">Resource</span></span>

* <span data-ttu-id="3c5b0-3681">Incompatibilidade corrigida com a versão mais recente de dependência msrest em `group export`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3681">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="3c5b0-3682">`policy assignment create` corrigido para trabalhar com as definições de política internas e as definições do conjunto de políticas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3682">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="3c5b0-3683">VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3683">VM</span></span>

* <span data-ttu-id="3c5b0-3684">Adicionado o argumento `--accelerated-networking` para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3684">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="3c5b0-3685">9 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3685">October 9, 2017</span></span>

<span data-ttu-id="3c5b0-3686">Versão 2.0.19</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3686">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="3c5b0-3687">Núcleo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3687">Core</span></span>

* <span data-ttu-id="3c5b0-3688">Tratamento de URLs de autoridade do AD FS adicionado com uma barra à direita para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3688">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-3689">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3689">Appservice</span></span>

* <span data-ttu-id="3c5b0-3690">Atualização genérica adicionada com o novo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3690">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="3c5b0-3691">Lote</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3691">Batch</span></span>

* <span data-ttu-id="3c5b0-3692">Atualizado para o SDK do Lote 4.0.0</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3692">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="3c5b0-3693">A opção `--image` de VirtualMachineConfiguration foi atualizada para dar suporte a referências de imagem ARM além de publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3693">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="3c5b0-3694">Suporte adicionado para o novo modelo de extensão da CLI para comandos de Extensões de Lote</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3694">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="3c5b0-3695">Removeu o suporte de Lote do modelo de componente</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3695">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="3c5b0-3696">Batchai</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3696">Batchai</span></span>

* <span data-ttu-id="3c5b0-3697">Versão inicial do módulo de IA de Lote</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3697">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="3c5b0-3698">Keyvault</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3698">Keyvault</span></span>

* <span data-ttu-id="3c5b0-3699">Correção do problema de autenticação do Cofre de Chaves ao usar o AD FS no Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3699">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="3c5b0-3700">(#4448)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3700">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="3c5b0-3701">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3701">Network</span></span>

* <span data-ttu-id="3c5b0-3702">Alterado `--server` argumento de `application-gateway address-pool create` para ser opcional, permitindo pools de endereços vazios</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3702">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="3c5b0-3703">`traffic-manager` foi atualizado para oferecer suporte aos recursos mais recentes</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3703">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="3c5b0-3704">Recurso</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3704">Resource</span></span>

* <span data-ttu-id="3c5b0-3705">Suporte adicionado para `--resource-group/-g` opções do nome do grupo de recursos para `group`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3705">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="3c5b0-3706">Comandos adicionados a `account lock` para funcionar com bloqueios no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3706">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="3c5b0-3707">Comandos adicionados a `group lock` para funcionar com bloqueios no nível do grupo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3707">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="3c5b0-3708">Comandos adicionados a `resource lock` para funcionar com bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3708">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="3c5b0-3709">Sql</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3709">Sql</span></span>

* <span data-ttu-id="3c5b0-3710">Suporte adicionado para SQL TDE (Transparent Data Encryption) e TDE com Traga sua própria chave</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3710">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="3c5b0-3711">Comando `db list-deleted` e parâmetro `db restore --deleted-time` adicionados, permitindo localizar e restaurar bancos de dados excluídos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3711">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="3c5b0-3712">`db op list` e `db op cancel` adicionados, permitindo listar e cancelar operações em andamento no banco de dados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3712">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-3713">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3713">Storage</span></span>

* <span data-ttu-id="3c5b0-3714">Suporte adicionado para instantâneo de compartilhamento de arquivos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3714">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="3c5b0-3715">VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3715">Vm</span></span>

* <span data-ttu-id="3c5b0-3716">Correção de um bug em `vm show` onde o uso de `-d` causou uma falha nos endereços IP privados ausentes</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3716">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="3c5b0-3717">[VERSÃO PRÉVIA] Suporte adicionado para atualização sem interrupção para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3717">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="3c5b0-3718">Suporte adicionado para atualizar as configurações de criptografia com `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3718">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="3c5b0-3719">Parâmetro `--os-disk-size-gb` adicionado a `vm create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3719">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="3c5b0-3720">Parâmetro `--license-type` adicionado ao Windows para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3720">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="3c5b0-3721">22 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3721">September 22, 2017</span></span>

<span data-ttu-id="3c5b0-3722">Versão 2.0.1.8</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3722">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="3c5b0-3723">Recurso</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3723">Resource</span></span>

* <span data-ttu-id="3c5b0-3724">Suporte adicionado para mostrar as definições de políticas internas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3724">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="3c5b0-3725">Parâmetro de modo de suporte adicionado para a criação de definições de política</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3725">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="3c5b0-3726">Suporte adicionado para definições de interface do usuário e modelos em `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3726">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="3c5b0-3727">[ALTERAÇÃO SIGNIFICATIVA] Tipo de recurso `managedapp` alterado de `appliances` para `applications` e de `applianceDefinitions` para `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3727">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-3728">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3728">Network</span></span>

* <span data-ttu-id="3c5b0-3729">Suporte adicionado para a zona de disponibilidade para os subcomandos `network lb` e `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3729">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="3c5b0-3730">Suporte adicionado ao Emparelhamento IPv6 da Microsoft para `express-route`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3730">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="3c5b0-3731">Adicionados `asg` comandos de grupo de segurança do aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3731">Added `asg` application security group commands</span></span>
* <span data-ttu-id="3c5b0-3732">Adicionado o argumento `--application-security-groups` para `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3732">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="3c5b0-3733">Adicionados os argumentos `--source-asgs` e `--destination-asgs` para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3733">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="3c5b0-3734">Adicionados os argumentos `--ddos-protection` e `--vm-protection` para `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3734">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="3c5b0-3735">Adicionados os comandos `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3735">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-3736">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3736">Storage</span></span>

* <span data-ttu-id="3c5b0-3737">Correção do problema onde `storage account network-rule` comandos poderão falhar após a atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3737">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="3c5b0-3738">Grade de eventos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3738">Eventgrid</span></span>

* <span data-ttu-id="3c5b0-3739">Atualizada SDK Python da Grade de Eventos do Azure para usar a versão de API mais recente "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3739">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="3c5b0-3740">SQL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3740">SQL</span></span>

* <span data-ttu-id="3c5b0-3741">Alterado o `sql server list` argumento `--resource-group` para ser opcional.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3741">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="3c5b0-3742">Se não for especificado, todos os servidores sql na assinatura serão retornados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3742">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="3c5b0-3743">Adicionado o `--no-wait` parâmetro para `db [create|copy|restore|update|replica create|create|update]` e `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3743">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="3c5b0-3744">Keyvault</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3744">Keyvault</span></span>

* <span data-ttu-id="3c5b0-3745">Adicionado suporte para comandos Keyvault por trás de um proxy</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3745">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="3c5b0-3746">VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3746">VM</span></span>

* <span data-ttu-id="3c5b0-3747">Adicionado suporte à zona de disponibilidade para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3747">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="3c5b0-3748">Correção do problema onde usar`--app-gateway ID` com `vmss create` poderia causar uma falha</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3748">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="3c5b0-3749">Adicionado o argumento `--asgs` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3749">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="3c5b0-3750">Suporte adicionado para executar comandos em VMs com `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3750">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="3c5b0-3751">[VERSÃO PRÉVIA] Adicionado suporte para criptografia de disco VMSS com `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3751">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="3c5b0-3752">Suporte adicionado para realizar a manutenção em VMs com `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3752">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="3c5b0-3753">ACS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3753">ACS</span></span>

* <span data-ttu-id="3c5b0-3754">[VERSÃO PRÉVIA] Adicionado `--orchestrator-release` argumento para `acs create` para regiões de versão prévia do ACS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3754">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-3755">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3755">Appservice</span></span>

* <span data-ttu-id="3c5b0-3756">Adicionada a capacidade para atualizar e mostrar as configurações de autenticação com `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3756">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="3c5b0-3757">Backup</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3757">Backup</span></span>

* <span data-ttu-id="3c5b0-3758">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3758">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="3c5b0-3759">11 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3759">September 11, 2017</span></span>

<span data-ttu-id="3c5b0-3760">Versão 2.0.17</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3760">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="3c5b0-3761">Núcleo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3761">Core</span></span>

* <span data-ttu-id="3c5b0-3762">Módulo de comando habilitado para definir sua própria ID de correlação na telemetria</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3762">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="3c5b0-3763">Problema de despejo de JSON corrigido quando a telemetria é definida como modo de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3763">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="3c5b0-3764">Acs</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3764">Acs</span></span>

* <span data-ttu-id="3c5b0-3765">Adicionado o comando `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3765">Added `acs list-locations` command</span></span>
* <span data-ttu-id="3c5b0-3766">Fez `ssh-key-file` vir com o valor padrão esperado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3766">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-3767">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3767">Appservice</span></span>

* <span data-ttu-id="3c5b0-3768">Foi incluída a capacidade de criar um aplicativo Web em um grupo de recursos que não seja o plano de serviço ativo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3768">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="3c5b0-3769">CDN</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3769">CDN</span></span>

* <span data-ttu-id="3c5b0-3770">Foi corrigido o bug 'Não é possível interar CustomDomain' para `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3770">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="3c5b0-3771">Extensão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3771">Extension</span></span>

* <span data-ttu-id="3c5b0-3772">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3772">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="3c5b0-3773">Keyvault</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3773">Keyvault</span></span>

* <span data-ttu-id="3c5b0-3774">Foi corrigido o problema onde permissões diferenciavam maiúsculas de minúsculas para `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3774">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-3775">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3775">Network</span></span>

* <span data-ttu-id="3c5b0-3776">`vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3776">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="3c5b0-3777">Foi renomeado o argumento `--private-access-services` para `--service-endpoints` para `vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3777">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="3c5b0-3778">Foi adicionado suporte a vários intervalos de IP e intervalos de portas para `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3778">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="3c5b0-3779">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3779">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="3c5b0-3780">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3780">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="3c5b0-3781">Recurso</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3781">Resource</span></span>

* <span data-ttu-id="3c5b0-3782">Permitir a passagem de definições de parâmetro de políticas de recursos em `policy definition create` e`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3782">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="3c5b0-3783">Permitir a passagem de valores de parâmetro para`policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3783">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="3c5b0-3784">Permitir a passagem de JSON ou arquivo para todos os parâmetros</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3784">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="3c5b0-3785">Versão da API incrementada</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3785">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="3c5b0-3786">SQL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3786">SQL</span></span>

* <span data-ttu-id="3c5b0-3787">Adicionados os comandos `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3787">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="3c5b0-3788">VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3788">VM</span></span>

* <span data-ttu-id="3c5b0-3789">Corrigido: não atribuir acesso, a menos que `--scope` seja fornecido</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3789">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="3c5b0-3790">Corrigido: usar a mesma nomenclatura de extensão do que o portal</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3790">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="3c5b0-3791">Foi removido `subscription` da saída de `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3791">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="3c5b0-3792">Corrigido: SKU de armazenamento do `[vm|vmss] create` não é aplicada em discos de dados com uma imagem</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3792">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="3c5b0-3793">Corrigido: `vm format-secret --secrets` não aceita IDs de separados de nova linha</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3793">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="3c5b0-3794">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3794">August 31, 2017</span></span>

<span data-ttu-id="3c5b0-3795">Versão 2.0.16</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3795">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="3c5b0-3796">Keyvault</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3796">Keyvault</span></span>

* <span data-ttu-id="3c5b0-3797">Correção do bug ao tentar resolver automaticamente a codificação secreta com `secret download`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3797">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="3c5b0-3798">Sf</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3798">Sf</span></span>

* <span data-ttu-id="3c5b0-3799">Substituição de todos os comandos em favor da CLI do Service Fabric (sfctl)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3799">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-3800">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3800">Storage</span></span>

* <span data-ttu-id="3c5b0-3801">Correção de problema onde as contas de armazenamento não conseguiam ser criadas em regiões sem suporte ao recurso NetworkACLs</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3801">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="3c5b0-3802">Determinar o tipo de conteúdo e a codificação do conteúdo durante o upload de arquivo e de blob se nem o tipo de conteúdo nem a codificação de conteúdo forem especificados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3802">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="3c5b0-3803">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3803">August 28, 2017</span></span>

<span data-ttu-id="3c5b0-3804">Versão 2.0.15</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3804">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="3c5b0-3805">CLI</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3805">CLI</span></span>

* <span data-ttu-id="3c5b0-3806">Nota legal adicionada ao `--version`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3806">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="3c5b0-3807">ACS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3807">ACS</span></span>

* <span data-ttu-id="3c5b0-3808">Corrigidas as regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3808">Corrected preview regions</span></span>
* <span data-ttu-id="3c5b0-3809">Corrigida a formatação padrão de `dns_name_prefix`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3809">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="3c5b0-3810">Saída de comando ACS otimizada</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3810">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-3811">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3811">Appservice</span></span>

* <span data-ttu-id="3c5b0-3812">[ALTERAÇÃO SIGNIFICATIVA] Corrigidas as inconsistências na saída de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3812">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="3c5b0-3813">Adicionado um novo alias de `-i` para `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3813">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="3c5b0-3814">Exposto `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3814">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="3c5b0-3815">Expostos novos argumentos de `az webapp delete` para manter o plano, as métricas ou o registro de DNS do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3815">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="3c5b0-3816">Corrigido: detectar as configurações de slot corretamente</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3816">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="3c5b0-3817">IoT</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3817">IoT</span></span>

* <span data-ttu-id="3c5b0-3818">Corrigido #3934: a criação de uma política não limpa mais as políticas existentes</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3818">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-3819">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3819">Network</span></span>

* <span data-ttu-id="3c5b0-3820">[ALTERAÇÃO SIGNIFICATIVA]`vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3820">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="3c5b0-3821">[ALTERAÇÃO SIGNIFICATIVA] Opção `--private-access-services` renomeada como `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3821">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="3c5b0-3822">Adicionado suporte para vários  intervalos de IP e portas para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3822">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="3c5b0-3823">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3823">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="3c5b0-3824">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3824">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="3c5b0-3825">Perfil</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3825">Profile</span></span>

* <span data-ttu-id="3c5b0-3826">`--msi` e `--msi-port` expostos a logon usando a identidade de uma máquina virtual</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3826">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="3c5b0-3827">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3827">Service Fabric</span></span>

* <span data-ttu-id="3c5b0-3828">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3828">Preview release</span></span>
* <span data-ttu-id="3c5b0-3829">Simplificadas as regras de registro de usuário/senha para comando</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3829">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="3c5b0-3830">Corrigido o prompt de senha para o usuário mesmo após a passagem do parâmetro</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3830">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="3c5b0-3831">Adicionado suporte para `registry_cred` vazio</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3831">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-3832">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3832">Storage</span></span>

* <span data-ttu-id="3c5b0-3833">Habilitada a camada de blob de configuração</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3833">Enabled setting blob tier</span></span>
* <span data-ttu-id="3c5b0-3834">Adicionados os argumentos `--bypass` e `--default-action` ao `storage account [create|update]` para dar suporte ao serviço de túnel</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3834">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="3c5b0-3835">Comandos adicionados ao `storage account network-rule` para adicionar as regras de rede virtual e regras baseadas em IP</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3835">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="3c5b0-3836">Habilitada a criptografia de serviço por chave gerenciada de cliente</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3836">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="3c5b0-3837">[ALTERAÇÃO SIGNIFICATIVA] Opção `--encryption` renomeada como `--encryption-services` para o comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3837">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="3c5b0-3838">Correção #4220: `az storage account update encryption` - incompatibilidade de sintaxe</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3838">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="3c5b0-3839">VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3839">VM</span></span>

* <span data-ttu-id="3c5b0-3840">Corrigido o problema em que informações incorretas extras eram exibidas para `vmss get-instance-view` ao usar `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3840">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="3c5b0-3841">Adicionado suporte ao `--lb-sku` para `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3841">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="3c5b0-3842">Removidos nomes humanos da lista de bloqueio de nome de administrador para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3842">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="3c5b0-3843">Corrigido o problema onde `[vm|vmss] create` geraria um erro se não for possível extrair informações do plano de uma imagem</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3843">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="3c5b0-3844">Corrigida uma falha ao criar um conjunto de dimensionamento de máquinas virtuais com um balanceamento de carga interno</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3844">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="3c5b0-3845">Corrigido o problema onde o argumento `--no-wait` não funcionava com `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3845">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="3c5b0-3846">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3846">August 15, 2017</span></span>

<span data-ttu-id="3c5b0-3847">Versão 2.0.14</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3847">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="3c5b0-3848">ACS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3848">ACS</span></span>

* <span data-ttu-id="3c5b0-3849">Corrigido o número da porta SSH Master0 para kubernetes</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3849">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-3850">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3850">Appservice</span></span>

* <span data-ttu-id="3c5b0-3851">Corrigida uma exceção ao criar um novo GIT com base no aplicativo Web Linux</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3851">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="3c5b0-3852">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3852">Event Grid</span></span>

* <span data-ttu-id="3c5b0-3853">Adicionadas dependências SDK</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3853">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="3c5b0-3854">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3854">August 11, 2017</span></span>

<span data-ttu-id="3c5b0-3855">Versão 2.0.13</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3855">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="3c5b0-3856">ACS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3856">ACS</span></span>

* <span data-ttu-id="3c5b0-3857">Adicionadas mais regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3857">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="3c5b0-3858">Lote</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3858">Batch</span></span>

* <span data-ttu-id="3c5b0-3859">Atualizado para o Lote SDK 3.1.0 e Gerenciamento de Lote SDK 4.1.0</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3859">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="3c5b0-3860">Adicionado um novo comando que mostra as contagens de tarefas de um trabalho</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3860">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="3c5b0-3861">Corrigido o bug no processamento de URL de SAS do arquivo de recurso</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3861">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="3c5b0-3862">Ponto de extremidade da conta de lote agora dá suporte ao prefixo opcional “https://”</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3862">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="3c5b0-3863">Suporte para adicionar listas de mais de 100 tarefas a um trabalho</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3863">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="3c5b0-3864">Adicionado log de depuração para carregar o módulo do comando de Extensões</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3864">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="3c5b0-3865">Componente</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3865">Component</span></span>

* <span data-ttu-id="3c5b0-3866">Aviso de substituição adicionado aos comandos 'az component'</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3866">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="3c5b0-3867">Contêiner</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3867">Container</span></span>

* <span data-ttu-id="3c5b0-3868">`create`: corrigido o problema em que o sinal de igual não era permitido dentro de uma variável de ambiente</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3868">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="3c5b0-3869">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3869">Data Lake Store</span></span>

* <span data-ttu-id="3c5b0-3870">Habilitado o controle do andamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3870">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="3c5b0-3871">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3871">Event Grid</span></span>

* <span data-ttu-id="3c5b0-3872">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3872">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-3873">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3873">Network</span></span>

* <span data-ttu-id="3c5b0-3874">`lb`: corrigido o problema em que os nomes de recursos filhos específicos não eram resolvidos corretamente quando omitidos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3874">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="3c5b0-3875">`application-gateway {subresource} delete`: corrigido o problema em que `--no-wait` não foi liquidado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3875">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="3c5b0-3876">`application-gateway http-settings update`: corrigido o problema em que `--connection-draining-timeout` não podia ser desativado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3876">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="3c5b0-3877">Corrigido o erro de argumento de palavra-chave inesperado `sa_data_size_kilobyes` com `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3877">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="3c5b0-3878">Perfil</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3878">Profile</span></span>

* <span data-ttu-id="3c5b0-3879">`account list`: adicionado `--refresh` para sincronizar as assinaturas mais recentes do servidor</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3879">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-3880">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3880">Storage</span></span>

* <span data-ttu-id="3c5b0-3881">Habilitar atualização de conta de armazenamento com a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3881">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="3c5b0-3882">VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3882">VM</span></span>

* <span data-ttu-id="3c5b0-3883">`availability-set`: exposta a contagem de domínios de falha durante a conversão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3883">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="3c5b0-3884">Exposto o comando `list-skus`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3884">Exposed `list-skus` command</span></span>
* <span data-ttu-id="3c5b0-3885">Suporte para atribuir identidade sem criar atribuições de função</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3885">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="3c5b0-3886">Aplicar o SKU de armazenamento ao anexar discos de dados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3886">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="3c5b0-3887">Removido o nome do disco do sistema operacional padrão e SKU de armazenamento ao usar discos gerenciados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3887">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="3c5b0-3888">28 de julho de 2017</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3888">July 28, 2017</span></span>

<span data-ttu-id="3c5b0-3889">Versão 2.0.12</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3889">Version 2.0.12</span></span>

* <span data-ttu-id="3c5b0-3890">Adicionado os comandos de contêiner</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3890">Added container commands</span></span>
* <span data-ttu-id="3c5b0-3891">Adicionados módulos de cobrança e de consumo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3891">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="3c5b0-3892">Núcleo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3892">Core</span></span>

* <span data-ttu-id="3c5b0-3893">Informações de autenticação de SDK de saída para entidades de serviço com certificados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3893">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="3c5b0-3894">Corrigidas as exceções de andamento da implantação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3894">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="3c5b0-3895">Usar o ponto de extremidade do ARM da nuvem atual para criar cliente da assinatura</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3895">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="3c5b0-3896">Melhor manipulação simultânea do arquivo clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3896">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="3c5b0-3897">Atualização da ID de solicitação do cliente para cada execução de comando</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3897">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="3c5b0-3898">Criar clientes de assinatura com o perfil correto do SDK (#3635)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3898">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="3c5b0-3899">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3899">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="3c5b0-3900">Adicionado suporte para escolher campos de saída da tabela através da consulta JMESpath (#3581)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3900">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="3c5b0-3901">Aprimoramento da desativação de áudio de argumentos de análise e da adição do histórico com gestos (#3434)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3901">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="3c5b0-3902">Criar clientes de assinatura com o perfil correto do SDK</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3902">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="3c5b0-3903">Mover todos os arquivos existentes de gravação para a pasta mais recente</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3903">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="3c5b0-3904">Corrigida a idempotência para a criação de VM/VMSS (#3586)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3904">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="3c5b0-3905">Os caminhos de comando não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3905">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="3c5b0-3906">Determinados parâmetros do tipo booliano não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3906">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="3c5b0-3907">Suporte para logon do ADFS em um servidor local como o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3907">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="3c5b0-3908">Corrigidas as gravações simultâneas para clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3908">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="3c5b0-3909">ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3909">ACR</span></span>

* <span data-ttu-id="3c5b0-3910">Adicionado o comando `show-usage` para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3910">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="3c5b0-3911">Suporte para atualização do SKU para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3911">Support SKU update for managed registries</span></span>
* <span data-ttu-id="3c5b0-3912">Adicionados registros gerenciados com o SKU gerenciado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3912">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="3c5b0-3913">Adicionados webhooks para registros gerenciados com o módulo de comando de webhook do ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3913">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="3c5b0-3914">Adicionada autenticação do AAD com o comando de logon de ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3914">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="3c5b0-3915">Adicionado comando de exclusão para marcas, manifestos e repositórios do Docker</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3915">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="3c5b0-3916">ACS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3916">ACS</span></span>

* <span data-ttu-id="3c5b0-3917">Suporte para a API versão 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3917">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-3918">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3918">Appservice</span></span>

* <span data-ttu-id="3c5b0-3919">Corrigido o bug onde listar o aplicativo Web Linux não retornava nada</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3919">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="3c5b0-3920">Suporte para recuperar credenciais de ACR</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3920">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="3c5b0-3921">Remover todos os comandos em `appservice web`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3921">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="3c5b0-3922">Ocultar as senhas de registro do Docker da saída do comando (#3656)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3922">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="3c5b0-3923">Verifique se o navegador padrão é usado no macOS sem erros (#3623)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3923">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="3c5b0-3924">Aprimorada a Ajuda de `webapp log tail` e `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3924">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="3c5b0-3925">Exposto o comando `traffic-routing` para configurar roteamento estático (#3566)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3925">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="3c5b0-3926">Adicionadas correções de confiabilidade na configuração de controle do código-fonte (#3245)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3926">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="3c5b0-3927">Removido o argumento `--node-version` sem suporte de `webapp config update` para aplicativos Web do Windows.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3927">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="3c5b0-3928">Em vez disso, use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3928">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="3c5b0-3929">Lote</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3929">Batch</span></span>

* <span data-ttu-id="3c5b0-3930">Atualizado para o Lote SDK 3.0.0 com suporte para VMs de baixa prioridade em pools</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3930">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="3c5b0-3931">Opção `pool create` renomeada como `--target-dedicated` para `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3931">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="3c5b0-3932">Adicionadas as opções `pool create` e `--target-low-priority-nodes` de `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3932">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="3c5b0-3933">CDN</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3933">CDN</span></span>

* <span data-ttu-id="3c5b0-3934">Uma mensagem de erro mais adequada foi fornecida para `cdn endpoint list` quando o perfil especificado por `--profile-name` não existir</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3934">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="3c5b0-3935">Nuvem</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3935">Cloud</span></span>

* <span data-ttu-id="3c5b0-3936">Alterada a versão de API do ponto de extremidade de metadados de nuvem para o formato AAAA-MM-DD</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3936">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="3c5b0-3937">Ponto de extremidade da galeria não é necessário</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3937">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="3c5b0-3938">Suporte para registrar a nuvem somente com o ponto de extremidade de gerenciador de recursos do ARM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3938">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="3c5b0-3939">Fornecida uma opção para `cloud set` para escolher o perfil ao selecionar a nuvem atual</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3939">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="3c5b0-3940">Exposto `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3940">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="3c5b0-3941">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3941">CosmosDB</span></span>

* <span data-ttu-id="3c5b0-3942">Corrigida a permissão para criação de coleção com chave de partição personalizada</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3942">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="3c5b0-3943">Adicionado suporte para o TTL padrão de coleção</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3943">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="3c5b0-3944">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3944">Data Lake Analytics</span></span>

* <span data-ttu-id="3c5b0-3945">Adicionados comandos para gerenciamento de política de computação sob o título `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3945">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="3c5b0-3946">Adicionado `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3946">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="3c5b0-3947">Adicionado `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3947">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="3c5b0-3948">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3948">Data Lake Store</span></span>

* <span data-ttu-id="3c5b0-3949">Adicionado suporte para a rotação de chave de cofre de chaves gerenciado do usuário em `dls account update`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3949">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="3c5b0-3950">Atualizada a versão SDK do sistema de arquivos do Data Lake Store subjacente para resolver um problema de desempenho</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3950">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="3c5b0-3951">Adicionado o comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3951">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="3c5b0-3952">Esse comando tenta permitir que um Cofre de Chaves fornecido pelo usuário use a criptografia de dados em uma conta do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3952">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="3c5b0-3953">Interativo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3953">Interactive</span></span>

* <span data-ttu-id="3c5b0-3954">Melhor tempo de inicialização, usando comandos em cache</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3954">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="3c5b0-3955">Maior cobertura de teste</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3955">Increased test coverage</span></span>
* <span data-ttu-id="3c5b0-3956">Aprimorado o gesto “?” para injetar também o próximo comando</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3956">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="3c5b0-3957">Corrigidos os erros interativos com o perfil 2017-03-09-profile-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3957">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="3c5b0-3958">Permitido `--version` como um parâmetro para o modo interativo (#3645)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3958">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="3c5b0-3959">Impedir que o modo interativo gere erros de conclusões de validação (#3570)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3959">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="3c5b0-3960">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3960">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="3c5b0-3961">Adicionado o sinalizador `--progress`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3961">Added `--progress` flag</span></span>
* <span data-ttu-id="3c5b0-3962">Removidos `--debug` e `--verbose` de conclusões</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3962">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="3c5b0-3963">Removido `interactive` de conclusões (#3324)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3963">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="3c5b0-3964">IoT</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3964">IoT</span></span>

* <span data-ttu-id="3c5b0-3965">A criação de uma política não limpa as políticas existentes.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3965">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="3c5b0-3966">(#3934)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3966">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="3c5b0-3967">Cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3967">Key vault</span></span>

* <span data-ttu-id="3c5b0-3968">Comandos adicionados para recursos de recuperação do cofre de chaves:</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3968">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="3c5b0-3969">Subcomandos `purge`, `recover`, `keyvault list-deleted` de `keyvault`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3969">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="3c5b0-3970">Subcomandos `backup`, `restore`, `purge`, `recover`, `list-deleted` de `keyvault secret`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3970">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="3c5b0-3971">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault certificate`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3971">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="3c5b0-3972">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault key`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3972">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="3c5b0-3973">Adicionada a integração do cofre de chaves da entidade de serviço (#3133)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3973">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="3c5b0-3974">Atualizado o plano de dados de cofre de chaves para 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3974">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="3c5b0-3975">(#3307)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3975">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="3c5b0-3976">Laboratório</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3976">Lab</span></span>

* <span data-ttu-id="3c5b0-3977">Adicionado o suporte para reivindicar qualquer VM no laboratório através de `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3977">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="3c5b0-3978">Adicionado o formatador de saída da tabela para `az lab vm list` e `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3978">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="3c5b0-3979">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3979">Monitor</span></span>

* <span data-ttu-id="3c5b0-3980">Correção para o arquivo de modelo com o comando `monitor autoscale-settings get-parameters-template` (#3349)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3980">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="3c5b0-3981">`monitor alert-rule-incidents list` renomeado para `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3981">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="3c5b0-3982">`monitor alert-rule-incidents show` renomeado para `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3982">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="3c5b0-3983">`monitor metric-defintions list` renomeado para `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3983">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="3c5b0-3984">`monitor alert-rules` renomeado para `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3984">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="3c5b0-3985">Alterado `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3985">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="3c5b0-3986">Os subcomandos `condition` e `action` não aceitarão mais JSON</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3986">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="3c5b0-3987">Adicionar vários parâmetros para simplificar o processo de criação de regra</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3987">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="3c5b0-3988">`location` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3988">`location` no longer required</span></span>
  * <span data-ttu-id="3c5b0-3989">Adicionar nome e o suporte a ID de destino</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3989">Add name and ID support for target</span></span>
  * <span data-ttu-id="3c5b0-3990">Remover `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3990">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="3c5b0-3991">Renomear `is-enabled` para `enabled` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3991">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="3c5b0-3992">Padrões de `description` agora baseados na condição fornecida</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3992">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="3c5b0-3993">Adicionar exemplos para ajudar a esclarecer o novo formato</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3993">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="3c5b0-3994">Suporte para nomes ou IDs para comandos `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3994">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="3c5b0-3995">Exemplos e argumentos de conveniência adicionados ao `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3995">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-3996">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3996">Network</span></span>

* <span data-ttu-id="3c5b0-3997">Adicionado o comando `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3997">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="3c5b0-3998">Adicionado argumento `--private-access-services` para `vnet subnet create` e `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3998">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="3c5b0-3999">Corrigido o problema onde `application-gateway redirect-config create` falhava</span><span class="sxs-lookup"><span data-stu-id="3c5b0-3999">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="3c5b0-4000">Corrigido o problema onde `application-gateway redirect-config update` com `--no-wait` não funcionava</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4000">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="3c5b0-4001">Corrigido o bug ao usar o argumento `--servers` com `application-gateway address-pool create` e `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4001">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="3c5b0-4002">Adicionados os comandos `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4002">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="3c5b0-4003">Adicionados os comandos para `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4003">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="3c5b0-4004">Adicionados os argumentos para `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4004">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="3c5b0-4005">Adicionados os argumentos para `application-gateway http-settings create` e `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4005">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="3c5b0-4006">Adicionados os argumentos para `application-gateway url-path-map create` e `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4006">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="3c5b0-4007">Adicionado o argumento `--redirect-config` para `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4007">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="3c5b0-4008">Adicionado o suporte ao `--no-wait` para `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4008">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="3c5b0-4009">Adicionados os argumentos para `application-gateway probe create` e `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4009">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="3c5b0-4010">Adicionado o argumento `--redirect-config` para `application-gateway rule create` e `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4010">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="3c5b0-4011">Adicionado o suporte ao `--accelerated-networking` para `nic create` e `nic update`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4011">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="3c5b0-4012">Removido o argumento `--internal-dns-name-suffix` de `nic create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4012">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="3c5b0-4013">Adicionado o suporte ao `--dns-servers` para `nic update` e `nic create`: Adicionar suporte para --dns-servers</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4013">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="3c5b0-4014">Corrigido o bug onde `local-gateway create` ignorava `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4014">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="3c5b0-4015">Adicionado o suporte ao `--dns-servers` para `vnet update`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4015">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="3c5b0-4016">Corrigido o bug ao criar um emparelhamento sem filtragem de rotas com `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4016">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="3c5b0-4017">Corrigido o bug onde os argumentos `--provider` e `--bandwidth` não funcionavam com `express-route update`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4017">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="3c5b0-4018">Corrigido o bug com a lógica padrão de `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4018">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="3c5b0-4019">Aprimorada a formatação de saída para `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4019">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="3c5b0-4020">Usar IP de front-end padrão para `application-gateway http-listener create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4020">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="3c5b0-4021">Usar o pool padrão de endereços, configurações de HTTP e o ouvinte HTTP para `application-gateway rule create`, se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4021">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="3c5b0-4022">Usar IP de front-end e pool de back-end padrão para `lb rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4022">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="3c5b0-4023">Usar IP de front-end padrão para `lb inbound-nat-rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4023">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="3c5b0-4024">Perfil</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4024">Profile</span></span>

* <span data-ttu-id="3c5b0-4025">Suporte a logon em uma VM com uma identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4025">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="3c5b0-4026">Suporte a saída para `account show` em formato de arquivo de autenticação do SDK</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4026">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="3c5b0-4027">Mostrar avisos de código obsoleto ao usar o “modo de exibição expandido”</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4027">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="3c5b0-4028">Adicionado o comando `get-access-token` para fornecer o token bruto do AAD</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4028">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="3c5b0-4029">Suporte a logon com uma conta de usuário sem nenhuma assinatura associada</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4029">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="3c5b0-4030">RDBMS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4030">RDBMS</span></span>

* <span data-ttu-id="3c5b0-4031">Suporte para listar servidores em uma assinatura (#3417)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4031">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="3c5b0-4032">Corrigido o `%s` não processado devido à ausência de `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4032">Fixed `%s` not processed because of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="3c5b0-4033">Corrigido o mapa do código-fonte do documento e adicionada a tarefa CI para verificação (#3361)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4033">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="3c5b0-4034">Corrigida a ajuda de MySQL e PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4034">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="3c5b0-4035">Recurso</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4035">Resource</span></span>

* <span data-ttu-id="3c5b0-4036">Aprimorados os prompts para parâmetros ausentes para `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4036">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="3c5b0-4037">Aprimorada a análise da sintaxe `--parameters KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4037">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="3c5b0-4038">Corrigidos os problemas onde os arquivos de parâmetros `group deployment create` não eram mais reconhecidos usando a sintaxe `@<file>`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4038">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="3c5b0-4039">Suporte do argumento `--ids` para os comandos `resource` e `managedapp`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4039">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="3c5b0-4040">Corrigidas algumas mensagens de erro e análise (#3584)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4040">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="3c5b0-4041">Corrigida a análise de `--resource-type` para o comando `lock` aceitar `<resource-namespace>` e `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4041">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="3c5b0-4042">Adicionados parâmetros de verificação para modelos de link do modelo (#3629)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4042">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="3c5b0-4043">Adicionado suporte para especificar parâmetros de implantação usando a sintaxe `KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4043">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="3c5b0-4044">Função</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4044">Role</span></span>

* <span data-ttu-id="3c5b0-4045">Suporte à saída no formato de arquivo de autenticação do SDK para `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4045">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="3c5b0-4046">Limpar as atribuições de função e aplicativos relacionados ao AAD ao excluir uma entidade de serviço (#3610)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4046">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="3c5b0-4047">Incluir o formato de hora nos argumentos `app create` e descrições `--start-date` e `--end-date`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4047">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="3c5b0-4048">Mostrar avisos de código obsoleto ao usar `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4048">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="3c5b0-4049">Adicionada a integração do cofre de chaves para os comandos `create-for-rbac` e `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4049">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="3c5b0-4050">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4050">Service Fabric</span></span>
* <span data-ttu-id="3c5b0-4051">Corrigido um problema com arquivos grandes em aplicativos que eram truncados ao serem carregados (#3666)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4051">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="3c5b0-4052">Adicionados testes para os comandos do Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4052">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="3c5b0-4053">Corrigidos vários comandos do Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4053">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="3c5b0-4054">SQL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4054">SQL</span></span>

* <span data-ttu-id="3c5b0-4055">Removido o parâmetro `sql server create` `--identity` desfeito</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4055">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="3c5b0-4056">Remover os valores de senha da saída dos comandos `sql server create` e `sql server update`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4056">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="3c5b0-4057">Adicionados os comandos para `sql db list-editions` e `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4057">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-4058">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4058">Storage</span></span>

* <span data-ttu-id="3c5b0-4059">Removida a opção `--marker` dos comandos `storage blob list`, `storage container list`, e `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4059">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="3c5b0-4060">Habilitado a criação de uma conta de armazenamento somente para https</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4060">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="3c5b0-4061">Atualizadas as métricas de armazenamento, registro em log e os comandos do CORS (#3495)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4061">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="3c5b0-4062">Mensagem de exceção reformulada do ADD do CORS adicionar (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4062">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="3c5b0-4063">Convertido o gerador para uma lista no modo de simulação de comando do lote de download (#3592)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4063">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="3c5b0-4064">Corrigido o problema de simulação do lote de download de blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4064">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="3c5b0-4065">VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4065">VM</span></span>

* <span data-ttu-id="3c5b0-4066">Suporte para configuração de NSG</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4066">Support configuring nsg</span></span>
* <span data-ttu-id="3c5b0-4067">Corrigido o bug onde o servidor DNS não era configurado corretamente</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4067">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="3c5b0-4068">Suporte às identidades de serviço gerenciado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4068">Support managed service identities</span></span>
* <span data-ttu-id="3c5b0-4069">Corrigido o problema onde `cmss create` com um balanceador de carga existente exigia `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4069">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="3c5b0-4070">Os discos de dados criados com LUN do `vm image create` agora começam com 0</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4070">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="3c5b0-4071">10 de maio de 2017</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4071">May 10, 2017</span></span>

<span data-ttu-id="3c5b0-4072">Versão 2.0.6</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4072">Version 2.0.6</span></span>

* <span data-ttu-id="3c5b0-4073">Renomeação do DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4073">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="3c5b0-4074">Adição do RDBMS (MySQL, Postgres)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4074">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="3c5b0-4075">Inclusão dos módulos Data Lake Analytics e Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4075">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="3c5b0-4076">Inclusão do módulo Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4076">Include Cognitive Services module</span></span>
* <span data-ttu-id="3c5b0-4077">Inclusão do módulo Service Fabric</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4077">Include Service Fabric module</span></span>
* <span data-ttu-id="3c5b0-4078">Inclusão do módulo Interativo (renomeação de az-shell)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4078">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="3c5b0-4079">Adição de suporte para comandos CDN</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4079">Add support for CDN commands</span></span>
* <span data-ttu-id="3c5b0-4080">Remoção do módulo Contêiner</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4080">Remove Container module</span></span>
* <span data-ttu-id="3c5b0-4081">Adição de “az -v” como atalho para “az --version” ([nº 2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4081">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="3c5b0-4082">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4082">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="3c5b0-4083">Núcleo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4083">Core</span></span>

* <span data-ttu-id="3c5b0-4084">núcleo: captura de exceções causadas por um provedor não registrado e seu registro automático</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4084">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="3c5b0-4085">desempenho: persistência do cache de tokens do ADAL na memória até o encerramento do processo ([nº 2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4085">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="3c5b0-4086">Correção de bytes retornados da impressão digital hexadecimal -o tsv ([nº 3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4086">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="3c5b0-4087">Melhoria do download do Certificado do Key Vault e da integração de SP do AAD ([nº 3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4087">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="3c5b0-4088">Adição da localização do Python a “az —version” ([nº 2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4088">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="3c5b0-4089">logon: suporte ao logon quando não há nenhuma assinatura ([nº 2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4089">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="3c5b0-4090">núcleo: correção de uma falha ao fazer logon usando uma entidade de serviço duas vezes ([nº 2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4090">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="3c5b0-4091">núcleo: permitir que o caminho do arquivo accessTokens.json seja configurável por meio de uma variável de ambiente ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4091">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="3c5b0-4092">núcleo: permitir que padrões configurados sejam aplicados em argumentos opcionais ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4092">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="3c5b0-4093">núcleo: desempenho aprimorado</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4093">core: Improved performance</span></span>
* <span data-ttu-id="3c5b0-4094">núcleo: certificados de AC personalizados – suporte à configuração da variável de ambiente REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4094">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="3c5b0-4095">núcleo: configuração na nuvem – uso do ponto de extremidade do “Resource Manager” caso o ponto de extremidade de “Gerenciamento” não esteja definido</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4095">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="3c5b0-4096">ACS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4096">ACS</span></span>

* <span data-ttu-id="3c5b0-4097">correção da contagem mestre e de agente para ser inteiro em vez de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4097">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="3c5b0-4098">exposição de “az acs create --no-wait” e “az acs wait” para a criação assíncrona</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4098">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="3c5b0-4099">exposição de “az acs create --validate” para validações de simulação</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4099">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="3c5b0-4100">remoção do perfil do Windows antes da chamada PUT ao comando scale ([nº 2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4100">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-4101">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4101">AppService</span></span>

* <span data-ttu-id="3c5b0-4102">functionapp: adição de suportes completos a functionapp, incluindo create, show, list, delete, hostname, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4102">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="3c5b0-4103">Adição do VSTS (Team Services) como uma opção de entrega contínua a “appservice web source-control config”</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4103">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="3c5b0-4104">Criação de “az webapp” para substituição de “az appservice web” (para compatibilidade com versões anteriores, “az appservice web” permanecerá por duas versões)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4104">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="3c5b0-4105">Exposição de argumentos para configurar a implantação e as “pilhas em runtime” em webapp create</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4105">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="3c5b0-4106">Exposição de “webapp list-runtimes”</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4106">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="3c5b0-4107">suporte à configuração de cadeias de conexão ([nº 2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4107">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="3c5b0-4108">suporte à permuta de slots com visualização</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4108">support slot swap with preview</span></span>
* <span data-ttu-id="3c5b0-4109">Correção de erros em comandos appservice ([nº 2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4109">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="3c5b0-4110">Uso do grupo de recursos do plano do serviço de aplicativo para operações de certificado ([nº 2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4110">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="3c5b0-4111">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4111">CosmosDB</span></span>

* <span data-ttu-id="3c5b0-4112">Renomeação do módulo DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4112">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="3c5b0-4113">Adição de suporte para APIs do plano de dados do DocumentDB: gerenciamento de banco de dados e de coleção</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4113">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="3c5b0-4114">Adição de suporte para habilitar o failover automático em contas de banco de dados</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4114">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="3c5b0-4115">Adição de suporte para nova política de consistência ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4115">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="3c5b0-4116">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4116">Data Lake Analytics</span></span>

* <span data-ttu-id="3c5b0-4117">Correção de um bug em que a filtragem no resultado e no estado das listas de trabalho gera um erro</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4117">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="3c5b0-4118">Adição de suporte para o novo tipo de item de catálogo: pacote.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4118">Add support for new catalog item type: package.</span></span> <span data-ttu-id="3c5b0-4119">acessado por meio de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4119">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="3c5b0-4120">Possibilidade de listar os seguintes itens de catálogo no banco de dados (sem a necessidade de especificação de esquema):</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4120">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="3c5b0-4121">Tabela</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4121">Table</span></span>
  * <span data-ttu-id="3c5b0-4122">Função com valor de tabela</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4122">Table valued function</span></span>
  * <span data-ttu-id="3c5b0-4123">Visualizar</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4123">View</span></span>
  * <span data-ttu-id="3c5b0-4124">Estatísticas de Tabela.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4124">Table Statistics.</span></span> <span data-ttu-id="3c5b0-4125">Isso também pode ser listado com um esquema, mas sem a especificação de um nome de tabela</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4125">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="3c5b0-4126">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4126">Data Lake Store</span></span>

* <span data-ttu-id="3c5b0-4127">Atualização da versão do SDK do sistema de arquivos subjacente, que fornece melhor suporte para lidar com cenários de limitação do servidor</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4127">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="3c5b0-4128">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4128">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="3c5b0-4129">Ausência de ajuda para mostrar o acesso.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4129">missed help for access show.</span></span> <span data-ttu-id="3c5b0-4130">Adição em andamento.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4130">adding it.</span></span> <span data-ttu-id="3c5b0-4131">([nº 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4131">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="3c5b0-4132">Localizar</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4132">Find</span></span>

* <span data-ttu-id="3c5b0-4133">melhoria dos resultados da pesquisa e permissão de controle de versão do índice de pesquisa</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4133">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="3c5b0-4134">KeyVault</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4134">KeyVault</span></span>

* <span data-ttu-id="3c5b0-4135">BC:`az keyvault certificate download` alteração de -e da cadeia de caracteres ou do binário para PEM ou DER a fim de representar melhor as opções</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4135">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="3c5b0-4136">BC: remoção de --expires e --not-before de `keyvault certificate create`, pois estes parâmetros não têm suporte no serviço</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4136">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="3c5b0-4137">Adição do parâmetro --validity a `keyvault certificate create` para substituir seletivamente o valor em --policy</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4137">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="3c5b0-4138">Correção do problema em `keyvault certificate get-default-policy`, em que “expires” e “not_before” eram expostos, ao contrário de “validity_in_months”</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4138">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="3c5b0-4139">Correção do cofre de chaves para importação de PEM e PFX ([nº 2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4139">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="3c5b0-4140">Laboratório</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4140">Lab</span></span>

* <span data-ttu-id="3c5b0-4141">Adição dos comandos create, show, delete e list ao ambiente do laboratório</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4141">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="3c5b0-4142">Adição dos comandos show e list para exibir modelos ARM no laboratório</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4142">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="3c5b0-4143">Adição do sinalizador --environment a `az lab vm list` para filtrar as VMs por ambiente no laboratório</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4143">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="3c5b0-4144">Adição do comando de conveniência `az lab formula export-artifacts` para exportar o scaffold de artefato em uma fórmula do Laboratório</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4144">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="3c5b0-4145">Adição de comandos para gerenciar segredos em um Laboratório</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4145">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="3c5b0-4146">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4146">Monitor</span></span>

* <span data-ttu-id="3c5b0-4147">Correção de bug: modelagem de `--actions` de `az alert-rules create` para consumir a cadeia de caracteres JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4147">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="3c5b0-4148">Correção de bug – as configurações de diagnóstico criam, mas não aceitam logs e métrica de comandos show ([nº 2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4148">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="3c5b0-4149">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4149">Network</span></span>

* <span data-ttu-id="3c5b0-4150">Adição do comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4150">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="3c5b0-4151">Adição de suporte para o parâmetro `--filters` de `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4151">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="3c5b0-4152">Adição de suporte para drenagem de conexão do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4152">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="3c5b0-4153">Adição de suporte para a configuração do conjunto de regras WAF do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4153">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="3c5b0-4154">Adição de suporte para filtros de rota e regras do ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4154">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="3c5b0-4155">Adição de suporte para o roteamento geográfico do Gerenciador de Tráfego</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4155">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="3c5b0-4156">Adição de suporte para seletores de tráfego baseados em política da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4156">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="3c5b0-4157">Adição de suporte para políticas IPsec da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4157">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="3c5b0-4158">Correção de um bug com `vpn-connection create` ao usar os parâmetros `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4158">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="3c5b0-4159">Adição de suporte para gateways de VNet ativos/ativos</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4159">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="3c5b0-4160">Remoção de valores nulos na saída de comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4160">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="3c5b0-4161">BC: corrigido um bug na saída de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4161">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="3c5b0-4162">Correção de um bug em que o argumento “--key-length” de “vpn-connection create” não é analisado corretamente</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4162">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="3c5b0-4163">Correção de um bug em `dns zone import`, em que os registros não são importados corretamente</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4163">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="3c5b0-4164">Correção de um bug em que `traffic-manager endpoint update` não funciona</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4164">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="3c5b0-4165">Adição de comandos de visualização “network watcher”</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4165">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="3c5b0-4166">Perfil</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4166">Profile</span></span>

* <span data-ttu-id="3c5b0-4167">Suporte ao logon quando não há nenhuma assinatura encontrada ([nº 2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4167">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="3c5b0-4168">Suporte ao nome curto do parâmetro em az account set --subscription ([nº 2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4168">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="3c5b0-4169">Redis</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4169">Redis</span></span>

* <span data-ttu-id="3c5b0-4170">Adição do comando update que também adiciona a capacidade de dimensionar o Cache Redis</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4170">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="3c5b0-4171">Preterição do comando “update-settings”</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4171">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="3c5b0-4172">Recurso</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4172">Resource</span></span>

* <span data-ttu-id="3c5b0-4173">Adição dos comandos de definição managedapp e managedapp ([nº 2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4173">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="3c5b0-4174">Suporte aos comandos “provider operation” ([nº 2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4174">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="3c5b0-4175">Suporte à criação de recurso genérico ([nº 2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4175">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="3c5b0-4176">Correção da análise de recurso e da pesquisa de versão de API.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4176">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="3c5b0-4177">([nº 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4177">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="3c5b0-4178">Adição de documentos a az lock update.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4178">Add docs for az lock update.</span></span> <span data-ttu-id="3c5b0-4179">([nº 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4179">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="3c5b0-4180">Erro ao tentar listar recursos de um grupo que não existe.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4180">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="3c5b0-4181">([nº 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4181">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="3c5b0-4182">[Computação] Correção de problemas com a atualização do conjunto de disponibilidade da VMSS e da VM.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4182">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="3c5b0-4183">([nº 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4183">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="3c5b0-4184">Correção de lock create e delete se parent-resource-path é None ([nº 2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4184">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="3c5b0-4185">Função</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4185">Role</span></span>

* <span data-ttu-id="3c5b0-4186">create-for-rbac: garantia de que a data de término do SP não excederá a data de validade do certificado ([nº 2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4186">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="3c5b0-4187">RBAC: adição de suporte completo a “ad group” ([nº 2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4187">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="3c5b0-4188">função: correção de problemas na atualização de definição de função ([nº 2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4188">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="3c5b0-4189">create-for-rbac: garantia de que a senha fornecida pelo usuário é coletada</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4189">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="3c5b0-4190">SQL</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4190">SQL</span></span>

* <span data-ttu-id="3c5b0-4191">Adição dos comandos az sql server list-usages e az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4191">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="3c5b0-4192">SQL – capacidade de se conectar diretamente ao provedor de recursos ([nº 2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4192">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="3c5b0-4193">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4193">Storage</span></span>

* <span data-ttu-id="3c5b0-4194">Localização padrão da localização do grupo de recursos de `storage account create`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4194">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="3c5b0-4195">Adição de suporte para cópia incremental de blob</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4195">Add support for incremental blob copy</span></span>
* <span data-ttu-id="3c5b0-4196">Adição de suporte para upload de blobs de blocos grandes</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4196">Add support for large block blob upload</span></span>
* <span data-ttu-id="3c5b0-4197">Alteração do tamanho do bloco para 100MB quando o arquivo a ser carregado é maior que 200GB</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4197">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="3c5b0-4198">VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4198">VM</span></span>

* <span data-ttu-id="3c5b0-4199">avail-set: as contagens de domínio de UD e FD agora são opcionais</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4199">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="3c5b0-4200">observação: em comandos da VM em nuvens soberanas, evite recursos relacionados ao disco gerenciado, incluindo os seguintes:</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4200">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="3c5b0-4201">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4201">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="3c5b0-4202">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4202">az vm/vmss disk</span></span>
  3. <span data-ttu-id="3c5b0-4203">Em “az vm/vmss create”, use “—use-unmanaged-disk” para evitar o disco gerenciado Outros comandos deverão funcionar</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4203">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="3c5b0-4204">VM/VMSS: melhoria do texto de aviso ao gerar pares de chaves SSH</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4204">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="3c5b0-4205">VM/VMSS: suporte à criação com base em uma imagem do Marketplace que exige informações de plano ([nº 1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4205">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="3c5b0-4206">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4206">April 3, 2017</span></span>

<span data-ttu-id="3c5b0-4207">Versão 2.0.2</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4207">Version 2.0.2</span></span>

<span data-ttu-id="3c5b0-4208">Lançamos os componentes ACR, Batch, KeyVault, e SQL nessa versão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4208">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="3c5b0-4209">Núcleo</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4209">Core</span></span>

* <span data-ttu-id="3c5b0-4210">Adicionar módulos acr, laboratório, monitor e localizar à lista padrão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4210">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="3c5b0-4211">Logon: ignorar locatário errado ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4211">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="3c5b0-4212">logon: definir assinatura padrão como um com o estado de "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4212">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="3c5b0-4213">Adicionar comandos de espera e suporte --no-wait para mais comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4213">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="3c5b0-4214">núcleo: suporte a logon usando a entidade de serviço com um certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4214">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="3c5b0-4215">Adicione solicitação para parâmetros de modelo ausentes.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4215">Add prompting for missing template parameters.</span></span> <span data-ttu-id="3c5b0-4216">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4216">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="3c5b0-4217">Suporte à definição de valores padrão para os argumentos comuns como grupo de recursos padrão, Web padrão, vm padrão</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4217">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="3c5b0-4218">Suporte a logon para um locatário específico</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4218">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="3c5b0-4219">ACS</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4219">ACS</span></span>

* <span data-ttu-id="3c5b0-4220">[ACS] Adicionar suporte para configurar um cluster do ACS padrão ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4220">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="3c5b0-4221">Adicione suporte para solicitação de senha de chave ssh.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4221">Add support for ssh key password prompting.</span></span> <span data-ttu-id="3c5b0-4222">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4222">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="3c5b0-4223">Adicione suporte para clusters do windows.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4223">Add support for windows clusters.</span></span> <span data-ttu-id="3c5b0-4224">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4224">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="3c5b0-4225">Alterne da função Proprietário para Colaborador.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4225">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="3c5b0-4226">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4226">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="3c5b0-4227">AppService</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4227">AppService</span></span>

* <span data-ttu-id="3c5b0-4228">AppService: suporte para obter o endereço ip externo usado para registros de DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4228">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="3c5b0-4229">AppService: suporte à associação de certificados curinga ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4229">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="3c5b0-4230">AppService: lista de suporte à publicação de perfis ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4230">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="3c5b0-4231">AppService - Aciona a sincronização de controle de origem após a configuração ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4231">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="3c5b0-4232">DataLake</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4232">DataLake</span></span>

* <span data-ttu-id="3c5b0-4233">Versão inicial do módulo do Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4233">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="3c5b0-4234">Versão inicial do módulo do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4234">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="3c5b0-4235">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4235">DocuemntDB</span></span>

* <span data-ttu-id="3c5b0-4236">DocumentDB: adicionado suporte para a listagem de cadeias de conexão ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4236">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="3c5b0-4237">VM</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4237">VM</span></span>

* <span data-ttu-id="3c5b0-4238">[Compute] Adicionar suporte a AppGateway para criar o conjunto de dimensionamento de máquinas virtuais ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4238">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="3c5b0-4239">[VM/VMSS] Suporte aprimorado ao cache de disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4239">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="3c5b0-4240">VM/VMSS: incorporar a lógica de validação de credenciais usada pelo portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4240">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="3c5b0-4241">Adicionar comandos de espera e suporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4241">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="3c5b0-4242">Conjunto de dimensionamento de máquinas virtuais: suporte à \* para listar a exibição de instâncias em vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4242">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="3c5b0-4243">Adicionar: segredos da VM e do conjunto de dimensionamento de máquinas virtuais ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4243">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="3c5b0-4244">Permitir a criação de VMs com VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4244">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="3c5b0-4245">27 de fevereiro de 2017</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4245">February 27, 2017</span></span>

<span data-ttu-id="3c5b0-4246">Versão 2.0.0</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4246">Version 2.0.0</span></span>

<span data-ttu-id="3c5b0-4247">Esta versão da CLI do Azure 2.0 é a primeira versão "Amplamente Disponível". A disponibilidade geral se aplica a estes módulos de comando:</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4247">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="3c5b0-4248">Serviço de Contêiner (acs)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4248">Container Service (acs)</span></span>
- <span data-ttu-id="3c5b0-4249">Computação (incluindo Gerenciador de Recursos, VM, conjunto de dimensionamento de máquinas virtuais, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4249">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="3c5b0-4250">Rede</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4250">Networking</span></span>
- <span data-ttu-id="3c5b0-4251">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4251">Storage</span></span>

<span data-ttu-id="3c5b0-4252">Esses módulos de comando podem ser usados na produção e têm suporte do SLA padrão da Microsoft. Você pode abrir problemas diretamente com o suporte da Microsoft ou em nossa [lista de problemas do github](https://github.com/azure/azure-cli/issues/). Faça perguntas no [StackOverflow usando a marca azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contate a equipe de produto em [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) Forneça comentários na linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4252">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="3c5b0-4253">Os comandos nesses módulos são estáveis e a sintaxe não deve ser alterada em versões futuras dessa versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4253">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="3c5b0-4254">Para verificar a versão da CLI, use `az --version` A saída lista a versão da CLI (2.0.0 nessa versão), os módulos de comando individuais, as versões do Python e GCC que você está usando</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4254">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="3c5b0-4255">Alguns dos módulos de comando têm um sufixo "b *n* " ou "rc *n* ". Esses módulos de comando ainda estão em versão prévia e estarão disponíveis no futuro</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4255">Some of the command modules have a "b *n* " or "rc *n* " postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="3c5b0-4256">Também temos compilações de versão prévia noturnas da CLI. Para obter informações, consulte essas instruções sobre [como obter as compilações diárias](https://github.com/Azure/azure-cli#nightly-builds) e essas instruções sobre [configuração do desenvolvedor e código de contribuição](https://github.com/Azure/azure-cli#developer-setup)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4256">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="3c5b0-4257">Você pode relatar problemas com as compilações de visualização diárias das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4257">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="3c5b0-4258">Relatar problemas na [lista de problemas do github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4258">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="3c5b0-4259">Entre em contato com a equipe do produto no endereço [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4259">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="3c5b0-4260">Forneça comentários a partir da linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4260">Provide feedback from the command line with the `az feedback` command</span></span>

# <a name="beta-release-notes"></a>[<span data-ttu-id="3c5b0-4261">Notas sobre a versão beta</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4261">Beta release notes</span></span>](#tab/azure-cli-beta)

<span data-ttu-id="3c5b0-4262">A versão beta da CLI do Azure é uma migração do método de autenticação da plataforma AAD (v 1.0) para a [plataforma de Identidade da Microsoft (v 2.0)](/azure/active-directory/develop/v2-overview).</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4262">The Azure CLI beta release is a migration from the authentican method of AAD platform (v1.0) to [Microsoft Identity platform (v2.0)](/azure/active-directory/develop/v2-overview).</span></span>

## <a name="june-23-2020"></a><span data-ttu-id="3c5b0-4263">23 de junho de 2020</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4263">June 23, 2020</span></span>

### <a name="things-to-know-about-the-new-azure-cli-beta-release"></a><span data-ttu-id="3c5b0-4264">O que você precisa saber sobre a nova versão beta da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4264">Things to know about the new Azure CLI beta release</span></span>

-   <span data-ttu-id="3c5b0-4265">A versão beta da CLI do Azure dá suporte a todos os comandos da CLI que você encontrará na versão lançada atual.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4265">The beta version of the Azure CLI supports all CLI commands that you will find in the current released version.</span></span>
-   <span data-ttu-id="3c5b0-4266">Fazer logon novamente é necessário após a instalação da versão beta.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4266">Relogin is required after install the beta version.</span></span>
-   <span data-ttu-id="3c5b0-4267">A versão beta dá suporte apenas à plataforma Windows.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4267">The beta release only supports the Windows platform.</span></span>
-   <span data-ttu-id="3c5b0-4268">Não há suporte para o Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4268">The Azure Stack is not supported.</span></span>
-   <span data-ttu-id="3c5b0-4269">Não há suporte para o parâmetro `--use-cert-sn-issuer` ao usar a chave de entidade de serviço para se autenticar.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4269">`--use-cert-sn-issuer` parameter is not supported when using service principal key to authenticate.</span></span>
-   <span data-ttu-id="3c5b0-4270">Não há suporte para ignorar a verificação SSL por meio do ambiente `ADAL_PYTHON_SSL_NO_VERIFY`.</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4270">Skip SSL verification via environment `ADAL_PYTHON_SSL_NO_VERIFY` is not supported.</span></span>

<span data-ttu-id="3c5b0-4271">Se você encontrar problemas com a versão beta, a equipe de engenharia da CLI do Azure ficará feliz por receber seus comentários no [GitHub](https://github.com/Azure/azure-cli/issues/new/choose).</span><span class="sxs-lookup"><span data-stu-id="3c5b0-4271">If you find any issues in the beta release, the Azure CLI engineering team welcomes your comments on [GitHub](https://github.com/Azure/azure-cli/issues/new/choose).</span></span>

---
