---
title: Instalar a CLI do Azure para Linux manualmente
description: Como instalar a CLI do Azure no Linux manualmente
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 221e8904fdb938b15b28cb369085dcacb08e4091
ms.sourcegitcommit: c4462456dfb17993f098d47c37bc19f4d78b8179
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/25/2018
ms.locfileid: "47177939"
---
# <a name="install-azure-cli-on-linux-manually"></a><span data-ttu-id="bc1a1-103">Instalar CLI do Azure no Linux manualmente</span><span class="sxs-lookup"><span data-stu-id="bc1a1-103">Install Azure CLI on Linux manually</span></span>

<span data-ttu-id="bc1a1-104">Se não houver nenhum pacote da CLI do Azure para a sua distribuição, instale a CLI manualmente executando um script.</span><span class="sxs-lookup"><span data-stu-id="bc1a1-104">If there's no package for the Azure CLI for you your distribution, install the CLI manually by running a script.</span></span>

> [!NOTE]
> <span data-ttu-id="bc1a1-105">É altamente recomendável instalar a CLI com um gerenciador de pacotes.</span><span class="sxs-lookup"><span data-stu-id="bc1a1-105">It's strongly recommend to install the CLI with a package manager.</span></span> <span data-ttu-id="bc1a1-106">Um gerenciador de pacotes garante que você sempre obtenha as atualizações mais recentes, além da estabilidade dos componentes da CLI.</span><span class="sxs-lookup"><span data-stu-id="bc1a1-106">A package manager makes sure you always get the latest updates, and guarantees the stability of CLI components.</span></span> <span data-ttu-id="bc1a1-107">Verifique e veja se há um pacote de distribuição antes de instalar manualmente.</span><span class="sxs-lookup"><span data-stu-id="bc1a1-107">Check and see if there is a package for your distribution before installing manually.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bc1a1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bc1a1-108">Prerequisites</span></span>

<span data-ttu-id="bc1a1-109">A CLI requer o seguinte software:</span><span class="sxs-lookup"><span data-stu-id="bc1a1-109">The CLI requires the following software:</span></span>

* [<span data-ttu-id="bc1a1-110">Python 2.7 ou Python 3. x</span><span class="sxs-lookup"><span data-stu-id="bc1a1-110">Python 2.7 or Python 3.x</span></span>](https://www.python.org/downloads/)
* [<span data-ttu-id="bc1a1-111">libffi</span><span class="sxs-lookup"><span data-stu-id="bc1a1-111">libffi</span></span>](https://sourceware.org/libffi/)
* [<span data-ttu-id="bc1a1-112">OpenSSL 1.0.2</span><span class="sxs-lookup"><span data-stu-id="bc1a1-112">OpenSSL 1.0.2</span></span>](https://www.openssl.org/source/)

## <a name="install-or-update"></a><span data-ttu-id="bc1a1-113">Instalar ou atualizar</span><span class="sxs-lookup"><span data-stu-id="bc1a1-113">Install or update</span></span>

<span data-ttu-id="bc1a1-114">Instalar e atualizar a CLI exige executar novamente o script de instalação.</span><span class="sxs-lookup"><span data-stu-id="bc1a1-114">Both installing and updating the CLI requires re-running the install script.</span></span> <span data-ttu-id="bc1a1-115">Instale a CLI executando `curl`.</span><span class="sxs-lookup"><span data-stu-id="bc1a1-115">Install the CLI by running `curl`.</span></span>

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

<span data-ttu-id="bc1a1-116">O script também pode ser baixado e executado localmente.</span><span class="sxs-lookup"><span data-stu-id="bc1a1-116">The script can also be downloaded and run locally.</span></span> <span data-ttu-id="bc1a1-117">Talvez você precise reiniciar o shell para que as alterações entrem em vigor.</span><span class="sxs-lookup"><span data-stu-id="bc1a1-117">You may have to restart your shell in order for changes to take effect.</span></span>

<span data-ttu-id="bc1a1-118">É possível executar a CLI do Azure com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="bc1a1-118">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="bc1a1-119">Para entrar, use o comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="bc1a1-119">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="bc1a1-120">Para saber mais sobre os diferentes métodos de autenticação, confira [Entrar com a CLI do Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="bc1a1-120">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="bc1a1-121">solução de problemas</span><span class="sxs-lookup"><span data-stu-id="bc1a1-121">Troubleshooting</span></span>

<span data-ttu-id="bc1a1-122">Aqui estão alguns problemas comuns observados durante uma instalação manual.</span><span class="sxs-lookup"><span data-stu-id="bc1a1-122">Here are some common problems seen during a manual installation.</span></span> <span data-ttu-id="bc1a1-123">Se você tiver um problema não abordado aqui, [arquive um problema no github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="bc1a1-123">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="curl-object-moved-error"></a><span data-ttu-id="bc1a1-124">Erro "Objeto movido" de cURL</span><span class="sxs-lookup"><span data-stu-id="bc1a1-124">curl "Object Moved" error</span></span>

<span data-ttu-id="bc1a1-125">Se você receber um erro de `curl` relacionado ao parâmetro `-L` ou uma mensagem de erro incluindo o texto "Objeto movido", tente usar a URL completa em vez da `aka.ms` de redirecionamento:</span><span class="sxs-lookup"><span data-stu-id="bc1a1-125">If you get an error from `curl` related to the `-L` parameter, or an error message including the text "Object Moved", try using the full URL instead of the `aka.ms` redirect:</span></span>

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a><span data-ttu-id="bc1a1-126">`az` comando não encontrado</span><span class="sxs-lookup"><span data-stu-id="bc1a1-126">`az` command not found</span></span>

<span data-ttu-id="bc1a1-127">Se não conseguir executar o comando após a instalação e usar `bash` ou `zsh`, limpe o cache do hash de comando do shell.</span><span class="sxs-lookup"><span data-stu-id="bc1a1-127">If you can't run the command after installation and using `bash` or `zsh`, clear your shell's command hash cache.</span></span> <span data-ttu-id="bc1a1-128">Executar</span><span class="sxs-lookup"><span data-stu-id="bc1a1-128">Run</span></span>

```bash
hash -r
```

<span data-ttu-id="bc1a1-129">e verificar se o problema foi resolvido.</span><span class="sxs-lookup"><span data-stu-id="bc1a1-129">and check if the problem is resolved.</span></span>

<span data-ttu-id="bc1a1-130">O problema também pode ocorrer se você não reiniciou o shell após a instalação.</span><span class="sxs-lookup"><span data-stu-id="bc1a1-130">The issue can also occur if you didn't restart your shell after installation.</span></span> <span data-ttu-id="bc1a1-131">Verifique se o local do comando `az` está no `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="bc1a1-131">Make sure that the location of the `az` command is in your `$PATH`.</span></span> <span data-ttu-id="bc1a1-132">A localização do comando `az` é</span><span class="sxs-lookup"><span data-stu-id="bc1a1-132">The location of the `az` command is</span></span>

```bash
<install path>/bin
```

## <a name="uninstall"></a><span data-ttu-id="bc1a1-133">Desinstalar</span><span class="sxs-lookup"><span data-stu-id="bc1a1-133">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="bc1a1-134">Desinstale a CLI excluindo diretamente os arquivos do local escolhido no momento da instalação.</span><span class="sxs-lookup"><span data-stu-id="bc1a1-134">Uninstall the CLI by directly deleting the files from the location chosen at the time of installation.</span></span> <span data-ttu-id="bc1a1-135">O local de instalação padrão é `$HOME`.</span><span class="sxs-lookup"><span data-stu-id="bc1a1-135">The default install location is `$HOME`.</span></span>

1. <span data-ttu-id="bc1a1-136">Remova os arquivos da CLI instalados.</span><span class="sxs-lookup"><span data-stu-id="bc1a1-136">Remove the installed CLI files.</span></span>

  ```bash
  rm -r <install location>/lib/azure-cli
  rm <install location>/bin/az
  ```

2. <span data-ttu-id="bc1a1-137">Modifique o arquivo `$HOME/.bash_profile` para remover a seguinte linha:</span><span class="sxs-lookup"><span data-stu-id="bc1a1-137">Modify your `$HOME/.bash_profile` file to remove the following line:</span></span>

  ```text
  <install location>/lib/azure-cli/az.completion
  ```

3. <span data-ttu-id="bc1a1-138">Se usar `bash` ou `zsh`, recarregue o cache de comando do shell.</span><span class="sxs-lookup"><span data-stu-id="bc1a1-138">If using `bash` or `zsh`, reload your shell's command cache.</span></span>

  ```bash
  hash -r
  ```

## <a name="next-steps"></a><span data-ttu-id="bc1a1-139">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="bc1a1-139">Next Steps</span></span>

<span data-ttu-id="bc1a1-140">Agora que você instalou a CLI do Azure, faça um tour breve de seus recursos e comandos comuns.</span><span class="sxs-lookup"><span data-stu-id="bc1a1-140">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="bc1a1-141">Introdução à CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="bc1a1-141">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
