---
title: Instalar a CLI do Azure 2.0 no Linux com yum
description: Como instalar a CLI do Azure 2.0 com o yum
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 6a63d1ccd6b182b0c7144101f7efbf3264a6cb72
ms.sourcegitcommit: 0e9aafa07311526f43661c8bd3a7eba7cbc2caed
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/20/2018
---
# <a name="install-azure-cli-20-with-yum"></a><span data-ttu-id="6f6b5-103">Instalar CLI do Azure 2.0 com o yum</span><span class="sxs-lookup"><span data-stu-id="6f6b5-103">Install Azure CLI 2.0 with yum</span></span>

<span data-ttu-id="6f6b5-104">Se você estiver executando uma distribuição que vem com `yum`, como RHEL, Fedora ou CentOS, há um pacote disponível para a CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="6f6b5-104">If you are running a distribution that comes with `yum`, such as RHEL, Fedora, or CentOS, there is a package available for the Azure CLI.</span></span> <span data-ttu-id="6f6b5-105">Este pacote foi testado com RHEL 7, Fedora 19 e posterior e CentOS 7.</span><span class="sxs-lookup"><span data-stu-id="6f6b5-105">This package has been tested with RHEL 7, Fedora 19 and higher, and CentOS 7.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a><span data-ttu-id="6f6b5-106">Instalar</span><span class="sxs-lookup"><span data-stu-id="6f6b5-106">Install</span></span>

1. <span data-ttu-id="6f6b5-107">Importe a chave do repositório da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="6f6b5-107">Import the Microsoft repository key.</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="6f6b5-108">Crie informações sobre o repositório do local `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="6f6b5-108">Create local `azure-cli` repository information.</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="6f6b5-109">Instale com o comando `yum install`.</span><span class="sxs-lookup"><span data-stu-id="6f6b5-109">Install with the `yum install` command.</span></span> 

   ```bash
   sudo yum install azure-cli
   ```

<span data-ttu-id="6f6b5-110">É possível executar a CLI do Azure com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="6f6b5-110">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="6f6b5-111">Para fazer logon, execute o comando `az login`.</span><span class="sxs-lookup"><span data-stu-id="6f6b5-111">To log in, run the `az login` command.</span></span>

```azurecli
az login
```

<span data-ttu-id="6f6b5-112">Para saber mais sobre os métodos de logon diferente, consulte [Fazer logon com a CLI do Azure 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="6f6b5-112">To learn more about different login methods, see [Log in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="update"></a><span data-ttu-id="6f6b5-113">Atualizar</span><span class="sxs-lookup"><span data-stu-id="6f6b5-113">Update</span></span>

<span data-ttu-id="6f6b5-114">Atualize a CLI do Azure com o comando `yum update`.</span><span class="sxs-lookup"><span data-stu-id="6f6b5-114">Update the Azure CLI with the `yum update` command.</span></span>

```bash
sudo yum update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="6f6b5-115">Desinstalar</span><span class="sxs-lookup"><span data-stu-id="6f6b5-115">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="6f6b5-116">Remova o pacote do seu sistema.</span><span class="sxs-lookup"><span data-stu-id="6f6b5-116">Remove the package from your system.</span></span>

   ```bash
   sudo yum remove azure-cli
   ```

2. <span data-ttu-id="6f6b5-117">Se você não pretende reinstalar a CLI, remova as informações do repositório.</span><span class="sxs-lookup"><span data-stu-id="6f6b5-117">If you do not plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="6f6b5-118">Se você removeu as informações do repositório, remova também a chave de assinatura do Microsoft GPG.</span><span class="sxs-lookup"><span data-stu-id="6f6b5-118">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```
