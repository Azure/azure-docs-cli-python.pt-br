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
ms.openlocfilehash: 40810b25bf776025c82b48ba7aa424369483ceeb
ms.sourcegitcommit: 08043c47d3ccf23522b91e6bba3932e312c04c7f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2019
ms.locfileid: "66516267"
---
# <a name="install-azure-cli-on-windows"></a><span data-ttu-id="5e70a-103">Instalar a CLI do Azure no Windows</span><span class="sxs-lookup"><span data-stu-id="5e70a-103">Install Azure CLI on Windows</span></span>

<span data-ttu-id="5e70a-104">Para Windows, a CLI do Azure é instalada por meio de um MSI, o que fornece acesso à CLI por meio do Prompt de Comando do Windows (CMD) ou o PowerShell.</span><span class="sxs-lookup"><span data-stu-id="5e70a-104">For Windows the Azure CLI is installed via an MSI, which gives you access to the CLI through the Windows Command Prompt (CMD) or PowerShell.</span></span>
<span data-ttu-id="5e70a-105">Ao instalar o Subsistema do Windows para Linux (WSL), há pacotes disponíveis para a distribuição do Linux.</span><span class="sxs-lookup"><span data-stu-id="5e70a-105">When installing for Windows Subsystem for Linux (WSL), packages are available for your Linux distribution.</span></span> <span data-ttu-id="5e70a-106">Consulte a [página instalação principal](install-azure-cli.md) para ver a lista de gerenciadores de pacotes com suporte ou como instalar manualmente no WSL.</span><span class="sxs-lookup"><span data-stu-id="5e70a-106">See the [main install page](install-azure-cli.md) for the list of supported package managers or how to install manually under WSL.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

## <a name="install-or-update"></a><span data-ttu-id="5e70a-107">Instalar ou atualizar</span><span class="sxs-lookup"><span data-stu-id="5e70a-107">Install or update</span></span>

<span data-ttu-id="5e70a-108">O MSI distribuível é usado para instalar ou atualizar a CLI do Azure no Windows.</span><span class="sxs-lookup"><span data-stu-id="5e70a-108">The MSI distributable is used for installing or updating the Azure CLI on Windows.</span></span> <span data-ttu-id="5e70a-109">Você não precisa desinstalar as versões atuais antes de usar o instalador MSI.</span><span class="sxs-lookup"><span data-stu-id="5e70a-109">You don't need to uninstall any current versions before using the MSI installer.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="5e70a-110">Baixe o instalador MSI</span><span class="sxs-lookup"><span data-stu-id="5e70a-110">Download the MSI installer</span></span>](https://aka.ms/installazurecliwindows)

<span data-ttu-id="5e70a-111">Quando o instalador perguntar se pode fazer alterações no computador, clique na caixa "Sim".</span><span class="sxs-lookup"><span data-stu-id="5e70a-111">When the installer asks if it can make changes to your computer, click the "Yes" box.</span></span>

<span data-ttu-id="5e70a-112">Agora, você pode executar a CLI do Azure com o comando `az` no Prompt de Comando do Windows ou no PowerShell.</span><span class="sxs-lookup"><span data-stu-id="5e70a-112">You can now run the Azure CLI with the `az` command from either Windows Command Prompt or PowerShell.</span></span> <span data-ttu-id="5e70a-113">O PowerShell oferece alguns recursos de conclusão de guia não disponíveis no prompt de comando do Windows.</span><span class="sxs-lookup"><span data-stu-id="5e70a-113">PowerShell offers some tab completion features not available from Windows Command Prompt.</span></span> <span data-ttu-id="5e70a-114">Para entrar, execute o comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="5e70a-114">To sign in, run the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="5e70a-115">Para saber mais sobre os diferentes métodos de autenticação, confira [Entrar com a CLI do Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="5e70a-115">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="5e70a-116">solução de problemas</span><span class="sxs-lookup"><span data-stu-id="5e70a-116">Troubleshooting</span></span>

<span data-ttu-id="5e70a-117">Veja alguns problemas comuns que ocorrem durante a instalação no Windows.</span><span class="sxs-lookup"><span data-stu-id="5e70a-117">Here are some common problems seen when installing on Windows.</span></span> <span data-ttu-id="5e70a-118">Se você tiver um problema não abordado aqui, [arquive um problema no GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="5e70a-118">If you experience a problem not covered here, [file an issue on GitHub](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="proxy-blocks-connection"></a><span data-ttu-id="5e70a-119">Conexão de blocos de proxy</span><span class="sxs-lookup"><span data-stu-id="5e70a-119">Proxy blocks connection</span></span>

<span data-ttu-id="5e70a-120">Se não for possível baixar o instalador do MSI porque o proxy está bloqueando a conexão, verifique se o proxy foi configurado corretamente.</span><span class="sxs-lookup"><span data-stu-id="5e70a-120">If you can't download the MSI installer because your proxy is blocking the connection, make sure that you have your proxy properly configured.</span></span> <span data-ttu-id="5e70a-121">No Windows 10, essas configurações são gerenciadas no painel `Settings > Network & Internet > Proxy`.</span><span class="sxs-lookup"><span data-stu-id="5e70a-121">For Windows 10, these settings are managed in the `Settings > Network & Internet > Proxy` pane.</span></span> <span data-ttu-id="5e70a-122">Entre em contato com o administrador do sistema para saber as configurações exigidas ou em situações em que o computador pode ser gerenciado por configuração ou precise de configurações avançadas.</span><span class="sxs-lookup"><span data-stu-id="5e70a-122">Contact your system administrator for the required settings, or for situations where your machine may be configuration-managed or require advanced setup.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="5e70a-123">Essas configurações também precisam ser capazes de acessar os serviços do Azure com a CLI, tanto do PowerShell quanto do prompt de comando.</span><span class="sxs-lookup"><span data-stu-id="5e70a-123">These settings are also required to be able to access Azure services with the CLI, from both PowerShell or the Command Prompt.</span></span> <span data-ttu-id="5e70a-124">No PowerShell, faça isso com o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="5e70a-124">In PowerShell, you do this with the following command:</span></span>
>
> ```powershell
> (New-Object System.Net.WebClient).Proxy.Credentials = `
>   [System.Net.CredentialCache]::DefaultNetworkCredentials
> ```

<span data-ttu-id="5e70a-125">Para obter o MSI, o proxy precisa permitir conexões HTTPS com os seguintes endereços:</span><span class="sxs-lookup"><span data-stu-id="5e70a-125">In order to get the MSI, your proxy needs to allow HTTPS connections to the following addresses:</span></span>

* `https://aka.ms/`
* `https://azurecliprod.blob.core.windows.net/`

## <a name="uninstall"></a><span data-ttu-id="5e70a-126">Desinstalar</span><span class="sxs-lookup"><span data-stu-id="5e70a-126">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="5e70a-127">Desinstale a CLI do Azure da lista de "Aplicativos e recursos" do Windows.</span><span class="sxs-lookup"><span data-stu-id="5e70a-127">You uninstall the Azure CLI from the Windows "Apps and Features" list.</span></span> <span data-ttu-id="5e70a-128">Para desinstalar:</span><span class="sxs-lookup"><span data-stu-id="5e70a-128">To uninstall:</span></span>

| <span data-ttu-id="5e70a-129">Plataforma</span><span class="sxs-lookup"><span data-stu-id="5e70a-129">Platform</span></span> | <span data-ttu-id="5e70a-130">Instruções</span><span class="sxs-lookup"><span data-stu-id="5e70a-130">Instructions</span></span> |
|---|---|
| <span data-ttu-id="5e70a-131">Windows 10</span><span class="sxs-lookup"><span data-stu-id="5e70a-131">Windows 10</span></span> | <span data-ttu-id="5e70a-132">Iniciar > Configurações > Aplicativos</span><span class="sxs-lookup"><span data-stu-id="5e70a-132">Start > Settings > Apps</span></span> |
| <span data-ttu-id="5e70a-133">Windows 8</span><span class="sxs-lookup"><span data-stu-id="5e70a-133">Windows 8</span></span><br/><span data-ttu-id="5e70a-134">Windows 7</span><span class="sxs-lookup"><span data-stu-id="5e70a-134">Windows 7</span></span> | <span data-ttu-id="5e70a-135">Iniciar > Painel de Controle > Programas > Desinstalar um programa</span><span class="sxs-lookup"><span data-stu-id="5e70a-135">Start > Control Panel > Programs > Uninstall a program</span></span> |

<span data-ttu-id="5e70a-136">Uma vez nessa tela, digite __CLI do Azure__ na barra de pesquisa do programa.</span><span class="sxs-lookup"><span data-stu-id="5e70a-136">Once on this screen type __Azure CLI__ into the program search bar.</span></span> <span data-ttu-id="5e70a-137">O programa de desinstalação aparece como __Microsoft CLI 2.0 para Azure__.</span><span class="sxs-lookup"><span data-stu-id="5e70a-137">The program to uninstall is listed as __Microsoft CLI 2.0 for Azure__.</span></span> <span data-ttu-id="5e70a-138">Selecione este aplicativo e clique no botão `Uninstall`.</span><span class="sxs-lookup"><span data-stu-id="5e70a-138">Select this application, then click the `Uninstall` button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="5e70a-139">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="5e70a-139">Next Steps</span></span>

<span data-ttu-id="5e70a-140">Agora que você instalou a CLI do Azure, faça um tour breve de seus recursos e comandos comuns.</span><span class="sxs-lookup"><span data-stu-id="5e70a-140">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="5e70a-141">Introdução à CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="5e70a-141">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
