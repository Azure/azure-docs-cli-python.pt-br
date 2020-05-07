---
title: Instalar a CLI do Azure para Windows
description: Como instalar a CLI do Azure no Windows
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 05/01/2019
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: c5e9118a04b0dc608309093866307fdc7083f591
ms.sourcegitcommit: ee64dc738cfe689a2a479e32a87bf420f96c31c8
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2020
ms.locfileid: "80417834"
---
# <a name="install-azure-cli-on-windows"></a><span data-ttu-id="f33b3-103">Instalar a CLI do Azure no Windows</span><span class="sxs-lookup"><span data-stu-id="f33b3-103">Install Azure CLI on Windows</span></span>

<span data-ttu-id="f33b3-104">Para Windows, a CLI do Azure é instalada por meio de um MSI, o que fornece acesso à CLI por meio do Prompt de Comando do Windows (CMD) ou o PowerShell.</span><span class="sxs-lookup"><span data-stu-id="f33b3-104">For Windows the Azure CLI is installed via an MSI, which gives you access to the CLI through the Windows Command Prompt (CMD) or PowerShell.</span></span>
<span data-ttu-id="f33b3-105">Ao instalar o Subsistema do Windows para Linux (WSL), há pacotes disponíveis para a distribuição do Linux.</span><span class="sxs-lookup"><span data-stu-id="f33b3-105">When installing for Windows Subsystem for Linux (WSL), packages are available for your Linux distribution.</span></span> <span data-ttu-id="f33b3-106">Consulte a [página instalação principal](install-azure-cli.md) para ver a lista de gerenciadores de pacotes com suporte ou como instalar manualmente no WSL.</span><span class="sxs-lookup"><span data-stu-id="f33b3-106">See the [main install page](install-azure-cli.md) for the list of supported package managers or how to install manually under WSL.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

## <a name="install-or-update"></a><span data-ttu-id="f33b3-107">Instalar ou atualizar</span><span class="sxs-lookup"><span data-stu-id="f33b3-107">Install or update</span></span>

<span data-ttu-id="f33b3-108">O MSI distribuível é usado para instalar ou atualizar a CLI do Azure no Windows.</span><span class="sxs-lookup"><span data-stu-id="f33b3-108">The MSI distributable is used for installing or updating the Azure CLI on Windows.</span></span> <span data-ttu-id="f33b3-109">Você não precisa desinstalar as versões atuais antes de usar o instalador MSI.</span><span class="sxs-lookup"><span data-stu-id="f33b3-109">You don't need to uninstall any current versions before using the MSI installer.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="f33b3-110">Baixe o instalador MSI</span><span class="sxs-lookup"><span data-stu-id="f33b3-110">Download the MSI installer</span></span>](https://aka.ms/installazurecliwindows)

<span data-ttu-id="f33b3-111">Quando o instalador perguntar se pode fazer alterações no computador, clique na caixa "Sim".</span><span class="sxs-lookup"><span data-stu-id="f33b3-111">When the installer asks if it can make changes to your computer, click the "Yes" box.</span></span>

<span data-ttu-id="f33b3-112">Também é possível instalar a CLI do Azure usando o PowerShell.</span><span class="sxs-lookup"><span data-stu-id="f33b3-112">You can also install the Azure CLI using PowerShell.</span></span> <span data-ttu-id="f33b3-113">Inicie o PowerShell como administrador e execute o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="f33b3-113">Start PowerShell as administrator and run the following command:</span></span>

   ```PowerShell
   Invoke-WebRequest -Uri https://aka.ms/installazurecliwindows -OutFile .\AzureCLI.msi; Start-Process msiexec.exe -Wait -ArgumentList '/I AzureCLI.msi /quiet'; rm .\AzureCLI.msi
   ```
<span data-ttu-id="f33b3-114">Isso baixará e instalará a versão mais recente da CLI do Azure para Windows.</span><span class="sxs-lookup"><span data-stu-id="f33b3-114">This will download and install the latest version of the Azure CLI for Windows.</span></span> <span data-ttu-id="f33b3-115">Se você já tiver uma versão instalada, ela atualizará a versão existente.</span><span class="sxs-lookup"><span data-stu-id="f33b3-115">If you already have a version installed, it will update the existing version.</span></span> <span data-ttu-id="f33b3-116">Após a conclusão da instalação, será preciso reabrir o PowerShell para usar a CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="f33b3-116">After the installation is complete, you will need to reopen PowerShell to use the Azure CLI.</span></span>

<span data-ttu-id="f33b3-117">Agora, você pode executar a CLI do Azure com o comando `az` no Prompt de Comando do Windows ou no PowerShell.</span><span class="sxs-lookup"><span data-stu-id="f33b3-117">You can now run the Azure CLI with the `az` command from either Windows Command Prompt or PowerShell.</span></span> <span data-ttu-id="f33b3-118">O PowerShell oferece alguns recursos de conclusão de guia não disponíveis no prompt de comando do Windows.</span><span class="sxs-lookup"><span data-stu-id="f33b3-118">PowerShell offers some tab completion features not available from Windows Command Prompt.</span></span> <span data-ttu-id="f33b3-119">Para entrar, execute o comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="f33b3-119">To sign in, run the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="f33b3-120">Para saber mais sobre os diferentes métodos de autenticação, confira [Entrar com a CLI do Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="f33b3-120">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="f33b3-121">solução de problemas</span><span class="sxs-lookup"><span data-stu-id="f33b3-121">Troubleshooting</span></span>

<span data-ttu-id="f33b3-122">Veja alguns problemas comuns que ocorrem durante a instalação no Windows.</span><span class="sxs-lookup"><span data-stu-id="f33b3-122">Here are some common problems seen when installing on Windows.</span></span> <span data-ttu-id="f33b3-123">Se você tiver um problema não abordado aqui, [arquive um problema no GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="f33b3-123">If you experience a problem not covered here, [file an issue on GitHub](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="proxy-blocks-connection"></a><span data-ttu-id="f33b3-124">Conexão de blocos de proxy</span><span class="sxs-lookup"><span data-stu-id="f33b3-124">Proxy blocks connection</span></span>

<span data-ttu-id="f33b3-125">Se não for possível baixar o instalador do MSI porque o proxy está bloqueando a conexão, verifique se o proxy foi configurado corretamente.</span><span class="sxs-lookup"><span data-stu-id="f33b3-125">If you can't download the MSI installer because your proxy is blocking the connection, make sure that you have your proxy properly configured.</span></span> <span data-ttu-id="f33b3-126">No Windows 10, essas configurações são gerenciadas no painel `Settings > Network & Internet > Proxy`.</span><span class="sxs-lookup"><span data-stu-id="f33b3-126">For Windows 10, these settings are managed in the `Settings > Network & Internet > Proxy` pane.</span></span> <span data-ttu-id="f33b3-127">Entre em contato com o administrador do sistema para saber as configurações exigidas ou em situações em que o computador pode ser gerenciado por configuração ou precise de configurações avançadas.</span><span class="sxs-lookup"><span data-stu-id="f33b3-127">Contact your system administrator for the required settings, or for situations where your machine may be configuration-managed or require advanced setup.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="f33b3-128">Essas configurações também precisam ser capazes de acessar os serviços do Azure com a CLI, tanto do PowerShell quanto do prompt de comando.</span><span class="sxs-lookup"><span data-stu-id="f33b3-128">These settings are also required to be able to access Azure services with the CLI, from both PowerShell or the Command Prompt.</span></span> <span data-ttu-id="f33b3-129">No PowerShell, faça isso com o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="f33b3-129">In PowerShell, you do this with the following command:</span></span>
>
> ```powershell
> (New-Object System.Net.WebClient).Proxy.Credentials = `
>   [System.Net.CredentialCache]::DefaultNetworkCredentials
> ```

<span data-ttu-id="f33b3-130">Para obter o MSI, o proxy precisa permitir conexões HTTPS com os seguintes endereços:</span><span class="sxs-lookup"><span data-stu-id="f33b3-130">In order to get the MSI, your proxy needs to allow HTTPS connections to the following addresses:</span></span>

* `https://aka.ms/`
* `https://azurecliprod.blob.core.windows.net/`

## <a name="uninstall"></a><span data-ttu-id="f33b3-131">Desinstalar</span><span class="sxs-lookup"><span data-stu-id="f33b3-131">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="f33b3-132">Desinstale a CLI do Azure da lista de "Aplicativos e recursos" do Windows.</span><span class="sxs-lookup"><span data-stu-id="f33b3-132">You uninstall the Azure CLI from the Windows "Apps and Features" list.</span></span> <span data-ttu-id="f33b3-133">Para desinstalar:</span><span class="sxs-lookup"><span data-stu-id="f33b3-133">To uninstall:</span></span>

| <span data-ttu-id="f33b3-134">Plataforma</span><span class="sxs-lookup"><span data-stu-id="f33b3-134">Platform</span></span> | <span data-ttu-id="f33b3-135">Instruções</span><span class="sxs-lookup"><span data-stu-id="f33b3-135">Instructions</span></span> |
|---|---|
| <span data-ttu-id="f33b3-136">Windows 10</span><span class="sxs-lookup"><span data-stu-id="f33b3-136">Windows 10</span></span> | <span data-ttu-id="f33b3-137">Iniciar > Configurações > Aplicativos</span><span class="sxs-lookup"><span data-stu-id="f33b3-137">Start > Settings > Apps</span></span> |
| <span data-ttu-id="f33b3-138">Windows 8</span><span class="sxs-lookup"><span data-stu-id="f33b3-138">Windows 8</span></span><br/><span data-ttu-id="f33b3-139">Windows 7</span><span class="sxs-lookup"><span data-stu-id="f33b3-139">Windows 7</span></span> | <span data-ttu-id="f33b3-140">Iniciar > Painel de Controle > Programas > Desinstalar um programa</span><span class="sxs-lookup"><span data-stu-id="f33b3-140">Start > Control Panel > Programs > Uninstall a program</span></span> |

<span data-ttu-id="f33b3-141">Uma vez nessa tela, digite __CLI do Azure__ na barra de pesquisa do programa.</span><span class="sxs-lookup"><span data-stu-id="f33b3-141">Once on this screen type __Azure CLI__ into the program search bar.</span></span> <span data-ttu-id="f33b3-142">O programa de desinstalação aparece como __Microsoft CLI 2.0 para Azure__.</span><span class="sxs-lookup"><span data-stu-id="f33b3-142">The program to uninstall is listed as __Microsoft CLI 2.0 for Azure__.</span></span> <span data-ttu-id="f33b3-143">Selecione este aplicativo e clique no botão `Uninstall`.</span><span class="sxs-lookup"><span data-stu-id="f33b3-143">Select this application, then click the `Uninstall` button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="f33b3-144">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="f33b3-144">Next Steps</span></span>

<span data-ttu-id="f33b3-145">Agora que você instalou a CLI do Azure, faça um tour breve de seus recursos e comandos comuns.</span><span class="sxs-lookup"><span data-stu-id="f33b3-145">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="f33b3-146">Introdução à CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="f33b3-146">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
