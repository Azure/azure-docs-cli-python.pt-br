---
title: Instalar a CLI do Azure no Linux com apt
description: Como instalar a CLI do Azure com o gerenciador de pacotes apt
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 10/14/2019
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 5e665fb9318f505a5097f6daf4f3020201306679
ms.sourcegitcommit: bf84dfb62e910ea246586481863bb43d09d07795
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/04/2020
ms.locfileid: "87551193"
---
# <a name="install-azure-cli-with-apt"></a><span data-ttu-id="24fc9-103">Instalar CLI do Azure com o apt</span><span class="sxs-lookup"><span data-stu-id="24fc9-103">Install Azure CLI with apt</span></span>

<span data-ttu-id="24fc9-104">Se você estiver executando uma distribuição fornecida com `apt`, como Ubuntu ou Debian, há um pacote x86_64 disponível para a CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="24fc9-104">If you are running a distribution that comes with `apt`, such as Ubuntu or Debian, there's an x86_64 package available for the Azure CLI.</span></span> <span data-ttu-id="24fc9-105">Este pacote foi testado e é compatível com:</span><span class="sxs-lookup"><span data-stu-id="24fc9-105">This package has been tested with and is supported for:</span></span>

* <span data-ttu-id="24fc9-106">Ubuntu trusty, xenial, artful, bionic e disco</span><span class="sxs-lookup"><span data-stu-id="24fc9-106">Ubuntu trusty, xenial, artful, bionic, and disco</span></span>
* <span data-ttu-id="24fc9-107">Debian wheezy, jessie, stretch e buster</span><span class="sxs-lookup"><span data-stu-id="24fc9-107">Debian wheezy, jessie, stretch, and buster</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

> [!NOTE]
>
> <span data-ttu-id="24fc9-108">O pacote para a CLI do Azure instala seu próprio interpretador de Python e não usa o Python do sistema.</span><span class="sxs-lookup"><span data-stu-id="24fc9-108">The package for Azure CLI installs its own Python interpreter, and does not use the system Python.</span></span>

## <a name="install"></a><span data-ttu-id="24fc9-109">Instalar</span><span class="sxs-lookup"><span data-stu-id="24fc9-109">Install</span></span>

<span data-ttu-id="24fc9-110">Oferecemos duas maneiras de instalar a CLI do Azure com distribuições que dão suporte a `apt`: Como um script tudo-em-um que executa os comandos de instalação para você, e instruções que podem ser executadas como um processo passo a passo por conta própria.</span><span class="sxs-lookup"><span data-stu-id="24fc9-110">We offer two ways to install the Azure CLI with distributions that support `apt`: As an all-in-one script that runs the install commands for you, and instructions that you can run as a step-by-step process on your own.</span></span>

### <a name="install-with-one-command"></a><span data-ttu-id="24fc9-111">Instalar com um comando</span><span class="sxs-lookup"><span data-stu-id="24fc9-111">Install with one command</span></span>

<span data-ttu-id="24fc9-112">Oferecemos e mantemos um script que executa todos os comandos de instalação em uma única etapa.</span><span class="sxs-lookup"><span data-stu-id="24fc9-112">We offer and maintain a script which runs all of the installation commands in one step.</span></span> <span data-ttu-id="24fc9-113">Executá-lo usando `curl` e redirecione diretamente para `bash`, ou baixe o script para um arquivo e inspecione-o antes da execução.</span><span class="sxs-lookup"><span data-stu-id="24fc9-113">Run it by using `curl` and pipe directly to `bash`, or download the script to a file and inspect it before running.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="24fc9-114">Esse script é verificado somente para o Ubuntu 16.04+ e Debian 8+.</span><span class="sxs-lookup"><span data-stu-id="24fc9-114">This script is only verified for Ubuntu 16.04+ and Debian 8+.</span></span> <span data-ttu-id="24fc9-115">Ele pode não funcionar em outras distribuições.</span><span class="sxs-lookup"><span data-stu-id="24fc9-115">It may not work on other distributions.</span></span>
> <span data-ttu-id="24fc9-116">Se você estiver usando uma distribuição derivada como Linux Mint, siga as instruções de instalação manual e execute qualquer solução de problemas necessária.</span><span class="sxs-lookup"><span data-stu-id="24fc9-116">If you're using a derived distribution such as Linux Mint, follow the manual install instructions and perform any necessary troubleshooting.</span></span>

```bash
curl -sL https://aka.ms/InstallAzureCLIDeb | sudo bash
```

### <a name="manual-install-instructions"></a><span data-ttu-id="24fc9-117">Instruções para instalação manual</span><span class="sxs-lookup"><span data-stu-id="24fc9-117">Manual install instructions</span></span>

<span data-ttu-id="24fc9-118">Se você não quiser executar um script como superusuário ou se o script tudo-em-um falhar, siga estas etapas para instalar a CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="24fc9-118">If you don't want to run a script as superuser or the all-in-one script fails, follow these steps to install the Azure CLI.</span></span>

1. <span data-ttu-id="24fc9-119">Obtenha os pacotes necessários para o processo de instalação:</span><span class="sxs-lookup"><span data-stu-id="24fc9-119">Get packages needed for the install process:</span></span>

    ```bash
    sudo apt-get update
    sudo apt-get install ca-certificates curl apt-transport-https lsb-release gnupg
    ```

2. <span data-ttu-id="24fc9-120">Baixe e instale a chave de autenticação da Microsoft:</span><span class="sxs-lookup"><span data-stu-id="24fc9-120">Download and install the Microsoft signing key:</span></span>

    ```bash
    curl -sL https://packages.microsoft.com/keys/microsoft.asc |
        gpg --dearmor |
        sudo tee /etc/apt/trusted.gpg.d/microsoft.gpg > /dev/null
    ```

3. <div id="set-release"/><span data-ttu-id="24fc9-121">Adicione o repositório de software da CLI do Azure:</span><span class="sxs-lookup"><span data-stu-id="24fc9-121">Add the Azure CLI software repository:</span></span>

    ```bash
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" |
        sudo tee /etc/apt/sources.list.d/azure-cli.list
    ```

4. <span data-ttu-id="24fc9-122">Atualize as informações do repositório e instale o pacote `azure-cli`:</span><span class="sxs-lookup"><span data-stu-id="24fc9-122">Update repository information and install the `azure-cli` package:</span></span>

    ```bash
    sudo apt-get update
    sudo apt-get install azure-cli
    ```

<span data-ttu-id="24fc9-123">Execute a CLI do Azure com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="24fc9-123">Run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="24fc9-124">Para entrar, use o comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="24fc9-124">To sign in, use the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="24fc9-125">Para saber mais sobre os diferentes métodos de autenticação, confira [Entrar com a CLI do Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="24fc9-125">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="24fc9-126">Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="24fc9-126">Troubleshooting</span></span>

<span data-ttu-id="24fc9-127">Aqui estão alguns problemas comuns vistos durante a instalação com `apt`.</span><span class="sxs-lookup"><span data-stu-id="24fc9-127">Here are some common problems seen when installing with `apt`.</span></span> <span data-ttu-id="24fc9-128">Se você tiver um problema não abordado aqui, [arquive um problema no github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="24fc9-128">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="lsb_release-does-not-return-the-correct-base-distribution-version"></a><span data-ttu-id="24fc9-129">lsb_release não retorna a versão correta da distribuição de base</span><span class="sxs-lookup"><span data-stu-id="24fc9-129">lsb_release does not return the correct base distribution version</span></span>

<span data-ttu-id="24fc9-130">Algumas distribuições derivadas do Ubuntu ou do Debian, como o Linux Mint, podem não retornar o nome correto da versão de `lsb_release`.</span><span class="sxs-lookup"><span data-stu-id="24fc9-130">Some Ubuntu- or Debian-derived distributions such as Linux Mint may not return the correct version name from `lsb_release`.</span></span> <span data-ttu-id="24fc9-131">Esse valor é usado no processo de instalação para determinar o pacote de instalação.</span><span class="sxs-lookup"><span data-stu-id="24fc9-131">This value is used in the install process to determine the package to install.</span></span> <span data-ttu-id="24fc9-132">Se você souber o nome do código da versão do Ubuntu ou do Debian da qual sua distribuição é derivada, poderá definir o valor de `AZ_REPO` manualmente ao [adicionar o repositório](#set-release).</span><span class="sxs-lookup"><span data-stu-id="24fc9-132">If you know the code name of the Ubuntu or Debian version your distribution is derived from, you can set the `AZ_REPO` value manually when [adding the repository](#set-release).</span></span> <span data-ttu-id="24fc9-133">Caso contrário, procure informações para sua distribuição sobre como determinar o nome do código da distribuição de base e defina `AZ_REPO` com o valor correto.</span><span class="sxs-lookup"><span data-stu-id="24fc9-133">Otherwise, look up information for your distribution on how to determine the base distribution code name and set `AZ_REPO` to the correct value.</span></span>

### <a name="no-package-for-your-distribution"></a><span data-ttu-id="24fc9-134">Nenhum pacote para distribuição</span><span class="sxs-lookup"><span data-stu-id="24fc9-134">No package for your distribution</span></span>

<span data-ttu-id="24fc9-135">Às vezes, um pacote da CLI do Azure pode ser disponibilizado somente um tempo depois do lançamento da distribuição.</span><span class="sxs-lookup"><span data-stu-id="24fc9-135">Sometimes it may be a while after a distribution is released before there's an Azure CLI package available for it.</span></span> <span data-ttu-id="24fc9-136">A CLI do Azure é projetada para ser resiliente em relação a versões futuras das dependências e precisam da menor quantidade possível delas.</span><span class="sxs-lookup"><span data-stu-id="24fc9-136">The Azure CLI designed to be resilient with regards to future versions of dependencies and rely on as few of them as possible.</span></span> <span data-ttu-id="24fc9-137">Se não houver pacotes disponíveis para sua distribuição de base, tente um pacote de uma distribuição anterior.</span><span class="sxs-lookup"><span data-stu-id="24fc9-137">If there's no package available for your base distribution, try a package for an earlier distribution.</span></span>

<span data-ttu-id="24fc9-138">Para isso, defina o valor de `AZ_REPO` manualmente ao [adicionar o repositório](#set-release).</span><span class="sxs-lookup"><span data-stu-id="24fc9-138">To do this, set the value of `AZ_REPO` manually when [adding the repository](#set-release).</span></span> <span data-ttu-id="24fc9-139">Para as distribuições do Ubuntu, use o repositório `bionic`; para as distribuições do Debian, use `stretch`.</span><span class="sxs-lookup"><span data-stu-id="24fc9-139">For Ubuntu distributions use the `bionic` repository, and for Debian distributions use `stretch`.</span></span> <span data-ttu-id="24fc9-140">Não há suporte para as distribuições lançadas antes do Ubuntu Trusty e do Debian Wheezy.</span><span class="sxs-lookup"><span data-stu-id="24fc9-140">Distributions released before Ubuntu Trusty and Debian Wheezy are not supported.</span></span>

### <a name="elementary-os-eos-fails-to-install-the-azure-cli"></a><span data-ttu-id="24fc9-141">O EOS (SO elementar) falha ao instalar a CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="24fc9-141">Elementary OS (EOS) fails to install the Azure CLI</span></span>

<span data-ttu-id="24fc9-142">O EOS não consegue instalar a CLI do Azure porque `lsb_release` retorna `HERA`, que é o nome da versão de EOS.</span><span class="sxs-lookup"><span data-stu-id="24fc9-142">EOS fails to install the Azure cli because `lsb_release` returns `HERA`, which is the EOS release name.</span></span>  <span data-ttu-id="24fc9-143">A solução é corrigir o arquivo `/etc/apt/sources.list.d/azure-cli.list` e alterar `hera main` para `bionic main`.</span><span class="sxs-lookup"><span data-stu-id="24fc9-143">The solution is to fix the file `/etc/apt/sources.list.d/azure-cli.list` and change `hera main` to `bionic main`.</span></span>

<span data-ttu-id="24fc9-144">Conteúdo do arquivo original:</span><span class="sxs-lookup"><span data-stu-id="24fc9-144">Original file contents:</span></span>

```
deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ hera main
```

<span data-ttu-id="24fc9-145">Conteúdo do arquivo modificado</span><span class="sxs-lookup"><span data-stu-id="24fc9-145">Modified file contents</span></span>

```
deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ bionic main
```

### <a name="proxy-blocks-connection"></a><span data-ttu-id="24fc9-146">Conexão de blocos de proxy</span><span class="sxs-lookup"><span data-stu-id="24fc9-146">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](includes/configure-proxy.md)]

<span data-ttu-id="24fc9-147">Talvez você queira configurar explicitamente `apt` para usar esse proxy sempre.</span><span class="sxs-lookup"><span data-stu-id="24fc9-147">You may also want to explicitly configure `apt` to use this proxy at all times.</span></span> <span data-ttu-id="24fc9-148">Verifique se as linhas a seguir aparecem em um arquivo de configuração `apt` em `/etc/apt/apt.conf.d/`.</span><span class="sxs-lookup"><span data-stu-id="24fc9-148">Make sure that the following lines appear in an `apt` configuration file in `/etc/apt/apt.conf.d/`.</span></span> <span data-ttu-id="24fc9-149">É recomendável usar o arquivo de configuração global existente, um arquivo de configuração de proxy existente, `40proxies` ou `99local`. No entanto, siga os requisitos de administração do sistema.</span><span class="sxs-lookup"><span data-stu-id="24fc9-149">We recommend using either your existing global configuration file, an existing proxy configuration file, `40proxies`, or `99local`, but follow your system administration requirements.</span></span>

```apt.conf
Acquire {
    http::proxy "http://[username]:[password]@[proxy]:[port]";
    https::proxy "https://[username]:[password]@[proxy]:[port]";
}
```

<span data-ttu-id="24fc9-150">Se o proxy não usar autenticação básica, __remova__ a parte `[username]:[password]@` do URI do proxy.</span><span class="sxs-lookup"><span data-stu-id="24fc9-150">If your proxy does not use basic auth, __remove__ the `[username]:[password]@` portion of the proxy URI.</span></span> <span data-ttu-id="24fc9-151">Se você precisar de mais informações sobre a configuração do proxy, confira a documentação oficial do Ubuntu:</span><span class="sxs-lookup"><span data-stu-id="24fc9-151">If you require more information for proxy configuration, see the official Ubuntu documentation:</span></span>

* [<span data-ttu-id="24fc9-152">apt.conf manpage</span><span class="sxs-lookup"><span data-stu-id="24fc9-152">apt.conf manpage</span></span>](http://manpages.ubuntu.com/manpages/bionic/en/man5/apt.conf.5.html)
* [<span data-ttu-id="24fc9-153">Wiki do Ubuntu – apt-get howto</span><span class="sxs-lookup"><span data-stu-id="24fc9-153">Ubuntu wiki - apt-get howto</span></span>](https://help.ubuntu.com/community/AptGet/Howto#Setting_up_apt-get_to_use_a_http-proxy)

<span data-ttu-id="24fc9-154">Para obter a chave de assinatura da Microsoft e o pacote do nosso repositório, o proxy precisa permitir conexões HTTPS com o seguinte endereço:</span><span class="sxs-lookup"><span data-stu-id="24fc9-154">In order to get the Microsoft signing key and get the package from our repository, your proxy needs to allow HTTPS connections to the following address:</span></span>

* `https://packages.microsoft.com`

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="24fc9-155">Atualizar</span><span class="sxs-lookup"><span data-stu-id="24fc9-155">Update</span></span>

<span data-ttu-id="24fc9-156">Use `apt-get upgrade` para atualizar o pacote da CLI.</span><span class="sxs-lookup"><span data-stu-id="24fc9-156">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="24fc9-157">Esse comando atualiza todos os pacotes instalados no sistema que não tiveram uma alteração de dependência.</span><span class="sxs-lookup"><span data-stu-id="24fc9-157">This command upgrades all of the installed packages on your system that have not had a dependency change.</span></span>
> <span data-ttu-id="24fc9-158">Para atualizar apenas a CLI, use `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="24fc9-158">To upgrade the CLI only, use `apt-get install`.</span></span>
>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a><span data-ttu-id="24fc9-159">Desinstalar</span><span class="sxs-lookup"><span data-stu-id="24fc9-159">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="24fc9-160">Desinstalar com `apt-get remove`:</span><span class="sxs-lookup"><span data-stu-id="24fc9-160">Uninstall with `apt-get remove`:</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="24fc9-161">Se você não pretender reinstalar a CLI, remova as informações do repositório da CLI do Azure:</span><span class="sxs-lookup"><span data-stu-id="24fc9-161">If you don't plan to reinstall the CLI, remove the Azure CLI repository information:</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="24fc9-162">Se você não usa nenhum outro pacote da Microsoft, remova a chave de assinatura:</span><span class="sxs-lookup"><span data-stu-id="24fc9-162">If you use no other packages from Microsoft, remove the signing key:</span></span>

    ```bash
    sudo rm /etc/apt/trusted.gpg.d/microsoft.gpg
    ```

4. <span data-ttu-id="24fc9-163">Remova quaisquer pacotes desnecessários:</span><span class="sxs-lookup"><span data-stu-id="24fc9-163">Remove any unneeded packages:</span></span>

   ```bash
   sudo apt autoremove
   ```

## <a name="next-steps"></a><span data-ttu-id="24fc9-164">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="24fc9-164">Next Steps</span></span>

<span data-ttu-id="24fc9-165">Agora que você instalou a CLI do Azure, faça um tour breve de seus recursos e comandos comuns.</span><span class="sxs-lookup"><span data-stu-id="24fc9-165">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="24fc9-166">Introdução à CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="24fc9-166">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
