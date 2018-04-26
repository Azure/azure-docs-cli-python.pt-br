---
title: Instalar a CLI do Azure para macOS
description: Como instalar a CLI do Azure 2.0 no macOS
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 295e84d2d30365aac4334e1e962f23c7b8e38d37
ms.sourcegitcommit: 0e9aafa07311526f43661c8bd3a7eba7cbc2caed
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/20/2018
---
# <a name="install-azure-cli-20-on-macos"></a><span data-ttu-id="d75e3-103">Instalar CLI do Azure 2.0 no macOS</span><span class="sxs-lookup"><span data-stu-id="d75e3-103">Install Azure CLI 2.0 on macOS</span></span>

<span data-ttu-id="d75e3-104">Para a plataforma macOS, você pode instalar a CLI do Azure com o [gerenciador de pacotes homebrew](http://brew.sh).</span><span class="sxs-lookup"><span data-stu-id="d75e3-104">For the macOS platform, you can install the Azure CLI with [homebrew package manager](http://brew.sh).</span></span> <span data-ttu-id="d75e3-105">O Homebrew torna mais fácil manter a instalação da CLI atualizada.</span><span class="sxs-lookup"><span data-stu-id="d75e3-105">Homebrew makes it easy to keep your installation of the CLI update to date.</span></span> <span data-ttu-id="d75e3-106">O pacote da CLI foi testado em versões do macOS 10.9 e posteriores.</span><span class="sxs-lookup"><span data-stu-id="d75e3-106">The CLI package has been tested on macOS versions 10.9 and later.</span></span>

## <a name="install"></a><span data-ttu-id="d75e3-107">Instalar</span><span class="sxs-lookup"><span data-stu-id="d75e3-107">Install</span></span>

<span data-ttu-id="d75e3-108">O homebrew é a maneira mais fácil de gerenciar a instalação da CLI.</span><span class="sxs-lookup"><span data-stu-id="d75e3-108">Homebrew is the easiest way to manage your CLI install.</span></span> <span data-ttu-id="d75e3-109">Ele fornece maneiras convenientes de instalar, atualizar e desinstalar.</span><span class="sxs-lookup"><span data-stu-id="d75e3-109">It provides convenient ways to install, update, and uninstall.</span></span>
<span data-ttu-id="d75e3-110">Se você não tiver o homebrew disponível em seu sistema, [instale-o](https://docs.brew.sh/Installation.html) antes de continuar.</span><span class="sxs-lookup"><span data-stu-id="d75e3-110">If you don't have homebrew available on your system, [install homebrew](https://docs.brew.sh/Installation.html) before continuing.</span></span>

<span data-ttu-id="d75e3-111">Você pode instalar a CLI atualizando suas informações de repositório brew e executando o comando `install`:</span><span class="sxs-lookup"><span data-stu-id="d75e3-111">You can install the CLI by updating your brew repository information, and then running the `install` command:</span></span>

```bash
brew update && brew install azure-cli
```

<span data-ttu-id="d75e3-112">É possível executar a CLI do Azure com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="d75e3-112">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="d75e3-113">Para fazer logon, execute o comando `az login`.</span><span class="sxs-lookup"><span data-stu-id="d75e3-113">To log in, run the `az login` command.</span></span>

```azurecli
az login
```

<span data-ttu-id="d75e3-114">Para saber mais sobre os métodos de logon diferente, consulte [Fazer logon com a CLI do Azure 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="d75e3-114">To learn more about different login methods, see [Log in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="d75e3-115">solução de problemas</span><span class="sxs-lookup"><span data-stu-id="d75e3-115">Troubleshooting</span></span>

<span data-ttu-id="d75e3-116">Se você encontrar um problema ao instalar a CLI através do Homebrew, aqui estão alguns erros comuns.</span><span class="sxs-lookup"><span data-stu-id="d75e3-116">If you encounter a problem when installing the CLI through Homebrew, here are some common errors.</span></span> <span data-ttu-id="d75e3-117">Se o problema não estiver listado aqui, [registre um problema no github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="d75e3-117">If your issue is not listed here, please [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="unable-to-find-python-or-installed-packages"></a><span data-ttu-id="d75e3-118">Não é possível localizar o Python ou os pacotes instalados</span><span class="sxs-lookup"><span data-stu-id="d75e3-118">Unable to find Python or installed packages</span></span>

<span data-ttu-id="d75e3-119">Se a instalação não conseguir localizar o Python nem os pacotes instalados, poderá haver uma incompatibilidade de versão secundária ou outro problema que ocorreu durante a instalação do homebrew.</span><span class="sxs-lookup"><span data-stu-id="d75e3-119">If your install is unable to find Python or installed packages, there may be a minor version mismatch or other issue that occurred during homebrew installation.</span></span> <span data-ttu-id="d75e3-120">Como a CLI não usa um ambiente virtual Python, ela depende de conseguir localizar as versões corretas do Python.</span><span class="sxs-lookup"><span data-stu-id="d75e3-120">Since the CLI does not use a Python virtual environment, it relies on being able to find correct Python version.</span></span> <span data-ttu-id="d75e3-121">Você pode corrigir esses problemas vinculando novamente a instalação do Python.</span><span class="sxs-lookup"><span data-stu-id="d75e3-121">You may be able to fix these issues by relinking your Python installation.</span></span>

```bash
brew link --overwrite python3
```

### <a name="cli-version-1x-is-installed"></a><span data-ttu-id="d75e3-122">A versão 1.x da CLI está instalada</span><span class="sxs-lookup"><span data-stu-id="d75e3-122">CLI version 1.x is installed</span></span>

<span data-ttu-id="d75e3-123">Se tiver sido instalada uma versão desatualizada, pode ser devido a um cache de homebrew obsoleto.</span><span class="sxs-lookup"><span data-stu-id="d75e3-123">If an out-of-date version was installed, it could be due to a stale homebrew cache.</span></span> <span data-ttu-id="d75e3-124">Siga as instruções de [atualização](#Update).</span><span class="sxs-lookup"><span data-stu-id="d75e3-124">Follow the [update](#Update) instructions.</span></span>

## <a name="update"></a><span data-ttu-id="d75e3-125">Atualizar</span><span class="sxs-lookup"><span data-stu-id="d75e3-125">Update</span></span>

<span data-ttu-id="d75e3-126">A CLI é atualizada regularmente com correções de bugs, aprimoramentos, novos recursos e funcionalidade de visualização.</span><span class="sxs-lookup"><span data-stu-id="d75e3-126">The CLI is regularly updated with bug fixes, improvements, new features, and preview functionality.</span></span> <span data-ttu-id="d75e3-127">Uma nova versão fica disponível aproximadamente a cada duas semanas.</span><span class="sxs-lookup"><span data-stu-id="d75e3-127">A new release is available roughly every two weeks.</span></span> <span data-ttu-id="d75e3-128">Atualize as informações do repositório local e atualize o pacote `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="d75e3-128">Update your local repository information and then upgrade the `azure-cli` package.</span></span>

```bash
brew update && brew upgrade azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="d75e3-129">Desinstalar</span><span class="sxs-lookup"><span data-stu-id="d75e3-129">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="d75e3-130">Use o homebrew para desinstalar o pacote `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="d75e3-130">Use homebrew to uninstall the `azure-cli` package.</span></span>

```bash
brew uninstall azure-cli
```
