---
title: Instalar a CLI do Azure no Linux com apt
description: Como instalar a CLI do Azure com o gerenciador de pacotes apt
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/29/2020
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 242c634717cf964af718873ab9ecf84ff707db3d
ms.sourcegitcommit: aa44ec97af5c0e7558d254b3159f95921e22ff1c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/01/2020
ms.locfileid: "91625407"
---
# <a name="install-azure-cli-with-apt"></a><span data-ttu-id="cc62f-103">Instalar CLI do Azure com o apt</span><span class="sxs-lookup"><span data-stu-id="cc62f-103">Install Azure CLI with apt</span></span>

<span data-ttu-id="cc62f-104">Se você estiver executando uma distribuição fornecida com `apt`, como Ubuntu ou Debian, há um pacote x86_64 disponível para a CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="cc62f-104">If you are running a distribution that comes with `apt`, such as Ubuntu or Debian, there's an x86_64 package available for the Azure CLI.</span></span> <span data-ttu-id="cc62f-105">Este pacote foi testado e é compatível com:</span><span class="sxs-lookup"><span data-stu-id="cc62f-105">This package has been tested with and is supported for:</span></span>

* <span data-ttu-id="cc62f-106">Ubuntu trusty, xenial, Bionic, eoan e focal</span><span class="sxs-lookup"><span data-stu-id="cc62f-106">Ubuntu trusty, xenial, bionic, eoan and focal</span></span>
* <span data-ttu-id="cc62f-107">Debian jessie, stretch e buster</span><span class="sxs-lookup"><span data-stu-id="cc62f-107">Debian jessie, stretch, and buster</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

> [!NOTE]
>
> <span data-ttu-id="cc62f-108">O pacote para a CLI do Azure instala seu próprio interpretador de Python e não usa o Python do sistema.</span><span class="sxs-lookup"><span data-stu-id="cc62f-108">The package for Azure CLI installs its own Python interpreter, and does not use the system Python.</span></span> 
>
> <span data-ttu-id="cc62f-109">No Ubuntu 20.04 (Focal), há um pacote `azure-cli` com a versão `2.0.81` fornecida pelo repositório `focal/universe`.</span><span class="sxs-lookup"><span data-stu-id="cc62f-109">On Ubuntu 20.04 (Focal), there is an `azure-cli` package with version `2.0.81` provided by the `focal/universe` repository.</span></span> <span data-ttu-id="cc62f-110">Ele está desatualizado e não é recomendado.</span><span class="sxs-lookup"><span data-stu-id="cc62f-110">It's outdated and not recommended.</span></span> <span data-ttu-id="cc62f-111">Se você já o instalou, remova-o primeiro executando `sudo apt remove azure-cli -y && sudo apt autoremove -y` antes de seguir as etapas abaixo para instalar o pacote `azure-cli` mais recente.</span><span class="sxs-lookup"><span data-stu-id="cc62f-111">If you already installed it, please remove it first by running `sudo apt remove azure-cli -y && sudo apt autoremove -y` before following the below steps to install the latest `azure-cli` package.</span></span>

## <a name="install"></a><span data-ttu-id="cc62f-112">Instalar</span><span class="sxs-lookup"><span data-stu-id="cc62f-112">Install</span></span>

<span data-ttu-id="cc62f-113">Oferecemos duas maneiras de instalar a CLI do Azure com distribuições que dão suporte a `apt`: Como um script tudo-em-um que executa os comandos de instalação para você, e instruções que podem ser executadas como um processo passo a passo por conta própria.</span><span class="sxs-lookup"><span data-stu-id="cc62f-113">We offer two ways to install the Azure CLI with distributions that support `apt`: As an all-in-one script that runs the install commands for you, and instructions that you can run as a step-by-step process on your own.</span></span>

### <a name="install-with-one-command"></a><span data-ttu-id="cc62f-114">Instalar com um comando</span><span class="sxs-lookup"><span data-stu-id="cc62f-114">Install with one command</span></span>

<span data-ttu-id="cc62f-115">Oferecemos e mantemos um script que executa todos os comandos de instalação em uma única etapa.</span><span class="sxs-lookup"><span data-stu-id="cc62f-115">We offer and maintain a script which runs all of the installation commands in one step.</span></span> <span data-ttu-id="cc62f-116">Executá-lo usando `curl` e redirecione diretamente para `bash`, ou baixe o script para um arquivo e inspecione-o antes da execução.</span><span class="sxs-lookup"><span data-stu-id="cc62f-116">Run it by using `curl` and pipe directly to `bash`, or download the script to a file and inspect it before running.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="cc62f-117">Esse script é verificado somente para o Ubuntu 16.04+ e Debian 8+.</span><span class="sxs-lookup"><span data-stu-id="cc62f-117">This script is only verified for Ubuntu 16.04+ and Debian 8+.</span></span> <span data-ttu-id="cc62f-118">Ele pode não funcionar em outras distribuições.</span><span class="sxs-lookup"><span data-stu-id="cc62f-118">It may not work on other distributions.</span></span>
> <span data-ttu-id="cc62f-119">Se você estiver usando uma distribuição derivada como Linux Mint, siga as instruções de instalação manual e execute qualquer solução de problemas necessária.</span><span class="sxs-lookup"><span data-stu-id="cc62f-119">If you're using a derived distribution such as Linux Mint, follow the manual install instructions and perform any necessary troubleshooting.</span></span>

```bash
curl -sL https://aka.ms/InstallAzureCLIDeb | sudo bash
```

### <a name="manual-install-instructions"></a><span data-ttu-id="cc62f-120">Instruções para instalação manual</span><span class="sxs-lookup"><span data-stu-id="cc62f-120">Manual install instructions</span></span>

<span data-ttu-id="cc62f-121">Se você não quiser executar um script como superusuário ou se o script tudo-em-um falhar, siga estas etapas para instalar a CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="cc62f-121">If you don't want to run a script as superuser or the all-in-one script fails, follow these steps to install the Azure CLI.</span></span>

1. <span data-ttu-id="cc62f-122">Obtenha os pacotes necessários para o processo de instalação:</span><span class="sxs-lookup"><span data-stu-id="cc62f-122">Get packages needed for the install process:</span></span>

    ```bash
    sudo apt-get update
    sudo apt-get install ca-certificates curl apt-transport-https lsb-release gnupg
    ```

2. <span data-ttu-id="cc62f-123">Baixe e instale a chave de autenticação da Microsoft:</span><span class="sxs-lookup"><span data-stu-id="cc62f-123">Download and install the Microsoft signing key:</span></span>

    ```bash
    curl -sL https://packages.microsoft.com/keys/microsoft.asc |
        gpg --dearmor |
        sudo tee /etc/apt/trusted.gpg.d/microsoft.gpg > /dev/null
    ```

3. <div id="set-release"/><span data-ttu-id="cc62f-124">Adicione o repositório de software da CLI do Azure:</span><span class="sxs-lookup"><span data-stu-id="cc62f-124">Add the Azure CLI software repository:</span></span>

    ```bash
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" |
        sudo tee /etc/apt/sources.list.d/azure-cli.list
    ```

4. <span data-ttu-id="cc62f-125">Atualize as informações do repositório e instale o pacote `azure-cli`:</span><span class="sxs-lookup"><span data-stu-id="cc62f-125">Update repository information and install the `azure-cli` package:</span></span>

    ```bash
    sudo apt-get update
    sudo apt-get install azure-cli
    ```

<span data-ttu-id="cc62f-126">Execute a CLI do Azure com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="cc62f-126">Run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="cc62f-127">Para entrar, use o comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="cc62f-127">To sign in, use the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="cc62f-128">Para saber mais sobre os diferentes métodos de autenticação, confira [Entrar com a CLI do Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="cc62f-128">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="cc62f-129">Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="cc62f-129">Troubleshooting</span></span>

<span data-ttu-id="cc62f-130">Aqui estão alguns problemas comuns vistos durante a instalação com `apt`.</span><span class="sxs-lookup"><span data-stu-id="cc62f-130">Here are some common problems seen when installing with `apt`.</span></span> <span data-ttu-id="cc62f-131">Se você tiver um problema não abordado aqui, [arquive um problema no github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="cc62f-131">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="no-module-issue-on-ubuntu-2004-focalwsl"></a><span data-ttu-id="cc62f-132">Nenhum problema com o módulo no Ubuntu 20.04 (Focal)/WSL</span><span class="sxs-lookup"><span data-stu-id="cc62f-132">No module issue on Ubuntu 20.04 (Focal)/WSL</span></span>
<span data-ttu-id="cc62f-133">Se você tiver instalado `azure-cli` em `Focal` sem adicionar o repositório de software da CLI do Azure na [etapa 3](#set-release) das instruções de instalação manual ou sem usar nosso [script](#install-with-one-command), poderá encontrar problemas indicando, por exemplo, que não há nenhum módulo chamado "decorator" ou "antlr4", já que o pacote instalado é o `azure-cli 2.0.81` desatualizado do repositório `focal/universe`.</span><span class="sxs-lookup"><span data-stu-id="cc62f-133">If you installed `azure-cli` on `Focal` without adding the Azure CLI software repository in [step 3](#set-release) of the manual install instructions or using our [script](#install-with-one-command), you may encounter issues such as no module named 'decorator' or 'antlr4' as the package you installed is the outdated `azure-cli 2.0.81` from the `focal/universe` repository.</span></span> <span data-ttu-id="cc62f-134">Remova-a primeiro executando `sudo apt remove azure-cli -y && sudo apt autoremove -y` e, em seguida, siga as [instruções](#install) acima para instalar o pacote `azure-cli` mais recente.</span><span class="sxs-lookup"><span data-stu-id="cc62f-134">Please remove it first by running `sudo apt remove azure-cli -y && sudo apt autoremove -y`, then follow the above [instructions](#install) to install the latest `azure-cli` package.</span></span>

### <a name="lsb_release-does-not-return-the-correct-base-distribution-version"></a><span data-ttu-id="cc62f-135">lsb_release não retorna a versão correta da distribuição de base</span><span class="sxs-lookup"><span data-stu-id="cc62f-135">lsb_release does not return the correct base distribution version</span></span>

<span data-ttu-id="cc62f-136">Algumas distribuições derivadas do Ubuntu ou do Debian, como o Linux Mint, podem não retornar o nome correto da versão de `lsb_release`.</span><span class="sxs-lookup"><span data-stu-id="cc62f-136">Some Ubuntu- or Debian-derived distributions such as Linux Mint may not return the correct version name from `lsb_release`.</span></span> <span data-ttu-id="cc62f-137">Esse valor é usado no processo de instalação para determinar o pacote de instalação.</span><span class="sxs-lookup"><span data-stu-id="cc62f-137">This value is used in the install process to determine the package to install.</span></span> <span data-ttu-id="cc62f-138">Se você souber o nome do código da versão do Ubuntu ou do Debian da qual sua distribuição é derivada, poderá definir o valor de `AZ_REPO` manualmente ao [adicionar o repositório](#set-release).</span><span class="sxs-lookup"><span data-stu-id="cc62f-138">If you know the code name of the Ubuntu or Debian version your distribution is derived from, you can set the `AZ_REPO` value manually when [adding the repository](#set-release).</span></span> <span data-ttu-id="cc62f-139">Caso contrário, procure informações para sua distribuição sobre como determinar o nome do código da distribuição de base e defina `AZ_REPO` com o valor correto.</span><span class="sxs-lookup"><span data-stu-id="cc62f-139">Otherwise, look up information for your distribution on how to determine the base distribution code name and set `AZ_REPO` to the correct value.</span></span>

### <a name="no-package-for-your-distribution"></a><span data-ttu-id="cc62f-140">Nenhum pacote para distribuição</span><span class="sxs-lookup"><span data-stu-id="cc62f-140">No package for your distribution</span></span>

<span data-ttu-id="cc62f-141">Às vezes, um pacote da CLI do Azure pode ser disponibilizado somente um tempo depois do lançamento da distribuição.</span><span class="sxs-lookup"><span data-stu-id="cc62f-141">Sometimes it may be a while after a distribution is released before there's an Azure CLI package available for it.</span></span> <span data-ttu-id="cc62f-142">A CLI do Azure é projetada para ser resiliente em relação a versões futuras das dependências e precisam da menor quantidade possível delas.</span><span class="sxs-lookup"><span data-stu-id="cc62f-142">The Azure CLI designed to be resilient with regards to future versions of dependencies and rely on as few of them as possible.</span></span> <span data-ttu-id="cc62f-143">Se não houver pacotes disponíveis para sua distribuição de base, tente um pacote de uma distribuição anterior.</span><span class="sxs-lookup"><span data-stu-id="cc62f-143">If there's no package available for your base distribution, try a package for an earlier distribution.</span></span>

<span data-ttu-id="cc62f-144">Para isso, defina o valor de `AZ_REPO` manualmente ao [adicionar o repositório](#set-release).</span><span class="sxs-lookup"><span data-stu-id="cc62f-144">To do this, set the value of `AZ_REPO` manually when [adding the repository](#set-release).</span></span> <span data-ttu-id="cc62f-145">Para as distribuições do Ubuntu, use o repositório `bionic`; para as distribuições do Debian, use `stretch`.</span><span class="sxs-lookup"><span data-stu-id="cc62f-145">For Ubuntu distributions use the `bionic` repository, and for Debian distributions use `stretch`.</span></span> <span data-ttu-id="cc62f-146">Não há suporte para as distribuições lançadas antes do Ubuntu Trusty e do Debian Wheezy.</span><span class="sxs-lookup"><span data-stu-id="cc62f-146">Distributions released before Ubuntu Trusty and Debian Wheezy are not supported.</span></span>

### <a name="elementary-os-eos-fails-to-install-the-azure-cli"></a><span data-ttu-id="cc62f-147">O EOS (SO elementar) falha ao instalar a CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="cc62f-147">Elementary OS (EOS) fails to install the Azure CLI</span></span>

<span data-ttu-id="cc62f-148">O EOS não consegue instalar a CLI do Azure porque `lsb_release` retorna `HERA`, que é o nome da versão de EOS.</span><span class="sxs-lookup"><span data-stu-id="cc62f-148">EOS fails to install the Azure cli because `lsb_release` returns `HERA`, which is the EOS release name.</span></span>  <span data-ttu-id="cc62f-149">A solução é corrigir o arquivo `/etc/apt/sources.list.d/azure-cli.list` e alterar `hera main` para `bionic main`.</span><span class="sxs-lookup"><span data-stu-id="cc62f-149">The solution is to fix the file `/etc/apt/sources.list.d/azure-cli.list` and change `hera main` to `bionic main`.</span></span>

<span data-ttu-id="cc62f-150">Conteúdo do arquivo original:</span><span class="sxs-lookup"><span data-stu-id="cc62f-150">Original file contents:</span></span>

```
deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ hera main
```

<span data-ttu-id="cc62f-151">Conteúdo do arquivo modificado</span><span class="sxs-lookup"><span data-stu-id="cc62f-151">Modified file contents</span></span>

```
deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ bionic main
```

### <a name="proxy-blocks-connection"></a><span data-ttu-id="cc62f-152">Conexão de blocos de proxy</span><span class="sxs-lookup"><span data-stu-id="cc62f-152">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](includes/configure-proxy.md)]

<span data-ttu-id="cc62f-153">Talvez você queira configurar explicitamente `apt` para usar esse proxy sempre.</span><span class="sxs-lookup"><span data-stu-id="cc62f-153">You may also want to explicitly configure `apt` to use this proxy at all times.</span></span> <span data-ttu-id="cc62f-154">Verifique se as linhas a seguir aparecem em um arquivo de configuração `apt` em `/etc/apt/apt.conf.d/`.</span><span class="sxs-lookup"><span data-stu-id="cc62f-154">Make sure that the following lines appear in an `apt` configuration file in `/etc/apt/apt.conf.d/`.</span></span> <span data-ttu-id="cc62f-155">É recomendável usar o arquivo de configuração global existente, um arquivo de configuração de proxy existente, `40proxies` ou `99local`. No entanto, siga os requisitos de administração do sistema.</span><span class="sxs-lookup"><span data-stu-id="cc62f-155">We recommend using either your existing global configuration file, an existing proxy configuration file, `40proxies`, or `99local`, but follow your system administration requirements.</span></span>

```apt.conf
Acquire {
    http::proxy "http://[username]:[password]@[proxy]:[port]";
    https::proxy "https://[username]:[password]@[proxy]:[port]";
}
```

<span data-ttu-id="cc62f-156">Se o proxy não usar autenticação básica, __remova__ a parte `[username]:[password]@` do URI do proxy.</span><span class="sxs-lookup"><span data-stu-id="cc62f-156">If your proxy does not use basic auth, __remove__ the `[username]:[password]@` portion of the proxy URI.</span></span> <span data-ttu-id="cc62f-157">Se você precisar de mais informações sobre a configuração do proxy, confira a documentação oficial do Ubuntu:</span><span class="sxs-lookup"><span data-stu-id="cc62f-157">If you require more information for proxy configuration, see the official Ubuntu documentation:</span></span>

* [<span data-ttu-id="cc62f-158">apt.conf manpage</span><span class="sxs-lookup"><span data-stu-id="cc62f-158">apt.conf manpage</span></span>](http://manpages.ubuntu.com/manpages/bionic/en/man5/apt.conf.5.html)
* [<span data-ttu-id="cc62f-159">Wiki do Ubuntu – apt-get howto</span><span class="sxs-lookup"><span data-stu-id="cc62f-159">Ubuntu wiki - apt-get howto</span></span>](https://help.ubuntu.com/community/AptGet/Howto#Setting_up_apt-get_to_use_a_http-proxy)

<span data-ttu-id="cc62f-160">Para obter a chave de assinatura da Microsoft e o pacote do nosso repositório, o proxy precisa permitir conexões HTTPS com o seguinte endereço:</span><span class="sxs-lookup"><span data-stu-id="cc62f-160">In order to get the Microsoft signing key and get the package from our repository, your proxy needs to allow HTTPS connections to the following address:</span></span>

* `https://packages.microsoft.com`

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="cc62f-161">Atualizar</span><span class="sxs-lookup"><span data-stu-id="cc62f-161">Update</span></span>
[!INCLUDE [az-upgrade](includes/az-upgrade.md)]

<span data-ttu-id="cc62f-162">Você também pode usar `apt-get upgrade` para atualizar o pacote da CLI.</span><span class="sxs-lookup"><span data-stu-id="cc62f-162">You can also use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="cc62f-163">Esse comando atualiza todos os pacotes instalados no sistema que não tiveram uma alteração de dependência.</span><span class="sxs-lookup"><span data-stu-id="cc62f-163">This command upgrades all of the installed packages on your system that have not had a dependency change.</span></span>
> <span data-ttu-id="cc62f-164">Para atualizar apenas a CLI, use `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="cc62f-164">To upgrade the CLI only, use `apt-get install`.</span></span>
>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a><span data-ttu-id="cc62f-165">Desinstalar</span><span class="sxs-lookup"><span data-stu-id="cc62f-165">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="cc62f-166">Desinstalar com `apt-get remove`:</span><span class="sxs-lookup"><span data-stu-id="cc62f-166">Uninstall with `apt-get remove`:</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="cc62f-167">Se você não pretender reinstalar a CLI, remova as informações do repositório da CLI do Azure:</span><span class="sxs-lookup"><span data-stu-id="cc62f-167">If you don't plan to reinstall the CLI, remove the Azure CLI repository information:</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="cc62f-168">Se você não usa nenhum outro pacote da Microsoft, remova a chave de assinatura:</span><span class="sxs-lookup"><span data-stu-id="cc62f-168">If you use no other packages from Microsoft, remove the signing key:</span></span>

    ```bash
    sudo rm /etc/apt/trusted.gpg.d/microsoft.gpg
    ```

4. <span data-ttu-id="cc62f-169">Remova quaisquer pacotes desnecessários:</span><span class="sxs-lookup"><span data-stu-id="cc62f-169">Remove any unneeded packages:</span></span>

   ```bash
   sudo apt autoremove
   ```

## <a name="next-steps"></a><span data-ttu-id="cc62f-170">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="cc62f-170">Next Steps</span></span>

<span data-ttu-id="cc62f-171">Agora que você instalou a CLI do Azure, faça um tour breve de seus recursos e comandos comuns.</span><span class="sxs-lookup"><span data-stu-id="cc62f-171">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="cc62f-172">Introdução à CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="cc62f-172">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
