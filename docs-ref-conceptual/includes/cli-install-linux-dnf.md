---
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 11/24/2020
ms.topic: include
ms.custom: devx-track-azurecli
ms.openlocfilehash: c0de92ff9aed581d192d72ca920fafea8bbd192b
ms.sourcegitcommit: 594e9c620a6f74f5eaedf91a7f6a791e03a64c74
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2021
ms.locfileid: "100630992"
---
## <a name="overview"></a><span data-ttu-id="f57fc-101">Visão geral</span><span class="sxs-lookup"><span data-stu-id="f57fc-101">Overview</span></span>

<span data-ttu-id="f57fc-102">Para distribuições Linux com `dnf`, como o RHEL, Fedora ou CentOS há um pacote para a CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="f57fc-102">For Linux distributions with `dnf` such as RHEL, Fedora, or CentOS, there's a package for the Azure CLI.</span></span> <span data-ttu-id="f57fc-103">Este pacote foi testado com RHEL 7.7, RHEL 8, Fedora 24 e superior, CentOS 7 e CentOS 8.</span><span class="sxs-lookup"><span data-stu-id="f57fc-103">This package has been tested with RHEL 7.7, RHEL 8, Fedora 24 and higher, CentOS 7 and CentOS 8.</span></span>

[!INCLUDE [current-version](current-version.md)]

[!INCLUDE [rpm-warning](rpm-warning.md)]

> [!NOTE]
>
> <span data-ttu-id="f57fc-104">Use o gerenciador de pacotes `yum` se você estiver utilizando sistemas Linux que não dão suporte ao gerenciador de pacotes `dnf`.</span><span class="sxs-lookup"><span data-stu-id="f57fc-104">Use `yum` package manager if you are using Linux systems that don't support `dnf` package manager.</span></span>

## <a name="install"></a><span data-ttu-id="f57fc-105">Instalar</span><span class="sxs-lookup"><span data-stu-id="f57fc-105">Install</span></span>

1. <span data-ttu-id="f57fc-106">Importe a chave do repositório da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="f57fc-106">Import the Microsoft repository key.</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="f57fc-107">Crie informações sobre o repositório do local `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="f57fc-107">Create local `azure-cli` repository information.</span></span>

   ```bash
   echo -e "[azure-cli]
   name=Azure CLI
   baseurl=https://packages.microsoft.com/yumrepos/azure-cli
   enabled=1
   gpgcheck=1
   gpgkey=https://packages.microsoft.com/keys/microsoft.asc" | sudo tee /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="f57fc-108">Instale com o comando `dnf install`.</span><span class="sxs-lookup"><span data-stu-id="f57fc-108">Install with the `dnf install` command.</span></span>

   ```bash
   sudo dnf install azure-cli
   ```
 
<span data-ttu-id="f57fc-109">Execute a CLI do Azure com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="f57fc-109">Run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="f57fc-110">Para entrar, use o comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="f57fc-110">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>


[!INCLUDE [interactive-login](interactive-login.md)]

<span data-ttu-id="f57fc-111">Para saber mais sobre os diferentes métodos de autenticação, confira [Entrar com a CLI do Azure](../authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="f57fc-111">To learn more about different authentication methods, see [Sign in with Azure CLI](../authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="f57fc-112">Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="f57fc-112">Troubleshooting</span></span>

<span data-ttu-id="f57fc-113">Aqui estão alguns problemas comuns vistos durante a instalação com `dnf`.</span><span class="sxs-lookup"><span data-stu-id="f57fc-113">Here are some common problems seen when installing with `dnf`.</span></span> <span data-ttu-id="f57fc-114">Se você tiver um problema não abordado aqui, [arquive um problema no GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="f57fc-114">If you experience a problem not covered here, [file an issue on GitHub](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="install-on-rhel-76-or-other-systems-without-python-3"></a><span data-ttu-id="f57fc-115">Instalar no RHEL 7.6 ou em outros sistemas sem Python 3</span><span class="sxs-lookup"><span data-stu-id="f57fc-115">Install on RHEL 7.6 or other systems without Python 3</span></span>

<span data-ttu-id="f57fc-116">Se puder, atualize seu sistema para uma versão com suporte oficial para o pacote `python 3.6+`.</span><span class="sxs-lookup"><span data-stu-id="f57fc-116">If you can, please upgrade your system to a version with official support for `python 3.6+` package.</span></span> <span data-ttu-id="f57fc-117">Caso contrário, primeiro, você precisará instalar um pacote do `python3` e instalar a CLI do Azure sem nenhuma dependência.</span><span class="sxs-lookup"><span data-stu-id="f57fc-117">Otherwise, you need to first install a `python3` package then install Azure CLI without dependency.</span></span>

<span data-ttu-id="f57fc-118">Use o seguinte comando para instalar a CLI do Azure com o `python 3.6` compilado da origem:</span><span class="sxs-lookup"><span data-stu-id="f57fc-118">You can use the following one command to install Azure CLI with `python 3.6` built from source:</span></span>

```bash
curl -sL https://azurecliprod.blob.core.windows.net/rhel7_6_install.sh | sudo bash
```

<span data-ttu-id="f57fc-119">Faça isso também passo a passo:</span><span class="sxs-lookup"><span data-stu-id="f57fc-119">You can also do it step by step:</span></span>

<span data-ttu-id="f57fc-120">Primeiro, a CLI do Azure exige o `SSL 1.1+` e você precisará criar o `openssl 1.1` da origem antes de compilar o `python3`:</span><span class="sxs-lookup"><span data-stu-id="f57fc-120">First, Azure CLI requires `SSL 1.1+` and you need to build `openssl 1.1` from source before building `python3`:</span></span>

```bash
$ sudo dnf install gcc gcc-c++ make ncurses patch wget tar zlib zlib-devel -y
# build openssl from source
$ cd ~
$ wget https://www.openssl.org/source/openssl-1.1.1d.tar.gz
$ tar -xzf openssl-1.1.1d.tar.gz
$ cd openssl-1.1.1d
$ ./config --prefix=/usr/local/ssl --openssldir=/usr/local/ssl
$ make
$ sudo make install
# configure shared object lookup directory so that libssl.so.1.1 can be found
$ echo "/usr/local/ssl/lib" | sudo tee /etc/ld.so.conf.d/openssl-1.1.1d.conf
# reload config
$ sudo ldconfig -v
```

<span data-ttu-id="f57fc-121">Em seguida, crie o Python 3 da origem:</span><span class="sxs-lookup"><span data-stu-id="f57fc-121">Then build Python 3 from source:</span></span>

```bash
$ PYTHON_VERSION="3.6.9"
$ PYTHON_SRC_DIR=$(mktemp -d)
$ wget -qO- https://www.python.org/ftp/python/$PYTHON_VERSION/Python-$PYTHON_VERSION.tgz | tar -xz -C "$PYTHON_SRC_DIR"
$ cd $PYTHON_SRC_DIR/Python-$PYTHON_VERSION
$ ./configure --prefix=/usr --with-openssl=/usr/local/ssl
$ make
$ sudo make install
```

<span data-ttu-id="f57fc-122">Por fim, siga as etapas 1 e 2 das [instruções de instalação](#install) para adicionar o repositório da CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="f57fc-122">Finally, follow step 1 and 2 of the [install instruction](#install) to add Azure CLI repository.</span></span> <span data-ttu-id="f57fc-123">Agora, você pode baixar o pacote e instalá-lo sem nenhuma dependência.</span><span class="sxs-lookup"><span data-stu-id="f57fc-123">You can now download the package and install it without dependency.</span></span>

> [!NOTE]
>
> <span data-ttu-id="f57fc-124">Caso você não tenha o plug-in de download do dnf instalado, um erro de comando não encontrado será exibido durante a execução do código abaixo.</span><span class="sxs-lookup"><span data-stu-id="f57fc-124">In case you don't have the dnf download plugin installed, you will encounter command not found error on executing the below code.</span></span> <span data-ttu-id="f57fc-125">Use `dnf install 'dnf-command(download)'` para instalar o plug-in de download do dnf.</span><span class="sxs-lookup"><span data-stu-id="f57fc-125">Use `dnf install 'dnf-command(download)'` to   install the dnf download plugin.</span></span>

```bash
$ sudo dnf download azure-cli
$ sudo rpm -ivh --nodeps azure-cli-*.rpm
```

<span data-ttu-id="f57fc-126">Como alternativa, você também pode instalar o Python 3 por meio de um [repositório adicional](https://developers.redhat.com/blog/2018/08/13/install-python3-rhel/).</span><span class="sxs-lookup"><span data-stu-id="f57fc-126">As an alternative, you can also install Python 3 through some [additional repo](https://developers.redhat.com/blog/2018/08/13/install-python3-rhel/).</span></span> <span data-ttu-id="f57fc-127">Seguindo esse procedimento, se você configurou o `python3` mas ainda está recebendo um erro do `python3: command not found` ao tentar executar a CLI, adicione-o ao caminho.</span><span class="sxs-lookup"><span data-stu-id="f57fc-127">Following this way, if you have set up `python3` but are still getting an error `python3: command not found` when trying to run the cli, you need to add it to your path.</span></span>

```bash
$ scl enable rh-python36 bash
```

### <a name="proxy-blocks-connection"></a><span data-ttu-id="f57fc-128">Conexão de blocos de proxy</span><span class="sxs-lookup"><span data-stu-id="f57fc-128">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](configure-proxy.md)]

<span data-ttu-id="f57fc-129">Talvez você queira configurar explicitamente `dnf` para usar esse proxy sempre.</span><span class="sxs-lookup"><span data-stu-id="f57fc-129">You may also want to explicitly configure `dnf` to use this proxy at all times.</span></span> <span data-ttu-id="f57fc-130">Verifique se as linhas a seguir aparecem na seção `[main]` de `/etc/dnf/dnf.conf`:</span><span class="sxs-lookup"><span data-stu-id="f57fc-130">Make sure that the following lines appear under the `[main]` section of `/etc/dnf/dnf.conf`:</span></span>

```dnf.conf
[main]
# ...
proxy=http://[proxy]:[port] # If your proxy requires https, change http->https
proxy_username=[username] # Only required for basic auth
proxy_password=[password] # Only required for basic auth
```

<span data-ttu-id="f57fc-131">Para obter a chave de assinatura da Microsoft e o pacote do nosso repositório, o proxy precisa permitir conexões HTTPS com o seguinte endereço:</span><span class="sxs-lookup"><span data-stu-id="f57fc-131">In order to get the Microsoft signing key and get the package from our repository, your proxy needs to allow HTTPS connections to the following address:</span></span>

* `https://packages.microsoft.com`

[!INCLUDE[troubleshoot-wsl.md](troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="f57fc-132">Atualizar</span><span class="sxs-lookup"><span data-stu-id="f57fc-132">Update</span></span>

[!INCLUDE [az-upgrade](az-upgrade.md)]

<span data-ttu-id="f57fc-133">Você também pode atualizar a CLI do Azure com o comando `dnf update`.</span><span class="sxs-lookup"><span data-stu-id="f57fc-133">You can also update the Azure CLI with the `dnf update` command.</span></span>

```bash
sudo dnf update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="f57fc-134">Desinstalar</span><span class="sxs-lookup"><span data-stu-id="f57fc-134">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](uninstall-boilerplate.md)]

1. <span data-ttu-id="f57fc-135">Remova o pacote do seu sistema.</span><span class="sxs-lookup"><span data-stu-id="f57fc-135">Remove the package from your system.</span></span>

   ```bash
   sudo dnf remove azure-cli
   ```

2. <span data-ttu-id="f57fc-136">Se você não pretende reinstalar a CLI, remova as informações do repositório.</span><span class="sxs-lookup"><span data-stu-id="f57fc-136">If you don't plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="f57fc-137">Se você não usa outros pacotes da Microsoft, remova a chave de assinatura.</span><span class="sxs-lookup"><span data-stu-id="f57fc-137">If you don't use any other Microsoft packages, remove the signing key.</span></span>

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```
