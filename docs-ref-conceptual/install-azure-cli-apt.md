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
ms.openlocfilehash: 65e8e78275b0f40a2298934fe8bc9368bbf796a7
ms.sourcegitcommit: 59f0b667f2202bae8914e6fc8dc5c9dc79fef91c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/25/2018
---
# <a name="install-azure-cli-20-with-apt"></a><span data-ttu-id="590ed-104">Instalar CLI do Azure 2.0 com o apt</span><span class="sxs-lookup"><span data-stu-id="590ed-104">Install Azure CLI 2.0 with apt</span></span>

<span data-ttu-id="590ed-105">Se você estiver executando uma distribuição que vem com o `apt`, como o Ubuntu ou Debian, há um pacote disponível para a CLI do Azure que pode ser instalado em seu sistema.</span><span class="sxs-lookup"><span data-stu-id="590ed-105">If you are running a distirbution that comes with `apt`, such as Ubuntu or Debian, there is an available package for the Azure CLI that you can install on your system.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a><span data-ttu-id="590ed-106">Instalar</span><span class="sxs-lookup"><span data-stu-id="590ed-106">Install</span></span>

1. <span data-ttu-id="590ed-107">Modifique sua lista de fontes:</span><span class="sxs-lookup"><span data-stu-id="590ed-107">Modify your sources list:</span></span>

   - <span data-ttu-id="590ed-108">sistema de 32 bits</span><span class="sxs-lookup"><span data-stu-id="590ed-108">32-bit system</span></span>

     ```bash
     echo "deb https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

   - <span data-ttu-id="590ed-109">sistema de 64 bits</span><span class="sxs-lookup"><span data-stu-id="590ed-109">64-bit system</span></span>

     ```bash
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="590ed-110">Execute os comandos sudo a seguir:</span><span class="sxs-lookup"><span data-stu-id="590ed-110">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

<span data-ttu-id="590ed-111">É possível executar a CLI do Azure com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="590ed-111">You can run the Azure CLI with the `az` command.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="590ed-112">solução de problemas</span><span class="sxs-lookup"><span data-stu-id="590ed-112">Troubleshooting</span></span>

### <a name="apt-key-fails-with-no-dirmngr"></a><span data-ttu-id="590ed-113">A apt-key falha com “Sem dirmngr”</span><span class="sxs-lookup"><span data-stu-id="590ed-113">apt-key fails with "No dirmngr"</span></span>

<span data-ttu-id="590ed-114">Ao executar o comando `apt-key`, você verá uma saída semelhante ao seguinte erro.</span><span class="sxs-lookup"><span data-stu-id="590ed-114">When running the `apt-key` command, you may see output similar to the following error.</span></span>

```output
gpg: failed to start the dirmngr '/usr/bin/dirmngr': No such file or directory
gpg: connecting dirmngr at '/tmp/apt-key-gpghome.kt5zo27tp1/S.dirmngr' failed: No such file or directory
gpg: keyserver receive failed: No dirmngr
```

<span data-ttu-id="590ed-115">Isso ocorre devido a um componente ausente exigido por `apt-key`.</span><span class="sxs-lookup"><span data-stu-id="590ed-115">This is due to a missing component required by `apt-key`.</span></span> <span data-ttu-id="590ed-116">Você pode resolver isso instalando o pacote `dirmngr`.</span><span class="sxs-lookup"><span data-stu-id="590ed-116">You can resolve this by installing the `dirmngr` package.</span></span>

```bash
sudo apt-get install dirmngr
```

## <a name="update"></a><span data-ttu-id="590ed-117">Atualizar</span><span class="sxs-lookup"><span data-stu-id="590ed-117">Update</span></span>

<span data-ttu-id="590ed-118">Use `apt-get upgrade` para atualizar o pacote da CLI.</span><span class="sxs-lookup"><span data-stu-id="590ed-118">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="590ed-119">Isso atualizará todos os pacotes instalados no sistema que não tiveram uma alteração de dependência.</span><span class="sxs-lookup"><span data-stu-id="590ed-119">This will upgrade all of the installed packages on your system which have not had a dependency change.</span></span>
> <span data-ttu-id="590ed-120">Para atualizar somente a CLI, use `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="590ed-120">To upgrade only the CLI, use `apt-get install`.</span></span>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

### <a name="uninstall"></a><span data-ttu-id="590ed-121">Desinstalar</span><span class="sxs-lookup"><span data-stu-id="590ed-121">Uninstall</span></span>

<span data-ttu-id="590ed-122">Se você decidiu desinstalar a CLI do Azure, lamentamos sua saída.</span><span class="sxs-lookup"><span data-stu-id="590ed-122">If you ever decide to uninstall the Azure CLI, we're sorry to see you go.</span></span> <span data-ttu-id="590ed-123">Antes de desinstalar, use o comando `az feedback` para nos fornecer algumas razões por ter escolhido desinstalar e como poderíamos melhorar a experiência da CLI.</span><span class="sxs-lookup"><span data-stu-id="590ed-123">Before you uninstall, use the `az feedback` command to give us some reasons why you chose to uninstall and how we could improve the CLI experience.</span></span> <span data-ttu-id="590ed-124">Queremos assegurar que a CLI do Azure não tenha bugs e seja amigável o máximo possível.</span><span class="sxs-lookup"><span data-stu-id="590ed-124">We want to make sure that the Azure CLI is as bug-free and user-friendly as we can make it.</span></span> <span data-ttu-id="590ed-125">Você também pode [registrar um problema do github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="590ed-125">You can also [file a github issue](https://github.com/Azure/azure-cli/issues).</span></span>

1. <span data-ttu-id="590ed-126">Desinstalar com `apt-get remove`.</span><span class="sxs-lookup"><span data-stu-id="590ed-126">Uninstall with `apt-get remove`.</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="590ed-127">Se você não pretende reinstalar a CLI, remova as informações do repositório da CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="590ed-127">If you do not plan to reinstall the CLI, remove the Azure CLI repository information.</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="590ed-128">Remova quaisquer pacotes desnecessários.</span><span class="sxs-lookup"><span data-stu-id="590ed-128">Remove any unneeded packages.</span></span>

   ```bash
   sudo apt autoremove
   ```
