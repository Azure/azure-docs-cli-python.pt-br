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
ms.openlocfilehash: 2f4f9950dd663ae85f41bf4efe114b15770ace5d
ms.sourcegitcommit: bcf93ad8ed8802072249cd8187cd4420da89b4c6
ms.translationtype: HT
ms.contentlocale: pt-BR
---
# <a name="azure-cli-20"></a><span data-ttu-id="571cb-104">CLI do Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="571cb-104">Azure CLI 2.0</span></span>

<span data-ttu-id="571cb-105">A CLI 2.0 do Azure é a nova experiência de linha de comando do Azure para gerenciar recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="571cb-105">The Azure CLI 2.0 is Azure's new command-line experience for managing Azure resources.</span></span>  <span data-ttu-id="571cb-106">Ela pode ser usada em Windows, Linux e macOS.</span><span class="sxs-lookup"><span data-stu-id="571cb-106">It can be used on macOS, Linux, and Windows.</span></span> 

<span data-ttu-id="571cb-107">A CLI do Azure 2.0 foi projetada para gerenciar e administrar os recursos do Azure da linha de comando e para a compilação de scripts de automação que funcionam no Azure Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="571cb-107">Azure CLI 2.0 is optimized for managing and administering Azure resources from the command line, and for building automation scripts that work against the Azure Resource Manager.</span></span> <span data-ttu-id="571cb-108">Com a CLI do Azure 2.0, a criação de VMs no Azure é tão fácil quanto digitar o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="571cb-108">Using the Azure CLI 2.0, you can create VMs within Azure as easily as typing the following command:</span></span>

```azurecli
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

<span data-ttu-id="571cb-109">Examine o artigo [Instalar](install-azure-cli.md) para colocar a CLI do Azure 2.0 em funcionamento no sistema.</span><span class="sxs-lookup"><span data-stu-id="571cb-109">Review the [Install article](install-azure-cli.md) to get Azure CLI 2.0 up and running on your system.</span></span> <span data-ttu-id="571cb-110">Em seguida, leia o artigo de [Introdução](get-started-with-azure-cli.md) para começar a usá-lo.</span><span class="sxs-lookup"><span data-stu-id="571cb-110">Then read the [Get Started](get-started-with-azure-cli.md) article to begin using it.</span></span>
<span data-ttu-id="571cb-111">Para saber mais sobre a versão mais recente, consulte as [notas de versão](release-notes-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="571cb-111">For information about the latest release, see the [release notes](release-notes-azure-cli.md).</span></span>

<span data-ttu-id="571cb-112">Os exemplos a seguir podem ajudar você a saber mais sobre como executar cenários comuns com a CLI do Azure 2.0:</span><span class="sxs-lookup"><span data-stu-id="571cb-112">The following samples can help you learn how to perform common scenarios with Azure CLI 2.0:</span></span>
- [<span data-ttu-id="571cb-113">Máquinas Virtuais do Linux</span><span class="sxs-lookup"><span data-stu-id="571cb-113">Linux Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="571cb-114">Máquinas Virtuais do Windows</span><span class="sxs-lookup"><span data-stu-id="571cb-114">Windows Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="571cb-115">Aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="571cb-115">Web Apps</span></span>](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="571cb-116">Banco de Dados SQL</span><span class="sxs-lookup"><span data-stu-id="571cb-116">SQL Database</span></span>](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)

<span data-ttu-id="571cb-117">Além disso, uma [referência](/cli/azure/) detalhada está disponível e documenta a forma de usar cada comando individual da CLI do Azure 2.0.</span><span class="sxs-lookup"><span data-stu-id="571cb-117">A detailed [reference](/cli/azure/) is also available that documents how to use each individual Azure CLI 2.0 command.</span></span>

<span data-ttu-id="571cb-118">[Comece a usar](get-started-with-azure-cli.md) a CLI do Azure 2.0 agora.</span><span class="sxs-lookup"><span data-stu-id="571cb-118">[Get started](get-started-with-azure-cli.md) with Azure CLI 2.0 now.</span></span>


> [!NOTE]
> <span data-ttu-id="571cb-119">Se você usa a versão anterior da CLI (CLI do Azure), continue a usá-la.</span><span class="sxs-lookup"><span data-stu-id="571cb-119">If you use the previous version of the CLI (Azure CLI), you can continue to use it.</span></span>
> <span data-ttu-id="571cb-120">Se você usa ambas CLIs, lembre-se de que `azure` é a CLI antiga (CLI do Azure) e que `az` é a nova CLI (CLI do Azure 2.0).</span><span class="sxs-lookup"><span data-stu-id="571cb-120">If you use both CLIs, remember that `azure` is the old CLI - Azure CLI, and that `az` is the new CLI - Azure CLI 2.0.</span></span> 