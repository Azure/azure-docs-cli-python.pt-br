---
title: Visão geral da CLI do Azure 2.0
description: Visão geral da CLI do Azure 2.0.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 55c5ea3ad69df60d211cc076e3570e9f07040af7
ms.sourcegitcommit: 0e688704889fc88b91588bb6678a933c2d54f020
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/11/2018
ms.locfileid: "44388370"
---
# <a name="azure-cli-20"></a><span data-ttu-id="9eb61-103">CLI do Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="9eb61-103">Azure CLI 2.0</span></span>

<span data-ttu-id="9eb61-104">A CLI do Azure 2.0 é a experiência da linha de comando entre plataformas da Microsoft para gerenciar os recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="9eb61-104">The Azure CLI 2.0 is Microsoft's cross-platform command-line experience for managing Azure resources.</span></span>
<span data-ttu-id="9eb61-105">Você pode usá-la em seu navegador com o [Azure Cloud Shell](/azure/cloud-shell/overview) ou [instalá-la](install-azure-cli.md) no macOS, Linux ou Windows e executá-la na linha de comando.</span><span class="sxs-lookup"><span data-stu-id="9eb61-105">You can use it in your browser with [Azure Cloud Shell](/azure/cloud-shell/overview), or [install](install-azure-cli.md) it on macOS, Linux, or Windows and run it from the command line.</span></span>

<span data-ttu-id="9eb61-106">A CLI 2.0 do Azure é simples de usar e é indicada para a criação de scripts de automação que funcionam no Azure Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="9eb61-106">Azure CLI 2.0 is simple to get started with, and best used for building automation scripts that work against the Azure Resource Manager.</span></span> <span data-ttu-id="9eb61-107">Com a CLI do Azure 2.0, a criação de VMs no Azure é tão fácil quanto digitar o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="9eb61-107">Using the Azure CLI 2.0, you can create VMs within Azure as easily as typing the following command:</span></span>

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

## <a name="run-or-install"></a><span data-ttu-id="9eb61-108">Executar ou instalar</span><span class="sxs-lookup"><span data-stu-id="9eb61-108">Run or Install</span></span>

<span data-ttu-id="9eb61-109">Você pode instalar a CLI localmente, executá-la no navegador com o Azure Cloud Shell ou executar em um contêiner do Docker.</span><span class="sxs-lookup"><span data-stu-id="9eb61-109">You can install the CLI locally, run it in the browser with Azure Cloud Shell, or run in a Docker container.</span></span>

* <span data-ttu-id="9eb61-110">Para executar no seu navegador com o Azure Cloud Shell, consulte [Início rápido para Bash no Azure Cloud Shell](/azure/cloud-shell/quickstart) ou [Início rápido para PowerShell no Azure Cloud Shell](/azure/cloud-shell/quickstart-powershell).</span><span class="sxs-lookup"><span data-stu-id="9eb61-110">To run in your browser with Azure Cloud Shell, see [Quickstart for Bash in Azure Cloud Shell](/azure/cloud-shell/quickstart) or [Quickstart for PowerShell in Azure Cloud Shell](/azure/cloud-shell/quickstart-powershell).</span></span>
* <span data-ttu-id="9eb61-111">Para instalar a CLI, confira [Instalar a CLI do Azure 2.0](install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="9eb61-111">To install the CLI, see [Install the Azure CLI 2.0](install-azure-cli.md).</span></span>
* <span data-ttu-id="9eb61-112">Para ser executado como um contêiner do Docker, consulte [Executar CLI do Azure 2.0 em um contêiner do Docker](run-azure-cli-docker.md)</span><span class="sxs-lookup"><span data-stu-id="9eb61-112">To run as a Docker container, see [Run Azure CLI 2.0 in a Docker Container](run-azure-cli-docker.md)</span></span>

## <a name="get-started"></a><span data-ttu-id="9eb61-113">Introdução</span><span class="sxs-lookup"><span data-stu-id="9eb61-113">Get started</span></span>

<span data-ttu-id="9eb61-114">Leia o artigo de [Introdução](get-started-with-azure-cli.md) para aprender os conceitos básicos sobre a CLI.</span><span class="sxs-lookup"><span data-stu-id="9eb61-114">Read the [Get Started](get-started-with-azure-cli.md) article to learn the CLI basics.</span></span> <span data-ttu-id="9eb61-115">Os exemplos a seguir demonstram que alguns casos de uso comuns:</span><span class="sxs-lookup"><span data-stu-id="9eb61-115">The following samples demonstrate some common uses cases:</span></span>

- [<span data-ttu-id="9eb61-116">Máquinas Virtuais do Linux</span><span class="sxs-lookup"><span data-stu-id="9eb61-116">Linux Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="9eb61-117">Máquinas Virtuais do Windows</span><span class="sxs-lookup"><span data-stu-id="9eb61-117">Windows Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="9eb61-118">Aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="9eb61-118">Web Apps</span></span>](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="9eb61-119">Banco de Dados SQL</span><span class="sxs-lookup"><span data-stu-id="9eb61-119">SQL Database</span></span>](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)

<span data-ttu-id="9eb61-120">Além disso, uma [referência](/cli/azure/reference-index) detalhada está disponível e documenta a forma de usar cada comando individual da CLI do Azure 2.0.</span><span class="sxs-lookup"><span data-stu-id="9eb61-120">A detailed [reference](/cli/azure/reference-index) is also available that documents how to use each individual Azure CLI 2.0 command.</span></span>

> [!NOTE]
> <span data-ttu-id="9eb61-121">Se você usa a versão anterior da CLI (CLI do Azure 1.0), pode continuar a usá-la.</span><span class="sxs-lookup"><span data-stu-id="9eb61-121">If you use the previous version of the CLI (Azure CLI 1.0), you can continue to use it.</span></span>
> <span data-ttu-id="9eb61-122">No entanto, é recomendável atualizar para usar a versão mais recente da CLI do Azure 2.0 para ter a melhor experiência.</span><span class="sxs-lookup"><span data-stu-id="9eb61-122">However, we recommend updating to use the latest version of Azure CLI 2.0 for the best experience.</span></span>
> <span data-ttu-id="9eb61-123">Se você usa ambas CLIs, lembre-se de que `azure` é a CLI antiga (CLI do Azure) e que `az` é a nova CLI (CLI do Azure 2.0).</span><span class="sxs-lookup"><span data-stu-id="9eb61-123">If you use both CLIs, remember that `azure` is the old CLI - Azure CLI, and that `az` is the new CLI - Azure CLI 2.0.</span></span>
