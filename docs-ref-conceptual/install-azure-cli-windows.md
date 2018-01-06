---
title: Instalar a CLI do Azure para Windows
description: Como instalar a CLI do Azure 2.0 no Windows
keywords: CLI do Azure, Instalar CLI do Azure, windows instalar azure, windows da cli do azure, windows do azure
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 11/01/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ROBOTS: NOINDEX,NOFOLLOW
ms.openlocfilehash: 247ae43813ca9ca7b7b98ebd8e933e02989c6649
ms.sourcegitcommit: 2e4d0bdd94c626e061434883032367b5619de4fe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2017
---
# <a name="install-azure-cli-20-on-windows"></a>Instalar CLI do Azure 2.0 no Windows

No Windows, você pode instalar um binário nativo de um MSI, que pode ser usado com o Prompt de Comando do Windows ou PowerShell. Se você estiver executando o Subsistema do Windows para Linux (WSL), pacotes estarão disponíveis para a distribuição executada. Consulte a [página instalação principal](install-azure-cli.md) para ver a lista de gerenciadores de pacotes com suporte ou como instalar manualmente no WSL.

## <a name="install-or-update-with-msi"></a>Instalar ou atualizar com o MSI

O MSI distribuível é usado para instalar, atualizar e desinstalar o comando `az` no Windows. Você pode [baixar o instalador MSI](https://aka.ms/InstallAzureCliWindows) e executá-lo para instalar ou atualizar.

Quando o instalador perguntar se pode fazer alterações no computador, clique na caixa "Sim".

Agora, você pode executar a CLI do Azure com o comando `az` no Prompt de Comando do Windows ou no PowerShell.

## <a name="uninstall-with-msi"></a>Desinstalar com MSI

Se você decidiu desinstalar a CLI do Azure, lamentamos sua saída. Antes de desinstalar, use o comando `az feedback` para nos fornecer algumas razões por ter escolhido desinstalar e como poderíamos melhorar a experiência da CLI. Queremos assegurar que a CLI do Azure não tenha bugs e seja amigável o máximo possível. Você também pode [registrar um problema do github](https://github.com/Azure/azure-cli/issues).

A desinstalação pode ser feita executando o MSI novamente e escolhendo a opção "Desinstalar". É possível [baixar o instalador MSI](https://aka.ms/InstallAzureCliWindows) se você o não tiver mais disponível.
