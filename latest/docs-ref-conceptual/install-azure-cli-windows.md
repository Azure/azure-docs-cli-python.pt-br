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
# <a name="install-azure-cli-20-on-windows"></a><span data-ttu-id="c1422-104">Instalar CLI do Azure 2.0 no Windows</span><span class="sxs-lookup"><span data-stu-id="c1422-104">Install Azure CLI 2.0 on Windows</span></span>

<span data-ttu-id="c1422-105">No Windows, você pode instalar um binário nativo de um MSI, que pode ser usado com o Prompt de Comando do Windows ou PowerShell.</span><span class="sxs-lookup"><span data-stu-id="c1422-105">On Windows, you can install a native binary from an MSI, which you can use through the Windows Command Prompt or PowerShell.</span></span> <span data-ttu-id="c1422-106">Se você estiver executando o Subsistema do Windows para Linux (WSL), pacotes estarão disponíveis para a distribuição executada.</span><span class="sxs-lookup"><span data-stu-id="c1422-106">If you are running Windows Subsystem for Linux (WSL) there are packages available for the distribution you are running.</span></span> <span data-ttu-id="c1422-107">Consulte a [página instalação principal](install-azure-cli.md) para ver a lista de gerenciadores de pacotes com suporte ou como instalar manualmente no WSL.</span><span class="sxs-lookup"><span data-stu-id="c1422-107">See the [main install page](install-azure-cli.md) for the list of supported package managers or how to install manually under WSL.</span></span>

## <a name="install-or-update-with-msi"></a><span data-ttu-id="c1422-108">Instalar ou atualizar com o MSI</span><span class="sxs-lookup"><span data-stu-id="c1422-108">Install or update with MSI</span></span>

<span data-ttu-id="c1422-109">O MSI distribuível é usado para instalar, atualizar e desinstalar o comando `az` no Windows.</span><span class="sxs-lookup"><span data-stu-id="c1422-109">The MSI distributable is used for installing, updating, and uninstalling the `az` command on Windows.</span></span> <span data-ttu-id="c1422-110">Você pode [baixar o instalador MSI](https://aka.ms/InstallAzureCliWindows) e executá-lo para instalar ou atualizar.</span><span class="sxs-lookup"><span data-stu-id="c1422-110">You can [download the MSI installer](https://aka.ms/InstallAzureCliWindows) and then run it to install or update.</span></span>

<span data-ttu-id="c1422-111">Quando o instalador perguntar se pode fazer alterações no computador, clique na caixa "Sim".</span><span class="sxs-lookup"><span data-stu-id="c1422-111">When the installer asks if it can make changes to your computer, click the "Yes" box.</span></span>

<span data-ttu-id="c1422-112">Agora, você pode executar a CLI do Azure com o comando `az` no Prompt de Comando do Windows ou no PowerShell.</span><span class="sxs-lookup"><span data-stu-id="c1422-112">You can now run the Azure CLI with the `az` command from either Windows Command Prompt or PowerShell.</span></span>

## <a name="uninstall-with-msi"></a><span data-ttu-id="c1422-113">Desinstalar com MSI</span><span class="sxs-lookup"><span data-stu-id="c1422-113">Uninstall with MSI</span></span>

<span data-ttu-id="c1422-114">Se você decidiu desinstalar a CLI do Azure, lamentamos sua saída.</span><span class="sxs-lookup"><span data-stu-id="c1422-114">If you ever decide to uninstall the Azure CLI, we're sorry to see you go.</span></span> <span data-ttu-id="c1422-115">Antes de desinstalar, use o comando `az feedback` para nos fornecer algumas razões por ter escolhido desinstalar e como poderíamos melhorar a experiência da CLI.</span><span class="sxs-lookup"><span data-stu-id="c1422-115">Before you uninstall, use the `az feedback` command to give us some reasons why you chose to uninstall and how we could improve the CLI experience.</span></span> <span data-ttu-id="c1422-116">Queremos assegurar que a CLI do Azure não tenha bugs e seja amigável o máximo possível.</span><span class="sxs-lookup"><span data-stu-id="c1422-116">We want to make sure that the Azure CLI is as bug-free and user-friendly as we can make it.</span></span> <span data-ttu-id="c1422-117">Você também pode [registrar um problema do github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="c1422-117">You can also [file a github issue](https://github.com/Azure/azure-cli/issues).</span></span>

<span data-ttu-id="c1422-118">A desinstalação pode ser feita executando o MSI novamente e escolhendo a opção "Desinstalar".</span><span class="sxs-lookup"><span data-stu-id="c1422-118">Uninstalling can be done by running the MSI again, and choosing the "Uninstall" option.</span></span> <span data-ttu-id="c1422-119">É possível [baixar o instalador MSI](https://aka.ms/InstallAzureCliWindows) se você o não tiver mais disponível.</span><span class="sxs-lookup"><span data-stu-id="c1422-119">You can [download the MSI installer](https://aka.ms/InstallAzureCliWindows) if you no longer have it available.</span></span>
