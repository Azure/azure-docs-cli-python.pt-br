---
title: Instalar a CLI do Azure 2.0
description: "Documentos de referência para a instalação da CLI do Azure 2.0"
keywords: "CLI do Azure 2.0, Referência da CLI do Azure 2.0, Instalar a CLI do Azure 2.0, CLI Python do Azure, Desinstalar a CLI do Azure 2.0, Referência da CLI do Azure"
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
ms.openlocfilehash: 00d5b555975007d7e57f04ce5d69f4f29e6d0219
ms.sourcegitcommit: f107cf927ea1ef51de181d87fc4bc078e9288e47
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2017
---
# <a name="install-azure-cli-20"></a><span data-ttu-id="f8d80-104">Instalar a CLI 2.0 do Azure</span><span class="sxs-lookup"><span data-stu-id="f8d80-104">Install Azure CLI 2.0</span></span>

<span data-ttu-id="f8d80-105">Instale hoje mesmo a nova versão da CLI do Azure!</span><span class="sxs-lookup"><span data-stu-id="f8d80-105">Install the new version of the Azure CLI today!</span></span>
<span data-ttu-id="f8d80-106">Nós a aprimoramos e atualizamos para fornecer uma ótima experiência de linha de comando nativa para gerenciar os recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="f8d80-106">We've improved and updated it to provide a great native command-line experience for managing Azure resources.</span></span>
<span data-ttu-id="f8d80-107">Ela pode ser usada em Windows, Linux e macOS.</span><span class="sxs-lookup"><span data-stu-id="f8d80-107">It can be used on macOS, Linux, and Windows.</span></span>
<span data-ttu-id="f8d80-108">Para saber mais sobre a versão mais recente, veja as [notas de versão](release-notes-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="f8d80-108">For information about the latest release, see the [release notes](release-notes-azure-cli.md).</span></span>

> [!NOTE]
> <span data-ttu-id="f8d80-109">Se você precisa da versão anterior da CLI do Azure, veja como [instalar a CLI do Azure 1.0](/azure/cli-install-nodejs).</span><span class="sxs-lookup"><span data-stu-id="f8d80-109">If you need the previous version of the Azure CLI, here's how to [install Azure CLI 1.0](/azure/cli-install-nodejs).</span></span>

## <a name="a-namemacosinstall-on-macos"></a><span data-ttu-id="f8d80-110"><a name="macOS"/>Instalar no macOS</span><span class="sxs-lookup"><span data-stu-id="f8d80-110"><a name="macOS"/>Install on macOS</span></span>

1. <span data-ttu-id="f8d80-111">Instale a CLI do Azure 2.0 com `curl`.</span><span class="sxs-lookup"><span data-stu-id="f8d80-111">Install Azure CLI 2.0 with `curl`.</span></span>

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

2. <span data-ttu-id="f8d80-112">Talvez você precise reiniciar o shell para que algumas alterações entrem em vigor.</span><span class="sxs-lookup"><span data-stu-id="f8d80-112">You may have to restart your shell for some changes to take effect.</span></span>

   ```bash
   exec -l $SHELL
   ```
   
3. <span data-ttu-id="f8d80-113">Execute a CLI no prompt de comando com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="f8d80-113">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-on-windows"></a><span data-ttu-id="f8d80-114">Instalar no Windows</span><span class="sxs-lookup"><span data-stu-id="f8d80-114">Install on Windows</span></span>

<span data-ttu-id="f8d80-115">É possível instalar a CLI do Azure 2.0 com o MSI e usá-la na linha de comando do Windows ou instalar a CLI com o `apt-get` no Bash, no Ubuntu no Windows.</span><span class="sxs-lookup"><span data-stu-id="f8d80-115">You can install Azure CLI 2.0 with the MSI and use it in the Windows command-line, or you can install the CLI with `apt-get` on Bash on Ubuntu on Windows.</span></span>

### <a name="install-with-msi-for-the-windows-command-line"></a><span data-ttu-id="f8d80-116">Instalar com MSI para a linha de comando do Windows</span><span class="sxs-lookup"><span data-stu-id="f8d80-116">Install with MSI for the Windows command-line</span></span> 

<span data-ttu-id="f8d80-117">Para instalar a CLI no Windows e usá-la na linha de comando do Windows, baixe e execute o [MSI](https://aka.ms/InstallAzureCliWindows).</span><span class="sxs-lookup"><span data-stu-id="f8d80-117">To install the CLI on Windows and use it in the Windows command-line, download and run the [MSI](https://aka.ms/InstallAzureCliWindows).</span></span>

### <a name="install-with-apt-get-for-bash-on-ubuntu-on-windows"></a><span data-ttu-id="f8d80-118">Instalar com apt-get para Bash no Ubuntu no Windows</span><span class="sxs-lookup"><span data-stu-id="f8d80-118">Install with apt-get for Bash on Ubuntu on Windows</span></span>

1. <span data-ttu-id="f8d80-119">Se você não tiver o Bash no Windows, [instale-o](https://msdn.microsoft.com/commandline/wsl/install_guide).</span><span class="sxs-lookup"><span data-stu-id="f8d80-119">If you don't have Bash on Windows, [install it](https://msdn.microsoft.com/commandline/wsl/install_guide).</span></span>

2. <span data-ttu-id="f8d80-120">Abra o shell do Bash.</span><span class="sxs-lookup"><span data-stu-id="f8d80-120">Open the Bash shell.</span></span>

3. <span data-ttu-id="f8d80-121">Modifique sua lista de fontes.</span><span class="sxs-lookup"><span data-stu-id="f8d80-121">Modify your sources list.</span></span>

   ```bash
   echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
   ```

4. <span data-ttu-id="f8d80-122">Execute os comandos sudo a seguir:</span><span class="sxs-lookup"><span data-stu-id="f8d80-122">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

5.  <span data-ttu-id="f8d80-123">Execute a CLI no prompt de comando com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="f8d80-123">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-on-debianubuntu-with-apt-get"></a><span data-ttu-id="f8d80-124">Instalar no Debian/Ubuntu com apt get</span><span class="sxs-lookup"><span data-stu-id="f8d80-124">Install on Debian/Ubuntu with apt-get</span></span>

<span data-ttu-id="f8d80-125">Para sistemas baseados em Debian/Ubuntu, instale a CLI 2.0 do Azure por meio de `apt-get`.</span><span class="sxs-lookup"><span data-stu-id="f8d80-125">For Debian/Ubuntu based systems, you can install Azure CLI 2.0 via `apt-get`.</span></span>

1. <span data-ttu-id="f8d80-126">Modifique sua lista de fontes.</span><span class="sxs-lookup"><span data-stu-id="f8d80-126">Modify your sources list.</span></span>
 
   - <span data-ttu-id="f8d80-127">sistema de 32 bits</span><span class="sxs-lookup"><span data-stu-id="f8d80-127">32-bit system</span></span>

     ```bash
     echo "deb https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

   - <span data-ttu-id="f8d80-128">sistema de 64 bits</span><span class="sxs-lookup"><span data-stu-id="f8d80-128">64-bit system</span></span>

     ```bash
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="f8d80-129">Execute os comandos sudo a seguir:</span><span class="sxs-lookup"><span data-stu-id="f8d80-129">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

3.  <span data-ttu-id="f8d80-130">Execute a CLI no prompt de comando com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="f8d80-130">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-with-docker"></a><span data-ttu-id="f8d80-131">Instalar com o Docker</span><span class="sxs-lookup"><span data-stu-id="f8d80-131">Install with Docker</span></span>

<span data-ttu-id="f8d80-132">Vamos manter uma imagem de Docker pré-configurada com a CLI do Azure 2.0.</span><span class="sxs-lookup"><span data-stu-id="f8d80-132">We maintain a Docker image preconfigured with the Azure CLI 2.0.</span></span>

<span data-ttu-id="f8d80-133">Instalar a CLI usando `docker run`.</span><span class="sxs-lookup"><span data-stu-id="f8d80-133">Install the CLI using `docker run`.</span></span>

  ```bash
  docker run azuresdk/azure-cli-python:<version>
  ```

<span data-ttu-id="f8d80-134">Confira nossas [marcas do Docker](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/) para versões disponíveis.</span><span class="sxs-lookup"><span data-stu-id="f8d80-134">See our [Docker tags](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/) for available versions.</span></span>

<span data-ttu-id="f8d80-135">A CLI está instalada na imagem como o comando `az` no `/usr/local/bin`.</span><span class="sxs-lookup"><span data-stu-id="f8d80-135">The CLI is installed on the image as the `az` command in `/usr/local/bin`.</span></span>

> [!NOTE]
> <span data-ttu-id="f8d80-136">Se você quiser acompanhar as chaves SSH do seu ambiente de usuário, use `-v ${HOME}:/root` para montar $HOME como `/root`.</span><span class="sxs-lookup"><span data-stu-id="f8d80-136">If you want to pick up the SSH keys from your user environment, you can use `-v ${HOME}:/root` to mount $HOME as `/root`.</span></span>

> ```bash
> docker run -v ${HOME}:/root azuresdk/azure-cli-python:<version>
> ```

## <a name="a-namelinuxinstall-on-linux-without-apt-get"></a><span data-ttu-id="f8d80-137"><a name="Linux"/>Instalar no Linux sem apt get</span><span class="sxs-lookup"><span data-stu-id="f8d80-137"><a name="Linux"/>Install on Linux without apt-get</span></span>

<span data-ttu-id="f8d80-138">É recomendável que você instale a CLI com `apt-get` se for possível.</span><span class="sxs-lookup"><span data-stu-id="f8d80-138">It is recommended that you install the CLI with `apt-get` if you are able to.</span></span> <span data-ttu-id="f8d80-139">Para as distribuições que não usam o gerenciador de pacote `apt`, você pode fazer a instalação manualmente.</span><span class="sxs-lookup"><span data-stu-id="f8d80-139">For distributions which do not use the `apt` package manager, you can manually install.</span></span>

1. <span data-ttu-id="f8d80-140">Instale os pré-requisitos com base na sua distribuição do Linux.</span><span class="sxs-lookup"><span data-stu-id="f8d80-140">Install the prerequisites based on your Linux distribution.</span></span>

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

<span data-ttu-id="f8d80-141">Se a distribuição não estiver listada acima, você precisará instalar [Python](https://www.python.org/downloads/), [libffi](https://sourceware.org/libffi/) e [OpenSSL](https://www.openssl.org/source/).</span><span class="sxs-lookup"><span data-stu-id="f8d80-141">If your distribution is not listed above, you will need to install [Python](https://www.python.org/downloads/), [libffi](https://sourceware.org/libffi/), and [OpenSSL](https://www.openssl.org/source/).</span></span>

2. <span data-ttu-id="f8d80-142">Instalar a CLI com `curl`.</span><span class="sxs-lookup"><span data-stu-id="f8d80-142">Install the CLI with  `curl`.</span></span>

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

3. <span data-ttu-id="f8d80-143">Talvez você precise reiniciar o shell para que algumas alterações entrem em vigor.</span><span class="sxs-lookup"><span data-stu-id="f8d80-143">You may have to restart your shell for some changes to take effect.</span></span>

   ```bash
   exec -l $SHELL
   ```

4. <span data-ttu-id="f8d80-144">Execute a CLI no prompt de comando com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="f8d80-144">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="f8d80-145">Solucionar problemas</span><span class="sxs-lookup"><span data-stu-id="f8d80-145">Troubleshooting</span></span>

<span data-ttu-id="f8d80-146">Se você encontrar um problema durante a instalação do CLI, verifique essa seção para ver se o seu caso específico é abordado.</span><span class="sxs-lookup"><span data-stu-id="f8d80-146">If you encounter an issue during CLI install, check this section to see if your particular case is covered.</span></span> <span data-ttu-id="f8d80-147">Se o problema não estiver aqui, [faça um registro do problema do Github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="f8d80-147">If your issue is not here, please [file a Github issue](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="curl-object-moved-error"></a><span data-ttu-id="f8d80-148">Erro "Objeto movido" de cURL</span><span class="sxs-lookup"><span data-stu-id="f8d80-148">curl "Object Moved" error</span></span>

<span data-ttu-id="f8d80-149">Se você receber um erro de `curl` relacionado ao parâmetro `-L` ou uma mensagem de erro incluindo o texto "Objeto movido", tente usar a URL completa em vez da `aka.ms` de redirecionamento:</span><span class="sxs-lookup"><span data-stu-id="f8d80-149">If you get an error from `curl` related to the `-L` parameter, or an error message including the text "Object Moved", try using the full URL instead of the `aka.ms` redirect:</span></span>

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="homebrew-on-macos-installing-older-version"></a><span data-ttu-id="f8d80-150">Instalação de versão mais antiga com o Homebrew no macOS</span><span class="sxs-lookup"><span data-stu-id="f8d80-150">Homebrew on macOS installing older version</span></span>

<span data-ttu-id="f8d80-151">A fórmula `azure-cli` de Homebrew disponível para macOS está atualmente desatualizada e instalará uma versão 1.x da CLI.</span><span class="sxs-lookup"><span data-stu-id="f8d80-151">The Homebrew `azure-cli` formula available for macOS is currently out of date, and will install a 1.x version of the CLI.</span></span> <span data-ttu-id="f8d80-152">Você pode ver quando ela é atualizada verificando `brew info azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="f8d80-152">You can see when it is updated by checking `brew info azure-cli`.</span></span>

<span data-ttu-id="f8d80-153">Até lá, [desinstale a versão mais antiga](#uninstall_brew) e siga as [instruções de instalação para macOS](#macOS).</span><span class="sxs-lookup"><span data-stu-id="f8d80-153">Until then, [uninstall the older version](#uninstall_brew) and follow the [macOS install instructions](#macOS).</span></span>

## <a name="uninstall-cli-1x-versions"></a><span data-ttu-id="f8d80-154">Desinstale as versões 1.x da CLI</span><span class="sxs-lookup"><span data-stu-id="f8d80-154">Uninstall CLI 1.x versions</span></span>

<span data-ttu-id="f8d80-155">Se você tiver uma versão anterior a 1.x da CLI disponível em seu sistema, você pode desinstalá-la com base no tipo de instalação usada.</span><span class="sxs-lookup"><span data-stu-id="f8d80-155">If you have an earlier CLI 1.x version available on your system, you can uninstall it based upon the type of install used.</span></span>

### <a name="uninstall-with-npm"></a><span data-ttu-id="f8d80-156">Desinstalar com NPM</span><span class="sxs-lookup"><span data-stu-id="f8d80-156">Uninstall with npm</span></span>

<span data-ttu-id="f8d80-157">Remover a CLI mais antiga com `npm uninstall`.</span><span class="sxs-lookup"><span data-stu-id="f8d80-157">Remove the older CLI with `npm uninstall`.</span></span>

  ```bash
  npm uninstall -g azure-cli
  ```

### <a name="a-nameuninstallbrewuninstall-with-homebrew-on-macos"></a><span data-ttu-id="f8d80-158"><a name="uninstall_brew"/>Desinstalar com Homebrew no macOS</span><span class="sxs-lookup"><span data-stu-id="f8d80-158"><a name="uninstall_brew"/>Uninstall with Homebrew on macOS</span></span>

<span data-ttu-id="f8d80-159">Remover a CLI mais antiga com `brew uninstall`.</span><span class="sxs-lookup"><span data-stu-id="f8d80-159">Remove the older CLI with `brew uninstall`.</span></span>

```bash
brew uninstall azure-cli
```

### <a name="uninstall-with-distributable"></a><span data-ttu-id="f8d80-160">Desinstalar com distribuível</span><span class="sxs-lookup"><span data-stu-id="f8d80-160">Uninstall with distributable</span></span>

<span data-ttu-id="f8d80-161">Se você tiver instalado por meio de [MSI](http://aka.ms/webpi-azure-cli) ou um [pacote de macOS](http://aka.ms/mac-azure-cli), use a mesma ferramenta para remover a instalação.</span><span class="sxs-lookup"><span data-stu-id="f8d80-161">If you installed via [MSI](http://aka.ms/webpi-azure-cli) or a [macOS package](http://aka.ms/mac-azure-cli), use the same tool to remove your install.</span></span>

### <a name="uninstall-with-docker"></a><span data-ttu-id="f8d80-162">Desinstalar com o Docker</span><span class="sxs-lookup"><span data-stu-id="f8d80-162">Uninstall with Docker</span></span>

<span data-ttu-id="f8d80-163">Se você instalou uma imagem do Docker para usar a versão anterior da CLI, remova a imagem e qualquer contêiner associado.</span><span class="sxs-lookup"><span data-stu-id="f8d80-163">If you installed a Docker image to use the earlier CLI version, remove that image and any associated containers.</span></span> <span data-ttu-id="f8d80-164">Você pode criar os contêineres novamente depois de instalar a nova imagem do Docker, conforme descrito nas instruções de instalação.</span><span class="sxs-lookup"><span data-stu-id="f8d80-164">You can then re-create the containers after installing the new Docker image as described in the install instructions.</span></span>

  ```bash
  docker rmi -f microsoft/azure-cli
  ```

## <a name="update-the-cli"></a><span data-ttu-id="f8d80-165">Atualizar a CLI</span><span class="sxs-lookup"><span data-stu-id="f8d80-165">Update the CLI</span></span>

<span data-ttu-id="f8d80-166">Para atualizar a CLI do Azure, use o mesmo método que você usou para instalá-la.</span><span class="sxs-lookup"><span data-stu-id="f8d80-166">To update the Azure CLI, use the same method that you used to install it.</span></span>

### <a name="update-with-msi"></a><span data-ttu-id="f8d80-167">Atualizar com MSI</span><span class="sxs-lookup"><span data-stu-id="f8d80-167">Update with MSI</span></span>

<span data-ttu-id="f8d80-168">Execute o [MSI](https://aka.ms/InstallAzureCliWindows) novamente.</span><span class="sxs-lookup"><span data-stu-id="f8d80-168">Run the [MSI](https://aka.ms/InstallAzureCliWindows) again.</span></span>

### <a name="update-with-apt-get"></a><span data-ttu-id="f8d80-169">Atualizar com apt get</span><span class="sxs-lookup"><span data-stu-id="f8d80-169">Update with apt-get</span></span>

<span data-ttu-id="f8d80-170">Use `apt-get upgrade` para atualizar o pacote da CLI.</span><span class="sxs-lookup"><span data-stu-id="f8d80-170">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="f8d80-171">Isso atualizará todos os pacotes instalados no sistema que não tiveram uma alteração de dependência.</span><span class="sxs-lookup"><span data-stu-id="f8d80-171">This will upgrade all of the installed packages on your system which have not had a dependency change.</span></span>
> <span data-ttu-id="f8d80-172">Para atualizar somente a CLI, use `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="f8d80-172">To upgrade only the CLI, use `apt-get install`.</span></span>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

### <a name="update-with-docker"></a><span data-ttu-id="f8d80-173">Atualizar com o Docker</span><span class="sxs-lookup"><span data-stu-id="f8d80-173">Update with Docker</span></span>

1. <span data-ttu-id="f8d80-174">Atualizar sua imagem local com `docker pull`.</span><span class="sxs-lookup"><span data-stu-id="f8d80-174">Update your local image with `docker pull`.</span></span>

   ```bash
   docker pull azuresdk/azure-cli-python
   ```

2. <span data-ttu-id="f8d80-175">Obter os contêineres atuais usando a imagem CLI.</span><span class="sxs-lookup"><span data-stu-id="f8d80-175">Get the containers currently using the CLI image.</span></span>

   ```bash
   docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```

> [!NOTE]
> <span data-ttu-id="f8d80-176">Se você instalou uma versão específica da imagem, você precisará adicionar `:<version>` ao final do nome da imagem.</span><span class="sxs-lookup"><span data-stu-id="f8d80-176">If you installed a specific version of the image, you will need to add `:<version>` to the end of the image name.</span></span>

3. <span data-ttu-id="f8d80-177">Interromper e recriar os contêineres.</span><span class="sxs-lookup"><span data-stu-id="f8d80-177">Halt and recreate the containers.</span></span>

   ```bash
   docker stop inspiring_benz
   docker rm inspiring_benz
   docker run azuresdk/azure-cli-python
   ```

### <a name="update-manually"></a><span data-ttu-id="f8d80-178">Atualizar manualmente</span><span class="sxs-lookup"><span data-stu-id="f8d80-178">Update manually</span></span>

<span data-ttu-id="f8d80-179">Siga as instruções de instalação manual para [macOS](#macOS) ou [Linux](#Linux) para atualizar.</span><span class="sxs-lookup"><span data-stu-id="f8d80-179">Follow the manual installation instructions for [macOS](#macOS) or [Linux](#Linux) to update.</span></span>

## <a name="uninstall"></a><span data-ttu-id="f8d80-180">Desinstalar</span><span class="sxs-lookup"><span data-stu-id="f8d80-180">Uninstall</span></span>

<span data-ttu-id="f8d80-181">Se você decidir desinstalar a CLI, lamentamos a sua saída.</span><span class="sxs-lookup"><span data-stu-id="f8d80-181">If you decide to uninstall the CLI, we're sorry to see you go.</span></span> <span data-ttu-id="f8d80-182">Você deve desinstalar usando o mesmo método que você usou para instalar a CLI.</span><span class="sxs-lookup"><span data-stu-id="f8d80-182">You should uninstall using the same method that you used to install the CLI.</span></span>

### <a name="uninstall-with-msi"></a><span data-ttu-id="f8d80-183">Desinstalar com MSI</span><span class="sxs-lookup"><span data-stu-id="f8d80-183">Uninstall with MSI</span></span>

<span data-ttu-id="f8d80-184">Execute o [MSI](https://aka.ms/InstallAzureCliWindows) novamente e escolha Desinstalar.</span><span class="sxs-lookup"><span data-stu-id="f8d80-184">Run the [MSI](https://aka.ms/InstallAzureCliWindows) again and choose uninstall.</span></span>

### <a name="uninstall-with-apt-get"></a><span data-ttu-id="f8d80-185">Desinstalar com apt-get</span><span class="sxs-lookup"><span data-stu-id="f8d80-185">Uninstall with apt-get</span></span>

<span data-ttu-id="f8d80-186">Desinstalar através de `apt-get remove`:</span><span class="sxs-lookup"><span data-stu-id="f8d80-186">Uninstall via `apt-get remove`:</span></span>

  ```bash
  sudo apt-get remove -y azure-cli
  ```

### <a name="uninstall-with-docker"></a><span data-ttu-id="f8d80-187">Desinstalar com o Docker</span><span class="sxs-lookup"><span data-stu-id="f8d80-187">Uninstall with Docker</span></span>

<span data-ttu-id="f8d80-188">Se você instalou uma imagem do Docker, será necessário remover qualquer contêiner que a estiver executando e, em seguida, excluir a imagem local.</span><span class="sxs-lookup"><span data-stu-id="f8d80-188">If you installed a docker image, you will need to remove any containers running it, and then delete the local image.</span></span>

1. <span data-ttu-id="f8d80-189">Obtenha os contêineres que estão executando a imagem da CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="f8d80-189">Get the containers which are running the azure-cli image.</span></span>

  ```bash
  docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
  ```

  ```output
  CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
  34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
  ```

2. <span data-ttu-id="f8d80-190">Exclua todos os contêineres com a imagem da CLI.</span><span class="sxs-lookup"><span data-stu-id="f8d80-190">Delete any containers with the CLI image.</span></span>

  ```bash
  docker rm 34a868beb2ab
  ```

3. <span data-ttu-id="f8d80-191">Remova a imagem da CLI instalada localmente.</span><span class="sxs-lookup"><span data-stu-id="f8d80-191">Remove the locally installed CLI image.</span></span>

  ```bash
  docker rmi azuresdk/azure-cli-python
  ```

> [!NOTE]
> <span data-ttu-id="f8d80-192">Se você instalou uma versão específica da imagem, você precisará adicionar `:<version>` ao final do nome da imagem.</span><span class="sxs-lookup"><span data-stu-id="f8d80-192">If you installed a specific version of the image, you will need to add `:<version>` to the end of the image name.</span></span>

### <a name="uninstall-manually"></a><span data-ttu-id="f8d80-193">Desinstalar manualmente</span><span class="sxs-lookup"><span data-stu-id="f8d80-193">Uninstall manually</span></span>

<span data-ttu-id="f8d80-194">Se você usou o script em https://aka.ms/InstallAzureCli para instalar a CLI, é possível desinstalá-la com estas etapas.</span><span class="sxs-lookup"><span data-stu-id="f8d80-194">If you used the script at https://aka.ms/InstallAzureCli to install the CLI, you can uninstall it with these steps.</span></span>

1. <span data-ttu-id="f8d80-195">Remova os arquivos instalados.</span><span class="sxs-lookup"><span data-stu-id="f8d80-195">Remove the installed files.</span></span>

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. <span data-ttu-id="f8d80-196">Exclua a linha `<install location>/lib/azure-cli/az.completion` de `<install location>/.bash_profile`.</span><span class="sxs-lookup"><span data-stu-id="f8d80-196">Delete the line `<install location>/lib/azure-cli/az.completion` from `<install location>/.bash_profile`.</span></span>

> [!Note]
> <span data-ttu-id="f8d80-197">O local de instalação padrão é `/Users/<username>`.</span><span class="sxs-lookup"><span data-stu-id="f8d80-197">The default install location is `/Users/<username>`.</span></span>

## <a name="report-cli-issues-and-feedback"></a><span data-ttu-id="f8d80-198">Relatar comentários e problemas da CLI</span><span class="sxs-lookup"><span data-stu-id="f8d80-198">Report CLI issues and feedback</span></span>

<span data-ttu-id="f8d80-199">Se você encontrar bugs na ferramenta, faça o registro do problema na seção [Problemas](https://github.com/Azure/azure-cli/issues) do nosso repositório do GitHub.</span><span class="sxs-lookup"><span data-stu-id="f8d80-199">If you encounter any bugs with the tool, file an issue in the [Issues](https://github.com/Azure/azure-cli/issues) section of our GitHub repository.</span></span>
<span data-ttu-id="f8d80-200">Para fornecer comentários na linha de comando, use o comando `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="f8d80-200">To provide feedback from the command line, use the `az feedback` command.</span></span>
