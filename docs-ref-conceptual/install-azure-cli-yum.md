---
title: Instalar a CLI do Azure no Linux com yum
description: Como instalar a CLI do Azure com o yum
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/25/2020
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 08ef942ace04f018d52cf1f6f7b20dc344953485
ms.sourcegitcommit: aa44ec97af5c0e7558d254b3159f95921e22ff1c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/01/2020
ms.locfileid: "91625356"
---
# <a name="install-azure-cli-with-yum"></a><span data-ttu-id="ea500-103">Instalar a CLI do Azure com o yum</span><span class="sxs-lookup"><span data-stu-id="ea500-103">Install Azure CLI with yum</span></span>

<span data-ttu-id="ea500-104">Para distribuições Linux com `yum`, como o RHEL, Fedora ou CentOS há um pacote para a CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="ea500-104">For Linux distributions with `yum` such as RHEL, Fedora, or CentOS, there's a package for the Azure CLI.</span></span> <span data-ttu-id="ea500-105">Este pacote foi testado com RHEL 7.7, RHEL 8, Fedora 24 e superior, CentOS 7 e CentOS 8.</span><span class="sxs-lookup"><span data-stu-id="ea500-105">This package has been tested with RHEL 7.7, RHEL 8, Fedora 24 and higher, CentOS 7 and CentOS 8.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

[!INCLUDE [rpm-warning](includes/rpm-warning.md)]

## <a name="install"></a><span data-ttu-id="ea500-106">Instalar</span><span class="sxs-lookup"><span data-stu-id="ea500-106">Install</span></span>

1. <span data-ttu-id="ea500-107">Importe a chave do repositório da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ea500-107">Import the Microsoft repository key.</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="ea500-108">Crie informações sobre o repositório do local `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="ea500-108">Create local `azure-cli` repository information.</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]
   name=Azure CLI
   baseurl=https://packages.microsoft.com/yumrepos/azure-cli
   enabled=1
   gpgcheck=1
   gpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="ea500-109">Instale com o comando `yum install`.</span><span class="sxs-lookup"><span data-stu-id="ea500-109">Install with the `yum install` command.</span></span>

   ```bash
   sudo yum install azure-cli
   ```

<span data-ttu-id="ea500-110">Execute a CLI do Azure com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="ea500-110">Run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="ea500-111">Para entrar, use o comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="ea500-111">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="ea500-112">Para saber mais sobre os diferentes métodos de autenticação, confira [Entrar com a CLI do Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="ea500-112">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="ea500-113">solução de problemas</span><span class="sxs-lookup"><span data-stu-id="ea500-113">Troubleshooting</span></span>

<span data-ttu-id="ea500-114">Aqui estão alguns problemas comuns vistos durante a instalação com `yum`.</span><span class="sxs-lookup"><span data-stu-id="ea500-114">Here are some common problems seen when installing with `yum`.</span></span> <span data-ttu-id="ea500-115">Se você tiver um problema não abordado aqui, [arquive um problema no github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="ea500-115">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="install-on-rhel-76-or-other-systems-without-python-3"></a><span data-ttu-id="ea500-116">Instalar no RHEL 7.6 ou em outros sistemas sem Python 3</span><span class="sxs-lookup"><span data-stu-id="ea500-116">Install on RHEL 7.6 or other systems without Python 3</span></span>

<span data-ttu-id="ea500-117">Se puder, atualize seu sistema para uma versão com suporte oficial para o pacote `python3`.</span><span class="sxs-lookup"><span data-stu-id="ea500-117">If you can, please upgrade your system to a version with official support for `python3` package.</span></span> <span data-ttu-id="ea500-118">Caso contrário, você precisará instalar primeiro um pacote `python3`, ou [build da origem](https://github.com/linux-on-ibm-z/docs/wiki/Building-Python-3.6.x) ou instalar por meio de algum [repositório adicional](https://developers.redhat.com/blog/2018/08/13/install-python3-rhel/).</span><span class="sxs-lookup"><span data-stu-id="ea500-118">Otherwise, you need to first install a `python3` package, either [build from source](https://github.com/linux-on-ibm-z/docs/wiki/Building-Python-3.6.x) or install through some [additional repo](https://developers.redhat.com/blog/2018/08/13/install-python3-rhel/).</span></span> <span data-ttu-id="ea500-119">Em seguida, você poderá baixar o pacote e instalá-lo sem dependência.</span><span class="sxs-lookup"><span data-stu-id="ea500-119">Then you can download the package and install it without dependency.</span></span>
```bash
$ sudo yum install yum-utils
$ sudo yumdownloader azure-cli
$ sudo rpm -ivh --nodeps azure-cli-*.rpm
```

<span data-ttu-id="ea500-120">Se você instalou o python3 mas ainda está tendo um erro `python3: command not found` ao tentar executar o CLI, você precisa adicioná-lo ao seu caminho.</span><span class="sxs-lookup"><span data-stu-id="ea500-120">If you have setup python3 but are still getting an error `python3: command not found` when trying to run the cli, you need to add it to your path.</span></span>
```bash
$ scl enable rh-python36 bash
```

### <a name="proxy-blocks-connection"></a><span data-ttu-id="ea500-121">Conexão de blocos de proxy</span><span class="sxs-lookup"><span data-stu-id="ea500-121">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](includes/configure-proxy.md)]

<span data-ttu-id="ea500-122">Talvez você queira configurar explicitamente `yum` para usar esse proxy sempre.</span><span class="sxs-lookup"><span data-stu-id="ea500-122">You may also want to explicitly configure `yum` to use this proxy at all times.</span></span> <span data-ttu-id="ea500-123">Verifique se as linhas a seguir aparecem na seção `[main]` de `/etc/yum.conf`:</span><span class="sxs-lookup"><span data-stu-id="ea500-123">Make sure that the following lines appear under the `[main]` section of `/etc/yum.conf`:</span></span>

```yum.conf
[main]
# ...
proxy=http://[proxy]:[port] # If your proxy requires https, change http->https
proxy_username=[username] # Only required for basic auth
proxy_password=[password] # Only required for basic auth
```

<span data-ttu-id="ea500-124">Para obter a chave de assinatura da Microsoft e o pacote do nosso repositório, o proxy precisa permitir conexões HTTPS com o seguinte endereço:</span><span class="sxs-lookup"><span data-stu-id="ea500-124">In order to get the Microsoft signing key and get the package from our repository, your proxy needs to allow HTTPS connections to the following address:</span></span>

* `https://packages.microsoft.com`

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="ea500-125">Atualizar</span><span class="sxs-lookup"><span data-stu-id="ea500-125">Update</span></span>

[!INCLUDE [az-upgrade](includes/az-upgrade.md)]

<span data-ttu-id="ea500-126">Você também pode atualizar a CLI do Azure com o comando `yum update`.</span><span class="sxs-lookup"><span data-stu-id="ea500-126">You can also update the Azure CLI with the `yum update` command.</span></span>

```bash
sudo yum update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="ea500-127">Desinstalar</span><span class="sxs-lookup"><span data-stu-id="ea500-127">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="ea500-128">Remova o pacote do seu sistema.</span><span class="sxs-lookup"><span data-stu-id="ea500-128">Remove the package from your system.</span></span>

   ```bash
   sudo yum remove azure-cli
   ```

2. <span data-ttu-id="ea500-129">Se você não pretende reinstalar a CLI, remova as informações do repositório.</span><span class="sxs-lookup"><span data-stu-id="ea500-129">If you don't plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="ea500-130">Se você não usa outros pacotes da Microsoft, remova a chave de assinatura.</span><span class="sxs-lookup"><span data-stu-id="ea500-130">If you don't use any other Microsoft packages, remove the signing key.</span></span>

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```

## <a name="next-steps"></a><span data-ttu-id="ea500-131">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="ea500-131">Next Steps</span></span>

<span data-ttu-id="ea500-132">Agora que você instalou a CLI do Azure, faça um tour breve de seus recursos e comandos comuns.</span><span class="sxs-lookup"><span data-stu-id="ea500-132">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="ea500-133">Introdução à CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="ea500-133">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)