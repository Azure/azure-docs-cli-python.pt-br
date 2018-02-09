---
title: Instalar a CLI do Azure para Windows
description: Como instalar a CLI do Azure 2.0 no Windows
keywords: CLI do Azure, Instalar CLI do Azure, windows instalar azure, windows da cli do azure, windows do azure
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/18
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: fc84b80e44a994495ef97cf9d7ec4e4a79a5c5b3
ms.sourcegitcommit: b41c5ed4a26c771a1a32b4560131f7a65b80fd33
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2018
---
# <a name="install-azure-cli-20-on-windows"></a>Instalar CLI do Azure 2.0 no Windows

No Windows, o binário da CLI do Azure é instalado por meio de uma MSI, o que fornece acesso à CLI por meio do Prompt de Comando do Windows (CMD) ou o PowerShell.
Se você estiver executando o Subsistema do Windows para Linux (WSL), há pacotes disponíveis para a distribuição do Linux. Consulte a [página instalação principal](install-azure-cli.md) para ver a lista de gerenciadores de pacotes com suporte ou como instalar manualmente no WSL.

## <a name="install-or-update"></a>Instalar ou atualizar

O MSI distribuível é usado para instalar, atualizar e desinstalar o comando `az` no Windows.

> [!div class="nextstepaction"]
> [Baixe o instalador MSI](https://azurecliprod.blob.core.windows.net/msi/azure-cli-latest.msi)

Quando o instalador perguntar se pode fazer alterações no computador, clique na caixa "Sim".

Agora, você pode executar a CLI do Azure com o comando `az` no Prompt de Comando do Windows ou no PowerShell. O PowerShell oferece alguns recursos de conclusão de guia não disponíveis de CMD.

## <a name="uninstall"></a>Desinstalar

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

A desinstalação pode ser feita executando o MSI novamente e escolhendo a opção "Desinstalar". 

> [!div class="nextstepaction"]
> [Baixe o instalador MSI](https://azurecliprod.blob.core.windows.net/msi/azure-cli-latest.msi)
