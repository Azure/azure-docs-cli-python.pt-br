---
title: CLI do Azure 2.0
description: "Visão geral da CLI do Azure 2.0."
keywords: CLI do Azure 2.0, Linux, Mac, Windows, OS X, Ubuntu, Debian, CentOS, RHEL, SUSE, CoreOS, Docker, Windows, Python, PIP
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 80ae9f6c-adb7-483c-bfb4-fbb958e075ba
ms.openlocfilehash: 2f4f9950dd663ae85f41bf4efe114b15770ace5d
ms.sourcegitcommit: bcf93ad8ed8802072249cd8187cd4420da89b4c6
ms.translationtype: HT
ms.contentlocale: pt-BR
---
# <a name="azure-cli-20"></a>CLI do Azure 2.0

A CLI 2.0 do Azure é a nova experiência de linha de comando do Azure para gerenciar recursos do Azure.  Ela pode ser usada em Windows, Linux e macOS. 

A CLI do Azure 2.0 foi projetada para gerenciar e administrar os recursos do Azure da linha de comando e para a compilação de scripts de automação que funcionam no Azure Resource Manager. Com a CLI do Azure 2.0, a criação de VMs no Azure é tão fácil quanto digitar o seguinte comando:

```azurecli
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

Examine o artigo [Instalar](install-azure-cli.md) para colocar a CLI do Azure 2.0 em funcionamento no sistema. Em seguida, leia o artigo de [Introdução](get-started-with-azure-cli.md) para começar a usá-lo.
Para saber mais sobre a versão mais recente, consulte as [notas de versão](release-notes-azure-cli.md).

Os exemplos a seguir podem ajudar você a saber mais sobre como executar cenários comuns com a CLI do Azure 2.0:
- [Máquinas Virtuais do Linux](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [Máquinas Virtuais do Windows](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [Aplicativos Web](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [Banco de Dados SQL](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)

Além disso, uma [referência](/cli/azure/) detalhada está disponível e documenta a forma de usar cada comando individual da CLI do Azure 2.0.

[Comece a usar](get-started-with-azure-cli.md) a CLI do Azure 2.0 agora.


> [!NOTE]
> Se você usa a versão anterior da CLI (CLI do Azure), continue a usá-la.
> Se você usa ambas CLIs, lembre-se de que `azure` é a CLI antiga (CLI do Azure) e que `az` é a nova CLI (CLI do Azure 2.0). 