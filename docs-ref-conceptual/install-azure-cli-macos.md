---
title: Instalar a CLI do Azure para macOS
description: Como instalar a CLI do Azure no macOS
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 9eb816ef68d24d1dbbaaeb5fd4877580edbe87ad
ms.sourcegitcommit: c4462456dfb17993f098d47c37bc19f4d78b8179
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/25/2018
ms.locfileid: "47177650"
---
# <a name="install-azure-cli-on-macos"></a><span data-ttu-id="299c9-103">Instalar a CLI do Azure no macOS</span><span class="sxs-lookup"><span data-stu-id="299c9-103">Install Azure CLI on macOS</span></span>

<span data-ttu-id="299c9-104">Para a plataforma macOS, você pode instalar a CLI do Azure com o [gerenciador de pacotes homebrew](https://brew.sh).</span><span class="sxs-lookup"><span data-stu-id="299c9-104">For the macOS platform, you can install the Azure CLI with [homebrew package manager](https://brew.sh).</span></span> <span data-ttu-id="299c9-105">O Homebrew torna mais fácil manter a instalação da CLI atualizada.</span><span class="sxs-lookup"><span data-stu-id="299c9-105">Homebrew makes it easy to keep your installation of the CLI update to date.</span></span> <span data-ttu-id="299c9-106">O pacote da CLI foi testado em versões do macOS 10.9 e posteriores.</span><span class="sxs-lookup"><span data-stu-id="299c9-106">The CLI package has been tested on macOS versions 10.9 and later.</span></span>

## <a name="install"></a><span data-ttu-id="299c9-107">Instalar</span><span class="sxs-lookup"><span data-stu-id="299c9-107">Install</span></span>

<span data-ttu-id="299c9-108">O homebrew é a maneira mais fácil de gerenciar a instalação da CLI.</span><span class="sxs-lookup"><span data-stu-id="299c9-108">Homebrew is the easiest way to manage your CLI install.</span></span> <span data-ttu-id="299c9-109">Ele fornece maneiras convenientes de instalar, atualizar e desinstalar.</span><span class="sxs-lookup"><span data-stu-id="299c9-109">It provides convenient ways to install, update, and uninstall.</span></span>
<span data-ttu-id="299c9-110">Se você não tiver o homebrew disponível em seu sistema, [instale-o](https://docs.brew.sh/Installation.html) antes de continuar.</span><span class="sxs-lookup"><span data-stu-id="299c9-110">If you don't have homebrew available on your system, [install homebrew](https://docs.brew.sh/Installation.html) before continuing.</span></span>

<span data-ttu-id="299c9-111">Você pode instalar a CLI atualizando suas informações de repositório brew e executando o comando `install`:</span><span class="sxs-lookup"><span data-stu-id="299c9-111">You can install the CLI by updating your brew repository information, and then running the `install` command:</span></span>

```bash
brew update && brew install azure-cli
```

<span data-ttu-id="299c9-112">É possível executar a CLI do Azure com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="299c9-112">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="299c9-113">Para entrar, use o comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="299c9-113">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="299c9-114">Para saber mais sobre os diferentes métodos de autenticação, confira [Entrar com a CLI do Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="299c9-114">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="299c9-115">solução de problemas</span><span class="sxs-lookup"><span data-stu-id="299c9-115">Troubleshooting</span></span>

<span data-ttu-id="299c9-116">Se você encontrar um problema ao instalar a CLI através do Homebrew, aqui estão alguns erros comuns.</span><span class="sxs-lookup"><span data-stu-id="299c9-116">If you encounter a problem when installing the CLI through Homebrew, here are some common errors.</span></span> <span data-ttu-id="299c9-117">Se você tiver um problema não abordado aqui, [arquive um problema no github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="299c9-117">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="unable-to-find-python-or-installed-packages"></a><span data-ttu-id="299c9-118">Não é possível localizar o Python ou os pacotes instalados</span><span class="sxs-lookup"><span data-stu-id="299c9-118">Unable to find Python or installed packages</span></span>

<span data-ttu-id="299c9-119">Pode haver uma pequena incompatibilidade de versão ou outro problema durante a instalação do homebrew.</span><span class="sxs-lookup"><span data-stu-id="299c9-119">There may be a minor version mismatch or other issue during homebrew installation.</span></span> <span data-ttu-id="299c9-120">A CLI não usa um ambiente virtual Python, portanto, ela se baseia em localizar a versão instalada do Python.</span><span class="sxs-lookup"><span data-stu-id="299c9-120">The CLI doesn't use a Python virtual environment, so it relies on finding the installed Python version.</span></span> <span data-ttu-id="299c9-121">Uma possível correção é instalar e revincular a dependência `python3` do Homebrew.</span><span class="sxs-lookup"><span data-stu-id="299c9-121">A possible fix is to install and relink the `python3` dependency from Homebrew.</span></span>

```bash
brew update && brew install python3 && brew upgrade python3
brew link --overwrite python3
```

### <a name="cli-version-1x-is-installed"></a><span data-ttu-id="299c9-122">A versão 1.x da CLI está instalada</span><span class="sxs-lookup"><span data-stu-id="299c9-122">CLI version 1.x is installed</span></span>

<span data-ttu-id="299c9-123">Se tiver sido instalada uma versão desatualizada, pode ser devido a um cache de homebrew obsoleto.</span><span class="sxs-lookup"><span data-stu-id="299c9-123">If an out-of-date version was installed, it could be because of a stale homebrew cache.</span></span> <span data-ttu-id="299c9-124">Siga as instruções de [atualização](#Update).</span><span class="sxs-lookup"><span data-stu-id="299c9-124">Follow the [update](#Update) instructions.</span></span>

## <a name="update"></a><span data-ttu-id="299c9-125">Atualizar</span><span class="sxs-lookup"><span data-stu-id="299c9-125">Update</span></span>

<span data-ttu-id="299c9-126">A CLI é atualizada regularmente com correções de bugs, aprimoramentos, novos recursos e funcionalidade de visualização.</span><span class="sxs-lookup"><span data-stu-id="299c9-126">The CLI is regularly updated with bug fixes, improvements, new features, and preview functionality.</span></span> <span data-ttu-id="299c9-127">Uma nova versão fica disponível aproximadamente a cada duas semanas.</span><span class="sxs-lookup"><span data-stu-id="299c9-127">A new release is available roughly every two weeks.</span></span> <span data-ttu-id="299c9-128">Atualize as informações do repositório local e atualize o pacote `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="299c9-128">Update your local repository information and then upgrade the `azure-cli` package.</span></span>

```bash
brew update && brew upgrade azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="299c9-129">Desinstalar</span><span class="sxs-lookup"><span data-stu-id="299c9-129">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="299c9-130">Use o homebrew para desinstalar o pacote `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="299c9-130">Use homebrew to uninstall the `azure-cli` package.</span></span>

```bash
brew uninstall azure-cli
```

## <a name="next-steps"></a><span data-ttu-id="299c9-131">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="299c9-131">Next Steps</span></span>

<span data-ttu-id="299c9-132">Agora que você instalou a CLI do Azure, faça um tour breve de seus recursos e comandos comuns.</span><span class="sxs-lookup"><span data-stu-id="299c9-132">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="299c9-133">Introdução à CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="299c9-133">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
