---
title: Instalar a CLI do Azure para Windows
description: Como instalar a CLI do Azure no Windows
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/01/2019
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: c5c499800e49dcdc536337e7655ec1ee280d48f2
ms.sourcegitcommit: 65bf8561a6e047e4eab52186e066a2e8c21f1d40
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2019
ms.locfileid: "65240553"
---
# <a name="install-azure-cli-on-windows"></a>Instalar a CLI do Azure no Windows

Para Windows, a CLI do Azure é instalada por meio de um MSI, o que fornece acesso à CLI por meio do Prompt de Comando do Windows (CMD) ou o PowerShell.
Ao instalar o Subsistema do Windows para Linux (WSL), há pacotes disponíveis para a distribuição do Linux. Consulte a [página instalação principal](install-azure-cli.md) para ver a lista de gerenciadores de pacotes com suporte ou como instalar manualmente no WSL.

[!INCLUDE [current-version](includes/current-version.md)]

## <a name="install-or-update"></a>Instalar ou atualizar

O MSI distribuível é usado para instalar ou atualizar a CLI do Azure no Windows. Você não precisa desinstalar as versões atuais antes de usar o instalador MSI.

> [!div class="nextstepaction"]
> [Baixe o instalador MSI](https://aka.ms/installazurecliwindows)

Quando o instalador perguntar se pode fazer alterações no computador, clique na caixa "Sim".

Agora, você pode executar a CLI do Azure com o comando `az` no Prompt de Comando do Windows ou no PowerShell. O PowerShell oferece alguns recursos de conclusão de guia não disponíveis no prompt de comando do Windows. Para entrar, execute o comando [az login](/cli/azure/reference-index#az-login).

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Para saber mais sobre os diferentes métodos de autenticação, confira [Entrar com a CLI do Azure](authenticate-azure-cli.md).

## <a name="uninstall"></a>Desinstalar

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

Desinstale a CLI do Azure da lista de "Aplicativos e recursos" do Windows. Para desinstalar:

| Plataforma | Instruções |
|---|---|
| Windows 10 | Iniciar > Configurações > Aplicativos |
| Windows 8<br/>Windows 7 | Iniciar > Painel de Controle > Programas > Desinstalar um programa |

Uma vez nessa tela, digite __CLI do Azure__ na barra de pesquisa do programa. O programa de desinstalação aparece como __Microsoft CLI 2.0 para Azure__. Selecione este aplicativo e clique no botão `Uninstall`.

## <a name="next-steps"></a>Próximas etapas

Agora que você instalou a CLI do Azure, faça um tour breve de seus recursos e comandos comuns.

> [!div class="nextstepaction"]
> [Introdução à CLI do Azure](get-started-with-azure-cli.md)
