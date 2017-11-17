---
title: Instalar a CLI do Azure 2.0
description: "Documentos de referência para a instalação da CLI do Azure 2.0"
keywords: "CLI do Azure, Instalar a CLI do Azure, Azure Python CLI, Referência da CLI do Azure"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 11/01/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: ea5c0ee1-c530-4a1e-a83f-e1be71f6d416
ms.openlocfilehash: 2b56382355cad5313a604ed1f493a2bcbebf3e27
ms.sourcegitcommit: e9b4c6dd9093980b69ca47f93f44ac54d0e5b68a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2017
---
# <a name="install-azure-cli-20"></a><span data-ttu-id="87ce0-104">Instalar a CLI 2.0 do Azure</span><span class="sxs-lookup"><span data-stu-id="87ce0-104">Install Azure CLI 2.0</span></span>

<span data-ttu-id="87ce0-105">Instale hoje mesmo a nova versão da CLI do Azure!</span><span class="sxs-lookup"><span data-stu-id="87ce0-105">Install the new version of the Azure CLI today!</span></span>
<span data-ttu-id="87ce0-106">Nós a aprimoramos e atualizamos para fornecer uma ótima experiência de linha de comando nativa para gerenciar os recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="87ce0-106">We've improved and updated it to provide a great native command-line experience for managing Azure resources.</span></span>
<span data-ttu-id="87ce0-107">Ela pode ser usada em Windows, Linux e macOS.</span><span class="sxs-lookup"><span data-stu-id="87ce0-107">It can be used on macOS, Linux, and Windows.</span></span>
<span data-ttu-id="87ce0-108">Para saber mais sobre a versão mais recente, veja as [notas de versão](release-notes-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="87ce0-108">For information about the latest release, see the [release notes](release-notes-azure-cli.md).</span></span>

> [!NOTE]
> <span data-ttu-id="87ce0-109">Se você precisa da versão anterior da CLI do Azure, veja como [instalar a CLI do Azure 1.0](/azure/cli-install-nodejs).</span><span class="sxs-lookup"><span data-stu-id="87ce0-109">If you need the previous version of the Azure CLI, here's how to [install Azure CLI 1.0](/azure/cli-install-nodejs).</span></span>

## <a name="a-namemacosinstall-on-macos"></a><span data-ttu-id="87ce0-110"><a name="macOS"/>Instalar no macOS</span><span class="sxs-lookup"><span data-stu-id="87ce0-110"><a name="macOS"/>Install on macOS</span></span>

<span data-ttu-id="87ce0-111">No macOS, é possível instalar qualquer um com [Homebrew](https://brew.sh/) ou manualmente.</span><span class="sxs-lookup"><span data-stu-id="87ce0-111">On macOS, you are able to install either with [Homebrew](https://brew.sh/) or manually.</span></span>

### <a name="install-with-homebrew"></a><span data-ttu-id="87ce0-112">Instalar com o Homebrew</span><span class="sxs-lookup"><span data-stu-id="87ce0-112">Install with Homebrew</span></span>

1. <span data-ttu-id="87ce0-113">Se não tiver feito já, instale o Homebrew seguindo as [instruções de instalação do Homebrew](https://docs.brew.sh/Installation.html).</span><span class="sxs-lookup"><span data-stu-id="87ce0-113">If you don't have it already, install Homebrew by following the [Homebrew installation instructions](https://docs.brew.sh/Installation.html).</span></span>

2. <span data-ttu-id="87ce0-114">Se você instalou anteriormente a CLI manualmente, siga as instruções de [desinstalação manual](#UninstallManually).</span><span class="sxs-lookup"><span data-stu-id="87ce0-114">If you have previously installed the CLI manually, follow the [manual uninstall](#UninstallManually) instructions.</span></span>

3. <span data-ttu-id="87ce0-115">Atualize seus repositórios locais do Homebrew.</span><span class="sxs-lookup"><span data-stu-id="87ce0-115">Update your local Homebrew repositories.</span></span>

   ```bash
   brew update
   ```

4. <span data-ttu-id="87ce0-116">Instale o pacote `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="87ce0-116">Install the `azure-cli` package.</span></span>

  ```bash
  brew install azure-cli
  ```

> [!NOTE]
> <span data-ttu-id="87ce0-117">Se você instalou anteriormente a CLI do Azure 1.0 com o Homebrew, em vez de instalar com o pacote, pode obter a CLI 2.0 pelo processo de atualização regular do Homebrew.</span><span class="sxs-lookup"><span data-stu-id="87ce0-117">If you previously installed the Azure CLI 1.0 with Homebrew, instead of installing the package you can get CLI 2.0 through the regular Homebrew upgrade process.</span></span>
>
> ```bash
> brew upgrade
> ```

### <a name="install-manually"></a><span data-ttu-id="87ce0-118">Instalar manualmente</span><span class="sxs-lookup"><span data-stu-id="87ce0-118">Install manually</span></span>

1. <span data-ttu-id="87ce0-119">Instale a CLI do Azure 2.0 com `curl`.</span><span class="sxs-lookup"><span data-stu-id="87ce0-119">Install Azure CLI 2.0 with `curl`.</span></span>

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

2. <span data-ttu-id="87ce0-120">Talvez você precise reiniciar o shell para que algumas alterações entrem em vigor.</span><span class="sxs-lookup"><span data-stu-id="87ce0-120">You may have to restart your shell for some changes to take effect.</span></span>

   ```bash
   exec -l $SHELL
   ```
   
3. <span data-ttu-id="87ce0-121">Execute a CLI no prompt de comando com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="87ce0-121">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-on-windows"></a><span data-ttu-id="87ce0-122">Instalar no Windows</span><span class="sxs-lookup"><span data-stu-id="87ce0-122">Install on Windows</span></span>

### <a name="install-with-msi-for-the-windows-command-line"></a><span data-ttu-id="87ce0-123">Instalar com MSI para a linha de comando do Windows</span><span class="sxs-lookup"><span data-stu-id="87ce0-123">Install with MSI for the Windows command-line</span></span> 

<span data-ttu-id="87ce0-124">Para instalar a CLI no Windows e usá-la na linha de comando do Windows, baixe e execute o [Instalador da CLI do Azure (MSI)](https://aka.ms/InstallAzureCliWindows).</span><span class="sxs-lookup"><span data-stu-id="87ce0-124">To install the CLI on Windows and use it in the Windows command-line, download and run the [Azure CLI Installer (MSI)](https://aka.ms/InstallAzureCliWindows).</span></span>

### <a name="install-with-apt-get-for-bash-on-ubuntu-on-windows"></a><span data-ttu-id="87ce0-125">Instalar com apt-get para Bash no Ubuntu no Windows</span><span class="sxs-lookup"><span data-stu-id="87ce0-125">Install with apt-get for Bash on Ubuntu on Windows</span></span>

1. <span data-ttu-id="87ce0-126">Se você não tiver o Bash no Windows, [instale-o](https://msdn.microsoft.com/commandline/wsl/install_guide).</span><span class="sxs-lookup"><span data-stu-id="87ce0-126">If you don't have Bash on Windows, [install it](https://msdn.microsoft.com/commandline/wsl/install_guide).</span></span>

2. <span data-ttu-id="87ce0-127">Abra o shell do Bash.</span><span class="sxs-lookup"><span data-stu-id="87ce0-127">Open the Bash shell.</span></span>

3. <span data-ttu-id="87ce0-128">Modifique sua lista de fontes.</span><span class="sxs-lookup"><span data-stu-id="87ce0-128">Modify your sources list.</span></span>

   ```bash
   echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
   ```

4. <span data-ttu-id="87ce0-129">Execute os comandos sudo a seguir:</span><span class="sxs-lookup"><span data-stu-id="87ce0-129">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

5.  <span data-ttu-id="87ce0-130">Execute a CLI no prompt de comando com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="87ce0-130">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-with-apt-package-manager"></a><span data-ttu-id="87ce0-131">Instalar com gerenciador de pacotes apt</span><span class="sxs-lookup"><span data-stu-id="87ce0-131">Install with apt package manager</span></span> 

<span data-ttu-id="87ce0-132">Para obter distribuições usando o gerenciador de pacote `apt` como Ubuntu ou Debian, você pode instalar a CLI do Azure 2.0 via `apt-get`.</span><span class="sxs-lookup"><span data-stu-id="87ce0-132">For distributions using the `apt` package manager such as Ubuntu or Debian, you can install Azure CLI 2.0 via `apt-get`.</span></span>

> [!NOTE]
> <span data-ttu-id="87ce0-133">Você deve ter o Python 2.7.x ou Python 3.x para usar a CLI.</span><span class="sxs-lookup"><span data-stu-id="87ce0-133">You must have Python 2.7.x or Python 3.x in order to use the CLI.</span></span> <span data-ttu-id="87ce0-134">Se a distribuição não tiver um pacote para cada um, [instale o Python](https://www.python.org/downloads/).</span><span class="sxs-lookup"><span data-stu-id="87ce0-134">If your distribution does not have a package for either, [install Python](https://www.python.org/downloads/).</span></span>

1. <span data-ttu-id="87ce0-135">Modifique sua lista de fontes:</span><span class="sxs-lookup"><span data-stu-id="87ce0-135">Modify your sources list:</span></span>
 
   - <span data-ttu-id="87ce0-136">sistema de 32 bits</span><span class="sxs-lookup"><span data-stu-id="87ce0-136">32-bit system</span></span>

     ```bash
     echo "deb https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

   - <span data-ttu-id="87ce0-137">sistema de 64 bits</span><span class="sxs-lookup"><span data-stu-id="87ce0-137">64-bit system</span></span>

     ```bash
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="87ce0-138">Execute os comandos sudo a seguir:</span><span class="sxs-lookup"><span data-stu-id="87ce0-138">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

3.  <span data-ttu-id="87ce0-139">Execute a CLI no prompt de comando com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="87ce0-139">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-with-yum-package-manager"></a><span data-ttu-id="87ce0-140">Instalar com gerenciador de pacotes yum</span><span class="sxs-lookup"><span data-stu-id="87ce0-140">Install with yum package manager</span></span>

<span data-ttu-id="87ce0-141">Para as distribuições que usam o gerenciador de pacotes `yum` como Red Hat Enterprise Linux (RHEL), Fedora ou CentOS, você pode instalar o CLI do Azure 2.0 via `yum`.</span><span class="sxs-lookup"><span data-stu-id="87ce0-141">For distributions which use the `yum` package manager such as Red Hat Enterprise Linux (RHEL), Fedora, or CentOS, you can install Azure CLI 2.0 via `yum`.</span></span>

> [!NOTE]
> <span data-ttu-id="87ce0-142">Você deve ter o Python 2.7.x ou Python 3.x para usar a CLI.</span><span class="sxs-lookup"><span data-stu-id="87ce0-142">You must have Python 2.7.x or Python 3.x in order to use the CLI.</span></span> <span data-ttu-id="87ce0-143">Se a distribuição não tiver um pacote para cada um, [instale o Python](https://www.python.org/downloads/).</span><span class="sxs-lookup"><span data-stu-id="87ce0-143">If your distribution does not have a package for either, [install Python](https://www.python.org/downloads/).</span></span>

1. <span data-ttu-id="87ce0-144">Importe a chave de repositório da Microsoft:</span><span class="sxs-lookup"><span data-stu-id="87ce0-144">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="87ce0-145">Crie informações sobre o repositório do `azure-cli` local:</span><span class="sxs-lookup"><span data-stu-id="87ce0-145">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="87ce0-146">Atualize o índice de pacote do `yum` e instale:</span><span class="sxs-lookup"><span data-stu-id="87ce0-146">Update the `yum` package index and install:</span></span>

   ```bash
   yum check-update
   sudo yum install azure-cli
   ```

4. <span data-ttu-id="87ce0-147">Execute a CLI no prompt de comando com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="87ce0-147">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-with-zypper-package-manager"></a><span data-ttu-id="87ce0-148">Instalar com gerenciador de pacotes zypper</span><span class="sxs-lookup"><span data-stu-id="87ce0-148">Install with zypper package manager</span></span>

<span data-ttu-id="87ce0-149">Para distribuições que usam o gerenciador de pacotes `zypper` como OpenSUSE ou SLE, instale a CLI do Azure 2.0 via `zypper`.</span><span class="sxs-lookup"><span data-stu-id="87ce0-149">For distributions which use the `zypper` package manager such as OpenSUSE or SLE, you can install Azure CLI 2.0 via `zypper`.</span></span>

> [!NOTE]
> <span data-ttu-id="87ce0-150">Você deve ter o Python 2.7.x ou Python 3.x para usar a CLI.</span><span class="sxs-lookup"><span data-stu-id="87ce0-150">You must have Python 2.7.x or Python 3.x in order to use the CLI.</span></span> <span data-ttu-id="87ce0-151">Se a distribuição não tiver um pacote para cada um, [instale o Python](https://www.python.org/downloads/).</span><span class="sxs-lookup"><span data-stu-id="87ce0-151">If your distribution does not have a package for either, [install Python](https://www.python.org/downloads/).</span></span>

1. <span data-ttu-id="87ce0-152">Importe a chave de repositório da Microsoft:</span><span class="sxs-lookup"><span data-stu-id="87ce0-152">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="87ce0-153">Crie informações sobre o repositório do `azure-cli` local:</span><span class="sxs-lookup"><span data-stu-id="87ce0-153">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ntype=rpm-md\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/zypp/repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="87ce0-154">Atualize o índice de pacote do `zypper` e instale:</span><span class="sxs-lookup"><span data-stu-id="87ce0-154">Update the `zypper` package index and install:</span></span>

   ```bash
   sudo zypper refresh
   sudo zypper install azure-cli
   ```

4. <span data-ttu-id="87ce0-155">Execute a CLI no prompt de comando com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="87ce0-155">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-with-docker"></a><span data-ttu-id="87ce0-156">Instalar com o Docker</span><span class="sxs-lookup"><span data-stu-id="87ce0-156">Install with Docker</span></span>

<span data-ttu-id="87ce0-157">Vamos manter uma imagem de Docker pré-configurada com a CLI do Azure 2.0.</span><span class="sxs-lookup"><span data-stu-id="87ce0-157">We maintain a Docker image preconfigured with the Azure CLI 2.0.</span></span>

<span data-ttu-id="87ce0-158">Instalar a CLI usando `docker run`.</span><span class="sxs-lookup"><span data-stu-id="87ce0-158">Install the CLI using `docker run`.</span></span>

   ```bash
   docker run -it azuresdk/azure-cli-python:<version>
   ```

<span data-ttu-id="87ce0-159">Confira nossas [marcas do Docker](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/) para versões disponíveis.</span><span class="sxs-lookup"><span data-stu-id="87ce0-159">See our [Docker tags](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/) for available versions.</span></span>

<span data-ttu-id="87ce0-160">A CLI está instalada na imagem como o comando `az` no `/usr/local/bin`.</span><span class="sxs-lookup"><span data-stu-id="87ce0-160">The CLI is installed on the image as the `az` command in `/usr/local/bin`.</span></span>

> [!NOTE]
> <span data-ttu-id="87ce0-161">Se você quiser acompanhar as chaves SSH do seu ambiente de usuário, use `-v ${HOME}:/root` para montar $HOME como `/root`.</span><span class="sxs-lookup"><span data-stu-id="87ce0-161">If you want to pick up the SSH keys from your user environment, you can use `-v ${HOME}:/root` to mount $HOME as `/root`.</span></span>

> ```bash
> docker run -it -v ${HOME}:/root azuresdk/azure-cli-python:<version>
> ```

## <a name="a-namelinuxinstall-on-linux-without-a-package-manager"></a><span data-ttu-id="87ce0-162"><a name="Linux"/>Instalar no Linux sem um gerenciador de pacotes</span><span class="sxs-lookup"><span data-stu-id="87ce0-162"><a name="Linux"/>Install on Linux without a package manager</span></span>

<span data-ttu-id="87ce0-163">É recomendável que você instale a CLI com um gerenciador de pacotes, se for possível.</span><span class="sxs-lookup"><span data-stu-id="87ce0-163">It is recommended that you install the CLI with a package manager if you are able to.</span></span> <span data-ttu-id="87ce0-164">Se você não quiser adicionar repositórios da Microsoft, ou estiver trabalhando com uma distribuição que não tem um pacote fornecido, você pode instalar manualmente a CLI.</span><span class="sxs-lookup"><span data-stu-id="87ce0-164">If you do not want to add Microsoft's repositories, or are working with a distribution which does not have a provided package, you can manually install the CLI.</span></span>

1. <span data-ttu-id="87ce0-165">Instale os pré-requisitos com base na sua distribuição do Linux.</span><span class="sxs-lookup"><span data-stu-id="87ce0-165">Install the prerequisites based on your Linux distribution.</span></span>

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

<span data-ttu-id="87ce0-166">Se a distribuição não estiver listada acima, você precisará instalar o [Python 2.7 ou posterior](https://www.python.org/downloads/), [libffi](https://sourceware.org/libffi/) e [OpenSSL](https://www.openssl.org/source/).</span><span class="sxs-lookup"><span data-stu-id="87ce0-166">If your distribution is not listed above, you will need to install [Python 2.7 or later](https://www.python.org/downloads/), [libffi](https://sourceware.org/libffi/), and [OpenSSL](https://www.openssl.org/source/).</span></span>

2. <span data-ttu-id="87ce0-167">Instalar a CLI com `curl`.</span><span class="sxs-lookup"><span data-stu-id="87ce0-167">Install the CLI with  `curl`.</span></span>

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

3. <span data-ttu-id="87ce0-168">Talvez você precise reiniciar o shell para que algumas alterações entrem em vigor.</span><span class="sxs-lookup"><span data-stu-id="87ce0-168">You may have to restart your shell for some changes to take effect.</span></span>

   ```bash
   exec -l $SHELL
   ```

4. <span data-ttu-id="87ce0-169">Execute a CLI no prompt de comando com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="87ce0-169">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="87ce0-170">Solucionar problemas</span><span class="sxs-lookup"><span data-stu-id="87ce0-170">Troubleshooting</span></span>

<span data-ttu-id="87ce0-171">Se você encontrar um problema durante a instalação do CLI, verifique essa seção para ver se o seu caso específico é abordado.</span><span class="sxs-lookup"><span data-stu-id="87ce0-171">If you encounter an issue during CLI install, check this section to see if your particular case is covered.</span></span> <span data-ttu-id="87ce0-172">Se o problema não estiver aqui, [faça um registro do problema do Github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="87ce0-172">If your issue is not here, please [file a Github issue](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="curl-object-moved-error"></a><span data-ttu-id="87ce0-173">Erro "Objeto movido" de cURL</span><span class="sxs-lookup"><span data-stu-id="87ce0-173">curl "Object Moved" error</span></span>

<span data-ttu-id="87ce0-174">Se você receber um erro de `curl` relacionado ao parâmetro `-L` ou uma mensagem de erro incluindo o texto "Objeto movido", tente usar a URL completa em vez da `aka.ms` de redirecionamento:</span><span class="sxs-lookup"><span data-stu-id="87ce0-174">If you get an error from `curl` related to the `-L` parameter, or an error message including the text "Object Moved", try using the full URL instead of the `aka.ms` redirect:</span></span>

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a><span data-ttu-id="87ce0-175">`az` comando não encontrado</span><span class="sxs-lookup"><span data-stu-id="87ce0-175">`az` command not found</span></span>

<span data-ttu-id="87ce0-176">Talvez seja necessário limpar o cache de hash de comando do shell.</span><span class="sxs-lookup"><span data-stu-id="87ce0-176">You may need to clear your shell's command hash cache.</span></span> <span data-ttu-id="87ce0-177">Executar</span><span class="sxs-lookup"><span data-stu-id="87ce0-177">Run</span></span>

```bash
hash -r
```

<span data-ttu-id="87ce0-178">e ver se o problema foi resolvido.</span><span class="sxs-lookup"><span data-stu-id="87ce0-178">and see if the problem is resolved.</span></span> <span data-ttu-id="87ce0-179">O comando também pode não estar em seu `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="87ce0-179">The command may also not be in your `$PATH`.</span></span> <span data-ttu-id="87ce0-180">Verifique se `<install path>/bin` aparece em seu `$PATH` e reinicie o shell se necessário.</span><span class="sxs-lookup"><span data-stu-id="87ce0-180">Make sure that `<install path>/bin` appears in your `$PATH`, and restart your shell if necessary.</span></span>

## <a name="uninstall-cli-1x-versions"></a><span data-ttu-id="87ce0-181">Desinstale as versões 1.x da CLI</span><span class="sxs-lookup"><span data-stu-id="87ce0-181">Uninstall CLI 1.x versions</span></span>

<span data-ttu-id="87ce0-182">Se você tiver uma versão anterior a 1.x da CLI disponível em seu sistema, você pode desinstalá-la com base no tipo de instalação usada.</span><span class="sxs-lookup"><span data-stu-id="87ce0-182">If you have an earlier CLI 1.x version available on your system, you can uninstall it based upon the type of install used.</span></span>

### <a name="uninstall-with-npm"></a><span data-ttu-id="87ce0-183">Desinstalar com NPM</span><span class="sxs-lookup"><span data-stu-id="87ce0-183">Uninstall with npm</span></span>

<span data-ttu-id="87ce0-184">Remover a CLI mais antiga com `npm uninstall`.</span><span class="sxs-lookup"><span data-stu-id="87ce0-184">Remove the older CLI with `npm uninstall`.</span></span>

  ```bash
  npm uninstall -g azure-cli
  ```

### <a name="uninstall-with-distributable"></a><span data-ttu-id="87ce0-185">Desinstalar com distribuível</span><span class="sxs-lookup"><span data-stu-id="87ce0-185">Uninstall with distributable</span></span>

<span data-ttu-id="87ce0-186">Se você tiver instalado por meio do [Instalador da CLI do Azure (MSI)](http://aka.ms/webpi-azure-cli) ou de um [pacote de macOS](http://aka.ms/mac-azure-cli), use a mesma ferramenta para remover a instalação.</span><span class="sxs-lookup"><span data-stu-id="87ce0-186">If you installed via the [Azure CLI Installer (MSI)](http://aka.ms/webpi-azure-cli) or a [macOS package](http://aka.ms/mac-azure-cli), use the same tool to remove your install.</span></span>

### <a name="uninstall-with-docker"></a><span data-ttu-id="87ce0-187">Desinstalar com o Docker</span><span class="sxs-lookup"><span data-stu-id="87ce0-187">Uninstall with Docker</span></span>

<span data-ttu-id="87ce0-188">Se você instalou uma imagem do Docker para usar a versão anterior da CLI, remova a imagem e qualquer contêiner associado.</span><span class="sxs-lookup"><span data-stu-id="87ce0-188">If you installed a Docker image to use the earlier CLI version, remove that image and any associated containers.</span></span> <span data-ttu-id="87ce0-189">Você pode criar os contêineres novamente depois de instalar a nova imagem do Docker, conforme descrito nas instruções de instalação.</span><span class="sxs-lookup"><span data-stu-id="87ce0-189">You can then re-create the containers after installing the new Docker image as described in the install instructions.</span></span>

  ```bash
  docker rmi -f microsoft/azure-cli
  ```

## <a name="update-the-cli"></a><span data-ttu-id="87ce0-190">Atualizar a CLI</span><span class="sxs-lookup"><span data-stu-id="87ce0-190">Update the CLI</span></span>

<span data-ttu-id="87ce0-191">Para atualizar a CLI do Azure, use o mesmo método que você usou para instalá-la.</span><span class="sxs-lookup"><span data-stu-id="87ce0-191">To update the Azure CLI, use the same method that you used to install it.</span></span>

### <a name="update-with-homebrew"></a><span data-ttu-id="87ce0-192">Atualizar com o Homebrew</span><span class="sxs-lookup"><span data-stu-id="87ce0-192">Update with Homebrew</span></span>

1. <span data-ttu-id="87ce0-193">Se você tiver instalado manualmente, siga as instruções para [instalar com o Homebrew](#macOS).</span><span class="sxs-lookup"><span data-stu-id="87ce0-193">If you previously installed manually, follow the [install with Homebrew](#macOS) instructions.</span></span>

2. <span data-ttu-id="87ce0-194">Atualize suas informações de repositório do Homebrew local.</span><span class="sxs-lookup"><span data-stu-id="87ce0-194">Update your local Homebrew repository information.</span></span>

   ```bash
   brew update
   ```

3. <span data-ttu-id="87ce0-195">Atualize os seus pacotes instalados.</span><span class="sxs-lookup"><span data-stu-id="87ce0-195">Upgrade your installed packages.</span></span>

   ```bash
   brew upgrade
   ```

### <a name="update-with-msi"></a><span data-ttu-id="87ce0-196">Atualizar com MSI</span><span class="sxs-lookup"><span data-stu-id="87ce0-196">Update with MSI</span></span>

<span data-ttu-id="87ce0-197">Execute o [Instalador da CLI do Azure (MSI)](https://aka.ms/InstallAzureCliWindows) novamente.</span><span class="sxs-lookup"><span data-stu-id="87ce0-197">Run the [Azure CLI Installer (MSI)](https://aka.ms/InstallAzureCliWindows) again.</span></span>

### <a name="update-with-apt"></a><span data-ttu-id="87ce0-198">Atualizar com apt</span><span class="sxs-lookup"><span data-stu-id="87ce0-198">Update with apt</span></span>

<span data-ttu-id="87ce0-199">Use `apt-get upgrade` para atualizar o pacote da CLI.</span><span class="sxs-lookup"><span data-stu-id="87ce0-199">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="87ce0-200">Isso atualizará todos os pacotes instalados no sistema que não tiveram uma alteração de dependência.</span><span class="sxs-lookup"><span data-stu-id="87ce0-200">This will upgrade all of the installed packages on your system which have not had a dependency change.</span></span>
> <span data-ttu-id="87ce0-201">Para atualizar somente a CLI, use `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="87ce0-201">To upgrade only the CLI, use `apt-get install`.</span></span>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

### <a name="update-with-yum"></a><span data-ttu-id="87ce0-202">Atualizar com yum</span><span class="sxs-lookup"><span data-stu-id="87ce0-202">Update with yum</span></span>

<span data-ttu-id="87ce0-203">Atualize a CLI do Azure com o comando `yum update`.</span><span class="sxs-lookup"><span data-stu-id="87ce0-203">Update the Azure CLI with the `yum update` command.</span></span>

```bash
yum check-update
sudo yum update azure-cli
```

### <a name="update-with-zypper"></a><span data-ttu-id="87ce0-204">Atualizar com zypper</span><span class="sxs-lookup"><span data-stu-id="87ce0-204">Update with zypper</span></span>

<span data-ttu-id="87ce0-205">Você pode atualizar o pacote com o comando `zypper update`.</span><span class="sxs-lookup"><span data-stu-id="87ce0-205">You can update the package with the `zypper update` command.</span></span>

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

### <a name="update-with-docker"></a><span data-ttu-id="87ce0-206">Atualizar com o Docker</span><span class="sxs-lookup"><span data-stu-id="87ce0-206">Update with Docker</span></span>

1. <span data-ttu-id="87ce0-207">Atualizar sua imagem local com `docker pull`.</span><span class="sxs-lookup"><span data-stu-id="87ce0-207">Update your local image with `docker pull`.</span></span>

   ```bash
   docker pull azuresdk/azure-cli-python
   ```

2. <span data-ttu-id="87ce0-208">Obter os contêineres atuais usando a imagem CLI.</span><span class="sxs-lookup"><span data-stu-id="87ce0-208">Get the containers currently using the CLI image.</span></span>

   ```bash
   docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```

> [!NOTE]
> <span data-ttu-id="87ce0-209">Se você instalou uma versão específica da imagem, você precisará adicionar `:<version>` ao final do nome da imagem.</span><span class="sxs-lookup"><span data-stu-id="87ce0-209">If you installed a specific version of the image, you will need to add `:<version>` to the end of the image name.</span></span>

3. <span data-ttu-id="87ce0-210">Interromper e recriar os contêineres.</span><span class="sxs-lookup"><span data-stu-id="87ce0-210">Halt and recreate the containers.</span></span>

   ```bash
   docker stop inspiring_benz
   docker rm inspiring_benz
   docker run azuresdk/azure-cli-python
   ```

### <a name="update-manually"></a><span data-ttu-id="87ce0-211">Atualizar manualmente</span><span class="sxs-lookup"><span data-stu-id="87ce0-211">Update manually</span></span>

<span data-ttu-id="87ce0-212">Siga as instruções de instalação manual para [macOS](#macOS) ou [Linux](#Linux) para atualizar.</span><span class="sxs-lookup"><span data-stu-id="87ce0-212">Follow the manual installation instructions for [macOS](#macOS) or [Linux](#Linux) to update.</span></span>

## <a name="uninstall"></a><span data-ttu-id="87ce0-213">Desinstalar</span><span class="sxs-lookup"><span data-stu-id="87ce0-213">Uninstall</span></span>

<span data-ttu-id="87ce0-214">Se você decidir desinstalar a CLI, lamentamos a sua saída.</span><span class="sxs-lookup"><span data-stu-id="87ce0-214">If you decide to uninstall the CLI, we're sorry to see you go.</span></span> <span data-ttu-id="87ce0-215">Você deve desinstalar usando o mesmo método que você usou para instalar a CLI.</span><span class="sxs-lookup"><span data-stu-id="87ce0-215">You should uninstall using the same method that you used to install the CLI.</span></span>

### <a name="uninstall-with-homebrew"></a><span data-ttu-id="87ce0-216">Desinstalar com o Homebrew</span><span class="sxs-lookup"><span data-stu-id="87ce0-216">Uninstall with Homebrew</span></span>

<span data-ttu-id="87ce0-217">Desinstalar o pacote `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="87ce0-217">Uninstall the `azure-cli` package.</span></span>

   ```bash
   brew uninstall azure-cli
   ```

### <a name="uninstall-with-msi"></a><span data-ttu-id="87ce0-218">Desinstalar com MSI</span><span class="sxs-lookup"><span data-stu-id="87ce0-218">Uninstall with MSI</span></span>

<span data-ttu-id="87ce0-219">Execute o [MSI](https://aka.ms/InstallAzureCliWindows) novamente e escolha Desinstalar.</span><span class="sxs-lookup"><span data-stu-id="87ce0-219">Run the [MSI](https://aka.ms/InstallAzureCliWindows) again and choose uninstall.</span></span>

### <a name="uninstall-with-apt"></a><span data-ttu-id="87ce0-220">Desinstalar com apt</span><span class="sxs-lookup"><span data-stu-id="87ce0-220">Uninstall with apt</span></span>

<span data-ttu-id="87ce0-221">Desinstalar através de `apt-get remove`:</span><span class="sxs-lookup"><span data-stu-id="87ce0-221">Uninstall via `apt-get remove`:</span></span>

  ```bash
  sudo apt-get remove -y azure-cli
  ```

### <a name="uninstall-with-yum"></a><span data-ttu-id="87ce0-222">Desinstalar com yum</span><span class="sxs-lookup"><span data-stu-id="87ce0-222">Uninstall with yum</span></span>

1. <span data-ttu-id="87ce0-223">Remova o pacote do seu sistema.</span><span class="sxs-lookup"><span data-stu-id="87ce0-223">Remove the package from your system.</span></span>

   ```bash
   sudo yum remove azure-cli
   ```

2. <span data-ttu-id="87ce0-224">Se você não pretende reinstalar a CLI, remova as informações do repositório.</span><span class="sxs-lookup"><span data-stu-id="87ce0-224">If you do not plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="87ce0-225">Se você removeu as informações do repositório, remova também a chave de assinatura do Microsoft GPG.</span><span class="sxs-lookup"><span data-stu-id="87ce0-225">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```

### <a name="uninstall-with-zypper"></a><span data-ttu-id="87ce0-226">Desinstalar com zypper</span><span class="sxs-lookup"><span data-stu-id="87ce0-226">Uninstall with zypper</span></span>

1. <span data-ttu-id="87ce0-227">Remova o pacote do seu sistema.</span><span class="sxs-lookup"><span data-stu-id="87ce0-227">Remove the package from your system.</span></span>

    ```bash
    sudo zypper remove -y azure-cli
    ```

2. <span data-ttu-id="87ce0-228">Se você não pretende reinstalar a CLI, remova as informações do repositório.</span><span class="sxs-lookup"><span data-stu-id="87ce0-228">If you do not plan to reinstall the CLI, remove the repository information.</span></span>

  ```bash
  sudo rm /etc/zypp/repos.d/azure-cli.repo
  ```

3. <span data-ttu-id="87ce0-229">Se você removeu as informações do repositório, remova também a chave de assinatura do Microsoft GPG.</span><span class="sxs-lookup"><span data-stu-id="87ce0-229">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```

### <a name="uninstall-with-docker"></a><span data-ttu-id="87ce0-230">Desinstalar com o Docker</span><span class="sxs-lookup"><span data-stu-id="87ce0-230">Uninstall with Docker</span></span>

<span data-ttu-id="87ce0-231">Se você instalou uma imagem do Docker, será necessário remover qualquer contêiner que a estiver executando e, em seguida, excluir a imagem local.</span><span class="sxs-lookup"><span data-stu-id="87ce0-231">If you installed a docker image, you will need to remove any containers running it, and then delete the local image.</span></span>

1. <span data-ttu-id="87ce0-232">Obtenha os contêineres que estão executando a imagem da CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="87ce0-232">Get the containers which are running the azure-cli image.</span></span>

   ```bash
   docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```

2. <span data-ttu-id="87ce0-233">Exclua todos os contêineres com a imagem da CLI.</span><span class="sxs-lookup"><span data-stu-id="87ce0-233">Delete any containers with the CLI image.</span></span>

   ```bash
   docker rm 34a868beb2ab
   ```

3. <span data-ttu-id="87ce0-234">Remova a imagem da CLI instalada localmente.</span><span class="sxs-lookup"><span data-stu-id="87ce0-234">Remove the locally installed CLI image.</span></span>

   ```bash
   docker rmi azuresdk/azure-cli-python
   ```

> [!NOTE]
> <span data-ttu-id="87ce0-235">Se você instalou uma versão específica da imagem, você precisará adicionar `:<version>` ao final do nome da imagem.</span><span class="sxs-lookup"><span data-stu-id="87ce0-235">If you installed a specific version of the image, you will need to add `:<version>` to the end of the image name.</span></span>

###<a name="a-nameuninstallmanuallyuninstall-manually"></a><span data-ttu-id="87ce0-236"><a name="UninstallManually"/>Desinstalar manualmente</span><span class="sxs-lookup"><span data-stu-id="87ce0-236"><a name="UninstallManually"/>Uninstall manually</span></span>

<span data-ttu-id="87ce0-237">Se você usou o script em https://aka.ms/InstallAzureCli para instalar a CLI, é possível desinstalá-la com estas etapas.</span><span class="sxs-lookup"><span data-stu-id="87ce0-237">If you used the script at https://aka.ms/InstallAzureCli to install the CLI, you can uninstall it with these steps.</span></span>

1. <span data-ttu-id="87ce0-238">Remova os arquivos instalados.</span><span class="sxs-lookup"><span data-stu-id="87ce0-238">Remove the installed files.</span></span>

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. <span data-ttu-id="87ce0-239">Exclua a linha `<install location>/lib/azure-cli/az.completion` de `<install location>/.bash_profile`.</span><span class="sxs-lookup"><span data-stu-id="87ce0-239">Delete the line `<install location>/lib/azure-cli/az.completion` from `<install location>/.bash_profile`.</span></span>

3. <span data-ttu-id="87ce0-240">Se o shell usa um cache de comando, recarregue-o.</span><span class="sxs-lookup"><span data-stu-id="87ce0-240">If your shell uses a command cache, reload it.</span></span>

   ```bash
   hash -r
   ```

> [!Note]
> <span data-ttu-id="87ce0-241">O local de instalação padrão é `/Users/<username>`.</span><span class="sxs-lookup"><span data-stu-id="87ce0-241">The default install location is `/Users/<username>`.</span></span>

## <a name="report-cli-issues-and-feedback"></a><span data-ttu-id="87ce0-242">Relatar comentários e problemas da CLI</span><span class="sxs-lookup"><span data-stu-id="87ce0-242">Report CLI issues and feedback</span></span>

<span data-ttu-id="87ce0-243">Se você encontrar bugs na ferramenta, faça o registro do problema na seção [Problemas](https://github.com/Azure/azure-cli/issues) do nosso repositório do GitHub.</span><span class="sxs-lookup"><span data-stu-id="87ce0-243">If you encounter any bugs with the tool, file an issue in the [Issues](https://github.com/Azure/azure-cli/issues) section of our GitHub repository.</span></span>
<span data-ttu-id="87ce0-244">Para fornecer comentários na linha de comando, use o comando `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="87ce0-244">To provide feedback from the command line, use the `az feedback` command.</span></span>
