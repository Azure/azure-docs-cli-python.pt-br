---
title: Instalar a CLI do Azure 2.0 no Linux com zypper
description: Como instalar a CLI do Azure 2.0 com o zypper
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: ed92443b6de4e538eaf5da41376e836aa2c771a0
ms.sourcegitcommit: 0e688704889fc88b91588bb6678a933c2d54f020
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/11/2018
ms.locfileid: "44388296"
---
# <a name="install-azure-cli-20-with-zypper"></a><span data-ttu-id="cca3b-103">Instalar CLI do Azure 2.0 com zypper</span><span class="sxs-lookup"><span data-stu-id="cca3b-103">Install Azure CLI 2.0 with zypper</span></span>

<span data-ttu-id="cca3b-104">Para distribuições Linux com `zypper`, como o openSUSE ou SLES, há um pacote disponível para a CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="cca3b-104">For Linux distributions with `zypper`, such as openSUSE or SLES, there's a package available for the Azure CLI.</span></span> <span data-ttu-id="cca3b-105">Este pacote foi testado com openSUSE 42.2 e SLES 12 SP 2.</span><span class="sxs-lookup"><span data-stu-id="cca3b-105">This package has been tested with openSUSE 42.2 and SLES 12 SP 2.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a><span data-ttu-id="cca3b-106">Instalar</span><span class="sxs-lookup"><span data-stu-id="cca3b-106">Install</span></span>

1. <span data-ttu-id="cca3b-107">Instale `curl`:</span><span class="sxs-lookup"><span data-stu-id="cca3b-107">Install `curl`:</span></span>

   ```bash
   sudo zypper install -y curl
   ```

2. <span data-ttu-id="cca3b-108">Importe a chave de repositório da Microsoft:</span><span class="sxs-lookup"><span data-stu-id="cca3b-108">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

3. <span data-ttu-id="cca3b-109">Crie informações sobre o repositório do `azure-cli` local:</span><span class="sxs-lookup"><span data-stu-id="cca3b-109">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo zypper addrepo --name 'Azure CLI' --check https://packages.microsoft.com/yumrepos/azure-cli azure-cli
   ```

4. <span data-ttu-id="cca3b-110">Atualize o índice de pacote do `zypper` e instale:</span><span class="sxs-lookup"><span data-stu-id="cca3b-110">Update the `zypper` package index and install:</span></span>

   ```bash
   sudo zypper install --from azure-cli -y azure-cli
   ```

<span data-ttu-id="cca3b-111">É possível executar a CLI do Azure com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="cca3b-111">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="cca3b-112">Para entrar, use o comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="cca3b-112">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="cca3b-113">Para saber mais sobre os diferentes métodos de autenticação, consulte [Conectar com a CLI do Azure 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="cca3b-113">To learn more about different authentication methods, see [Sign in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="update"></a><span data-ttu-id="cca3b-114">Atualizar</span><span class="sxs-lookup"><span data-stu-id="cca3b-114">Update</span></span>

<span data-ttu-id="cca3b-115">Você pode atualizar o pacote com o comando `zypper update`.</span><span class="sxs-lookup"><span data-stu-id="cca3b-115">You can update the package with the `zypper update` command.</span></span>

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="cca3b-116">Desinstalar</span><span class="sxs-lookup"><span data-stu-id="cca3b-116">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="cca3b-117">Remova o pacote do seu sistema.</span><span class="sxs-lookup"><span data-stu-id="cca3b-117">Remove the package from your system.</span></span>

    ```bash
    sudo zypper remove -y azure-cli
    ```

2. <span data-ttu-id="cca3b-118">Se você não pretende reinstalar a CLI, remova as informações do repositório.</span><span class="sxs-lookup"><span data-stu-id="cca3b-118">If you don't plan to reinstall the CLI, remove the repository information.</span></span>

  ```bash
  sudo zypper removerepo azure-cli
  ```

3. <span data-ttu-id="cca3b-119">Se você removeu as informações do repositório, remova também a chave de assinatura do Microsoft GPG.</span><span class="sxs-lookup"><span data-stu-id="cca3b-119">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```