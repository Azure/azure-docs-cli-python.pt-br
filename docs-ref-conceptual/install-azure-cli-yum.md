---
title: Instalar a CLI do Azure no Linux com yum
description: Como instalar a CLI do Azure com o yum
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 11/26/2019
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: ad773a58cf784c46a1c605e7e7eca58de8a4a722
ms.sourcegitcommit: 7caa6673f65e61deb8d6def6386e4eb9acdac923
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/28/2020
ms.locfileid: "77780104"
---
# <a name="install-azure-cli-with-yum"></a><span data-ttu-id="23d72-103">Instalar a CLI do Azure com o yum</span><span class="sxs-lookup"><span data-stu-id="23d72-103">Install Azure CLI with yum</span></span>

<span data-ttu-id="23d72-104">Para distribuições Linux com `yum`, como o RHEL, Fedora ou CentOS há um pacote para a CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="23d72-104">For Linux distributions with `yum` such as RHEL, Fedora, or CentOS, there's a package for the Azure CLI.</span></span> <span data-ttu-id="23d72-105">Este pacote foi testado com RHEL 7.7, RHEL 8, Fedora 24 e superior, CentOS 7 e CentOS 8.</span><span class="sxs-lookup"><span data-stu-id="23d72-105">This package has been tested with RHEL 7.7, RHEL 8, Fedora 24 and higher, CentOS 7 and CentOS 8.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

[!INCLUDE [rpm-warning](includes/rpm-warning.md)]

## <a name="install"></a><span data-ttu-id="23d72-106">Instalar</span><span class="sxs-lookup"><span data-stu-id="23d72-106">Install</span></span>

1. <span data-ttu-id="23d72-107">Importe a chave do repositório da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="23d72-107">Import the Microsoft repository key.</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="23d72-108">Crie informações sobre o repositório do local `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="23d72-108">Create local `azure-cli` repository information.</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]
   name=Azure CLI
   baseurl=https://packages.microsoft.com/yumrepos/azure-cli
   enabled=1
   gpgcheck=1
   gpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="23d72-109">Instale com o comando `yum install`.</span><span class="sxs-lookup"><span data-stu-id="23d72-109">Install with the `yum install` command.</span></span>

   ```bash
   sudo yum install azure-cli
   ```

<span data-ttu-id="23d72-110">Execute a CLI do Azure com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="23d72-110">Run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="23d72-111">Para entrar, use o comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="23d72-111">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="23d72-112">Para saber mais sobre os diferentes métodos de autenticação, confira [Entrar com a CLI do Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="23d72-112">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="23d72-113">Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="23d72-113">Troubleshooting</span></span>

<span data-ttu-id="23d72-114">Aqui estão alguns problemas comuns vistos durante a instalação com `yum`.</span><span class="sxs-lookup"><span data-stu-id="23d72-114">Here are some common problems seen when installing with `yum`.</span></span> <span data-ttu-id="23d72-115">Se você tiver um problema não abordado aqui, [arquive um problema no github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="23d72-115">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="install-on-rhel-76-or-other-systems-without-python-3"></a><span data-ttu-id="23d72-116">Instalar no RHEL 7.6 ou em outros sistemas sem Python 3</span><span class="sxs-lookup"><span data-stu-id="23d72-116">Install on RHEL 7.6 or other systems without Python 3</span></span>

<span data-ttu-id="23d72-117">Se puder, atualize seu sistema para uma versão com suporte oficial para o pacote `python3`.</span><span class="sxs-lookup"><span data-stu-id="23d72-117">If you can, please upgrade your system to a version with official support for `python3` package.</span></span> <span data-ttu-id="23d72-118">Caso contrário, você precisará instalar primeiro um pacote `python3`, ou [build da origem](https://github.com/linux-on-ibm-z/docs/wiki/Building-Python-3.6.x) ou instalar por meio de algum [repositório adicional](https://developers.redhat.com/blog/2018/08/13/install-python3-rhel/).</span><span class="sxs-lookup"><span data-stu-id="23d72-118">Otherwise, you need to first install a `python3` package, either [build from source](https://github.com/linux-on-ibm-z/docs/wiki/Building-Python-3.6.x) or install through some [additional repo](https://developers.redhat.com/blog/2018/08/13/install-python3-rhel/).</span></span> <span data-ttu-id="23d72-119">Em seguida, você poderá baixar o pacote e instalá-lo sem dependência.</span><span class="sxs-lookup"><span data-stu-id="23d72-119">Then you can download the package and install it without dependency.</span></span>
```bash
$ sudo yum install yum-utils
$ sudo yumdownloader azure-cli
$ sudo rpm -ivh --nodeps azure-cli-*.rpm
```

### <a name="proxy-blocks-connection"></a><span data-ttu-id="23d72-120">Conexão de blocos de proxy</span><span class="sxs-lookup"><span data-stu-id="23d72-120">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](includes/configure-proxy.md)]

<span data-ttu-id="23d72-121">Talvez você queira configurar explicitamente `yum` para usar esse proxy sempre.</span><span class="sxs-lookup"><span data-stu-id="23d72-121">You may also want to explicitly configure `yum` to use this proxy at all times.</span></span> <span data-ttu-id="23d72-122">Verifique se as linhas a seguir aparecem na seção `[main]` de `/etc/yum.conf`:</span><span class="sxs-lookup"><span data-stu-id="23d72-122">Make sure that the following lines appear under the `[main]` section of `/etc/yum.conf`:</span></span>

```yum.conf
[main]
# ...
proxy=http://[proxy]:[port] # If your proxy requires https, change http->https
proxy_username=[username] # Only required for basic auth
proxy_password=[password] # Only required for basic auth
```

<span data-ttu-id="23d72-123">Para obter a chave de assinatura da Microsoft e o pacote do nosso repositório, o proxy precisa permitir conexões HTTPS com o seguinte endereço:</span><span class="sxs-lookup"><span data-stu-id="23d72-123">In order to get the Microsoft signing key and get the package from our repository, your proxy needs to allow HTTPS connections to the following address:</span></span>

* `https://packages.microsoft.com`

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="23d72-124">Atualizar</span><span class="sxs-lookup"><span data-stu-id="23d72-124">Update</span></span>

<span data-ttu-id="23d72-125">Atualize a CLI do Azure com o comando `yum update`.</span><span class="sxs-lookup"><span data-stu-id="23d72-125">Update the Azure CLI with the `yum update` command.</span></span>

```bash
sudo yum update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="23d72-126">Desinstalar</span><span class="sxs-lookup"><span data-stu-id="23d72-126">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="23d72-127">Remova o pacote do seu sistema.</span><span class="sxs-lookup"><span data-stu-id="23d72-127">Remove the package from your system.</span></span>

   ```bash
   sudo yum remove azure-cli
   ```

2. <span data-ttu-id="23d72-128">Se você não pretende reinstalar a CLI, remova as informações do repositório.</span><span class="sxs-lookup"><span data-stu-id="23d72-128">If you don't plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="23d72-129">Se você não usa outros pacotes da Microsoft, remova a chave de assinatura.</span><span class="sxs-lookup"><span data-stu-id="23d72-129">If you don't use any other Microsoft packages, remove the signing key.</span></span>

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```

## <a name="next-steps"></a><span data-ttu-id="23d72-130">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="23d72-130">Next Steps</span></span>

<span data-ttu-id="23d72-131">Agora que você instalou a CLI do Azure, faça um tour breve de seus recursos e comandos comuns.</span><span class="sxs-lookup"><span data-stu-id="23d72-131">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="23d72-132">Introdução à CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="23d72-132">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
