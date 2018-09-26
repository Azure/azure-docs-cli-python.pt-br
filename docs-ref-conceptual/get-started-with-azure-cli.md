---
title: Introdução à CLI do Azure 2.0
description: Comece a usar a CLI do Azure 2.0 aprendendo as noções básicas de comando.
keywords: CLI do Azure, ajuda da CLI, ajuda do Azure, consulta, automação,
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 00cfca8d55f0b404cae32ba9b4ce464dfa8afa08
ms.sourcegitcommit: 8318ce761c279afa4cd45a81a58d83fc38c616bc
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/13/2018
ms.locfileid: "45561568"
---
# <a name="get-started-with-azure-cli-20"></a><span data-ttu-id="18ba2-104">Introdução à CLI do Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="18ba2-104">Get started with Azure CLI 2.0</span></span>

<span data-ttu-id="18ba2-105">Bem-vindo à CLI do Azure 2.0!</span><span class="sxs-lookup"><span data-stu-id="18ba2-105">Welcome to the Azure CLI 2.0!</span></span> <span data-ttu-id="18ba2-106">A CLI é uma ferramenta projetada para ajudar você a trabalhar de forma rápida e eficaz com os serviços do Azure, com ênfase na automação.</span><span class="sxs-lookup"><span data-stu-id="18ba2-106">The CLI is a tool designed to get you working quickly and efficiently with Azure services, with an emphasis on automation.</span></span> <span data-ttu-id="18ba2-107">Este artigo apresenta recursos da CLI e links externos para recursos que ajudarão você a ser produtivo.</span><span class="sxs-lookup"><span data-stu-id="18ba2-107">This article introduces features of the CLI and links out to resources that help you be productive.</span></span>

## <a name="install-or-run-in-azure-cloud-shell"></a><span data-ttu-id="18ba2-108">Instalar ou executar no Azure Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="18ba2-108">Install or run in Azure Cloud Shell</span></span>

<span data-ttu-id="18ba2-109">A maneira mais fácil começar a usar a CLI do Azure é executando-a em um ambiente do Azure Cloud Shell por meio do seu navegador.</span><span class="sxs-lookup"><span data-stu-id="18ba2-109">The easiest way to get started with the Azure CLI is by running it in an Azure Cloud Shell environment through your browser.</span></span> <span data-ttu-id="18ba2-110">Para saber mais sobre o Cloud Shell, consulte [Início Rápido para Bash no Azure Cloud Shell](/azure/cloud-shell/quickstart).</span><span class="sxs-lookup"><span data-stu-id="18ba2-110">To learn about Cloud Shell, see  [Quickstart for Bash in Azure Cloud Shell](/azure/cloud-shell/quickstart).</span></span>

<span data-ttu-id="18ba2-111">Quando você estiver pronto para instalar a CLI, confira as [instruções de instalação](install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="18ba2-111">When you're ready to install the CLI, see the [installation instructions](install-azure-cli.md).</span></span>

## <a name="sign-in"></a><span data-ttu-id="18ba2-112">Entrar</span><span class="sxs-lookup"><span data-stu-id="18ba2-112">Sign in</span></span>

<span data-ttu-id="18ba2-113">Antes de usar os comandos da CLI com uma instalação local, é preciso entrar com [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="18ba2-113">Before using any CLI commands with a local install, you need to sign in with [az login](/cli/azure/reference-index#az-login).</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="18ba2-114">Há maneiras de entrar de modo não interativo, como mostrado em detalhes em [Entrar com a CLI do Azure 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="18ba2-114">There are ways to sign in non-interactively, which are covered in detail in [Sign in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="common-commands"></a><span data-ttu-id="18ba2-115">Comandos comuns</span><span class="sxs-lookup"><span data-stu-id="18ba2-115">Common commands</span></span>

<span data-ttu-id="18ba2-116">Esta tabela lista alguns comandos comuns usados na CLI e está vinculada à documentação de referência.</span><span class="sxs-lookup"><span data-stu-id="18ba2-116">This table lists some common commands used in the CLI and links to their reference documentation.</span></span>

| <span data-ttu-id="18ba2-117">Tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="18ba2-117">Resource type</span></span> | <span data-ttu-id="18ba2-118">Grupo de comando da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="18ba2-118">Azure CLI command group</span></span> |
|---------------|-------------------------|
| [<span data-ttu-id="18ba2-119">Grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="18ba2-119">Resource group</span></span>](/azure/azure-resource-manager/resource-group-overview) | [<span data-ttu-id="18ba2-120">az group</span><span class="sxs-lookup"><span data-stu-id="18ba2-120">az group</span></span>](/cli/azure/group) |
| [<span data-ttu-id="18ba2-121">Máquinas virtuais</span><span class="sxs-lookup"><span data-stu-id="18ba2-121">Virtual machines</span></span>](/azure/virtual-machines) | [<span data-ttu-id="18ba2-122">az vm</span><span class="sxs-lookup"><span data-stu-id="18ba2-122">az vm</span></span>](/cli/azure/vm) |
| [<span data-ttu-id="18ba2-123">Contas de armazenamento</span><span class="sxs-lookup"><span data-stu-id="18ba2-123">Storage accounts</span></span>](/azure/storage/common/storage-introduction) | [<span data-ttu-id="18ba2-124">az storage account</span><span class="sxs-lookup"><span data-stu-id="18ba2-124">az storage account</span></span>](/cli/azure/storage/account) |
| [<span data-ttu-id="18ba2-125">Key Vault</span><span class="sxs-lookup"><span data-stu-id="18ba2-125">Key Vault</span></span>](/azure/key-vault/key-vault-whatis) | [<span data-ttu-id="18ba2-126">az keyvault</span><span class="sxs-lookup"><span data-stu-id="18ba2-126">az keyvault</span></span>](/cli/azure/keyvault) |
| [<span data-ttu-id="18ba2-127">Aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="18ba2-127">Web applications</span></span>](/azure/app-service) | [<span data-ttu-id="18ba2-128">az webapp</span><span class="sxs-lookup"><span data-stu-id="18ba2-128">az webapp</span></span>](/cli/azure/webapp) |
| [<span data-ttu-id="18ba2-129">Bancos de dados SQL</span><span class="sxs-lookup"><span data-stu-id="18ba2-129">SQL databases</span></span>](/azure/sql-database) | [<span data-ttu-id="18ba2-130">az sql server</span><span class="sxs-lookup"><span data-stu-id="18ba2-130">az sql server</span></span>](/cli/azure/sql/server) |
| [<span data-ttu-id="18ba2-131">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="18ba2-131">CosmosDB</span></span>](/azure/cosmos-db) | [<span data-ttu-id="18ba2-132">az cosmosdb</span><span class="sxs-lookup"><span data-stu-id="18ba2-132">az cosmosdb</span></span>](/cli/azure/cosmosdb) |

## <a name="finding-commands"></a><span data-ttu-id="18ba2-133">Encontrando comandos</span><span class="sxs-lookup"><span data-stu-id="18ba2-133">Finding commands</span></span>

<span data-ttu-id="18ba2-134">Os comandos na CLI são organizados como _comandos_ de _grupos_.</span><span class="sxs-lookup"><span data-stu-id="18ba2-134">Commands in the CLI are organized as _commands_ of _groups_.</span></span> <span data-ttu-id="18ba2-135">Cada grupo representa um serviço do Azure e os comandos operam nesse serviço.</span><span class="sxs-lookup"><span data-stu-id="18ba2-135">Each group represents an Azure service, and commands operate on that service.</span></span>

<span data-ttu-id="18ba2-136">Para procurar comandos, use [az find](/cli/azure/reference-index#az-find).</span><span class="sxs-lookup"><span data-stu-id="18ba2-136">To search for commands, use [az find](/cli/azure/reference-index#az-find).</span></span> <span data-ttu-id="18ba2-137">Por exemplo, para procurar nomes de comando que contenham `secret`, use o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="18ba2-137">For example, to search for command names containing `secret`, use the following command:</span></span>

```azurecli-interactive
az find -q secret
```

<span data-ttu-id="18ba2-138">Use o argumento `--help` para obter uma lista completa de comandos e subgrupos de um grupo.</span><span class="sxs-lookup"><span data-stu-id="18ba2-138">Use the `--help` argument to get a complete list of commands and subgroups of a group.</span></span> <span data-ttu-id="18ba2-139">Por exemplo, para localizar os comandos da CLI para trabalhar com Grupos de Segurança de Rede (NSGs):</span><span class="sxs-lookup"><span data-stu-id="18ba2-139">For example, to find the CLI commands for working with Network Security Groups (NSGs):</span></span>

```azurecli-interactive
az network nsg --help
```

<span data-ttu-id="18ba2-140">A CLI tem o preenchimento completo de guia para comandos sob o shell do Bash.</span><span class="sxs-lookup"><span data-stu-id="18ba2-140">The CLI has full tab completion for commands under the bash shell.</span></span>

## <a name="globally-available-arguments"></a><span data-ttu-id="18ba2-141">Argumentos disponíveis globalmente</span><span class="sxs-lookup"><span data-stu-id="18ba2-141">Globally available arguments</span></span>

<span data-ttu-id="18ba2-142">Há alguns argumentos disponíveis para cada comando.</span><span class="sxs-lookup"><span data-stu-id="18ba2-142">There are some arguments that are available for every command.</span></span>

* <span data-ttu-id="18ba2-143">`--help` imprime as informações de referência da CLI sobre comandos e seus argumentos, além de listar os comandos e subgrupos disponíveis.</span><span class="sxs-lookup"><span data-stu-id="18ba2-143">`--help` prints CLI reference information about commands and their arguments and lists available subgroups and commands.</span></span>
* <span data-ttu-id="18ba2-144">`--output` altera o formato de saída.</span><span class="sxs-lookup"><span data-stu-id="18ba2-144">`--output` changes the output format.</span></span> <span data-ttu-id="18ba2-145">Os formatos de saída disponíveis são `json`, `jsonc`(JSON colorido), `tsv` (valores separados por tabulação) e `table` (tabelas ASCII legível por humanos).</span><span class="sxs-lookup"><span data-stu-id="18ba2-145">The available output formats are `json`, `jsonc` (colorized JSON), `tsv` (Tab-Separated Values), and `table` (human-readable ASCII tables).</span></span> <span data-ttu-id="18ba2-146">Por padrão, a CLI gera `json`.</span><span class="sxs-lookup"><span data-stu-id="18ba2-146">By default the CLI outputs `json`.</span></span> <span data-ttu-id="18ba2-147">Para saber mais sobre os formatos de saída disponível, consulte [Formatos de saída da CLI do Azure 2.0](format-output-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="18ba2-147">To learn more about the available output formats, see [Output formats for Azure CLI 2.0](format-output-azure-cli.md).</span></span>
* <span data-ttu-id="18ba2-148">`--query` usa o [linguagem de consulta JMESPath](http://jmespath.org/) para filtrar a saída retornada dos serviços do Azure.</span><span class="sxs-lookup"><span data-stu-id="18ba2-148">`--query` uses the [JMESPath query language](http://jmespath.org/) to filter the output returned from Azure services.</span></span> <span data-ttu-id="18ba2-149">Para saber mais sobre consultas, consulte [Consultar resultados do comando com a CLI do Azure 2.0](query-azure-cli.md) e [tutorial do JMESPath](http://jmespath.org/tutorial.html).</span><span class="sxs-lookup"><span data-stu-id="18ba2-149">To learn To learn more about queries, see [Query command results with Azure CLI 2.0](query-azure-cli.md) and the [JMESPath tutorial](http://jmespath.org/tutorial.html).</span></span>
* <span data-ttu-id="18ba2-150">`--verbose` imprime informações sobre recursos criados no Azure durante uma operação, além de outras informações úteis.</span><span class="sxs-lookup"><span data-stu-id="18ba2-150">`--verbose` prints information about resources created in Azure during an operation, and other useful information.</span></span>
* <span data-ttu-id="18ba2-151">`--debug` imprime ainda mais informações sobre operações de CLI e é usado para fins de depuração.</span><span class="sxs-lookup"><span data-stu-id="18ba2-151">`--debug` prints even more information about CLI operations, used for debugging purposes.</span></span> <span data-ttu-id="18ba2-152">Se você encontrar um bug, forneça a saída gerada com o sinalizador `--debug` ao enviar um relatório de bugs.</span><span class="sxs-lookup"><span data-stu-id="18ba2-152">If you find a bug, provide output generated with the `--debug` flag on when submitting a bug report.</span></span>

## <a name="interactive-mode"></a><span data-ttu-id="18ba2-153">Modo interativo</span><span class="sxs-lookup"><span data-stu-id="18ba2-153">Interactive mode</span></span>

<span data-ttu-id="18ba2-154">A CLI oferece um modo interativo que exibe informações de ajuda automaticamente e torna mais fácil selecionar subcomandos.</span><span class="sxs-lookup"><span data-stu-id="18ba2-154">The CLI offers an interactive mode that automatically displays help information and makes it easier to select subcommands.</span></span> <span data-ttu-id="18ba2-155">Você entra no modo interativo com o comando [az interactive](/cli/azure/reference-index#az-interactive).</span><span class="sxs-lookup"><span data-stu-id="18ba2-155">You enter interactive mode with the [az interactive](/cli/azure/reference-index#az-interactive) command.</span></span>

```azurecli-interactive
az interactive
```

<span data-ttu-id="18ba2-156">Para obter mais informações sobre o modo interativo, consulte [Modo Interativo da CLI 2.0 do Azure](interactive-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="18ba2-156">For more information on interactive mode, see [Azure CLI 2.0 Interactive Mode](interactive-azure-cli.md).</span></span>

<span data-ttu-id="18ba2-157">Também há um [plug-in do Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli) que oferece uma experiência interativa, incluindo documentação de preenchimento automático e com o passar do mouse.</span><span class="sxs-lookup"><span data-stu-id="18ba2-157">There's also a [Visual Studio Code plugin](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli) that offers an interactive experience, including autocomplete and mouse-over documentation.</span></span>

## <a name="learn-cli-basics-with-quickstarts-and-tutorials"></a><span data-ttu-id="18ba2-158">Aprenda as noções básica da CLI com os guias de início rápido e tutoriais</span><span class="sxs-lookup"><span data-stu-id="18ba2-158">Learn CLI basics with quickstarts and tutorials</span></span>

<span data-ttu-id="18ba2-159">Para a introdução à CLI do Azure 2.0, experimente ver um tutorial aprofundado para configurar máquinas virtuais e usar o poder da CLI para consultar recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="18ba2-159">To get you started with the Azure CLI 2.0, try an in-depth tutorial for setting up virtual machines and using the power of the CLI to query Azure resources.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="18ba2-160">Tutorial Criar máquinas virtuais com a CLI do Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="18ba2-160">Create virtual machines with the Azure CLI 2.0 tutorial</span></span>](azure-cli-vm-tutorial.yml)

<span data-ttu-id="18ba2-161">Também há guias de início rápido para outros serviços populares.</span><span class="sxs-lookup"><span data-stu-id="18ba2-161">There are also quickstarts for other popular services.</span></span>

* [<span data-ttu-id="18ba2-162">Criar uma conta de armazenamento usando a CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="18ba2-162">Create a storage account using the Azure CLI</span></span>](/azure/storage/common/storage-quickstart-create-storage-account-cli)
* [<span data-ttu-id="18ba2-163">Transferir objetos de/para o Armazenamento de blobs do Azure usando a CLI</span><span class="sxs-lookup"><span data-stu-id="18ba2-163">Transfer objects to/from Azure Blob storage using the CLI</span></span>](/azure/storage/blobs/storage-quickstart-blobs-cli)
* [<span data-ttu-id="18ba2-164">Criar um único banco de dados SQL do Azure usando a CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="18ba2-164">Create a single Azure SQL database using the Azure CLI</span></span>](/azure/sql-database/sql-database-get-started-cli)
* [<span data-ttu-id="18ba2-165">Criar um servidor de Banco de Dados do Azure para MySQL usando a CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="18ba2-165">Create an Azure Database for MySQL server using the Azure CLI</span></span>](/azure/mysql/quickstart-create-mysql-server-database-using-azure-cli)
* [<span data-ttu-id="18ba2-166">Criar um servidor de Banco de Dados do Azure para PostgreSQL usando a CLI Azure</span><span class="sxs-lookup"><span data-stu-id="18ba2-166">Create an Azure Database for PostgreSQL using the Azure CLI</span></span>](/azure/postgresql/quickstart-create-server-database-azure-cli)
* [<span data-ttu-id="18ba2-167">Criar um aplicativo Web do Python no Azure</span><span class="sxs-lookup"><span data-stu-id="18ba2-167">Create a Python web app in Azure</span></span>](/azure/app-service/app-service-web-get-started-python)
* [<span data-ttu-id="18ba2-168">Executar uma imagem personalizada do Hub do Docker nos Aplicativos Web para Contêineres do Azure</span><span class="sxs-lookup"><span data-stu-id="18ba2-168">Run a custom Docker Hub image in Azure Web Apps for Containers</span></span>](/azure/app-service/containers/quickstart-custom-docker-image)

## <a name="give-feedback"></a><span data-ttu-id="18ba2-169">Fornecer comentários</span><span class="sxs-lookup"><span data-stu-id="18ba2-169">Give feedback</span></span>

<span data-ttu-id="18ba2-170">Apreciamos seus comentários da CLI para ajudar-nos a melhorar e resolver bugs.</span><span class="sxs-lookup"><span data-stu-id="18ba2-170">We welcome your feedback for the CLI to help us make improvements and resolve bugs.</span></span> <span data-ttu-id="18ba2-171">Você pode [arquivar um problema no Github](https://github.com/azure/azure-cli/issues) ou usar os recursos internos da CLI para deixar um comentário geral com o comando [az feedback](/cli/azure/reference-index#az-feedback).</span><span class="sxs-lookup"><span data-stu-id="18ba2-171">You can [file an issue on Github](https://github.com/azure/azure-cli/issues) or use the built-in features of the CLI to leave general feedback with the [az feedback](/cli/azure/reference-index#az-feedback) command.</span></span>

```azurecli-interactive
az feedback
```
