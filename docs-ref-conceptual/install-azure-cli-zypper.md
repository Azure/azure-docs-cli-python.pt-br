---
title: Instalar a CLI do Azure 2.0 com o zypper
description: Como instalar a CLI do Azure 2.0 com o zypper
keywords: cli do azure, instalar cli do azure, zypper cli do azure, opensuse cli do azure, sle cli do azure
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
ms.openlocfilehash: 6b9a97e73f45c8271f1e8f19d5a8cf5f9f748d07
ms.sourcegitcommit: 3eef136ae752eb90c67af604d4ddd298d70b1c9d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/06/2018
---
# <a name="install-azure-cli-20-with-zypper"></a><span data-ttu-id="2ceb4-104">Instalar CLI do Azure 2.0 com zypper</span><span class="sxs-lookup"><span data-stu-id="2ceb4-104">Install Azure CLI 2.0 with zypper</span></span>

<span data-ttu-id="2ceb4-105">Se você estiver executando uma distribuição que vem com o `zypper`, como o OpenSUSE ou SLE, há um pacote disponível para a CLI do Azure que pode ser instalado em seu sistema.</span><span class="sxs-lookup"><span data-stu-id="2ceb4-105">If you are running a distirbution that comes with `zypper`, such as OpenSUSE or SLE, there is an available package for the Azure CLI that you can install on your system.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a><span data-ttu-id="2ceb4-106">Instalar</span><span class="sxs-lookup"><span data-stu-id="2ceb4-106">Install</span></span>

1. <span data-ttu-id="2ceb4-107">Instale `curl`:</span><span class="sxs-lookup"><span data-stu-id="2ceb4-107">Install `curl`:</span></span>

   ```bash
   sudo zypper refresh
   sudo zypper install -y curl
   ```

2. <span data-ttu-id="2ceb4-108">Importe a chave de repositório da Microsoft:</span><span class="sxs-lookup"><span data-stu-id="2ceb4-108">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

3. <span data-ttu-id="2ceb4-109">Crie informações sobre o repositório do `azure-cli` local:</span><span class="sxs-lookup"><span data-stu-id="2ceb4-109">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ntype=rpm-md\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/zypp/repos.d/azure-cli.repo'
   ```

4. <span data-ttu-id="2ceb4-110">Atualize o índice de pacote do `zypper` e instale:</span><span class="sxs-lookup"><span data-stu-id="2ceb4-110">Update the `zypper` package index and install:</span></span>

   ```bash
   sudo zypper refresh
   sudo zypper install -y azure-cli
   ```

<span data-ttu-id="2ceb4-111">É possível executar a CLI com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="2ceb4-111">You can run the CLI with the `az` command.</span></span>

## <a name="update"></a><span data-ttu-id="2ceb4-112">Atualizar</span><span class="sxs-lookup"><span data-stu-id="2ceb4-112">Update</span></span>

<span data-ttu-id="2ceb4-113">Você pode atualizar o pacote com o comando `zypper update`.</span><span class="sxs-lookup"><span data-stu-id="2ceb4-113">You can update the package with the `zypper update` command.</span></span>

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="2ceb4-114">Desinstalar</span><span class="sxs-lookup"><span data-stu-id="2ceb4-114">Uninstall</span></span>

<span data-ttu-id="2ceb4-115">Se você decidiu desinstalar a CLI do Azure, lamentamos sua saída.</span><span class="sxs-lookup"><span data-stu-id="2ceb4-115">If you ever decide to uninstall the Azure CLI, we're sorry to see you go.</span></span> <span data-ttu-id="2ceb4-116">Antes de desinstalar, use o comando `az feedback` para nos fornecer algumas razões por ter escolhido desinstalar e como poderíamos melhorar a experiência da CLI.</span><span class="sxs-lookup"><span data-stu-id="2ceb4-116">Before you uninstall, use the `az feedback` command to give us some reasons why you chose to uninstall and how we could improve the CLI experience.</span></span> <span data-ttu-id="2ceb4-117">Queremos assegurar que a CLI do Azure não tenha bugs e seja amigável o máximo possível.</span><span class="sxs-lookup"><span data-stu-id="2ceb4-117">We want to make sure that the Azure CLI is as bug-free and user-friendly as we can make it.</span></span> <span data-ttu-id="2ceb4-118">Você também pode [registrar um problema do github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="2ceb4-118">You can also [file a github issue](https://github.com/Azure/azure-cli/issues).</span></span>

1. <span data-ttu-id="2ceb4-119">Remova o pacote do seu sistema.</span><span class="sxs-lookup"><span data-stu-id="2ceb4-119">Remove the package from your system.</span></span>

    ```bash
    sudo zypper remove -y azure-cli
    ```

2. <span data-ttu-id="2ceb4-120">Se você não pretende reinstalar a CLI, remova as informações do repositório.</span><span class="sxs-lookup"><span data-stu-id="2ceb4-120">If you do not plan to reinstall the CLI, remove the repository information.</span></span>

  ```bash
  sudo rm /etc/zypp/repos.d/azure-cli.repo
  ```

3. <span data-ttu-id="2ceb4-121">Se você removeu as informações do repositório, remova também a chave de assinatura do Microsoft GPG.</span><span class="sxs-lookup"><span data-stu-id="2ceb4-121">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```

