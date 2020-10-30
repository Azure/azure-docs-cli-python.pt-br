---
title: Instalar a CLI do Azure no Linux com zypper
description: Como instalar a CLI do Azure com o zypper
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/25/2020
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: e501d05985b0483442ab11f78343d773fd7e55bf
ms.sourcegitcommit: 1187fb75b68426c46e84b3f294c509ee7b7da9be
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/27/2020
ms.locfileid: "92687088"
---
# <a name="install-azure-cli-with-zypper"></a><span data-ttu-id="2cce1-103">Instalar CLI do Azure com zypper</span><span class="sxs-lookup"><span data-stu-id="2cce1-103">Install Azure CLI with zypper</span></span>

<span data-ttu-id="2cce1-104">Para distribuições Linux com `zypper`, como o openSUSE ou SLES, há um pacote disponível para a CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="2cce1-104">For Linux distributions with `zypper`, such as openSUSE or SLES, there's a package available for the Azure CLI.</span></span> <span data-ttu-id="2cce1-105">Este pacote foi testado com openSUSE Leap 15.1 e SLES 15.</span><span class="sxs-lookup"><span data-stu-id="2cce1-105">This package has been tested with openSUSE Leap 15.1, and SLES 15.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

[!INCLUDE [rpm-warning](includes/rpm-warning.md)]

## <a name="install"></a><span data-ttu-id="2cce1-106">Instalar</span><span class="sxs-lookup"><span data-stu-id="2cce1-106">Install</span></span>

1. <span data-ttu-id="2cce1-107">Instale `curl`:</span><span class="sxs-lookup"><span data-stu-id="2cce1-107">Install `curl`:</span></span>

   ```bash
   sudo zypper install -y curl
   ```

2. <span data-ttu-id="2cce1-108">Importe a chave de repositório da Microsoft:</span><span class="sxs-lookup"><span data-stu-id="2cce1-108">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

3. <span data-ttu-id="2cce1-109">Crie informações sobre o repositório do `azure-cli` local:</span><span class="sxs-lookup"><span data-stu-id="2cce1-109">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo zypper addrepo --name 'Azure CLI' --check https://packages.microsoft.com/yumrepos/azure-cli azure-cli
   ```

4. <span data-ttu-id="2cce1-110">Atualize o índice de pacote do `zypper` e instale:</span><span class="sxs-lookup"><span data-stu-id="2cce1-110">Update the `zypper` package index and install:</span></span>

   ```bash
   sudo zypper install --from azure-cli azure-cli
   ```
   <span data-ttu-id="2cce1-111">Entrada 2 para continuar a instalar, ignorando algumas dependências.</span><span class="sxs-lookup"><span data-stu-id="2cce1-111">Input 2 to continue install by ignoring some of its dependencies.</span></span>

<span data-ttu-id="2cce1-112">É possível executar a CLI do Azure com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="2cce1-112">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="2cce1-113">Para entrar, use o comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="2cce1-113">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="2cce1-114">Para saber mais sobre os diferentes métodos de autenticação, confira [Entrar com a CLI do Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="2cce1-114">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="2cce1-115">Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="2cce1-115">Troubleshooting</span></span>

<span data-ttu-id="2cce1-116">Aqui estão alguns problemas comuns vistos durante a instalação com `zypper`.</span><span class="sxs-lookup"><span data-stu-id="2cce1-116">Here are some common problems seen when installing with `zypper`.</span></span> <span data-ttu-id="2cce1-117">Se você tiver um problema não abordado aqui, [arquive um problema no github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="2cce1-117">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="notimplementederror-on-opensuse-15-vm"></a><span data-ttu-id="2cce1-118">NotImplementedError na VM do OpenSUSE 15</span><span class="sxs-lookup"><span data-stu-id="2cce1-118">NotImplementedError on OpenSUSE 15 VM</span></span>
<span data-ttu-id="2cce1-119">A VM do OpenSUSE 15 tem uma CLI do Azure pré-instalada com a versão `2.0.45`, que está desatualizada e apresenta problemas com o comando `az login`.</span><span class="sxs-lookup"><span data-stu-id="2cce1-119">The OpenSUSE 15 VM has a pre-installed Azure CLI with version `2.0.45`, it's outdated and has issues with `az login`.</span></span> <span data-ttu-id="2cce1-120">Remova-a junto com as dependências antes de seguir as instruções de [instalação](#install) para adicionar a última CLI do Azure:</span><span class="sxs-lookup"><span data-stu-id="2cce1-120">Please remove it along with its dependencies before following the [Install](#install) instruction to add the latest Azure CLI:</span></span>
```bash
sudo zypper rm -y --clean-deps azure-cli
```

<span data-ttu-id="2cce1-121">Se você atualizou a CLI do Azure sem remover as dependências da versão `2.0.45`, as dependências antigas podem afetar a última versão da CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="2cce1-121">If you updated Azure CLI without removing the dependencies of version `2.0.45`, its old dependencies may affect the latest version of Azure CLI.</span></span> <span data-ttu-id="2cce1-122">Você precisará adicionar novamente a versão antiga para vinculá-la às dependências e remover a `azure-cli` junto com as dependências:</span><span class="sxs-lookup"><span data-stu-id="2cce1-122">You need to add back the old version to link to its dependencies and then remove `azure-cli` along with its dependencies:</span></span>
```bash
# The package name may vary on different system version, run 'zypper --no-refresh info azure-cli' to check the source package format
sudo zypper install --oldpackage azure-cli-2.0.45-4.22.noarch

sudo zypper rm -y --clean-deps azure-cli
```


### <a name="install-on-sles-12-or-other-systems-without-python-36"></a><span data-ttu-id="2cce1-123">Instalar no SLES 12 ou em sistemas sem o Python 3.6</span><span class="sxs-lookup"><span data-stu-id="2cce1-123">Install on SLES 12 or other systems without Python 3.6</span></span>

<span data-ttu-id="2cce1-124">No SLES 12, o pacote `python3` padrão é `3.4` e não é compatível com a CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="2cce1-124">On SLES 12, the default `python3` package is `3.4` and not supported by Azure CLI.</span></span> <span data-ttu-id="2cce1-125">Primeiro, siga as etapas 1 a 3 das [instruções de instalação](#install) para adicionar o repositório da `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="2cce1-125">You can first follow step 1-3 of the [install instruction](#install) to add the `azure-cli` repository.</span></span> <span data-ttu-id="2cce1-126">Em seguida, crie uma versão posterior do `python3` da origem.</span><span class="sxs-lookup"><span data-stu-id="2cce1-126">Then build a higher version `python3` from source.</span></span> <span data-ttu-id="2cce1-127">Por fim, você poderá baixar o pacote da CLI do Azure e instalá-lo sem nenhuma dependência.</span><span class="sxs-lookup"><span data-stu-id="2cce1-127">Finally, you can download the Azure CLI package and install it without dependency.</span></span>

<span data-ttu-id="2cce1-128">Use o seguinte comando para instalar a CLI do Azure (lembre-se de que a versão existente do Python 3 será substituída pelo Python 3.6):</span><span class="sxs-lookup"><span data-stu-id="2cce1-128">You can use the following one command to install Azure CLI (be aware that your existing Python 3 version will be overridden by Python 3.6):</span></span>
```bash
curl -sL https://azurecliprod.blob.core.windows.net/sles12_install.sh | sudo bash
```

<span data-ttu-id="2cce1-129">Ou, então, faça isso passo a passo:</span><span class="sxs-lookup"><span data-stu-id="2cce1-129">Or you can do it step by step:</span></span>

```bash
# !Please add azure-cli repository first following step 1-3 of the install instruction before running below commands
$ sudo zypper refresh
$ sudo zypper install -y gcc gcc-c++ make ncurses patch wget tar zlib-devel zlib openssl-devel
# Download Python source code
$ PYTHON_VERSION="3.6.9"
$ PYTHON_SRC_DIR=$(mktemp -d)
$ wget -qO- https://www.python.org/ftp/python/$PYTHON_VERSION/Python-$PYTHON_VERSION.tgz | tar -xz -C "$PYTHON_SRC_DIR"
# Build Python
# Please be aware that with --prefix=/usr, the command will override the existing Python 3 version
$ $PYTHON_SRC_DIR/*/configure --prefix=/usr
$ make
$ sudo make install
# Download azure-cli package 
$ AZ_VERSION=$(zypper --no-refresh info azure-cli |grep Version | awk -F': ' '{print $2}' | awk '{$1=$1;print}')
$ wget https://packages.microsoft.com/yumrepos/azure-cli/azure-cli-$AZ_VERSION.x86_64.rpm
# Install without dependency
$ sudo rpm -ivh --nodeps azure-cli-$AZ_VERSION.x86_64.rpm
```

### <a name="proxy-blocks-connection"></a><span data-ttu-id="2cce1-130">Conexão de blocos de proxy</span><span class="sxs-lookup"><span data-stu-id="2cce1-130">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](includes/configure-proxy.md)]

<span data-ttu-id="2cce1-131">Talvez você queira configurar explicitamente `zypper` (por meio de `yast2`) para usar esse proxy sempre.</span><span class="sxs-lookup"><span data-stu-id="2cce1-131">You may also want to explicitly configure `zypper` (via `yast2`) to use this proxy at all times.</span></span> <span data-ttu-id="2cce1-132">Para fazer isso, execute o comando `yast2 proxy` como superusuário e preencha as informações apresentadas no formulário.</span><span class="sxs-lookup"><span data-stu-id="2cce1-132">To do so, run the `yast2 proxy` command as superuser, and fill in the information presented in the form.</span></span> <span data-ttu-id="2cce1-133">Se você tiver um gerenciador de janelas disponível no sistema, também poderá usar o painel `Network Services > Proxy` no `YaST Control Center`.</span><span class="sxs-lookup"><span data-stu-id="2cce1-133">If you have a window manager available on your system, you can also use the `Network Services > Proxy` pane in the `YaST Control Center`.</span></span>

<span data-ttu-id="2cce1-134">Para configurações avançadas ou mais informações, confira a [documentação de configuração do Proxy do OpenSUSE](https://www.suse.com/documentation/slms1/book_slms/data/sec_wy_config_updates_proxy.html)</span><span class="sxs-lookup"><span data-stu-id="2cce1-134">For advanced configuration or more information, see the [OpenSUSE Proxy configuration documentation](https://www.suse.com/documentation/slms1/book_slms/data/sec_wy_config_updates_proxy.html)</span></span>

<span data-ttu-id="2cce1-135">Para obter a chave de assinatura da Microsoft e o pacote do nosso repositório, o proxy precisa permitir conexões HTTPS com os seguintes endereços:</span><span class="sxs-lookup"><span data-stu-id="2cce1-135">In order to get the Microsoft signing key and get the package from our repository, your proxy needs to allow HTTPS connections to the following addresses:</span></span>

* `https://packages.microsoft.com`
* `https://download.opensuse.org`

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

### <a name="ssl-certificate-problem"></a><span data-ttu-id="2cce1-136">Problema com o certificado SSL</span><span class="sxs-lookup"><span data-stu-id="2cce1-136">SSL certificate problem</span></span>

<span data-ttu-id="2cce1-137">Quando um certificado é inválido ou está desatualizado em um computador, você pode receber um erro indicando que o cURL falhou ao verificar a legitimidade do servidor e, portanto, não foi possível estabelecer uma conexão segura.</span><span class="sxs-lookup"><span data-stu-id="2cce1-137">When a certificate is broken or outdated on a machine, you may receive an error indicating that curl failed to verify the legitimacy of the server and therefore could not establish a secure connection.</span></span>  <span data-ttu-id="2cce1-138">Atualize o certificado para corrigir o problema.</span><span class="sxs-lookup"><span data-stu-id="2cce1-138">Update your certificate to correct the problem.</span></span>  

```bach
sudo zypper update-ca-certificates
```

## <a name="update"></a><span data-ttu-id="2cce1-139">Atualizar</span><span class="sxs-lookup"><span data-stu-id="2cce1-139">Update</span></span>

[!INCLUDE [az-upgrade](includes/az-upgrade.md)]

<span data-ttu-id="2cce1-140">Você também pode atualizar o pacote com o comando `zypper update`.</span><span class="sxs-lookup"><span data-stu-id="2cce1-140">You can also update the package with the `zypper update` command.</span></span>

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="2cce1-141">Desinstalar</span><span class="sxs-lookup"><span data-stu-id="2cce1-141">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="2cce1-142">Remova o pacote do seu sistema.</span><span class="sxs-lookup"><span data-stu-id="2cce1-142">Remove the package from your system.</span></span>

    ```bash
    sudo zypper remove -y azure-cli
    ```

2. <span data-ttu-id="2cce1-143">Se você não pretende reinstalar a CLI, remova as informações do repositório.</span><span class="sxs-lookup"><span data-stu-id="2cce1-143">If you don't plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo zypper removerepo azure-cli
   ```

3. <span data-ttu-id="2cce1-144">Se você não usa outros pacotes da Microsoft, remova a chave de assinatura da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="2cce1-144">If you don't use other Microsoft packages, remove the Microsoft signing key.</span></span>

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```

## <a name="next-steps"></a><span data-ttu-id="2cce1-145">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="2cce1-145">Next Steps</span></span>

<span data-ttu-id="2cce1-146">Agora que você instalou a CLI do Azure, faça um tour breve de seus recursos e comandos comuns.</span><span class="sxs-lookup"><span data-stu-id="2cce1-146">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="2cce1-147">Introdução à CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="2cce1-147">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)