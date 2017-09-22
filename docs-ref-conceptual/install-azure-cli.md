---
title: Instalar a CLI do Azure 2.0
description: "Documentos de referência para instalar a CLI do Azure 2.0"
keywords: "CLI 2.0 do Azure, Referência da CLI 2.0 do Azure, Instalar a CLI 2.0 do Azure, CLI Python do Azure, Desinstalar a CLI 2.0 do Azure"
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 08/17/2017
ms.topic: "articleå"
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: ea5c0ee1-c530-4a1e-a83f-e1be71f6d416
ms.openlocfilehash: 432edac070e238a6f1be0ccd76b9b3582b082219
ms.sourcegitcommit: 2ec80224c6b831e31038b710d912c0dbb1ddfef6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/17/2017
---
# <a name="install-azure-cli-20"></a><span data-ttu-id="5dbcc-104">Instalar a CLI 2.0 do Azure</span><span class="sxs-lookup"><span data-stu-id="5dbcc-104">Install Azure CLI 2.0</span></span>

<span data-ttu-id="5dbcc-105">Instale hoje mesmo a nova versão da CLI do Azure!</span><span class="sxs-lookup"><span data-stu-id="5dbcc-105">Install the new version of the Azure CLI today!</span></span>
<span data-ttu-id="5dbcc-106">Nós a aprimoramos e atualizamos para fornecer uma ótima experiência de linha de comando nativa para gerenciar os recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="5dbcc-106">We've improved and updated it to provide a great native command-line experience for managing Azure resources.</span></span>
<span data-ttu-id="5dbcc-107">Ela pode ser usada em Windows, Linux e macOS.</span><span class="sxs-lookup"><span data-stu-id="5dbcc-107">It can be used on macOS, Linux, and Windows.</span></span>
<span data-ttu-id="5dbcc-108">Para saber mais sobre a versão mais recente, veja as [notas de versão](release-notes-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="5dbcc-108">For information about the latest release, see the [release notes](release-notes-azure-cli.md).</span></span>

> [!NOTE]
> <span data-ttu-id="5dbcc-109">Se você precisa da versão anterior da CLI do Azure, veja como [instalar a CLI do Azure 1.0](/azure/cli-install-nodejs).</span><span class="sxs-lookup"><span data-stu-id="5dbcc-109">If you need the previous version of the Azure CLI, here's how to [install Azure CLI 1.0](/azure/cli-install-nodejs).</span></span>

## <a name="macos"></a><span data-ttu-id="5dbcc-110">macOS</span><span class="sxs-lookup"><span data-stu-id="5dbcc-110">macOS</span></span>

> [!WARNING]
> <span data-ttu-id="5dbcc-111">A fórmula Homebrew para a CLI do Azure, `azure-cli`, está atualmente desatualizada e vai instalar uma versão anterior.</span><span class="sxs-lookup"><span data-stu-id="5dbcc-111">The Homebrew formula for the Azure CLI, `azure-cli`, is currently out of date and will install a previous version.</span></span>

1. <span data-ttu-id="5dbcc-112">Instalar a CLI 2.0 do Azure com um comando `curl`.</span><span class="sxs-lookup"><span data-stu-id="5dbcc-112">Install Azure CLI 2.0 with one `curl` command.</span></span>

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

2. <span data-ttu-id="5dbcc-113">Talvez você precise reiniciar o shell de comando para algumas alterações entrarem em vigor.</span><span class="sxs-lookup"><span data-stu-id="5dbcc-113">You may have to restart your command shell for some changes to take effect.</span></span>

   ```bash
   exec -l $SHELL
   ```
   
3. <span data-ttu-id="5dbcc-114">Execute a CLI no prompt de comando com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="5dbcc-114">Run the CLI from the command prompt with the `az` command.</span></span>

> [!Note]
> <span data-ttu-id="5dbcc-115">Quando você instala com InstallAzureCli, [`az component update`](/cli/azure/component#update) não tem suporte.</span><span class="sxs-lookup"><span data-stu-id="5dbcc-115">When you install with InstallAzureCli, [`az component update`](/cli/azure/component#update) isn't supported.</span></span>
> <span data-ttu-id="5dbcc-116">Para atualizar para a CLI mais recente, execute `curl -L https://aka.ms/InstallAzureCli | bash` novamente.</span><span class="sxs-lookup"><span data-stu-id="5dbcc-116">To update to the latest CLI, run `curl -L https://aka.ms/InstallAzureCli | bash` again.</span></span>
> 
> <span data-ttu-id="5dbcc-117">Para desinstalar, confira as [instruções para a desinstalação manual](#uninstall).</span><span class="sxs-lookup"><span data-stu-id="5dbcc-117">To uninstall, see the [manual uninstall instructions](#uninstall).</span></span>

## <a name="windows"></a><span data-ttu-id="5dbcc-118">Windows</span><span class="sxs-lookup"><span data-stu-id="5dbcc-118">Windows</span></span>

<span data-ttu-id="5dbcc-119">É possível instalar a CLI do Azure 2.0 com o MSI e usá-la na linha de comando do Windows ou instalar a CLI com o apt-get no Bash, no Ubuntu no Windows.</span><span class="sxs-lookup"><span data-stu-id="5dbcc-119">You can install Azure CLI 2.0 with the MSI and use it in the Windows command-line, or you can install the CLI with apt-get on Bash on Ubuntu on Windows.</span></span>

### <a name="msi-for-the-windows-command-line"></a><span data-ttu-id="5dbcc-120">MSI para a linha de comando do Windows</span><span class="sxs-lookup"><span data-stu-id="5dbcc-120">MSI for the Windows command-line</span></span> 

<span data-ttu-id="5dbcc-121">Para instalar a CLI no Windows e usá-la na linha de comando do Windows, baixe e execute o [msi](https://aka.ms/InstallAzureCliWindows).</span><span class="sxs-lookup"><span data-stu-id="5dbcc-121">To install the CLI on Windows and use it in the Windows command-line, download and run the [msi](https://aka.ms/InstallAzureCliWindows).</span></span>

> [!NOTE]
> <span data-ttu-id="5dbcc-122">Ao instalar com o msi, não há suporte para [`az component`](/cli/azure/component).</span><span class="sxs-lookup"><span data-stu-id="5dbcc-122">When you install with the msi, [`az component`](/cli/azure/component) isn't supported.</span></span>
> <span data-ttu-id="5dbcc-123">Para atualizar para a última CLI, execute o [msi](https://aka.ms/InstallAzureCliWindows) novamente.</span><span class="sxs-lookup"><span data-stu-id="5dbcc-123">To update to the latest CLI, run the [msi](https://aka.ms/InstallAzureCliWindows) again.</span></span>
> 
> <span data-ttu-id="5dbcc-124">Para desinstalar a CLI, execute o [msi](https://aka.ms/InstallAzureCliWindows) novamente e escolha Desinstalar.</span><span class="sxs-lookup"><span data-stu-id="5dbcc-124">To uninstall the CLI, run the [msi](https://aka.ms/InstallAzureCliWindows) again and choose uninstall.</span></span>

### <a name="apt-get-for-bash-on-ubuntu-on-windows"></a><span data-ttu-id="5dbcc-125">apt-get para Bash no Ubuntu no Windows</span><span class="sxs-lookup"><span data-stu-id="5dbcc-125">apt-get for Bash on Ubuntu on Windows</span></span>

1. <span data-ttu-id="5dbcc-126">Se você não tiver o Bash no Windows, [instale-o](https://msdn.microsoft.com/commandline/wsl/install_guide).</span><span class="sxs-lookup"><span data-stu-id="5dbcc-126">If you don't have Bash on Windows, [install it](https://msdn.microsoft.com/commandline/wsl/install_guide).</span></span>

2. <span data-ttu-id="5dbcc-127">Abra o shell do Bash.</span><span class="sxs-lookup"><span data-stu-id="5dbcc-127">Open the Bash shell.</span></span>

3. <span data-ttu-id="5dbcc-128">Modifique sua lista de fontes.</span><span class="sxs-lookup"><span data-stu-id="5dbcc-128">Modify your sources list.</span></span>

   ```bash
   echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
   ```

4. <span data-ttu-id="5dbcc-129">Execute os comandos sudo a seguir:</span><span class="sxs-lookup"><span data-stu-id="5dbcc-129">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

5.  <span data-ttu-id="5dbcc-130">Execute a CLI no prompt de comando com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="5dbcc-130">Run the CLI from the command prompt with the `az` command.</span></span>

> [!NOTE]
> <span data-ttu-id="5dbcc-131">Quando você instala com apt-get, [`az component`](/cli/azure/component) não tem suporte.</span><span class="sxs-lookup"><span data-stu-id="5dbcc-131">When you install with apt-get, [`az component`](/cli/azure/component) isn't supported.</span></span>
> <span data-ttu-id="5dbcc-132">Para atualizar a CLI, execute `sudo apt-get update && sudo apt-get install azure-cli` novamente.</span><span class="sxs-lookup"><span data-stu-id="5dbcc-132">To update the CLI, run `sudo apt-get update && sudo apt-get install azure-cli` again.</span></span>
> 
> <span data-ttu-id="5dbcc-133">Para desinstalar, execute `sudo apt-get remove azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="5dbcc-133">To uninstall, run `sudo apt-get remove azure-cli`.</span></span>

## <a name="apt-get-for-debianubuntu"></a><span data-ttu-id="5dbcc-134">apt-get para Debian/Ubuntu</span><span class="sxs-lookup"><span data-stu-id="5dbcc-134">apt-get for Debian/Ubuntu</span></span>

<span data-ttu-id="5dbcc-135">Para sistemas baseados em Debian/Ubuntu, instale a CLI 2.0 do Azure por meio de `apt-get`.</span><span class="sxs-lookup"><span data-stu-id="5dbcc-135">For Debian/Ubuntu based systems, you can install Azure CLI 2.0 via `apt-get`.</span></span>

1. <span data-ttu-id="5dbcc-136">Modifique sua lista de fontes.</span><span class="sxs-lookup"><span data-stu-id="5dbcc-136">Modify your sources list.</span></span>
 
   - <span data-ttu-id="5dbcc-137">sistema de 32 bits</span><span class="sxs-lookup"><span data-stu-id="5dbcc-137">32-bit system</span></span>

     ```bash
     echo "deb https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

   - <span data-ttu-id="5dbcc-138">sistema de 64 bits</span><span class="sxs-lookup"><span data-stu-id="5dbcc-138">64-bit system</span></span>

     ```bash
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="5dbcc-139">Execute os comandos sudo a seguir:</span><span class="sxs-lookup"><span data-stu-id="5dbcc-139">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

3.  <span data-ttu-id="5dbcc-140">Execute a CLI no prompt de comando com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="5dbcc-140">Run the CLI from the command prompt with the `az` command.</span></span>

> [!NOTE]
> <span data-ttu-id="5dbcc-141">Quando você instala com apt-get, [`az component`](/cli/azure/component) não tem suporte.</span><span class="sxs-lookup"><span data-stu-id="5dbcc-141">When you install with apt-get, [`az component`](/cli/azure/component) isn't supported.</span></span>
> <span data-ttu-id="5dbcc-142">Para atualizar a CLI, execute `sudo apt-get update && sudo apt-get install azure-cli` novamente.</span><span class="sxs-lookup"><span data-stu-id="5dbcc-142">To update the CLI, run `sudo apt-get update && sudo apt-get install azure-cli` again.</span></span>
> 
> <span data-ttu-id="5dbcc-143">Para desinstalar, execute `sudo apt-get remove azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="5dbcc-143">To uninstall, run `sudo apt-get remove azure-cli`.</span></span>

## <a name="docker"></a><span data-ttu-id="5dbcc-144">Docker</span><span class="sxs-lookup"><span data-stu-id="5dbcc-144">Docker</span></span>

<span data-ttu-id="5dbcc-145">Vamos manter uma imagem de Docker pré-configurada com a CLI do Azure 2.0.</span><span class="sxs-lookup"><span data-stu-id="5dbcc-145">We maintain a Docker image preconfigured with the Azure CLI 2.0.</span></span>

<span data-ttu-id="5dbcc-146">Instalar a CLI usando `docker run`.</span><span class="sxs-lookup"><span data-stu-id="5dbcc-146">Install the CLI using `docker run`.</span></span>

```bash
docker run azuresdk/azure-cli-python:<version>
```

<span data-ttu-id="5dbcc-147">Confira nossas [marcas do Docker](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/) para versões disponíveis.</span><span class="sxs-lookup"><span data-stu-id="5dbcc-147">See our [Docker tags](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/) for available versions.</span></span>

> [!NOTE]
> <span data-ttu-id="5dbcc-148">Se você quiser acompanhar as chaves SSH do seu ambiente de usuário, use `-v ${HOME}:/root` para montar $HOME como `/root`.</span><span class="sxs-lookup"><span data-stu-id="5dbcc-148">If you want to pick up the SSH keys from your user environment, you can use `-v ${HOME}:/root` to mount $HOME as `/root`.</span></span>

>> ```bash
> docker run -v ${HOME}:/root azuresdk/azure-cli-python:<version>
> ```

<span data-ttu-id="5dbcc-149">A CLI está instalada na imagem como o comando `az` no `/usr/local/bin`.</span><span class="sxs-lookup"><span data-stu-id="5dbcc-149">The CLI is installed on the image as the `az` command in `/usr/local/bin`.</span></span>

> [!NOTE]
> <span data-ttu-id="5dbcc-150">A imagem do Docker não oferece suporte ao recurso [`az component`](/cli/azure/component).</span><span class="sxs-lookup"><span data-stu-id="5dbcc-150">The Docker image does not support the [`az component`](/cli/azure/component) feature.</span></span>
> <span data-ttu-id="5dbcc-151">Para atualizar a CLI 2.0 do Azure, use `docker run` para instalar a imagem mais recente ou a imagem específica que você deseja.</span><span class="sxs-lookup"><span data-stu-id="5dbcc-151">To update the Azure CLI 2.0, use `docker run` to install the latest image, or the specific image that you want.</span></span>

## <a name="linux"></a><span data-ttu-id="5dbcc-152">Linux</span><span class="sxs-lookup"><span data-stu-id="5dbcc-152">Linux</span></span>

1. <span data-ttu-id="5dbcc-153">Se você não tiver, instale o [Python](https://www.python.org/downloads).</span><span class="sxs-lookup"><span data-stu-id="5dbcc-153">If you don't have it, install [Python](https://www.python.org/downloads).</span></span>

2. <span data-ttu-id="5dbcc-154">Dependendo de sua distribuição do Linux, instale os pré-requisitos.</span><span class="sxs-lookup"><span data-stu-id="5dbcc-154">Depending on your Linux distribution, install the prerequisites.</span></span>

   ```
   Platform              | Prerequisites
   ----------------------|---------------------------------------------
   Ubuntu 15.10 or 16.04 | sudo apt-get update && sudo apt-get install -y libssl-dev libffi-dev python-dev build-essential
   Ubuntu 12.04 or 14.04 | sudo apt-get update && sudo apt-get install -y libssl-dev libffi-dev python-dev
   Debian 8              | sudo apt-get update && sudo apt-get install -y libssl-dev libffi-dev python-dev build-essential
   Debian 7              | sudo apt-get update && sudo apt-get install -y libssl-dev libffi-dev python-dev
   CentOS 7.1 or 7.2     | sudo yum check-update; sudo yum install -y gcc libffi-devel python-devel openssl-devel
   RedHat 7.2            | sudo yum check-update; sudo yum install -y gcc libffi-devel python-devel openssl-devel
   SUSE OpenSUSE 13.2    | sudo zypper refresh && sudo zypper --non-interactive install gcc libffi-devel python-devel openssl-devel
   ```

3. <span data-ttu-id="5dbcc-155">Instalar a CLI com um comando `curl`.</span><span class="sxs-lookup"><span data-stu-id="5dbcc-155">Install the CLI with one `curl` command.</span></span>

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

4. <span data-ttu-id="5dbcc-156">Talvez você precise reiniciar o shell de comando para algumas alterações entrarem em vigor.</span><span class="sxs-lookup"><span data-stu-id="5dbcc-156">You may have to restart your command shell for some changes to take effect.</span></span>

   ```bash
   exec -l $SHELL
   ```

5. <span data-ttu-id="5dbcc-157">Execute a CLI no prompt de comando com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="5dbcc-157">Run the CLI from the command prompt with the `az` command.</span></span>

> [!Note]
> <span data-ttu-id="5dbcc-158">Quando você instala com InstallAzureCli, [`az component update`](/cli/azure/component#update) não tem suporte.</span><span class="sxs-lookup"><span data-stu-id="5dbcc-158">When you install with InstallAzureCli, [`az component update`](/cli/azure/component#update) isn't supported.</span></span>
> <span data-ttu-id="5dbcc-159">Para atualizar para a CLI mais recente, execute `curl -L https://aka.ms/InstallAzureCli | bash` novamente.</span><span class="sxs-lookup"><span data-stu-id="5dbcc-159">To update to the latest CLI, run `curl -L https://aka.ms/InstallAzureCli | bash` again.</span></span>
> 
> <span data-ttu-id="5dbcc-160">Para desinstalar, confira as [instruções para a desinstalação manual](#uninstall).</span><span class="sxs-lookup"><span data-stu-id="5dbcc-160">To uninstall, see the [manual uninstall instructions](#uninstall).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="5dbcc-161">Solucionar problemas</span><span class="sxs-lookup"><span data-stu-id="5dbcc-161">Troubleshooting</span></span>

### <a name="errors-with-curl-redirection"></a><span data-ttu-id="5dbcc-162">Erros com o redirecionamento de rotação</span><span class="sxs-lookup"><span data-stu-id="5dbcc-162">Errors with curl redirection</span></span>

<span data-ttu-id="5dbcc-163">Se você receber um erro do comando `curl` sobre o parâmetro `-L` ou um erro informando "Objeto Movido", tente usar a URL completa em vez da URL aka.ms:</span><span class="sxs-lookup"><span data-stu-id="5dbcc-163">If you get an error from the `curl` command regarding the `-L` parameter, or an error saying "Object Moved", try using the full url instead of the aka.ms url:</span></span>

```
# If you see this:
curl -L https://aka.ms/InstallAzureCli | bash
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100   175  100   175    0     0    562      0 --:--:-- --:--:-- --:--:--   560
bash: line 1: syntax error near unexpected token `<'
'ash: line 1: `<html><head><title>Object moved</title></head><body>

#### Try this instead:
curl https://azurecliprod.blob.core.windows.net/install | bash
```

## <a name="uninstall"></a><span data-ttu-id="5dbcc-164">Desinstalar</span><span class="sxs-lookup"><span data-stu-id="5dbcc-164">Uninstall</span></span>

<span data-ttu-id="5dbcc-165">Se você usou o script em https://aka.ms/InstallAzureCli para instalar a CLI, é possível desinstalá-la com estas etapas.</span><span class="sxs-lookup"><span data-stu-id="5dbcc-165">If you used the script at https://aka.ms/InstallAzureCli to install the CLI, you can uninstall it with these steps.</span></span>

1. <span data-ttu-id="5dbcc-166">Remova os arquivos instalados.</span><span class="sxs-lookup"><span data-stu-id="5dbcc-166">Remove the installed files.</span></span>

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. <span data-ttu-id="5dbcc-167">Exclua a linha `<install location>/lib/azure-cli/az.completion` de `<install location>/.bash_profile`.</span><span class="sxs-lookup"><span data-stu-id="5dbcc-167">Delete the line `<install location>/lib/azure-cli/az.completion` from `<install location>/.bash_profile`.</span></span>

> [!Note]
> <span data-ttu-id="5dbcc-168">O local de instalação padrão é `/Users/<username>`.</span><span class="sxs-lookup"><span data-stu-id="5dbcc-168">The default install location is `/Users/<username>`.</span></span>

<span data-ttu-id="5dbcc-169">Se você usou apt-get, o Docker ou o msi para instalar a CLI, use a mesma ferramenta para desinstalá-la.</span><span class="sxs-lookup"><span data-stu-id="5dbcc-169">If you used apt-get, Docker, or the msi to install the CLI, use the same tool to uninstall it.</span></span>

## <a name="reporting-issues-and-feedback"></a><span data-ttu-id="5dbcc-170">Relatando comentários e problemas</span><span class="sxs-lookup"><span data-stu-id="5dbcc-170">Reporting issues and feedback</span></span>

<span data-ttu-id="5dbcc-171">Se você encontrar erros com a ferramenta, emita um problema na seção [Problemas](https://github.com/Azure/azure-cli/issues) de nosso repositório do GitHub.</span><span class="sxs-lookup"><span data-stu-id="5dbcc-171">If you encounter any bugs with the tool, file an issue in the [Issues](https://github.com/Azure/azure-cli/issues) section of our GitHub repo.</span></span>
<span data-ttu-id="5dbcc-172">Para fornecer comentários a partir da linha de comando, experimente o comando `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="5dbcc-172">To provide feedback from the command line, try the `az feedback` command.</span></span>
