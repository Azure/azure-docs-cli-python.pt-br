---
title: Instalar a CLI do Azure 2.0
description: "Documentos de referência para a instalação da CLI do Azure 2.0"
keywords: "CLI do Azure, Instalar a CLI do Azure, Azure Python CLI, Referência da CLI do Azure"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 08/17/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: ea5c0ee1-c530-4a1e-a83f-e1be71f6d416
ms.openlocfilehash: a61f47076854d0ff0a7056f82240794b7533fe3e
ms.sourcegitcommit: 3db5fb207db551a0d3fe0a88fe09e8f5e2ec184d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2017
---
# <a name="install-azure-cli-20"></a><span data-ttu-id="13516-104">Instalar a CLI 2.0 do Azure</span><span class="sxs-lookup"><span data-stu-id="13516-104">Install Azure CLI 2.0</span></span>

<span data-ttu-id="13516-105">Instale hoje mesmo a nova versão da CLI do Azure!</span><span class="sxs-lookup"><span data-stu-id="13516-105">Install the new version of the Azure CLI today!</span></span>
<span data-ttu-id="13516-106">Nós a aprimoramos e atualizamos para fornecer uma ótima experiência de linha de comando nativa para gerenciar os recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="13516-106">We've improved and updated it to provide a great native command-line experience for managing Azure resources.</span></span>
<span data-ttu-id="13516-107">Ela pode ser usada em Windows, Linux e macOS.</span><span class="sxs-lookup"><span data-stu-id="13516-107">It can be used on macOS, Linux, and Windows.</span></span>
<span data-ttu-id="13516-108">Para saber mais sobre a versão mais recente, veja as [notas de versão](release-notes-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="13516-108">For information about the latest release, see the [release notes](release-notes-azure-cli.md).</span></span>

> [!NOTE]
> <span data-ttu-id="13516-109">Se você precisa da versão anterior da CLI do Azure, veja como [instalar a CLI do Azure 1.0](/azure/cli-install-nodejs).</span><span class="sxs-lookup"><span data-stu-id="13516-109">If you need the previous version of the Azure CLI, here's how to [install Azure CLI 1.0](/azure/cli-install-nodejs).</span></span>

## <a name="a-namemacosinstall-on-macos"></a><span data-ttu-id="13516-110"><a name="macOS"/>Instalar no macOS</span><span class="sxs-lookup"><span data-stu-id="13516-110"><a name="macOS"/>Install on macOS</span></span>

1. <span data-ttu-id="13516-111">Instale a CLI do Azure 2.0 com `curl`.</span><span class="sxs-lookup"><span data-stu-id="13516-111">Install Azure CLI 2.0 with `curl`.</span></span>

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

2. <span data-ttu-id="13516-112">Talvez você precise reiniciar o shell para que algumas alterações entrem em vigor.</span><span class="sxs-lookup"><span data-stu-id="13516-112">You may have to restart your shell for some changes to take effect.</span></span>

   ```bash
   exec -l $SHELL
   ```
   
3. <span data-ttu-id="13516-113">Execute a CLI no prompt de comando com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="13516-113">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-on-windows"></a><span data-ttu-id="13516-114">Instalar no Windows</span><span class="sxs-lookup"><span data-stu-id="13516-114">Install on Windows</span></span>

<span data-ttu-id="13516-115">É possível instalar a CLI do Azure 2.0 com o MSI e usá-la na linha de comando do Windows ou instalar a CLI com o `apt-get` no Bash, no Ubuntu no Windows.</span><span class="sxs-lookup"><span data-stu-id="13516-115">You can install Azure CLI 2.0 with the MSI and use it in the Windows command-line, or you can install the CLI with `apt-get` on Bash on Ubuntu on Windows.</span></span>

### <a name="install-with-msi-for-the-windows-command-line"></a><span data-ttu-id="13516-116">Instalar com MSI para a linha de comando do Windows</span><span class="sxs-lookup"><span data-stu-id="13516-116">Install with MSI for the Windows command-line</span></span> 

<span data-ttu-id="13516-117">Para instalar a CLI no Windows e usá-la na linha de comando do Windows, baixe e execute o [MSI](https://aka.ms/InstallAzureCliWindows).</span><span class="sxs-lookup"><span data-stu-id="13516-117">To install the CLI on Windows and use it in the Windows command-line, download and run the [MSI](https://aka.ms/InstallAzureCliWindows).</span></span>

### <a name="install-with-apt-get-for-bash-on-ubuntu-on-windows"></a><span data-ttu-id="13516-118">Instalar com apt-get para Bash no Ubuntu no Windows</span><span class="sxs-lookup"><span data-stu-id="13516-118">Install with apt-get for Bash on Ubuntu on Windows</span></span>

1. <span data-ttu-id="13516-119">Se você não tiver o Bash no Windows, [instale-o](https://msdn.microsoft.com/commandline/wsl/install_guide).</span><span class="sxs-lookup"><span data-stu-id="13516-119">If you don't have Bash on Windows, [install it](https://msdn.microsoft.com/commandline/wsl/install_guide).</span></span>

2. <span data-ttu-id="13516-120">Abra o shell do Bash.</span><span class="sxs-lookup"><span data-stu-id="13516-120">Open the Bash shell.</span></span>

3. <span data-ttu-id="13516-121">Modifique sua lista de fontes.</span><span class="sxs-lookup"><span data-stu-id="13516-121">Modify your sources list.</span></span>

   ```bash
   echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
   ```

4. <span data-ttu-id="13516-122">Execute os comandos sudo a seguir:</span><span class="sxs-lookup"><span data-stu-id="13516-122">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

5.  <span data-ttu-id="13516-123">Execute a CLI no prompt de comando com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="13516-123">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-on-debianubuntu-with-apt-get"></a><span data-ttu-id="13516-124">Instalar no Debian/Ubuntu com apt get</span><span class="sxs-lookup"><span data-stu-id="13516-124">Install on Debian/Ubuntu with apt-get</span></span>

<span data-ttu-id="13516-125">Para sistemas baseados em Debian/Ubuntu, instale a CLI 2.0 do Azure por meio de `apt-get`.</span><span class="sxs-lookup"><span data-stu-id="13516-125">For Debian/Ubuntu based systems, you can install Azure CLI 2.0 via `apt-get`.</span></span>

1. <span data-ttu-id="13516-126">Modifique sua lista de fontes:</span><span class="sxs-lookup"><span data-stu-id="13516-126">Modify your sources list:</span></span>
 
   - <span data-ttu-id="13516-127">sistema de 32 bits</span><span class="sxs-lookup"><span data-stu-id="13516-127">32-bit system</span></span>

     ```bash
     echo "deb https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

   - <span data-ttu-id="13516-128">sistema de 64 bits</span><span class="sxs-lookup"><span data-stu-id="13516-128">64-bit system</span></span>

     ```bash
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="13516-129">Execute os comandos sudo a seguir:</span><span class="sxs-lookup"><span data-stu-id="13516-129">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

3.  <span data-ttu-id="13516-130">Execute a CLI no prompt de comando com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="13516-130">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-on-rhel-fedora-and-centos-with-yum"></a><span data-ttu-id="13516-131">Instalar no RHEL, Fedora e CentOS com yum</span><span class="sxs-lookup"><span data-stu-id="13516-131">Install on RHEL, Fedora, and CentOS with yum</span></span>

<span data-ttu-id="13516-132">Para qualquer distribuição baseada no RedHat e que contenha o gerenciador de pacotes do `yum`, você poderá instalar a CLI do Azure 2.0 por meio do `yum`.</span><span class="sxs-lookup"><span data-stu-id="13516-132">For any distribution which is based off of RedHat and contains the `yum` package manager, you can install Azure CLI 2.0 via `yum`.</span></span>

1. <span data-ttu-id="13516-133">Importe a chave de repositório da Microsoft:</span><span class="sxs-lookup"><span data-stu-id="13516-133">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="13516-134">Crie informações sobre o repositório do `azure-cli` local:</span><span class="sxs-lookup"><span data-stu-id="13516-134">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="13516-135">Atualize o índice de pacote do `yum` e instale:</span><span class="sxs-lookup"><span data-stu-id="13516-135">Update the `yum` package index and install:</span></span>

   ```bash
   yum check-update
   sudo yum install azure-cli
   ```

4. <span data-ttu-id="13516-136">Execute a CLI no prompt de comando com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="13516-136">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-on-opensuse-and-sle-with-zypper"></a><span data-ttu-id="13516-137">Instalar no openSUSE e SLE com zypper</span><span class="sxs-lookup"><span data-stu-id="13516-137">Install on openSUSE and SLE with zypper</span></span>

1. <span data-ttu-id="13516-138">Importe a chave de repositório da Microsoft:</span><span class="sxs-lookup"><span data-stu-id="13516-138">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="13516-139">Crie informações sobre o repositório do `azure-cli` local:</span><span class="sxs-lookup"><span data-stu-id="13516-139">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ntype=rpm-md\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/zypp/repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="13516-140">Atualize o índice de pacote do `zypper` e instale:</span><span class="sxs-lookup"><span data-stu-id="13516-140">Update the `zypper` package index and install:</span></span>

   ```bash
   sudo zypper refresh
   sudo zypper install azure-cli
   ```

4. <span data-ttu-id="13516-141">Execute a CLI no prompt de comando com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="13516-141">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-with-docker"></a><span data-ttu-id="13516-142">Instalar com o Docker</span><span class="sxs-lookup"><span data-stu-id="13516-142">Install with Docker</span></span>

<span data-ttu-id="13516-143">Vamos manter uma imagem de Docker pré-configurada com a CLI do Azure 2.0.</span><span class="sxs-lookup"><span data-stu-id="13516-143">We maintain a Docker image preconfigured with the Azure CLI 2.0.</span></span>

<span data-ttu-id="13516-144">Instalar a CLI usando `docker run`.</span><span class="sxs-lookup"><span data-stu-id="13516-144">Install the CLI using `docker run`.</span></span>

   ```bash
   docker run azuresdk/azure-cli-python:<version>
   ```

<span data-ttu-id="13516-145">Confira nossas [marcas do Docker](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/) para versões disponíveis.</span><span class="sxs-lookup"><span data-stu-id="13516-145">See our [Docker tags](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/) for available versions.</span></span>

<span data-ttu-id="13516-146">A CLI está instalada na imagem como o comando `az` no `/usr/local/bin`.</span><span class="sxs-lookup"><span data-stu-id="13516-146">The CLI is installed on the image as the `az` command in `/usr/local/bin`.</span></span>

> [!NOTE]
> <span data-ttu-id="13516-147">Se você quiser acompanhar as chaves SSH do seu ambiente de usuário, use `-v ${HOME}:/root` para montar $HOME como `/root`.</span><span class="sxs-lookup"><span data-stu-id="13516-147">If you want to pick up the SSH keys from your user environment, you can use `-v ${HOME}:/root` to mount $HOME as `/root`.</span></span>

> ```bash
> docker run -v ${HOME}:/root azuresdk/azure-cli-python:<version>
> ```

## <a name="a-namelinuxinstall-on-linux-without-apt-get"></a><span data-ttu-id="13516-148"><a name="Linux"/>Instalar no Linux sem apt get</span><span class="sxs-lookup"><span data-stu-id="13516-148"><a name="Linux"/>Install on Linux without apt-get</span></span>

<span data-ttu-id="13516-149">É recomendável que você instale a CLI com um gerenciador de pacotes, se for possível.</span><span class="sxs-lookup"><span data-stu-id="13516-149">It is recommended that you install the CLI with a package manager if you are able to.</span></span> <span data-ttu-id="13516-150">Para as distribuições que não têm um pacote fornecido para elas, você pode instalar manualmente.</span><span class="sxs-lookup"><span data-stu-id="13516-150">For distributions which do not have a package provided for them, you can manually install.</span></span>

1. <span data-ttu-id="13516-151">Instale os pré-requisitos com base na sua distribuição do Linux.</span><span class="sxs-lookup"><span data-stu-id="13516-151">Install the prerequisites based on your Linux distribution.</span></span>

   ```
   Platform              | Prerequisites
   ----------------------|---------------------------------------------
   Ubuntu 15.10 or 16.04 | sudo apt-get update && sudo apt-get install -y python libssl-dev libffi-dev python-dev build-essential
   Ubuntu 12.04 or 14.04 | sudo apt-get update && sudo apt-get install -y python libssl-dev libffi-dev python-dev
   Debian 8              | sudo apt-get update && sudo apt-get install -y python libssl-dev libffi-dev python-dev build-essential
   Debian 7              | sudo apt-get update && sudo apt-get install -y python libssl-dev libffi-dev python-dev
   CentOS 7.1 or 7.2     | sudo yum check-update; sudo yum install -y gcc python libffi-devel python-devel openssl-devel
   RedHat 7.2            | sudo yum check-update; sudo yum install -y gcc python libffi-devel python-devel openssl-devel
   SUSE OpenSUSE 13.2    | sudo zypper refresh && sudo zypper --non-interactive install curl gcc python python-xml libffi-devel python-devel openssl-devel
   ```

<span data-ttu-id="13516-152">Se a distribuição não estiver listada acima, você precisará instalar [Python](https://www.python.org/downloads/), [libffi](https://sourceware.org/libffi/) e [OpenSSL](https://www.openssl.org/source/).</span><span class="sxs-lookup"><span data-stu-id="13516-152">If your distribution is not listed above, you will need to install [Python](https://www.python.org/downloads/), [libffi](https://sourceware.org/libffi/), and [OpenSSL](https://www.openssl.org/source/).</span></span>

2. <span data-ttu-id="13516-153">Instalar a CLI com `curl`.</span><span class="sxs-lookup"><span data-stu-id="13516-153">Install the CLI with  `curl`.</span></span>

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

3. <span data-ttu-id="13516-154">Talvez você precise reiniciar o shell para que algumas alterações entrem em vigor.</span><span class="sxs-lookup"><span data-stu-id="13516-154">You may have to restart your shell for some changes to take effect.</span></span>

   ```bash
   exec -l $SHELL
   ```

4. <span data-ttu-id="13516-155">Execute a CLI no prompt de comando com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="13516-155">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="13516-156">Solucionar problemas</span><span class="sxs-lookup"><span data-stu-id="13516-156">Troubleshooting</span></span>

<span data-ttu-id="13516-157">Se você encontrar um problema durante a instalação do CLI, verifique essa seção para ver se o seu caso específico é abordado.</span><span class="sxs-lookup"><span data-stu-id="13516-157">If you encounter an issue during CLI install, check this section to see if your particular case is covered.</span></span> <span data-ttu-id="13516-158">Se o problema não estiver aqui, [faça um registro do problema do Github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="13516-158">If your issue is not here, please [file a Github issue](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="curl-object-moved-error"></a><span data-ttu-id="13516-159">Erro "Objeto movido" de cURL</span><span class="sxs-lookup"><span data-stu-id="13516-159">curl "Object Moved" error</span></span>

<span data-ttu-id="13516-160">Se você receber um erro de `curl` relacionado ao parâmetro `-L` ou uma mensagem de erro incluindo o texto "Objeto movido", tente usar a URL completa em vez da `aka.ms` de redirecionamento:</span><span class="sxs-lookup"><span data-stu-id="13516-160">If you get an error from `curl` related to the `-L` parameter, or an error message including the text "Object Moved", try using the full URL instead of the `aka.ms` redirect:</span></span>

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="homebrew-on-macos-installing-older-version"></a><span data-ttu-id="13516-161">Instalação de versão mais antiga com o Homebrew no macOS</span><span class="sxs-lookup"><span data-stu-id="13516-161">Homebrew on macOS installing older version</span></span>

<span data-ttu-id="13516-162">A fórmula `azure-cli` de Homebrew disponível para macOS está atualmente desatualizada e instalará uma versão 1.x da CLI.</span><span class="sxs-lookup"><span data-stu-id="13516-162">The Homebrew `azure-cli` formula available for macOS is currently out of date, and will install a 1.x version of the CLI.</span></span> <span data-ttu-id="13516-163">Você pode ver quando ela é atualizada verificando `brew info azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="13516-163">You can see when it is updated by checking `brew info azure-cli`.</span></span>

<span data-ttu-id="13516-164">Até lá, [desinstale a versão mais antiga](#uninstall_brew) e siga as [instruções de instalação para macOS](#macOS).</span><span class="sxs-lookup"><span data-stu-id="13516-164">Until then, [uninstall the older version](#uninstall_brew) and follow the [macOS install instructions](#macOS).</span></span>

## <a name="uninstall-cli-1x-versions"></a><span data-ttu-id="13516-165">Desinstale as versões 1.x da CLI</span><span class="sxs-lookup"><span data-stu-id="13516-165">Uninstall CLI 1.x versions</span></span>

<span data-ttu-id="13516-166">Se você tiver uma versão anterior a 1.x da CLI disponível em seu sistema, você pode desinstalá-la com base no tipo de instalação usada.</span><span class="sxs-lookup"><span data-stu-id="13516-166">If you have an earlier CLI 1.x version available on your system, you can uninstall it based upon the type of install used.</span></span>

### <a name="uninstall-with-npm"></a><span data-ttu-id="13516-167">Desinstalar com NPM</span><span class="sxs-lookup"><span data-stu-id="13516-167">Uninstall with npm</span></span>

<span data-ttu-id="13516-168">Remover a CLI mais antiga com `npm uninstall`.</span><span class="sxs-lookup"><span data-stu-id="13516-168">Remove the older CLI with `npm uninstall`.</span></span>

  ```bash
  npm uninstall -g azure-cli
  ```

### <a name="a-nameuninstallbrewuninstall-with-homebrew-on-macos"></a><span data-ttu-id="13516-169"><a name="uninstall_brew"/>Desinstalar com Homebrew no macOS</span><span class="sxs-lookup"><span data-stu-id="13516-169"><a name="uninstall_brew"/>Uninstall with Homebrew on macOS</span></span>

<span data-ttu-id="13516-170">Remover a CLI mais antiga com `brew uninstall`.</span><span class="sxs-lookup"><span data-stu-id="13516-170">Remove the older CLI with `brew uninstall`.</span></span>

```bash
brew uninstall azure-cli
```

### <a name="uninstall-with-distributable"></a><span data-ttu-id="13516-171">Desinstalar com distribuível</span><span class="sxs-lookup"><span data-stu-id="13516-171">Uninstall with distributable</span></span>

<span data-ttu-id="13516-172">Se você tiver instalado por meio de [MSI](http://aka.ms/webpi-azure-cli) ou um [pacote de macOS](http://aka.ms/mac-azure-cli), use a mesma ferramenta para remover a instalação.</span><span class="sxs-lookup"><span data-stu-id="13516-172">If you installed via [MSI](http://aka.ms/webpi-azure-cli) or a [macOS package](http://aka.ms/mac-azure-cli), use the same tool to remove your install.</span></span>

### <a name="uninstall-with-docker"></a><span data-ttu-id="13516-173">Desinstalar com o Docker</span><span class="sxs-lookup"><span data-stu-id="13516-173">Uninstall with Docker</span></span>

<span data-ttu-id="13516-174">Se você instalou uma imagem do Docker para usar a versão anterior da CLI, remova a imagem e qualquer contêiner associado.</span><span class="sxs-lookup"><span data-stu-id="13516-174">If you installed a Docker image to use the earlier CLI version, remove that image and any associated containers.</span></span> <span data-ttu-id="13516-175">Você pode criar os contêineres novamente depois de instalar a nova imagem do Docker, conforme descrito nas instruções de instalação.</span><span class="sxs-lookup"><span data-stu-id="13516-175">You can then re-create the containers after installing the new Docker image as described in the install instructions.</span></span>

  ```bash
  docker rmi -f microsoft/azure-cli
  ```

## <a name="update-the-cli"></a><span data-ttu-id="13516-176">Atualizar a CLI</span><span class="sxs-lookup"><span data-stu-id="13516-176">Update the CLI</span></span>

<span data-ttu-id="13516-177">Para atualizar a CLI do Azure, use o mesmo método que você usou para instalá-la.</span><span class="sxs-lookup"><span data-stu-id="13516-177">To update the Azure CLI, use the same method that you used to install it.</span></span>

### <a name="update-with-msi"></a><span data-ttu-id="13516-178">Atualizar com MSI</span><span class="sxs-lookup"><span data-stu-id="13516-178">Update with MSI</span></span>

<span data-ttu-id="13516-179">Execute o [MSI](https://aka.ms/InstallAzureCliWindows) novamente.</span><span class="sxs-lookup"><span data-stu-id="13516-179">Run the [MSI](https://aka.ms/InstallAzureCliWindows) again.</span></span>

### <a name="update-with-apt-get"></a><span data-ttu-id="13516-180">Atualizar com apt get</span><span class="sxs-lookup"><span data-stu-id="13516-180">Update with apt-get</span></span>

<span data-ttu-id="13516-181">Use `apt-get upgrade` para atualizar o pacote da CLI.</span><span class="sxs-lookup"><span data-stu-id="13516-181">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="13516-182">Isso atualizará todos os pacotes instalados no sistema que não tiveram uma alteração de dependência.</span><span class="sxs-lookup"><span data-stu-id="13516-182">This will upgrade all of the installed packages on your system which have not had a dependency change.</span></span>
> <span data-ttu-id="13516-183">Para atualizar somente a CLI, use `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="13516-183">To upgrade only the CLI, use `apt-get install`.</span></span>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

### <a name="update-with-docker"></a><span data-ttu-id="13516-184">Atualizar com o Docker</span><span class="sxs-lookup"><span data-stu-id="13516-184">Update with Docker</span></span>

1. <span data-ttu-id="13516-185">Atualizar sua imagem local com `docker pull`.</span><span class="sxs-lookup"><span data-stu-id="13516-185">Update your local image with `docker pull`.</span></span>

   ```bash
   docker pull azuresdk/azure-cli-python
   ```

2. <span data-ttu-id="13516-186">Obter os contêineres atuais usando a imagem CLI.</span><span class="sxs-lookup"><span data-stu-id="13516-186">Get the containers currently using the CLI image.</span></span>

   ```bash
   docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```

> [!NOTE]
> <span data-ttu-id="13516-187">Se você instalou uma versão específica da imagem, você precisará adicionar `:<version>` ao final do nome da imagem.</span><span class="sxs-lookup"><span data-stu-id="13516-187">If you installed a specific version of the image, you will need to add `:<version>` to the end of the image name.</span></span>

3. <span data-ttu-id="13516-188">Interromper e recriar os contêineres.</span><span class="sxs-lookup"><span data-stu-id="13516-188">Halt and recreate the containers.</span></span>

   ```bash
   docker stop inspiring_benz
   docker rm inspiring_benz
   docker run azuresdk/azure-cli-python
   ```

### <a name="update-manually"></a><span data-ttu-id="13516-189">Atualizar manualmente</span><span class="sxs-lookup"><span data-stu-id="13516-189">Update manually</span></span>

<span data-ttu-id="13516-190">Siga as instruções de instalação manual para [macOS](#macOS) ou [Linux](#Linux) para atualizar.</span><span class="sxs-lookup"><span data-stu-id="13516-190">Follow the manual installation instructions for [macOS](#macOS) or [Linux](#Linux) to update.</span></span>

## <a name="uninstall"></a><span data-ttu-id="13516-191">Desinstalar</span><span class="sxs-lookup"><span data-stu-id="13516-191">Uninstall</span></span>

<span data-ttu-id="13516-192">Se você decidir desinstalar a CLI, lamentamos a sua saída.</span><span class="sxs-lookup"><span data-stu-id="13516-192">If you decide to uninstall the CLI, we're sorry to see you go.</span></span> <span data-ttu-id="13516-193">Você deve desinstalar usando o mesmo método que você usou para instalar a CLI.</span><span class="sxs-lookup"><span data-stu-id="13516-193">You should uninstall using the same method that you used to install the CLI.</span></span>

### <a name="uninstall-with-msi"></a><span data-ttu-id="13516-194">Desinstalar com MSI</span><span class="sxs-lookup"><span data-stu-id="13516-194">Uninstall with MSI</span></span>

<span data-ttu-id="13516-195">Execute o [MSI](https://aka.ms/InstallAzureCliWindows) novamente e escolha Desinstalar.</span><span class="sxs-lookup"><span data-stu-id="13516-195">Run the [MSI](https://aka.ms/InstallAzureCliWindows) again and choose uninstall.</span></span>

### <a name="uninstall-with-apt-get"></a><span data-ttu-id="13516-196">Desinstalar com apt-get</span><span class="sxs-lookup"><span data-stu-id="13516-196">Uninstall with apt-get</span></span>

<span data-ttu-id="13516-197">Desinstalar através de `apt-get remove`:</span><span class="sxs-lookup"><span data-stu-id="13516-197">Uninstall via `apt-get remove`:</span></span>

  ```bash
  sudo apt-get remove -y azure-cli
  ```

### <a name="uninstall-with-docker"></a><span data-ttu-id="13516-198">Desinstalar com o Docker</span><span class="sxs-lookup"><span data-stu-id="13516-198">Uninstall with Docker</span></span>

<span data-ttu-id="13516-199">Se você instalou uma imagem do Docker, será necessário remover qualquer contêiner que a estiver executando e, em seguida, excluir a imagem local.</span><span class="sxs-lookup"><span data-stu-id="13516-199">If you installed a docker image, you will need to remove any containers running it, and then delete the local image.</span></span>

1. <span data-ttu-id="13516-200">Obtenha os contêineres que estão executando a imagem da CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="13516-200">Get the containers which are running the azure-cli image.</span></span>

   ```bash
   docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```

2. <span data-ttu-id="13516-201">Exclua todos os contêineres com a imagem da CLI.</span><span class="sxs-lookup"><span data-stu-id="13516-201">Delete any containers with the CLI image.</span></span>

   ```bash
   docker rm 34a868beb2ab
   ```

3. <span data-ttu-id="13516-202">Remova a imagem da CLI instalada localmente.</span><span class="sxs-lookup"><span data-stu-id="13516-202">Remove the locally installed CLI image.</span></span>

   ```bash
   docker rmi azuresdk/azure-cli-python
   ```

> [!NOTE]
> <span data-ttu-id="13516-203">Se você instalou uma versão específica da imagem, você precisará adicionar `:<version>` ao final do nome da imagem.</span><span class="sxs-lookup"><span data-stu-id="13516-203">If you installed a specific version of the image, you will need to add `:<version>` to the end of the image name.</span></span>

### <a name="uninstall-manually"></a><span data-ttu-id="13516-204">Desinstalar manualmente</span><span class="sxs-lookup"><span data-stu-id="13516-204">Uninstall manually</span></span>

<span data-ttu-id="13516-205">Se você usou o script em https://aka.ms/InstallAzureCli para instalar a CLI, é possível desinstalá-la com estas etapas.</span><span class="sxs-lookup"><span data-stu-id="13516-205">If you used the script at https://aka.ms/InstallAzureCli to install the CLI, you can uninstall it with these steps.</span></span>

1. <span data-ttu-id="13516-206">Remova os arquivos instalados.</span><span class="sxs-lookup"><span data-stu-id="13516-206">Remove the installed files.</span></span>

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. <span data-ttu-id="13516-207">Exclua a linha `<install location>/lib/azure-cli/az.completion` de `<install location>/.bash_profile`.</span><span class="sxs-lookup"><span data-stu-id="13516-207">Delete the line `<install location>/lib/azure-cli/az.completion` from `<install location>/.bash_profile`.</span></span>

> [!Note]
> <span data-ttu-id="13516-208">O local de instalação padrão é `/Users/<username>`.</span><span class="sxs-lookup"><span data-stu-id="13516-208">The default install location is `/Users/<username>`.</span></span>

## <a name="report-cli-issues-and-feedback"></a><span data-ttu-id="13516-209">Relatar comentários e problemas da CLI</span><span class="sxs-lookup"><span data-stu-id="13516-209">Report CLI issues and feedback</span></span>

<span data-ttu-id="13516-210">Se você encontrar bugs na ferramenta, faça o registro do problema na seção [Problemas](https://github.com/Azure/azure-cli/issues) do nosso repositório do GitHub.</span><span class="sxs-lookup"><span data-stu-id="13516-210">If you encounter any bugs with the tool, file an issue in the [Issues](https://github.com/Azure/azure-cli/issues) section of our GitHub repository.</span></span>
<span data-ttu-id="13516-211">Para fornecer comentários na linha de comando, use o comando `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="13516-211">To provide feedback from the command line, use the `az feedback` command.</span></span>
