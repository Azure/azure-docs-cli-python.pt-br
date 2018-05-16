---
title: CLI do Azure 2.0
description: Visão geral da CLI do Azure 2.0.
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: ee82c06e5b5b614b5557c6e6426d2da488468318
ms.sourcegitcommit: 15d6dfaee2075d0abceb2aa2423f0b6ef7b2ac9b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2018
---
# <a name="azure-cli-20"></a>CLI do Azure 2.0

A CLI 2.0 do Azure é a nova experiência de linha de comando do Azure para gerenciar recursos do Azure.
Você pode usá-lo no seu navegador com o [Azure Cloud Shell](/azure/cloud-shell/overview) ou pode [instalá-lo](install-azure-cli.md) no macOS, Linux e Windows e executá-lo da linha de comando.

A CLI do Azure 2.0 foi projetada para gerenciar e administrar os recursos do Azure da linha de comando e para a compilação de scripts de automação que funcionam no Azure Resource Manager. Com a CLI do Azure 2.0, a criação de VMs no Azure é tão fácil quanto digitar o seguinte comando:

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

Use o [Cloud Shell](/azure/cloud-shell/overview) para executar a CLI no seu navegador ou [instale-o](install-azure-cli.md) no macOS, Linux ou Windows.
Leia o artigo de [Introdução](get-started-with-azure-cli.md) para começar a usar a CLI.
Para saber mais sobre a versão mais recente, veja as [notas de versão](release-notes-azure-cli.md).

Os exemplos a seguir podem ajudar você a saber mais sobre como executar cenários comuns com a CLI do Azure 2.0:
- [Máquinas Virtuais do Linux](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [Máquinas Virtuais do Windows](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)

Além disso, uma [referência](/cli/azure/reference-index) detalhada está disponível e documenta a forma de usar cada comando individual da CLI do Azure 2.0.

[Comece a usar](get-started-with-azure-cli.md) a CLI do Azure 2.0 agora.


> [!NOTE]
> Se você usa a versão anterior da CLI (CLI do Azure), continue a usá-la.
> Se você usa ambas CLIs, lembre-se de que `azure` é a CLI antiga (CLI do Azure) e que `az` é a nova CLI (CLI do Azure 2.0).
