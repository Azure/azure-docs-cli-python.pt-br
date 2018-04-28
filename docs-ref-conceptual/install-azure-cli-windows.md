---
title: Instalar a CLI do Azure para Windows
description: Como instalar a CLI do Azure 2.0 no Windows
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 01/29/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 27284520d923524c5f772c82246889b2f1e6cb8b
ms.sourcegitcommit: ae72b6c8916aeb372a92188090529037e63930ba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2018
---
# <a name="install-azure-cli-20-on-windows"></a>Instalar CLI do Azure 2.0 no Windows

No Windows, o binário da CLI do Azure é instalado por meio de uma MSI, o que fornece acesso à CLI por meio do Prompt de Comando do Windows (CMD) ou o PowerShell.
Se você estiver executando o Subsistema do Windows para Linux (WSL), há pacotes disponíveis para a distribuição do Linux. Consulte a [página instalação principal](install-azure-cli.md) para ver a lista de gerenciadores de pacotes com suporte ou como instalar manualmente no WSL.

## <a name="install-or-update"></a>Instalar ou atualizar

O MSI distribuível é usado para instalar, atualizar e desinstalar o comando `az` no Windows.

> [!div class="nextstepaction"]
> [Baixe o instalador MSI](https://aka.ms/installazurecliwindows)

Quando o instalador perguntar se pode fazer alterações no computador, clique na caixa "Sim".

Agora, você pode executar a CLI do Azure com o comando `az` no Prompt de Comando do Windows ou no PowerShell. O PowerShell oferece alguns recursos de conclusão de guia não disponíveis no prompt de comando do Windows. Para fazer logon, execute o comando `az login`.

```azurecli
az login
```

Para saber mais sobre os métodos de logon diferente, consulte [Fazer logon com a CLI do Azure 2.0](authenticate-azure-cli.md).

## <a name="uninstall"></a>Desinstalar

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

A desinstalação pode ser feita executando o MSI novamente e escolhendo a opção "Desinstalar".

> [!div class="nextstepaction"]
> [Baixe o instalador MSI](https://aka.ms/installazurecliwindows)
