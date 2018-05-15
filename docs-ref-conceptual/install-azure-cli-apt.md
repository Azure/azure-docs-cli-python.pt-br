---
title: Instalar a CLI do Azure 2.0 no Linux com apt
description: Como instalar a CLI do Azure 2.0 com o gerenciador de pacotes apt
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 02/06/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 7eb04b408f403264f3951bf663d43686601c4ab8
ms.sourcegitcommit: 1d18f667af28b59f5524a3499a4b7dc12af5163d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2018
---
# <a name="install-azure-cli-20-with-apt"></a><span data-ttu-id="817d1-103">Instalar CLI do Azure 2.0 com o apt</span><span class="sxs-lookup"><span data-stu-id="817d1-103">Install Azure CLI 2.0 with apt</span></span>

<span data-ttu-id="817d1-104">Se você estiver executando uma distribuição que venha com o `apt`, como o Ubuntu ou Debian, há um pacote 64-bit disponível para a CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="817d1-104">If you are running a distribution that comes with `apt`, such as Ubuntu or Debian, there is a 64-bit package available for the Azure CLI.</span></span> <span data-ttu-id="817d1-105">Esse pacote foi testado com:</span><span class="sxs-lookup"><span data-stu-id="817d1-105">This package has been tested with:</span></span>

* <span data-ttu-id="817d1-106">Ubuntu trusty, xenial e artful</span><span class="sxs-lookup"><span data-stu-id="817d1-106">Ubuntu trusty, xenial, and artful</span></span>
* <span data-ttu-id="817d1-107">Debian wheezy, jessie e stretch</span><span class="sxs-lookup"><span data-stu-id="817d1-107">Debian wheezy, jessie, and stretch</span></span>

## <a name="install"></a><span data-ttu-id="817d1-108">Instalar</span><span class="sxs-lookup"><span data-stu-id="817d1-108">Install</span></span>

1. <span data-ttu-id="817d1-109">Modifique sua lista de fontes:</span><span class="sxs-lookup"><span data-stu-id="817d1-109">Modify your sources list:</span></span>

     ```bash
     AZ_REPO=$(lsb_release -cs)
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="817d1-110">Obtenha a chave de assinatura da Microsoft:</span><span class="sxs-lookup"><span data-stu-id="817d1-110">Get the Microsoft signing key:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   ```

  > [!WARNING]
  > <span data-ttu-id="817d1-111">Esta chave de assinatura foi preterida e será substituída no final de maio de 2018.</span><span class="sxs-lookup"><span data-stu-id="817d1-111">This signing key is deprecated, and will be replaced at the end of May 2018.</span></span> <span data-ttu-id="817d1-112">Para continuar recebendo atualizações com `apt`, verifique se você instalou a nova chave:</span><span class="sxs-lookup"><span data-stu-id="817d1-112">In order to keep getting updates with `apt`, make sure that you also install the new key:</span></span>
  > 
  > ```bash
  > curl -L https://packages.microsoft.com/keys/microsoft.asc | sudo apt-key add -
  > ``` 

3. <span data-ttu-id="817d1-113">Instalar a CLI:</span><span class="sxs-lookup"><span data-stu-id="817d1-113">Install the CLI:</span></span>

   ```bash
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

<span data-ttu-id="817d1-114">É possível executar a CLI do Azure com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="817d1-114">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="817d1-115">Para fazer logon, execute o comando `az login`.</span><span class="sxs-lookup"><span data-stu-id="817d1-115">To log in, run the `az login` command.</span></span>

```azurecli
az login
```

<span data-ttu-id="817d1-116">Para saber mais sobre os métodos de logon diferente, consulte [Fazer logon com a CLI do Azure 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="817d1-116">To learn more about different login methods, see [Log in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="817d1-117">solução de problemas</span><span class="sxs-lookup"><span data-stu-id="817d1-117">Troubleshooting</span></span>

<span data-ttu-id="817d1-118">Aqui estão alguns problemas comuns vistos durante a instalação com `apt`.</span><span class="sxs-lookup"><span data-stu-id="817d1-118">Here are some common problems seen when installing with `apt`.</span></span> <span data-ttu-id="817d1-119">Se o problema não estiver listado aqui, [registre um problema no github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="817d1-119">If your issue is not listed here, please [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="lsbrelease-fails-with-command-not-found"></a><span data-ttu-id="817d1-120">lsb_release falha com "Command não encontrado"</span><span class="sxs-lookup"><span data-stu-id="817d1-120">lsb_release fails with "Command not found"</span></span>

<span data-ttu-id="817d1-121">Ao executar o comando `lsb_release`, pode ser que você veja uma saída semelhante ao seguinte erro:</span><span class="sxs-lookup"><span data-stu-id="817d1-121">When running the `lsb_release` command, you may see output similar to the following error:</span></span>

```output
-bash: lsb_release: command not found
```

<span data-ttu-id="817d1-122">O erro ocorre devido a lsb_release não estar sendo instalado.</span><span class="sxs-lookup"><span data-stu-id="817d1-122">The error is due to lsb_release not being installed.</span></span> <span data-ttu-id="817d1-123">Você pode resolver isso instalando o pacote `lsb-release`.</span><span class="sxs-lookup"><span data-stu-id="817d1-123">You can resolve it by installing the `lsb-release` package.</span></span>

```bash
sudo apt-get install lsb-release
```

### <a name="apt-key-fails-with-no-dirmngr"></a><span data-ttu-id="817d1-124">A apt-key falha com “Sem dirmngr”</span><span class="sxs-lookup"><span data-stu-id="817d1-124">apt-key fails with "No dirmngr"</span></span>

<span data-ttu-id="817d1-125">Ao executar o comando `apt-key`, pode ser que você veja uma saída semelhante ao seguinte erro:</span><span class="sxs-lookup"><span data-stu-id="817d1-125">When running the `apt-key` command, you may see output similar to the following error:</span></span>

```output
gpg: failed to start the dirmngr '/usr/bin/dirmngr': No such file or directory
gpg: connecting dirmngr at '/tmp/apt-key-gpghome.kt5zo27tp1/S.dirmngr' failed: No such file or directory
gpg: keyserver receive failed: No dirmngr
```

<span data-ttu-id="817d1-126">O erro ocorre devido a um componente ausente exigido por `apt-key`.</span><span class="sxs-lookup"><span data-stu-id="817d1-126">The error is due to a missing component required by `apt-key`.</span></span> <span data-ttu-id="817d1-127">Você pode resolver isso instalando o pacote `dirmngr`.</span><span class="sxs-lookup"><span data-stu-id="817d1-127">You can resolve it by installing the `dirmngr` package.</span></span>

```bash
sudo apt-get install dirmngr
```

### <a name="apt-key-hangs"></a><span data-ttu-id="817d1-128">A apt-key trava</span><span class="sxs-lookup"><span data-stu-id="817d1-128">apt-key hangs</span></span>

<span data-ttu-id="817d1-129">Quando atrás de um firewall bloqueando as conexões de saída para a porta 11371, o comando `apt-key` pode travar indefinidamente.</span><span class="sxs-lookup"><span data-stu-id="817d1-129">When behind a firewall blocking outgoing connections to port 11371, the `apt-key` command might hang indefinitely.</span></span> <span data-ttu-id="817d1-130">O firewall pode exigir o uso de um proxy HTTP para conexões de saída:</span><span class="sxs-lookup"><span data-stu-id="817d1-130">Your firewall may require the use of an HTTP proxy for outgoing connections:</span></span>

```bash
sudo apt-key adv --keyserver-options http-proxy=http://<USER>:<PASSWORD>@<PROXY-HOST>:<PROXY-PORT>/ --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
```

<span data-ttu-id="817d1-131">Se você não souber se tem um proxy, entre em contato com o administrador do sistema.</span><span class="sxs-lookup"><span data-stu-id="817d1-131">If you do not know if you have a proxy, contact your system administrator.</span></span> <span data-ttu-id="817d1-132">Se o proxy não precisar de um login, deixe usuário, senha e o token `@` de fora.</span><span class="sxs-lookup"><span data-stu-id="817d1-132">If your proxy does not require a login then leave out the user, password, and `@` token.</span></span>

## <a name="update"></a><span data-ttu-id="817d1-133">Atualizar</span><span class="sxs-lookup"><span data-stu-id="817d1-133">Update</span></span>

<span data-ttu-id="817d1-134">Use `apt-get upgrade` para atualizar o pacote da CLI.</span><span class="sxs-lookup"><span data-stu-id="817d1-134">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="817d1-135">Esse comando atualiza todos os pacotes instalados no seu sistema que não tiveram uma alteração de dependência.</span><span class="sxs-lookup"><span data-stu-id="817d1-135">This command upgrades all of the installed packages on your system that have not had a dependency change.</span></span>
> <span data-ttu-id="817d1-136">Para atualizar apenas a CLI, use `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="817d1-136">To upgrade the CLI only, use `apt-get install`.</span></span>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a><span data-ttu-id="817d1-137">Desinstalar</span><span class="sxs-lookup"><span data-stu-id="817d1-137">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="817d1-138">Desinstalar com `apt-get remove`.</span><span class="sxs-lookup"><span data-stu-id="817d1-138">Uninstall with `apt-get remove`.</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="817d1-139">Se você não pretende reinstalar a CLI, remova as informações do repositório da CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="817d1-139">If you do not plan to reinstall the CLI, remove the Azure CLI repository information.</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="817d1-140">Remova quaisquer pacotes desnecessários.</span><span class="sxs-lookup"><span data-stu-id="817d1-140">Remove any unneeded packages.</span></span>

   ```bash
   sudo apt autoremove
   ```
