---
title: Instalar a CLI do Azure no Linux com apt
description: Como instalar a CLI do Azure com o gerenciador de pacotes apt
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 03/19/2019
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: fa2e1db439b4836d7506409b3abcce74fb6e6695
ms.sourcegitcommit: 5864f72b9a6fbf82a4d98bf805b3a16a7da18556
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/22/2019
ms.locfileid: "58343138"
---
# <a name="install-azure-cli-with-apt"></a><span data-ttu-id="edbd6-103">Instalar CLI do Azure com o apt</span><span class="sxs-lookup"><span data-stu-id="edbd6-103">Install Azure CLI with apt</span></span>

<span data-ttu-id="edbd6-104">Se você estiver executando uma distribuição fornecida com `apt`, como Ubuntu ou Debian, há um pacote x86_64 disponível para a CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="edbd6-104">If you are running a distribution that comes with `apt`, such as Ubuntu or Debian, there's an x86_64 package available for the Azure CLI.</span></span> <span data-ttu-id="edbd6-105">Esse pacote foi testado com:</span><span class="sxs-lookup"><span data-stu-id="edbd6-105">This package has been tested with:</span></span>

* <span data-ttu-id="edbd6-106">Ubuntu trusty, xenial, artful e bionic</span><span class="sxs-lookup"><span data-stu-id="edbd6-106">Ubuntu trusty, xenial, artful, and bionic</span></span>
* <span data-ttu-id="edbd6-107">Debian wheezy, jessie e stretch</span><span class="sxs-lookup"><span data-stu-id="edbd6-107">Debian wheezy, jessie, and stretch</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

> [!NOTE]
>
> <span data-ttu-id="edbd6-108">O pacote para a CLI do Azure instala seu próprio interpretador de Python e não usa o Python do sistema.</span><span class="sxs-lookup"><span data-stu-id="edbd6-108">The package for Azure CLI installs its own Python interpreter, and does not use the system Python.</span></span>

## <a name="install"></a><span data-ttu-id="edbd6-109">Instalar</span><span class="sxs-lookup"><span data-stu-id="edbd6-109">Install</span></span>

1. <span data-ttu-id="edbd6-110">Obtenha os pacotes necessários para o processo de instalação:</span><span class="sxs-lookup"><span data-stu-id="edbd6-110">Get packages needed for the install process:</span></span>

    ```bash
    sudo apt-get update
    sudo apt-get install curl apt-transport-https lsb-release gpg
    ```

2. <span data-ttu-id="edbd6-111">Baixe e instale a chave de autenticação da Microsoft:</span><span class="sxs-lookup"><span data-stu-id="edbd6-111">Download and install the Microsoft signing key:</span></span>

    ```bash
    curl -sL https://packages.microsoft.com/keys/microsoft.asc | \
        gpg --dearmor | \
        sudo tee /etc/apt/trusted.gpg.d/microsoft.asc.gpg > /dev/null
    ```

3. <div id="set-release"/><span data-ttu-id="edbd6-112">Adicione o repositório de software da CLI do Azure:</span><span class="sxs-lookup"><span data-stu-id="edbd6-112">Add the Azure CLI software repository:</span></span>

    ```bash
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
    ```

4. <span data-ttu-id="edbd6-113">Atualize as informações do repositório e instale o pacote `azure-cli`:</span><span class="sxs-lookup"><span data-stu-id="edbd6-113">Update repository information and install the `azure-cli` package:</span></span>

    ```bash
    sudo apt-get update
    sudo apt-get install azure-cli
    ```

<span data-ttu-id="edbd6-114">Execute a CLI do Azure com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="edbd6-114">Run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="edbd6-115">Para entrar, use o comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="edbd6-115">To sign in, use the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="edbd6-116">Para saber mais sobre os diferentes métodos de autenticação, confira [Entrar com a CLI do Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="edbd6-116">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="edbd6-117">solução de problemas</span><span class="sxs-lookup"><span data-stu-id="edbd6-117">Troubleshooting</span></span>

<span data-ttu-id="edbd6-118">Aqui estão alguns problemas comuns vistos durante a instalação com `apt`.</span><span class="sxs-lookup"><span data-stu-id="edbd6-118">Here are some common problems seen when installing with `apt`.</span></span> <span data-ttu-id="edbd6-119">Se você tiver um problema não abordado aqui, [arquive um problema no github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="edbd6-119">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="lsbrelease-does-not-return-the-correct-base-distribution-version"></a><span data-ttu-id="edbd6-120">lsb_release não retorna a versão correta da distribuição de base</span><span class="sxs-lookup"><span data-stu-id="edbd6-120">lsb_release does not return the correct base distribution version</span></span>

<span data-ttu-id="edbd6-121">Algumas distribuições derivadas do Ubuntu ou do Debian, como o Linux Mint, podem não retornar o nome correto da versão de `lsb_release`.</span><span class="sxs-lookup"><span data-stu-id="edbd6-121">Some Ubuntu- or Debian-derived distributions such as Linux Mint may not return the correct version name from `lsb_release`.</span></span> <span data-ttu-id="edbd6-122">Esse valor é usado no processo de instalação para determinar o pacote de instalação.</span><span class="sxs-lookup"><span data-stu-id="edbd6-122">This value is used in the install process to determine the package to install.</span></span> <span data-ttu-id="edbd6-123">Se você souber o nome do código da versão do Ubuntu ou do Debian da qual sua distribuição é derivada, poderá definir o valor de `AZ_REPO` manualmente ao [adicionar o repositório](#set-release).</span><span class="sxs-lookup"><span data-stu-id="edbd6-123">If you know the code name of the Ubuntu or Debian version your distribution is derived from, you can set the `AZ_REPO` value manually when [adding the repository](#set-release).</span></span> <span data-ttu-id="edbd6-124">Caso contrário, procure informações para sua distribuição sobre como determinar o nome do código da distribuição de base e defina `AZ_REPO` com o valor correto.</span><span class="sxs-lookup"><span data-stu-id="edbd6-124">Otherwise, look up information for your distribution on how to determine the base distribution code name and set `AZ_REPO` to the correct value.</span></span>

### <a name="no-package-for-your-distribution"></a><span data-ttu-id="edbd6-125">Nenhum pacote para distribuição</span><span class="sxs-lookup"><span data-stu-id="edbd6-125">No package for your distribution</span></span>

<span data-ttu-id="edbd6-126">Às vezes, um pacote da CLI do Azure pode ser disponibilizado somente um tempo depois do lançamento da distribuição.</span><span class="sxs-lookup"><span data-stu-id="edbd6-126">Sometimes it may be a while after a distribution is released before there's an Azure CLI package available for it.</span></span> <span data-ttu-id="edbd6-127">A CLI do Azure é projetada para ser resiliente em relação a versões futuras das dependências e precisam da menor quantidade possível delas.</span><span class="sxs-lookup"><span data-stu-id="edbd6-127">The Azure CLI designed to be resilient with regards to future versions of dependencies and rely on as few of them as possible.</span></span> <span data-ttu-id="edbd6-128">Se não houver pacotes disponíveis para sua distribuição de base, tente um pacote de uma distribuição anterior.</span><span class="sxs-lookup"><span data-stu-id="edbd6-128">If there's no package available for your base distribution, try a package for an earlier distribution.</span></span>

<span data-ttu-id="edbd6-129">Para isso, defina o valor de `AZ_REPO` manualmente ao [adicionar o repositório](#set-release).</span><span class="sxs-lookup"><span data-stu-id="edbd6-129">To do this, set the value of `AZ_REPO` manually when [adding the repository](#set-release).</span></span> <span data-ttu-id="edbd6-130">Para as distribuições do Ubuntu, use o repositório `bionic`; para as distribuições do Debian, use `stretch`.</span><span class="sxs-lookup"><span data-stu-id="edbd6-130">For Ubuntu distributions use the `bionic` repository, and for Debian distributions use `stretch`.</span></span> <span data-ttu-id="edbd6-131">Não há suporte para as distribuições lançadas antes do Ubuntu Trusty e do Debian Wheezy.</span><span class="sxs-lookup"><span data-stu-id="edbd6-131">Distributions released before Ubuntu Trusty and Debian Wheezy are not supported.</span></span>

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="edbd6-132">Atualizar</span><span class="sxs-lookup"><span data-stu-id="edbd6-132">Update</span></span>

<span data-ttu-id="edbd6-133">Use `apt-get upgrade` para atualizar o pacote da CLI.</span><span class="sxs-lookup"><span data-stu-id="edbd6-133">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="edbd6-134">Esse comando atualiza todos os pacotes instalados no sistema que não tiveram uma alteração de dependência.</span><span class="sxs-lookup"><span data-stu-id="edbd6-134">This command upgrades all of the installed packages on your system that have not had a dependency change.</span></span>
> <span data-ttu-id="edbd6-135">Para atualizar apenas a CLI, use `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="edbd6-135">To upgrade the CLI only, use `apt-get install`.</span></span>
> 
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a><span data-ttu-id="edbd6-136">Desinstalar</span><span class="sxs-lookup"><span data-stu-id="edbd6-136">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="edbd6-137">Desinstalar com `apt-get remove`:</span><span class="sxs-lookup"><span data-stu-id="edbd6-137">Uninstall with `apt-get remove`:</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="edbd6-138">Se você não pretender reinstalar a CLI, remova as informações do repositório da CLI do Azure:</span><span class="sxs-lookup"><span data-stu-id="edbd6-138">If you don't plan to reinstall the CLI, remove the Azure CLI repository information:</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="edbd6-139">Remova a chave de autenticação:</span><span class="sxs-lookup"><span data-stu-id="edbd6-139">Remove the signing key:</span></span>

    ```bash
    sudo rm /etc/apt/trusted.gpg.d/microsoft.asc.gpg
    ```

4. <span data-ttu-id="edbd6-140">Remova quaisquer pacotes desnecessários:</span><span class="sxs-lookup"><span data-stu-id="edbd6-140">Remove any unneeded packages:</span></span>

   ```bash
   sudo apt autoremove
   ```

## <a name="next-steps"></a><span data-ttu-id="edbd6-141">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="edbd6-141">Next Steps</span></span>

<span data-ttu-id="edbd6-142">Agora que você instalou a CLI do Azure, faça um tour breve de seus recursos e comandos comuns.</span><span class="sxs-lookup"><span data-stu-id="edbd6-142">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="edbd6-143">Introdução à CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="edbd6-143">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
