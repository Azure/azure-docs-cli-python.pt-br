---
title: Instalar a CLI do Azure 2.0 com o yum
description: Como instalar a CLI do Azure 2.0 com o yum
keywords: CLI do Azure, Instalar CLI do Azure, yum do azure, rhel do azure, fedora do azure, centos do azure
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 11/01/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ROBOTS: NOINDEX,NOFOLLOW
ms.openlocfilehash: f0d5effcd8315094b30050a35119e41eddf89961
ms.sourcegitcommit: 2e4d0bdd94c626e061434883032367b5619de4fe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2017
---
# <a name="install-azure-cli-20-with-yum"></a><span data-ttu-id="b9c0a-104">Instalar CLI do Azure 2.0 com o yum</span><span class="sxs-lookup"><span data-stu-id="b9c0a-104">Install Azure CLI 2.0 with yum</span></span>

<span data-ttu-id="b9c0a-105">Se você estiver executando uma distribuição que vem com o `yum`, como o RHEL, Fedora ou CentOS, há um pacote disponível para a CLI do Azure que pode ser instalado em seu sistema.</span><span class="sxs-lookup"><span data-stu-id="b9c0a-105">If you are running a distirbution that comes with `yum`, such as RHEL, Fedora, or CentOS, there is an available package for the Azure CLI that you can install on your system.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a><span data-ttu-id="b9c0a-106">Instalar</span><span class="sxs-lookup"><span data-stu-id="b9c0a-106">Install</span></span>

1. <span data-ttu-id="b9c0a-107">Importe a chave de repositório da Microsoft:</span><span class="sxs-lookup"><span data-stu-id="b9c0a-107">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="b9c0a-108">Crie informações sobre o repositório do `azure-cli` local:</span><span class="sxs-lookup"><span data-stu-id="b9c0a-108">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="b9c0a-109">Atualize o índice de pacote do `yum` e instale:</span><span class="sxs-lookup"><span data-stu-id="b9c0a-109">Update the `yum` package index and install:</span></span>

   ```bash
   yum check-update
   sudo yum install azure-cli
   ```

<span data-ttu-id="b9c0a-110">Execute a CLI do Azure com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="b9c0a-110">Run the Azure CLI with the `az` command.</span></span>

## <a name="update"></a><span data-ttu-id="b9c0a-111">Atualização</span><span class="sxs-lookup"><span data-stu-id="b9c0a-111">Update</span></span>

<span data-ttu-id="b9c0a-112">Atualize a CLI do Azure com o comando `yum update`.</span><span class="sxs-lookup"><span data-stu-id="b9c0a-112">Update the Azure CLI with the `yum update` command.</span></span>

```bash
yum check-update
sudo yum update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="b9c0a-113">Desinstalar</span><span class="sxs-lookup"><span data-stu-id="b9c0a-113">Uninstall</span></span>

<span data-ttu-id="b9c0a-114">Se você decidiu desinstalar a CLI do Azure, lamentamos sua saída.</span><span class="sxs-lookup"><span data-stu-id="b9c0a-114">If you ever decide to uninstall the Azure CLI, we're sorry to see you go.</span></span> <span data-ttu-id="b9c0a-115">Antes de desinstalar, use o comando `az feedback` para nos fornecer algumas razões por ter escolhido desinstalar e como poderíamos melhorar a experiência da CLI.</span><span class="sxs-lookup"><span data-stu-id="b9c0a-115">Before you uninstall, use the `az feedback` command to give us some reasons why you chose to uninstall and how we could improve the CLI experience.</span></span> <span data-ttu-id="b9c0a-116">Queremos assegurar que a CLI do Azure não tenha bugs e seja amigável o máximo possível.</span><span class="sxs-lookup"><span data-stu-id="b9c0a-116">We want to make sure that the Azure CLI is as bug-free and user-friendly as we can make it.</span></span> <span data-ttu-id="b9c0a-117">Você também pode [registrar um problema do github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="b9c0a-117">You can also [file a github issue](https://github.com/Azure/azure-cli/issues).</span></span>

1. <span data-ttu-id="b9c0a-118">Remova o pacote do seu sistema.</span><span class="sxs-lookup"><span data-stu-id="b9c0a-118">Remove the package from your system.</span></span>

   ```bash
   sudo yum remove azure-cli
   ```

2. <span data-ttu-id="b9c0a-119">Se você não pretende reinstalar a CLI, remova as informações do repositório.</span><span class="sxs-lookup"><span data-stu-id="b9c0a-119">If you do not plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="b9c0a-120">Se você removeu as informações do repositório, remova também a chave de assinatura do Microsoft GPG.</span><span class="sxs-lookup"><span data-stu-id="b9c0a-120">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```
