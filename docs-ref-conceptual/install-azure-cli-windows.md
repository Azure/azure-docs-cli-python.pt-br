---
title: Instalar a CLI do Azure para Windows
description: Como instalar a CLI do Azure no Windows
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/01/2019
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: c5c499800e49dcdc536337e7655ec1ee280d48f2
ms.sourcegitcommit: 65bf8561a6e047e4eab52186e066a2e8c21f1d40
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2019
ms.locfileid: "65240553"
---
# <a name="install-azure-cli-on-windows"></a><span data-ttu-id="46e75-103">Instalar a CLI do Azure no Windows</span><span class="sxs-lookup"><span data-stu-id="46e75-103">Install Azure CLI on Windows</span></span>

<span data-ttu-id="46e75-104">Para Windows, a CLI do Azure é instalada por meio de um MSI, o que fornece acesso à CLI por meio do Prompt de Comando do Windows (CMD) ou o PowerShell.</span><span class="sxs-lookup"><span data-stu-id="46e75-104">For Windows the Azure CLI is installed via an MSI, which gives you access to the CLI through the Windows Command Prompt (CMD) or PowerShell.</span></span>
<span data-ttu-id="46e75-105">Ao instalar o Subsistema do Windows para Linux (WSL), há pacotes disponíveis para a distribuição do Linux.</span><span class="sxs-lookup"><span data-stu-id="46e75-105">When installing for Windows Subsystem for Linux (WSL), packages are available for your Linux distribution.</span></span> <span data-ttu-id="46e75-106">Consulte a [página instalação principal](install-azure-cli.md) para ver a lista de gerenciadores de pacotes com suporte ou como instalar manualmente no WSL.</span><span class="sxs-lookup"><span data-stu-id="46e75-106">See the [main install page](install-azure-cli.md) for the list of supported package managers or how to install manually under WSL.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

## <a name="install-or-update"></a><span data-ttu-id="46e75-107">Instalar ou atualizar</span><span class="sxs-lookup"><span data-stu-id="46e75-107">Install or update</span></span>

<span data-ttu-id="46e75-108">O MSI distribuível é usado para instalar ou atualizar a CLI do Azure no Windows.</span><span class="sxs-lookup"><span data-stu-id="46e75-108">The MSI distributable is used for installing or updating the Azure CLI on Windows.</span></span> <span data-ttu-id="46e75-109">Você não precisa desinstalar as versões atuais antes de usar o instalador MSI.</span><span class="sxs-lookup"><span data-stu-id="46e75-109">You don't need to uninstall any current versions before using the MSI installer.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="46e75-110">Baixe o instalador MSI</span><span class="sxs-lookup"><span data-stu-id="46e75-110">Download the MSI installer</span></span>](https://aka.ms/installazurecliwindows)

<span data-ttu-id="46e75-111">Quando o instalador perguntar se pode fazer alterações no computador, clique na caixa "Sim".</span><span class="sxs-lookup"><span data-stu-id="46e75-111">When the installer asks if it can make changes to your computer, click the "Yes" box.</span></span>

<span data-ttu-id="46e75-112">Agora, você pode executar a CLI do Azure com o comando `az` no Prompt de Comando do Windows ou no PowerShell.</span><span class="sxs-lookup"><span data-stu-id="46e75-112">You can now run the Azure CLI with the `az` command from either Windows Command Prompt or PowerShell.</span></span> <span data-ttu-id="46e75-113">O PowerShell oferece alguns recursos de conclusão de guia não disponíveis no prompt de comando do Windows.</span><span class="sxs-lookup"><span data-stu-id="46e75-113">PowerShell offers some tab completion features not available from Windows Command Prompt.</span></span> <span data-ttu-id="46e75-114">Para entrar, execute o comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="46e75-114">To sign in, run the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="46e75-115">Para saber mais sobre os diferentes métodos de autenticação, confira [Entrar com a CLI do Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="46e75-115">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="uninstall"></a><span data-ttu-id="46e75-116">Desinstalar</span><span class="sxs-lookup"><span data-stu-id="46e75-116">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="46e75-117">Desinstale a CLI do Azure da lista de "Aplicativos e recursos" do Windows.</span><span class="sxs-lookup"><span data-stu-id="46e75-117">You uninstall the Azure CLI from the Windows "Apps and Features" list.</span></span> <span data-ttu-id="46e75-118">Para desinstalar:</span><span class="sxs-lookup"><span data-stu-id="46e75-118">To uninstall:</span></span>

| <span data-ttu-id="46e75-119">Plataforma</span><span class="sxs-lookup"><span data-stu-id="46e75-119">Platform</span></span> | <span data-ttu-id="46e75-120">Instruções</span><span class="sxs-lookup"><span data-stu-id="46e75-120">Instructions</span></span> |
|---|---|
| <span data-ttu-id="46e75-121">Windows 10</span><span class="sxs-lookup"><span data-stu-id="46e75-121">Windows 10</span></span> | <span data-ttu-id="46e75-122">Iniciar > Configurações > Aplicativos</span><span class="sxs-lookup"><span data-stu-id="46e75-122">Start > Settings > Apps</span></span> |
| <span data-ttu-id="46e75-123">Windows 8</span><span class="sxs-lookup"><span data-stu-id="46e75-123">Windows 8</span></span><br/><span data-ttu-id="46e75-124">Windows 7</span><span class="sxs-lookup"><span data-stu-id="46e75-124">Windows 7</span></span> | <span data-ttu-id="46e75-125">Iniciar > Painel de Controle > Programas > Desinstalar um programa</span><span class="sxs-lookup"><span data-stu-id="46e75-125">Start > Control Panel > Programs > Uninstall a program</span></span> |

<span data-ttu-id="46e75-126">Uma vez nessa tela, digite __CLI do Azure__ na barra de pesquisa do programa.</span><span class="sxs-lookup"><span data-stu-id="46e75-126">Once on this screen type __Azure CLI__ into the program search bar.</span></span> <span data-ttu-id="46e75-127">O programa de desinstalação aparece como __Microsoft CLI 2.0 para Azure__.</span><span class="sxs-lookup"><span data-stu-id="46e75-127">The program to uninstall is listed as __Microsoft CLI 2.0 for Azure__.</span></span> <span data-ttu-id="46e75-128">Selecione este aplicativo e clique no botão `Uninstall`.</span><span class="sxs-lookup"><span data-stu-id="46e75-128">Select this application, then click the `Uninstall` button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="46e75-129">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="46e75-129">Next Steps</span></span>

<span data-ttu-id="46e75-130">Agora que você instalou a CLI do Azure, faça um tour breve de seus recursos e comandos comuns.</span><span class="sxs-lookup"><span data-stu-id="46e75-130">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="46e75-131">Introdução à CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="46e75-131">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
