---
title: Atualizar a CLI do Azure
description: Referência para a atualização da CLI do Azure
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 10/19/2020
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 475b58bca5ec9dca52a70416cb89860dcbd39278
ms.sourcegitcommit: e1faf297ba2cdf2ba7e821fbeedff9c9a724c975
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "97576778"
---
# <a name="update-the-azure-cli"></a><span data-ttu-id="55d89-103">Atualizar a CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="55d89-103">Update the Azure CLI</span></span>

<span data-ttu-id="55d89-104">Você pode contar com os gerenciadores de pacotes para atualizar uma instalação local da CLI do Azure em ambientes Windows, macOS e Linux (confira a seção `Update` em cada instrução de instalação específica da plataforma).</span><span class="sxs-lookup"><span data-stu-id="55d89-104">You can rely on package managers to update a local install of the Azure CLI on Windows, macOS and Linux environments (see the `Update` section in each platform-specific install instruction).</span></span> <span data-ttu-id="55d89-105">A CLI também fornece comandos dentro ferramenta para atualização manual ou automática.</span><span class="sxs-lookup"><span data-stu-id="55d89-105">The CLI also provides in-tool commands to upgrade manually or automatically.</span></span>

## <a name="manual-update"></a><span data-ttu-id="55d89-106">Atualização manual</span><span class="sxs-lookup"><span data-stu-id="55d89-106">Manual Update</span></span>
[!INCLUDE [az-upgrade](includes/az-upgrade.md)]

<span data-ttu-id="55d89-107">O `az upgrade` é compatível com o Windows, o macOS e algumas distribuições do Linux, desde que haja suporte para a instalação.</span><span class="sxs-lookup"><span data-stu-id="55d89-107">`az upgrade` is supported on Windows, macOS and some Linux distros as long as installation is supported.</span></span> <span data-ttu-id="55d89-108">Ele dá suporte apenas à atualização para a versão mais recente.</span><span class="sxs-lookup"><span data-stu-id="55d89-108">It only supports upgrading to the latest version.</span></span> <span data-ttu-id="55d89-109">Se você está executando a CLI do Azure por meio do Azure Cloud Shell, provavelmente já está usando a instalação da CLI do Azure mais recente.</span><span class="sxs-lookup"><span data-stu-id="55d89-109">If you are running the Azure CLI through Azure Cloud Shell, you are most likely already using the most recent Azure CLI install.</span></span> <span data-ttu-id="55d89-110">Exceto em casos como a versão ad hoc de uma versão de correção de bug secundária, você precisará esperar pelo próximo build do Azure Cloud Shell, já que não há suporte para `az upgrade` no Azure Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="55d89-110">If not due to cases like ad-hoc release of a minor bug fix version, you need to wait for the next build of Azure Cloud Shell as `az upgrade` is not supported in Azure Cloud Shell.</span></span>

<span data-ttu-id="55d89-111">Quando `azure-cli` já for a versão mais recente, a execução de `az upgrade` verificará e atualizará todas as [extensões](azure-cli-extensions-overview.md) instaladas.</span><span class="sxs-lookup"><span data-stu-id="55d89-111">When `azure-cli` is already the latest version, running `az upgrade` will check and update all installed [extensions](azure-cli-extensions-overview.md).</span></span>

## <a name="automatic-update"></a><span data-ttu-id="55d89-112">Atualização automática</span><span class="sxs-lookup"><span data-stu-id="55d89-112">Automatic Update</span></span>

<span data-ttu-id="55d89-113">Por padrão, a atualização automática da CLI do Azure está desabilitada.</span><span class="sxs-lookup"><span data-stu-id="55d89-113">By default, auto-upgrade for Azure CLI is disabled.</span></span> <span data-ttu-id="55d89-114">Se você quiser acompanhar a versão mais recente, poderá habilitar a atualização automática por meio da [configuração](/cli/azure/config).</span><span class="sxs-lookup"><span data-stu-id="55d89-114">If you would like to keep up with the latest version, you can enable auto-upgrade through [configuration](/cli/azure/config).</span></span>

```azurecli
az config set auto-upgrade.enable=yes
```

<span data-ttu-id="55d89-115">A CLI do Azure verificará novas versões regularmente e solicitará que você atualize após terminar a execução de qualquer comando quando a atualização estiver disponível.</span><span class="sxs-lookup"><span data-stu-id="55d89-115">The Azure CLI will check new versions regularly and prompt you to upgrade after any command finishes running once the update is available.</span></span>

<span data-ttu-id="55d89-116">A mensagem do prompt e as mensagens de saída durante a atualização poderão interromper o resultado do comando se ele for atribuído a alguma variável ou estiver em um fluxo automatizado.</span><span class="sxs-lookup"><span data-stu-id="55d89-116">The prompt message and output messages during upgrade may interrupt your command result if it is assigned to some variable or in an automated flow.</span></span> <span data-ttu-id="55d89-117">Para evitar a interrupção, você pode usar a configuração a seguir para permitir que a atualização ocorra automaticamente sem confirmação e mostrar apenas avisos e erros durante a atualização.</span><span class="sxs-lookup"><span data-stu-id="55d89-117">To avoid interruption, you can use the following configuration to allow the update to happen automatically without confirmation and only show warnings and errors during the upgrade.</span></span>

```azurecli
az config set auto-upgrade.prompt=no
```

<span data-ttu-id="55d89-118">Por padrão, todas as extensões instaladas também serão atualizadas.</span><span class="sxs-lookup"><span data-stu-id="55d89-118">By default, all installed extensions will also be updated.</span></span> <span data-ttu-id="55d89-119">Você pode desabilitar a atualização de extensão por meio da configuração.</span><span class="sxs-lookup"><span data-stu-id="55d89-119">You can disable extension update through configuration.</span></span>

```azurecli
az config set auto-upgrade.all=no
```

> [!NOTE]
> <span data-ttu-id="55d89-120">Aguarde até que `az upgrade` seja concluído antes de prosseguir para o próximo conjunto de comandos, caso contrário, as novas versões da CLI (+ extensões) poderão ter alterações da falha.</span><span class="sxs-lookup"><span data-stu-id="55d89-120">Please wait for `az upgrade` to complete before proceeding to the next set of commands, else the new versions of the CLI (+extensions) may have breaking changes.</span></span>

<span data-ttu-id="55d89-121">Se você decidir não usar mais o recurso de atualização automática para casos como manter scripts de comando em execução de modo estável, você poderá desativá-lo por meio da configuração.</span><span class="sxs-lookup"><span data-stu-id="55d89-121">If you decide not to use the automatic update feature any more for cases like keeping command scripts running stably, you can turn it off through configuration.</span></span>
```azurecli
az config set auto-upgrade.enable=no
```
