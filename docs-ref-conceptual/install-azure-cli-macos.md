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
ms.openlocfilehash: 40415bc7bec056dc1564c58c8df3f7263bee348c
ms.sourcegitcommit: f40bd067ece4e6ec13e259782ed8db3e33b61a75
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "53593159"
---
# <a name="install-azure-cli-on-macos"></a><span data-ttu-id="486af-103">Instalar a CLI do Azure no macOS</span><span class="sxs-lookup"><span data-stu-id="486af-103">Install Azure CLI on macOS</span></span>

<span data-ttu-id="486af-104">Para a plataforma macOS, você pode instalar a CLI do Azure com o [gerenciador de pacotes homebrew](https://brew.sh).</span><span class="sxs-lookup"><span data-stu-id="486af-104">For the macOS platform, you can install the Azure CLI with [homebrew package manager](https://brew.sh).</span></span> <span data-ttu-id="486af-105">O Homebrew torna mais fácil manter a instalação da CLI atualizada.</span><span class="sxs-lookup"><span data-stu-id="486af-105">Homebrew makes it easy to keep your installation of the CLI update to date.</span></span> <span data-ttu-id="486af-106">O pacote da CLI foi testado em versões do macOS 10.9 e posteriores.</span><span class="sxs-lookup"><span data-stu-id="486af-106">The CLI package has been tested on macOS versions 10.9 and later.</span></span>

## <a name="install"></a><span data-ttu-id="486af-107">Instalar</span><span class="sxs-lookup"><span data-stu-id="486af-107">Install</span></span>

<span data-ttu-id="486af-108">O homebrew é a maneira mais fácil de gerenciar a instalação da CLI.</span><span class="sxs-lookup"><span data-stu-id="486af-108">Homebrew is the easiest way to manage your CLI install.</span></span> <span data-ttu-id="486af-109">Ele fornece maneiras convenientes de instalar, atualizar e desinstalar.</span><span class="sxs-lookup"><span data-stu-id="486af-109">It provides convenient ways to install, update, and uninstall.</span></span>
<span data-ttu-id="486af-110">Se você não tiver o homebrew disponível em seu sistema, [instale-o](https://docs.brew.sh/Installation.html) antes de continuar.</span><span class="sxs-lookup"><span data-stu-id="486af-110">If you don't have homebrew available on your system, [install homebrew](https://docs.brew.sh/Installation.html) before continuing.</span></span>

<span data-ttu-id="486af-111">Você pode instalar a CLI atualizando suas informações de repositório brew e executando o comando `install`:</span><span class="sxs-lookup"><span data-stu-id="486af-111">You can install the CLI by updating your brew repository information, and then running the `install` command:</span></span>

```bash
brew update && brew install azure-cli
```

<span data-ttu-id="486af-112">É possível executar a CLI do Azure com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="486af-112">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="486af-113">Para entrar, use o comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="486af-113">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="486af-114">Para saber mais sobre os diferentes métodos de autenticação, confira [Entrar com a CLI do Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="486af-114">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="486af-115">solução de problemas</span><span class="sxs-lookup"><span data-stu-id="486af-115">Troubleshooting</span></span>

<span data-ttu-id="486af-116">Se você encontrar um problema ao instalar a CLI através do Homebrew, aqui estão alguns erros comuns.</span><span class="sxs-lookup"><span data-stu-id="486af-116">If you encounter a problem when installing the CLI through Homebrew, here are some common errors.</span></span> <span data-ttu-id="486af-117">Se você tiver um problema não abordado aqui, [arquive um problema no github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="486af-117">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="unable-to-find-python-or-installed-packages"></a><span data-ttu-id="486af-118">Não é possível localizar o Python ou os pacotes instalados</span><span class="sxs-lookup"><span data-stu-id="486af-118">Unable to find Python or installed packages</span></span>

<span data-ttu-id="486af-119">Pode haver uma pequena incompatibilidade de versão ou outro problema durante a instalação do homebrew.</span><span class="sxs-lookup"><span data-stu-id="486af-119">There may be a minor version mismatch or other issue during homebrew installation.</span></span> <span data-ttu-id="486af-120">A CLI não usa um ambiente virtual Python, portanto, ela se baseia em localizar a versão instalada do Python.</span><span class="sxs-lookup"><span data-stu-id="486af-120">The CLI doesn't use a Python virtual environment, so it relies on finding the installed Python version.</span></span> <span data-ttu-id="486af-121">Uma possível correção é instalar e revincular a dependência `python3` do Homebrew.</span><span class="sxs-lookup"><span data-stu-id="486af-121">A possible fix is to install and relink the `python3` dependency from Homebrew.</span></span>

```bash
brew update && brew install python3 && brew upgrade python3
brew link --overwrite python3
```

### <a name="cli-version-1x-is-installed"></a><span data-ttu-id="486af-122">A versão 1.x da CLI está instalada</span><span class="sxs-lookup"><span data-stu-id="486af-122">CLI version 1.x is installed</span></span>

<span data-ttu-id="486af-123">Se tiver sido instalada uma versão desatualizada, pode ser devido a um cache de homebrew obsoleto.</span><span class="sxs-lookup"><span data-stu-id="486af-123">If an out-of-date version was installed, it could be because of a stale homebrew cache.</span></span> <span data-ttu-id="486af-124">Siga as instruções de [atualização](#Update).</span><span class="sxs-lookup"><span data-stu-id="486af-124">Follow the [update](#Update) instructions.</span></span>

## <a name="update"></a><span data-ttu-id="486af-125">Atualizar</span><span class="sxs-lookup"><span data-stu-id="486af-125">Update</span></span>

<span data-ttu-id="486af-126">A CLI é atualizada regularmente com correções de bugs, aprimoramentos, novos recursos e funcionalidade de visualização.</span><span class="sxs-lookup"><span data-stu-id="486af-126">The CLI is regularly updated with bug fixes, improvements, new features, and preview functionality.</span></span> <span data-ttu-id="486af-127">Uma nova versão fica disponível aproximadamente a cada duas semanas.</span><span class="sxs-lookup"><span data-stu-id="486af-127">A new release is available roughly every two weeks.</span></span> <span data-ttu-id="486af-128">Atualize as informações do repositório local e atualize o pacote `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="486af-128">Update your local repository information and then upgrade the `azure-cli` package.</span></span>

```bash
brew update && brew upgrade azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="486af-129">Desinstalar</span><span class="sxs-lookup"><span data-stu-id="486af-129">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="486af-130">Use o homebrew para desinstalar o pacote `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="486af-130">Use homebrew to uninstall the `azure-cli` package.</span></span>

```bash
brew uninstall azure-cli
```

## <a name="other-installation-methods"></a><span data-ttu-id="486af-131">Outros métodos de instalação</span><span class="sxs-lookup"><span data-stu-id="486af-131">Other installation methods</span></span>

<span data-ttu-id="486af-132">Se você não pode usar o Homebrew para instalar a CLI do Azure em seu ambiente, é possível usar as instruções manuais para o Linux.</span><span class="sxs-lookup"><span data-stu-id="486af-132">If you can't use homebrew to install the Azure CLI in your environment, it's possible to use the manual instructions for Linux.</span></span> <span data-ttu-id="486af-133">Observe que esse processo não é oficialmente mantido para ser compatível com o macOS.</span><span class="sxs-lookup"><span data-stu-id="486af-133">Note that this process is not officially maintained to be compatible with macOS.</span></span> <span data-ttu-id="486af-134">É sempre recomendável usar um gerenciador de pacotes, como o Homebrew.</span><span class="sxs-lookup"><span data-stu-id="486af-134">Using a package manager such as Homebrew is always recommended.</span></span> <span data-ttu-id="486af-135">Somente use o método de instalação manual se não tiver nenhuma outra opção disponível.</span><span class="sxs-lookup"><span data-stu-id="486af-135">Only use the manual installation method if you have no other option available.</span></span>

<span data-ttu-id="486af-136">Para as instruções de instalação manual, confira [Instalar manualmente a CLI do Azure no Linux](install-azure-cli-linux.md).</span><span class="sxs-lookup"><span data-stu-id="486af-136">For the manual installation instructions, see [Install Azure CLI on Linux manually](install-azure-cli-linux.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="486af-137">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="486af-137">Next Steps</span></span>

<span data-ttu-id="486af-138">Agora que você instalou a CLI do Azure, faça um tour breve de seus recursos e comandos comuns.</span><span class="sxs-lookup"><span data-stu-id="486af-138">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="486af-139">Introdução à CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="486af-139">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
