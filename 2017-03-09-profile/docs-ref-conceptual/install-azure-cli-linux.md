---
title: Instalar a CLI do Azure 2.0 para Linux manualmente
description: Como instalar a CLI do Azure 2.0 no Linux manualmente
keywords: CLI do Azure, Instalar CLI do Azure, linux do azure, linux instalar azure
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 11/01/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ROBOTS: NOINDEX,NOFOLLOW
ms.openlocfilehash: cf1405cae70762146f63bc6629edc0dd1d949fff
ms.sourcegitcommit: 2e4d0bdd94c626e061434883032367b5619de4fe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2017
---
# <a name="install-azure-cli-20-on-linux-manually"></a><span data-ttu-id="33663-104">Instalar CLI do Azure 2.0 no Linux manualmente</span><span class="sxs-lookup"><span data-stu-id="33663-104">Install Azure CLI 2.0 on Linux manually</span></span>

<span data-ttu-id="33663-105">Se você não tiver um pacote para a CLI do Azure disponível em sua distribuição, sempre poderá instalar a CLI manualmente executando um script de instalação.</span><span class="sxs-lookup"><span data-stu-id="33663-105">If you do not have a package for the Azure CLI available on your distribution, you can always install the CLI manualy by running an installation script.</span></span> <span data-ttu-id="33663-106">Se tiver um pacote disponível, este sempre será o método de instalação recomendado.</span><span class="sxs-lookup"><span data-stu-id="33663-106">If you do have a package available, that is always the recommended installation method.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="33663-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="33663-107">Prerequisites</span></span>

<span data-ttu-id="33663-108">Para instalar a CLI, você precisará do seguinte software disponível em seu sistema:</span><span class="sxs-lookup"><span data-stu-id="33663-108">In order to install the CLI, you will need the following software available on your system:</span></span>

* [<span data-ttu-id="33663-109">Python 2.7 ou Python 3. x</span><span class="sxs-lookup"><span data-stu-id="33663-109">Python 2.7 or Python 3.x</span></span>](https://www.python.org/downloads/)
* [<span data-ttu-id="33663-110">libffi</span><span class="sxs-lookup"><span data-stu-id="33663-110">libffi</span></span>](https://sourceware.org/libffi/)
* [<span data-ttu-id="33663-111">OpenSSL 1.0.2</span><span class="sxs-lookup"><span data-stu-id="33663-111">OpenSSL 1.0.2</span></span>](https://www.openssl.org/source/)

## <a name="install-or-update-manually"></a><span data-ttu-id="33663-112">Instalar ou atualizar manualmente</span><span class="sxs-lookup"><span data-stu-id="33663-112">Install or update manually</span></span>

<span data-ttu-id="33663-113">Se você estiver instalando ou atualizando a CLI, precisará executar uma instalação completa.</span><span class="sxs-lookup"><span data-stu-id="33663-113">Whether you are installing or updating the CLI, you will need to perform a full installation.</span></span> <span data-ttu-id="33663-114">Assim que tiver os pré-requisitos, poderá instalar a CLI executando `curl`.</span><span class="sxs-lookup"><span data-stu-id="33663-114">Once you have the prerequisites, you can install the CLI by running `curl`.</span></span>

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

<span data-ttu-id="33663-115">Se preferir ou não tiver o `curl` em seu sistema, poderá baixar o script e executá-lo localmente.</span><span class="sxs-lookup"><span data-stu-id="33663-115">If you would prefer, or do not have `curl` on your system, you can download the script and run it locally instead.</span></span> <span data-ttu-id="33663-116">Talvez você precise reiniciar o shell para que as alterações entrem em vigor.</span><span class="sxs-lookup"><span data-stu-id="33663-116">You may have to restart your shell in order for changes to take effect.</span></span> <span data-ttu-id="33663-117">Após a instalação, execute a CLI com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="33663-117">After installation, run the CLI with the `az` command.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="33663-118">Solucionar problemas</span><span class="sxs-lookup"><span data-stu-id="33663-118">Troubleshooting</span></span>

### <a name="curl-object-moved-error"></a><span data-ttu-id="33663-119">Erro "Objeto movido" de cURL</span><span class="sxs-lookup"><span data-stu-id="33663-119">curl "Object Moved" error</span></span>

<span data-ttu-id="33663-120">Se você receber um erro de `curl` relacionado ao parâmetro `-L` ou uma mensagem de erro incluindo o texto "Objeto movido", tente usar a URL completa em vez da `aka.ms` de redirecionamento:</span><span class="sxs-lookup"><span data-stu-id="33663-120">If you get an error from `curl` related to the `-L` parameter, or an error message including the text "Object Moved", try using the full URL instead of the `aka.ms` redirect:</span></span>

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a><span data-ttu-id="33663-121">`az` comando não encontrado</span><span class="sxs-lookup"><span data-stu-id="33663-121">`az` command not found</span></span>

<span data-ttu-id="33663-122">Após a instalação, se não puder executar o comando, talvez seja necessário limpar o cache do hash de comando do shell.</span><span class="sxs-lookup"><span data-stu-id="33663-122">After installation if you can't run the command, you may need to clear your shell's command hash cache.</span></span> <span data-ttu-id="33663-123">Executar</span><span class="sxs-lookup"><span data-stu-id="33663-123">Run</span></span>

```bash
hash -r
```

<span data-ttu-id="33663-124">e ver se o problema foi resolvido.</span><span class="sxs-lookup"><span data-stu-id="33663-124">and see if the problem is resolved.</span></span>

<span data-ttu-id="33663-125">Isso também poderá ocorrer se você não reiniciou o shell após a instalação.</span><span class="sxs-lookup"><span data-stu-id="33663-125">This can also occur if you did not restart your shell after installation.</span></span> <span data-ttu-id="33663-126">Verifique se o local do comando `az` está no `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="33663-126">Make sure that the location of the `az` command is in your `$PATH`.</span></span>

<span data-ttu-id="33663-127">Se você executou o script de instalação, isso irá:</span><span class="sxs-lookup"><span data-stu-id="33663-127">If you ran the installation script, this will be:</span></span>

```bash
<install path>/bin
```

## <a name="unstinall-manually"></a><span data-ttu-id="33663-128">Desinstalar manualmente</span><span class="sxs-lookup"><span data-stu-id="33663-128">Unstinall manually</span></span>

<span data-ttu-id="33663-129">Se você decidiu desinstalar a CLI do Azure, lamentamos sua saída.</span><span class="sxs-lookup"><span data-stu-id="33663-129">If you ever decide to uninstall the Azure CLI, we're sorry to see you go.</span></span> <span data-ttu-id="33663-130">Antes de desinstalar, use o comando `az feedback` para nos fornecer algumas razões por ter escolhido desinstalar e como poderíamos melhorar a experiência da CLI.</span><span class="sxs-lookup"><span data-stu-id="33663-130">Before you uninstall, use the `az feedback` command to give us some reasons why you chose to uninstall and how we could improve the CLI experience.</span></span> <span data-ttu-id="33663-131">Queremos assegurar que a CLI do Azure não tenha bugs e seja amigável o máximo possível.</span><span class="sxs-lookup"><span data-stu-id="33663-131">We want to make sure that the Azure CLI is as bug-free and user-friendly as we can make it.</span></span> <span data-ttu-id="33663-132">Você também pode [registrar um problema do github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="33663-132">You can also [file a github issue](https://github.com/Azure/azure-cli/issues).</span></span>

<span data-ttu-id="33663-133">Você pode desinstalar a CLI excluindo diretamente os arquivos do local de instalação.</span><span class="sxs-lookup"><span data-stu-id="33663-133">You can uninstall the CLI by directly deleting the files from the install location.</span></span> <span data-ttu-id="33663-134">O local de instalação deve ter sido selecionado no momento da instalação, se você instalou via script `https://aka.ms/InstallAzureCLI`.</span><span class="sxs-lookup"><span data-stu-id="33663-134">Your install location should have been chosen at the time of install, if you installed via the `https://aka.ms/InstallAzureCLI` script.</span></span> <span data-ttu-id="33663-135">O local de instalação padrão é `$HOME`.</span><span class="sxs-lookup"><span data-stu-id="33663-135">The default installation location is `$HOME`.</span></span>

<span data-ttu-id="33663-136">Primeiro, remova os arquivos CLI instalados:</span><span class="sxs-lookup"><span data-stu-id="33663-136">First, remove the installed CLI files:</span></span>

```bash
rm -r <install location>/lib/azure-cli
rm <install location>/bin/az
```

<span data-ttu-id="33663-137">Então, modifique o arquivo `$HOME/.bash_profile` para remover a linha:</span><span class="sxs-lookup"><span data-stu-id="33663-137">Then modify your `$HOME/.bash_profile` file to remove the line:</span></span>

```
<install location>/lib/azure-cli/az.completion
```

<span data-ttu-id="33663-138">E, por fim, recarregue o cache de comando do shell se ele usar um.</span><span class="sxs-lookup"><span data-stu-id="33663-138">And finally, reload your shell's command cache if it uses one.</span></span> <span data-ttu-id="33663-139">Os usuários `bash` e `zsh` precisarão executar esta etapa:</span><span class="sxs-lookup"><span data-stu-id="33663-139">`bash` and `zsh` users will need to perform this step:</span></span>

```bash
hash -r
```
