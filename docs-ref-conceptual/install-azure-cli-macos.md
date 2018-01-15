---
title: Instalar a CLI do Azure para macOS
description: Como instalar a CLI do Azure 2.0 no macOS
keywords: CLI do Azure, Instalar CLI do Azure, macos do azure, macos instalar azure
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 10/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ROBOTS: NOINDEX,NOFOLLOW
ms.openlocfilehash: e615d2b3ab3b1307e982cb1d4d456633440afdf6
ms.sourcegitcommit: 3eef136ae752eb90c67af604d4ddd298d70b1c9d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/06/2018
---
# <a name="install-azure-cli-20-on-macos"></a><span data-ttu-id="ed17e-104">Instalar CLI do Azure 2.0 no macOS</span><span class="sxs-lookup"><span data-stu-id="ed17e-104">Install Azure CLI 2.0 on macOS</span></span>

<span data-ttu-id="ed17e-105">Para a plataforma macOS, você pode instalar a CLI do Azure usando o [gerenciador de pacotes homebrew](http://brew.sh) ou manualmente.</span><span class="sxs-lookup"><span data-stu-id="ed17e-105">For the macOS platform, you can install the Azure CLI either through the [homebrew package manager](http://brew.sh) or manually.</span></span> <span data-ttu-id="ed17e-106">O método preferencial de instalação é com o homebrew para que seja mais fácil instalar, atualizar e desinstalar se você precisar.</span><span class="sxs-lookup"><span data-stu-id="ed17e-106">The preferred installation method is through homebrew, so that it's easier to install, get updates, and uninstall if you need to.</span></span>

## <a name="use-homebrew-to-install"></a><span data-ttu-id="ed17e-107">Usar o homebrew para instalar</span><span class="sxs-lookup"><span data-stu-id="ed17e-107">Use homebrew to install</span></span>

<span data-ttu-id="ed17e-108">O homebrew é a maneira mais fácil de gerenciar a instalação da CLI.</span><span class="sxs-lookup"><span data-stu-id="ed17e-108">Homebrew is the easiest way to manage your CLI install.</span></span> <span data-ttu-id="ed17e-109">Ele fornece maneiras convenientes de instalar, atualizar e desinstalar.</span><span class="sxs-lookup"><span data-stu-id="ed17e-109">It provides convenient ways to install, update, and uninstall.</span></span> <span data-ttu-id="ed17e-110">É parecido com outros gerenciadores de pacotes, como o `apt` ou `yum`.</span><span class="sxs-lookup"><span data-stu-id="ed17e-110">It's similar to other package managers such as `apt` or `yum`.</span></span>
<span data-ttu-id="ed17e-111">Se você não tiver o homebrew disponível em seu sistema, [instale-o](https://docs.brew.sh/Installation.html) antes de continuar.</span><span class="sxs-lookup"><span data-stu-id="ed17e-111">If you don't have homebrew available on your system, [install homebrew](https://docs.brew.sh/Installation.html) before continuing.</span></span>

### <a name="install-with-homebrew"></a><span data-ttu-id="ed17e-112">Instalar com o homebrew</span><span class="sxs-lookup"><span data-stu-id="ed17e-112">Install with homebrew</span></span>

<span data-ttu-id="ed17e-113">Você pode instalar a CLI atualizando suas informações de repositório brew e executando o comando `install`:</span><span class="sxs-lookup"><span data-stu-id="ed17e-113">You can install the CLI by updating your brew repository information, and then running the `install` command:</span></span>

```bash
brew update && brew install azure-cli
```

<span data-ttu-id="ed17e-114">É possível executar a CLI do Azure com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="ed17e-114">You can then run the Azure CLI with the `az` command.</span></span>

### <a name="update-with-homebrew"></a><span data-ttu-id="ed17e-115">Atualizar com o homebrew</span><span class="sxs-lookup"><span data-stu-id="ed17e-115">Update with homebrew</span></span>

<span data-ttu-id="ed17e-116">A CLI é atualizada regularmente com correções de bugs, aprimoramentos, novos recursos e funcionalidade de visualização.</span><span class="sxs-lookup"><span data-stu-id="ed17e-116">The CLI is regularly updated with bug fixes, improvements, new features, and preview functionality.</span></span> <span data-ttu-id="ed17e-117">Uma nova versão fica disponível aproximadamente a cada duas semanas.</span><span class="sxs-lookup"><span data-stu-id="ed17e-117">A new release is available roughly every two weeks.</span></span> <span data-ttu-id="ed17e-118">Você precisará atualizar as informações do repositório local, assim como o pacote da CLI.</span><span class="sxs-lookup"><span data-stu-id="ed17e-118">You will need to update your local repository information, and then update the CLI package.</span></span>

```bash
brew update && brew upgrade azure-cli
```

### <a name="troubleshooting"></a><span data-ttu-id="ed17e-119">solução de problemas</span><span class="sxs-lookup"><span data-stu-id="ed17e-119">Troubleshooting</span></span>

<span data-ttu-id="ed17e-120">Você encontrou um problema ao instalar ou atualizar a CLI com o homebrew?</span><span class="sxs-lookup"><span data-stu-id="ed17e-120">Did you encounter a problem when installing or updating the CLI with homebrew?</span></span> <span data-ttu-id="ed17e-121">Veja alguns erros comuns que podem ocorrer e maneiras de diagnosticá-los e resolvê-los.</span><span class="sxs-lookup"><span data-stu-id="ed17e-121">Here are some common errors that might occur, and ways to diagnose and resolve them.</span></span>

#### <a name="unable-to-find-python-or-installed-packages"></a><span data-ttu-id="ed17e-122">Não é possível localizar o Python ou os pacotes instalados</span><span class="sxs-lookup"><span data-stu-id="ed17e-122">Unable to find Python or installed packages</span></span>

<span data-ttu-id="ed17e-123">Se a instalação não conseguir localizar o Python nem os pacotes instalados, poderá haver uma incompatibilidade de versão secundária ou outro problema que ocorreu durante a instalação do homebrew.</span><span class="sxs-lookup"><span data-stu-id="ed17e-123">If your install is unable to find Python or installed packages, there may be a minor version mismatch or other issue which occurred during homebrew installation.</span></span> <span data-ttu-id="ed17e-124">Como a CLI não usa um virtualenv, ela depende de conseguir localizar as versões corretas do Python instaladas pelo homebrew.</span><span class="sxs-lookup"><span data-stu-id="ed17e-124">Since the CLI does not use a virtualenv, it relies on being able to find correct versions of Python installed by homebrew.</span></span> <span data-ttu-id="ed17e-125">Você pode corrigir esses problemas vinculando novamente a instalação do Python:</span><span class="sxs-lookup"><span data-stu-id="ed17e-125">You may be able to fix these issues by re-linking your Python installation:</span></span>

```bash
brew link --overwrite python3
```

#### <a name="the-cli-version-is-out-of-date"></a><span data-ttu-id="ed17e-126">A versão da CLI está desatualizada</span><span class="sxs-lookup"><span data-stu-id="ed17e-126">The CLI version is out of date</span></span>

<span data-ttu-id="ed17e-127">Se você achar que a versão instalada da CLI pode estar desatualizada, precisará executar um comando `brew update`, seguido de `brew upgrade azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="ed17e-127">If you think that your installed CLI version might be out of date, you will need to run a `brew update` command, followed by `brew upgrade azure-cli`.</span></span> <span data-ttu-id="ed17e-128">Se isso não atualizar a CLI, lembre que os pacotes homebrew podem ser implementados mais lentamente que as versões gerais.</span><span class="sxs-lookup"><span data-stu-id="ed17e-128">If this does not update the CLI, be aware that homebrew packages may roll out more slowly than general releases.</span></span> <span data-ttu-id="ed17e-129">Se precisar de instalações mais atuais da CLI, deverá [instalar manualmente](#manage-the-cli-manually).</span><span class="sxs-lookup"><span data-stu-id="ed17e-129">If you require bleeding-edge installs of the CLI, then you should [install manually](#manage-the-cli-manually).</span></span>

### <a name="uninstall-with-homebrew"></a><span data-ttu-id="ed17e-130">Desinstalar com o homebrew</span><span class="sxs-lookup"><span data-stu-id="ed17e-130">Uninstall with homebrew</span></span>

<span data-ttu-id="ed17e-131">Se você decidiu desinstalar a CLI do Azure, lamentamos sua saída.</span><span class="sxs-lookup"><span data-stu-id="ed17e-131">If you ever decide to uninstall the Azure CLI, we're sorry to see you go.</span></span> <span data-ttu-id="ed17e-132">Antes de desinstalar, use o comando `az feedback` para nos fornecer algumas razões por ter escolhido desinstalar e como poderíamos melhorar a experiência da CLI.</span><span class="sxs-lookup"><span data-stu-id="ed17e-132">Before you uninstall, use the `az feedback` command to give us some reasons why you chose to uninstall and how we could improve the CLI experience.</span></span> <span data-ttu-id="ed17e-133">Queremos assegurar que a CLI do Azure não tenha bugs e seja amigável o máximo possível.</span><span class="sxs-lookup"><span data-stu-id="ed17e-133">We want to make sure that the Azure CLI is as bug-free and user-friendly as we can make it.</span></span> <span data-ttu-id="ed17e-134">Você também pode [registrar um problema do github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="ed17e-134">You can also [file a github issue](https://github.com/Azure/azure-cli/issues).</span></span>

<span data-ttu-id="ed17e-135">Se você instalou com o homebrew, também deve usá-lo para desinstalar.</span><span class="sxs-lookup"><span data-stu-id="ed17e-135">If you installed with homebrew, you should also use it to uninstall.</span></span>

```bash
brew uninstall azure-cli
```

## <a name="install-the-cli-manually"></a><span data-ttu-id="ed17e-136">Instalar a CLI manualmente</span><span class="sxs-lookup"><span data-stu-id="ed17e-136">Install the CLI manually</span></span>

<span data-ttu-id="ed17e-137">Se você não pode ou não deseja depender do homebrew para gerenciar a instalação da CLI, pode instalar manualmente.</span><span class="sxs-lookup"><span data-stu-id="ed17e-137">If you can't or don't want to rely on homebrew to manage the CLI install for you, then you can manually install.</span></span>

<span data-ttu-id="ed17e-138">Siga as [instruções de instalação manual do Linux](install-azure-cli-linux.md) para instalar manualmente no macOS.</span><span class="sxs-lookup"><span data-stu-id="ed17e-138">Follow the [manual Linux installation instructions](install-azure-cli-linux.md) to install manually on macOS.</span></span> <span data-ttu-id="ed17e-139">as versões 10.9 e posterior do macOS devem incluir todas as dependências necessárias.</span><span class="sxs-lookup"><span data-stu-id="ed17e-139">macOS versions 10.9 and later should include all of the required dependencies.</span></span>
