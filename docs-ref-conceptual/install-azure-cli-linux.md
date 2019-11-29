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
ms.openlocfilehash: caca30ec186f302e47f2978b9bfe616d4b2a5c02
ms.sourcegitcommit: 443e14098d6643cdb2e178847d1c79b1b95146ce
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/26/2019
ms.locfileid: "74543633"
---
# <a name="install-azure-cli-on-linux-manually"></a><span data-ttu-id="019b3-103">Instalar CLI do Azure no Linux manualmente</span><span class="sxs-lookup"><span data-stu-id="019b3-103">Install Azure CLI on Linux manually</span></span>

<span data-ttu-id="019b3-104">Se não houver nenhum pacote da CLI do Azure para a sua distribuição, instale a CLI manualmente executando um script.</span><span class="sxs-lookup"><span data-stu-id="019b3-104">If there's no package for the Azure CLI for you your distribution, install the CLI manually by running a script.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

> [!NOTE]
> <span data-ttu-id="019b3-105">É altamente recomendável instalar a CLI com um gerenciador de pacotes.</span><span class="sxs-lookup"><span data-stu-id="019b3-105">It's strongly recommend to install the CLI with a package manager.</span></span> <span data-ttu-id="019b3-106">Um gerenciador de pacotes garante que você sempre obtenha as atualizações mais recentes, além da estabilidade dos componentes da CLI.</span><span class="sxs-lookup"><span data-stu-id="019b3-106">A package manager makes sure you always get the latest updates, and guarantees the stability of CLI components.</span></span> <span data-ttu-id="019b3-107">Verifique e veja se há um pacote de distribuição antes de instalar manualmente.</span><span class="sxs-lookup"><span data-stu-id="019b3-107">Check and see if there is a package for your distribution before installing manually.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="019b3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="019b3-108">Prerequisites</span></span>

<span data-ttu-id="019b3-109">A CLI requer o seguinte software:</span><span class="sxs-lookup"><span data-stu-id="019b3-109">The CLI requires the following software:</span></span>

* <span data-ttu-id="019b3-110">[Python 3.6.x ou 3.7.x](https://www.python.org/downloads/).</span><span class="sxs-lookup"><span data-stu-id="019b3-110">[Python 3.6.x or 3.7.x](https://www.python.org/downloads/).</span></span> 
* [<span data-ttu-id="019b3-111">libffi</span><span class="sxs-lookup"><span data-stu-id="019b3-111">libffi</span></span>](https://sourceware.org/libffi/)
* [<span data-ttu-id="019b3-112">OpenSSL 1.0.2</span><span class="sxs-lookup"><span data-stu-id="019b3-112">OpenSSL 1.0.2</span></span>](https://www.openssl.org/source/)

> [!IMPORTANT]
>
> <span data-ttu-id="019b3-113">A CLI também é compatível com o Python 2.7.x, que será retirado do mercado em 1º de janeiro de 2020.</span><span class="sxs-lookup"><span data-stu-id="019b3-113">The CLI is also compatible with Python 2.7.x, which is being end-of-lifed on January 1, 2020.</span></span> <span data-ttu-id="019b3-114">Uma versão futura da CLI do Azure removerá o suporte para Python 2.7.</span><span class="sxs-lookup"><span data-stu-id="019b3-114">A future version of Azure CLI will drop support for Python 2.7.</span></span> <span data-ttu-id="019b3-115">Por esse motivo, é recomendável que você instale o Python 3 para executar a CLI.</span><span class="sxs-lookup"><span data-stu-id="019b3-115">For this reason we recommend that you install Python 3 to run the CLI.</span></span> 

## <a name="install-or-update"></a><span data-ttu-id="019b3-116">Instalar ou atualizar</span><span class="sxs-lookup"><span data-stu-id="019b3-116">Install or update</span></span>

<span data-ttu-id="019b3-117">Instalar e atualizar a CLI exige executar novamente o script de instalação.</span><span class="sxs-lookup"><span data-stu-id="019b3-117">Both installing and updating the CLI requires re-running the install script.</span></span> <span data-ttu-id="019b3-118">Instale a CLI executando `curl`.</span><span class="sxs-lookup"><span data-stu-id="019b3-118">Install the CLI by running `curl`.</span></span>

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

<span data-ttu-id="019b3-119">O script também pode ser baixado e executado localmente.</span><span class="sxs-lookup"><span data-stu-id="019b3-119">The script can also be downloaded and run locally.</span></span> <span data-ttu-id="019b3-120">Talvez você precise reiniciar o shell para que as alterações entrem em vigor.</span><span class="sxs-lookup"><span data-stu-id="019b3-120">You may have to restart your shell in order for changes to take effect.</span></span>

<span data-ttu-id="019b3-121">É possível executar a CLI do Azure com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="019b3-121">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="019b3-122">Para entrar, use o comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="019b3-122">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="019b3-123">Para saber mais sobre os diferentes métodos de autenticação, confira [Entrar com a CLI do Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="019b3-123">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="019b3-124">solução de problemas</span><span class="sxs-lookup"><span data-stu-id="019b3-124">Troubleshooting</span></span>

<span data-ttu-id="019b3-125">Aqui estão alguns problemas comuns observados durante uma instalação manual.</span><span class="sxs-lookup"><span data-stu-id="019b3-125">Here are some common problems seen during a manual installation.</span></span> <span data-ttu-id="019b3-126">Se você tiver um problema não abordado aqui, [arquive um problema no GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="019b3-126">If you experience a problem not covered here, [file an issue on GitHub](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="curl-object-moved-error"></a><span data-ttu-id="019b3-127">Erro "Objeto movido" de cURL</span><span class="sxs-lookup"><span data-stu-id="019b3-127">curl "Object Moved" error</span></span>

<span data-ttu-id="019b3-128">Se você receber um erro de `curl` relacionado ao parâmetro `-L` ou uma mensagem de erro incluindo o texto "Objeto movido", tente usar a URL completa em vez da `aka.ms` de redirecionamento:</span><span class="sxs-lookup"><span data-stu-id="019b3-128">If you get an error from `curl` related to the `-L` parameter, or an error message including the text "Object Moved", try using the full URL instead of the `aka.ms` redirect:</span></span>

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a><span data-ttu-id="019b3-129">`az` comando não encontrado</span><span class="sxs-lookup"><span data-stu-id="019b3-129">`az` command not found</span></span>

<span data-ttu-id="019b3-130">Se não conseguir executar o comando após a instalação e usar `bash` ou `zsh`, limpe o cache do hash de comando do shell.</span><span class="sxs-lookup"><span data-stu-id="019b3-130">If you can't run the command after installation and using `bash` or `zsh`, clear your shell's command hash cache.</span></span> <span data-ttu-id="019b3-131">Executar</span><span class="sxs-lookup"><span data-stu-id="019b3-131">Run</span></span>

```bash
hash -r
```

<span data-ttu-id="019b3-132">e verificar se o problema foi resolvido.</span><span class="sxs-lookup"><span data-stu-id="019b3-132">and check if the problem is resolved.</span></span>

<span data-ttu-id="019b3-133">O problema também pode ocorrer se você não reiniciou o shell após a instalação.</span><span class="sxs-lookup"><span data-stu-id="019b3-133">The issue can also occur if you didn't restart your shell after installation.</span></span> <span data-ttu-id="019b3-134">Verifique se o local do comando `az` está no `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="019b3-134">Make sure that the location of the `az` command is in your `$PATH`.</span></span> <span data-ttu-id="019b3-135">A localização do comando `az` é</span><span class="sxs-lookup"><span data-stu-id="019b3-135">The location of the `az` command is</span></span>

```bash
<install path>/bin
```

### <a name="proxy-blocks-connection"></a><span data-ttu-id="019b3-136">Conexão de blocos de proxy</span><span class="sxs-lookup"><span data-stu-id="019b3-136">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](includes/configure-proxy.md)]

<span data-ttu-id="019b3-137">Para obter os scripts de instalação, o proxy precisa permitir conexões HTTPS com os seguintes endereços:</span><span class="sxs-lookup"><span data-stu-id="019b3-137">In order to get the installation scripts, your proxy needs to allow HTTPS connections to the following addresses:</span></span>

* `https://aka.ms/`
* `https://azurecliprod.blob.core.windows.net/`
* `https://pypi.python.org`
* <span data-ttu-id="019b3-138">Pontos de extremidade usados pelo gerenciador de pacotes da distribuição (se houver) para pacotes essenciais</span><span class="sxs-lookup"><span data-stu-id="019b3-138">Endpoints used by your distribution's package manager (if any) for core packages</span></span>

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="uninstall"></a><span data-ttu-id="019b3-139">Desinstalar</span><span class="sxs-lookup"><span data-stu-id="019b3-139">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="019b3-140">Desinstale a CLI excluindo diretamente os arquivos do local escolhido no momento da instalação.</span><span class="sxs-lookup"><span data-stu-id="019b3-140">Uninstall the CLI by directly deleting the files from the location chosen at the time of installation.</span></span> <span data-ttu-id="019b3-141">O local de instalação padrão é `$HOME`.</span><span class="sxs-lookup"><span data-stu-id="019b3-141">The default install location is `$HOME`.</span></span>

1. <span data-ttu-id="019b3-142">Remova os arquivos da CLI instalados.</span><span class="sxs-lookup"><span data-stu-id="019b3-142">Remove the installed CLI files.</span></span>

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. <span data-ttu-id="019b3-143">Modifique o arquivo `$HOME/.bash_profile` para remover a seguinte linha:</span><span class="sxs-lookup"><span data-stu-id="019b3-143">Modify your `$HOME/.bash_profile` file to remove the following line:</span></span>

   ```text
   <install location>/lib/azure-cli/az.completion
   ```

3. <span data-ttu-id="019b3-144">Se usar `bash` ou `zsh`, recarregue o cache de comando do shell.</span><span class="sxs-lookup"><span data-stu-id="019b3-144">If using `bash` or `zsh`, reload your shell's command cache.</span></span>

   ```bash
   hash -r
   ```

## <a name="next-steps"></a><span data-ttu-id="019b3-145">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="019b3-145">Next Steps</span></span>

<span data-ttu-id="019b3-146">Agora que você instalou a CLI do Azure, faça um tour breve de seus recursos e comandos comuns.</span><span class="sxs-lookup"><span data-stu-id="019b3-146">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="019b3-147">Introdução à CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="019b3-147">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
