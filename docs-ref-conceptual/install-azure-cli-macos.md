---
title: Instalar a CLI do Azure para macOS
description: Como instalar a CLI do Azure 2.0 no macOS
keywords: CLI do Azure, Instalar CLI do Azure, macos do azure, macos instalar azure
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/18
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 36fd2604677db0b7f820ee11884bf790fb1d75cb
ms.sourcegitcommit: 8606f36963e8daa6448d637393d1e4ef2c9859a0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/01/2018
---
# <a name="install-azure-cli-20-on-macos"></a><span data-ttu-id="8efbf-104">Instalar CLI do Azure 2.0 no macOS</span><span class="sxs-lookup"><span data-stu-id="8efbf-104">Install Azure CLI 2.0 on macOS</span></span>

<span data-ttu-id="8efbf-105">Para a plataforma macOS, você pode instalar a CLI do Azure usando o [gerenciador de pacotes homebrew](http://brew.sh).</span><span class="sxs-lookup"><span data-stu-id="8efbf-105">For the macOS platform, you can install the Azure CLI either through the [homebrew package manager](http://brew.sh).</span></span> <span data-ttu-id="8efbf-106">O Homebrew torna mais fácil manter a instalação da CLI atualizada.</span><span class="sxs-lookup"><span data-stu-id="8efbf-106">Homebrew makes it easy to keep your installation of the CLI update to date.</span></span> <span data-ttu-id="8efbf-107">O pacote da CLI foi testado em versões do macOS 10.9 e posteriores.</span><span class="sxs-lookup"><span data-stu-id="8efbf-107">The CLI package has been tested on macOS versions 10.9 and later.</span></span>

## <a name="install"></a><span data-ttu-id="8efbf-108">Instalar</span><span class="sxs-lookup"><span data-stu-id="8efbf-108">Install</span></span>

<span data-ttu-id="8efbf-109">O homebrew é a maneira mais fácil de gerenciar a instalação da CLI.</span><span class="sxs-lookup"><span data-stu-id="8efbf-109">Homebrew is the easiest way to manage your CLI install.</span></span> <span data-ttu-id="8efbf-110">Ele fornece maneiras convenientes de instalar, atualizar e desinstalar.</span><span class="sxs-lookup"><span data-stu-id="8efbf-110">It provides convenient ways to install, update, and uninstall.</span></span> <span data-ttu-id="8efbf-111">Se você não tiver o homebrew disponível em seu sistema, [instale-o](https://docs.brew.sh/Installation.html) antes de continuar.</span><span class="sxs-lookup"><span data-stu-id="8efbf-111">If you don't have homebrew available on your system, [install homebrew](https://docs.brew.sh/Installation.html) before continuing.</span></span>

<span data-ttu-id="8efbf-112">Você pode instalar a CLI atualizando suas informações de repositório brew e executando o comando `install`:</span><span class="sxs-lookup"><span data-stu-id="8efbf-112">You can install the CLI by updating your brew repository information, and then running the `install` command:</span></span>

```bash
brew update && brew install azure-cli
```

<span data-ttu-id="8efbf-113">É possível executar a CLI do Azure com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="8efbf-113">You can then run the Azure CLI with the `az` command.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="8efbf-114">solução de problemas</span><span class="sxs-lookup"><span data-stu-id="8efbf-114">Troubleshooting</span></span>

<span data-ttu-id="8efbf-115">Se você encontrar um problema ao instalar a CLI através do Homebrew, aqui estão alguns erros comuns.</span><span class="sxs-lookup"><span data-stu-id="8efbf-115">If you encounter a problem when installing the CLI through Homebrew, here are some common errors.</span></span> <span data-ttu-id="8efbf-116">Se o problema não estiver listado aqui, [registre um problema no github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="8efbf-116">If your issue is not listed here, please [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="unable-to-find-python-or-installed-packages"></a><span data-ttu-id="8efbf-117">Não é possível localizar o Python ou os pacotes instalados</span><span class="sxs-lookup"><span data-stu-id="8efbf-117">Unable to find Python or installed packages</span></span>

<span data-ttu-id="8efbf-118">Se a instalação não conseguir localizar o Python nem os pacotes instalados, poderá haver uma incompatibilidade de versão secundária ou outro problema que ocorreu durante a instalação do homebrew.</span><span class="sxs-lookup"><span data-stu-id="8efbf-118">If your install is unable to find Python or installed packages, there may be a minor version mismatch or other issue that occurred during homebrew installation.</span></span> <span data-ttu-id="8efbf-119">Como a CLI não usa um ambiente virtual Python, ela depende de conseguir localizar as versões corretas do Python.</span><span class="sxs-lookup"><span data-stu-id="8efbf-119">Since the CLI does not use a Python virtual environment, it relies on being able to find correct Python version.</span></span> <span data-ttu-id="8efbf-120">Você pode corrigir esses problemas vinculando novamente a instalação do Python.</span><span class="sxs-lookup"><span data-stu-id="8efbf-120">You may be able to fix these issues by relinking your Python installation.</span></span>

```bash
brew link --overwrite python3
```

### <a name="cli-version-1x-is-installed"></a><span data-ttu-id="8efbf-121">A versão 1.x da CLI está instalada</span><span class="sxs-lookup"><span data-stu-id="8efbf-121">CLI version 1.x is installed</span></span>

<span data-ttu-id="8efbf-122">Se tiver sido instalada uma versão desatualizada, pode ser devido a um cache de homebrew obsoleto.</span><span class="sxs-lookup"><span data-stu-id="8efbf-122">If an out-of-date version was installed, it could be due to a stale homebrew cache.</span></span> <span data-ttu-id="8efbf-123">Siga as instruções de [atualização](#Update).</span><span class="sxs-lookup"><span data-stu-id="8efbf-123">Follow the [update](#Update) instructions.</span></span>

## <a name="update"></a><span data-ttu-id="8efbf-124">Atualizar</span><span class="sxs-lookup"><span data-stu-id="8efbf-124">Update</span></span>

<span data-ttu-id="8efbf-125">A CLI é atualizada regularmente com correções de bugs, aprimoramentos, novos recursos e funcionalidade de visualização.</span><span class="sxs-lookup"><span data-stu-id="8efbf-125">The CLI is regularly updated with bug fixes, improvements, new features, and preview functionality.</span></span> <span data-ttu-id="8efbf-126">Uma nova versão fica disponível aproximadamente a cada duas semanas.</span><span class="sxs-lookup"><span data-stu-id="8efbf-126">A new release is available roughly every two weeks.</span></span> <span data-ttu-id="8efbf-127">Atualize as informações do repositório local e atualize o pacote `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="8efbf-127">Update your local repository information and then upgrade the `azure-cli` package.</span></span>

```bash
brew update && brew upgrade azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="8efbf-128">Desinstalar</span><span class="sxs-lookup"><span data-stu-id="8efbf-128">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="8efbf-129">Use o homebrew para desinstalar o pacote `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="8efbf-129">Use homebrew to uninstall the `azure-cli` package.</span></span>

```bash
brew uninstall azure-cli
```
