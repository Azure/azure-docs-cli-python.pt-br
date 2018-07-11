---
title: Introdução à CLI do Azure 2.0
description: Comece a usar a CLI do Azure 2.0 aprendendo as noções básicas de comando.
keywords: CLI do Azure, ajuda da CLI, ajuda do Azure, consulta, automação,
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/16/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: c973d31312fbe0f9232bf3f0f3ed5f3b70b6559a
ms.sourcegitcommit: 308f9eb433a05b814999ac404f63d181169fffeb
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/03/2018
ms.locfileid: "37439934"
---
# <a name="get-started-with-azure-cli-20"></a><span data-ttu-id="05570-104">Introdução à CLI do Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="05570-104">Get started with Azure CLI 2.0</span></span>

<span data-ttu-id="05570-105">Bem-vindo à CLI do Azure 2.0!</span><span class="sxs-lookup"><span data-stu-id="05570-105">Welcome to the Azure CLI 2.0!</span></span> <span data-ttu-id="05570-106">A CLI é uma ferramenta projetada para ajudar você a trabalhar de forma rápida e eficaz com os serviços do Azure, com ênfase na automação.</span><span class="sxs-lookup"><span data-stu-id="05570-106">The CLI is a tool designed to get you working quickly and efficiently with Azure services, with an emphasis on automation.</span></span> <span data-ttu-id="05570-107">Este artigo apresenta recursos da CLI e links externos para recursos que ajudarão você a ser produtivo.</span><span class="sxs-lookup"><span data-stu-id="05570-107">This article introduces features of the CLI and links out to resources that help you be productive.</span></span>

## <a name="install-and-sign-in"></a><span data-ttu-id="05570-108">Instalar e entrar</span><span class="sxs-lookup"><span data-stu-id="05570-108">Install and sign in</span></span>

<span data-ttu-id="05570-109">Caso ainda não o tenha feito, [instale a CLI](install-azure-cli.md) ou experimento o [Azure Cloud Shell](/azure/cloud-shell/overview).</span><span class="sxs-lookup"><span data-stu-id="05570-109">If you haven't already, [install the CLI](install-azure-cli.md) or try out the [Azure Cloud Shell](/azure/cloud-shell/overview).</span></span>

<span data-ttu-id="05570-110">Antes de usar os comandos da CLI com uma instalação local, é preciso entrar com [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="05570-110">Before using any CLI commands with a local install, you need to sign in with [az login](/cli/azure/reference-index#az-login).</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="05570-111">Há maneiras de entrar de modo não interativo, o que é apresentado em detalhes em [Fazer logon com a CLI do Azure 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="05570-111">There are ways to sign in non-interactively, which are covered in detail in [Log in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="common-commands"></a><span data-ttu-id="05570-112">Comandos comuns</span><span class="sxs-lookup"><span data-stu-id="05570-112">Common commands</span></span>

<span data-ttu-id="05570-113">Esta tabela lista alguns dos comandos comuns usados nos links externos da CLI para suas páginas de documentação nas referências.</span><span class="sxs-lookup"><span data-stu-id="05570-113">This table lists a few of the common commands used in the CLI links out to their documentation pages in the reference.</span></span>
<span data-ttu-id="05570-114">Todos os subcomandos desses grupos e sua documentação podem ser pesquisados na referência online ou com o argumento `--help`.</span><span class="sxs-lookup"><span data-stu-id="05570-114">All subcommands of these groups and their documentation can be looked up in online reference or with the `--help` argument.</span></span>

| <span data-ttu-id="05570-115">Tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="05570-115">Resource type</span></span> | <span data-ttu-id="05570-116">Grupo de comando da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="05570-116">Azure CLI command group</span></span> |
|---------------|-------------------------|
| [<span data-ttu-id="05570-117">Grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="05570-117">Resource group</span></span>](/azure/azure-resource-manager/resource-group-overview) | [<span data-ttu-id="05570-118">az group</span><span class="sxs-lookup"><span data-stu-id="05570-118">az group</span></span>](/cli/azure/group) |
| [<span data-ttu-id="05570-119">Máquinas virtuais</span><span class="sxs-lookup"><span data-stu-id="05570-119">Virtual machines</span></span>](/azure/virtual-machines) | [<span data-ttu-id="05570-120">az vm</span><span class="sxs-lookup"><span data-stu-id="05570-120">az vm</span></span>](/cli/azure/vm) |
| [<span data-ttu-id="05570-121">Contas de armazenamento</span><span class="sxs-lookup"><span data-stu-id="05570-121">Storage accounts</span></span>](/azure/storage/common/storage-introduction) | [<span data-ttu-id="05570-122">az storage account</span><span class="sxs-lookup"><span data-stu-id="05570-122">az storage account</span></span>](/cli/azure/storage/account) |
| [<span data-ttu-id="05570-123">Key Vault</span><span class="sxs-lookup"><span data-stu-id="05570-123">Key Vault</span></span>](/azure/key-vault/key-vault-whatis) | [<span data-ttu-id="05570-124">az keyvault</span><span class="sxs-lookup"><span data-stu-id="05570-124">az keyvault</span></span>](/cli/azure/keyvault) |
| [<span data-ttu-id="05570-125">Aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="05570-125">Web applications</span></span>](/azure/app-service) | [<span data-ttu-id="05570-126">az webapp</span><span class="sxs-lookup"><span data-stu-id="05570-126">az webapp</span></span>](/cli/azure/webapp) |
| [<span data-ttu-id="05570-127">Bancos de dados SQL</span><span class="sxs-lookup"><span data-stu-id="05570-127">SQL databases</span></span>](/azure/sql-database) | [<span data-ttu-id="05570-128">az sql server</span><span class="sxs-lookup"><span data-stu-id="05570-128">az sql server</span></span>](/cli/azure/sql/server) |
| [<span data-ttu-id="05570-129">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="05570-129">CosmosDB</span></span>](/azure/cosmos-db) | [<span data-ttu-id="05570-130">az cosmosdb</span><span class="sxs-lookup"><span data-stu-id="05570-130">az cosmosdb</span></span>](/cli/azure/cosmosdb) |

## <a name="finding-commands"></a><span data-ttu-id="05570-131">Encontrando comandos</span><span class="sxs-lookup"><span data-stu-id="05570-131">Finding commands</span></span>

<span data-ttu-id="05570-132">Comandos na CLI são fornecidos como _subcomandos_ de _grupos_.</span><span class="sxs-lookup"><span data-stu-id="05570-132">Commands in the CLI are provided as _subcommands_ of _groups_.</span></span>
<span data-ttu-id="05570-133">Cada grupo representa um serviço fornecido pelo Azure, e os subgrupos dividem os comandos para esses serviços em agrupamentos lógicos.</span><span class="sxs-lookup"><span data-stu-id="05570-133">Each group represents a service provided by Azure, and the subgroups divide commands for these services into logical groupings.</span></span>

<span data-ttu-id="05570-134">Para procurar comandos, use [az find](/cli/azure/reference-index#az-find).</span><span class="sxs-lookup"><span data-stu-id="05570-134">To search for commands, use [az find](/cli/azure/reference-index#az-find).</span></span> <span data-ttu-id="05570-135">Por exemplo, para procurar nomes de comando que contenham `secret`, use o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="05570-135">For example, to search for command names containing `secret`, use the following command:</span></span>

```azurecli-interactive
az find -q secret
```

<span data-ttu-id="05570-136">Caso saiba com qual grupo de comandos deseja trabalhar, o argumento `--help` pode ser uma opção melhor.</span><span class="sxs-lookup"><span data-stu-id="05570-136">If you know which group of commands you want to work with, the `--help` argument may be a better choice.</span></span> <span data-ttu-id="05570-137">Ele exibe não apenas informações detalhadas de um comando, como também, quando usado com um grupo de comando, todos os subcomandos disponíveis.</span><span class="sxs-lookup"><span data-stu-id="05570-137">This displays not just detailed information for a command, but when used with a command group, displays all of the available subcommands.</span></span> <span data-ttu-id="05570-138">Por exemplo, ao trabalhar com Grupos de Segurança de Rede (NSGs), é possível encontrar os subgrupos de NSG e comandos disponíveis.</span><span class="sxs-lookup"><span data-stu-id="05570-138">For example, when working with Network Security Groups (NSGs) you can find the available NSG subgroups and commands.</span></span>

```azurecli-interactive
az network nsg --help
```

<span data-ttu-id="05570-139">A CLI tem o preenchimento completo de guia para comandos sob o shell do Bash.</span><span class="sxs-lookup"><span data-stu-id="05570-139">The CLI has full tab completion for commands under the bash shell.</span></span>

## <a name="globally-available-arguments"></a><span data-ttu-id="05570-140">Argumentos disponíveis globalmente</span><span class="sxs-lookup"><span data-stu-id="05570-140">Globally available arguments</span></span>

<span data-ttu-id="05570-141">Há alguns argumentos disponíveis para cada comando.</span><span class="sxs-lookup"><span data-stu-id="05570-141">There are some arguments that are available for every command.</span></span>

* <span data-ttu-id="05570-142">`--help` imprime as informações de referência da CLI sobre comandos e seus argumentos, além de listar os comandos e subgrupos disponíveis.</span><span class="sxs-lookup"><span data-stu-id="05570-142">`--help` prints CLI reference information about commands and their arguments and lists available subgroups and commands.</span></span>
* <span data-ttu-id="05570-143">`--output` altera o formato de saída.</span><span class="sxs-lookup"><span data-stu-id="05570-143">`--output` changes the output format.</span></span> <span data-ttu-id="05570-144">Os formatos de saída disponíveis são `json`, `jsonc`(JSON colorido), `tsv` (valores separados por tabulação) e `table` (tabelas ASCII legível por humanos).</span><span class="sxs-lookup"><span data-stu-id="05570-144">The available output formats are `json`, `jsonc` (colorized JSON), `tsv` (Tab-Separated Values), and `table` (human-readable ASCII tables).</span></span> <span data-ttu-id="05570-145">Por padrão, a CLI gera `json`.</span><span class="sxs-lookup"><span data-stu-id="05570-145">By default the CLI outputs `json`.</span></span> <span data-ttu-id="05570-146">Para saber mais sobre os formatos de saída disponível, consulte [Formatos de saída da CLI do Azure 2.0](format-output-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="05570-146">To learn more about the available output formats, see [Output formats for Azure CLI 2.0](format-output-azure-cli.md).</span></span>
* <span data-ttu-id="05570-147">`--query` usa o [linguagem de consulta JMESPath](http://jmespath.org/) para filtrar a saída retornada dos serviços do Azure.</span><span class="sxs-lookup"><span data-stu-id="05570-147">`--query` uses the [JMESPath query language](http://jmespath.org/) to filter the output returned from Azure services.</span></span> <span data-ttu-id="05570-148">Para saber mais sobre consultas, consulte [Consultar resultados do comando com a CLI do Azure 2.0](query-azure-cli.md) e [tutorial do JMESPath](http://jmespath.org/tutorial.html).</span><span class="sxs-lookup"><span data-stu-id="05570-148">To learn To learn more about queries, see [Query command results with Azure CLI 2.0](query-azure-cli.md) and the [JMESPath tutorial](http://jmespath.org/tutorial.html).</span></span>
* <span data-ttu-id="05570-149">`--verbose` imprime informações sobre recursos criados no Azure durante uma operação, além de outras informações úteis.</span><span class="sxs-lookup"><span data-stu-id="05570-149">`--verbose` prints information about resources created in Azure during an operation, and other useful information.</span></span>
* <span data-ttu-id="05570-150">`--debug` imprime ainda mais informações sobre operações de CLI e é usado para fins de depuração.</span><span class="sxs-lookup"><span data-stu-id="05570-150">`--debug` prints even more information about CLI operations, used for debugging purposes.</span></span> <span data-ttu-id="05570-151">Se você encontrar um bug, forneça a saída gerada com o sinalizador `--debug` ao enviar um relatório de bugs.</span><span class="sxs-lookup"><span data-stu-id="05570-151">If you encounter a bug, provide output generated with the `--debug` flag on when submitting a bug report.</span></span>


## <a name="interactive-mode"></a><span data-ttu-id="05570-152">Modo interativo</span><span class="sxs-lookup"><span data-stu-id="05570-152">Interactive mode</span></span>

<span data-ttu-id="05570-153">A CLI oferece um modo interativo que exibe informações de ajuda automaticamente e torna mais fácil selecionar subcomandos.</span><span class="sxs-lookup"><span data-stu-id="05570-153">The CLI offers an interactive mode that automatically displays help information and makes it easier to select subcommands.</span></span> <span data-ttu-id="05570-154">Você entra no modo interativo com o comando [az interactive](/cli/azure/reference-index#az-interactive).</span><span class="sxs-lookup"><span data-stu-id="05570-154">You enter interactive mode with the [az interactive](/cli/azure/reference-index#az-interactive) command.</span></span>

```azurecli-interactive
az interactive
```

<span data-ttu-id="05570-155">Para obter mais informações sobre o modo interativo, consulte [Modo Interativo da CLI 2.0 do Azure](interactive-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="05570-155">For more information on interactive mode, see [Azure CLI 2.0 Interactive Mode](interactive-azure-cli.md).</span></span>

<span data-ttu-id="05570-156">Também há um [Plug-in do Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli) que oferece uma experiência interativa, incluindo documentação de preenchimento automático e com o passar do mouse.</span><span class="sxs-lookup"><span data-stu-id="05570-156">There is also a [Visual Studio Code plugin](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli) that offers an interactive experience, including autocomplete and mouse-over documentation.</span></span>

## <a name="learn-cli-basics-with-quickstarts-and-tutorials"></a><span data-ttu-id="05570-157">Aprenda as noções básica da CLI com os guias de início rápido e tutoriais</span><span class="sxs-lookup"><span data-stu-id="05570-157">Learn CLI basics with quickstarts and tutorials</span></span>

<span data-ttu-id="05570-158">Para a introdução à CLI do Azure 2.0, experimente ver um tutorial aprofundado para configurar máquinas virtuais e usar o poder da CLI para consultar recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="05570-158">To get you started with the Azure CLI 2.0, try an in-depth tutorial for setting up virtual machines and using the power of the CLI to query Azure resources.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="05570-159">Tutorial Criar máquinas virtuais com a CLI do Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="05570-159">Create virtual machines with the Azure CLI 2.0 tutorial</span></span>](azure-cli-vm-tutorial.yml)

<span data-ttu-id="05570-160">Se você preferir se concentrar em outros serviços, há uma variedade de guias de início rápido para os serviços do Azure que usam a CLI.</span><span class="sxs-lookup"><span data-stu-id="05570-160">If you would rather focus on other services, there are a variety of quickstarts for Azure services that use the CLI.</span></span>

* [<span data-ttu-id="05570-161">Criar uma conta de armazenamento usando a CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="05570-161">Create a storage account using the Azure CLI</span></span>](/azure/storage/common/storage-quickstart-create-storage-account-cli)
* [<span data-ttu-id="05570-162">Transferir objetos de/para o Armazenamento de blobs do Azure usando a CLI</span><span class="sxs-lookup"><span data-stu-id="05570-162">Transfer objects to/from Azure Blob storage using the CLI</span></span>](/azure/storage/blobs/storage-quickstart-blobs-cli)
* [<span data-ttu-id="05570-163">Criar um único banco de dados SQL do Azure usando a CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="05570-163">Create a single Azure SQL database using the Azure CLI</span></span>](/azure/sql-database/sql-database-get-started-cli)
* [<span data-ttu-id="05570-164">Criar um servidor de Banco de Dados do Azure para MySQL usando a CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="05570-164">Create an Azure Database for MySQL server using the Azure CLI</span></span>](/azure/mysql/quickstart-create-mysql-server-database-using-azure-cli)
* [<span data-ttu-id="05570-165">Criar um servidor de Banco de Dados do Azure para PostgreSQL usando a CLI Azure</span><span class="sxs-lookup"><span data-stu-id="05570-165">Create an Azure Database for PostgreSQL using the Azure CLI</span></span>](/azure/postgresql/quickstart-create-server-database-azure-cli)
* [<span data-ttu-id="05570-166">Criar um aplicativo Web do Python no Azure</span><span class="sxs-lookup"><span data-stu-id="05570-166">Create a Python web app in Azure</span></span>](/azure/app-service/app-service-web-get-started-python)
* [<span data-ttu-id="05570-167">Executar uma imagem personalizada do Hub do Docker nos Aplicativos Web para Contêineres do Azure</span><span class="sxs-lookup"><span data-stu-id="05570-167">Run a custom Docker Hub image in Azure Web Apps for Containers</span></span>](/azure/app-service/containers/quickstart-custom-docker-image)

## <a name="give-feedback"></a><span data-ttu-id="05570-168">Fornecer comentários</span><span class="sxs-lookup"><span data-stu-id="05570-168">Give feedback</span></span>

<span data-ttu-id="05570-169">Apreciamos seus comentários da CLI para ajudar-nos a melhorar e resolver bugs.</span><span class="sxs-lookup"><span data-stu-id="05570-169">We welcome your feedback for the CLI to help us make improvements and resolve bugs.</span></span> <span data-ttu-id="05570-170">Você pode [arquivar um problema no Github](https://github.com/azure/azure-cli/issues) ou usar os recursos internos da CLI para deixar um comentário geral com o comando [az feedback](/cli/azure/reference-index#az-feedback).</span><span class="sxs-lookup"><span data-stu-id="05570-170">You can [file an issue on Github](https://github.com/azure/azure-cli/issues) or use the built-in features of the CLI to leave general feedback with the [az feedback](/cli/azure/reference-index#az-feedback) command.</span></span>

```azurecli-interactive
az feedback
```
