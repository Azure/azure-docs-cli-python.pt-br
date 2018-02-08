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
# <a name="install-azure-cli-20-on-windows"></a><span data-ttu-id="34322-104">Instalar CLI do Azure 2.0 no Windows</span><span class="sxs-lookup"><span data-stu-id="34322-104">Install Azure CLI 2.0 on Windows</span></span>

<span data-ttu-id="34322-105">No Windows, o binário da CLI do Azure é instalado por meio de uma MSI, o que fornece acesso à CLI por meio do Prompt de Comando do Windows (CMD) ou o PowerShell.</span><span class="sxs-lookup"><span data-stu-id="34322-105">On Windows the Azure CLI binary is installed via an MSI, which gives you access to the CLI through the Windows Command Prompt (CMD) or PowerShell.</span></span>
<span data-ttu-id="34322-106">Se você estiver executando o Subsistema do Windows para Linux (WSL), há pacotes disponíveis para a distribuição do Linux.</span><span class="sxs-lookup"><span data-stu-id="34322-106">If you are running Windows Subsystem for Linux (WSL), there are packages available for your Linux distribution.</span></span> <span data-ttu-id="34322-107">Consulte a [página instalação principal](install-azure-cli.md) para ver a lista de gerenciadores de pacotes com suporte ou como instalar manualmente no WSL.</span><span class="sxs-lookup"><span data-stu-id="34322-107">See the [main install page](install-azure-cli.md) for the list of supported package managers or how to install manually under WSL.</span></span>

## <a name="install-or-update"></a><span data-ttu-id="34322-108">Instalar ou atualizar</span><span class="sxs-lookup"><span data-stu-id="34322-108">Install or update</span></span>

<span data-ttu-id="34322-109">O MSI distribuível é usado para instalar, atualizar e desinstalar o comando `az` no Windows.</span><span class="sxs-lookup"><span data-stu-id="34322-109">The MSI distributable is used for installing, updating, and uninstalling the `az` command on Windows.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="34322-110">Baixe o instalador MSI</span><span class="sxs-lookup"><span data-stu-id="34322-110">Download the MSI installer</span></span>](https://azurecliprod.blob.core.windows.net/msi/azure-cli-latest.msi)

<span data-ttu-id="34322-111">Quando o instalador perguntar se pode fazer alterações no computador, clique na caixa "Sim".</span><span class="sxs-lookup"><span data-stu-id="34322-111">When the installer asks if it can make changes to your computer, click the "Yes" box.</span></span>

<span data-ttu-id="34322-112">Agora, você pode executar a CLI do Azure com o comando `az` no Prompt de Comando do Windows ou no PowerShell.</span><span class="sxs-lookup"><span data-stu-id="34322-112">You can now run the Azure CLI with the `az` command from either Windows Command Prompt or PowerShell.</span></span> <span data-ttu-id="34322-113">O PowerShell oferece alguns recursos de conclusão de guia não disponíveis de CMD.</span><span class="sxs-lookup"><span data-stu-id="34322-113">PowerShell offers some tab completion features not available from CMD.</span></span>

## <a name="uninstall"></a><span data-ttu-id="34322-114">Desinstalar</span><span class="sxs-lookup"><span data-stu-id="34322-114">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="34322-115">A desinstalação pode ser feita executando o MSI novamente e escolhendo a opção "Desinstalar".</span><span class="sxs-lookup"><span data-stu-id="34322-115">Uninstalling can be done by running the MSI again, and choosing the "Uninstall" option.</span></span> 

> [!div class="nextstepaction"]
> [<span data-ttu-id="34322-116">Baixe o instalador MSI</span><span class="sxs-lookup"><span data-stu-id="34322-116">Download the MSI installer</span></span>](https://azurecliprod.blob.core.windows.net/msi/azure-cli-latest.msi)
