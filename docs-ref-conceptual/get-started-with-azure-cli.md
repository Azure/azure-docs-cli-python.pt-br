---
title: Introdução à CLI do Azure
description: Comece a usar a CLI do Azure aprendendo as noções básicas de comando.
keywords: CLI do Azure, ajuda da CLI, ajuda do Azure, consulta, automação,
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 01/30/2020
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 741d092121bbd448595301000acb9a5f51d87ace
ms.sourcegitcommit: d0b2763cc856eef44a6ecb78f6b8c64291625750
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/04/2020
ms.locfileid: "77013243"
---
# <a name="get-started-with-azure-cli"></a><span data-ttu-id="0e893-104">Introdução à CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="0e893-104">Get started with Azure CLI</span></span>

<span data-ttu-id="0e893-105">Bem-vindo à CLI do Azure!</span><span class="sxs-lookup"><span data-stu-id="0e893-105">Welcome to the Azure CLI!</span></span>  <span data-ttu-id="0e893-106">Este artigo apresenta a CLI e fornece links para ajudar você a começar a usar.</span><span class="sxs-lookup"><span data-stu-id="0e893-106">This article introduces the CLI and provides links to help you get started.</span></span>

> [!NOTE]
>
> <span data-ttu-id="0e893-107">Em scripts e no site de documentação da Microsoft, os exemplos da CLI do Azure são escritos para o shell `bash`.</span><span class="sxs-lookup"><span data-stu-id="0e893-107">In scripts and on the Microsoft documentation site, Azure CLI examples are written for the `bash` shell.</span></span> <span data-ttu-id="0e893-108">Os exemplos de uma linha serão executados em qualquer plataforma.</span><span class="sxs-lookup"><span data-stu-id="0e893-108">One-line examples will run on any platform.</span></span> <span data-ttu-id="0e893-109">Os exemplos mais longos, que incluem continuações da linha (`\`) ou a atribuição de variáveis precisam ser modificados para funcionar em outros shells, incluindo o PowerShell.</span><span class="sxs-lookup"><span data-stu-id="0e893-109">Longer examples which include line continuations (`\`) or variable assignment need to be modified to work on other shells, including PowerShell.</span></span>

## <a name="install-or-run-in-azure-cloud-shell"></a><span data-ttu-id="0e893-110">Instalar ou executar no Azure Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="0e893-110">Install or run in Azure Cloud Shell</span></span>

<span data-ttu-id="0e893-111">A maneira mais fácil começar a usar a CLI do Azure é executando-a em um ambiente do Azure Cloud Shell por meio do seu navegador.</span><span class="sxs-lookup"><span data-stu-id="0e893-111">The easiest way to get started with the Azure CLI is by running it in an Azure Cloud Shell environment through your browser.</span></span> <span data-ttu-id="0e893-112">Para saber mais sobre o Cloud Shell, consulte [Início Rápido para Bash no Azure Cloud Shell](/azure/cloud-shell/quickstart).</span><span class="sxs-lookup"><span data-stu-id="0e893-112">To learn about Cloud Shell, see  [Quickstart for Bash in Azure Cloud Shell](/azure/cloud-shell/quickstart).</span></span>

<span data-ttu-id="0e893-113">Quando você estiver pronto para instalar a CLI, confira as [instruções de instalação](install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="0e893-113">When you're ready to install the CLI, see the [installation instructions](install-azure-cli.md).</span></span>

<span data-ttu-id="0e893-114">Depois de instalar a CLI pela primeira vez, verifique se ela está instalada e se você tem a versão correta, executando `az --version`.</span><span class="sxs-lookup"><span data-stu-id="0e893-114">After installing the CLI for the first time, check that it's installed and you've got the correct version by running `az --version`.</span></span>

## <a name="sign-in"></a><span data-ttu-id="0e893-115">Entrar</span><span class="sxs-lookup"><span data-stu-id="0e893-115">Sign in</span></span>

<span data-ttu-id="0e893-116">Antes de usar os comandos da CLI com uma instalação local, é preciso entrar com [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="0e893-116">Before using any CLI commands with a local install, you need to sign in with [az login](/cli/azure/reference-index#az-login).</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="0e893-117">Depois de entrar, você deve ver uma lista de assinaturas associadas à sua conta do Azure.</span><span class="sxs-lookup"><span data-stu-id="0e893-117">After logging in, you see a list of subscriptions associated with your Azure account.</span></span> <span data-ttu-id="0e893-118">A informação de assinatura com `isDefault: true` é a assinatura ativada no momento depois de entrar.</span><span class="sxs-lookup"><span data-stu-id="0e893-118">The subscription information with `isDefault: true` is the currently activated subscription after logging in.</span></span> <span data-ttu-id="0e893-119">Para selecionar outra assinatura, use o comando [az account set](/cli/azure/account#az-account-set) com a ID da assinatura para a qual alternar.</span><span class="sxs-lookup"><span data-stu-id="0e893-119">To select another subscription, use the [az account set](/cli/azure/account#az-account-set) command with the subscription ID to switch to.</span></span> <span data-ttu-id="0e893-120">Para obter mais informações sobre a seleção da assinatura, confira [Usar várias assinaturas do Azure](manage-azure-subscriptions-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="0e893-120">For more information about subscription selection, see [Use multiple Azure subscriptions](manage-azure-subscriptions-azure-cli.md).</span></span>

<span data-ttu-id="0e893-121">Há maneiras de entrar de modo não interativo, como mostrado em detalhes em [Entrar com a CLI do Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="0e893-121">There are ways to sign in non-interactively, which are covered in detail in [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="common-commands"></a><span data-ttu-id="0e893-122">Comandos comuns</span><span class="sxs-lookup"><span data-stu-id="0e893-122">Common commands</span></span>

<span data-ttu-id="0e893-123">Esta tabela lista alguns comandos comuns usados na CLI e está vinculada à documentação de referência.</span><span class="sxs-lookup"><span data-stu-id="0e893-123">This table lists some common commands used in the CLI and links to their reference documentation.</span></span>

| <span data-ttu-id="0e893-124">Tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="0e893-124">Resource type</span></span> | <span data-ttu-id="0e893-125">Grupo de comando da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="0e893-125">Azure CLI command group</span></span> |
|---------------|-------------------------|
| [<span data-ttu-id="0e893-126">Grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="0e893-126">Resource group</span></span>](/azure/azure-resource-manager/resource-group-overview) | [<span data-ttu-id="0e893-127">az group</span><span class="sxs-lookup"><span data-stu-id="0e893-127">az group</span></span>](/cli/azure/group) |
| [<span data-ttu-id="0e893-128">Máquinas virtuais</span><span class="sxs-lookup"><span data-stu-id="0e893-128">Virtual machines</span></span>](/azure/virtual-machines) | [<span data-ttu-id="0e893-129">az vm</span><span class="sxs-lookup"><span data-stu-id="0e893-129">az vm</span></span>](/cli/azure/vm) |
| [<span data-ttu-id="0e893-130">Contas de armazenamento</span><span class="sxs-lookup"><span data-stu-id="0e893-130">Storage accounts</span></span>](/azure/storage/common/storage-introduction) | [<span data-ttu-id="0e893-131">az storage account</span><span class="sxs-lookup"><span data-stu-id="0e893-131">az storage account</span></span>](/cli/azure/storage/account) |
| [<span data-ttu-id="0e893-132">Key Vault</span><span class="sxs-lookup"><span data-stu-id="0e893-132">Key Vault</span></span>](/azure/key-vault/key-vault-whatis) | [<span data-ttu-id="0e893-133">az keyvault</span><span class="sxs-lookup"><span data-stu-id="0e893-133">az keyvault</span></span>](/cli/azure/keyvault) |
| [<span data-ttu-id="0e893-134">Aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="0e893-134">Web applications</span></span>](/azure/app-service) | [<span data-ttu-id="0e893-135">az webapp</span><span class="sxs-lookup"><span data-stu-id="0e893-135">az webapp</span></span>](/cli/azure/webapp) |
| [<span data-ttu-id="0e893-136">Bancos de dados SQL</span><span class="sxs-lookup"><span data-stu-id="0e893-136">SQL databases</span></span>](/azure/sql-database) | [<span data-ttu-id="0e893-137">az sql server</span><span class="sxs-lookup"><span data-stu-id="0e893-137">az sql server</span></span>](/cli/azure/sql/server) |
| [<span data-ttu-id="0e893-138">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="0e893-138">CosmosDB</span></span>](/azure/cosmos-db) | [<span data-ttu-id="0e893-139">az cosmosdb</span><span class="sxs-lookup"><span data-stu-id="0e893-139">az cosmosdb</span></span>](/cli/azure/cosmosdb) |

## <a name="finding-commands"></a><span data-ttu-id="0e893-140">Encontrando comandos</span><span class="sxs-lookup"><span data-stu-id="0e893-140">Finding commands</span></span>

<span data-ttu-id="0e893-141">Os comandos na CLI são organizados como _comandos_ de _grupos_.</span><span class="sxs-lookup"><span data-stu-id="0e893-141">Commands in the CLI are organized as _commands_ of _groups_.</span></span> <span data-ttu-id="0e893-142">Cada grupo representa um serviço do Azure e os comandos operam nesse serviço.</span><span class="sxs-lookup"><span data-stu-id="0e893-142">Each group represents an Azure service, and commands operate on that service.</span></span>

<span data-ttu-id="0e893-143">Para procurar comandos, use [az find](/cli/azure/reference-index#az-find).</span><span class="sxs-lookup"><span data-stu-id="0e893-143">To search for commands, use [az find](/cli/azure/reference-index#az-find).</span></span> <span data-ttu-id="0e893-144">Por exemplo, para procurar nomes de comando que contenham `secret`, use o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="0e893-144">For example, to search for command names containing `secret`, use the following command:</span></span>

```azurecli-interactive
az find secret
```

<span data-ttu-id="0e893-145">Use o argumento `--help` para obter uma lista completa de comandos e subgrupos de um grupo.</span><span class="sxs-lookup"><span data-stu-id="0e893-145">Use the `--help` argument to get a complete list of commands and subgroups of a group.</span></span> <span data-ttu-id="0e893-146">Por exemplo, para localizar os comandos da CLI para trabalhar com Grupos de Segurança de Rede (NSGs):</span><span class="sxs-lookup"><span data-stu-id="0e893-146">For example, to find the CLI commands for working with Network Security Groups (NSGs):</span></span>

```azurecli-interactive
az network nsg --help
```

<span data-ttu-id="0e893-147">A CLI tem o preenchimento completo de guia para comandos sob o shell do Bash.</span><span class="sxs-lookup"><span data-stu-id="0e893-147">The CLI has full tab completion for commands under the bash shell.</span></span>

## <a name="globally-available-arguments"></a><span data-ttu-id="0e893-148">Argumentos disponíveis globalmente</span><span class="sxs-lookup"><span data-stu-id="0e893-148">Globally available arguments</span></span>

<span data-ttu-id="0e893-149">Há alguns argumentos disponíveis para cada comando.</span><span class="sxs-lookup"><span data-stu-id="0e893-149">There are some arguments that are available for every command.</span></span>

* <span data-ttu-id="0e893-150">`--help` imprime as informações de referência da CLI sobre comandos e seus argumentos, além de listar os comandos e subgrupos disponíveis.</span><span class="sxs-lookup"><span data-stu-id="0e893-150">`--help` prints CLI reference information about commands and their arguments and lists available subgroups and commands.</span></span>
* <span data-ttu-id="0e893-151">`--output` altera o formato de saída.</span><span class="sxs-lookup"><span data-stu-id="0e893-151">`--output` changes the output format.</span></span> <span data-ttu-id="0e893-152">Os formatos de saída disponíveis são `json`, `jsonc`(JSON colorido), `tsv` (valores separados por tabulação), `table` (tabelas ASCII legível por humanos) e `yaml`.</span><span class="sxs-lookup"><span data-stu-id="0e893-152">The available output formats are `json`, `jsonc` (colorized JSON), `tsv` (Tab-Separated Values), `table` (human-readable ASCII tables), and `yaml`.</span></span> <span data-ttu-id="0e893-153">Por padrão, a CLI gera `json`.</span><span class="sxs-lookup"><span data-stu-id="0e893-153">By default the CLI outputs `json`.</span></span> <span data-ttu-id="0e893-154">Para saber mais sobre os formatos de saída disponíveis, confira [Formatos de saída da CLI do Azure](format-output-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="0e893-154">To learn more about the available output formats, see [Output formats for Azure CLI](format-output-azure-cli.md).</span></span>
* <span data-ttu-id="0e893-155">`--query` usa o [linguagem de consulta JMESPath](http://jmespath.org/) para filtrar a saída retornada dos serviços do Azure.</span><span class="sxs-lookup"><span data-stu-id="0e893-155">`--query` uses the [JMESPath query language](http://jmespath.org/) to filter the output returned from Azure services.</span></span> <span data-ttu-id="0e893-156">Para saber mais sobre as consultas, confira [Consultar resultados do comando com a CLI do Azure](query-azure-cli.md) e [Tutorial do JMESPath](http://jmespath.org/tutorial.html).</span><span class="sxs-lookup"><span data-stu-id="0e893-156">To learn more about queries, see [Query command results with Azure CLI](query-azure-cli.md) and the [JMESPath tutorial](http://jmespath.org/tutorial.html).</span></span>
* <span data-ttu-id="0e893-157">`--verbose` imprime informações sobre recursos criados no Azure durante uma operação, além de outras informações úteis.</span><span class="sxs-lookup"><span data-stu-id="0e893-157">`--verbose` prints information about resources created in Azure during an operation, and other useful information.</span></span>
* <span data-ttu-id="0e893-158">`--debug` imprime ainda mais informações sobre operações de CLI e é usado para fins de depuração.</span><span class="sxs-lookup"><span data-stu-id="0e893-158">`--debug` prints even more information about CLI operations, used for debugging purposes.</span></span> <span data-ttu-id="0e893-159">Se você encontrar um bug, forneça a saída gerada com o sinalizador `--debug` ao enviar um relatório de bugs.</span><span class="sxs-lookup"><span data-stu-id="0e893-159">If you find a bug, provide output generated with the `--debug` flag on when submitting a bug report.</span></span>

## <a name="interactive-mode"></a><span data-ttu-id="0e893-160">Modo interativo</span><span class="sxs-lookup"><span data-stu-id="0e893-160">Interactive mode</span></span>

<span data-ttu-id="0e893-161">A CLI oferece um modo interativo que exibe informações de ajuda automaticamente e torna mais fácil selecionar subcomandos.</span><span class="sxs-lookup"><span data-stu-id="0e893-161">The CLI offers an interactive mode that automatically displays help information and makes it easier to select subcommands.</span></span> <span data-ttu-id="0e893-162">Você entra no modo interativo com o comando [az interactive](/cli/azure/reference-index#az-interactive).</span><span class="sxs-lookup"><span data-stu-id="0e893-162">You enter interactive mode with the [az interactive](/cli/azure/reference-index#az-interactive) command.</span></span>

```azurecli-interactive
az interactive
```

<span data-ttu-id="0e893-163">Para obter mais informações sobre o modo interativo, confira [Modo interativo da CLI do Azure](interactive-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="0e893-163">For more information on interactive mode, see [Azure CLI Interactive Mode](interactive-azure-cli.md).</span></span>

<span data-ttu-id="0e893-164">Também há um [plug-in do Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli) que oferece uma experiência interativa, incluindo documentação de preenchimento automático e com o passar do mouse.</span><span class="sxs-lookup"><span data-stu-id="0e893-164">There's also a [Visual Studio Code plugin](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli) that offers an interactive experience, including autocomplete and mouse-over documentation.</span></span>

## <a name="learn-cli-basics-with-quickstarts-and-tutorials"></a><span data-ttu-id="0e893-165">Aprenda as noções básica da CLI com os guias de início rápido e tutoriais</span><span class="sxs-lookup"><span data-stu-id="0e893-165">Learn CLI basics with quickstarts and tutorials</span></span>

<span data-ttu-id="0e893-166">Para a introdução à CLI do Azure, experimente ver um tutorial aprofundado para configurar máquinas virtuais e usar o poder da CLI para consultar recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="0e893-166">To get you started with the Azure CLI, try an in-depth tutorial for setting up virtual machines and using the power of the CLI to query Azure resources.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="0e893-167">Tutorial Criar máquinas virtuais com a CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="0e893-167">Create virtual machines with the Azure CLI tutorial</span></span>](azure-cli-vm-tutorial.yml)

<span data-ttu-id="0e893-168">Também há guias de início rápido para outros serviços populares.</span><span class="sxs-lookup"><span data-stu-id="0e893-168">There are also quickstarts for other popular services.</span></span>

* [<span data-ttu-id="0e893-169">Criar uma conta de armazenamento usando a CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="0e893-169">Create a storage account using the Azure CLI</span></span>](/azure/storage/common/storage-quickstart-create-storage-account-cli)
* [<span data-ttu-id="0e893-170">Transferir objetos de/para o Armazenamento de blobs do Azure usando a CLI</span><span class="sxs-lookup"><span data-stu-id="0e893-170">Transfer objects to/from Azure Blob storage using the CLI</span></span>](/azure/storage/blobs/storage-quickstart-blobs-cli)
* [<span data-ttu-id="0e893-171">Criar um único banco de dados SQL do Azure usando a CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="0e893-171">Create a single Azure SQL database using the Azure CLI</span></span>](/azure/sql-database/sql-database-get-started-cli)
* [<span data-ttu-id="0e893-172">Criar um servidor de Banco de Dados do Azure para MySQL usando a CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="0e893-172">Create an Azure Database for MySQL server using the Azure CLI</span></span>](/azure/mysql/quickstart-create-mysql-server-database-using-azure-cli)
* [<span data-ttu-id="0e893-173">Criar um servidor de Banco de Dados do Azure para PostgreSQL usando a CLI Azure</span><span class="sxs-lookup"><span data-stu-id="0e893-173">Create an Azure Database for PostgreSQL using the Azure CLI</span></span>](/azure/postgresql/quickstart-create-server-database-azure-cli)
* [<span data-ttu-id="0e893-174">Criar um aplicativo Web do Python no Azure</span><span class="sxs-lookup"><span data-stu-id="0e893-174">Create a Python web app in Azure</span></span>](/azure/app-service/app-service-web-get-started-python)
* [<span data-ttu-id="0e893-175">Executar uma imagem personalizada do Hub do Docker nos Aplicativos Web para Contêineres do Azure</span><span class="sxs-lookup"><span data-stu-id="0e893-175">Run a custom Docker Hub image in Azure Web Apps for Containers</span></span>](/azure/app-service/containers/quickstart-custom-docker-image)

## <a name="give-feedback"></a><span data-ttu-id="0e893-176">Fornecer comentários</span><span class="sxs-lookup"><span data-stu-id="0e893-176">Give feedback</span></span>

<span data-ttu-id="0e893-177">Apreciamos seus comentários da CLI para ajudar-nos a melhorar e resolver bugs.</span><span class="sxs-lookup"><span data-stu-id="0e893-177">We welcome your feedback for the CLI to help us make improvements and resolve bugs.</span></span> <span data-ttu-id="0e893-178">Você pode [arquivar um problema no GitHub](https://github.com/azure/azure-cli/issues) ou usar os recursos internos da CLI para deixar um comentário geral com o comando [az feedback](/cli/azure/reference-index#az-feedback).</span><span class="sxs-lookup"><span data-stu-id="0e893-178">You can [file an issue on GitHub](https://github.com/azure/azure-cli/issues) or use the built-in features of the CLI to leave general feedback with the [az feedback](/cli/azure/reference-index#az-feedback) command.</span></span>

```azurecli-interactive
az feedback
```
