---
title: Instalar a CLI do Azure para Windows
description: Como instalar a CLI do Azure 2.0 no Windows
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 30bdb327601c7d898b5e64a3a472a104dc5db3b4
ms.sourcegitcommit: 0e688704889fc88b91588bb6678a933c2d54f020
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/11/2018
ms.locfileid: "44388449"
---
# <a name="install-azure-cli-20-on-windows"></a><span data-ttu-id="9126c-103">Instalar CLI do Azure 2.0 no Windows</span><span class="sxs-lookup"><span data-stu-id="9126c-103">Install Azure CLI 2.0 on Windows</span></span>

<span data-ttu-id="9126c-104">Para Windows, a CLI do Azure é instalada por meio de um MSI, o que fornece acesso à CLI por meio do Prompt de Comando do Windows (CMD) ou o PowerShell.</span><span class="sxs-lookup"><span data-stu-id="9126c-104">For Windows the Azure CLI is installed via an MSI, which gives you access to the CLI through the Windows Command Prompt (CMD) or PowerShell.</span></span>
<span data-ttu-id="9126c-105">Ao instalar o Subsistema do Windows para Linux (WSL), há pacotes disponíveis para a distribuição do Linux.</span><span class="sxs-lookup"><span data-stu-id="9126c-105">When installing for Windows Subsystem for Linux (WSL), packages are available for your Linux distribution.</span></span> <span data-ttu-id="9126c-106">Consulte a [página instalação principal](install-azure-cli.md) para ver a lista de gerenciadores de pacotes com suporte ou como instalar manualmente no WSL.</span><span class="sxs-lookup"><span data-stu-id="9126c-106">See the [main install page](install-azure-cli.md) for the list of supported package managers or how to install manually under WSL.</span></span>

## <a name="install-or-update"></a><span data-ttu-id="9126c-107">Instalar ou atualizar</span><span class="sxs-lookup"><span data-stu-id="9126c-107">Install or update</span></span>

<span data-ttu-id="9126c-108">O MSI distribuível é usado para instalar, atualizar e desinstalar o comando `az` no Windows.</span><span class="sxs-lookup"><span data-stu-id="9126c-108">The MSI distributable is used for installing, updating, and uninstalling the `az` command on Windows.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="9126c-109">Baixe o instalador MSI</span><span class="sxs-lookup"><span data-stu-id="9126c-109">Download the MSI installer</span></span>](https://aka.ms/installazurecliwindows)

<span data-ttu-id="9126c-110">Quando o instalador perguntar se pode fazer alterações no computador, clique na caixa "Sim".</span><span class="sxs-lookup"><span data-stu-id="9126c-110">When the installer asks if it can make changes to your computer, click the "Yes" box.</span></span>

<span data-ttu-id="9126c-111">Agora, você pode executar a CLI do Azure com o comando `az` no Prompt de Comando do Windows ou no PowerShell.</span><span class="sxs-lookup"><span data-stu-id="9126c-111">You can now run the Azure CLI with the `az` command from either Windows Command Prompt or PowerShell.</span></span> <span data-ttu-id="9126c-112">O PowerShell oferece alguns recursos de conclusão de guia não disponíveis no prompt de comando do Windows.</span><span class="sxs-lookup"><span data-stu-id="9126c-112">PowerShell offers some tab completion features not available from Windows Command Prompt.</span></span> <span data-ttu-id="9126c-113">Para entrar, execute o comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="9126c-113">To sign in, run the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="9126c-114">Para saber mais sobre os diferentes métodos de autenticação, consulte [Conectar com a CLI do Azure 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="9126c-114">To learn more about different authentication methods, see [Sign in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="uninstall"></a><span data-ttu-id="9126c-115">Desinstalar</span><span class="sxs-lookup"><span data-stu-id="9126c-115">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="9126c-116">A desinstalação pode ser feita executando o MSI novamente e escolhendo a opção "Desinstalar".</span><span class="sxs-lookup"><span data-stu-id="9126c-116">Uninstalling can be done by running the MSI again, and choosing the "Uninstall" option.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="9126c-117">Baixe o instalador MSI</span><span class="sxs-lookup"><span data-stu-id="9126c-117">Download the MSI installer</span></span>](https://aka.ms/installazurecliwindows)
