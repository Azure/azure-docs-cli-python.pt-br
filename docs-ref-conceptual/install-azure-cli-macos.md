---
title: Instalar a CLI do Azure para macOS
description: Como instalar a CLI do Azure no macOS
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/05/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 61be6c31e7251c8b374bf09072a9ecba9b914342
ms.sourcegitcommit: 1987a39809f9865034b27130e56f30b2bd1eb72c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/19/2019
ms.locfileid: "56422044"
---
# <a name="install-azure-cli-on-macos"></a><span data-ttu-id="7f179-103">Instalar a CLI do Azure no macOS</span><span class="sxs-lookup"><span data-stu-id="7f179-103">Install Azure CLI on macOS</span></span>

<span data-ttu-id="7f179-104">Para a plataforma macOS, você pode instalar a CLI do Azure com o [gerenciador de pacotes homebrew](https://brew.sh).</span><span class="sxs-lookup"><span data-stu-id="7f179-104">For the macOS platform, you can install the Azure CLI with [homebrew package manager](https://brew.sh).</span></span> <span data-ttu-id="7f179-105">O Homebrew torna mais fácil manter a instalação da CLI atualizada.</span><span class="sxs-lookup"><span data-stu-id="7f179-105">Homebrew makes it easy to keep your installation of the CLI update to date.</span></span> <span data-ttu-id="7f179-106">O pacote da CLI foi testado em versões do macOS 10.9 e posteriores.</span><span class="sxs-lookup"><span data-stu-id="7f179-106">The CLI package has been tested on macOS versions 10.9 and later.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

## <a name="install"></a><span data-ttu-id="7f179-107">Instalar</span><span class="sxs-lookup"><span data-stu-id="7f179-107">Install</span></span>

<span data-ttu-id="7f179-108">O homebrew é a maneira mais fácil de gerenciar a instalação da CLI.</span><span class="sxs-lookup"><span data-stu-id="7f179-108">Homebrew is the easiest way to manage your CLI install.</span></span> <span data-ttu-id="7f179-109">Ele fornece maneiras convenientes de instalar, atualizar e desinstalar.</span><span class="sxs-lookup"><span data-stu-id="7f179-109">It provides convenient ways to install, update, and uninstall.</span></span>
<span data-ttu-id="7f179-110">Se você não tiver o homebrew disponível em seu sistema, [instale-o](https://docs.brew.sh/Installation.html) antes de continuar.</span><span class="sxs-lookup"><span data-stu-id="7f179-110">If you don't have homebrew available on your system, [install homebrew](https://docs.brew.sh/Installation.html) before continuing.</span></span>

<span data-ttu-id="7f179-111">Você pode instalar a CLI atualizando suas informações de repositório brew e executando o comando `install`:</span><span class="sxs-lookup"><span data-stu-id="7f179-111">You can install the CLI by updating your brew repository information, and then running the `install` command:</span></span>

```bash
brew update && brew install azure-cli
```

> [!IMPORTANT]
>
> <span data-ttu-id="7f179-112">A CLI do Azure possui uma dependência do pacote `python3` no Homebrew de pacote e irá instalá-lo em seu sistema, mesmo se o Python 2 estiver disponível.</span><span class="sxs-lookup"><span data-stu-id="7f179-112">The Azure CLI has a dependency on the `python3` package in Homebrew, and will install it on your system, even if Python 2 is available.</span></span> <span data-ttu-id="7f179-113">A CLI do Azure é certamente compatível com a versão mais recente do `python3` publicada no Homebrew.</span><span class="sxs-lookup"><span data-stu-id="7f179-113">The Azure CLI is guaranteed to be compatible with the latest version of `python3` published on Homebrew.</span></span>

<span data-ttu-id="7f179-114">É possível executar a CLI do Azure com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="7f179-114">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="7f179-115">Para entrar, use o comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="7f179-115">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="7f179-116">Para saber mais sobre os diferentes métodos de autenticação, confira [Entrar com a CLI do Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="7f179-116">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="7f179-117">solução de problemas</span><span class="sxs-lookup"><span data-stu-id="7f179-117">Troubleshooting</span></span>

<span data-ttu-id="7f179-118">Se você encontrar um problema ao instalar a CLI através do Homebrew, aqui estão alguns erros comuns.</span><span class="sxs-lookup"><span data-stu-id="7f179-118">If you encounter a problem when installing the CLI through Homebrew, here are some common errors.</span></span> <span data-ttu-id="7f179-119">Se você tiver um problema não abordado aqui, [arquive um problema no github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="7f179-119">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="unable-to-find-python-or-installed-packages"></a><span data-ttu-id="7f179-120">Não é possível localizar o Python ou os pacotes instalados</span><span class="sxs-lookup"><span data-stu-id="7f179-120">Unable to find Python or installed packages</span></span>

<span data-ttu-id="7f179-121">Pode haver uma pequena incompatibilidade de versão ou outro problema durante a instalação do homebrew.</span><span class="sxs-lookup"><span data-stu-id="7f179-121">There may be a minor version mismatch or other issue during homebrew installation.</span></span> <span data-ttu-id="7f179-122">A CLI não usa um ambiente virtual Python, portanto, ela se baseia em localizar a versão instalada do Python.</span><span class="sxs-lookup"><span data-stu-id="7f179-122">The CLI doesn't use a Python virtual environment, so it relies on finding the installed Python version.</span></span> <span data-ttu-id="7f179-123">Uma possível correção é instalar e revincular a dependência `python3` do Homebrew.</span><span class="sxs-lookup"><span data-stu-id="7f179-123">A possible fix is to install and relink the `python3` dependency from Homebrew.</span></span>

```bash
brew update && brew install python3 && brew upgrade python3
brew link --overwrite python3
```

### <a name="cli-version-1x-is-installed"></a><span data-ttu-id="7f179-124">A versão 1.x da CLI está instalada</span><span class="sxs-lookup"><span data-stu-id="7f179-124">CLI version 1.x is installed</span></span>

<span data-ttu-id="7f179-125">Se tiver sido instalada uma versão desatualizada, pode ser devido a um cache de homebrew obsoleto.</span><span class="sxs-lookup"><span data-stu-id="7f179-125">If an out-of-date version was installed, it could be because of a stale homebrew cache.</span></span> <span data-ttu-id="7f179-126">Siga as instruções de [atualização](#Update).</span><span class="sxs-lookup"><span data-stu-id="7f179-126">Follow the [update](#Update) instructions.</span></span>

## <a name="update"></a><span data-ttu-id="7f179-127">Atualizar</span><span class="sxs-lookup"><span data-stu-id="7f179-127">Update</span></span>

<span data-ttu-id="7f179-128">A CLI é atualizada regularmente com correções de bugs, aprimoramentos, novos recursos e funcionalidade de visualização.</span><span class="sxs-lookup"><span data-stu-id="7f179-128">The CLI is regularly updated with bug fixes, improvements, new features, and preview functionality.</span></span> <span data-ttu-id="7f179-129">Uma nova versão fica disponível aproximadamente a cada duas semanas.</span><span class="sxs-lookup"><span data-stu-id="7f179-129">A new release is available roughly every two weeks.</span></span> <span data-ttu-id="7f179-130">Atualize as informações do repositório local e atualize o pacote `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="7f179-130">Update your local repository information and then upgrade the `azure-cli` package.</span></span>

```bash
brew update && brew upgrade azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="7f179-131">Desinstalar</span><span class="sxs-lookup"><span data-stu-id="7f179-131">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="7f179-132">Use o homebrew para desinstalar o pacote `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="7f179-132">Use homebrew to uninstall the `azure-cli` package.</span></span>

```bash
brew uninstall azure-cli
```

## <a name="other-installation-methods"></a><span data-ttu-id="7f179-133">Outros métodos de instalação</span><span class="sxs-lookup"><span data-stu-id="7f179-133">Other installation methods</span></span>

<span data-ttu-id="7f179-134">Se você não pode usar o Homebrew para instalar a CLI do Azure em seu ambiente, é possível usar as instruções manuais para o Linux.</span><span class="sxs-lookup"><span data-stu-id="7f179-134">If you can't use homebrew to install the Azure CLI in your environment, it's possible to use the manual instructions for Linux.</span></span> <span data-ttu-id="7f179-135">Observe que esse processo não é oficialmente mantido para ser compatível com o macOS.</span><span class="sxs-lookup"><span data-stu-id="7f179-135">Note that this process is not officially maintained to be compatible with macOS.</span></span> <span data-ttu-id="7f179-136">É sempre recomendável usar um gerenciador de pacotes, como o Homebrew.</span><span class="sxs-lookup"><span data-stu-id="7f179-136">Using a package manager such as Homebrew is always recommended.</span></span> <span data-ttu-id="7f179-137">Somente use o método de instalação manual se não tiver nenhuma outra opção disponível.</span><span class="sxs-lookup"><span data-stu-id="7f179-137">Only use the manual installation method if you have no other option available.</span></span>

<span data-ttu-id="7f179-138">Para as instruções de instalação manual, confira [Instalar manualmente a CLI do Azure no Linux](install-azure-cli-linux.md).</span><span class="sxs-lookup"><span data-stu-id="7f179-138">For the manual installation instructions, see [Install Azure CLI on Linux manually](install-azure-cli-linux.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="7f179-139">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="7f179-139">Next Steps</span></span>

<span data-ttu-id="7f179-140">Agora que você instalou a CLI do Azure, faça um tour breve de seus recursos e comandos comuns.</span><span class="sxs-lookup"><span data-stu-id="7f179-140">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="7f179-141">Introdução à CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="7f179-141">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
