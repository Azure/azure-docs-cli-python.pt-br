---
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/29/2020
ms.topic: include
ms.custom: devx-track-azurecli
ms.openlocfilehash: 31b6a6e1c4c987ea351ccebc5d5bf23313ed856f
ms.sourcegitcommit: 547d3db8a1469f11d33e738a82d96cb51de61bd6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2021
ms.locfileid: "98147506"
---
## <a name="overview"></a><span data-ttu-id="2c71f-101">Visão geral</span><span class="sxs-lookup"><span data-stu-id="2c71f-101">Overview</span></span>

<span data-ttu-id="2c71f-102">O gerenciador de pacotes `apt` contém um pacote x86_64 para a CLI do Azure que foi testado nas distribuições a seguir.</span><span class="sxs-lookup"><span data-stu-id="2c71f-102">The `apt` package manager contains an x86_64 package for the Azure CLI that has been tested on the following distributions.</span></span>

| <span data-ttu-id="2c71f-103">Distribuição</span><span class="sxs-lookup"><span data-stu-id="2c71f-103">Distribution</span></span> | <span data-ttu-id="2c71f-104">Versão</span><span class="sxs-lookup"><span data-stu-id="2c71f-104">Version</span></span> |
|:-------------|:--------|
| <span data-ttu-id="2c71f-105">Ubuntu</span><span class="sxs-lookup"><span data-stu-id="2c71f-105">Ubuntu</span></span>       | <span data-ttu-id="2c71f-106">14.04 LTS (Trusty Tahir), 16.04 LTS (Xenial Xerus), 18.04 LTS (Bionic Beaver), 20.04 LTS (Focal Fossa), 20.10 (Groovy Gorilla)</span><span class="sxs-lookup"><span data-stu-id="2c71f-106">14.04 LTS (Trusty Tahir), 16.04 LTS (Xenial Xerus), 18.04 LTS (Bionic Beaver), 20.04 LTS (Focal Fossa), 20.10 (Groovy Gorilla)</span></span> |
| <span data-ttu-id="2c71f-107">Debian</span><span class="sxs-lookup"><span data-stu-id="2c71f-107">Debian</span></span>       | <span data-ttu-id="2c71f-108">Debian 8 (Jessie), Debian 9 (Stretch), Debian 10 (Buster)</span><span class="sxs-lookup"><span data-stu-id="2c71f-108">Debian 8 (Jessie), Debian 9 (Stretch), Debian 10 (Buster)</span></span> |

> [!WARNING]
> <span data-ttu-id="2c71f-109">Ubuntu 20.04 (Focal Fossa) e 20.10 (Groovy Gorilla) incluem um pacote `azure-cli` com a versão `2.0.81` fornecido pelo repositório `universe`.</span><span class="sxs-lookup"><span data-stu-id="2c71f-109">Ubuntu 20.04 (Focal Fossa) and 20.10 (Groovy Gorilla) include an `azure-cli` package with version `2.0.81` provided by the `universe` repository.</span></span> <span data-ttu-id="2c71f-110">Esse pacote está desatualizado e não é recomendado.</span><span class="sxs-lookup"><span data-stu-id="2c71f-110">This package is outdated and not recommended.</span></span> <span data-ttu-id="2c71f-111">Se esse pacote estiver instalado, remova-o antes de continuar executando o comando `sudo apt remove azure-cli -y && sudo apt autoremove -y`.</span><span class="sxs-lookup"><span data-stu-id="2c71f-111">If this package is installed, remove the package before continuing by running the command `sudo apt remove azure-cli -y && sudo apt autoremove -y`.</span></span>

## <a name="installation-options"></a><span data-ttu-id="2c71f-112">Opções de instalação</span><span class="sxs-lookup"><span data-stu-id="2c71f-112">Installation Options</span></span>

<span data-ttu-id="2c71f-113">Há duas formas de instalar a CLI do Azure no seu sistema.</span><span class="sxs-lookup"><span data-stu-id="2c71f-113">There are two options to install the Azure CLI on your system.</span></span>  <span data-ttu-id="2c71f-114">Primeiro, você pode executar um comando que vai baixar um script de instalação e executar os comandos de instalação.</span><span class="sxs-lookup"><span data-stu-id="2c71f-114">First, you may execute a single command that will download an install script and run the install commands for you.</span></span>  <span data-ttu-id="2c71f-115">Ou, se preferir, você pode executar os comandos de instalação por conta própria em um processo passo a passo.</span><span class="sxs-lookup"><span data-stu-id="2c71f-115">Or if you prefer, you can execute the install commands yourself in a step-by-step process.</span></span>  <span data-ttu-id="2c71f-116">Os dois métodos são apresentados abaixo.</span><span class="sxs-lookup"><span data-stu-id="2c71f-116">Both methods are provided below.</span></span>

## <a name="option-1-install-with-one-command"></a><span data-ttu-id="2c71f-117">Opção 1: Instalar com um comando</span><span class="sxs-lookup"><span data-stu-id="2c71f-117">Option 1: Install with one command</span></span>

<span data-ttu-id="2c71f-118">A equipe da CLI do Azure mantém um script para executar todos os comandos de instalação em uma etapa.</span><span class="sxs-lookup"><span data-stu-id="2c71f-118">The Azure CLI team maintains a script to run all installation commands in one step.</span></span>  <span data-ttu-id="2c71f-119">Esse script é baixado por meio de `curl` e encaminhado diretamente para `bash` a fim de instalar a CLI.</span><span class="sxs-lookup"><span data-stu-id="2c71f-119">This script is downloaded via `curl` and piped directly to `bash` to install the CLI.</span></span>

<span data-ttu-id="2c71f-120">Se você quiser inspecionar o conteúdo do script por conta própria antes de executá-lo, basta baixar o script usando `curl` e inspecioná-lo no seu editor de texto favorito.</span><span class="sxs-lookup"><span data-stu-id="2c71f-120">If you wish to inspect the contents of the script yourself before executing, simply download the script first using `curl` and inspect it in your favorite text editor.</span></span>

```bash
curl -sL https://aka.ms/InstallAzureCLIDeb | sudo bash
```

## <a name="option-2-step-by-step-installation-instructions"></a><span data-ttu-id="2c71f-121">Opção 2: Instruções de instalação passo a passo</span><span class="sxs-lookup"><span data-stu-id="2c71f-121">Option 2: Step-by-step installation instructions</span></span>

<span data-ttu-id="2c71f-122">Se você preferir um processo de instalação passo a passo, conclua as etapas a seguir para instalar a CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="2c71f-122">If you prefer a step-by-step installation process, complete the following steps to install the Azure CLI.</span></span>

1. <span data-ttu-id="2c71f-123">Obtenha os pacotes necessários para o processo de instalação:</span><span class="sxs-lookup"><span data-stu-id="2c71f-123">Get packages needed for the install process:</span></span>

    ```bash
    sudo apt-get update
    sudo apt-get install ca-certificates curl apt-transport-https lsb-release gnupg
    ```

2. <span data-ttu-id="2c71f-124">Baixe e instale a chave de autenticação da Microsoft:</span><span class="sxs-lookup"><span data-stu-id="2c71f-124">Download and install the Microsoft signing key:</span></span>

    ```bash
    curl -sL https://packages.microsoft.com/keys/microsoft.asc |
        gpg --dearmor |
        sudo tee /etc/apt/trusted.gpg.d/microsoft.gpg > /dev/null
    ```

3. <div id="set-release"/><span data-ttu-id="2c71f-125">Adicione o repositório de software da CLI do Azure (pule esta etapa em distribuições do Linux ARM64):</span><span class="sxs-lookup"><span data-stu-id="2c71f-125">Add the Azure CLI software repository (skip this step on ARM64 Linux distributions):</span></span>

    ```bash
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" |
        sudo tee /etc/apt/sources.list.d/azure-cli.list
    ```

4. <span data-ttu-id="2c71f-126">Atualize as informações do repositório e instale o pacote `azure-cli`:</span><span class="sxs-lookup"><span data-stu-id="2c71f-126">Update repository information and install the `azure-cli` package:</span></span>

    ```bash
    sudo apt-get update
    sudo apt-get install azure-cli
    ```

## <a name="sign-in-to-azure-with-the-azure-cli"></a><span data-ttu-id="2c71f-127">Entrar no Azure com a CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="2c71f-127">Sign in to Azure with the Azure CLI</span></span>

<span data-ttu-id="2c71f-128">Execute a CLI do Azure com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="2c71f-128">Run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="2c71f-129">Para entrar, use o comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="2c71f-129">To sign in, use the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](interactive-login.md)]

<span data-ttu-id="2c71f-130">Para saber mais sobre os diferentes métodos de autenticação, confira [Entrar com a CLI do Azure](../authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="2c71f-130">To learn more about different authentication methods, see [Sign in with Azure CLI](../authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="2c71f-131">Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="2c71f-131">Troubleshooting</span></span>

<span data-ttu-id="2c71f-132">Aqui estão alguns problemas comuns vistos durante a instalação com `apt`.</span><span class="sxs-lookup"><span data-stu-id="2c71f-132">Here are some common problems seen when installing with `apt`.</span></span> <span data-ttu-id="2c71f-133">Se você tiver um problema não abordado aqui, [arquive um problema no github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="2c71f-133">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="no-module-issue-on-ubuntu-2004-focalwsl"></a><span data-ttu-id="2c71f-134">Nenhum problema com o módulo no Ubuntu 20.04 (Focal)/WSL</span><span class="sxs-lookup"><span data-stu-id="2c71f-134">No module issue on Ubuntu 20.04 (Focal)/WSL</span></span>

<span data-ttu-id="2c71f-135">Se você tiver instalado `azure-cli` em `Focal` sem adicionar o repositório de software da CLI do Azure na [etapa 3](#set-release) das instruções de instalação manual ou sem usar nosso [script](#option-1-install-with-one-command), poderá encontrar problemas indicando, por exemplo, que não há nenhum módulo chamado "decorator" ou "antlr4", já que o pacote instalado é o `azure-cli 2.0.81` desatualizado do repositório `focal/universe`.</span><span class="sxs-lookup"><span data-stu-id="2c71f-135">If you installed `azure-cli` on `Focal` without adding the Azure CLI software repository in [step 3](#set-release) of the manual install instructions or using our [script](#option-1-install-with-one-command), you may encounter issues such as no module named 'decorator' or 'antlr4' as the package you installed is the outdated `azure-cli 2.0.81` from the `focal/universe` repository.</span></span> <span data-ttu-id="2c71f-136">Remova-a primeiro executando `sudo apt remove azure-cli -y && sudo apt autoremove -y` e, em seguida, siga as [instruções](#install) acima para instalar o pacote `azure-cli` mais recente.</span><span class="sxs-lookup"><span data-stu-id="2c71f-136">Please remove it first by running `sudo apt remove azure-cli -y && sudo apt autoremove -y`, then follow the above [instructions](#install) to install the latest `azure-cli` package.</span></span>

### <a name="lsb_release-does-not-return-the-correct-base-distribution-version"></a><span data-ttu-id="2c71f-137">lsb_release não retorna a versão correta da distribuição de base</span><span class="sxs-lookup"><span data-stu-id="2c71f-137">lsb_release does not return the correct base distribution version</span></span>

<span data-ttu-id="2c71f-138">Algumas distribuições derivadas do Ubuntu ou do Debian, como o Linux Mint, podem não retornar o nome correto da versão de `lsb_release`.</span><span class="sxs-lookup"><span data-stu-id="2c71f-138">Some Ubuntu- or Debian-derived distributions such as Linux Mint may not return the correct version name from `lsb_release`.</span></span> <span data-ttu-id="2c71f-139">Esse valor é usado no processo de instalação para determinar o pacote de instalação.</span><span class="sxs-lookup"><span data-stu-id="2c71f-139">This value is used in the install process to determine the package to install.</span></span> <span data-ttu-id="2c71f-140">Se você souber o nome do código da versão do Ubuntu ou do Debian da qual sua distribuição é derivada, poderá definir o valor de `AZ_REPO` manualmente ao [adicionar o repositório](#set-release).</span><span class="sxs-lookup"><span data-stu-id="2c71f-140">If you know the code name of the Ubuntu or Debian version your distribution is derived from, you can set the `AZ_REPO` value manually when [adding the repository](#set-release).</span></span> <span data-ttu-id="2c71f-141">Caso contrário, procure informações para sua distribuição sobre como determinar o nome do código da distribuição de base e defina `AZ_REPO` com o valor correto.</span><span class="sxs-lookup"><span data-stu-id="2c71f-141">Otherwise, look up information for your distribution on how to determine the base distribution code name and set `AZ_REPO` to the correct value.</span></span>

### <a name="no-package-for-your-distribution"></a><span data-ttu-id="2c71f-142">Nenhum pacote para distribuição</span><span class="sxs-lookup"><span data-stu-id="2c71f-142">No package for your distribution</span></span>

<span data-ttu-id="2c71f-143">Às vezes, um pacote da CLI do Azure pode ser disponibilizado somente um tempo depois do lançamento da distribuição.</span><span class="sxs-lookup"><span data-stu-id="2c71f-143">Sometimes it may be a while after a distribution is released before there's an Azure CLI package available for it.</span></span> <span data-ttu-id="2c71f-144">A CLI do Azure é projetada para ser resiliente em relação a versões futuras das dependências e precisam da menor quantidade possível delas.</span><span class="sxs-lookup"><span data-stu-id="2c71f-144">The Azure CLI designed to be resilient with regards to future versions of dependencies and rely on as few of them as possible.</span></span> <span data-ttu-id="2c71f-145">Se não houver pacotes disponíveis para sua distribuição de base, tente um pacote de uma distribuição anterior.</span><span class="sxs-lookup"><span data-stu-id="2c71f-145">If there's no package available for your base distribution, try a package for an earlier distribution.</span></span>

<span data-ttu-id="2c71f-146">Para isso, defina o valor de `AZ_REPO` manualmente ao [adicionar o repositório](#set-release).</span><span class="sxs-lookup"><span data-stu-id="2c71f-146">To do this, set the value of `AZ_REPO` manually when [adding the repository](#set-release).</span></span> <span data-ttu-id="2c71f-147">Para as distribuições do Ubuntu, use o repositório `bionic`; para as distribuições do Debian, use `stretch`.</span><span class="sxs-lookup"><span data-stu-id="2c71f-147">For Ubuntu distributions use the `bionic` repository, and for Debian distributions use `stretch`.</span></span> <span data-ttu-id="2c71f-148">Não há suporte para as distribuições lançadas antes do Ubuntu Trusty e do Debian Wheezy.</span><span class="sxs-lookup"><span data-stu-id="2c71f-148">Distributions released before Ubuntu Trusty and Debian Wheezy are not supported.</span></span>

### <a name="elementary-os-eos-fails-to-install-the-azure-cli"></a><span data-ttu-id="2c71f-149">O EOS (SO elementar) falha ao instalar a CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="2c71f-149">Elementary OS (EOS) fails to install the Azure CLI</span></span>

<span data-ttu-id="2c71f-150">O EOS não consegue instalar a CLI do Azure porque `lsb_release` retorna `HERA`, que é o nome da versão de EOS.</span><span class="sxs-lookup"><span data-stu-id="2c71f-150">EOS fails to install the Azure cli because `lsb_release` returns `HERA`, which is the EOS release name.</span></span>  <span data-ttu-id="2c71f-151">A solução é corrigir o arquivo `/etc/apt/sources.list.d/azure-cli.list` e alterar `hera main` para `bionic main`.</span><span class="sxs-lookup"><span data-stu-id="2c71f-151">The solution is to fix the file `/etc/apt/sources.list.d/azure-cli.list` and change `hera main` to `bionic main`.</span></span>

<span data-ttu-id="2c71f-152">Conteúdo do arquivo original:</span><span class="sxs-lookup"><span data-stu-id="2c71f-152">Original file contents:</span></span>

```
deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ hera main
```

<span data-ttu-id="2c71f-153">Conteúdo do arquivo modificado</span><span class="sxs-lookup"><span data-stu-id="2c71f-153">Modified file contents</span></span>

```
deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ bionic main
```

### <a name="proxy-blocks-connection"></a><span data-ttu-id="2c71f-154">Conexão de blocos de proxy</span><span class="sxs-lookup"><span data-stu-id="2c71f-154">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](configure-proxy.md)]

<span data-ttu-id="2c71f-155">Talvez você queira configurar explicitamente `apt` para usar esse proxy sempre.</span><span class="sxs-lookup"><span data-stu-id="2c71f-155">You may also want to explicitly configure `apt` to use this proxy at all times.</span></span> <span data-ttu-id="2c71f-156">Verifique se as linhas a seguir aparecem em um arquivo de configuração `apt` em `/etc/apt/apt.conf.d/`.</span><span class="sxs-lookup"><span data-stu-id="2c71f-156">Make sure that the following lines appear in an `apt` configuration file in `/etc/apt/apt.conf.d/`.</span></span> <span data-ttu-id="2c71f-157">É recomendável usar o arquivo de configuração global existente, um arquivo de configuração de proxy existente, `40proxies` ou `99local`. No entanto, siga os requisitos de administração do sistema.</span><span class="sxs-lookup"><span data-stu-id="2c71f-157">We recommend using either your existing global configuration file, an existing proxy configuration file, `40proxies`, or `99local`, but follow your system administration requirements.</span></span>

```apt.conf
Acquire {
    http::proxy "http://[username]:[password]@[proxy]:[port]";
    https::proxy "https://[username]:[password]@[proxy]:[port]";
}
```

<span data-ttu-id="2c71f-158">Se o proxy não usar autenticação básica, __remova__ a parte `[username]:[password]@` do URI do proxy.</span><span class="sxs-lookup"><span data-stu-id="2c71f-158">If your proxy does not use basic auth, __remove__ the `[username]:[password]@` portion of the proxy URI.</span></span> <span data-ttu-id="2c71f-159">Se você precisar de mais informações sobre a configuração do proxy, confira a documentação oficial do Ubuntu:</span><span class="sxs-lookup"><span data-stu-id="2c71f-159">If you require more information for proxy configuration, see the official Ubuntu documentation:</span></span>

* [<span data-ttu-id="2c71f-160">apt.conf manpage</span><span class="sxs-lookup"><span data-stu-id="2c71f-160">apt.conf manpage</span></span>](http://manpages.ubuntu.com/manpages/bionic/en/man5/apt.conf.5.html)
* [<span data-ttu-id="2c71f-161">Wiki do Ubuntu – apt-get howto</span><span class="sxs-lookup"><span data-stu-id="2c71f-161">Ubuntu wiki - apt-get howto</span></span>](https://help.ubuntu.com/community/AptGet/Howto#Setting_up_apt-get_to_use_a_http-proxy)

<span data-ttu-id="2c71f-162">Para obter a chave de assinatura da Microsoft e o pacote do nosso repositório, o proxy precisa permitir conexões HTTPS com o seguinte endereço:</span><span class="sxs-lookup"><span data-stu-id="2c71f-162">In order to get the Microsoft signing key and get the package from our repository, your proxy needs to allow HTTPS connections to the following address:</span></span>

* `https://packages.microsoft.com`

[!INCLUDE[troubleshoot-wsl.md](troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="2c71f-163">Atualizar</span><span class="sxs-lookup"><span data-stu-id="2c71f-163">Update</span></span>
[!INCLUDE [az-upgrade](az-upgrade.md)]

<span data-ttu-id="2c71f-164">Você também pode usar `apt-get upgrade` para atualizar o pacote da CLI.</span><span class="sxs-lookup"><span data-stu-id="2c71f-164">You can also use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="2c71f-165">Esse comando atualiza todos os pacotes instalados no sistema que não tiveram uma alteração de dependência.</span><span class="sxs-lookup"><span data-stu-id="2c71f-165">This command upgrades all of the installed packages on your system that have not had a dependency change.</span></span>
> <span data-ttu-id="2c71f-166">Para atualizar apenas a CLI, use `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="2c71f-166">To upgrade the CLI only, use `apt-get install`.</span></span>
>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a><span data-ttu-id="2c71f-167">Desinstalar</span><span class="sxs-lookup"><span data-stu-id="2c71f-167">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](uninstall-boilerplate.md)]

1. <span data-ttu-id="2c71f-168">Desinstalar com `apt-get remove`:</span><span class="sxs-lookup"><span data-stu-id="2c71f-168">Uninstall with `apt-get remove`:</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="2c71f-169">Se você não pretender reinstalar a CLI, remova as informações do repositório da CLI do Azure:</span><span class="sxs-lookup"><span data-stu-id="2c71f-169">If you don't plan to reinstall the CLI, remove the Azure CLI repository information:</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="2c71f-170">Se você não usa nenhum outro pacote da Microsoft, remova a chave de assinatura:</span><span class="sxs-lookup"><span data-stu-id="2c71f-170">If you use no other packages from Microsoft, remove the signing key:</span></span>

    ```bash
    sudo rm /etc/apt/trusted.gpg.d/microsoft.gpg
    ```

4. <span data-ttu-id="2c71f-171">Remova quaisquer pacotes desnecessários:</span><span class="sxs-lookup"><span data-stu-id="2c71f-171">Remove any unneeded packages:</span></span>

   ```bash
   sudo apt autoremove
   ```
