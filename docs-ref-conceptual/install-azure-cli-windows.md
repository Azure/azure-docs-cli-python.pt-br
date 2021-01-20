---
title: Instalar a CLI do Azure para Windows
description: Como instalar a CLI do Azure no Windows
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.prod: azure
ms.date: 09/25/2020
ms.topic: conceptual
ms.devlang: azurecli
ms.technology: azure-cli
ms.custom: devx-track-azurecli
ms.openlocfilehash: e8103b8b235c7ac003b2434c72e69839a39f4a9f
ms.sourcegitcommit: e672284b83a9dbb46cbc54be17f5cd8512310e0a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2021
ms.locfileid: "98594185"
---
# <a name="install-azure-cli-on-windows"></a><span data-ttu-id="21ce9-103">Instalar a CLI do Azure no Windows</span><span class="sxs-lookup"><span data-stu-id="21ce9-103">Install Azure CLI on Windows</span></span>

<span data-ttu-id="21ce9-104">Para o Windows, a CLI do Azure é instalada por meio de um MSI, o que fornece acesso à CLI por meio do Prompt de Comando do Windows (CMD) ou o PowerShell.</span><span class="sxs-lookup"><span data-stu-id="21ce9-104">For Windows, the Azure CLI is installed via a MSI, which gives you access to the CLI through the Windows Command Prompt (CMD) or PowerShell.</span></span>
<span data-ttu-id="21ce9-105">Ao instalar o Subsistema do Windows para Linux (WSL), há pacotes disponíveis para a distribuição do Linux.</span><span class="sxs-lookup"><span data-stu-id="21ce9-105">When installing for Windows Subsystem for Linux (WSL), packages are available for your Linux distribution.</span></span> <span data-ttu-id="21ce9-106">Consulte a [página instalação principal](install-azure-cli.md) para ver a lista de gerenciadores de pacotes com suporte ou como instalar manualmente no WSL.</span><span class="sxs-lookup"><span data-stu-id="21ce9-106">See the [main install page](install-azure-cli.md) for the list of supported package managers or how to install manually under WSL.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

## <a name="install-or-update"></a><span data-ttu-id="21ce9-107">Instalar ou atualizar</span><span class="sxs-lookup"><span data-stu-id="21ce9-107">Install or update</span></span>

<span data-ttu-id="21ce9-108">O MSI distribuível é usado para instalar ou atualizar a CLI do Azure no Windows.</span><span class="sxs-lookup"><span data-stu-id="21ce9-108">The MSI distributable is used for installing or updating the Azure CLI on Windows.</span></span> <span data-ttu-id="21ce9-109">Você não precisa desinstalar as versões atuais antes de usar o instalador MSI, pois o MSI atualizará qualquer versão existente.</span><span class="sxs-lookup"><span data-stu-id="21ce9-109">You don't need to uninstall current versions before using the MSI installer because the MSI will update any existing version.</span></span>

# <a name="microsoft-installer-msi"></a>[<span data-ttu-id="21ce9-110">Microsoft Installer (MSI)</span><span class="sxs-lookup"><span data-stu-id="21ce9-110">Microsoft Installer (MSI)</span></span>](#tab/azure-cli)

<span data-ttu-id="21ce9-111">Quando o instalador perguntar se pode fazer alterações no computador, clique na caixa "Sim".</span><span class="sxs-lookup"><span data-stu-id="21ce9-111">When the installer asks if it can make changes to your computer, click the "Yes" box.</span></span>

### <a name="azure-cli-current-version"></a><span data-ttu-id="21ce9-112">Versão atual da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="21ce9-112">Azure CLI current version</span></span>

<span data-ttu-id="21ce9-113">Baixe e instale a versão atual da CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="21ce9-113">Download and install the current release of the Azure CLI.</span></span>  

> [!div class="nextstepaction"]
> [<span data-ttu-id="21ce9-114">Versão atual da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="21ce9-114">Current release of the Azure CLI</span></span>](https://aka.ms/installazurecliwindows)

### <a name="azure-cli-beta-version"></a><span data-ttu-id="21ce9-115">Versão beta da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="21ce9-115">Azure CLI beta version</span></span>

<span data-ttu-id="21ce9-116">A versão beta da CLI do Azure dá suporte a todos os comandos da CLI que você encontrará na versão lançada atual.</span><span class="sxs-lookup"><span data-stu-id="21ce9-116">The beta version of the Azure CLI supports all CLI commands that you will find in the current released version.</span></span> <span data-ttu-id="21ce9-117">A versão beta é uma migração da CLI do Azure lançada, pois a plataforma de autenticação do AAD (v1.0) está sendo preterida.</span><span class="sxs-lookup"><span data-stu-id="21ce9-117">The beta version is a migration from the released Azure CLI as the AAD authentication platform (v1.0) is being deprecated.</span></span>  <span data-ttu-id="21ce9-118">A [plataforma de Identidade da Microsoft (v 2.0)](/azure/active-directory/develop/v2-overview) é o novo método de autenticação e é usada pela CLI do Azure beta.</span><span class="sxs-lookup"><span data-stu-id="21ce9-118">[Microsoft Identity platform (v2.0)](/azure/active-directory/develop/v2-overview) is the new authentication method and is used by Azure CLI beta.</span></span>  <span data-ttu-id="21ce9-119">Recomendamos que você experimente a versão beta com antecedência.</span><span class="sxs-lookup"><span data-stu-id="21ce9-119">We recommend that you try the beta version in advance.</span></span>  

<span data-ttu-id="21ce9-120">Para obter mais informações sobre a CLI do Azure beta, confira as [notas sobre a versão](./release-notes-azure-cli.md?tabs=azure-cli-beta).</span><span class="sxs-lookup"><span data-stu-id="21ce9-120">For more information about Azure CLI beta, please see [release notes](./release-notes-azure-cli.md?tabs=azure-cli-beta).</span></span>

> [!IMPORTANT]
>
> <span data-ttu-id="21ce9-121">A versão beta não garante um nível de qualidade igual ao do produto, portanto, não deve ser usada em seu ambiente de produção.</span><span class="sxs-lookup"><span data-stu-id="21ce9-121">The beta version does not guarantee product level quality so it should not be used in your production environment.</span></span>

<span data-ttu-id="21ce9-122">Baixar e instalar a versão beta da CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="21ce9-122">Download and install the beta version of the Azure CLI.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="21ce9-123">Versão beta da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="21ce9-123">Beta release of the Azure CLI</span></span>](https://aka.ms/installazurecliwindowsbeta)

# <a name="microsoft-installer-msi-with-command"></a>[<span data-ttu-id="21ce9-124">Microsoft Installer (MSI) com o Comando</span><span class="sxs-lookup"><span data-stu-id="21ce9-124">Microsoft Installer (MSI) with Command</span></span>](#tab/azure-powershell)

### <a name="powershell-command"></a><span data-ttu-id="21ce9-125">Comando do PowerShell</span><span class="sxs-lookup"><span data-stu-id="21ce9-125">Powershell Command</span></span>

<span data-ttu-id="21ce9-126">Também é possível instalar a CLI do Azure usando o PowerShell.</span><span class="sxs-lookup"><span data-stu-id="21ce9-126">You can also install the Azure CLI using PowerShell.</span></span> <span data-ttu-id="21ce9-127">Inicie o PowerShell como administrador e execute o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="21ce9-127">Start PowerShell as administrator and run the following command:</span></span>

   ```PowerShell
   Invoke-WebRequest -Uri https://aka.ms/installazurecliwindows -OutFile .\AzureCLI.msi; Start-Process msiexec.exe -Wait -ArgumentList '/I AzureCLI.msi /quiet'; rm .\AzureCLI.msi
   ```

<span data-ttu-id="21ce9-128">Isso baixará e instalará a versão mais recente da CLI do Azure para Windows.</span><span class="sxs-lookup"><span data-stu-id="21ce9-128">This will download and install the latest version of the Azure CLI for Windows.</span></span> <span data-ttu-id="21ce9-129">Se você já tiver uma versão instalada, o instalador atualizará a versão existente.</span><span class="sxs-lookup"><span data-stu-id="21ce9-129">If you already have a version installed, the installer will update the existing version.</span></span> <span data-ttu-id="21ce9-130">Após a conclusão da instalação, será preciso reabrir o PowerShell para usar a CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="21ce9-130">After the installation is complete, you will need to reopen PowerShell to use the Azure CLI.</span></span>

### <a name="azure-cli-command-for-update-only"></a><span data-ttu-id="21ce9-131">Comando da CLI do Azure (somente para atualização)</span><span class="sxs-lookup"><span data-stu-id="21ce9-131">Azure CLI Command (for update only)</span></span>
[!INCLUDE [az-upgrade](includes/az-upgrade.md)]

---

## <a name="run-the-azure-cli"></a><span data-ttu-id="21ce9-132">Executar a CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="21ce9-132">Run the Azure CLI</span></span>

<span data-ttu-id="21ce9-133">Agora, você pode executar a CLI do Azure com o comando `az` no Prompt de Comando do Windows ou no PowerShell.</span><span class="sxs-lookup"><span data-stu-id="21ce9-133">You can now run the Azure CLI with the `az` command from either Windows Command Prompt or PowerShell.</span></span> <span data-ttu-id="21ce9-134">O PowerShell oferece alguns recursos de conclusão de guia não disponíveis no prompt de comando do Windows.</span><span class="sxs-lookup"><span data-stu-id="21ce9-134">PowerShell offers some tab completion features not available from Windows Command Prompt.</span></span> <span data-ttu-id="21ce9-135">Para entrar, execute o comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="21ce9-135">To sign in, run the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="21ce9-136">Para saber mais sobre os diferentes métodos de autenticação, confira [Entrar com a CLI do Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="21ce9-136">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="21ce9-137">Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="21ce9-137">Troubleshooting</span></span>

<span data-ttu-id="21ce9-138">Veja alguns problemas comuns que ocorrem durante a instalação no Windows.</span><span class="sxs-lookup"><span data-stu-id="21ce9-138">Here are some common problems seen when installing on Windows.</span></span> <span data-ttu-id="21ce9-139">Se você tiver um problema não abordado aqui, [arquive um problema no GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="21ce9-139">If you experience a problem not covered here, [file an issue on GitHub](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="proxy-blocks-connection"></a><span data-ttu-id="21ce9-140">Conexão de blocos de proxy</span><span class="sxs-lookup"><span data-stu-id="21ce9-140">Proxy blocks connection</span></span>

<span data-ttu-id="21ce9-141">Se não for possível baixar o instalador do MSI porque o proxy está bloqueando a conexão, verifique se o proxy foi configurado corretamente.</span><span class="sxs-lookup"><span data-stu-id="21ce9-141">If you can't download the MSI installer because your proxy is blocking the connection, make sure that you have your proxy properly configured.</span></span> <span data-ttu-id="21ce9-142">No Windows 10, essas configurações são gerenciadas no painel `Settings > Network & Internet > Proxy`.</span><span class="sxs-lookup"><span data-stu-id="21ce9-142">For Windows 10, these settings are managed in the `Settings > Network & Internet > Proxy` pane.</span></span> <span data-ttu-id="21ce9-143">Entre em contato com o administrador do sistema para saber as configurações exigidas ou em situações em que o computador pode ser gerenciado por configuração ou precise de configurações avançadas.</span><span class="sxs-lookup"><span data-stu-id="21ce9-143">Contact your system administrator for the required settings, or for situations where your machine may be configuration-managed or require advanced setup.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="21ce9-144">Essas configurações também precisam ser capazes de acessar os serviços do Azure com a CLI, tanto do PowerShell quanto do prompt de comando.</span><span class="sxs-lookup"><span data-stu-id="21ce9-144">These settings are also required to be able to access Azure services with the CLI, from both PowerShell or the Command Prompt.</span></span> <span data-ttu-id="21ce9-145">No PowerShell, faça isso com o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="21ce9-145">In PowerShell, you do this with the following command:</span></span>
>
> ```powershell
> (New-Object System.Net.WebClient).Proxy.Credentials = `
>   [System.Net.CredentialCache]::DefaultNetworkCredentials
> ```

<span data-ttu-id="21ce9-146">Para obter o MSI, o proxy precisa permitir conexões HTTPS com os seguintes endereços:</span><span class="sxs-lookup"><span data-stu-id="21ce9-146">In order to get the MSI, your proxy needs to allow HTTPS connections to the following addresses:</span></span>

* `https://aka.ms/`
* `https://azcliprod.blob.core.windows.net/`

## <a name="uninstall"></a><span data-ttu-id="21ce9-147">Desinstalar</span><span class="sxs-lookup"><span data-stu-id="21ce9-147">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="21ce9-148">Desinstale a CLI do Azure da lista de "Aplicativos e recursos" do Windows.</span><span class="sxs-lookup"><span data-stu-id="21ce9-148">You uninstall the Azure CLI from the Windows "Apps and Features" list.</span></span> <span data-ttu-id="21ce9-149">Para desinstalar:</span><span class="sxs-lookup"><span data-stu-id="21ce9-149">To uninstall:</span></span>

| <span data-ttu-id="21ce9-150">Plataforma</span><span class="sxs-lookup"><span data-stu-id="21ce9-150">Platform</span></span> | <span data-ttu-id="21ce9-151">Instruções</span><span class="sxs-lookup"><span data-stu-id="21ce9-151">Instructions</span></span> |
|---|---|
| <span data-ttu-id="21ce9-152">Windows 10</span><span class="sxs-lookup"><span data-stu-id="21ce9-152">Windows 10</span></span> | <span data-ttu-id="21ce9-153">Iniciar > Configurações > Aplicativos</span><span class="sxs-lookup"><span data-stu-id="21ce9-153">Start > Settings > Apps</span></span> |
| <span data-ttu-id="21ce9-154">Windows 8 e Windows 7</span><span class="sxs-lookup"><span data-stu-id="21ce9-154">Windows 8 and Windows 7</span></span> | <span data-ttu-id="21ce9-155">Iniciar > Painel de Controle > Programas > Desinstalar um programa</span><span class="sxs-lookup"><span data-stu-id="21ce9-155">Start > Control Panel > Programs > Uninstall a program</span></span> |

<span data-ttu-id="21ce9-156">Uma vez nessa tela, digite __CLI do Azure__ na barra de pesquisa do programa.</span><span class="sxs-lookup"><span data-stu-id="21ce9-156">Once on this screen type __Azure CLI__ into the program search bar.</span></span> <span data-ttu-id="21ce9-157">O programa de desinstalação aparece como __Microsoft CLI 2.0 para Azure__.</span><span class="sxs-lookup"><span data-stu-id="21ce9-157">The program to uninstall is listed as __Microsoft CLI 2.0 for Azure__.</span></span> <span data-ttu-id="21ce9-158">Selecione este aplicativo e clique no botão `Uninstall`.</span><span class="sxs-lookup"><span data-stu-id="21ce9-158">Select this application, then click the `Uninstall` button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="21ce9-159">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="21ce9-159">Next Steps</span></span>

<span data-ttu-id="21ce9-160">Agora que você instalou a CLI do Azure, faça um tour breve de seus recursos e comandos comuns.</span><span class="sxs-lookup"><span data-stu-id="21ce9-160">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="21ce9-161">Introdução à CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="21ce9-161">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)