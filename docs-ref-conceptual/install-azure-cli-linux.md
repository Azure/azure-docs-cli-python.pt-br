---
title: Instalar a CLI do Azure 2.0 para Linux manualmente
description: Como instalar a CLI do Azure 2.0 no Linux manualmente
keywords: CLI do Azure, Instalar CLI do Azure, linux do azure, linux instalar azure
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/18
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: d8c88d111c50a3cbb6b643a14dcd2a9773699657
ms.sourcegitcommit: 8606f36963e8daa6448d637393d1e4ef2c9859a0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/01/2018
---
# <a name="install-azure-cli-20-on-linux-manually"></a><span data-ttu-id="699e8-104">Instalar CLI do Azure 2.0 no Linux manualmente</span><span class="sxs-lookup"><span data-stu-id="699e8-104">Install Azure CLI 2.0 on Linux manually</span></span>

<span data-ttu-id="699e8-105">Se não tiver um pacote para a CLI do Azure disponível em sua distribuição, você sempre poderá instalar a CLI manualmente executando um script de instalação.</span><span class="sxs-lookup"><span data-stu-id="699e8-105">If you do not have a package for the Azure CLI available on your distribution, you can always install the CLI manually by running an installation script.</span></span>

> [!NOTE]
> <span data-ttu-id="699e8-106">É altamente recomendável que você use um gerenciador de pacotes para a CLI.</span><span class="sxs-lookup"><span data-stu-id="699e8-106">It's strongly recommend that you use a package manager for the CLI.</span></span> <span data-ttu-id="699e8-107">Um gerenciador de pacotes garante que você sempre obtenha as atualizações mais recentes, além da estabilidade dos componentes da CLI.</span><span class="sxs-lookup"><span data-stu-id="699e8-107">A package manager makes sure you always get the latest updates, and guarantees the stability of CLI components.</span></span> <span data-ttu-id="699e8-108">Verifique e veja se há um pacote de distribuição antes de instalar manualmente.</span><span class="sxs-lookup"><span data-stu-id="699e8-108">Check and see if there is a package for your distribution before installing manually.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="699e8-109">pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="699e8-109">Prerequisites</span></span>

<span data-ttu-id="699e8-110">Para instalar a CLI, você precisa dos seguintes softwares disponíveis em seu sistema:</span><span class="sxs-lookup"><span data-stu-id="699e8-110">In order to install the CLI, you need the following software available on your system:</span></span>

* [<span data-ttu-id="699e8-111">Python 2.7 ou Python 3. x</span><span class="sxs-lookup"><span data-stu-id="699e8-111">Python 2.7 or Python 3.x</span></span>](https://www.python.org/downloads/)
* [<span data-ttu-id="699e8-112">libffi</span><span class="sxs-lookup"><span data-stu-id="699e8-112">libffi</span></span>](https://sourceware.org/libffi/)
* [<span data-ttu-id="699e8-113">OpenSSL 1.0.2</span><span class="sxs-lookup"><span data-stu-id="699e8-113">OpenSSL 1.0.2</span></span>](https://www.openssl.org/source/)

## <a name="install-or-update"></a><span data-ttu-id="699e8-114">Instalar ou atualizar</span><span class="sxs-lookup"><span data-stu-id="699e8-114">Install or update</span></span> 

<span data-ttu-id="699e8-115">Se você estiver instalando ou atualizando a CLI, precisa executar uma instalação completa.</span><span class="sxs-lookup"><span data-stu-id="699e8-115">Whether you are installing or updating the CLI, you need to perform a full installation.</span></span> <span data-ttu-id="699e8-116">Assim que tiver os pré-requisitos, poderá instalar a CLI executando `curl`.</span><span class="sxs-lookup"><span data-stu-id="699e8-116">Once you have the prerequisites, you can install the CLI by running `curl`.</span></span>

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

<span data-ttu-id="699e8-117">Você também pode baixar o script e executá-lo localmente.</span><span class="sxs-lookup"><span data-stu-id="699e8-117">You can also download the script and run it locally instead.</span></span> <span data-ttu-id="699e8-118">Talvez você precise reiniciar o shell para que as alterações entrem em vigor.</span><span class="sxs-lookup"><span data-stu-id="699e8-118">You may have to restart your shell in order for changes to take effect.</span></span> <span data-ttu-id="699e8-119">Após a instalação, execute a CLI com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="699e8-119">After installation, run the CLI with the `az` command.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="699e8-120">solução de problemas</span><span class="sxs-lookup"><span data-stu-id="699e8-120">Troubleshooting</span></span>

<span data-ttu-id="699e8-121">Aqui estão alguns problemas comuns observados durante uma instalação manual.</span><span class="sxs-lookup"><span data-stu-id="699e8-121">Here are some common problems seen during a manual installation.</span></span> <span data-ttu-id="699e8-122">Se o problema não estiver listado aqui, [registre um problema no github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="699e8-122">If your issue is not listed here, please [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>
### <a name="curl-object-moved-error"></a><span data-ttu-id="699e8-123">Erro "Objeto movido" de cURL</span><span class="sxs-lookup"><span data-stu-id="699e8-123">curl "Object Moved" error</span></span>

<span data-ttu-id="699e8-124">Se você receber um erro de `curl` relacionado ao parâmetro `-L` ou uma mensagem de erro incluindo o texto "Objeto movido", tente usar a URL completa em vez da `aka.ms` de redirecionamento:</span><span class="sxs-lookup"><span data-stu-id="699e8-124">If you get an error from `curl` related to the `-L` parameter, or an error message including the text "Object Moved", try using the full URL instead of the `aka.ms` redirect:</span></span>

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a><span data-ttu-id="699e8-125">`az` comando não encontrado</span><span class="sxs-lookup"><span data-stu-id="699e8-125">`az` command not found</span></span>

<span data-ttu-id="699e8-126">Se não conseguir executar o comando após a instalação e usar `bash` ou `zsh`, limpe o cache do hash de comando do shell.</span><span class="sxs-lookup"><span data-stu-id="699e8-126">If you can't run the command after installation and using `bash` or `zsh`, clear your shell's command hash cache.</span></span> <span data-ttu-id="699e8-127">Executar</span><span class="sxs-lookup"><span data-stu-id="699e8-127">Run</span></span>

```bash
hash -r
```

<span data-ttu-id="699e8-128">e verificar se o problema foi resolvido.</span><span class="sxs-lookup"><span data-stu-id="699e8-128">and check if the problem is resolved.</span></span>

<span data-ttu-id="699e8-129">O problema também pode ocorrer se você não reiniciou o shell após a instalação.</span><span class="sxs-lookup"><span data-stu-id="699e8-129">The issue can also occur if you did not restart your shell after installation.</span></span> <span data-ttu-id="699e8-130">Verifique se o local do comando `az` está no `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="699e8-130">Make sure that the location of the `az` command is in your `$PATH`.</span></span> <span data-ttu-id="699e8-131">A localização do comando `az` é</span><span class="sxs-lookup"><span data-stu-id="699e8-131">The location of the `az` command is</span></span>

```bash
<install path>/bin
```

## <a name="uninstall"></a><span data-ttu-id="699e8-132">Desinstalar</span><span class="sxs-lookup"><span data-stu-id="699e8-132">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="699e8-133">Desinstale a CLI excluindo diretamente os arquivos do local escolhido no momento da instalação.</span><span class="sxs-lookup"><span data-stu-id="699e8-133">Uninstall the CLI by directly deleting the files from the location chosen at the time of installation.</span></span> <span data-ttu-id="699e8-134">O local de instalação padrão é `$HOME`.</span><span class="sxs-lookup"><span data-stu-id="699e8-134">The default install location is `$HOME`.</span></span>

1. <span data-ttu-id="699e8-135">Remova os arquivos da CLI instalados.</span><span class="sxs-lookup"><span data-stu-id="699e8-135">Remove the installed CLI files.</span></span>
  
  ```bash
  rm -r <install location>/lib/azure-cli
  rm <install location>/bin/az
  ```
2. <span data-ttu-id="699e8-136">Modifique o arquivo `$HOME/.bash_profile` para remover a seguinte linha:</span><span class="sxs-lookup"><span data-stu-id="699e8-136">Modify your `$HOME/.bash_profile` file to remove the following line:</span></span>
  
  ```
  <install location>/lib/azure-cli/az.completion
  ```

3. <span data-ttu-id="699e8-137">Se usar `bash` ou `zsh`, recarregue o cache de comando do shell.</span><span class="sxs-lookup"><span data-stu-id="699e8-137">If using `bash` or `zsh`, reload your shell's command cache.</span></span>
  
  ```bash
  hash -r
  ```
