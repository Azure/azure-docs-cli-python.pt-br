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
ms.openlocfilehash: f45c3acfdb4edb82cde755472d240ae18d82aba2
ms.sourcegitcommit: 64f2c628e83d687d0e172c01f13d71c8c39a8040
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/11/2018
ms.locfileid: "38967734"
---
# <a name="get-started-with-azure-cli-20"></a>Introdução à CLI do Azure 2.0

Bem-vindo à CLI do Azure 2.0! A CLI é uma ferramenta projetada para ajudar você a trabalhar de forma rápida e eficaz com os serviços do Azure, com ênfase na automação. Este artigo apresenta recursos da CLI e links externos para recursos que ajudarão você a ser produtivo.

## <a name="install-and-sign-in"></a>Instalar e entrar

Caso ainda não o tenha feito, [instale a CLI](install-azure-cli.md) ou experimento o [Azure Cloud Shell](/azure/cloud-shell/overview).

Antes de usar os comandos da CLI com uma instalação local, é preciso entrar com [az login](/cli/azure/reference-index#az-login).

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Há maneiras de entrar de modo não interativo, como mostrado em detalhes em [Entrar com a CLI do Azure 2.0](authenticate-azure-cli.md).

## <a name="common-commands"></a>Comandos comuns

Esta tabela lista alguns dos comandos comuns usados nos links externos da CLI para suas páginas de documentação nas referências.
Todos os subcomandos desses grupos e sua documentação podem ser pesquisados na referência online ou com o argumento `--help`.

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

Comandos na CLI são fornecidos como _subcomandos_ de _grupos_.
Cada grupo representa um serviço fornecido pelo Azure, e os subgrupos dividem os comandos para esses serviços em agrupamentos lógicos.

Para procurar comandos, use [az find](/cli/azure/reference-index#az-find). Por exemplo, para procurar nomes de comando que contenham `secret`, use o seguinte comando:

```azurecli-interactive
az find -q secret
```

Caso saiba com qual grupo de comandos deseja trabalhar, o argumento `--help` pode ser uma opção melhor. Ele exibe não apenas informações detalhadas de um comando, como também, quando usado com um grupo de comando, todos os subcomandos disponíveis. Por exemplo, ao trabalhar com Grupos de Segurança de Rede (NSGs), é possível encontrar os subgrupos de NSG e comandos disponíveis.

```azurecli-interactive
az network nsg --help
```

A CLI tem o preenchimento completo de guia para comandos sob o shell do Bash.

## <a name="globally-available-arguments"></a>Argumentos disponíveis globalmente

Há alguns argumentos disponíveis para cada comando.

* `--help` imprime as informações de referência da CLI sobre comandos e seus argumentos, além de listar os comandos e subgrupos disponíveis.
* `--output` altera o formato de saída. Os formatos de saída disponíveis são `json`, `jsonc`(JSON colorido), `tsv` (valores separados por tabulação) e `table` (tabelas ASCII legível por humanos). Por padrão, a CLI gera `json`. Para saber mais sobre os formatos de saída disponível, consulte [Formatos de saída da CLI do Azure 2.0](format-output-azure-cli.md).
* `--query` usa o [linguagem de consulta JMESPath](http://jmespath.org/) para filtrar a saída retornada dos serviços do Azure. Para saber mais sobre consultas, consulte [Consultar resultados do comando com a CLI do Azure 2.0](query-azure-cli.md) e [tutorial do JMESPath](http://jmespath.org/tutorial.html).
* `--verbose` imprime informações sobre recursos criados no Azure durante uma operação, além de outras informações úteis.
* `--debug` imprime ainda mais informações sobre operações de CLI e é usado para fins de depuração. Se você encontrar um bug, forneça a saída gerada com o sinalizador `--debug` ao enviar um relatório de bugs.

## <a name="interactive-mode"></a>Modo interativo

A CLI oferece um modo interativo que exibe informações de ajuda automaticamente e torna mais fácil selecionar subcomandos. Você entra no modo interativo com o comando [az interactive](/cli/azure/reference-index#az-interactive).

```azurecli-interactive
az interactive
```

Para obter mais informações sobre o modo interativo, consulte [Modo Interativo da CLI 2.0 do Azure](interactive-azure-cli.md).

Também há um [Plug-in do Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli) que oferece uma experiência interativa, incluindo documentação de preenchimento automático e com o passar do mouse.

## <a name="learn-cli-basics-with-quickstarts-and-tutorials"></a>Aprenda as noções básica da CLI com os guias de início rápido e tutoriais

Para a introdução à CLI do Azure 2.0, experimente ver um tutorial aprofundado para configurar máquinas virtuais e usar o poder da CLI para consultar recursos do Azure.

> [!div class="nextstepaction"]
> [Tutorial Criar máquinas virtuais com a CLI do Azure 2.0](azure-cli-vm-tutorial.yml)

Se você preferir se concentrar em outros serviços, há uma variedade de guias de início rápido para os serviços do Azure que usam a CLI.

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
