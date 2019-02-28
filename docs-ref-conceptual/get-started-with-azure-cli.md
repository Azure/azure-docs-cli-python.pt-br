---
title: Introdução à CLI do Azure
description: Comece a usar a CLI do Azure aprendendo as noções básicas de comando.
keywords: CLI do Azure, ajuda da CLI, ajuda do Azure, consulta, automação,
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: b018f41824946dca36d0b806de0dd32a335a15b5
ms.sourcegitcommit: 1987a39809f9865034b27130e56f30b2bd1eb72c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/19/2019
ms.locfileid: "56422010"
---
# <a name="get-started-with-azure-cli"></a><span data-ttu-id="836cf-104">Introdução à CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="836cf-104">Get started with Azure CLI</span></span>

<span data-ttu-id="836cf-105">Bem-vindo à CLI do Azure!</span><span class="sxs-lookup"><span data-stu-id="836cf-105">Welcome to the Azure CLI!</span></span> <span data-ttu-id="836cf-106">A CLI é uma ferramenta projetada para ajudar você a trabalhar de forma rápida e eficaz com os serviços do Azure, com ênfase na automação.</span><span class="sxs-lookup"><span data-stu-id="836cf-106">The CLI is a tool designed to get you working quickly and efficiently with Azure services, with an emphasis on automation.</span></span> <span data-ttu-id="836cf-107">Este artigo apresenta recursos da CLI e links externos para recursos que ajudarão você a ser produtivo.</span><span class="sxs-lookup"><span data-stu-id="836cf-107">This article introduces features of the CLI and links out to resources that help you be productive.</span></span>

## <a name="install-or-run-in-azure-cloud-shell"></a><span data-ttu-id="836cf-108">Instalar ou executar no Azure Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="836cf-108">Install or run in Azure Cloud Shell</span></span>

<span data-ttu-id="836cf-109">A maneira mais fácil começar a usar a CLI do Azure é executando-a em um ambiente do Azure Cloud Shell por meio do seu navegador.</span><span class="sxs-lookup"><span data-stu-id="836cf-109">The easiest way to get started with the Azure CLI is by running it in an Azure Cloud Shell environment through your browser.</span></span> <span data-ttu-id="836cf-110">Para saber mais sobre o Cloud Shell, consulte [Início Rápido para Bash no Azure Cloud Shell](/azure/cloud-shell/quickstart).</span><span class="sxs-lookup"><span data-stu-id="836cf-110">To learn about Cloud Shell, see  [Quickstart for Bash in Azure Cloud Shell](/azure/cloud-shell/quickstart).</span></span>

<span data-ttu-id="836cf-111">Quando você estiver pronto para instalar a CLI, confira as [instruções de instalação](install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="836cf-111">When you're ready to install the CLI, see the [installation instructions](install-azure-cli.md).</span></span>

<span data-ttu-id="836cf-112">Depois de instalar a CLI pela primeira vez, verifique se ela está instalada e se você tem a versão correta, executando `az --version`.</span><span class="sxs-lookup"><span data-stu-id="836cf-112">After installing the CLI for the first time, check that it's installed and you've got the correct version by running `az --version`.</span></span>

## <a name="sign-in"></a><span data-ttu-id="836cf-113">Entrar</span><span class="sxs-lookup"><span data-stu-id="836cf-113">Sign in</span></span>

<span data-ttu-id="836cf-114">Antes de usar os comandos da CLI com uma instalação local, é preciso entrar com [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="836cf-114">Before using any CLI commands with a local install, you need to sign in with [az login](/cli/azure/reference-index#az-login).</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="836cf-115">Há maneiras de entrar de modo não interativo, como mostrado em detalhes em [Entrar com a CLI do Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="836cf-115">There are ways to sign in non-interactively, which are covered in detail in [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="common-commands"></a><span data-ttu-id="836cf-116">Comandos comuns</span><span class="sxs-lookup"><span data-stu-id="836cf-116">Common commands</span></span>

<span data-ttu-id="836cf-117">Esta tabela lista alguns comandos comuns usados na CLI e está vinculada à documentação de referência.</span><span class="sxs-lookup"><span data-stu-id="836cf-117">This table lists some common commands used in the CLI and links to their reference documentation.</span></span>

| <span data-ttu-id="836cf-118">Tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="836cf-118">Resource type</span></span> | <span data-ttu-id="836cf-119">Grupo de comando da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="836cf-119">Azure CLI command group</span></span> |
|---------------|-------------------------|
| [<span data-ttu-id="836cf-120">Grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="836cf-120">Resource group</span></span>](/azure/azure-resource-manager/resource-group-overview) | [<span data-ttu-id="836cf-121">az group</span><span class="sxs-lookup"><span data-stu-id="836cf-121">az group</span></span>](/cli/azure/group) |
| [<span data-ttu-id="836cf-122">Máquinas virtuais</span><span class="sxs-lookup"><span data-stu-id="836cf-122">Virtual machines</span></span>](/azure/virtual-machines) | [<span data-ttu-id="836cf-123">az vm</span><span class="sxs-lookup"><span data-stu-id="836cf-123">az vm</span></span>](/cli/azure/vm) |
| [<span data-ttu-id="836cf-124">Contas de armazenamento</span><span class="sxs-lookup"><span data-stu-id="836cf-124">Storage accounts</span></span>](/azure/storage/common/storage-introduction) | [<span data-ttu-id="836cf-125">az storage account</span><span class="sxs-lookup"><span data-stu-id="836cf-125">az storage account</span></span>](/cli/azure/storage/account) |
| [<span data-ttu-id="836cf-126">Key Vault</span><span class="sxs-lookup"><span data-stu-id="836cf-126">Key Vault</span></span>](/azure/key-vault/key-vault-whatis) | [<span data-ttu-id="836cf-127">az keyvault</span><span class="sxs-lookup"><span data-stu-id="836cf-127">az keyvault</span></span>](/cli/azure/keyvault) |
| [<span data-ttu-id="836cf-128">Aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="836cf-128">Web applications</span></span>](/azure/app-service) | [<span data-ttu-id="836cf-129">az webapp</span><span class="sxs-lookup"><span data-stu-id="836cf-129">az webapp</span></span>](/cli/azure/webapp) |
| [<span data-ttu-id="836cf-130">Bancos de dados SQL</span><span class="sxs-lookup"><span data-stu-id="836cf-130">SQL databases</span></span>](/azure/sql-database) | [<span data-ttu-id="836cf-131">az sql server</span><span class="sxs-lookup"><span data-stu-id="836cf-131">az sql server</span></span>](/cli/azure/sql/server) |
| [<span data-ttu-id="836cf-132">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="836cf-132">CosmosDB</span></span>](/azure/cosmos-db) | [<span data-ttu-id="836cf-133">az cosmosdb</span><span class="sxs-lookup"><span data-stu-id="836cf-133">az cosmosdb</span></span>](/cli/azure/cosmosdb) |

## <a name="finding-commands"></a><span data-ttu-id="836cf-134">Encontrando comandos</span><span class="sxs-lookup"><span data-stu-id="836cf-134">Finding commands</span></span>

<span data-ttu-id="836cf-135">Os comandos na CLI são organizados como _comandos_ de _grupos_.</span><span class="sxs-lookup"><span data-stu-id="836cf-135">Commands in the CLI are organized as _commands_ of _groups_.</span></span> <span data-ttu-id="836cf-136">Cada grupo representa um serviço do Azure e os comandos operam nesse serviço.</span><span class="sxs-lookup"><span data-stu-id="836cf-136">Each group represents an Azure service, and commands operate on that service.</span></span>

<span data-ttu-id="836cf-137">Para procurar comandos, use [az find](/cli/azure/reference-index#az-find).</span><span class="sxs-lookup"><span data-stu-id="836cf-137">To search for commands, use [az find](/cli/azure/reference-index#az-find).</span></span> <span data-ttu-id="836cf-138">Por exemplo, para procurar nomes de comando que contenham `secret`, use o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="836cf-138">For example, to search for command names containing `secret`, use the following command:</span></span>

```azurecli-interactive
az find -q secret
```

<span data-ttu-id="836cf-139">Use o argumento `--help` para obter uma lista completa de comandos e subgrupos de um grupo.</span><span class="sxs-lookup"><span data-stu-id="836cf-139">Use the `--help` argument to get a complete list of commands and subgroups of a group.</span></span> <span data-ttu-id="836cf-140">Por exemplo, para localizar os comandos da CLI para trabalhar com Grupos de Segurança de Rede (NSGs):</span><span class="sxs-lookup"><span data-stu-id="836cf-140">For example, to find the CLI commands for working with Network Security Groups (NSGs):</span></span>

```azurecli-interactive
az network nsg --help
```

<span data-ttu-id="836cf-141">A CLI tem o preenchimento completo de guia para comandos sob o shell do Bash.</span><span class="sxs-lookup"><span data-stu-id="836cf-141">The CLI has full tab completion for commands under the bash shell.</span></span>

## <a name="globally-available-arguments"></a><span data-ttu-id="836cf-142">Argumentos disponíveis globalmente</span><span class="sxs-lookup"><span data-stu-id="836cf-142">Globally available arguments</span></span>

<span data-ttu-id="836cf-143">Há alguns argumentos disponíveis para cada comando.</span><span class="sxs-lookup"><span data-stu-id="836cf-143">There are some arguments that are available for every command.</span></span>

* <span data-ttu-id="836cf-144">`--help` imprime as informações de referência da CLI sobre comandos e seus argumentos, além de listar os comandos e subgrupos disponíveis.</span><span class="sxs-lookup"><span data-stu-id="836cf-144">`--help` prints CLI reference information about commands and their arguments and lists available subgroups and commands.</span></span>
* <span data-ttu-id="836cf-145">`--output` altera o formato de saída.</span><span class="sxs-lookup"><span data-stu-id="836cf-145">`--output` changes the output format.</span></span> <span data-ttu-id="836cf-146">Os formatos de saída disponíveis são `json`, `jsonc`(JSON colorido), `tsv` (valores separados por tabulação), `table` (tabelas ASCII legível por humanos) e `yaml`.</span><span class="sxs-lookup"><span data-stu-id="836cf-146">The available output formats are `json`, `jsonc` (colorized JSON), `tsv` (Tab-Separated Values), `table` (human-readable ASCII tables), and `yaml`.</span></span> <span data-ttu-id="836cf-147">Por padrão, a CLI gera `json`.</span><span class="sxs-lookup"><span data-stu-id="836cf-147">By default the CLI outputs `json`.</span></span> <span data-ttu-id="836cf-148">Para saber mais sobre os formatos de saída disponíveis, confira [Formatos de saída da CLI do Azure](format-output-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="836cf-148">To learn more about the available output formats, see [Output formats for Azure CLI](format-output-azure-cli.md).</span></span>
* <span data-ttu-id="836cf-149">`--query` usa o [linguagem de consulta JMESPath](http://jmespath.org/) para filtrar a saída retornada dos serviços do Azure.</span><span class="sxs-lookup"><span data-stu-id="836cf-149">`--query` uses the [JMESPath query language](http://jmespath.org/) to filter the output returned from Azure services.</span></span> <span data-ttu-id="836cf-150">Para saber mais sobre as consultas, confira [Consultar resultados do comando com a CLI do Azure](query-azure-cli.md) e [Tutorial do JMESPath](http://jmespath.org/tutorial.html).</span><span class="sxs-lookup"><span data-stu-id="836cf-150">To learn more about queries, see [Query command results with Azure CLI](query-azure-cli.md) and the [JMESPath tutorial](http://jmespath.org/tutorial.html).</span></span>
* <span data-ttu-id="836cf-151">`--verbose` imprime informações sobre recursos criados no Azure durante uma operação, além de outras informações úteis.</span><span class="sxs-lookup"><span data-stu-id="836cf-151">`--verbose` prints information about resources created in Azure during an operation, and other useful information.</span></span>
* <span data-ttu-id="836cf-152">`--debug` imprime ainda mais informações sobre operações de CLI e é usado para fins de depuração.</span><span class="sxs-lookup"><span data-stu-id="836cf-152">`--debug` prints even more information about CLI operations, used for debugging purposes.</span></span> <span data-ttu-id="836cf-153">Se você encontrar um bug, forneça a saída gerada com o sinalizador `--debug` ao enviar um relatório de bugs.</span><span class="sxs-lookup"><span data-stu-id="836cf-153">If you find a bug, provide output generated with the `--debug` flag on when submitting a bug report.</span></span>

## <a name="interactive-mode"></a><span data-ttu-id="836cf-154">Modo interativo</span><span class="sxs-lookup"><span data-stu-id="836cf-154">Interactive mode</span></span>

<span data-ttu-id="836cf-155">A CLI oferece um modo interativo que exibe informações de ajuda automaticamente e torna mais fácil selecionar subcomandos.</span><span class="sxs-lookup"><span data-stu-id="836cf-155">The CLI offers an interactive mode that automatically displays help information and makes it easier to select subcommands.</span></span> <span data-ttu-id="836cf-156">Você entra no modo interativo com o comando [az interactive](/cli/azure/reference-index#az-interactive).</span><span class="sxs-lookup"><span data-stu-id="836cf-156">You enter interactive mode with the [az interactive](/cli/azure/reference-index#az-interactive) command.</span></span>

```azurecli-interactive
az interactive
```

<span data-ttu-id="836cf-157">Para obter mais informações sobre o modo interativo, confira [Modo interativo da CLI do Azure](interactive-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="836cf-157">For more information on interactive mode, see [Azure CLI Interactive Mode](interactive-azure-cli.md).</span></span>

<span data-ttu-id="836cf-158">Também há um [plug-in do Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli) que oferece uma experiência interativa, incluindo documentação de preenchimento automático e com o passar do mouse.</span><span class="sxs-lookup"><span data-stu-id="836cf-158">There's also a [Visual Studio Code plugin](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli) that offers an interactive experience, including autocomplete and mouse-over documentation.</span></span>

## <a name="learn-cli-basics-with-quickstarts-and-tutorials"></a><span data-ttu-id="836cf-159">Aprenda as noções básica da CLI com os guias de início rápido e tutoriais</span><span class="sxs-lookup"><span data-stu-id="836cf-159">Learn CLI basics with quickstarts and tutorials</span></span>

<span data-ttu-id="836cf-160">Para a introdução à CLI do Azure, experimente ver um tutorial aprofundado para configurar máquinas virtuais e usar o poder da CLI para consultar recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="836cf-160">To get you started with the Azure CLI, try an in-depth tutorial for setting up virtual machines and using the power of the CLI to query Azure resources.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="836cf-161">Tutorial Criar máquinas virtuais com a CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="836cf-161">Create virtual machines with the Azure CLI tutorial</span></span>](azure-cli-vm-tutorial.yml)

<span data-ttu-id="836cf-162">Também há guias de início rápido para outros serviços populares.</span><span class="sxs-lookup"><span data-stu-id="836cf-162">There are also quickstarts for other popular services.</span></span>

* [<span data-ttu-id="836cf-163">Criar uma conta de armazenamento usando a CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="836cf-163">Create a storage account using the Azure CLI</span></span>](/azure/storage/common/storage-quickstart-create-storage-account-cli)
* [<span data-ttu-id="836cf-164">Transferir objetos de/para o Armazenamento de blobs do Azure usando a CLI</span><span class="sxs-lookup"><span data-stu-id="836cf-164">Transfer objects to/from Azure Blob storage using the CLI</span></span>](/azure/storage/blobs/storage-quickstart-blobs-cli)
* [<span data-ttu-id="836cf-165">Criar um único banco de dados SQL do Azure usando a CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="836cf-165">Create a single Azure SQL database using the Azure CLI</span></span>](/azure/sql-database/sql-database-get-started-cli)
* [<span data-ttu-id="836cf-166">Criar um servidor de Banco de Dados do Azure para MySQL usando a CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="836cf-166">Create an Azure Database for MySQL server using the Azure CLI</span></span>](/azure/mysql/quickstart-create-mysql-server-database-using-azure-cli)
* [<span data-ttu-id="836cf-167">Criar um servidor de Banco de Dados do Azure para PostgreSQL usando a CLI Azure</span><span class="sxs-lookup"><span data-stu-id="836cf-167">Create an Azure Database for PostgreSQL using the Azure CLI</span></span>](/azure/postgresql/quickstart-create-server-database-azure-cli)
* [<span data-ttu-id="836cf-168">Criar um aplicativo Web do Python no Azure</span><span class="sxs-lookup"><span data-stu-id="836cf-168">Create a Python web app in Azure</span></span>](/azure/app-service/app-service-web-get-started-python)
* [<span data-ttu-id="836cf-169">Executar uma imagem personalizada do Hub do Docker nos Aplicativos Web para Contêineres do Azure</span><span class="sxs-lookup"><span data-stu-id="836cf-169">Run a custom Docker Hub image in Azure Web Apps for Containers</span></span>](/azure/app-service/containers/quickstart-custom-docker-image)

## <a name="give-feedback"></a><span data-ttu-id="836cf-170">Fornecer comentários</span><span class="sxs-lookup"><span data-stu-id="836cf-170">Give feedback</span></span>

<span data-ttu-id="836cf-171">Apreciamos seus comentários da CLI para ajudar-nos a melhorar e resolver bugs.</span><span class="sxs-lookup"><span data-stu-id="836cf-171">We welcome your feedback for the CLI to help us make improvements and resolve bugs.</span></span> <span data-ttu-id="836cf-172">Você pode [arquivar um problema no GitHub](https://github.com/azure/azure-cli/issues) ou usar os recursos internos da CLI para deixar um comentário geral com o comando [az feedback](/cli/azure/reference-index#az-feedback).</span><span class="sxs-lookup"><span data-stu-id="836cf-172">You can [file an issue on GitHub](https://github.com/azure/azure-cli/issues) or use the built-in features of the CLI to leave general feedback with the [az feedback](/cli/azure/reference-index#az-feedback) command.</span></span>

```azurecli-interactive
az feedback
```
