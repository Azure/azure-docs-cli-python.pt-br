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
ms.devlang: azurecli
ms.openlocfilehash: 229b109b307453c87abf260a66084c94ced33d81
ms.sourcegitcommit: 1987a39809f9865034b27130e56f30b2bd1eb72c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/19/2019
ms.locfileid: "56421993"
---
# <a name="install-azure-cli-on-linux-manually"></a><span data-ttu-id="29312-103">Instalar CLI do Azure no Linux manualmente</span><span class="sxs-lookup"><span data-stu-id="29312-103">Install Azure CLI on Linux manually</span></span>

<span data-ttu-id="29312-104">Se não houver nenhum pacote da CLI do Azure para a sua distribuição, instale a CLI manualmente executando um script.</span><span class="sxs-lookup"><span data-stu-id="29312-104">If there's no package for the Azure CLI for you your distribution, install the CLI manually by running a script.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

> [!NOTE]
> <span data-ttu-id="29312-105">É altamente recomendável instalar a CLI com um gerenciador de pacotes.</span><span class="sxs-lookup"><span data-stu-id="29312-105">It's strongly recommend to install the CLI with a package manager.</span></span> <span data-ttu-id="29312-106">Um gerenciador de pacotes garante que você sempre obtenha as atualizações mais recentes, além da estabilidade dos componentes da CLI.</span><span class="sxs-lookup"><span data-stu-id="29312-106">A package manager makes sure you always get the latest updates, and guarantees the stability of CLI components.</span></span> <span data-ttu-id="29312-107">Verifique e veja se há um pacote de distribuição antes de instalar manualmente.</span><span class="sxs-lookup"><span data-stu-id="29312-107">Check and see if there is a package for your distribution before installing manually.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="29312-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="29312-108">Prerequisites</span></span>

<span data-ttu-id="29312-109">A CLI requer o seguinte software:</span><span class="sxs-lookup"><span data-stu-id="29312-109">The CLI requires the following software:</span></span>

* <span data-ttu-id="29312-110">[Python 3.6.x ou 3.7.x](https://www.python.org/downloads/).</span><span class="sxs-lookup"><span data-stu-id="29312-110">[Python 3.6.x or 3.7.x](https://www.python.org/downloads/).</span></span> 
* [<span data-ttu-id="29312-111">libffi</span><span class="sxs-lookup"><span data-stu-id="29312-111">libffi</span></span>](https://sourceware.org/libffi/)
* [<span data-ttu-id="29312-112">OpenSSL 1.0.2</span><span class="sxs-lookup"><span data-stu-id="29312-112">OpenSSL 1.0.2</span></span>](https://www.openssl.org/source/)

> [!IMPORTANT]
>
> <span data-ttu-id="29312-113">A CLI também é compatível com o Python 2.7.x, que será retirado do mercado em 1º de janeiro de 2020.</span><span class="sxs-lookup"><span data-stu-id="29312-113">The CLI is also compatible with Python 2.7.x, which is being end-of-lifed on January 1, 2020.</span></span> <span data-ttu-id="29312-114">Por esse motivo, é recomendável que você instale o Python 3 para executar a CLI.</span><span class="sxs-lookup"><span data-stu-id="29312-114">For this reason we recommend that you install Python 3 to run the CLI.</span></span>

## <a name="install-or-update"></a><span data-ttu-id="29312-115">Instalar ou atualizar</span><span class="sxs-lookup"><span data-stu-id="29312-115">Install or update</span></span>

<span data-ttu-id="29312-116">Instalar e atualizar a CLI exige executar novamente o script de instalação.</span><span class="sxs-lookup"><span data-stu-id="29312-116">Both installing and updating the CLI requires re-running the install script.</span></span> <span data-ttu-id="29312-117">Instale a CLI executando `curl`.</span><span class="sxs-lookup"><span data-stu-id="29312-117">Install the CLI by running `curl`.</span></span>

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

<span data-ttu-id="29312-118">O script também pode ser baixado e executado localmente.</span><span class="sxs-lookup"><span data-stu-id="29312-118">The script can also be downloaded and run locally.</span></span> <span data-ttu-id="29312-119">Talvez você precise reiniciar o shell para que as alterações entrem em vigor.</span><span class="sxs-lookup"><span data-stu-id="29312-119">You may have to restart your shell in order for changes to take effect.</span></span>

<span data-ttu-id="29312-120">É possível executar a CLI do Azure com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="29312-120">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="29312-121">Para entrar, use o comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="29312-121">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="29312-122">Para saber mais sobre os diferentes métodos de autenticação, confira [Entrar com a CLI do Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="29312-122">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="29312-123">solução de problemas</span><span class="sxs-lookup"><span data-stu-id="29312-123">Troubleshooting</span></span>

<span data-ttu-id="29312-124">Aqui estão alguns problemas comuns observados durante uma instalação manual.</span><span class="sxs-lookup"><span data-stu-id="29312-124">Here are some common problems seen during a manual installation.</span></span> <span data-ttu-id="29312-125">Se você tiver um problema não abordado aqui, [arquive um problema no GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="29312-125">If you experience a problem not covered here, [file an issue on GitHub](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="curl-object-moved-error"></a><span data-ttu-id="29312-126">Erro "Objeto movido" de cURL</span><span class="sxs-lookup"><span data-stu-id="29312-126">curl "Object Moved" error</span></span>

<span data-ttu-id="29312-127">Se você receber um erro de `curl` relacionado ao parâmetro `-L` ou uma mensagem de erro incluindo o texto "Objeto movido", tente usar a URL completa em vez da `aka.ms` de redirecionamento:</span><span class="sxs-lookup"><span data-stu-id="29312-127">If you get an error from `curl` related to the `-L` parameter, or an error message including the text "Object Moved", try using the full URL instead of the `aka.ms` redirect:</span></span>

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a><span data-ttu-id="29312-128">`az` comando não encontrado</span><span class="sxs-lookup"><span data-stu-id="29312-128">`az` command not found</span></span>

<span data-ttu-id="29312-129">Se não conseguir executar o comando após a instalação e usar `bash` ou `zsh`, limpe o cache do hash de comando do shell.</span><span class="sxs-lookup"><span data-stu-id="29312-129">If you can't run the command after installation and using `bash` or `zsh`, clear your shell's command hash cache.</span></span> <span data-ttu-id="29312-130">Executar</span><span class="sxs-lookup"><span data-stu-id="29312-130">Run</span></span>

```bash
hash -r
```

<span data-ttu-id="29312-131">e verificar se o problema foi resolvido.</span><span class="sxs-lookup"><span data-stu-id="29312-131">and check if the problem is resolved.</span></span>

<span data-ttu-id="29312-132">O problema também pode ocorrer se você não reiniciou o shell após a instalação.</span><span class="sxs-lookup"><span data-stu-id="29312-132">The issue can also occur if you didn't restart your shell after installation.</span></span> <span data-ttu-id="29312-133">Verifique se o local do comando `az` está no `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="29312-133">Make sure that the location of the `az` command is in your `$PATH`.</span></span> <span data-ttu-id="29312-134">A localização do comando `az` é</span><span class="sxs-lookup"><span data-stu-id="29312-134">The location of the `az` command is</span></span>

```bash
<install path>/bin
```

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="uninstall"></a><span data-ttu-id="29312-135">Desinstalar</span><span class="sxs-lookup"><span data-stu-id="29312-135">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="29312-136">Desinstale a CLI excluindo diretamente os arquivos do local escolhido no momento da instalação.</span><span class="sxs-lookup"><span data-stu-id="29312-136">Uninstall the CLI by directly deleting the files from the location chosen at the time of installation.</span></span> <span data-ttu-id="29312-137">O local de instalação padrão é `$HOME`.</span><span class="sxs-lookup"><span data-stu-id="29312-137">The default install location is `$HOME`.</span></span>

1. <span data-ttu-id="29312-138">Remova os arquivos da CLI instalados.</span><span class="sxs-lookup"><span data-stu-id="29312-138">Remove the installed CLI files.</span></span>

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. <span data-ttu-id="29312-139">Modifique o arquivo `$HOME/.bash_profile` para remover a seguinte linha:</span><span class="sxs-lookup"><span data-stu-id="29312-139">Modify your `$HOME/.bash_profile` file to remove the following line:</span></span>

   ```text
   <install location>/lib/azure-cli/az.completion
   ```

3. <span data-ttu-id="29312-140">Se usar `bash` ou `zsh`, recarregue o cache de comando do shell.</span><span class="sxs-lookup"><span data-stu-id="29312-140">If using `bash` or `zsh`, reload your shell's command cache.</span></span>

   ```bash
   hash -r
   ```

## <a name="next-steps"></a><span data-ttu-id="29312-141">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="29312-141">Next Steps</span></span>

<span data-ttu-id="29312-142">Agora que você instalou a CLI do Azure, faça um tour breve de seus recursos e comandos comuns.</span><span class="sxs-lookup"><span data-stu-id="29312-142">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="29312-143">Introdução à CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="29312-143">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
