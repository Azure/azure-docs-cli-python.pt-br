---
title: Instalar a CLI do Azure para Windows
description: Como instalar a CLI do Azure no Windows
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.prod: azure
ms.date: 09/25/2020
ms.topic: conceptual
ms.devlang: azurecli
ms.technology: azure-cli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 26e7f55d661928af78e645e820990a3617724644
ms.sourcegitcommit: aa44ec97af5c0e7558d254b3159f95921e22ff1c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/01/2020
ms.locfileid: "91625373"
---
# <a name="install-azure-cli-on-windows"></a>Instalar a CLI do Azure no Windows

Para o Windows, a CLI do Azure é instalada por meio de um MSI, o que fornece acesso à CLI por meio do Prompt de Comando do Windows (CMD) ou o PowerShell.
Ao instalar o Subsistema do Windows para Linux (WSL), há pacotes disponíveis para a distribuição do Linux. Consulte a [página instalação principal](install-azure-cli.md) para ver a lista de gerenciadores de pacotes com suporte ou como instalar manualmente no WSL.

[!INCLUDE [current-version](includes/current-version.md)]

## <a name="install-or-update"></a>Instalar ou atualizar

O MSI distribuível é usado para instalar ou atualizar a CLI do Azure no Windows. Você não precisa desinstalar as versões atuais antes de usar o instalador MSI, pois o MSI atualizará qualquer versão existente.

# <a name="microsoft-installer-msi"></a>[Microsoft Installer (MSI)](#tab/azure-cli)

Quando o instalador perguntar se pode fazer alterações no computador, clique na caixa "Sim".

### <a name="azure-cli-current-version"></a>Versão atual da CLI do Azure

Baixe e instale a versão atual da CLI do Azure.  

> [!div class="nextstepaction"]
> [Versão atual da CLI do Azure](https://aka.ms/installazurecliwindows)

### <a name="azure-cli-beta-version"></a>Versão beta da CLI do Azure

A versão beta da CLI do Azure dá suporte a todos os comandos da CLI que você encontrará na versão lançada atual. A versão beta é uma migração da CLI do Azure lançada, pois a plataforma de autenticação do AAD (v1.0) está sendo preterida.  A [plataforma de Identidade da Microsoft (v 2.0)](/azure/active-directory/develop/v2-overview) é o novo método de autenticação e é usada pela CLI do Azure beta.  Recomendamos que você experimente a versão beta com antecedência.  

Para obter mais informações sobre a CLI do Azure beta, confira as [notas sobre a versão](./release-notes-azure-cli.md?tabs=azure-cli-beta).

> [!IMPORTANT]
>
> A versão beta não garante um nível de qualidade igual ao do produto, portanto, não deve ser usada em seu ambiente de produção.

Baixar e instalar a versão beta da CLI do Azure.

> [!div class="nextstepaction"]
> [Versão beta da CLI do Azure](https://aka.ms/installazurecliwindowsbeta)

# <a name="microsoft-installer-msi-with-command"></a>[Microsoft Installer (MSI) com o Comando](#tab/azure-powershell)

### <a name="powershell-command"></a>Comando do PowerShell

Também é possível instalar a CLI do Azure usando o PowerShell. Inicie o PowerShell como administrador e execute o seguinte comando:

   ```PowerShell
   Invoke-WebRequest -Uri https://aka.ms/installazurecliwindows -OutFile .\AzureCLI.msi; Start-Process msiexec.exe -Wait -ArgumentList '/I AzureCLI.msi /quiet'; rm .\AzureCLI.msi
   ```

Isso baixará e instalará a versão mais recente da CLI do Azure para Windows. Se você já tiver uma versão instalada, o instalador atualizará a versão existente. Após a conclusão da instalação, será preciso reabrir o PowerShell para usar a CLI do Azure.

### <a name="azure-cli-command-for-update-only"></a>Comando da CLI do Azure (somente para atualização)
[!INCLUDE [az-upgrade](includes/az-upgrade.md)]

---

## <a name="run-the-azure-cli"></a>Executar a CLI do Azure

Agora, você pode executar a CLI do Azure com o comando `az` no Prompt de Comando do Windows ou no PowerShell. O PowerShell oferece alguns recursos de conclusão de guia não disponíveis no prompt de comando do Windows. Para entrar, execute o comando [az login](/cli/azure/reference-index#az-login).

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Para saber mais sobre os diferentes métodos de autenticação, confira [Entrar com a CLI do Azure](authenticate-azure-cli.md).

## <a name="troubleshooting"></a>Solução de problemas

Veja alguns problemas comuns que ocorrem durante a instalação no Windows. Se você tiver um problema não abordado aqui, [arquive um problema no GitHub](https://github.com/Azure/azure-cli/issues).

### <a name="proxy-blocks-connection"></a>Conexão de blocos de proxy

Se não for possível baixar o instalador do MSI porque o proxy está bloqueando a conexão, verifique se o proxy foi configurado corretamente. No Windows 10, essas configurações são gerenciadas no painel `Settings > Network & Internet > Proxy`. Entre em contato com o administrador do sistema para saber as configurações exigidas ou em situações em que o computador pode ser gerenciado por configuração ou precise de configurações avançadas.

> [!IMPORTANT]
> Essas configurações também precisam ser capazes de acessar os serviços do Azure com a CLI, tanto do PowerShell quanto do prompt de comando. No PowerShell, faça isso com o seguinte comando:
>
> ```powershell
> (New-Object System.Net.WebClient).Proxy.Credentials = `
>   [System.Net.CredentialCache]::DefaultNetworkCredentials
> ```

Para obter o MSI, o proxy precisa permitir conexões HTTPS com os seguintes endereços:

* `https://aka.ms/`
* `https://azurecliprod.blob.core.windows.net/`

## <a name="uninstall"></a>Desinstalar

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

Desinstale a CLI do Azure da lista de "Aplicativos e recursos" do Windows. Para desinstalar:

| Plataforma | Instruções |
|---|---|
| Windows 10 | Iniciar > Configurações > Aplicativos |
| Windows 8 e Windows 7 | Iniciar > Painel de Controle > Programas > Desinstalar um programa |

Uma vez nessa tela, digite __CLI do Azure__ na barra de pesquisa do programa. O programa de desinstalação aparece como __Microsoft CLI 2.0 para Azure__. Selecione este aplicativo e clique no botão `Uninstall`.

## <a name="next-steps"></a>Próximas etapas

Agora que você instalou a CLI do Azure, faça um tour breve de seus recursos e comandos comuns.

> [!div class="nextstepaction"]
> [Introdução à CLI do Azure](get-started-with-azure-cli.md)