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
ms.openlocfilehash: a56ce4acf070c17d8deaec9674593ba930cca70f
ms.sourcegitcommit: f40bd067ece4e6ec13e259782ed8db3e33b61a75
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "53593601"
---
# <a name="get-started-with-azure-cli"></a>Introdução à CLI do Azure

Bem-vindo à CLI do Azure! A CLI é uma ferramenta projetada para ajudar você a trabalhar de forma rápida e eficaz com os serviços do Azure, com ênfase na automação. Este artigo apresenta recursos da CLI e links externos para recursos que ajudarão você a ser produtivo.

## <a name="install-or-run-in-azure-cloud-shell"></a>Instalar ou executar no Azure Cloud Shell

A maneira mais fácil começar a usar a CLI do Azure é executando-a em um ambiente do Azure Cloud Shell por meio do seu navegador. Para saber mais sobre o Cloud Shell, consulte [Início Rápido para Bash no Azure Cloud Shell](/azure/cloud-shell/quickstart).

Quando você estiver pronto para instalar a CLI, confira as [instruções de instalação](install-azure-cli.md).

## <a name="sign-in"></a>Entrar

Antes de usar os comandos da CLI com uma instalação local, é preciso entrar com [az login](/cli/azure/reference-index#az-login).

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Há maneiras de entrar de modo não interativo, como mostrado em detalhes em [Entrar com a CLI do Azure](authenticate-azure-cli.md).

## <a name="common-commands"></a>Comandos comuns

Esta tabela lista alguns comandos comuns usados na CLI e está vinculada à documentação de referência.

| Tipo de recurso | Grupo de comando da CLI do Azure |
|---------------|-------------------------|
| [Grupo de recursos](/azure/azure-resource-manager/resource-group-overview) | [az group](/cli/azure/group) |
| [Máquinas virtuais](/azure/virtual-machines) | [az vm](/cli/azure/vm) |
| [Contas de armazenamento](/azure/storage/common/storage-introduction) | [az storage account](/cli/azure/storage/account) |
| [Key Vault](/azure/key-vault/key-vault-whatis) | [az keyvault](/cli/azure/keyvault) |
| [Aplicativos Web](/azure/app-service) | [az webapp](/cli/azure/webapp) |
| [Bancos de dados SQL](/azure/sql-database) | [az sql server](/cli/azure/sql/server) |
| [CosmosDB](/azure/cosmos-db) | [az cosmosdb](/cli/azure/cosmosdb) |

## <a name="finding-commands"></a>Encontrando comandos

Os comandos na CLI são organizados como _comandos_ de _grupos_. Cada grupo representa um serviço do Azure e os comandos operam nesse serviço.

Para procurar comandos, use [az find](/cli/azure/reference-index#az-find). Por exemplo, para procurar nomes de comando que contenham `secret`, use o seguinte comando:

```azurecli-interactive
az find -q secret
```

Use o argumento `--help` para obter uma lista completa de comandos e subgrupos de um grupo. Por exemplo, para localizar os comandos da CLI para trabalhar com Grupos de Segurança de Rede (NSGs):

```azurecli-interactive
az network nsg --help
```

A CLI tem o preenchimento completo de guia para comandos sob o shell do Bash.

## <a name="globally-available-arguments"></a>Argumentos disponíveis globalmente

Há alguns argumentos disponíveis para cada comando.

* `--help` imprime as informações de referência da CLI sobre comandos e seus argumentos, além de listar os comandos e subgrupos disponíveis.
* `--output` altera o formato de saída. Os formatos de saída disponíveis são `json`, `jsonc`(JSON colorido), `tsv` (valores separados por tabulação) e `table` (tabelas ASCII legível por humanos). Por padrão, a CLI gera `json`. Para saber mais sobre os formatos de saída disponíveis, confira [Formatos de saída da CLI do Azure](format-output-azure-cli.md).
* `--query` usa o [linguagem de consulta JMESPath](http://jmespath.org/) para filtrar a saída retornada dos serviços do Azure. Para saber mais sobre confira, confira [Consultar resultados do comando com a CLI do Azure](query-azure-cli.md) e [Tutorial do JMESPath](http://jmespath.org/tutorial.html).
* `--verbose` imprime informações sobre recursos criados no Azure durante uma operação, além de outras informações úteis.
* `--debug` imprime ainda mais informações sobre operações de CLI e é usado para fins de depuração. Se você encontrar um bug, forneça a saída gerada com o sinalizador `--debug` ao enviar um relatório de bugs.

## <a name="interactive-mode"></a>Modo interativo

A CLI oferece um modo interativo que exibe informações de ajuda automaticamente e torna mais fácil selecionar subcomandos. Você entra no modo interativo com o comando [az interactive](/cli/azure/reference-index#az-interactive).

```azurecli-interactive
az interactive
```

Para obter mais informações sobre o modo interativo, confira [Modo interativo da CLI do Azure](interactive-azure-cli.md).

Também há um [plug-in do Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli) que oferece uma experiência interativa, incluindo documentação de preenchimento automático e com o passar do mouse.

## <a name="learn-cli-basics-with-quickstarts-and-tutorials"></a>Aprenda as noções básica da CLI com os guias de início rápido e tutoriais

Para a introdução à CLI do Azure, experimente ver um tutorial aprofundado para configurar máquinas virtuais e usar o poder da CLI para consultar recursos do Azure.

> [!div class="nextstepaction"]
> [Tutorial Criar máquinas virtuais com a CLI do Azure](azure-cli-vm-tutorial.yml)

Também há guias de início rápido para outros serviços populares.

* [Criar uma conta de armazenamento usando a CLI do Azure](/azure/storage/common/storage-quickstart-create-storage-account-cli)
* [Transferir objetos de/para o Armazenamento de blobs do Azure usando a CLI](/azure/storage/blobs/storage-quickstart-blobs-cli)
* [Criar um único banco de dados SQL do Azure usando a CLI do Azure](/azure/sql-database/sql-database-get-started-cli)
* [Criar um servidor de Banco de Dados do Azure para MySQL usando a CLI do Azure](/azure/mysql/quickstart-create-mysql-server-database-using-azure-cli)
* [Criar um servidor de Banco de Dados do Azure para PostgreSQL usando a CLI Azure](/azure/postgresql/quickstart-create-server-database-azure-cli)
* [Criar um aplicativo Web do Python no Azure](/azure/app-service/app-service-web-get-started-python)
* [Executar uma imagem personalizada do Hub do Docker nos Aplicativos Web para Contêineres do Azure](/azure/app-service/containers/quickstart-custom-docker-image)

## <a name="give-feedback"></a>Fornecer comentários

Apreciamos seus comentários da CLI para ajudar-nos a melhorar e resolver bugs. Você pode [arquivar um problema no Github](https://github.com/azure/azure-cli/issues) ou usar os recursos internos da CLI para deixar um comentário geral com o comando [az feedback](/cli/azure/reference-index#az-feedback).

```azurecli-interactive
az feedback
```
