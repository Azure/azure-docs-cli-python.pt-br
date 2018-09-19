---
title: Visão geral da CLI do Azure 2.0
description: Visão geral da CLI do Azure 2.0.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 55c5ea3ad69df60d211cc076e3570e9f07040af7
ms.sourcegitcommit: 0e688704889fc88b91588bb6678a933c2d54f020
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/11/2018
ms.locfileid: "44388370"
---
# <a name="azure-cli-20"></a>CLI do Azure 2.0

A CLI do Azure 2.0 é a experiência da linha de comando entre plataformas da Microsoft para gerenciar os recursos do Azure.
Você pode usá-la em seu navegador com o [Azure Cloud Shell](/azure/cloud-shell/overview) ou [instalá-la](install-azure-cli.md) no macOS, Linux ou Windows e executá-la na linha de comando.

A CLI 2.0 do Azure é simples de usar e é indicada para a criação de scripts de automação que funcionam no Azure Resource Manager. Com a CLI do Azure 2.0, a criação de VMs no Azure é tão fácil quanto digitar o seguinte comando:

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

## <a name="run-or-install"></a>Executar ou instalar

Você pode instalar a CLI localmente, executá-la no navegador com o Azure Cloud Shell ou executar em um contêiner do Docker.

* Para executar no seu navegador com o Azure Cloud Shell, consulte [Início rápido para Bash no Azure Cloud Shell](/azure/cloud-shell/quickstart) ou [Início rápido para PowerShell no Azure Cloud Shell](/azure/cloud-shell/quickstart-powershell).
* Para instalar a CLI, confira [Instalar a CLI do Azure 2.0](install-azure-cli.md).
* Para ser executado como um contêiner do Docker, consulte [Executar CLI do Azure 2.0 em um contêiner do Docker](run-azure-cli-docker.md)

## <a name="get-started"></a>Introdução

Leia o artigo de [Introdução](get-started-with-azure-cli.md) para aprender os conceitos básicos sobre a CLI. Os exemplos a seguir demonstram que alguns casos de uso comuns:

- [Máquinas Virtuais do Linux](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [Máquinas Virtuais do Windows](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [Aplicativos Web](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [Banco de Dados SQL](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)

Além disso, uma [referência](/cli/azure/reference-index) detalhada está disponível e documenta a forma de usar cada comando individual da CLI do Azure 2.0.

> [!NOTE]
> Se você usa a versão anterior da CLI (CLI do Azure 1.0), pode continuar a usá-la.
> No entanto, é recomendável atualizar para usar a versão mais recente da CLI do Azure 2.0 para ter a melhor experiência.
> Se você usa ambas CLIs, lembre-se de que `azure` é a CLI antiga (CLI do Azure) e que `az` é a nova CLI (CLI do Azure 2.0).
