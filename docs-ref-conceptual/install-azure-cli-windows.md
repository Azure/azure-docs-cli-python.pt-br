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
# <a name="install-azure-cli-20-on-windows"></a><span data-ttu-id="9d107-103">Instalar CLI do Azure 2.0 no Windows</span><span class="sxs-lookup"><span data-stu-id="9d107-103">Install Azure CLI 2.0 on Windows</span></span>

<span data-ttu-id="9d107-104">No Windows, o binário da CLI do Azure é instalado por meio de uma MSI, o que fornece acesso à CLI por meio do Prompt de Comando do Windows (CMD) ou o PowerShell.</span><span class="sxs-lookup"><span data-stu-id="9d107-104">On Windows the Azure CLI binary is installed via an MSI, which gives you access to the CLI through the Windows Command Prompt (CMD) or PowerShell.</span></span>
<span data-ttu-id="9d107-105">Se você estiver executando o Subsistema do Windows para Linux (WSL), há pacotes disponíveis para a distribuição do Linux.</span><span class="sxs-lookup"><span data-stu-id="9d107-105">If you are running Windows Subsystem for Linux (WSL), there are packages available for your Linux distribution.</span></span> <span data-ttu-id="9d107-106">Consulte a [página instalação principal](install-azure-cli.md) para ver a lista de gerenciadores de pacotes com suporte ou como instalar manualmente no WSL.</span><span class="sxs-lookup"><span data-stu-id="9d107-106">See the [main install page](install-azure-cli.md) for the list of supported package managers or how to install manually under WSL.</span></span>

## <a name="install-or-update"></a><span data-ttu-id="9d107-107">Instalar ou atualizar</span><span class="sxs-lookup"><span data-stu-id="9d107-107">Install or update</span></span>

<span data-ttu-id="9d107-108">O MSI distribuível é usado para instalar, atualizar e desinstalar o comando `az` no Windows.</span><span class="sxs-lookup"><span data-stu-id="9d107-108">The MSI distributable is used for installing, updating, and uninstalling the `az` command on Windows.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="9d107-109">Baixe o instalador MSI</span><span class="sxs-lookup"><span data-stu-id="9d107-109">Download the MSI installer</span></span>](https://aka.ms/installazurecliwindows)

<span data-ttu-id="9d107-110">Quando o instalador perguntar se pode fazer alterações no computador, clique na caixa "Sim".</span><span class="sxs-lookup"><span data-stu-id="9d107-110">When the installer asks if it can make changes to your computer, click the "Yes" box.</span></span>

<span data-ttu-id="9d107-111">Agora, você pode executar a CLI do Azure com o comando `az` no Prompt de Comando do Windows ou no PowerShell.</span><span class="sxs-lookup"><span data-stu-id="9d107-111">You can now run the Azure CLI with the `az` command from either Windows Command Prompt or PowerShell.</span></span> <span data-ttu-id="9d107-112">O PowerShell oferece alguns recursos de conclusão de guia não disponíveis no prompt de comando do Windows.</span><span class="sxs-lookup"><span data-stu-id="9d107-112">PowerShell offers some tab completion features not available from Windows Command Prompt.</span></span> <span data-ttu-id="9d107-113">Para fazer logon, execute o comando `az login`.</span><span class="sxs-lookup"><span data-stu-id="9d107-113">To log in, run the `az login` command.</span></span>

```azurecli
az login
```

<span data-ttu-id="9d107-114">Para saber mais sobre os métodos de logon diferente, consulte [Fazer logon com a CLI do Azure 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="9d107-114">To learn more about different login methods, see [Log in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="uninstall"></a><span data-ttu-id="9d107-115">Desinstalar</span><span class="sxs-lookup"><span data-stu-id="9d107-115">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="9d107-116">A desinstalação pode ser feita executando o MSI novamente e escolhendo a opção "Desinstalar".</span><span class="sxs-lookup"><span data-stu-id="9d107-116">Uninstalling can be done by running the MSI again, and choosing the "Uninstall" option.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="9d107-117">Baixe o instalador MSI</span><span class="sxs-lookup"><span data-stu-id="9d107-117">Download the MSI installer</span></span>](https://aka.ms/installazurecliwindows)
