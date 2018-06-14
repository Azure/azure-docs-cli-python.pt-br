---
title: Instalar a CLI do Azure 2.0 no Linux com zypper
description: Como instalar a CLI do Azure 2.0 com o zypper
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 01/29/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: a862cca17adb1bfa0201af250819158081c29813
ms.sourcegitcommit: 5c80e96e96f9608c92a94fa4a9c4afb25099f3fc
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/13/2018
ms.locfileid: "35512964"
---
# <a name="install-azure-cli-20-with-zypper"></a><span data-ttu-id="d4bce-103">Instalar CLI do Azure 2.0 com zypper</span><span class="sxs-lookup"><span data-stu-id="d4bce-103">Install Azure CLI 2.0 with zypper</span></span>

<span data-ttu-id="d4bce-104">Se você estiver executando uma distribuição que vem com `zypper`, como o openSUSE ou SLES, há um pacote disponível para a CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="d4bce-104">If you are running a distribution that comes with `zypper`, such as openSUSE or SLES, there is a package available for the Azure CLI.</span></span> <span data-ttu-id="d4bce-105">Este pacote foi testado com openSUSE 42.2 e SLES 12 SP 2.</span><span class="sxs-lookup"><span data-stu-id="d4bce-105">This package has been tested with openSUSE 42.2 and SLES 12 SP 2.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a><span data-ttu-id="d4bce-106">Instalar</span><span class="sxs-lookup"><span data-stu-id="d4bce-106">Install</span></span>

1. <span data-ttu-id="d4bce-107">Instale `curl`:</span><span class="sxs-lookup"><span data-stu-id="d4bce-107">Install `curl`:</span></span>

   ```bash
   sudo zypper install -y curl
   ```

2. <span data-ttu-id="d4bce-108">Importe a chave de repositório da Microsoft:</span><span class="sxs-lookup"><span data-stu-id="d4bce-108">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

3. <span data-ttu-id="d4bce-109">Crie informações sobre o repositório do `azure-cli` local:</span><span class="sxs-lookup"><span data-stu-id="d4bce-109">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo zypper addrepo --name 'Azure CLI' --check https://packages.microsoft.com/yumrepos/azure-cli azure-cli
   ```

4. <span data-ttu-id="d4bce-110">Atualize o índice de pacote do `zypper` e instale:</span><span class="sxs-lookup"><span data-stu-id="d4bce-110">Update the `zypper` package index and install:</span></span>

   ```bash
   sudo zypper install --from azure-cli -y azure-cli
   ```

<span data-ttu-id="d4bce-111">É possível executar a CLI do Azure com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="d4bce-111">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="d4bce-112">Para fazer logon, execute o comando `az login`.</span><span class="sxs-lookup"><span data-stu-id="d4bce-112">To log in, run the `az login` command.</span></span>

```azurecli
az login
```

<span data-ttu-id="d4bce-113">Para saber mais sobre os métodos de logon diferente, consulte [Fazer logon com a CLI do Azure 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="d4bce-113">To learn more about different login methods, see [Log in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="update"></a><span data-ttu-id="d4bce-114">Atualizar</span><span class="sxs-lookup"><span data-stu-id="d4bce-114">Update</span></span>

<span data-ttu-id="d4bce-115">Você pode atualizar o pacote com o comando `zypper update`.</span><span class="sxs-lookup"><span data-stu-id="d4bce-115">You can update the package with the `zypper update` command.</span></span>

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="d4bce-116">Desinstalar</span><span class="sxs-lookup"><span data-stu-id="d4bce-116">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="d4bce-117">Remova o pacote do seu sistema.</span><span class="sxs-lookup"><span data-stu-id="d4bce-117">Remove the package from your system.</span></span>

    ```bash
    sudo zypper remove -y azure-cli
    ```

2. <span data-ttu-id="d4bce-118">Se você não pretende reinstalar a CLI, remova as informações do repositório.</span><span class="sxs-lookup"><span data-stu-id="d4bce-118">If you do not plan to reinstall the CLI, remove the repository information.</span></span>

  ```bash
  sudo zypper removerepo azure-cli
  ```

3. <span data-ttu-id="d4bce-119">Se você removeu as informações do repositório, remova também a chave de assinatura do Microsoft GPG.</span><span class="sxs-lookup"><span data-stu-id="d4bce-119">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```

