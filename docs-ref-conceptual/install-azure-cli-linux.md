---
title: Instalar a CLI do Azure para Linux manualmente
description: Como instalar a CLI do Azure no Linux manualmente
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 12/15/2020
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
zone_pivot_group_filename: azure/zone-pivot-groups.json
zone_pivot_groups: cli-linux-installation-method
ms.openlocfilehash: 3b6a3c9faa8424189bb5d4ffaeb17bdfc7de0d6d
ms.sourcegitcommit: d5f026468ea20bbd7ef35bdbf9852bcb2b812d83
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/23/2020
ms.locfileid: "97744592"
---
# <a name="install-the-azure-cli-on-linux"></a><span data-ttu-id="8f08d-103">Instalar a CLI do Azure no Linux</span><span class="sxs-lookup"><span data-stu-id="8f08d-103">Install the Azure CLI on Linux</span></span>

<span data-ttu-id="8f08d-104">É recomendável instalar a CLI do Azure usando o gerenciador de pacotes da distribuição do Linux.</span><span class="sxs-lookup"><span data-stu-id="8f08d-104">It is recommended to install the Azure CLI using your Linux distribution's package manager.</span></span> <span data-ttu-id="8f08d-105">Selecione o gerenciador de pacotes apropriado para a sua distribuição nas opções acima.</span><span class="sxs-lookup"><span data-stu-id="8f08d-105">Select the appropriate package manager for your distribution from the options above.</span></span>  <span data-ttu-id="8f08d-106">Se você não tiver nenhum dos gerenciadores de pacotes listados, poderá instalar manualmente a CLI do Azure selecionando a opção *Instalar script*.</span><span class="sxs-lookup"><span data-stu-id="8f08d-106">If you do not have one of the listed package managers, you may manually install the Azure CLI by selecting the *Install script* option.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

::: zone pivot="apt"

[!INCLUDE [cli-install-linux-apt](includes/cli-install-linux-apt.md)]

::: zone-end

::: zone pivot="yum"

[!INCLUDE [cli-install-linux-apt](includes/cli-install-linux-yum.md)]

::: zone-end

::: zone pivot="zypper"

[!INCLUDE [cli-install-linux-apt](includes/cli-install-linux-zypper.md)]

::: zone-end

::: zone pivot="script"

[!INCLUDE [cli-install-linux-apt](includes/cli-install-linux-script.md)]

::: zone-end

## <a name="next-steps"></a><span data-ttu-id="8f08d-107">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="8f08d-107">Next Steps</span></span>

<span data-ttu-id="8f08d-108">Agora que você instalou a CLI do Azure, faça um tour breve de seus recursos e comandos comuns.</span><span class="sxs-lookup"><span data-stu-id="8f08d-108">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="8f08d-109">Introdução à CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="8f08d-109">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)