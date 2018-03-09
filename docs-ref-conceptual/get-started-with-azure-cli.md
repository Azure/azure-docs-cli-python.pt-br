---
title: "Introdução à CLI do Azure 2.0"
description: "Comece a usar a CLI do Azure 2.0 aprendendo as noções básicas de comando."
keywords: "CLI do Azure, ajuda da CLI, ajuda do Azure, consulta, automação,"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 02/05/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 3f5fe1b01a8ce691846126a6c03e7222e9b20e0d
ms.sourcegitcommit: 29d7366a0902488f4f4d39c2cb0e89368d5186ea
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2018
---
# <a name="get-started-with-azure-cli-20"></a><span data-ttu-id="c766a-104">Introdução à CLI do Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="c766a-104">Get started with Azure CLI 2.0</span></span>

<span data-ttu-id="c766a-105">Bem-vindo à CLI do Azure 2.0!</span><span class="sxs-lookup"><span data-stu-id="c766a-105">Welcome to the Azure CLI 2.0!</span></span> <span data-ttu-id="c766a-106">A CLI é uma ferramenta projetada para ajudar você a trabalhar de forma rápida e eficaz com os serviços do Azure, com ênfase na automação.</span><span class="sxs-lookup"><span data-stu-id="c766a-106">The CLI is a tool designed to get you working quickly and efficiently with Azure services, with an emphasis on automation.</span></span> <span data-ttu-id="c766a-107">Este artigo apresenta recursos da CLI e links externos para recursos que ajudarão você a ser produtivo.</span><span class="sxs-lookup"><span data-stu-id="c766a-107">This article introduces features of the CLI and links out to resources that help you be productive.</span></span>

## <a name="install-and-log-in"></a><span data-ttu-id="c766a-108">Instalar e fazer logon</span><span class="sxs-lookup"><span data-stu-id="c766a-108">Install and log in</span></span>

<span data-ttu-id="c766a-109">Caso ainda não o tenha feito, [instale a CLI](install-azure-cli.md) ou experimento o [Azure Cloud Shell](/azure/cloud-shell/overview).</span><span class="sxs-lookup"><span data-stu-id="c766a-109">If you haven't already, [install the CLI](install-azure-cli.md) or try out the [Azure Cloud Shell](/azure/cloud-shell/overview).</span></span>

<span data-ttu-id="c766a-110">Antes de usar os comandos da CLI com uma instalação local, é preciso fazer logon com [az login](/cli/azure/reference-index#az_login).</span><span class="sxs-lookup"><span data-stu-id="c766a-110">Before using any CLI commands with a local install, you need to log in with [az login](/cli/azure/reference-index#az_login).</span></span>

```azurecli
az login
```

<span data-ttu-id="c766a-111">Esse prompt de comando faz com que você faça logon com um código de autenticação por meio de um site.</span><span class="sxs-lookup"><span data-stu-id="c766a-111">This command prompts you to log in with an authentication code via a website.</span></span> <span data-ttu-id="c766a-112">Há maneiras de fazer logon não interativamente, o que é apresentado em detalhes em [Fazer logon com a CLI do Azure 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="c766a-112">There are ways to log in non-interactively, which are covered in detail in [Log in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="common-commands"></a><span data-ttu-id="c766a-113">Comandos comuns</span><span class="sxs-lookup"><span data-stu-id="c766a-113">Common commands</span></span>

<span data-ttu-id="c766a-114">Esta tabela lista alguns dos comandos comuns usados nos links externos da CLI para suas páginas de documentação nas referências.</span><span class="sxs-lookup"><span data-stu-id="c766a-114">This table lists a few of the common commands used in the CLI links out to their documentation pages in the reference.</span></span>
<span data-ttu-id="c766a-115">Todos os subcomandos desses grupos e sua documentação podem ser pesquisados na referência online ou com o argumento `--help`.</span><span class="sxs-lookup"><span data-stu-id="c766a-115">All subcommands of these groups and their documentation can be looked up in online reference or with the `--help` argument.</span></span>

| <span data-ttu-id="c766a-116">Tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="c766a-116">Resource type</span></span> | <span data-ttu-id="c766a-117">Grupo de comando da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="c766a-117">Azure CLI command group</span></span> |
|---------------|-------------------------|
| [<span data-ttu-id="c766a-118">Grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="c766a-118">Resource group</span></span>](/azure/azure-resource-manager/resource-group-overview) | [<span data-ttu-id="c766a-119">az group</span><span class="sxs-lookup"><span data-stu-id="c766a-119">az group</span></span>](/cli/azure/group) |
| [<span data-ttu-id="c766a-120">Máquinas virtuais</span><span class="sxs-lookup"><span data-stu-id="c766a-120">Virtual machines</span></span>](/azure/virtual-machines) | [<span data-ttu-id="c766a-121">az vm</span><span class="sxs-lookup"><span data-stu-id="c766a-121">az vm</span></span>](/cli/azure/vm) |
| [<span data-ttu-id="c766a-122">Contas de armazenamento</span><span class="sxs-lookup"><span data-stu-id="c766a-122">Storage accounts</span></span>](/azure/storage/common/storage-introduction) | [<span data-ttu-id="c766a-123">az storage account</span><span class="sxs-lookup"><span data-stu-id="c766a-123">az storage account</span></span>](/cli/azure/storage/account) |
| [<span data-ttu-id="c766a-124">Key Vault</span><span class="sxs-lookup"><span data-stu-id="c766a-124">Key Vault</span></span>](/azure/key-vault/key-vault-whatis) | [<span data-ttu-id="c766a-125">az keyvault</span><span class="sxs-lookup"><span data-stu-id="c766a-125">az keyvault</span></span>](/cli/azure/keyvault) |
| [<span data-ttu-id="c766a-126">Aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="c766a-126">Web applications</span></span>](/azure/ap-service) | [<span data-ttu-id="c766a-127">az webapp</span><span class="sxs-lookup"><span data-stu-id="c766a-127">az webapp</span></span>](/cli/azure/webapp) |
| [<span data-ttu-id="c766a-128">Bancos de dados SQL</span><span class="sxs-lookup"><span data-stu-id="c766a-128">SQL databases</span></span>](/azure/sql-database) | [<span data-ttu-id="c766a-129">az sql server</span><span class="sxs-lookup"><span data-stu-id="c766a-129">az sql server</span></span>](/cli/azure/sql/server) |
| [<span data-ttu-id="c766a-130">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="c766a-130">CosmosDB</span></span>](/azure/cosmos-db) | [<span data-ttu-id="c766a-131">az cosmosdb</span><span class="sxs-lookup"><span data-stu-id="c766a-131">az cosmosdb</span></span>](/cli/azure/cosmosdb) |

## <a name="finding-commands"></a><span data-ttu-id="c766a-132">Encontrando comandos</span><span class="sxs-lookup"><span data-stu-id="c766a-132">Finding commands</span></span>

<span data-ttu-id="c766a-133">Comandos na CLI são fornecidos como _subcomandos_ de _grupos_.</span><span class="sxs-lookup"><span data-stu-id="c766a-133">Commands in the CLI are provided as _subcommands_ of _groups_.</span></span>
<span data-ttu-id="c766a-134">Cada grupo representa um serviço fornecido pelo Azure, e os subgrupos dividem os comandos para esses serviços em agrupamentos lógicos.</span><span class="sxs-lookup"><span data-stu-id="c766a-134">Each group represents a service provided by Azure, and the subgroups divide commands for these services into logical groupings.</span></span>

<span data-ttu-id="c766a-135">Para procurar comandos, use [az find](/cli/azure/reference-index#az_find).</span><span class="sxs-lookup"><span data-stu-id="c766a-135">To search for commands, use [az find](/cli/azure/reference-index#az_find).</span></span> <span data-ttu-id="c766a-136">Por exemplo, para procurar nomes de comando que contenham `secret`, use o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="c766a-136">For example, to search for command names containing `secret`, use the following command:</span></span>

```azurecli
az find -q secret
```

<span data-ttu-id="c766a-137">Caso saiba com qual grupo de comandos deseja trabalhar, o argumento `--help` pode ser uma opção melhor.</span><span class="sxs-lookup"><span data-stu-id="c766a-137">If you know which group of commands you want to work with, the `--help` argument may be a better choice.</span></span> <span data-ttu-id="c766a-138">Ele exibe não apenas informações detalhadas de um comando, como também, quando usado com um grupo de comando, todos os subcomandos disponíveis.</span><span class="sxs-lookup"><span data-stu-id="c766a-138">This displays not just detailed information for a command, but when used with a command group, displays all of the available subcommands.</span></span> <span data-ttu-id="c766a-139">Por exemplo, ao trabalhar com Grupos de Segurança de Rede (NSGs), é possível encontrar os subgrupos de NSG e comandos disponíveis.</span><span class="sxs-lookup"><span data-stu-id="c766a-139">For example, when working with Network Security Groups (NSGs) you can find the available NSG subgroups and commands.</span></span>

```azurecli
az network nsg --help
```

<span data-ttu-id="c766a-140">A CLI tem o preenchimento completo de guia para comandos sob o shell do Bash.</span><span class="sxs-lookup"><span data-stu-id="c766a-140">The CLI has full tab completion for commands under the bash shell.</span></span>

## <a name="globally-available-arguments"></a><span data-ttu-id="c766a-141">Argumentos disponíveis globalmente</span><span class="sxs-lookup"><span data-stu-id="c766a-141">Globally available arguments</span></span>

<span data-ttu-id="c766a-142">Há alguns argumentos disponíveis para cada comando.</span><span class="sxs-lookup"><span data-stu-id="c766a-142">There are some arguments that are available for every command.</span></span>

* <span data-ttu-id="c766a-143">`--help` imprime as informações de referência da CLI sobre comandos e seus argumentos, além de listar os comandos e subgrupos disponíveis.</span><span class="sxs-lookup"><span data-stu-id="c766a-143">`--help` prints CLI reference information about commands and their arguments and lists available subgroups and commands.</span></span>
* <span data-ttu-id="c766a-144">`--output` altera o formato de saída.</span><span class="sxs-lookup"><span data-stu-id="c766a-144">`--output` changes the output format.</span></span> <span data-ttu-id="c766a-145">Os formatos de saída disponíveis são `json`, `jsonc`(JSON colorido), `tsv` (valores separados por tabulação) e `table` (tabelas ASCII legível por humanos).</span><span class="sxs-lookup"><span data-stu-id="c766a-145">The available output formats are `json`, `jsonc` (colorized JSON), `tsv` (Tab-Separated Values), and `table` (human-readable ASCII tables).</span></span> <span data-ttu-id="c766a-146">Por padrão, a CLI gera `json`.</span><span class="sxs-lookup"><span data-stu-id="c766a-146">By default the CLI outputs `json`.</span></span> <span data-ttu-id="c766a-147">Para saber mais sobre os formatos de saída disponível, consulte [Formatos de saída da CLI do Azure 2.0](format-output-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="c766a-147">To learn more about the available output formats, see [Output formats for Azure CLI 2.0](format-output-azure-cli.md).</span></span>
* <span data-ttu-id="c766a-148">`--query` usa o [linguagem de consulta JMESPath](http://jmespath.org/) para filtrar a saída retornada dos serviços do Azure.</span><span class="sxs-lookup"><span data-stu-id="c766a-148">`--query` uses the [JMESPath query language](http://jmespath.org/) to filter the output returned from Azure services.</span></span> <span data-ttu-id="c766a-149">Para saber mais sobre consultas, consulte [Consultar resultados do comando com a CLI do Azure 2.0](query-azure-cli.md) e [tutorial do JMESPath](http://jmespath.org/tutorial.html).</span><span class="sxs-lookup"><span data-stu-id="c766a-149">To learn To learn more about queries, see [Query command results with Azure CLI 2.0](query-azure-cli.md) and the [JMESPath tutorial](http://jmespath.org/tutorial.html).</span></span>
* <span data-ttu-id="c766a-150">`--verbose` imprime informações sobre recursos criados no Azure durante uma operação, além de outras informações úteis.</span><span class="sxs-lookup"><span data-stu-id="c766a-150">`--verbose` prints information about resources created in Azure during an operation, and other useful information.</span></span>
* <span data-ttu-id="c766a-151">`--debug` imprime ainda mais informações sobre operações de CLI e é usado para fins de depuração.</span><span class="sxs-lookup"><span data-stu-id="c766a-151">`--debug` prints even more information about CLI operations, used for debugging purposes.</span></span> <span data-ttu-id="c766a-152">Se você encontrar um bug, forneça a saída gerada com o sinalizador `--debug` ao enviar um relatório de bugs.</span><span class="sxs-lookup"><span data-stu-id="c766a-152">If you encounter a bug, provide output generated with the `--debug` flag on when submitting a bug report.</span></span>


## <a name="interactive-mode"></a><span data-ttu-id="c766a-153">Modo interativo</span><span class="sxs-lookup"><span data-stu-id="c766a-153">Interactive mode</span></span>

<span data-ttu-id="c766a-154">A CLI oferece um modo interativo que exibe informações de ajuda automaticamente e torna mais fácil selecionar subcomandos.</span><span class="sxs-lookup"><span data-stu-id="c766a-154">The CLI offers an interactive mode that automatically displays help information and makes it easier to select subcommands.</span></span> <span data-ttu-id="c766a-155">Você entra no modo interativo com o comando `az interactive`.</span><span class="sxs-lookup"><span data-stu-id="c766a-155">You enter interactive mode with the `az interactive` command.</span></span> <span data-ttu-id="c766a-156">Para obter mais informações sobre o modo interativo e como ele ajuda você a aprender sobre a CLI, consulte [Modo interativo da CLI do Azure 2.0](interactive-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="c766a-156">For more information on interactive mode and how it helps you learn the CLI, see [Azure CLI 2.0 Interactive Mode](interactive-azure-cli.md).</span></span>

<span data-ttu-id="c766a-157">Também há um [Plug-in do Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli) que oferece uma experiência interativa, incluindo documentação de preenchimento automático e com o passar do mouse.</span><span class="sxs-lookup"><span data-stu-id="c766a-157">There is also a [Visual Studio Code plugin](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli) that offers an interactive experience, including autocomplete and mouse-over documentation.</span></span>



## <a name="learn-cli-basics-with-quickstarts-and-tutorials"></a><span data-ttu-id="c766a-158">Aprenda as noções básica da CLI com os guias de início rápido e tutoriais</span><span class="sxs-lookup"><span data-stu-id="c766a-158">Learn CLI basics with quickstarts and tutorials</span></span>

<span data-ttu-id="c766a-159">Para a introdução à CLI do Azure 2.0, experimente ver um tutorial aprofundado para configurar máquinas virtuais e usar o poder da CLI para consultar recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="c766a-159">To get you started with the Azure CLI 2.0, try an in-depth tutorial for setting up virtual machines and using the power of the CLI to query Azure resources.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="c766a-160">Tutorial Criar máquinas virtuais com a CLI do Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="c766a-160">Create virtual machines with the Azure CLI 2.0 tutorial</span></span>](azure-cli-vm-tutorial.yml)

<span data-ttu-id="c766a-161">Se você preferir se concentrar em outros serviços, há uma variedade de guias de início rápido para os serviços do Azure que usam a CLI.</span><span class="sxs-lookup"><span data-stu-id="c766a-161">If you would rather focus on other services, there are a variety of quickstarts for Azure services that use the CLI.</span></span>

* [<span data-ttu-id="c766a-162">Criar uma conta de armazenamento usando a CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="c766a-162">Create a storage account using the Azure CLI</span></span>](/azure/storage/common/storage-quickstart-create-storage-account-cli)
* [<span data-ttu-id="c766a-163">Transferir objetos de/para o Armazenamento de blobs do Azure usando a CLI</span><span class="sxs-lookup"><span data-stu-id="c766a-163">Transfer objects to/from Azure Blob storage using the CLI</span></span>](/azure/storage/blobs/storage-quickstart-blobs-cli)
* [<span data-ttu-id="c766a-164">Criar um único banco de dados SQL do Azure usando a CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="c766a-164">Create a single Azure SQL database using the Azure CLI</span></span>](/azure/sql-database/sql-database-get-started-cli)
* [<span data-ttu-id="c766a-165">Criar um servidor de Banco de Dados do Azure para MySQL usando a CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="c766a-165">Create an Azure Database for MySQL server using the Azure CLI</span></span>](/azure/mysql/quickstart-create-mysql-server-database-using-azure-cli)
* [<span data-ttu-id="c766a-166">Criar um servidor de Banco de Dados do Azure para PostgreSQL usando a CLI Azure</span><span class="sxs-lookup"><span data-stu-id="c766a-166">Create an Azure Database for PostgreSQL using the Azure CLI</span></span>](/azure/postgresql/quickstart-create-server-database-azure-cli)
* [<span data-ttu-id="c766a-167">Criar um aplicativo Web do Python no Azure</span><span class="sxs-lookup"><span data-stu-id="c766a-167">Create a Python web app in Azure</span></span>](/azure/app-service/app-service-web-get-started-python)
* [<span data-ttu-id="c766a-168">Executar uma imagem personalizada do Hub do Docker nos Aplicativos Web para Contêineres do Azure</span><span class="sxs-lookup"><span data-stu-id="c766a-168">Run a custom Docker Hub image in Azure Web Apps for Containers</span></span>](/azure/app-service/containers/quickstart-custom-docker-image)

## <a name="give-feedback"></a><span data-ttu-id="c766a-169">Fornecer comentários</span><span class="sxs-lookup"><span data-stu-id="c766a-169">Give feedback</span></span>

<span data-ttu-id="c766a-170">Apreciamos seus comentários da CLI para ajudar-nos a melhorar e resolver bugs.</span><span class="sxs-lookup"><span data-stu-id="c766a-170">We welcome your feedback for the CLI to help us make improvements and resolve bugs.</span></span> <span data-ttu-id="c766a-171">Você pode [arquivar um problema no Github](https://github.com/azure/azure-cli/issues) ou usar os recursos internos da CLI para deixar um comentário geral com o comando `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="c766a-171">You can [file an issue on Github](https://github.com/azure/azure-cli/issues) or use the built-in features of the CLI to leave general feedback with the `az feedback` command.</span></span>

```azurecli
az feedback
```
