---
title: CLI do Azure 2.0
description: "Visão geral da CLI do Azure 2.0."
keywords: CLI do Azure 2.0, Linux, Mac, Windows, OS X, Ubuntu, Debian, CentOS, RHEL, SUSE, CoreOS, Docker, Windows, Python, PIP
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 80ae9f6c-adb7-483c-bfb4-fbb958e075ba
ms.openlocfilehash: 36a08835b9c4f6e71c5ddadbce8ba946c52a1e9b
ms.sourcegitcommit: 4fd631a58cf19c494162510d073fbbbdf0524d16
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/05/2017
---
# <a name="azure-cli-20"></a><span data-ttu-id="e4f9a-104">CLI do Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="e4f9a-104">Azure CLI 2.0</span></span>

<span data-ttu-id="e4f9a-105">A CLI 2.0 do Azure é a nova experiência de linha de comando do Azure para gerenciar recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="e4f9a-105">The Azure CLI 2.0 is Azure's new command-line experience for managing Azure resources.</span></span>
<span data-ttu-id="e4f9a-106">Você pode usá-lo no seu navegador com o [Azure Cloud Shell](/azure/cloud-shell/overview) ou pode [instalá-lo](install-azure-cli.md) no macOS, Linux e Windows e executá-lo da linha de comando.</span><span class="sxs-lookup"><span data-stu-id="e4f9a-106">You can use it in your browser with [Azure Cloud Shell](/azure/cloud-shell/overview), or you can [install](install-azure-cli.md) it on macOS, Linux, and Windows and run it from the command line.</span></span>

<span data-ttu-id="e4f9a-107">A CLI do Azure 2.0 foi projetada para gerenciar e administrar os recursos do Azure da linha de comando e para a compilação de scripts de automação que funcionam no Azure Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="e4f9a-107">Azure CLI 2.0 is optimized for managing and administering Azure resources from the command line, and for building automation scripts that work against the Azure Resource Manager.</span></span> <span data-ttu-id="e4f9a-108">Com a CLI do Azure 2.0, a criação de VMs no Azure é tão fácil quanto digitar o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="e4f9a-108">Using the Azure CLI 2.0, you can create VMs within Azure as easily as typing the following command:</span></span>

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

<span data-ttu-id="e4f9a-109">Use o [Cloud Shell](/azure/cloud-shell/overview) para executar a CLI no seu navegador ou [instale-o](install-azure-cli.md) no macOS, Linux ou Windows.</span><span class="sxs-lookup"><span data-stu-id="e4f9a-109">Use the [Cloud Shell](/azure/cloud-shell/overview) to run the CLI in your browser, or [install](install-azure-cli.md) it on macOS, Linux, or Windows.</span></span>
<span data-ttu-id="e4f9a-110">Leia o artigo de [Introdução](get-started-with-azure-cli.md) para começar a usar a CLI.</span><span class="sxs-lookup"><span data-stu-id="e4f9a-110">Read the [Get Started](get-started-with-azure-cli.md) article to begin using the CLI.</span></span>
<span data-ttu-id="e4f9a-111">Para saber mais sobre a versão mais recente, veja as [notas de versão](release-notes-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="e4f9a-111">For information about the latest release, see the [release notes](release-notes-azure-cli.md).</span></span>

<span data-ttu-id="e4f9a-112">Os exemplos a seguir podem ajudar você a saber mais sobre como executar cenários comuns com a CLI do Azure 2.0:</span><span class="sxs-lookup"><span data-stu-id="e4f9a-112">The following samples can help you learn how to perform common scenarios with Azure CLI 2.0:</span></span>
- [<span data-ttu-id="e4f9a-113">Máquinas Virtuais do Linux</span><span class="sxs-lookup"><span data-stu-id="e4f9a-113">Linux Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="e4f9a-114">Máquinas Virtuais do Windows</span><span class="sxs-lookup"><span data-stu-id="e4f9a-114">Windows Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="e4f9a-115">Aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="e4f9a-115">Web Apps</span></span>](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="e4f9a-116">Banco de Dados SQL</span><span class="sxs-lookup"><span data-stu-id="e4f9a-116">SQL Database</span></span>](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)

<span data-ttu-id="e4f9a-117">Além disso, uma [referência](/cli/azure/) detalhada está disponível e documenta a forma de usar cada comando individual da CLI do Azure 2.0.</span><span class="sxs-lookup"><span data-stu-id="e4f9a-117">A detailed [reference](/cli/azure/) is also available that documents how to use each individual Azure CLI 2.0 command.</span></span>

<span data-ttu-id="e4f9a-118">[Comece a usar](get-started-with-azure-cli.md) a CLI do Azure 2.0 agora.</span><span class="sxs-lookup"><span data-stu-id="e4f9a-118">[Get started](get-started-with-azure-cli.md) with Azure CLI 2.0 now.</span></span>


> [!NOTE]
> <span data-ttu-id="e4f9a-119">Se você usa a versão anterior da CLI (CLI do Azure), continue a usá-la.</span><span class="sxs-lookup"><span data-stu-id="e4f9a-119">If you use the previous version of the CLI (Azure CLI), you can continue to use it.</span></span>
> <span data-ttu-id="e4f9a-120">Se você usa ambas CLIs, lembre-se de que `azure` é a CLI antiga (CLI do Azure) e que `az` é a nova CLI (CLI do Azure 2.0).</span><span class="sxs-lookup"><span data-stu-id="e4f9a-120">If you use both CLIs, remember that `azure` is the old CLI - Azure CLI, and that `az` is the new CLI - Azure CLI 2.0.</span></span> 