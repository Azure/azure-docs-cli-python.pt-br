---
title: Instalar a CLI do Azure 2.0 no Linux com apt
description: Como instalar a CLI do Azure 2.0 com o gerenciador de pacotes apt
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 02/06/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 4076fefb902a324f77f97bc042b9f5ba3e787734
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/15/2018
---
# <a name="install-azure-cli-20-with-apt"></a><span data-ttu-id="37103-103">Instalar CLI do Azure 2.0 com o apt</span><span class="sxs-lookup"><span data-stu-id="37103-103">Install Azure CLI 2.0 with apt</span></span>

<span data-ttu-id="37103-104">Se você estiver executando uma distribuição que venha com o `apt`, como o Ubuntu ou Debian, há um pacote 64-bit disponível para a CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="37103-104">If you are running a distribution that comes with `apt`, such as Ubuntu or Debian, there is a 64-bit package available for the Azure CLI.</span></span> <span data-ttu-id="37103-105">Esse pacote foi testado com:</span><span class="sxs-lookup"><span data-stu-id="37103-105">This package has been tested with:</span></span>

* <span data-ttu-id="37103-106">Ubuntu wheezy, xenial e artful</span><span class="sxs-lookup"><span data-stu-id="37103-106">Ubuntu wheezy, xenial, and artful</span></span>
* <span data-ttu-id="37103-107">Debian wheezy, jessie e stretch</span><span class="sxs-lookup"><span data-stu-id="37103-107">Debian wheezy, jessie, and stretch</span></span>

## <a name="install"></a><span data-ttu-id="37103-108">Instalar</span><span class="sxs-lookup"><span data-stu-id="37103-108">Install</span></span>

1. <span data-ttu-id="37103-109">Modifique sua lista de fontes:</span><span class="sxs-lookup"><span data-stu-id="37103-109">Modify your sources list:</span></span>

     ```bash
     AZ_REPO=$(lsb_release -cs)
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="37103-110">Execute os comandos sudo a seguir:</span><span class="sxs-lookup"><span data-stu-id="37103-110">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

<span data-ttu-id="37103-111">É possível executar a CLI do Azure com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="37103-111">You can run the Azure CLI with the `az` command.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="37103-112">solução de problemas</span><span class="sxs-lookup"><span data-stu-id="37103-112">Troubleshooting</span></span>

<span data-ttu-id="37103-113">Aqui estão alguns problemas comuns vistos durante a instalação com `apt`.</span><span class="sxs-lookup"><span data-stu-id="37103-113">Here are some common problems seen when installing with `apt`.</span></span> <span data-ttu-id="37103-114">Se o problema não estiver listado aqui, [registre um problema no github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="37103-114">If your issue is not listed here, please [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="apt-key-fails-with-no-dirmngr"></a><span data-ttu-id="37103-115">A apt-key falha com “Sem dirmngr”</span><span class="sxs-lookup"><span data-stu-id="37103-115">apt-key fails with "No dirmngr"</span></span>

<span data-ttu-id="37103-116">Ao executar o comando `apt-key`, pode ser que você veja uma saída semelhante ao seguinte erro:</span><span class="sxs-lookup"><span data-stu-id="37103-116">When running the `apt-key` command, you may see output similar to the following error:</span></span>

```output
gpg: failed to start the dirmngr '/usr/bin/dirmngr': No such file or directory
gpg: connecting dirmngr at '/tmp/apt-key-gpghome.kt5zo27tp1/S.dirmngr' failed: No such file or directory
gpg: keyserver receive failed: No dirmngr
```

<span data-ttu-id="37103-117">O erro ocorre devido a um componente ausente exigido por `apt-key`.</span><span class="sxs-lookup"><span data-stu-id="37103-117">The error is due to a missing component required by `apt-key`.</span></span> <span data-ttu-id="37103-118">Você pode resolver isso instalando o pacote `dirmngr`.</span><span class="sxs-lookup"><span data-stu-id="37103-118">You can resolve it by installing the `dirmngr` package.</span></span>

```bash
sudo apt-get install dirmngr
```

## <a name="update"></a><span data-ttu-id="37103-119">Atualizar</span><span class="sxs-lookup"><span data-stu-id="37103-119">Update</span></span>

<span data-ttu-id="37103-120">Use `apt-get upgrade` para atualizar o pacote da CLI.</span><span class="sxs-lookup"><span data-stu-id="37103-120">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="37103-121">Esse comando atualiza todos os pacotes instalados no seu sistema que não tiveram uma alteração de dependência.</span><span class="sxs-lookup"><span data-stu-id="37103-121">This command upgrades all of the installed packages on your system that have not had a dependency change.</span></span>
> <span data-ttu-id="37103-122">Para atualizar apenas a CLI, use `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="37103-122">To upgrade the CLI only, use `apt-get install`.</span></span>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a><span data-ttu-id="37103-123">Desinstalar</span><span class="sxs-lookup"><span data-stu-id="37103-123">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="37103-124">Desinstalar com `apt-get remove`.</span><span class="sxs-lookup"><span data-stu-id="37103-124">Uninstall with `apt-get remove`.</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="37103-125">Se você não pretende reinstalar a CLI, remova as informações do repositório da CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="37103-125">If you do not plan to reinstall the CLI, remove the Azure CLI repository information.</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="37103-126">Remova quaisquer pacotes desnecessários.</span><span class="sxs-lookup"><span data-stu-id="37103-126">Remove any unneeded packages.</span></span>

   ```bash
   sudo apt autoremove
   ```
