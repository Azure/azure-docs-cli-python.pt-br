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
ms.devlang: azure-cli
ms.openlocfilehash: c33c3e75991979a72a7b82183dd88b87715907ae
ms.sourcegitcommit: a8aac038e6ede0b1b352ca6163a04b61ff4eed5b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/28/2018
ms.locfileid: "52450251"
---
# <a name="install-azure-cli-with-apt"></a><span data-ttu-id="4bcb1-103">Instalar CLI do Azure com o apt</span><span class="sxs-lookup"><span data-stu-id="4bcb1-103">Install Azure CLI with apt</span></span>

<span data-ttu-id="4bcb1-104">Se você estiver executando uma distribuição que vem com `apt`, como o Ubuntu ou o Debian, haverá um pacote de 64 bits disponível para a CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="4bcb1-104">If you are running a distribution that comes with `apt`, such as Ubuntu or Debian, there's a 64-bit package available for the Azure CLI.</span></span> <span data-ttu-id="4bcb1-105">Esse pacote foi testado com:</span><span class="sxs-lookup"><span data-stu-id="4bcb1-105">This package has been tested with:</span></span>

* <span data-ttu-id="4bcb1-106">Ubuntu trusty, xenial, artful e bionic</span><span class="sxs-lookup"><span data-stu-id="4bcb1-106">Ubuntu trusty, xenial, artful, and bionic</span></span>
* <span data-ttu-id="4bcb1-107">Debian wheezy, jessie e stretch</span><span class="sxs-lookup"><span data-stu-id="4bcb1-107">Debian wheezy, jessie, and stretch</span></span>

## <a name="install"></a><span data-ttu-id="4bcb1-108">Instalar</span><span class="sxs-lookup"><span data-stu-id="4bcb1-108">Install</span></span>

1. <div id="install-step-1"/><span data-ttu-id="4bcb1-109">Modifique sua lista de fontes:</span><span class="sxs-lookup"><span data-stu-id="4bcb1-109">Modify your sources list:</span></span>

    ```bash
    sudo apt-get install apt-transport-https lsb-release software-properties-common -y
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
    ```

2. <div id="signingKey"/><span data-ttu-id="4bcb1-110">Obtenha a chave de assinatura da Microsoft:</span><span class="sxs-lookup"><span data-stu-id="4bcb1-110">Get the Microsoft signing key:</span></span>

   ```bash
   sudo apt-key --keyring /etc/apt/trusted.gpg.d/Microsoft.gpg adv \
        --keyserver packages.microsoft.com \
        --recv-keys BC528686B50D79E339D3721CEB3E94ADBE1229CF
   ```

3. <span data-ttu-id="4bcb1-111">Instalar a CLI:</span><span class="sxs-lookup"><span data-stu-id="4bcb1-111">Install the CLI:</span></span>

   ```bash
   sudo apt-get update
   sudo apt-get install azure-cli
   ```

   > [!WARNING]
   > <span data-ttu-id="4bcb1-112">A chave de assinatura foi atualizada em maio de 2018 e foi substituída.</span><span class="sxs-lookup"><span data-stu-id="4bcb1-112">The signing key was updated in May 2018, and has been replaced.</span></span> <span data-ttu-id="4bcb1-113">Se você receber erros de autenticação, verifique se tem [a chave de autenticação mais recente](#signingKey).</span><span class="sxs-lookup"><span data-stu-id="4bcb1-113">If you receive signing errors, make sure you have [the latest signing key](#signingKey).</span></span>

<span data-ttu-id="4bcb1-114">É possível executar a CLI do Azure com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="4bcb1-114">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="4bcb1-115">Para entrar, use o comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="4bcb1-115">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="4bcb1-116">Para saber mais sobre os diferentes métodos de autenticação, confira [Entrar com a CLI do Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="4bcb1-116">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="4bcb1-117">solução de problemas</span><span class="sxs-lookup"><span data-stu-id="4bcb1-117">Troubleshooting</span></span>

<span data-ttu-id="4bcb1-118">Aqui estão alguns problemas comuns vistos durante a instalação com `apt`.</span><span class="sxs-lookup"><span data-stu-id="4bcb1-118">Here are some common problems seen when installing with `apt`.</span></span> <span data-ttu-id="4bcb1-119">Se você tiver um problema não abordado aqui, [arquive um problema no github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="4bcb1-119">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="lsbrelease-does-not-return-the-correct-base-distribution-version"></a><span data-ttu-id="4bcb1-120">lsb_release não retorna a versão correta da distribuição de base</span><span class="sxs-lookup"><span data-stu-id="4bcb1-120">lsb_release does not return the correct base distribution version</span></span>

<span data-ttu-id="4bcb1-121">Algumas distribuições derivadas do Ubuntu ou do Debian, como o Linux Mint, podem não retornar o nome correto da versão de `lsb_release`.</span><span class="sxs-lookup"><span data-stu-id="4bcb1-121">Some Ubuntu- or Debian-derived distributions such as Linux Mint may not return the correct version name from `lsb_release`.</span></span> <span data-ttu-id="4bcb1-122">Esse valor é usado no processo de instalação para determinar o pacote de instalação.</span><span class="sxs-lookup"><span data-stu-id="4bcb1-122">This value is used in the install process to determine the package to install.</span></span> <span data-ttu-id="4bcb1-123">Se você souber o nome da versão da qual sua distribuição é derivada, poderá definir o `AZ_REPO` valor manualmente em [instalar etapa 1](#install-step-1).</span><span class="sxs-lookup"><span data-stu-id="4bcb1-123">If you know the name of the version your distribution is derived from, you can set the `AZ_REPO` value manually in [install step 1](#install-step-1).</span></span> <span data-ttu-id="4bcb1-124">Caso contrário, procure informações para sua distribuição sobre como determinar o nome da distribuição de base e defina `AZ_REPO` para o valor correto.</span><span class="sxs-lookup"><span data-stu-id="4bcb1-124">Otherwise, look up information for your distribution on how to determine the base distribution name and set `AZ_REPO` to the correct value.</span></span>

### <a name="no-package-for-your-distribution"></a><span data-ttu-id="4bcb1-125">Nenhum pacote para distribuição</span><span class="sxs-lookup"><span data-stu-id="4bcb1-125">No package for your distribution</span></span>

<span data-ttu-id="4bcb1-126">Às vezes, um pacote da CLI do Azure pode ficar disponível somente um tempo depois de uma distribuição do Ubuntu ser lançada.</span><span class="sxs-lookup"><span data-stu-id="4bcb1-126">Sometimes it may be a while after an Ubuntu distribution is released before there's an Azure CLI package made available for it.</span></span> <span data-ttu-id="4bcb1-127">A CLI do Azure é projetada para ser resiliente em relação a versões futuras das dependências e precisam da menor quantidade possível delas.</span><span class="sxs-lookup"><span data-stu-id="4bcb1-127">The Azure CLI designed to be resilient with regards to future versions of dependencies and rely on as few of them as possible.</span></span> <span data-ttu-id="4bcb1-128">Se não houver pacotes disponíveis para sua distribuição de base, tente um pacote de uma distribuição anterior.</span><span class="sxs-lookup"><span data-stu-id="4bcb1-128">If there's no package available for your base distribution, try a package for an earlier distribution.</span></span>

<span data-ttu-id="4bcb1-129">Para isso, defina o valor `AZ_REPO` manualmente na [etapa 1 de instalação](#install-step-1).</span><span class="sxs-lookup"><span data-stu-id="4bcb1-129">To do this, set the value of `AZ_REPO` manually in [install step 1](#install-step-1).</span></span> <span data-ttu-id="4bcb1-130">Para as distribuições do Ubuntu, use o repositório `bionic`; para as distribuições do Debian, use `stretch`.</span><span class="sxs-lookup"><span data-stu-id="4bcb1-130">For Ubuntu distributions use the `bionic` repository, and for Debian distributions use `stretch`.</span></span> <span data-ttu-id="4bcb1-131">Não há suporte para as distribuições lançadas antes do Ubuntu Trusty e do Debian Wheezy.</span><span class="sxs-lookup"><span data-stu-id="4bcb1-131">Distributions released before Ubuntu Trusty and Debian Wheezy are not supported.</span></span>

### <a name="apt-key-fails-with-no-dirmngr"></a><span data-ttu-id="4bcb1-132">apt-key falha com “Sem dirmngr”</span><span class="sxs-lookup"><span data-stu-id="4bcb1-132">apt-key fails with "No dirmngr"</span></span>

<span data-ttu-id="4bcb1-133">Ao executar o comando `apt-key`, pode ser que você veja uma saída semelhante ao seguinte erro:</span><span class="sxs-lookup"><span data-stu-id="4bcb1-133">When running the `apt-key` command, you may see output similar to the following error:</span></span>

```output
gpg: failed to start the dirmngr '/usr/bin/dirmngr': No such file or directory
gpg: connecting dirmngr at '/tmp/apt-key-gpghome.kt5zo27tp1/S.dirmngr' failed: No such file or directory
gpg: keyserver receive failed: No dirmngr
```

<span data-ttu-id="4bcb1-134">O erro ocorre devido a um componente ausente requerido por `apt-key`.</span><span class="sxs-lookup"><span data-stu-id="4bcb1-134">The error is due to a missing component required by `apt-key`.</span></span> <span data-ttu-id="4bcb1-135">Você pode resolver isso instalando o pacote `dirmngr`.</span><span class="sxs-lookup"><span data-stu-id="4bcb1-135">You can resolve it by installing the `dirmngr` package.</span></span>

```bash
sudo apt-get install dirmngr
```

### <a name="apt-key-hangs"></a><span data-ttu-id="4bcb1-136">apt-key trava</span><span class="sxs-lookup"><span data-stu-id="4bcb1-136">apt-key hangs</span></span>

<span data-ttu-id="4bcb1-137">Quando atrás de um firewall que bloqueia as conexões de saída para a porta 11371, o comando `apt-key` pode travar indefinidamente.</span><span class="sxs-lookup"><span data-stu-id="4bcb1-137">When behind a firewall blocking outgoing connections to port 11371, the `apt-key` command might hang indefinitely.</span></span>
<span data-ttu-id="4bcb1-138">O firewall pode exigir um proxy HTTP para as conexões de saída:</span><span class="sxs-lookup"><span data-stu-id="4bcb1-138">Your firewall may require an HTTP proxy for outgoing connections:</span></span>

```bash
sudo apt-key --keyring /etc/apt/trusted.gpg.d/Microsoft.gpg adv \
    --keyserver-options http-proxy=http://<USER>:<PASSWORD>@<PROXY-HOST>:<PROXY-PORT>/ \
    --keyserver packages.microsoft.com \
    --recv-keys BC528686B50D79E339D3721CEB3E94ADBE1229CF
```

<span data-ttu-id="4bcb1-139">Para determinar se você tem um proxy, entre em contato com o administrador do sistema.</span><span class="sxs-lookup"><span data-stu-id="4bcb1-139">To determine if you have a proxy, contact your system administrator.</span></span> <span data-ttu-id="4bcb1-140">Se o proxy não precisar de logon, omita as informações sobre usuário e senha.</span><span class="sxs-lookup"><span data-stu-id="4bcb1-140">If your proxy does not require a login, then leave out the user and password information.</span></span>

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="4bcb1-141">Atualizar</span><span class="sxs-lookup"><span data-stu-id="4bcb1-141">Update</span></span>

<span data-ttu-id="4bcb1-142">Use `apt-get upgrade` para atualizar o pacote da CLI.</span><span class="sxs-lookup"><span data-stu-id="4bcb1-142">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!WARNING]
> <span data-ttu-id="4bcb1-143">A chave de assinatura foi atualizada em maio de 2018 e foi substituída.</span><span class="sxs-lookup"><span data-stu-id="4bcb1-143">The signing key was updated in May 2018, and has been replaced.</span></span> <span data-ttu-id="4bcb1-144">Se você receber erros de autenticação, verifique se tem [a chave de autenticação mais recente](#signingKey).</span><span class="sxs-lookup"><span data-stu-id="4bcb1-144">If you receive signing errors, make sure you have [the latest signing key](#signingKey).</span></span>
>
> [!NOTE]
> <span data-ttu-id="4bcb1-145">Esse comando atualiza todos os pacotes instalados no sistema que não tiveram uma alteração de dependência.</span><span class="sxs-lookup"><span data-stu-id="4bcb1-145">This command upgrades all of the installed packages on your system that have not had a dependency change.</span></span>
> <span data-ttu-id="4bcb1-146">Para atualizar apenas a CLI, use `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="4bcb1-146">To upgrade the CLI only, use `apt-get install`.</span></span>
> 
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a><span data-ttu-id="4bcb1-147">Desinstalar</span><span class="sxs-lookup"><span data-stu-id="4bcb1-147">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="4bcb1-148">Desinstalar com `apt-get remove`:</span><span class="sxs-lookup"><span data-stu-id="4bcb1-148">Uninstall with `apt-get remove`:</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="4bcb1-149">Se você não pretender reinstalar a CLI, remova as informações do repositório da CLI do Azure:</span><span class="sxs-lookup"><span data-stu-id="4bcb1-149">If you don't plan to reinstall the CLI, remove the Azure CLI repository information:</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="4bcb1-150">Remova a chave de autenticação:</span><span class="sxs-lookup"><span data-stu-id="4bcb1-150">Remove the signing key:</span></span>

    ```bash
    sudo rm /etc/apt/trusted.gpg.d/Microsoft.gpg
    ```

4. <span data-ttu-id="4bcb1-151">Remova quaisquer pacotes desnecessários:</span><span class="sxs-lookup"><span data-stu-id="4bcb1-151">Remove any unneeded packages:</span></span>

   ```bash
   sudo apt autoremove
   ```

## <a name="next-steps"></a><span data-ttu-id="4bcb1-152">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="4bcb1-152">Next Steps</span></span>

<span data-ttu-id="4bcb1-153">Agora que você instalou a CLI do Azure, faça um tour breve de seus recursos e comandos comuns.</span><span class="sxs-lookup"><span data-stu-id="4bcb1-153">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="4bcb1-154">Introdução à CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="4bcb1-154">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
