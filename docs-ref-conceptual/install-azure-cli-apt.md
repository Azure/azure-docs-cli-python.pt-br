---
title: Instalar a CLI do Azure no Linux com apt
description: Como instalar a CLI do Azure com o gerenciador de pacotes apt
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/27/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 1973c933cbffa494cbe9c0749346450251feefcb
ms.sourcegitcommit: 9bd90875a324908ec7195fc4c4f63ebf124760f9
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/02/2019
ms.locfileid: "53982579"
---
# <a name="install-azure-cli-with-apt"></a><span data-ttu-id="ea02f-103">Instalar CLI do Azure com o apt</span><span class="sxs-lookup"><span data-stu-id="ea02f-103">Install Azure CLI with apt</span></span>

<span data-ttu-id="ea02f-104">Se você estiver executando uma distribuição que vem com `apt`, como o Ubuntu ou o Debian, haverá um pacote de 64 bits disponível para a CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="ea02f-104">If you are running a distribution that comes with `apt`, such as Ubuntu or Debian, there's a 64-bit package available for the Azure CLI.</span></span> <span data-ttu-id="ea02f-105">Esse pacote foi testado com:</span><span class="sxs-lookup"><span data-stu-id="ea02f-105">This package has been tested with:</span></span>

* <span data-ttu-id="ea02f-106">Ubuntu trusty, xenial, artful e bionic</span><span class="sxs-lookup"><span data-stu-id="ea02f-106">Ubuntu trusty, xenial, artful, and bionic</span></span>
* <span data-ttu-id="ea02f-107">Debian wheezy, jessie e stretch</span><span class="sxs-lookup"><span data-stu-id="ea02f-107">Debian wheezy, jessie, and stretch</span></span>

## <a name="install"></a><span data-ttu-id="ea02f-108">Instalar</span><span class="sxs-lookup"><span data-stu-id="ea02f-108">Install</span></span>

1. <span data-ttu-id="ea02f-109">Instale os pacotes de pré-requisito:</span><span class="sxs-lookup"><span data-stu-id="ea02f-109">Install prerequisite packages:</span></span>

    ```bash
    sudo apt-get install apt-transport-https lsb-release software-properties-common dirmngr -y
    ```

2. <div id="set-release"/><span data-ttu-id="ea02f-110">Modifique sua lista de fontes:</span><span class="sxs-lookup"><span data-stu-id="ea02f-110">Modify your sources list:</span></span>

    ```bash
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
    ```

3. <div id="signingKey"/><span data-ttu-id="ea02f-111">Obtenha a chave de assinatura da Microsoft:</span><span class="sxs-lookup"><span data-stu-id="ea02f-111">Get the Microsoft signing key:</span></span>

   ```bash
   sudo apt-key --keyring /etc/apt/trusted.gpg.d/Microsoft.gpg adv \
        --keyserver packages.microsoft.com \
        --recv-keys BC528686B50D79E339D3721CEB3E94ADBE1229CF
   ```

4. <span data-ttu-id="ea02f-112">Instalar a CLI:</span><span class="sxs-lookup"><span data-stu-id="ea02f-112">Install the CLI:</span></span>

   ```bash
   sudo apt-get update
   sudo apt-get install azure-cli
   ```

   > [!WARNING]
   > <span data-ttu-id="ea02f-113">A chave de assinatura foi atualizada em maio de 2018 e foi substituída.</span><span class="sxs-lookup"><span data-stu-id="ea02f-113">The signing key was updated in May 2018, and has been replaced.</span></span> <span data-ttu-id="ea02f-114">Se você receber erros de autenticação, verifique se tem [a chave de autenticação mais recente](#signingKey).</span><span class="sxs-lookup"><span data-stu-id="ea02f-114">If you receive signing errors, make sure you have [the latest signing key](#signingKey).</span></span>

<span data-ttu-id="ea02f-115">É possível executar a CLI do Azure com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="ea02f-115">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="ea02f-116">Para entrar, use o comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="ea02f-116">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="ea02f-117">Para saber mais sobre os diferentes métodos de autenticação, confira [Entrar com a CLI do Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="ea02f-117">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="ea02f-118">solução de problemas</span><span class="sxs-lookup"><span data-stu-id="ea02f-118">Troubleshooting</span></span>

<span data-ttu-id="ea02f-119">Aqui estão alguns problemas comuns vistos durante a instalação com `apt`.</span><span class="sxs-lookup"><span data-stu-id="ea02f-119">Here are some common problems seen when installing with `apt`.</span></span> <span data-ttu-id="ea02f-120">Se você tiver um problema não abordado aqui, [arquive um problema no github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="ea02f-120">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="lsbrelease-does-not-return-the-correct-base-distribution-version"></a><span data-ttu-id="ea02f-121">lsb_release não retorna a versão correta da distribuição de base</span><span class="sxs-lookup"><span data-stu-id="ea02f-121">lsb_release does not return the correct base distribution version</span></span>

<span data-ttu-id="ea02f-122">Algumas distribuições derivadas do Ubuntu ou do Debian, como o Linux Mint, podem não retornar o nome correto da versão de `lsb_release`.</span><span class="sxs-lookup"><span data-stu-id="ea02f-122">Some Ubuntu- or Debian-derived distributions such as Linux Mint may not return the correct version name from `lsb_release`.</span></span> <span data-ttu-id="ea02f-123">Esse valor é usado no processo de instalação para determinar o pacote de instalação.</span><span class="sxs-lookup"><span data-stu-id="ea02f-123">This value is used in the install process to determine the package to install.</span></span> <span data-ttu-id="ea02f-124">Se você souber o nome da versão da qual sua distribuição é derivada, poderá definir o `AZ_REPO` valor manualmente em [instalar etapa 2](#set-release).</span><span class="sxs-lookup"><span data-stu-id="ea02f-124">If you know the name of the version your distribution is derived from, you can set the `AZ_REPO` value manually in [install step 2](#set-release).</span></span> <span data-ttu-id="ea02f-125">Caso contrário, procure informações para sua distribuição sobre como determinar o nome da distribuição de base e defina `AZ_REPO` para o valor correto.</span><span class="sxs-lookup"><span data-stu-id="ea02f-125">Otherwise, look up information for your distribution on how to determine the base distribution name and set `AZ_REPO` to the correct value.</span></span>

### <a name="no-package-for-your-distribution"></a><span data-ttu-id="ea02f-126">Nenhum pacote para distribuição</span><span class="sxs-lookup"><span data-stu-id="ea02f-126">No package for your distribution</span></span>

<span data-ttu-id="ea02f-127">Às vezes, um pacote da CLI do Azure pode ficar disponível somente um tempo depois de uma distribuição do Ubuntu ser lançada.</span><span class="sxs-lookup"><span data-stu-id="ea02f-127">Sometimes it may be a while after an Ubuntu distribution is released before there's an Azure CLI package made available for it.</span></span> <span data-ttu-id="ea02f-128">A CLI do Azure é projetada para ser resiliente em relação a versões futuras das dependências e precisam da menor quantidade possível delas.</span><span class="sxs-lookup"><span data-stu-id="ea02f-128">The Azure CLI designed to be resilient with regards to future versions of dependencies and rely on as few of them as possible.</span></span> <span data-ttu-id="ea02f-129">Se não houver pacotes disponíveis para sua distribuição de base, tente um pacote de uma distribuição anterior.</span><span class="sxs-lookup"><span data-stu-id="ea02f-129">If there's no package available for your base distribution, try a package for an earlier distribution.</span></span>

<span data-ttu-id="ea02f-130">Para isso, defina o valor `AZ_REPO` manualmente na [etapa 1 de instalação](#install-step-1).</span><span class="sxs-lookup"><span data-stu-id="ea02f-130">To do this, set the value of `AZ_REPO` manually in [install step 1](#install-step-1).</span></span> <span data-ttu-id="ea02f-131">Para as distribuições do Ubuntu, use o repositório `bionic`; para as distribuições do Debian, use `stretch`.</span><span class="sxs-lookup"><span data-stu-id="ea02f-131">For Ubuntu distributions use the `bionic` repository, and for Debian distributions use `stretch`.</span></span> <span data-ttu-id="ea02f-132">Não há suporte para as distribuições lançadas antes do Ubuntu Trusty e do Debian Wheezy.</span><span class="sxs-lookup"><span data-stu-id="ea02f-132">Distributions released before Ubuntu Trusty and Debian Wheezy are not supported.</span></span>

### <a name="apt-key-fails-with-no-dirmngr"></a><span data-ttu-id="ea02f-133">apt-key falha com “Sem dirmngr”</span><span class="sxs-lookup"><span data-stu-id="ea02f-133">apt-key fails with "No dirmngr"</span></span>

<span data-ttu-id="ea02f-134">Ao executar o comando `apt-key`, pode ser que você veja uma saída semelhante ao seguinte erro:</span><span class="sxs-lookup"><span data-stu-id="ea02f-134">When running the `apt-key` command, you may see output similar to the following error:</span></span>

```output
gpg: failed to start the dirmngr '/usr/bin/dirmngr': No such file or directory
gpg: connecting dirmngr at '/tmp/apt-key-gpghome.kt5zo27tp1/S.dirmngr' failed: No such file or directory
gpg: keyserver receive failed: No dirmngr
```

<span data-ttu-id="ea02f-135">O erro ocorre devido a um componente ausente requerido por `apt-key`.</span><span class="sxs-lookup"><span data-stu-id="ea02f-135">The error is due to a missing component required by `apt-key`.</span></span> <span data-ttu-id="ea02f-136">Você pode resolver isso instalando o pacote `dirmngr`.</span><span class="sxs-lookup"><span data-stu-id="ea02f-136">You can resolve it by installing the `dirmngr` package.</span></span>

```bash
sudo apt-get install dirmngr
```

<span data-ttu-id="ea02f-137">Se você estiver usando o subsistema do Windows para Linux (WSL), esse erro também aparece nas versões do Windows anteriores ao Windows 10 1809.</span><span class="sxs-lookup"><span data-stu-id="ea02f-137">If you are on Windows Subsystem for Linux (WSL), this error also appears on versions of Windows prior to Windows 10 1809.</span></span> <span data-ttu-id="ea02f-138">Para resolver o problema, atualize sua versão do Windows.</span><span class="sxs-lookup"><span data-stu-id="ea02f-138">To resolve the issue, update your version of Windows.</span></span>

### <a name="apt-key-hangs"></a><span data-ttu-id="ea02f-139">apt-key trava</span><span class="sxs-lookup"><span data-stu-id="ea02f-139">apt-key hangs</span></span>

<span data-ttu-id="ea02f-140">Quando atrás de um firewall que bloqueia as conexões de saída para a porta 11371, o comando `apt-key` pode travar indefinidamente.</span><span class="sxs-lookup"><span data-stu-id="ea02f-140">When behind a firewall blocking outgoing connections to port 11371, the `apt-key` command might hang indefinitely.</span></span>
<span data-ttu-id="ea02f-141">O firewall pode exigir um proxy HTTP para as conexões de saída:</span><span class="sxs-lookup"><span data-stu-id="ea02f-141">Your firewall may require an HTTP proxy for outgoing connections:</span></span>

```bash
sudo apt-key --keyring /etc/apt/trusted.gpg.d/Microsoft.gpg adv \
    --keyserver-options http-proxy=http://<USER>:<PASSWORD>@<PROXY-HOST>:<PROXY-PORT>/ \
    --keyserver packages.microsoft.com \
    --recv-keys BC528686B50D79E339D3721CEB3E94ADBE1229CF
```

<span data-ttu-id="ea02f-142">Para determinar se você tem um proxy, entre em contato com o administrador do sistema.</span><span class="sxs-lookup"><span data-stu-id="ea02f-142">To determine if you have a proxy, contact your system administrator.</span></span> <span data-ttu-id="ea02f-143">Se o proxy não precisar de logon, omita as informações sobre usuário e senha.</span><span class="sxs-lookup"><span data-stu-id="ea02f-143">If your proxy does not require a login, then leave out the user and password information.</span></span>

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="ea02f-144">Atualizar</span><span class="sxs-lookup"><span data-stu-id="ea02f-144">Update</span></span>

<span data-ttu-id="ea02f-145">Use `apt-get upgrade` para atualizar o pacote da CLI.</span><span class="sxs-lookup"><span data-stu-id="ea02f-145">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!WARNING]
> <span data-ttu-id="ea02f-146">A chave de assinatura foi atualizada em maio de 2018 e foi substituída.</span><span class="sxs-lookup"><span data-stu-id="ea02f-146">The signing key was updated in May 2018, and has been replaced.</span></span> <span data-ttu-id="ea02f-147">Se você receber erros de autenticação, verifique se tem [a chave de autenticação mais recente](#signingKey).</span><span class="sxs-lookup"><span data-stu-id="ea02f-147">If you receive signing errors, make sure you have [the latest signing key](#signingKey).</span></span>
>
> [!NOTE]
> <span data-ttu-id="ea02f-148">Esse comando atualiza todos os pacotes instalados no sistema que não tiveram uma alteração de dependência.</span><span class="sxs-lookup"><span data-stu-id="ea02f-148">This command upgrades all of the installed packages on your system that have not had a dependency change.</span></span>
> <span data-ttu-id="ea02f-149">Para atualizar apenas a CLI, use `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="ea02f-149">To upgrade the CLI only, use `apt-get install`.</span></span>
> 
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a><span data-ttu-id="ea02f-150">Desinstalar</span><span class="sxs-lookup"><span data-stu-id="ea02f-150">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="ea02f-151">Desinstalar com `apt-get remove`:</span><span class="sxs-lookup"><span data-stu-id="ea02f-151">Uninstall with `apt-get remove`:</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="ea02f-152">Se você não pretender reinstalar a CLI, remova as informações do repositório da CLI do Azure:</span><span class="sxs-lookup"><span data-stu-id="ea02f-152">If you don't plan to reinstall the CLI, remove the Azure CLI repository information:</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="ea02f-153">Remova a chave de autenticação:</span><span class="sxs-lookup"><span data-stu-id="ea02f-153">Remove the signing key:</span></span>

    ```bash
    sudo rm /etc/apt/trusted.gpg.d/Microsoft.gpg
    ```

4. <span data-ttu-id="ea02f-154">Remova quaisquer pacotes desnecessários:</span><span class="sxs-lookup"><span data-stu-id="ea02f-154">Remove any unneeded packages:</span></span>

   ```bash
   sudo apt autoremove
   ```

## <a name="next-steps"></a><span data-ttu-id="ea02f-155">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="ea02f-155">Next Steps</span></span>

<span data-ttu-id="ea02f-156">Agora que você instalou a CLI do Azure, faça um tour breve de seus recursos e comandos comuns.</span><span class="sxs-lookup"><span data-stu-id="ea02f-156">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="ea02f-157">Introdução à CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="ea02f-157">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
