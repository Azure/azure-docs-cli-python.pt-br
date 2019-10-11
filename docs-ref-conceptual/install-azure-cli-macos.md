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
ms.openlocfilehash: 790c63a60a5d23863b48227dcc99462bbf950d80
ms.sourcegitcommit: b42ce26476b135bb2047c8d9d787580c858f8b6b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2019
ms.locfileid: "72163844"
---
# <a name="install-azure-cli-on-macos"></a><span data-ttu-id="02db4-103">Instalar a CLI do Azure no macOS</span><span class="sxs-lookup"><span data-stu-id="02db4-103">Install Azure CLI on macOS</span></span>

<span data-ttu-id="02db4-104">Para a plataforma macOS, você pode instalar a CLI do Azure com o [gerenciador de pacotes homebrew](https://brew.sh).</span><span class="sxs-lookup"><span data-stu-id="02db4-104">For the macOS platform, you can install the Azure CLI with [homebrew package manager](https://brew.sh).</span></span> <span data-ttu-id="02db4-105">O Homebrew torna mais fácil manter a instalação da CLI atualizada.</span><span class="sxs-lookup"><span data-stu-id="02db4-105">Homebrew makes it easy to keep your installation of the CLI update to date.</span></span> <span data-ttu-id="02db4-106">O pacote da CLI foi testado em versões do macOS 10.9 e posteriores.</span><span class="sxs-lookup"><span data-stu-id="02db4-106">The CLI package has been tested on macOS versions 10.9 and later.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

## <a name="install-with-homebrew"></a><span data-ttu-id="02db4-107">Instalar com o Homebrew</span><span class="sxs-lookup"><span data-stu-id="02db4-107">Install with Homebrew</span></span>

<span data-ttu-id="02db4-108">O homebrew é a maneira mais fácil de gerenciar a instalação da CLI.</span><span class="sxs-lookup"><span data-stu-id="02db4-108">Homebrew is the easiest way to manage your CLI install.</span></span> <span data-ttu-id="02db4-109">Ele fornece maneiras convenientes de instalar, atualizar e desinstalar.</span><span class="sxs-lookup"><span data-stu-id="02db4-109">It provides convenient ways to install, update, and uninstall.</span></span>
<span data-ttu-id="02db4-110">Se você não tiver o homebrew disponível em seu sistema, [instale-o](https://docs.brew.sh/Installation.html) antes de continuar.</span><span class="sxs-lookup"><span data-stu-id="02db4-110">If you don't have homebrew available on your system, [install homebrew](https://docs.brew.sh/Installation.html) before continuing.</span></span>

<span data-ttu-id="02db4-111">Você pode instalar a CLI atualizando suas informações de repositório brew e executando o comando `install`:</span><span class="sxs-lookup"><span data-stu-id="02db4-111">You can install the CLI by updating your brew repository information, and then running the `install` command:</span></span>

```bash
brew update && brew install azure-cli
```

> [!IMPORTANT]
>
> <span data-ttu-id="02db4-112">A CLI do Azure tem uma dependência no pacote `python3` do Homebrew, e a instalará.</span><span class="sxs-lookup"><span data-stu-id="02db4-112">The Azure CLI has a dependency on the Homebrew `python3` package, and will install it.</span></span>
> <span data-ttu-id="02db4-113">A CLI do Azure é certamente compatível com a versão mais recente do `python3` publicada no Homebrew.</span><span class="sxs-lookup"><span data-stu-id="02db4-113">The Azure CLI is guaranteed to be compatible with the latest version of `python3` published on Homebrew.</span></span>

<span data-ttu-id="02db4-114">É possível executar a CLI do Azure com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="02db4-114">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="02db4-115">Para entrar, use o comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="02db4-115">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="02db4-116">Para saber mais sobre os diferentes métodos de autenticação, confira [Entrar com a CLI do Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="02db4-116">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="02db4-117">solução de problemas</span><span class="sxs-lookup"><span data-stu-id="02db4-117">Troubleshooting</span></span>

<span data-ttu-id="02db4-118">Se você encontrar um problema ao instalar a CLI através do Homebrew, aqui estão alguns erros comuns.</span><span class="sxs-lookup"><span data-stu-id="02db4-118">If you encounter a problem when installing the CLI through Homebrew, here are some common errors.</span></span> <span data-ttu-id="02db4-119">Se você tiver um problema não abordado aqui, [arquive um problema no github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="02db4-119">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="unable-to-find-python-or-installed-packages"></a><span data-ttu-id="02db4-120">Não é possível localizar o Python ou os pacotes instalados</span><span class="sxs-lookup"><span data-stu-id="02db4-120">Unable to find Python or installed packages</span></span>

<span data-ttu-id="02db4-121">Pode haver uma pequena incompatibilidade de versão ou outro problema durante a instalação do homebrew.</span><span class="sxs-lookup"><span data-stu-id="02db4-121">There may be a minor version mismatch or other issue during homebrew installation.</span></span> <span data-ttu-id="02db4-122">A CLI não usa um ambiente virtual Python, portanto, ela se baseia em localizar a versão instalada do Python.</span><span class="sxs-lookup"><span data-stu-id="02db4-122">The CLI doesn't use a Python virtual environment, so it relies on finding the installed Python version.</span></span> <span data-ttu-id="02db4-123">Uma possível correção é instalar e revincular a dependência `python3` do Homebrew.</span><span class="sxs-lookup"><span data-stu-id="02db4-123">A possible fix is to install and relink the `python3` dependency from Homebrew.</span></span>

```bash
brew update && brew install python3 && brew upgrade python3
brew link --overwrite python3
```

### <a name="cli-version-1x-is-installed"></a><span data-ttu-id="02db4-124">A versão 1.x da CLI está instalada</span><span class="sxs-lookup"><span data-stu-id="02db4-124">CLI version 1.x is installed</span></span>

<span data-ttu-id="02db4-125">Se tiver sido instalada uma versão desatualizada, pode ser devido a um cache de homebrew obsoleto.</span><span class="sxs-lookup"><span data-stu-id="02db4-125">If an out-of-date version was installed, it could be because of a stale homebrew cache.</span></span> <span data-ttu-id="02db4-126">Siga as instruções de [atualização](#update).</span><span class="sxs-lookup"><span data-stu-id="02db4-126">Follow the [update](#update) instructions.</span></span>

### <a name="proxy-blocks-connection"></a><span data-ttu-id="02db4-127">Conexão de blocos de proxy</span><span class="sxs-lookup"><span data-stu-id="02db4-127">Proxy blocks connection</span></span>

<span data-ttu-id="02db4-128">Talvez você não consiga obter recursos do Homebrew, a menos que o tenha configurado corretamente para usar seu proxy.</span><span class="sxs-lookup"><span data-stu-id="02db4-128">You may be unable to get resources from Homebrew unless you have correctly configured it to use your proxy.</span></span> <span data-ttu-id="02db4-129">Siga as [instruções de configuração de proxy do Homebrew](https://docs.brew.sh/Manpage#using-homebrew-behind-a-proxy).</span><span class="sxs-lookup"><span data-stu-id="02db4-129">Follow the [Homebrew proxy configuration instructions](https://docs.brew.sh/Manpage#using-homebrew-behind-a-proxy).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="02db4-130">Se você estiver atrás de um proxy, as variáveis `HTTP_PROXY` e `HTTPS_PROXY` precisarão ser definidas para se conectarem aos serviços do Azure com a CLI.</span><span class="sxs-lookup"><span data-stu-id="02db4-130">If you are behind a proxy, `HTTP_PROXY` and `HTTPS_PROXY` must be set to connect to Azure services with the CLI.</span></span>
> <span data-ttu-id="02db4-131">Se você não estiver usando a autenticação básica, é recomendável exportar as variáveis no arquivo `.bashrc`.</span><span class="sxs-lookup"><span data-stu-id="02db4-131">If you are not using basic auth, it's recommended to export these variables in your `.bashrc` file.</span></span>
> <span data-ttu-id="02db4-132">Sempre siga as políticas de segurança da sua empresa e os requisitos do administrador do sistema.</span><span class="sxs-lookup"><span data-stu-id="02db4-132">Always follow your business' security policies and the requirements of your system administrator.</span></span>

<span data-ttu-id="02db4-133">Para obter os recursos de Bottle do Homebrew, o proxy precisa permitir conexões HTTPS com os seguintes endereços:</span><span class="sxs-lookup"><span data-stu-id="02db4-133">In order to get the bottle resources from Homebrew, your proxy needs to allow HTTPS connections to the following addresses:</span></span>

* `https://formulae.brew.sh`
* `https://homebrew.bintray.com`

## <a name="update"></a><span data-ttu-id="02db4-134">Atualizar</span><span class="sxs-lookup"><span data-stu-id="02db4-134">Update</span></span>

<span data-ttu-id="02db4-135">A CLI é atualizada regularmente com correções de bugs, aprimoramentos, novos recursos e funcionalidade de visualização.</span><span class="sxs-lookup"><span data-stu-id="02db4-135">The CLI is regularly updated with bug fixes, improvements, new features, and preview functionality.</span></span> <span data-ttu-id="02db4-136">Uma nova versão fica disponível aproximadamente a cada duas semanas.</span><span class="sxs-lookup"><span data-stu-id="02db4-136">A new release is available roughly every two weeks.</span></span> <span data-ttu-id="02db4-137">Atualize as informações do repositório local e atualize o pacote `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="02db4-137">Update your local repository information and then upgrade the `azure-cli` package.</span></span>

```bash
brew update && brew upgrade azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="02db4-138">Desinstalar</span><span class="sxs-lookup"><span data-stu-id="02db4-138">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="02db4-139">Use o homebrew para desinstalar o pacote `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="02db4-139">Use homebrew to uninstall the `azure-cli` package.</span></span>

```bash
brew uninstall azure-cli
```

## <a name="other-installation-methods"></a><span data-ttu-id="02db4-140">Outros métodos de instalação</span><span class="sxs-lookup"><span data-stu-id="02db4-140">Other installation methods</span></span>

<span data-ttu-id="02db4-141">Se você não pode usar o Homebrew para instalar a CLI do Azure em seu ambiente, é possível usar as instruções manuais para o Linux.</span><span class="sxs-lookup"><span data-stu-id="02db4-141">If you can't use homebrew to install the Azure CLI in your environment, it's possible to use the manual instructions for Linux.</span></span> <span data-ttu-id="02db4-142">Observe que esse processo não é oficialmente mantido para ser compatível com o macOS.</span><span class="sxs-lookup"><span data-stu-id="02db4-142">Note that this process is not officially maintained to be compatible with macOS.</span></span> <span data-ttu-id="02db4-143">É sempre recomendável usar um gerenciador de pacotes, como o Homebrew.</span><span class="sxs-lookup"><span data-stu-id="02db4-143">Using a package manager such as Homebrew is always recommended.</span></span> <span data-ttu-id="02db4-144">Somente use o método de instalação manual se não tiver nenhuma outra opção disponível.</span><span class="sxs-lookup"><span data-stu-id="02db4-144">Only use the manual installation method if you have no other option available.</span></span>

<span data-ttu-id="02db4-145">Para as instruções de instalação manual, confira [Instalar manualmente a CLI do Azure no Linux](install-azure-cli-linux.md).</span><span class="sxs-lookup"><span data-stu-id="02db4-145">For the manual installation instructions, see [Install Azure CLI on Linux manually](install-azure-cli-linux.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="02db4-146">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="02db4-146">Next Steps</span></span>

<span data-ttu-id="02db4-147">Agora que você instalou a CLI do Azure, faça um tour breve de seus recursos e comandos comuns.</span><span class="sxs-lookup"><span data-stu-id="02db4-147">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="02db4-148">Introdução à CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="02db4-148">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
