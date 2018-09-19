---
title: Instalar a CLI do Azure 2.0 no Linux com apt
description: Como instalar a CLI do Azure 2.0 com o gerenciador de pacotes apt
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 88b4570f62858ec1e12898aea51a5dbce6d677b5
ms.sourcegitcommit: 0e688704889fc88b91588bb6678a933c2d54f020
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/11/2018
ms.locfileid: "44388404"
---
# <a name="install-azure-cli-20-with-apt"></a><span data-ttu-id="2ffaf-103">Instalar CLI do Azure 2.0 com o apt</span><span class="sxs-lookup"><span data-stu-id="2ffaf-103">Install Azure CLI 2.0 with apt</span></span>

<span data-ttu-id="2ffaf-104">Se você estiver executando uma distribuição que vem com `apt`, como o Ubuntu ou o Debian, haverá um pacote de 64 bits disponível para a CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="2ffaf-104">If you are running a distribution that comes with `apt`, such as Ubuntu or Debian, there's a 64-bit package available for the Azure CLI.</span></span> <span data-ttu-id="2ffaf-105">Esse pacote foi testado com:</span><span class="sxs-lookup"><span data-stu-id="2ffaf-105">This package has been tested with:</span></span>

* <span data-ttu-id="2ffaf-106">Ubuntu trusty, xenial, artful e bionic</span><span class="sxs-lookup"><span data-stu-id="2ffaf-106">Ubuntu trusty, xenial, artful, and bionic</span></span>
* <span data-ttu-id="2ffaf-107">Debian wheezy, jessie e stretch</span><span class="sxs-lookup"><span data-stu-id="2ffaf-107">Debian wheezy, jessie, and stretch</span></span>

## <a name="install"></a><span data-ttu-id="2ffaf-108">Instalar</span><span class="sxs-lookup"><span data-stu-id="2ffaf-108">Install</span></span>

1. <div id="install-step-1"/><span data-ttu-id="2ffaf-109">Modifique sua lista de fontes:</span><span class="sxs-lookup"><span data-stu-id="2ffaf-109">Modify your sources list:</span></span>

    ```bash
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
    ```

2. <div id="signingKey"/><span data-ttu-id="2ffaf-110">Obtenha a chave de assinatura da Microsoft:</span><span class="sxs-lookup"><span data-stu-id="2ffaf-110">Get the Microsoft signing key:</span></span>

   ```bash
   curl -L https://packages.microsoft.com/keys/microsoft.asc | sudo apt-key add -
   ```

3. <span data-ttu-id="2ffaf-111">Instalar a CLI:</span><span class="sxs-lookup"><span data-stu-id="2ffaf-111">Install the CLI:</span></span>

   ```bash
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

   > [!WARNING]
   > <span data-ttu-id="2ffaf-112">A chave de assinatura foi atualizada em maio de 2018 e foi substituída.</span><span class="sxs-lookup"><span data-stu-id="2ffaf-112">The signing key was updated in May 2018, and has been replaced.</span></span> <span data-ttu-id="2ffaf-113">Se você receber erros da chave de assinatura, confirme se [adquiriu a chave de assinatura mais recente](#signingKey).</span><span class="sxs-lookup"><span data-stu-id="2ffaf-113">If you receive signing key errors, please ensure that you have [acquired the latest signing key](#signingKey).</span></span>

<span data-ttu-id="2ffaf-114">É possível executar a CLI do Azure com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="2ffaf-114">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="2ffaf-115">Para entrar, use o comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="2ffaf-115">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="2ffaf-116">Para saber mais sobre os diferentes métodos de autenticação, consulte [Conectar com a CLI do Azure 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="2ffaf-116">To learn more about different authentication methods, see [Sign in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="2ffaf-117">solução de problemas</span><span class="sxs-lookup"><span data-stu-id="2ffaf-117">Troubleshooting</span></span>

<span data-ttu-id="2ffaf-118">Aqui estão alguns problemas comuns vistos durante a instalação com `apt`.</span><span class="sxs-lookup"><span data-stu-id="2ffaf-118">Here are some common problems seen when installing with `apt`.</span></span> <span data-ttu-id="2ffaf-119">Se você tiver um problema não abordado aqui, [arquive um problema no github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="2ffaf-119">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="lsbrelease-fails-with-command-not-found"></a><span data-ttu-id="2ffaf-120">lsb_release falha com "Comando não encontrado"</span><span class="sxs-lookup"><span data-stu-id="2ffaf-120">lsb_release fails with "Command not found"</span></span>

<span data-ttu-id="2ffaf-121">Ao executar o comando `lsb_release`, pode ser que você veja uma saída semelhante ao seguinte erro:</span><span class="sxs-lookup"><span data-stu-id="2ffaf-121">When running the `lsb_release` command, you may see output similar to the following error:</span></span>

```output
-bash: lsb_release: command not found
```

<span data-ttu-id="2ffaf-122">O erro é devido ao comando `lsb_release` não estar instalado.</span><span class="sxs-lookup"><span data-stu-id="2ffaf-122">The error is due to the `lsb_release` command not being installed.</span></span> <span data-ttu-id="2ffaf-123">Você pode resolver isso instalando o pacote `lsb-release`.</span><span class="sxs-lookup"><span data-stu-id="2ffaf-123">You can resolve it by installing the `lsb-release` package.</span></span>

```bash
sudo apt-get install lsb-release
```

### <a name="lsbrelease-does-not-return-the-base-distribution-version"></a><span data-ttu-id="2ffaf-124">lsb_release não retorna a versão da distribuição de base</span><span class="sxs-lookup"><span data-stu-id="2ffaf-124">lsb_release does not return the base distribution version</span></span>

<span data-ttu-id="2ffaf-125">Algumas distribuições derivadas do Ubuntu ou do Debian, como o Linux Mint, podem não retornar o nome correto da versão de `lsb_release`.</span><span class="sxs-lookup"><span data-stu-id="2ffaf-125">Some Ubuntu- or Debian-derived distributions such as Linux Mint may not return the correct version name from `lsb_release`.</span></span> <span data-ttu-id="2ffaf-126">Esse valor é usado no processo de instalação para determinar o pacote de instalação.</span><span class="sxs-lookup"><span data-stu-id="2ffaf-126">This value is used in the install process to determine the package to install.</span></span> <span data-ttu-id="2ffaf-127">Se você souber o nome da versão da qual sua distribuição é derivada, poderá definir o `AZ_REPO` valor manualmente em [instalar etapa 1](#install-step-1).</span><span class="sxs-lookup"><span data-stu-id="2ffaf-127">If you know the name of the version your distribution is derived from, you can set the `AZ_REPO` value manually in [install step 1](#install-step-1).</span></span> <span data-ttu-id="2ffaf-128">Caso contrário, procure informações para sua distribuição sobre como determinar o nome da distribuição de base e defina `AZ_REPO` para o valor correto.</span><span class="sxs-lookup"><span data-stu-id="2ffaf-128">Otherwise, look up information for your distribution on how to determine the base distribution name and set `AZ_REPO` to the correct value.</span></span>

### <a name="apt-key-fails-with-no-dirmngr"></a><span data-ttu-id="2ffaf-129">apt-key falha com “Sem dirmngr”</span><span class="sxs-lookup"><span data-stu-id="2ffaf-129">apt-key fails with "No dirmngr"</span></span>

<span data-ttu-id="2ffaf-130">Ao executar o comando `apt-key`, pode ser que você veja uma saída semelhante ao seguinte erro:</span><span class="sxs-lookup"><span data-stu-id="2ffaf-130">When running the `apt-key` command, you may see output similar to the following error:</span></span>

```output
gpg: failed to start the dirmngr '/usr/bin/dirmngr': No such file or directory
gpg: connecting dirmngr at '/tmp/apt-key-gpghome.kt5zo27tp1/S.dirmngr' failed: No such file or directory
gpg: keyserver receive failed: No dirmngr
```

<span data-ttu-id="2ffaf-131">O erro ocorre devido a um componente ausente requerido por `apt-key`.</span><span class="sxs-lookup"><span data-stu-id="2ffaf-131">The error is due to a missing component required by `apt-key`.</span></span> <span data-ttu-id="2ffaf-132">Você pode resolver isso instalando o pacote `dirmngr`.</span><span class="sxs-lookup"><span data-stu-id="2ffaf-132">You can resolve it by installing the `dirmngr` package.</span></span>

```bash
sudo apt-get install dirmngr
```

### <a name="apt-key-hangs"></a><span data-ttu-id="2ffaf-133">apt-key trava</span><span class="sxs-lookup"><span data-stu-id="2ffaf-133">apt-key hangs</span></span>

<span data-ttu-id="2ffaf-134">Quando atrás de um firewall que bloqueia as conexões de saída para a porta 11371, o comando `apt-key` pode travar indefinidamente.</span><span class="sxs-lookup"><span data-stu-id="2ffaf-134">When behind a firewall blocking outgoing connections to port 11371, the `apt-key` command might hang indefinitely.</span></span> <span data-ttu-id="2ffaf-135">O firewall pode exigir o uso de um proxy HTTP para as conexões de saída:</span><span class="sxs-lookup"><span data-stu-id="2ffaf-135">Your firewall may require the use of an HTTP proxy for outgoing connections:</span></span>

```bash
sudo apt-key adv --keyserver-options http-proxy=http://<USER>:<PASSWORD>@<PROXY-HOST>:<PROXY-PORT>/ --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
```

<span data-ttu-id="2ffaf-136">Para determinar se você tem um proxy, entre em contato com o administrador do sistema.</span><span class="sxs-lookup"><span data-stu-id="2ffaf-136">To determine if you have a proxy, contact your system administrator.</span></span> <span data-ttu-id="2ffaf-137">Se o proxy não precisar de logon, omita o usuário, a senha e o token `@`.</span><span class="sxs-lookup"><span data-stu-id="2ffaf-137">If your proxy does not require a login, then leave out the user, password, and `@` token.</span></span>

## <a name="update"></a><span data-ttu-id="2ffaf-138">Atualizar</span><span class="sxs-lookup"><span data-stu-id="2ffaf-138">Update</span></span>

<span data-ttu-id="2ffaf-139">Use `apt-get upgrade` para atualizar o pacote da CLI.</span><span class="sxs-lookup"><span data-stu-id="2ffaf-139">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!WARNING]
> <span data-ttu-id="2ffaf-140">A chave de assinatura foi atualizada em maio de 2018 e foi substituída.</span><span class="sxs-lookup"><span data-stu-id="2ffaf-140">The signing key was updated in May 2018, and has been replaced.</span></span> <span data-ttu-id="2ffaf-141">Se você receber erros da chave de assinatura, confirme se [adquiriu a chave de assinatura mais recente](#signingKey).</span><span class="sxs-lookup"><span data-stu-id="2ffaf-141">If you receive signing key errors, please ensure that you have [acquired the latest signing key](#signingKey).</span></span>
>
> [!NOTE]
> <span data-ttu-id="2ffaf-142">Esse comando atualiza todos os pacotes instalados no sistema que não tiveram uma alteração de dependência.</span><span class="sxs-lookup"><span data-stu-id="2ffaf-142">This command upgrades all of the installed packages on your system that have not had a dependency change.</span></span>
> <span data-ttu-id="2ffaf-143">Para atualizar apenas a CLI, use `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="2ffaf-143">To upgrade the CLI only, use `apt-get install`.</span></span>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a><span data-ttu-id="2ffaf-144">Desinstalar</span><span class="sxs-lookup"><span data-stu-id="2ffaf-144">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="2ffaf-145">Desinstalar com `apt-get remove`.</span><span class="sxs-lookup"><span data-stu-id="2ffaf-145">Uninstall with `apt-get remove`.</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="2ffaf-146">Se você não pretende reinstalar a CLI, remova as informações do repositório da CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="2ffaf-146">If you don't plan to reinstall the CLI, remove the Azure CLI repository information.</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="2ffaf-147">Remova quaisquer pacotes desnecessários.</span><span class="sxs-lookup"><span data-stu-id="2ffaf-147">Remove any unneeded packages.</span></span>

   ```bash
   sudo apt autoremove
   ```
