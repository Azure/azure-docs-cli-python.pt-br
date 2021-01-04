---
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 11/24/2020
ms.topic: include
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: d80970432a116656a33a3dc6c0d4909b4b92f312
ms.sourcegitcommit: d5f026468ea20bbd7ef35bdbf9852bcb2b812d83
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/23/2020
ms.locfileid: "97744590"
---
## <a name="overview"></a><span data-ttu-id="08e2f-101">Visão geral</span><span class="sxs-lookup"><span data-stu-id="08e2f-101">Overview</span></span>

<span data-ttu-id="08e2f-102">Para distribuições Linux com `zypper`, como o openSUSE ou SLES, há um pacote disponível para a CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="08e2f-102">For Linux distributions with `zypper`, such as openSUSE or SLES, there's a package available for the Azure CLI.</span></span> <span data-ttu-id="08e2f-103">Este pacote foi testado com openSUSE Leap 15.1 e SLES 15.</span><span class="sxs-lookup"><span data-stu-id="08e2f-103">This package has been tested with openSUSE Leap 15.1, and SLES 15.</span></span>

[!INCLUDE [current-version](current-version.md)]

[!INCLUDE [rpm-warning](rpm-warning.md)]

## <a name="install"></a><span data-ttu-id="08e2f-104">Instalar</span><span class="sxs-lookup"><span data-stu-id="08e2f-104">Install</span></span>

1. <span data-ttu-id="08e2f-105">Instale `curl`:</span><span class="sxs-lookup"><span data-stu-id="08e2f-105">Install `curl`:</span></span>

   ```bash
   sudo zypper install -y curl
   ```

2. <span data-ttu-id="08e2f-106">Importe a chave de repositório da Microsoft:</span><span class="sxs-lookup"><span data-stu-id="08e2f-106">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

3. <span data-ttu-id="08e2f-107">Crie informações sobre o repositório do `azure-cli` local:</span><span class="sxs-lookup"><span data-stu-id="08e2f-107">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo zypper addrepo --name 'Azure CLI' --check https://packages.microsoft.com/yumrepos/azure-cli azure-cli
   ```

4. <span data-ttu-id="08e2f-108">Atualize o índice de pacote do `zypper` e instale:</span><span class="sxs-lookup"><span data-stu-id="08e2f-108">Update the `zypper` package index and install:</span></span>

   ```bash
   sudo zypper install --from azure-cli azure-cli
   ```

   <span data-ttu-id="08e2f-109">Entrada 2 para continuar a instalar, ignorando algumas dependências.</span><span class="sxs-lookup"><span data-stu-id="08e2f-109">Input 2 to continue install by ignoring some of its dependencies.</span></span>

<span data-ttu-id="08e2f-110">É possível executar a CLI do Azure com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="08e2f-110">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="08e2f-111">Para entrar, use o comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="08e2f-111">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](interactive-login.md)]

<span data-ttu-id="08e2f-112">Para saber mais sobre os diferentes métodos de autenticação, confira [Entrar com a CLI do Azure](../authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="08e2f-112">To learn more about different authentication methods, see [Sign in with Azure CLI](../authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="08e2f-113">Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="08e2f-113">Troubleshooting</span></span>

<span data-ttu-id="08e2f-114">Aqui estão alguns problemas comuns vistos durante a instalação com `zypper`.</span><span class="sxs-lookup"><span data-stu-id="08e2f-114">Here are some common problems seen when installing with `zypper`.</span></span> <span data-ttu-id="08e2f-115">Se você tiver um problema não abordado aqui, [arquive um problema no GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="08e2f-115">If you experience a problem not covered here, [file an issue on GitHub](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="notimplementederror-on-opensuse-15-vm"></a><span data-ttu-id="08e2f-116">NotImplementedError na VM do OpenSUSE 15</span><span class="sxs-lookup"><span data-stu-id="08e2f-116">NotImplementedError on OpenSUSE 15 VM</span></span>
<span data-ttu-id="08e2f-117">A VM do OpenSUSE 15 tem uma CLI do Azure pré-instalada com a versão `2.0.45`, que está desatualizada e apresenta problemas com o comando `az login`.</span><span class="sxs-lookup"><span data-stu-id="08e2f-117">The OpenSUSE 15 VM has a pre-installed Azure CLI with version `2.0.45`, it's outdated and has issues with `az login`.</span></span> <span data-ttu-id="08e2f-118">Remova-a junto com as dependências antes de seguir as instruções de [instalação](#install) para adicionar a última CLI do Azure:</span><span class="sxs-lookup"><span data-stu-id="08e2f-118">Please remove it along with its dependencies before following the [Install](#install) instruction to add the latest Azure CLI:</span></span>

```bash
sudo zypper rm -y --clean-deps azure-cli
```

<span data-ttu-id="08e2f-119">Se você atualizou a CLI do Azure sem remover as dependências da versão `2.0.45`, as dependências antigas podem afetar a última versão da CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="08e2f-119">If you updated Azure CLI without removing the dependencies of version `2.0.45`, its old dependencies may affect the latest version of Azure CLI.</span></span> <span data-ttu-id="08e2f-120">Você precisará adicionar novamente a versão antiga para vinculá-la às dependências e remover a `azure-cli` junto com as dependências:</span><span class="sxs-lookup"><span data-stu-id="08e2f-120">You need to add back the old version to link to its dependencies and then remove `azure-cli` along with its dependencies:</span></span>

```bash
# The package name may vary on different system version, run 'zypper --no-refresh info azure-cli' to check the source package format
sudo zypper install --oldpackage azure-cli-2.0.45-4.22.noarch

sudo zypper rm -y --clean-deps azure-cli
```

### <a name="install-on-sles-12-or-other-systems-without-python-36"></a><span data-ttu-id="08e2f-121">Instalar no SLES 12 ou em sistemas sem o Python 3.6</span><span class="sxs-lookup"><span data-stu-id="08e2f-121">Install on SLES 12 or other systems without Python 3.6</span></span>

<span data-ttu-id="08e2f-122">No SLES 12, o pacote `python3` padrão é `3.4` e não é compatível com a CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="08e2f-122">On SLES 12, the default `python3` package is `3.4` and not supported by Azure CLI.</span></span> <span data-ttu-id="08e2f-123">Primeiro, siga as etapas 1 a 3 das [instruções de instalação](#install) para adicionar o repositório da `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="08e2f-123">You can first follow step 1-3 of the [install instruction](#install) to add the `azure-cli` repository.</span></span> <span data-ttu-id="08e2f-124">Em seguida, crie uma versão posterior do `python3` da origem.</span><span class="sxs-lookup"><span data-stu-id="08e2f-124">Then build a higher version `python3` from source.</span></span> <span data-ttu-id="08e2f-125">Por fim, você poderá baixar o pacote da CLI do Azure e instalá-lo sem nenhuma dependência.</span><span class="sxs-lookup"><span data-stu-id="08e2f-125">Finally, you can download the Azure CLI package and install it without dependency.</span></span>

<span data-ttu-id="08e2f-126">Use o seguinte comando para instalar a CLI do Azure (lembre-se de que a versão existente do Python 3 será substituída pelo Python 3.6):</span><span class="sxs-lookup"><span data-stu-id="08e2f-126">You can use the following one command to install Azure CLI (be aware that your existing Python 3 version will be overridden by Python 3.6):</span></span>

```bash
curl -sL https://azurecliprod.blob.core.windows.net/sles12_install.sh | sudo bash
```

<span data-ttu-id="08e2f-127">Ou, então, faça isso passo a passo:</span><span class="sxs-lookup"><span data-stu-id="08e2f-127">Or you can do it step by step:</span></span>

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

### <a name="proxy-blocks-connection"></a><span data-ttu-id="08e2f-128">Conexão de blocos de proxy</span><span class="sxs-lookup"><span data-stu-id="08e2f-128">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](configure-proxy.md)]

<span data-ttu-id="08e2f-129">Talvez você queira configurar explicitamente `zypper` (por meio de `yast2`) para usar esse proxy sempre.</span><span class="sxs-lookup"><span data-stu-id="08e2f-129">You may also want to explicitly configure `zypper` (via `yast2`) to use this proxy at all times.</span></span> <span data-ttu-id="08e2f-130">Para fazer isso, execute o comando `yast2 proxy` como superusuário e preencha as informações apresentadas no formulário.</span><span class="sxs-lookup"><span data-stu-id="08e2f-130">To do so, run the `yast2 proxy` command as superuser, and fill in the information presented in the form.</span></span> <span data-ttu-id="08e2f-131">Se você tiver um gerenciador de janelas disponível no sistema, também poderá usar o painel `Network Services > Proxy` no `YaST Control Center`.</span><span class="sxs-lookup"><span data-stu-id="08e2f-131">If you have a window manager available on your system, you can also use the `Network Services > Proxy` pane in the `YaST Control Center`.</span></span>

<span data-ttu-id="08e2f-132">Para configurações avançadas ou mais informações, confira a [documentação de configuração do Proxy do OpenSUSE](https://www.suse.com/documentation/slms1/book_slms/data/sec_wy_config_updates_proxy.html)</span><span class="sxs-lookup"><span data-stu-id="08e2f-132">For advanced configuration or more information, see the [OpenSUSE Proxy configuration documentation](https://www.suse.com/documentation/slms1/book_slms/data/sec_wy_config_updates_proxy.html)</span></span>

<span data-ttu-id="08e2f-133">Para obter a chave de assinatura da Microsoft e o pacote do nosso repositório, o proxy precisa permitir conexões HTTPS com os seguintes endereços:</span><span class="sxs-lookup"><span data-stu-id="08e2f-133">In order to get the Microsoft signing key and get the package from our repository, your proxy needs to allow HTTPS connections to the following addresses:</span></span>

* `https://packages.microsoft.com`
* `https://download.opensuse.org`

[!INCLUDE[troubleshoot-wsl.md](troubleshoot-wsl.md)]

### <a name="ssl-certificate-problem"></a><span data-ttu-id="08e2f-134">Problema com o certificado SSL</span><span class="sxs-lookup"><span data-stu-id="08e2f-134">SSL certificate problem</span></span>

<span data-ttu-id="08e2f-135">Quando um certificado é inválido ou está desatualizado em um computador, você pode receber um erro indicando que o cURL falhou ao verificar a legitimidade do servidor e, portanto, não foi possível estabelecer uma conexão segura.</span><span class="sxs-lookup"><span data-stu-id="08e2f-135">When a certificate is broken or outdated on a machine, you may receive an error indicating that curl failed to verify the legitimacy of the server and therefore could not establish a secure connection.</span></span>  <span data-ttu-id="08e2f-136">Atualize o certificado para corrigir o problema.</span><span class="sxs-lookup"><span data-stu-id="08e2f-136">Update your certificate to correct the problem.</span></span>  

```bach
sudo zypper update-ca-certificates
```

## <a name="update"></a><span data-ttu-id="08e2f-137">Atualizar</span><span class="sxs-lookup"><span data-stu-id="08e2f-137">Update</span></span>

[!INCLUDE [az-upgrade](az-upgrade.md)]

<span data-ttu-id="08e2f-138">Você também pode atualizar o pacote com o comando `zypper update`.</span><span class="sxs-lookup"><span data-stu-id="08e2f-138">You can also update the package with the `zypper update` command.</span></span>

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="08e2f-139">Desinstalar</span><span class="sxs-lookup"><span data-stu-id="08e2f-139">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](uninstall-boilerplate.md)]

1. <span data-ttu-id="08e2f-140">Remova o pacote do seu sistema.</span><span class="sxs-lookup"><span data-stu-id="08e2f-140">Remove the package from your system.</span></span>

    ```bash
    sudo zypper remove -y azure-cli
    ```

2. <span data-ttu-id="08e2f-141">Se você não pretende reinstalar a CLI, remova as informações do repositório.</span><span class="sxs-lookup"><span data-stu-id="08e2f-141">If you don't plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo zypper removerepo azure-cli
   ```

3. <span data-ttu-id="08e2f-142">Se você não usa outros pacotes da Microsoft, remova a chave de assinatura da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="08e2f-142">If you don't use other Microsoft packages, remove the Microsoft signing key.</span></span>

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```
