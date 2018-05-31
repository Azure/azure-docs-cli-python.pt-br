---
title: CLI do Azure 2.0
description: Visão geral da CLI do Azure 2.0.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/16/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 9b6f7a5c79033c0b0bec2bf8b56eb40831484f1a
ms.sourcegitcommit: 8b4629a42ceecf30c1efbc6fdddf512f4dddfab0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/18/2018
ms.locfileid: "34306243"
---
# <a name="azure-cli-20"></a><span data-ttu-id="3ae84-103">CLI do Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="3ae84-103">Azure CLI 2.0</span></span>

<span data-ttu-id="3ae84-104">A CLI do Azure 2.0 é a experiência da linha de comando entre plataformas da Microsoft para gerenciar os recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="3ae84-104">The Azure CLI 2.0 is Microsoft's cross-platform command line experience for managing Azure resources.</span></span>
<span data-ttu-id="3ae84-105">Você pode usá-la em seu navegador com o [Azure Cloud Shell](/azure/cloud-shell/overview) ou [instalá-la](install-azure-cli.md) no macOS, Linux ou Windows e executá-la na linha de comando.</span><span class="sxs-lookup"><span data-stu-id="3ae84-105">You can use it in your browser with [Azure Cloud Shell](/azure/cloud-shell/overview), or [install](install-azure-cli.md) it on macOS, Linux, or Windows and run it from the command line.</span></span>

<span data-ttu-id="3ae84-106">A CLI do Azure 2.0 foi projetada para gerenciar e administrar os recursos do Azure da linha de comando e para a compilação de scripts de automação que funcionam no Azure Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="3ae84-106">Azure CLI 2.0 is optimized for managing and administering Azure resources from the command line, and for building automation scripts that work against the Azure Resource Manager.</span></span> <span data-ttu-id="3ae84-107">Com a CLI do Azure 2.0, a criação de VMs no Azure é tão fácil quanto digitar o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="3ae84-107">Using the Azure CLI 2.0, you can create VMs within Azure as easily as typing the following command:</span></span>

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

<span data-ttu-id="3ae84-108">Use o [Cloud Shell](/azure/cloud-shell/overview) para executar a CLI no seu navegador ou [instale-o](install-azure-cli.md) no macOS, Linux ou Windows.</span><span class="sxs-lookup"><span data-stu-id="3ae84-108">Use the [Cloud Shell](/azure/cloud-shell/overview) to run the CLI in your browser, or [install](install-azure-cli.md) it on macOS, Linux, or Windows.</span></span>
<span data-ttu-id="3ae84-109">Leia o artigo de [Introdução](get-started-with-azure-cli.md) para começar a usar a CLI.</span><span class="sxs-lookup"><span data-stu-id="3ae84-109">Read the [Get Started](get-started-with-azure-cli.md) article to begin using the CLI.</span></span>
<span data-ttu-id="3ae84-110">Para saber mais sobre a versão mais recente, veja as [notas de versão](release-notes-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="3ae84-110">For information about the latest release, see the [release notes](release-notes-azure-cli.md).</span></span>

<span data-ttu-id="3ae84-111">Os exemplos a seguir o ajudarão a começar com as tarefas comuns na CLI do Azure 2.0:</span><span class="sxs-lookup"><span data-stu-id="3ae84-111">The following samples help you get started with common tasks in Azure CLI 2.0:</span></span>
- [<span data-ttu-id="3ae84-112">Máquinas Virtuais do Linux</span><span class="sxs-lookup"><span data-stu-id="3ae84-112">Linux Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- <span data-ttu-id="3ae84-113">Interativo: [Criar máquinas virtuais do Linux](https://docs.microsoft.com/learn/azure-cli-2-0/index)</span><span class="sxs-lookup"><span data-stu-id="3ae84-113">Interactive: [Create Linux Virtual Machines](https://docs.microsoft.com/learn/azure-cli-2-0/index)</span></span>
- [<span data-ttu-id="3ae84-114">Máquinas Virtuais do Windows</span><span class="sxs-lookup"><span data-stu-id="3ae84-114">Windows Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="3ae84-115">Aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="3ae84-115">Web Apps</span></span>](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="3ae84-116">Banco de Dados SQL</span><span class="sxs-lookup"><span data-stu-id="3ae84-116">SQL Database</span></span>](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)

<span data-ttu-id="3ae84-117">Além disso, uma [referência](/cli/azure/reference-index) detalhada está disponível e documenta a forma de usar cada comando individual da CLI do Azure 2.0.</span><span class="sxs-lookup"><span data-stu-id="3ae84-117">A detailed [reference](/cli/azure/reference-index) is also available that documents how to use each individual Azure CLI 2.0 command.</span></span>

<span data-ttu-id="3ae84-118">[Comece a usar](get-started-with-azure-cli.md) a CLI do Azure 2.0 agora.</span><span class="sxs-lookup"><span data-stu-id="3ae84-118">[Get started](get-started-with-azure-cli.md) with Azure CLI 2.0 now.</span></span>

> [!NOTE]
> <span data-ttu-id="3ae84-119">Se você usa a versão anterior da CLI (CLI do Azure 1.0), pode continuar a usá-la.</span><span class="sxs-lookup"><span data-stu-id="3ae84-119">If you use the previous version of the CLI (Azure CLI 1.0), you can continue to use it.</span></span>
> <span data-ttu-id="3ae84-120">No entanto, é recomendável atualizar para usar a versão mais recente da CLI do Azure 2.0 para ter a melhor experiência.</span><span class="sxs-lookup"><span data-stu-id="3ae84-120">However, we recommend updating to use the latest version of Azure CLI 2.0 for the best experience.</span></span>
> <span data-ttu-id="3ae84-121">Se você usa ambas CLIs, lembre-se de que `azure` é a CLI antiga (CLI do Azure) e que `az` é a nova CLI (CLI do Azure 2.0).</span><span class="sxs-lookup"><span data-stu-id="3ae84-121">If you use both CLIs, remember that `azure` is the old CLI - Azure CLI, and that `az` is the new CLI - Azure CLI 2.0.</span></span>
