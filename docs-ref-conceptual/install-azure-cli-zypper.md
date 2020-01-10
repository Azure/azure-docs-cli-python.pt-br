---
title: Instalar a CLI do Azure no Linux com zypper
description: Como instalar a CLI do Azure com o zypper
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 7e5897fe545527aa2708432e0ad0cf626584c785
ms.sourcegitcommit: 0088160bdb1ea520724d3e1efe71a4a66f29753d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2019
ms.locfileid: "75216864"
---
# <a name="install-azure-cli-with-zypper"></a><span data-ttu-id="33c53-103">Instalar CLI do Azure com zypper</span><span class="sxs-lookup"><span data-stu-id="33c53-103">Install Azure CLI with zypper</span></span>

<span data-ttu-id="33c53-104">Para distribuições Linux com `zypper`, como o openSUSE ou SLES, há um pacote disponível para a CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="33c53-104">For Linux distributions with `zypper`, such as openSUSE or SLES, there's a package available for the Azure CLI.</span></span> <span data-ttu-id="33c53-105">Este pacote foi testado com openSUSE Leap 15.1 e SLES 15.</span><span class="sxs-lookup"><span data-stu-id="33c53-105">This package has been tested with openSUSE Leap 15.1, and SLES 15.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

[!INCLUDE [rpm-warning](includes/rpm-warning.md)]

## <a name="install"></a><span data-ttu-id="33c53-106">Instalar</span><span class="sxs-lookup"><span data-stu-id="33c53-106">Install</span></span>

1. <span data-ttu-id="33c53-107">Instale `curl`:</span><span class="sxs-lookup"><span data-stu-id="33c53-107">Install `curl`:</span></span>

   ```bash
   sudo zypper install -y curl
   ```

2. <span data-ttu-id="33c53-108">Importe a chave de repositório da Microsoft:</span><span class="sxs-lookup"><span data-stu-id="33c53-108">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

3. <span data-ttu-id="33c53-109">Crie informações sobre o repositório do `azure-cli` local:</span><span class="sxs-lookup"><span data-stu-id="33c53-109">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo zypper addrepo --name 'Azure CLI' --check https://packages.microsoft.com/yumrepos/azure-cli azure-cli
   ```

4. <span data-ttu-id="33c53-110">Atualize o índice de pacote do `zypper` e instale:</span><span class="sxs-lookup"><span data-stu-id="33c53-110">Update the `zypper` package index and install:</span></span>

   ```bash
   sudo zypper install --from azure-cli -y azure-cli
   ```

<span data-ttu-id="33c53-111">É possível executar a CLI do Azure com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="33c53-111">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="33c53-112">Para entrar, use o comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="33c53-112">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="33c53-113">Para saber mais sobre os diferentes métodos de autenticação, confira [Entrar com a CLI do Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="33c53-113">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="33c53-114">solução de problemas</span><span class="sxs-lookup"><span data-stu-id="33c53-114">Troubleshooting</span></span>

<span data-ttu-id="33c53-115">Aqui estão alguns problemas comuns vistos durante a instalação com `zypper`.</span><span class="sxs-lookup"><span data-stu-id="33c53-115">Here are some common problems seen when installing with `zypper`.</span></span> <span data-ttu-id="33c53-116">Se você tiver um problema não abordado aqui, [arquive um problema no github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="33c53-116">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="install-on-sles-12-or-other-other-systems-without-python-36"></a><span data-ttu-id="33c53-117">Instalar no SLES 12 ou em outros sistemas sem Python 3.6</span><span class="sxs-lookup"><span data-stu-id="33c53-117">Install on SLES 12 or other other systems without Python 3.6</span></span>

<span data-ttu-id="33c53-118">No SLES 12, o pacote python3 padrão é 3.4 e não é compatível com a CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="33c53-118">On SLES 12, the defualt python3 package is 3.4 and not supported by Azure CLI.</span></span> <span data-ttu-id="33c53-119">É possível criar primeiro uma versão superior do python3 da origem.</span><span class="sxs-lookup"><span data-stu-id="33c53-119">You can first build a higher version python3 from source.</span></span> <span data-ttu-id="33c53-120">Em seguida, você poderá baixar o pacote da CLI do Azure e instalá-lo sem dependência.</span><span class="sxs-lookup"><span data-stu-id="33c53-120">Then you can download the Azure CLI package and install it without dependency.</span></span>
```bash
$ sudo zypper install -y gcc gcc-c++ make ncurses patch wget tar zlib-devel zlib
# Download Python source code
$ PYTHON_VERSION="3.6.9"
$ PYTHON_SRC_DIR=$(mktemp -d)
$ wget -qO- https://www.python.org/ftp/python/$PYTHON_VERSION/Python-$PYTHON_VERSION.tgz | tar -xz -C "$PYTHON_SRC_DIR"
# Build Python
$ $PYTHON_SRC_DIR/*/configure --with-ssl
$ make
$ sudo make install
#Download azure-cli package 
$ AZ_VERSION=$(zypper --no-refresh info azure-cli |grep Version | awk -F': ' '{print $2}' | awk '{$1=$1;print}')
$ wget https://packages.microsoft.com/yumrepos/azure-cli/azure-cli-$AZ_VERSION.x86_64.rpm
#Install without dependency
$ sudo rpm -ivh --nodeps azure-cli-$AZ_VERSION.x86_64.rpm
```

### <a name="proxy-blocks-connection"></a><span data-ttu-id="33c53-121">Conexão de blocos de proxy</span><span class="sxs-lookup"><span data-stu-id="33c53-121">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](includes/configure-proxy.md)]

<span data-ttu-id="33c53-122">Talvez você queira configurar explicitamente `zypper` (por meio de `yast2`) para usar esse proxy sempre.</span><span class="sxs-lookup"><span data-stu-id="33c53-122">You may also want to explicitly configure `zypper` (via `yast2`) to use this proxy at all times.</span></span> <span data-ttu-id="33c53-123">Para fazer isso, execute o comando `yast2 proxy` como superusuário e preencha as informações apresentadas no formulário.</span><span class="sxs-lookup"><span data-stu-id="33c53-123">To do so, run the `yast2 proxy` command as superuser, and fill in the information presented in the form.</span></span> <span data-ttu-id="33c53-124">Se você tiver um gerenciador de janelas disponível no sistema, também poderá usar o painel `Network Services > Proxy` no `YaST Control Center`.</span><span class="sxs-lookup"><span data-stu-id="33c53-124">If you have a window manager available on your system, you can also use the `Network Services > Proxy` pane in the `YaST Control Center`.</span></span>

<span data-ttu-id="33c53-125">Para configurações avançadas ou mais informações, confira a [documentação de configuração do Proxy do OpenSUSE](https://www.suse.com/documentation/slms1/book_slms/data/sec_wy_config_updates_proxy.html)</span><span class="sxs-lookup"><span data-stu-id="33c53-125">For advanced configuration or more information, see the [OpenSUSE Proxy configuration documentation](https://www.suse.com/documentation/slms1/book_slms/data/sec_wy_config_updates_proxy.html)</span></span>

<span data-ttu-id="33c53-126">Para obter a chave de assinatura da Microsoft e o pacote do nosso repositório, o proxy precisa permitir conexões HTTPS com os seguintes endereços:</span><span class="sxs-lookup"><span data-stu-id="33c53-126">In order to get the Microsoft signing key and get the package from our repository, your proxy needs to allow HTTPS connections to the following addresses:</span></span>

* `https://packages.microsoft.com`
* `https://download.opensuse.org`

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="33c53-127">Atualizar</span><span class="sxs-lookup"><span data-stu-id="33c53-127">Update</span></span>

<span data-ttu-id="33c53-128">Você pode atualizar o pacote com o comando `zypper update`.</span><span class="sxs-lookup"><span data-stu-id="33c53-128">You can update the package with the `zypper update` command.</span></span>

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="33c53-129">Desinstalar</span><span class="sxs-lookup"><span data-stu-id="33c53-129">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="33c53-130">Remova o pacote do seu sistema.</span><span class="sxs-lookup"><span data-stu-id="33c53-130">Remove the package from your system.</span></span>

    ```bash
    sudo zypper remove -y azure-cli
    ```

2. <span data-ttu-id="33c53-131">Se você não pretende reinstalar a CLI, remova as informações do repositório.</span><span class="sxs-lookup"><span data-stu-id="33c53-131">If you don't plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo zypper removerepo azure-cli
   ```

3. <span data-ttu-id="33c53-132">Se você não usa outros pacotes da Microsoft, remova a chave de assinatura da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="33c53-132">If you don't use other Microsoft packages, remove the Microsoft signing key.</span></span>

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```

## <a name="next-steps"></a><span data-ttu-id="33c53-133">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="33c53-133">Next Steps</span></span>

<span data-ttu-id="33c53-134">Agora que você instalou a CLI do Azure, faça um tour breve de seus recursos e comandos comuns.</span><span class="sxs-lookup"><span data-stu-id="33c53-134">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="33c53-135">Introdução à CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="33c53-135">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
