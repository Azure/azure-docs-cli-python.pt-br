---
title: Instalar a CLI do Azure para Windows
description: Como instalar a CLI do Azure no Windows
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.prod: azure
ms.date: 06/16/2020
ms.topic: conceptual
ms.devlang: azurecli
ms.technology: azure-cli
ms.custom: devx-track-azurecli
ms.openlocfilehash: dc6386e8bc1dfc4d11dafcdb947e9ff0b336ed25
ms.sourcegitcommit: bf84dfb62e910ea246586481863bb43d09d07795
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/04/2020
ms.locfileid: "87551499"
---
# <a name="install-azure-cli-on-windows"></a><span data-ttu-id="32606-103">Instalar a CLI do Azure no Windows</span><span class="sxs-lookup"><span data-stu-id="32606-103">Install Azure CLI on Windows</span></span>

<span data-ttu-id="32606-104">Para o Windows, a CLI do Azure é instalada por meio de um MSI, o que fornece acesso à CLI por meio do Prompt de Comando do Windows (CMD) ou o PowerShell.</span><span class="sxs-lookup"><span data-stu-id="32606-104">For Windows, the Azure CLI is installed via a MSI, which gives you access to the CLI through the Windows Command Prompt (CMD) or PowerShell.</span></span>
<span data-ttu-id="32606-105">Ao instalar o Subsistema do Windows para Linux (WSL), há pacotes disponíveis para a distribuição do Linux.</span><span class="sxs-lookup"><span data-stu-id="32606-105">When installing for Windows Subsystem for Linux (WSL), packages are available for your Linux distribution.</span></span> <span data-ttu-id="32606-106">Consulte a [página instalação principal](install-azure-cli.md) para ver a lista de gerenciadores de pacotes com suporte ou como instalar manualmente no WSL.</span><span class="sxs-lookup"><span data-stu-id="32606-106">See the [main install page](install-azure-cli.md) for the list of supported package managers or how to install manually under WSL.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

## <a name="install-or-update"></a><span data-ttu-id="32606-107">Instalar ou atualizar</span><span class="sxs-lookup"><span data-stu-id="32606-107">Install or update</span></span>

<span data-ttu-id="32606-108">O MSI distribuível é usado para instalar ou atualizar a CLI do Azure no Windows.</span><span class="sxs-lookup"><span data-stu-id="32606-108">The MSI distributable is used for installing or updating the Azure CLI on Windows.</span></span> <span data-ttu-id="32606-109">Você não precisa desinstalar as versões atuais antes de usar o instalador MSI, pois o MSI atualizará qualquer versão existente.</span><span class="sxs-lookup"><span data-stu-id="32606-109">You don't need to uninstall current versions before using the MSI installer because the MSI will update any existing version.</span></span>

# <a name="microsoft-installer-msi"></a>[<span data-ttu-id="32606-110">Microsoft Installer (MSI)</span><span class="sxs-lookup"><span data-stu-id="32606-110">Microsoft Installer (MSI)</span></span>](#tab/azure-cli)

<span data-ttu-id="32606-111">Quando o instalador perguntar se pode fazer alterações no computador, clique na caixa "Sim".</span><span class="sxs-lookup"><span data-stu-id="32606-111">When the installer asks if it can make changes to your computer, click the "Yes" box.</span></span>

### <a name="azure-cli-current-version"></a><span data-ttu-id="32606-112">Versão atual da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="32606-112">Azure CLI current version</span></span>

<span data-ttu-id="32606-113">Baixe e instale a versão atual da CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="32606-113">Download and install the current release of the Azure CLI.</span></span>  

> [!div class="nextstepaction"]
> [<span data-ttu-id="32606-114">Versão atual da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="32606-114">Current release of the Azure CLI</span></span>](https://aka.ms/installazurecliwindows)

### <a name="azure-cli-beta-version"></a><span data-ttu-id="32606-115">Versão beta da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="32606-115">Azure CLI beta version</span></span>

<span data-ttu-id="32606-116">A versão beta da CLI do Azure dá suporte a todos os comandos da CLI que você encontrará na versão lançada atual.</span><span class="sxs-lookup"><span data-stu-id="32606-116">The beta version of the Azure CLI supports all CLI commands that you will find in the current released version.</span></span> <span data-ttu-id="32606-117">A versão beta é uma migração da CLI do Azure lançada, pois a plataforma de autenticação do AAD (v1.0) está sendo preterida.</span><span class="sxs-lookup"><span data-stu-id="32606-117">The beta version is a migration from the released Azure CLI as the AAD authentication platform (v1.0) is being deprecated.</span></span>  <span data-ttu-id="32606-118">A [plataforma de Identidade da Microsoft (v 2.0)](/azure/active-directory/develop/v2-overview) é o novo método de autenticação e é usada pela CLI do Azure beta.</span><span class="sxs-lookup"><span data-stu-id="32606-118">[Microsoft Identity platform (v2.0)](/azure/active-directory/develop/v2-overview) is the new authentication method and is used by Azure CLI beta.</span></span>  <span data-ttu-id="32606-119">Recomendamos que você experimente a versão beta com antecedência.</span><span class="sxs-lookup"><span data-stu-id="32606-119">We recommend that you try the beta version in advance.</span></span>  

<span data-ttu-id="32606-120">Para obter mais informações sobre a CLI do Azure beta, confira as [notas sobre a versão](release-notes-azure-cli?tabs=azure-cli-beta).</span><span class="sxs-lookup"><span data-stu-id="32606-120">For more information about Azure CLI beta, please see [release notes](release-notes-azure-cli?tabs=azure-cli-beta).</span></span>

> [!IMPORTANT]
>
> <span data-ttu-id="32606-121">A versão beta não garante um nível de qualidade igual ao do produto, portanto, não deve ser usada em seu ambiente de produção.</span><span class="sxs-lookup"><span data-stu-id="32606-121">The beta version does not guarantee product level quality so it should not be used in your production environment.</span></span>

<span data-ttu-id="32606-122">Baixar e instalar a versão beta da CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="32606-122">Download and install the beta version of the Azure CLI.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="32606-123">Versão beta da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="32606-123">Beta release of the Azure CLI</span></span>](https://aka.ms/installazurecliwindowsbeta)

# <a name="microsoft-installer-msi-with-powershell"></a>[<span data-ttu-id="32606-124">Microsoft Installer (MSI) com o PowerShell</span><span class="sxs-lookup"><span data-stu-id="32606-124">Microsoft Installer (MSI) with PowerShell</span></span>](#tab/azure-powershell)

<span data-ttu-id="32606-125">Também é possível instalar a CLI do Azure usando o PowerShell.</span><span class="sxs-lookup"><span data-stu-id="32606-125">You can also install the Azure CLI using PowerShell.</span></span> <span data-ttu-id="32606-126">Inicie o PowerShell como administrador e execute o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="32606-126">Start PowerShell as administrator and run the following command:</span></span>

   ```PowerShell
   Invoke-WebRequest -Uri https://aka.ms/installazurecliwindows -OutFile .\AzureCLI.msi; Start-Process msiexec.exe -Wait -ArgumentList '/I AzureCLI.msi /quiet'; rm .\AzureCLI.msi
   ```

<span data-ttu-id="32606-127">Isso baixará e instalará a versão mais recente da CLI do Azure para Windows.</span><span class="sxs-lookup"><span data-stu-id="32606-127">This will download and install the latest version of the Azure CLI for Windows.</span></span> <span data-ttu-id="32606-128">Se você já tiver uma versão instalada, o instalador atualizará a versão existente.</span><span class="sxs-lookup"><span data-stu-id="32606-128">If you already have a version installed, the installer will update the existing version.</span></span> <span data-ttu-id="32606-129">Após a conclusão da instalação, será preciso reabrir o PowerShell para usar a CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="32606-129">After the installation is complete, you will need to reopen PowerShell to use the Azure CLI.</span></span>

---

## <a name="run-the-azure-cli"></a><span data-ttu-id="32606-130">Executar a CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="32606-130">Run the Azure CLI</span></span>

<span data-ttu-id="32606-131">Agora, você pode executar a CLI do Azure com o comando `az` no Prompt de Comando do Windows ou no PowerShell.</span><span class="sxs-lookup"><span data-stu-id="32606-131">You can now run the Azure CLI with the `az` command from either Windows Command Prompt or PowerShell.</span></span> <span data-ttu-id="32606-132">O PowerShell oferece alguns recursos de conclusão de guia não disponíveis no prompt de comando do Windows.</span><span class="sxs-lookup"><span data-stu-id="32606-132">PowerShell offers some tab completion features not available from Windows Command Prompt.</span></span> <span data-ttu-id="32606-133">Para entrar, execute o comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="32606-133">To sign in, run the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="32606-134">Para saber mais sobre os diferentes métodos de autenticação, confira [Entrar com a CLI do Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="32606-134">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="32606-135">Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="32606-135">Troubleshooting</span></span>

<span data-ttu-id="32606-136">Veja alguns problemas comuns que ocorrem durante a instalação no Windows.</span><span class="sxs-lookup"><span data-stu-id="32606-136">Here are some common problems seen when installing on Windows.</span></span> <span data-ttu-id="32606-137">Se você tiver um problema não abordado aqui, [arquive um problema no GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="32606-137">If you experience a problem not covered here, [file an issue on GitHub](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="proxy-blocks-connection"></a><span data-ttu-id="32606-138">Conexão de blocos de proxy</span><span class="sxs-lookup"><span data-stu-id="32606-138">Proxy blocks connection</span></span>

<span data-ttu-id="32606-139">Se não for possível baixar o instalador do MSI porque o proxy está bloqueando a conexão, verifique se o proxy foi configurado corretamente.</span><span class="sxs-lookup"><span data-stu-id="32606-139">If you can't download the MSI installer because your proxy is blocking the connection, make sure that you have your proxy properly configured.</span></span> <span data-ttu-id="32606-140">No Windows 10, essas configurações são gerenciadas no painel `Settings > Network & Internet > Proxy`.</span><span class="sxs-lookup"><span data-stu-id="32606-140">For Windows 10, these settings are managed in the `Settings > Network & Internet > Proxy` pane.</span></span> <span data-ttu-id="32606-141">Entre em contato com o administrador do sistema para saber as configurações exigidas ou em situações em que o computador pode ser gerenciado por configuração ou precise de configurações avançadas.</span><span class="sxs-lookup"><span data-stu-id="32606-141">Contact your system administrator for the required settings, or for situations where your machine may be configuration-managed or require advanced setup.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="32606-142">Essas configurações também precisam ser capazes de acessar os serviços do Azure com a CLI, tanto do PowerShell quanto do prompt de comando.</span><span class="sxs-lookup"><span data-stu-id="32606-142">These settings are also required to be able to access Azure services with the CLI, from both PowerShell or the Command Prompt.</span></span> <span data-ttu-id="32606-143">No PowerShell, faça isso com o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="32606-143">In PowerShell, you do this with the following command:</span></span>
>
> ```powershell
> (New-Object System.Net.WebClient).Proxy.Credentials = `
>   [System.Net.CredentialCache]::DefaultNetworkCredentials
> ```

<span data-ttu-id="32606-144">Para obter o MSI, o proxy precisa permitir conexões HTTPS com os seguintes endereços:</span><span class="sxs-lookup"><span data-stu-id="32606-144">In order to get the MSI, your proxy needs to allow HTTPS connections to the following addresses:</span></span>

* `https://aka.ms/`
* `https://azurecliprod.blob.core.windows.net/`

## <a name="uninstall"></a><span data-ttu-id="32606-145">Desinstalar</span><span class="sxs-lookup"><span data-stu-id="32606-145">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="32606-146">Desinstale a CLI do Azure da lista de "Aplicativos e recursos" do Windows.</span><span class="sxs-lookup"><span data-stu-id="32606-146">You uninstall the Azure CLI from the Windows "Apps and Features" list.</span></span> <span data-ttu-id="32606-147">Para desinstalar:</span><span class="sxs-lookup"><span data-stu-id="32606-147">To uninstall:</span></span>

| <span data-ttu-id="32606-148">Plataforma</span><span class="sxs-lookup"><span data-stu-id="32606-148">Platform</span></span> | <span data-ttu-id="32606-149">Instruções</span><span class="sxs-lookup"><span data-stu-id="32606-149">Instructions</span></span> |
|---|---|
| <span data-ttu-id="32606-150">Windows 10</span><span class="sxs-lookup"><span data-stu-id="32606-150">Windows 10</span></span> | <span data-ttu-id="32606-151">Iniciar > Configurações > Aplicativos</span><span class="sxs-lookup"><span data-stu-id="32606-151">Start > Settings > Apps</span></span> |
| <span data-ttu-id="32606-152">Windows 8 e Windows 7</span><span class="sxs-lookup"><span data-stu-id="32606-152">Windows 8 and Windows 7</span></span> | <span data-ttu-id="32606-153">Iniciar > Painel de Controle > Programas > Desinstalar um programa</span><span class="sxs-lookup"><span data-stu-id="32606-153">Start > Control Panel > Programs > Uninstall a program</span></span> |

<span data-ttu-id="32606-154">Uma vez nessa tela, digite __CLI do Azure__ na barra de pesquisa do programa.</span><span class="sxs-lookup"><span data-stu-id="32606-154">Once on this screen type __Azure CLI__ into the program search bar.</span></span> <span data-ttu-id="32606-155">O programa de desinstalação aparece como __Microsoft CLI 2.0 para Azure__.</span><span class="sxs-lookup"><span data-stu-id="32606-155">The program to uninstall is listed as __Microsoft CLI 2.0 for Azure__.</span></span> <span data-ttu-id="32606-156">Selecione este aplicativo e clique no botão `Uninstall`.</span><span class="sxs-lookup"><span data-stu-id="32606-156">Select this application, then click the `Uninstall` button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="32606-157">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="32606-157">Next Steps</span></span>

<span data-ttu-id="32606-158">Agora que você instalou a CLI do Azure, faça um tour breve de seus recursos e comandos comuns.</span><span class="sxs-lookup"><span data-stu-id="32606-158">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="32606-159">Introdução à CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="32606-159">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
