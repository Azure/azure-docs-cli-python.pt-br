---
title: Visão geral da CLI do Azure
description: Visão geral da CLI (interface de linha de comando) do Azure.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 3b9589c769a90e82c35aa64c583dffdac4e4f063
ms.sourcegitcommit: 4906c38953bdaa344b66749685dedbf2da386dab
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "64319505"
---
# <a name="azure-command-line-interface-cli"></a>CLI (interface de linha de comando) do Azure

A CLI (interface de linha de comando) do Azure é a experiência da linha de comando de plataforma cruzada da Microsoft para gerenciar os recursos do Azure.
Use-a em seu navegador com o [Azure Cloud Shell](/azure/cloud-shell/overview) ou [instale-a](install-azure-cli.md) no macOS, Linux ou Windows e execute-a na linha de comando.

A CLI do Azure é fácil de usar e é indicada para a criação de scripts de automação que funcionam no Azure Resource Manager.
Com a CLI do Azure, a criação de VMs no Azure é tão fácil quanto digitar o seguinte comando:

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

> [!NOTE]
>
> Em scripts e no site de documentação da Microsoft, os exemplos da CLI do Azure são escritos para o shell `bash`. Os exemplos de uma linha serão executados em qualquer plataforma. Os exemplos mais longos, que incluem continuações da linha (`\`) ou a atribuição de variáveis precisam ser modificados para funcionar em outros shells, incluindo o PowerShell.

## <a name="run-or-install"></a>Executar ou instalar

Você pode instalar a CLI localmente, executá-la no navegador com o Azure Cloud Shell ou executar em um contêiner do Docker. Para obter a versão atual da CLI, execute `az --version`.

* Para executar no seu navegador com o Azure Cloud Shell, consulte [Início rápido para Bash no Azure Cloud Shell](/azure/cloud-shell/quickstart) ou [Início rápido para PowerShell no Azure Cloud Shell](/azure/cloud-shell/quickstart-powershell).
* Para instalar a CLI, confira [Instalar a CLI do Azure](install-azure-cli.md).
* Para ser executado como um contêiner do Docker, confira [Executar a CLI do Azure em um contêiner do Docker](run-azure-cli-docker.md)

## <a name="build-your-skills-with-microsoft-learn"></a>Desenvolva suas habilidades com o Microsoft Learn

- [Gerenciar máquinas virtuais com a CLI do Azure](/learn/modules/manage-virtual-machines-with-azure-cli/)
- [Controlar os serviços do Azure com a CLI](/learn/modules/control-azure-services-with-cli/)
- [Mais aprendizado interativo...](/learn/browse/?products=azure-clis)

## <a name="get-started"></a>Introdução

Leia o artigo de [Introdução](get-started-with-azure-cli.md) para aprender os conceitos básicos sobre a CLI. Os exemplos a seguir demonstram que alguns casos de uso comuns:

- [Máquinas Virtuais do Linux](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [Máquinas Virtuais do Windows](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [Aplicativos Web](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [Banco de Dados SQL](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)

Além disso, uma [referência](/cli/azure/reference-index) detalhada está disponível e documenta a forma de usar cada comando individual da CLI do Azure.

> [!NOTE]
> Se você usa a versão anterior da CLI (CLI clássica do Azure), continue a usá-la.
> No entanto, recomendamos a atualização para a versão mais recente da CLI do Azure a fim de ter a melhor experiência.
> Se você usa as duas CLIs, lembre-se de que `azure` é da CLI clássica e `az` é da CLI mais recente.
