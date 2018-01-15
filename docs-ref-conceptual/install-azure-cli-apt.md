---
title: Instalar a CLI do Azure 2.0 com o apt
description: Como instalar a CLI do Azure 2.0 com o gerenciador de pacotes apt
keywords: CLI do Azure, Instalar CLI do Azure, apt do azure, debian do azure, ubuntu do azure
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
ms.openlocfilehash: 75c531a13a4b730158cd2e874cb6c5d581a27598
ms.sourcegitcommit: 3eef136ae752eb90c67af604d4ddd298d70b1c9d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/06/2018
---
# <a name="install-azure-cli-20-with-apt"></a><span data-ttu-id="2598a-104">Instalar CLI do Azure 2.0 com o apt</span><span class="sxs-lookup"><span data-stu-id="2598a-104">Install Azure CLI 2.0 with apt</span></span>

<span data-ttu-id="2598a-105">Se você estiver executando uma distribuição que vem com o `apt`, como o Ubuntu ou Debian, há um pacote disponível para a CLI do Azure que pode ser instalado em seu sistema.</span><span class="sxs-lookup"><span data-stu-id="2598a-105">If you are running a distirbution that comes with `apt`, such as Ubuntu or Debian, there is an available package for the Azure CLI that you can install on your system.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a><span data-ttu-id="2598a-106">Instalar</span><span class="sxs-lookup"><span data-stu-id="2598a-106">Install</span></span>

1. <span data-ttu-id="2598a-107">Modifique sua lista de fontes:</span><span class="sxs-lookup"><span data-stu-id="2598a-107">Modify your sources list:</span></span>

   - <span data-ttu-id="2598a-108">sistema de 32 bits</span><span class="sxs-lookup"><span data-stu-id="2598a-108">32-bit system</span></span>

     ```bash
     echo "deb https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

   - <span data-ttu-id="2598a-109">sistema de 64 bits</span><span class="sxs-lookup"><span data-stu-id="2598a-109">64-bit system</span></span>

     ```bash
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="2598a-110">Execute os comandos sudo a seguir:</span><span class="sxs-lookup"><span data-stu-id="2598a-110">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

<span data-ttu-id="2598a-111">É possível executar a CLI do Azure com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="2598a-111">You can run the Azure CLI with the `az` command.</span></span>

## <a name="update"></a><span data-ttu-id="2598a-112">Atualizar</span><span class="sxs-lookup"><span data-stu-id="2598a-112">Update</span></span>

<span data-ttu-id="2598a-113">Use `apt-get upgrade` para atualizar o pacote da CLI.</span><span class="sxs-lookup"><span data-stu-id="2598a-113">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="2598a-114">Isso atualizará todos os pacotes instalados no sistema que não tiveram uma alteração de dependência.</span><span class="sxs-lookup"><span data-stu-id="2598a-114">This will upgrade all of the installed packages on your system which have not had a dependency change.</span></span>
> <span data-ttu-id="2598a-115">Para atualizar somente a CLI, use `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="2598a-115">To upgrade only the CLI, use `apt-get install`.</span></span>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

### <a name="uninstall"></a><span data-ttu-id="2598a-116">Desinstalar</span><span class="sxs-lookup"><span data-stu-id="2598a-116">Uninstall</span></span>

<span data-ttu-id="2598a-117">Se você decidiu desinstalar a CLI do Azure, lamentamos sua saída.</span><span class="sxs-lookup"><span data-stu-id="2598a-117">If you ever decide to uninstall the Azure CLI, we're sorry to see you go.</span></span> <span data-ttu-id="2598a-118">Antes de desinstalar, use o comando `az feedback` para nos fornecer algumas razões por ter escolhido desinstalar e como poderíamos melhorar a experiência da CLI.</span><span class="sxs-lookup"><span data-stu-id="2598a-118">Before you uninstall, use the `az feedback` command to give us some reasons why you chose to uninstall and how we could improve the CLI experience.</span></span> <span data-ttu-id="2598a-119">Queremos assegurar que a CLI do Azure não tenha bugs e seja amigável o máximo possível.</span><span class="sxs-lookup"><span data-stu-id="2598a-119">We want to make sure that the Azure CLI is as bug-free and user-friendly as we can make it.</span></span> <span data-ttu-id="2598a-120">Você também pode [registrar um problema do github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="2598a-120">You can also [file a github issue](https://github.com/Azure/azure-cli/issues).</span></span>

1. <span data-ttu-id="2598a-121">Desinstalar com `apt-get remove`.</span><span class="sxs-lookup"><span data-stu-id="2598a-121">Uninstall with `apt-get remove`.</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="2598a-122">Se você não pretende reinstalar a CLI, remova as informações do repositório da CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="2598a-122">If you do not plan to reinstall the CLI, remove the Azure CLI repository information.</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="2598a-123">Remova quaisquer pacotes desnecessários.</span><span class="sxs-lookup"><span data-stu-id="2598a-123">Remove any unneeded packages.</span></span>

   ```bash
   sudo apt autoremove
   ```
