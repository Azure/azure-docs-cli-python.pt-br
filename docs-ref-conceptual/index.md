---
title: CLI do Azure 2.0
description: Visão geral da CLI do Azure 2.0.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/16/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 9b6f7a5c79033c0b0bec2bf8b56eb40831484f1a
ms.sourcegitcommit: 8b4629a42ceecf30c1efbc6fdddf512f4dddfab0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/18/2018
ms.locfileid: "34306243"
---
# <a name="azure-cli-20"></a>CLI do Azure 2.0

A CLI do Azure 2.0 é a experiência da linha de comando entre plataformas da Microsoft para gerenciar os recursos do Azure.
Você pode usá-la em seu navegador com o [Azure Cloud Shell](/azure/cloud-shell/overview) ou [instalá-la](install-azure-cli.md) no macOS, Linux ou Windows e executá-la na linha de comando.

A CLI do Azure 2.0 foi projetada para gerenciar e administrar os recursos do Azure da linha de comando e para a compilação de scripts de automação que funcionam no Azure Resource Manager. Com a CLI do Azure 2.0, a criação de VMs no Azure é tão fácil quanto digitar o seguinte comando:

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

Use o [Cloud Shell](/azure/cloud-shell/overview) para executar a CLI no seu navegador ou [instale-o](install-azure-cli.md) no macOS, Linux ou Windows.
Leia o artigo de [Introdução](get-started-with-azure-cli.md) para começar a usar a CLI.
Para saber mais sobre a versão mais recente, veja as [notas de versão](release-notes-azure-cli.md).

Os exemplos a seguir o ajudarão a começar com as tarefas comuns na CLI do Azure 2.0:
- [Máquinas Virtuais do Linux](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- Interativo: [Criar máquinas virtuais do Linux](https://docs.microsoft.com/learn/azure-cli-2-0/index)
- [Máquinas Virtuais do Windows](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [Aplicativos Web](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [Banco de Dados SQL](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)

Além disso, uma [referência](/cli/azure/reference-index) detalhada está disponível e documenta a forma de usar cada comando individual da CLI do Azure 2.0.

[Comece a usar](get-started-with-azure-cli.md) a CLI do Azure 2.0 agora.

> [!NOTE]
> Se você usa a versão anterior da CLI (CLI do Azure 1.0), pode continuar a usá-la.
> No entanto, é recomendável atualizar para usar a versão mais recente da CLI do Azure 2.0 para ter a melhor experiência.
> Se você usa ambas CLIs, lembre-se de que `azure` é a CLI antiga (CLI do Azure) e que `az` é a nova CLI (CLI do Azure 2.0).
