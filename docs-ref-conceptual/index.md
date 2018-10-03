---
title: Visão geral da CLI do Azure
description: Visão geral da CLI do Azure.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 047a953a0ab8ccaf145d56e4d774d2bf9852ed6f
ms.sourcegitcommit: c4462456dfb17993f098d47c37bc19f4d78b8179
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/25/2018
ms.locfileid: "47177718"
---
# <a name="azure-cli"></a><span data-ttu-id="7da7d-103">CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="7da7d-103">Azure CLI</span></span>

<span data-ttu-id="7da7d-104">A CLI do Azure é a experiência da linha de comando de plataforma cruzada da Microsoft para gerenciar os recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="7da7d-104">The Azure CLI is Microsoft's cross-platform command-line experience for managing Azure resources.</span></span>
<span data-ttu-id="7da7d-105">Você pode usá-la em seu navegador com o [Azure Cloud Shell](/azure/cloud-shell/overview) ou [instalá-la](install-azure-cli.md) no macOS, Linux ou Windows e executá-la na linha de comando.</span><span class="sxs-lookup"><span data-stu-id="7da7d-105">You can use it in your browser with [Azure Cloud Shell](/azure/cloud-shell/overview), or [install](install-azure-cli.md) it on macOS, Linux, or Windows and run it from the command line.</span></span>

<span data-ttu-id="7da7d-106">A CLI do Azure é simples de usar e é indicada para a criação de scripts de automação que funcionam no Azure Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="7da7d-106">The Azure CLI is simple to get started with, and best used for building automation scripts that work against the Azure Resource Manager.</span></span> <span data-ttu-id="7da7d-107">Com a CLI do Azure, a criação de VMs no Azure é tão fácil quanto digitar o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="7da7d-107">Using the Azure CLI, you can create VMs within Azure as easily as typing the following command:</span></span>

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

## <a name="run-or-install"></a><span data-ttu-id="7da7d-108">Executar ou instalar</span><span class="sxs-lookup"><span data-stu-id="7da7d-108">Run or Install</span></span>

<span data-ttu-id="7da7d-109">Você pode instalar a CLI localmente, executá-la no navegador com o Azure Cloud Shell ou executar em um contêiner do Docker.</span><span class="sxs-lookup"><span data-stu-id="7da7d-109">You can install the CLI locally, run it in the browser with Azure Cloud Shell, or run in a Docker container.</span></span>

* <span data-ttu-id="7da7d-110">Para executar no seu navegador com o Azure Cloud Shell, consulte [Início rápido para Bash no Azure Cloud Shell](/azure/cloud-shell/quickstart) ou [Início rápido para PowerShell no Azure Cloud Shell](/azure/cloud-shell/quickstart-powershell).</span><span class="sxs-lookup"><span data-stu-id="7da7d-110">To run in your browser with Azure Cloud Shell, see [Quickstart for Bash in Azure Cloud Shell](/azure/cloud-shell/quickstart) or [Quickstart for PowerShell in Azure Cloud Shell](/azure/cloud-shell/quickstart-powershell).</span></span>
* <span data-ttu-id="7da7d-111">Para instalar a CLI, confira [Instalar a CLI do Azure](install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="7da7d-111">To install the CLI, see [Install the Azure CLI](install-azure-cli.md).</span></span>
* <span data-ttu-id="7da7d-112">Para ser executado como um contêiner do Docker, confira [Executar a CLI do Azure em um contêiner do Docker](run-azure-cli-docker.md)</span><span class="sxs-lookup"><span data-stu-id="7da7d-112">To run as a Docker container, see [Run Azure CLI in a Docker Container](run-azure-cli-docker.md)</span></span>

## <a name="build-your-skills-with-microsoft-learn"></a><span data-ttu-id="7da7d-113">Desenvolva suas habilidades com o Microsoft Learn</span><span class="sxs-lookup"><span data-stu-id="7da7d-113">Build your skills with Microsoft Learn</span></span>

- [<span data-ttu-id="7da7d-114">Gerenciar máquinas virtuais com a CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="7da7d-114">Manage virtual machines with the Azure CLI</span></span>](/learn/modules/manage-virtual-machines-with-azure-cli/)
- [<span data-ttu-id="7da7d-115">Controlar os serviços do Azure com a CLI</span><span class="sxs-lookup"><span data-stu-id="7da7d-115">Control Azure services with the CLI</span></span>](/learn/modules/control-azure-services-with-cli/)
- [<span data-ttu-id="7da7d-116">Mais aprendizado interativo...</span><span class="sxs-lookup"><span data-stu-id="7da7d-116">More interactive learning...</span></span>](/learn/browse/?products=azure-clis)

## <a name="get-started"></a><span data-ttu-id="7da7d-117">Introdução</span><span class="sxs-lookup"><span data-stu-id="7da7d-117">Get started</span></span>

<span data-ttu-id="7da7d-118">Leia o artigo de [Introdução](get-started-with-azure-cli.md) para aprender os conceitos básicos sobre a CLI.</span><span class="sxs-lookup"><span data-stu-id="7da7d-118">Read the [Get Started](get-started-with-azure-cli.md) article to learn the CLI basics.</span></span> <span data-ttu-id="7da7d-119">Os exemplos a seguir demonstram que alguns casos de uso comuns:</span><span class="sxs-lookup"><span data-stu-id="7da7d-119">The following samples demonstrate some common uses cases:</span></span>

- [<span data-ttu-id="7da7d-120">Máquinas Virtuais do Linux</span><span class="sxs-lookup"><span data-stu-id="7da7d-120">Linux Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="7da7d-121">Máquinas Virtuais do Windows</span><span class="sxs-lookup"><span data-stu-id="7da7d-121">Windows Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="7da7d-122">Aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="7da7d-122">Web Apps</span></span>](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="7da7d-123">Banco de Dados SQL</span><span class="sxs-lookup"><span data-stu-id="7da7d-123">SQL Database</span></span>](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)

<span data-ttu-id="7da7d-124">Além disso, uma [referência](/cli/azure/reference-index) detalhada está disponível e documenta a forma de usar cada comando individual da CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="7da7d-124">A detailed [reference](/cli/azure/reference-index) is also available that documents how to use each individual Azure CLI command.</span></span>

> [!NOTE]
> <span data-ttu-id="7da7d-125">Se você usa a versão anterior da CLI (CLI clássica do Azure), continue a usá-la.</span><span class="sxs-lookup"><span data-stu-id="7da7d-125">If you use the previous version of the CLI (Azure classic CLI), you can continue to use it.</span></span>
> <span data-ttu-id="7da7d-126">No entanto, recomendamos a atualização para a versão mais recente da CLI do Azure a fim de ter a melhor experiência.</span><span class="sxs-lookup"><span data-stu-id="7da7d-126">However, we recommend updating to use the latest version of the Azure CLI for the best experience.</span></span>
> <span data-ttu-id="7da7d-127">Se você usa as duas CLIs, lembre-se de que `azure` é da CLI clássica e `az` é da CLI mais recente.</span><span class="sxs-lookup"><span data-stu-id="7da7d-127">If you use both CLIs, remember that `azure` is the classic CLI and that `az` is the most recent CLI.</span></span>
