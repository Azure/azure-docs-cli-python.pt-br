---
title: Instalar a CLI do Azure no Linux com yum
description: Como instalar a CLI do Azure com o yum
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 11/24/2020
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 9053140a35c7bc1443a636d4150ee8f0ee94dba9
ms.sourcegitcommit: 05b58a872cdd165805df62614000637144d80066
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "96470445"
---
# <a name="install-azure-cli-with-yum"></a><span data-ttu-id="5f16a-103">Instalar a CLI do Azure com o yum</span><span class="sxs-lookup"><span data-stu-id="5f16a-103">Install Azure CLI with yum</span></span>

<span data-ttu-id="5f16a-104">Para distribuições Linux com `yum`, como o RHEL, Fedora ou CentOS há um pacote para a CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="5f16a-104">For Linux distributions with `yum` such as RHEL, Fedora, or CentOS, there's a package for the Azure CLI.</span></span> <span data-ttu-id="5f16a-105">Este pacote foi testado com RHEL 7.7, RHEL 8, Fedora 24 e superior, CentOS 7 e CentOS 8.</span><span class="sxs-lookup"><span data-stu-id="5f16a-105">This package has been tested with RHEL 7.7, RHEL 8, Fedora 24 and higher, CentOS 7 and CentOS 8.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

[!INCLUDE [rpm-warning](includes/rpm-warning.md)]

## <a name="install"></a><span data-ttu-id="5f16a-106">Instalar</span><span class="sxs-lookup"><span data-stu-id="5f16a-106">Install</span></span>

1. <span data-ttu-id="5f16a-107">Importe a chave do repositório da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="5f16a-107">Import the Microsoft repository key.</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="5f16a-108">Crie informações sobre o repositório do local `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="5f16a-108">Create local `azure-cli` repository information.</span></span>

   ```bash
   echo -e "[azure-cli]
   name=Azure CLI
   baseurl=https://packages.microsoft.com/yumrepos/azure-cli
   enabled=1
   gpgcheck=1
   gpgkey=https://packages.microsoft.com/keys/microsoft.asc" | sudo tee /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="5f16a-109">Instale com o comando `yum install`.</span><span class="sxs-lookup"><span data-stu-id="5f16a-109">Install with the `yum install` command.</span></span>

   ```bash
   sudo yum install azure-cli
   ```

<span data-ttu-id="5f16a-110">Execute a CLI do Azure com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="5f16a-110">Run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="5f16a-111">Para entrar, use o comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="5f16a-111">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="5f16a-112">Para saber mais sobre os diferentes métodos de autenticação, confira [Entrar com a CLI do Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="5f16a-112">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="5f16a-113">solução de problemas</span><span class="sxs-lookup"><span data-stu-id="5f16a-113">Troubleshooting</span></span>

<span data-ttu-id="5f16a-114">Aqui estão alguns problemas comuns vistos durante a instalação com `yum`.</span><span class="sxs-lookup"><span data-stu-id="5f16a-114">Here are some common problems seen when installing with `yum`.</span></span> <span data-ttu-id="5f16a-115">Se você tiver um problema não abordado aqui, [arquive um problema no github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="5f16a-115">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="install-on-rhel-76-or-other-systems-without-python-3"></a><span data-ttu-id="5f16a-116">Instalar no RHEL 7.6 ou em outros sistemas sem Python 3</span><span class="sxs-lookup"><span data-stu-id="5f16a-116">Install on RHEL 7.6 or other systems without Python 3</span></span>

<span data-ttu-id="5f16a-117">Se puder, atualize seu sistema para uma versão com suporte oficial para o pacote `python 3.6+`.</span><span class="sxs-lookup"><span data-stu-id="5f16a-117">If you can, please upgrade your system to a version with official support for `python 3.6+` package.</span></span> <span data-ttu-id="5f16a-118">Caso contrário, primeiro, você precisará instalar um pacote do `python3` e instalar a CLI do Azure sem nenhuma dependência.</span><span class="sxs-lookup"><span data-stu-id="5f16a-118">Otherwise, you need to first install a `python3` package then install Azure CLI without dependency.</span></span> 

<span data-ttu-id="5f16a-119">Use o seguinte comando para instalar a CLI do Azure com o `python 3.6` compilado da origem:</span><span class="sxs-lookup"><span data-stu-id="5f16a-119">You can use the following one command to install Azure CLI with `python 3.6` built from source:</span></span>
```bash
curl -sL https://azurecliprod.blob.core.windows.net/rhel7_6_install.sh | sudo bash
```
<span data-ttu-id="5f16a-120">Faça isso também passo a passo:</span><span class="sxs-lookup"><span data-stu-id="5f16a-120">You can also do it step by step:</span></span>

<span data-ttu-id="5f16a-121">Primeiro, a CLI do Azure exige o `SSL 1.1+` e você precisará criar o `openssl 1.1` da origem antes de compilar o `python3`:</span><span class="sxs-lookup"><span data-stu-id="5f16a-121">First, Azure CLI requires `SSL 1.1+` and you need to build `openssl 1.1` from source before building `python3`:</span></span>
```bash
$ sudo yum install gcc gcc-c++ make ncurses patch wget tar zlib zlib-devel -y
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

<span data-ttu-id="5f16a-122">Em seguida, crie o Python 3 da origem:</span><span class="sxs-lookup"><span data-stu-id="5f16a-122">Then build Python 3 from source:</span></span>
```bash
$ PYTHON_VERSION="3.6.9"
$ PYTHON_SRC_DIR=$(mktemp -d)
$ wget -qO- https://www.python.org/ftp/python/$PYTHON_VERSION/Python-$PYTHON_VERSION.tgz | tar -xz -C "$PYTHON_SRC_DIR"
$ cd $PYTHON_SRC_DIR/Python-$PYTHON_VERSION
$ ./configure --prefix=/usr --with-openssl=/usr/local/ssl
$ make
$ sudo make install
```

<span data-ttu-id="5f16a-123">Por fim, siga as etapas 1 e 2 das [instruções de instalação](#install) para adicionar o repositório da CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="5f16a-123">Finally, follow step 1 and 2 of the [install instruction](#install) to add Azure CLI repository.</span></span> <span data-ttu-id="5f16a-124">Agora, você pode baixar o pacote e instalá-lo sem nenhuma dependência.</span><span class="sxs-lookup"><span data-stu-id="5f16a-124">You can now download the package and install it without dependency.</span></span>
```bash
$ sudo yum install yum-utils -y
$ sudo yumdownloader azure-cli
$ sudo rpm -ivh --nodeps azure-cli-*.rpm
```

<span data-ttu-id="5f16a-125">Como alternativa, você também pode instalar o Python 3 por meio de um [repositório adicional](https://developers.redhat.com/blog/2018/08/13/install-python3-rhel/).</span><span class="sxs-lookup"><span data-stu-id="5f16a-125">As an alternative, you can also install Python 3 through some [additional repo](https://developers.redhat.com/blog/2018/08/13/install-python3-rhel/).</span></span> <span data-ttu-id="5f16a-126">Seguindo esse procedimento, se você configurou o `python3` mas ainda está recebendo um erro do `python3: command not found` ao tentar executar a CLI, adicione-o ao caminho.</span><span class="sxs-lookup"><span data-stu-id="5f16a-126">Following this way, if you have set up `python3` but are still getting an error `python3: command not found` when trying to run the cli, you need to add it to your path.</span></span>
```bash
$ scl enable rh-python36 bash
```

### <a name="proxy-blocks-connection"></a><span data-ttu-id="5f16a-127">Conexão de blocos de proxy</span><span class="sxs-lookup"><span data-stu-id="5f16a-127">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](includes/configure-proxy.md)]

<span data-ttu-id="5f16a-128">Talvez você queira configurar explicitamente `yum` para usar esse proxy sempre.</span><span class="sxs-lookup"><span data-stu-id="5f16a-128">You may also want to explicitly configure `yum` to use this proxy at all times.</span></span> <span data-ttu-id="5f16a-129">Verifique se as linhas a seguir aparecem na seção `[main]` de `/etc/yum.conf`:</span><span class="sxs-lookup"><span data-stu-id="5f16a-129">Make sure that the following lines appear under the `[main]` section of `/etc/yum.conf`:</span></span>

```yum.conf
[main]
# ...
proxy=http://[proxy]:[port] # If your proxy requires https, change http->https
proxy_username=[username] # Only required for basic auth
proxy_password=[password] # Only required for basic auth
```

<span data-ttu-id="5f16a-130">Para obter a chave de assinatura da Microsoft e o pacote do nosso repositório, o proxy precisa permitir conexões HTTPS com o seguinte endereço:</span><span class="sxs-lookup"><span data-stu-id="5f16a-130">In order to get the Microsoft signing key and get the package from our repository, your proxy needs to allow HTTPS connections to the following address:</span></span>

* `https://packages.microsoft.com`

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="5f16a-131">Atualizar</span><span class="sxs-lookup"><span data-stu-id="5f16a-131">Update</span></span>

[!INCLUDE [az-upgrade](includes/az-upgrade.md)]

<span data-ttu-id="5f16a-132">Você também pode atualizar a CLI do Azure com o comando `yum update`.</span><span class="sxs-lookup"><span data-stu-id="5f16a-132">You can also update the Azure CLI with the `yum update` command.</span></span>

```bash
sudo yum update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="5f16a-133">Desinstalar</span><span class="sxs-lookup"><span data-stu-id="5f16a-133">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="5f16a-134">Remova o pacote do seu sistema.</span><span class="sxs-lookup"><span data-stu-id="5f16a-134">Remove the package from your system.</span></span>

   ```bash
   sudo yum remove azure-cli
   ```

2. <span data-ttu-id="5f16a-135">Se você não pretende reinstalar a CLI, remova as informações do repositório.</span><span class="sxs-lookup"><span data-stu-id="5f16a-135">If you don't plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="5f16a-136">Se você não usa outros pacotes da Microsoft, remova a chave de assinatura.</span><span class="sxs-lookup"><span data-stu-id="5f16a-136">If you don't use any other Microsoft packages, remove the signing key.</span></span>

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```

## <a name="next-steps"></a><span data-ttu-id="5f16a-137">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="5f16a-137">Next Steps</span></span>

<span data-ttu-id="5f16a-138">Agora que você instalou a CLI do Azure, faça um tour breve de seus recursos e comandos comuns.</span><span class="sxs-lookup"><span data-stu-id="5f16a-138">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="5f16a-139">Introdução à CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="5f16a-139">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
