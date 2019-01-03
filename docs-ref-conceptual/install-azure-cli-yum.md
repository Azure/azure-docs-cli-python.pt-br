---
title: Instalar a CLI do Azure no Linux com yum
description: Como instalar a CLI do Azure com o yum
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: faa1855efe9651ee104880740338c30e7dd84810
ms.sourcegitcommit: f40bd067ece4e6ec13e259782ed8db3e33b61a75
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "53593227"
---
# <a name="install-azure-cli-with-yum"></a><span data-ttu-id="9dda2-103">Instalar a CLI do Azure com o yum</span><span class="sxs-lookup"><span data-stu-id="9dda2-103">Install Azure CLI with yum</span></span>

<span data-ttu-id="9dda2-104">Para distribuições Linux com `yum`, como o RHEL, Fedora ou CentOS há um pacote para a CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="9dda2-104">For Linux distributions with  `yum` such as RHEL, Fedora, or CentOS, there's a package for the Azure CLI.</span></span> <span data-ttu-id="9dda2-105">Este pacote foi testado com RHEL 7, Fedora 19 e posterior e CentOS 7.</span><span class="sxs-lookup"><span data-stu-id="9dda2-105">This package has been tested with RHEL 7, Fedora 19 and higher, and CentOS 7.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a><span data-ttu-id="9dda2-106">Instalar</span><span class="sxs-lookup"><span data-stu-id="9dda2-106">Install</span></span>

1. <span data-ttu-id="9dda2-107">Importe a chave do repositório da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="9dda2-107">Import the Microsoft repository key.</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="9dda2-108">Crie informações sobre o repositório do local `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="9dda2-108">Create local `azure-cli` repository information.</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="9dda2-109">Instale com o comando `yum install`.</span><span class="sxs-lookup"><span data-stu-id="9dda2-109">Install with the `yum install` command.</span></span>

   ```bash
   sudo yum install azure-cli
   ```

<span data-ttu-id="9dda2-110">É possível executar a CLI do Azure com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="9dda2-110">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="9dda2-111">Para entrar, use o comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="9dda2-111">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="9dda2-112">Para saber mais sobre os diferentes métodos de autenticação, confira [Entrar com a CLI do Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="9dda2-112">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="9dda2-113">solução de problemas</span><span class="sxs-lookup"><span data-stu-id="9dda2-113">Troubleshooting</span></span>

<span data-ttu-id="9dda2-114">Aqui estão alguns problemas comuns vistos durante a instalação com `yum`.</span><span class="sxs-lookup"><span data-stu-id="9dda2-114">Here are some common problems seen when installing with `yum`.</span></span> <span data-ttu-id="9dda2-115">Se você tiver um problema não abordado aqui, [arquive um problema no github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="9dda2-115">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="9dda2-116">Atualizar</span><span class="sxs-lookup"><span data-stu-id="9dda2-116">Update</span></span>

<span data-ttu-id="9dda2-117">Atualize a CLI do Azure com o comando `yum update`.</span><span class="sxs-lookup"><span data-stu-id="9dda2-117">Update the Azure CLI with the `yum update` command.</span></span>

```bash
sudo yum update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="9dda2-118">Desinstalar</span><span class="sxs-lookup"><span data-stu-id="9dda2-118">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="9dda2-119">Remova o pacote do seu sistema.</span><span class="sxs-lookup"><span data-stu-id="9dda2-119">Remove the package from your system.</span></span>

   ```bash
   sudo yum remove azure-cli
   ```

2. <span data-ttu-id="9dda2-120">Se você não pretende reinstalar a CLI, remova as informações do repositório.</span><span class="sxs-lookup"><span data-stu-id="9dda2-120">If you don't plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="9dda2-121">Se você removeu as informações do repositório, remova também a chave de assinatura do Microsoft GPG.</span><span class="sxs-lookup"><span data-stu-id="9dda2-121">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```

## <a name="next-steps"></a><span data-ttu-id="9dda2-122">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="9dda2-122">Next Steps</span></span>

<span data-ttu-id="9dda2-123">Agora que você instalou a CLI do Azure, faça um tour breve de seus recursos e comandos comuns.</span><span class="sxs-lookup"><span data-stu-id="9dda2-123">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="9dda2-124">Introdução à CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="9dda2-124">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
