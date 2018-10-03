---
title: Instalar a CLI do Azure para Windows
description: Como instalar a CLI do Azure no Windows
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: c65cff52211b4c77e32c2992cd71392c8b0e44d6
ms.sourcegitcommit: c4462456dfb17993f098d47c37bc19f4d78b8179
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/25/2018
ms.locfileid: "47177956"
---
# <a name="install-azure-cli-on-windows"></a><span data-ttu-id="ee92f-103">Instalar a CLI do Azure no Windows</span><span class="sxs-lookup"><span data-stu-id="ee92f-103">Install Azure CLI on Windows</span></span>

<span data-ttu-id="ee92f-104">Para Windows, a CLI do Azure é instalada por meio de um MSI, o que fornece acesso à CLI por meio do Prompt de Comando do Windows (CMD) ou o PowerShell.</span><span class="sxs-lookup"><span data-stu-id="ee92f-104">For Windows the Azure CLI is installed via an MSI, which gives you access to the CLI through the Windows Command Prompt (CMD) or PowerShell.</span></span>
<span data-ttu-id="ee92f-105">Ao instalar o Subsistema do Windows para Linux (WSL), há pacotes disponíveis para a distribuição do Linux.</span><span class="sxs-lookup"><span data-stu-id="ee92f-105">When installing for Windows Subsystem for Linux (WSL), packages are available for your Linux distribution.</span></span> <span data-ttu-id="ee92f-106">Consulte a [página instalação principal](install-azure-cli.md) para ver a lista de gerenciadores de pacotes com suporte ou como instalar manualmente no WSL.</span><span class="sxs-lookup"><span data-stu-id="ee92f-106">See the [main install page](install-azure-cli.md) for the list of supported package managers or how to install manually under WSL.</span></span>

## <a name="install-or-update"></a><span data-ttu-id="ee92f-107">Instalar ou atualizar</span><span class="sxs-lookup"><span data-stu-id="ee92f-107">Install or update</span></span>

<span data-ttu-id="ee92f-108">O MSI distribuível é usado para instalar, atualizar e desinstalar o comando `az` no Windows.</span><span class="sxs-lookup"><span data-stu-id="ee92f-108">The MSI distributable is used for installing, updating, and uninstalling the `az` command on Windows.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="ee92f-109">Baixe o instalador MSI</span><span class="sxs-lookup"><span data-stu-id="ee92f-109">Download the MSI installer</span></span>](https://aka.ms/installazurecliwindows)

<span data-ttu-id="ee92f-110">Quando o instalador perguntar se pode fazer alterações no computador, clique na caixa "Sim".</span><span class="sxs-lookup"><span data-stu-id="ee92f-110">When the installer asks if it can make changes to your computer, click the "Yes" box.</span></span>

<span data-ttu-id="ee92f-111">Agora, você pode executar a CLI do Azure com o comando `az` no Prompt de Comando do Windows ou no PowerShell.</span><span class="sxs-lookup"><span data-stu-id="ee92f-111">You can now run the Azure CLI with the `az` command from either Windows Command Prompt or PowerShell.</span></span> <span data-ttu-id="ee92f-112">O PowerShell oferece alguns recursos de conclusão de guia não disponíveis no prompt de comando do Windows.</span><span class="sxs-lookup"><span data-stu-id="ee92f-112">PowerShell offers some tab completion features not available from Windows Command Prompt.</span></span> <span data-ttu-id="ee92f-113">Para entrar, execute o comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="ee92f-113">To sign in, run the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="ee92f-114">Para saber mais sobre os diferentes métodos de autenticação, confira [Entrar com a CLI do Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="ee92f-114">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="uninstall"></a><span data-ttu-id="ee92f-115">Desinstalar</span><span class="sxs-lookup"><span data-stu-id="ee92f-115">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="ee92f-116">A desinstalação pode ser feita executando o MSI novamente e escolhendo a opção "Desinstalar".</span><span class="sxs-lookup"><span data-stu-id="ee92f-116">Uninstalling can be done by running the MSI again, and choosing the "Uninstall" option.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="ee92f-117">Baixe o instalador MSI</span><span class="sxs-lookup"><span data-stu-id="ee92f-117">Download the MSI installer</span></span>](https://aka.ms/installazurecliwindows)

## <a name="next-steps"></a><span data-ttu-id="ee92f-118">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="ee92f-118">Next Steps</span></span>

<span data-ttu-id="ee92f-119">Agora que você instalou a CLI do Azure, faça um tour breve de seus recursos e comandos comuns.</span><span class="sxs-lookup"><span data-stu-id="ee92f-119">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="ee92f-120">Introdução à CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="ee92f-120">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
