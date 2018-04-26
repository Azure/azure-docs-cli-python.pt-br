---
title: Instalar a CLI do Azure 2.0 para Linux manualmente
description: Como instalar a CLI do Azure 2.0 no Linux manualmente
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: a74a4d30709f5d10fc3a3f2b63c9df931ab0516b
ms.sourcegitcommit: 0e9aafa07311526f43661c8bd3a7eba7cbc2caed
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/20/2018
---
# <a name="install-azure-cli-20-on-linux-manually"></a><span data-ttu-id="0cc06-103">Instalar CLI do Azure 2.0 no Linux manualmente</span><span class="sxs-lookup"><span data-stu-id="0cc06-103">Install Azure CLI 2.0 on Linux manually</span></span>

<span data-ttu-id="0cc06-104">Se não tiver um pacote para a CLI do Azure disponível em sua distribuição, você sempre poderá instalar a CLI manualmente executando um script de instalação.</span><span class="sxs-lookup"><span data-stu-id="0cc06-104">If you do not have a package for the Azure CLI available on your distribution, you can always install the CLI manually by running an installation script.</span></span>

> [!NOTE]
> <span data-ttu-id="0cc06-105">É altamente recomendável que você use um gerenciador de pacotes para a CLI.</span><span class="sxs-lookup"><span data-stu-id="0cc06-105">It's strongly recommend that you use a package manager for the CLI.</span></span> <span data-ttu-id="0cc06-106">Um gerenciador de pacotes garante que você sempre obtenha as atualizações mais recentes, além da estabilidade dos componentes da CLI.</span><span class="sxs-lookup"><span data-stu-id="0cc06-106">A package manager makes sure you always get the latest updates, and guarantees the stability of CLI components.</span></span> <span data-ttu-id="0cc06-107">Verifique e veja se há um pacote de distribuição antes de instalar manualmente.</span><span class="sxs-lookup"><span data-stu-id="0cc06-107">Check and see if there is a package for your distribution before installing manually.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0cc06-108">pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0cc06-108">Prerequisites</span></span>

<span data-ttu-id="0cc06-109">Para instalar a CLI, você precisa dos seguintes softwares disponíveis em seu sistema:</span><span class="sxs-lookup"><span data-stu-id="0cc06-109">In order to install the CLI, you need the following software available on your system:</span></span>

* [<span data-ttu-id="0cc06-110">Python 2.7 ou Python 3. x</span><span class="sxs-lookup"><span data-stu-id="0cc06-110">Python 2.7 or Python 3.x</span></span>](https://www.python.org/downloads/)
* [<span data-ttu-id="0cc06-111">libffi</span><span class="sxs-lookup"><span data-stu-id="0cc06-111">libffi</span></span>](https://sourceware.org/libffi/)
* [<span data-ttu-id="0cc06-112">OpenSSL 1.0.2</span><span class="sxs-lookup"><span data-stu-id="0cc06-112">OpenSSL 1.0.2</span></span>](https://www.openssl.org/source/)

## <a name="install-or-update"></a><span data-ttu-id="0cc06-113">Instalar ou atualizar</span><span class="sxs-lookup"><span data-stu-id="0cc06-113">Install or update</span></span>

<span data-ttu-id="0cc06-114">Se você estiver instalando ou atualizando a CLI, precisa executar uma instalação completa.</span><span class="sxs-lookup"><span data-stu-id="0cc06-114">Whether you are installing or updating the CLI, you need to perform a full installation.</span></span> <span data-ttu-id="0cc06-115">Assim que tiver os pré-requisitos, poderá instalar a CLI executando `curl`.</span><span class="sxs-lookup"><span data-stu-id="0cc06-115">Once you have the prerequisites, you can install the CLI by running `curl`.</span></span>

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

<span data-ttu-id="0cc06-116">Você também pode baixar o script e executá-lo localmente.</span><span class="sxs-lookup"><span data-stu-id="0cc06-116">You can also download the script and run it locally instead.</span></span> <span data-ttu-id="0cc06-117">Talvez você precise reiniciar o shell para que as alterações entrem em vigor.</span><span class="sxs-lookup"><span data-stu-id="0cc06-117">You may have to restart your shell in order for changes to take effect.</span></span> 

<span data-ttu-id="0cc06-118">É possível executar a CLI do Azure com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="0cc06-118">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="0cc06-119">Para fazer logon, execute o comando `az login`.</span><span class="sxs-lookup"><span data-stu-id="0cc06-119">To log in, run the `az login` command.</span></span>

```azurecli
az login
```

<span data-ttu-id="0cc06-120">Para saber mais sobre os métodos de logon diferente, consulte [Fazer logon com a CLI do Azure 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="0cc06-120">To learn more about different login methods, see [Log in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="0cc06-121">solução de problemas</span><span class="sxs-lookup"><span data-stu-id="0cc06-121">Troubleshooting</span></span>

<span data-ttu-id="0cc06-122">Aqui estão alguns problemas comuns observados durante uma instalação manual.</span><span class="sxs-lookup"><span data-stu-id="0cc06-122">Here are some common problems seen during a manual installation.</span></span> <span data-ttu-id="0cc06-123">Se o problema não estiver listado aqui, [registre um problema no github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="0cc06-123">If your issue is not listed here, please [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>
### <a name="curl-object-moved-error"></a><span data-ttu-id="0cc06-124">Erro "Objeto movido" de cURL</span><span class="sxs-lookup"><span data-stu-id="0cc06-124">curl "Object Moved" error</span></span>

<span data-ttu-id="0cc06-125">Se você receber um erro de `curl` relacionado ao parâmetro `-L` ou uma mensagem de erro incluindo o texto "Objeto movido", tente usar a URL completa em vez da `aka.ms` de redirecionamento:</span><span class="sxs-lookup"><span data-stu-id="0cc06-125">If you get an error from `curl` related to the `-L` parameter, or an error message including the text "Object Moved", try using the full URL instead of the `aka.ms` redirect:</span></span>

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a><span data-ttu-id="0cc06-126">`az` comando não encontrado</span><span class="sxs-lookup"><span data-stu-id="0cc06-126">`az` command not found</span></span>

<span data-ttu-id="0cc06-127">Se não conseguir executar o comando após a instalação e usar `bash` ou `zsh`, limpe o cache do hash de comando do shell.</span><span class="sxs-lookup"><span data-stu-id="0cc06-127">If you can't run the command after installation and using `bash` or `zsh`, clear your shell's command hash cache.</span></span> <span data-ttu-id="0cc06-128">Executar</span><span class="sxs-lookup"><span data-stu-id="0cc06-128">Run</span></span>

```bash
hash -r
```

<span data-ttu-id="0cc06-129">e verificar se o problema foi resolvido.</span><span class="sxs-lookup"><span data-stu-id="0cc06-129">and check if the problem is resolved.</span></span>

<span data-ttu-id="0cc06-130">O problema também pode ocorrer se você não reiniciou o shell após a instalação.</span><span class="sxs-lookup"><span data-stu-id="0cc06-130">The issue can also occur if you did not restart your shell after installation.</span></span> <span data-ttu-id="0cc06-131">Verifique se o local do comando `az` está no `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="0cc06-131">Make sure that the location of the `az` command is in your `$PATH`.</span></span> <span data-ttu-id="0cc06-132">A localização do comando `az` é</span><span class="sxs-lookup"><span data-stu-id="0cc06-132">The location of the `az` command is</span></span>

```bash
<install path>/bin
```

## <a name="uninstall"></a><span data-ttu-id="0cc06-133">Desinstalar</span><span class="sxs-lookup"><span data-stu-id="0cc06-133">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="0cc06-134">Desinstale a CLI excluindo diretamente os arquivos do local escolhido no momento da instalação.</span><span class="sxs-lookup"><span data-stu-id="0cc06-134">Uninstall the CLI by directly deleting the files from the location chosen at the time of installation.</span></span> <span data-ttu-id="0cc06-135">O local de instalação padrão é `$HOME`.</span><span class="sxs-lookup"><span data-stu-id="0cc06-135">The default install location is `$HOME`.</span></span>

1. <span data-ttu-id="0cc06-136">Remova os arquivos da CLI instalados.</span><span class="sxs-lookup"><span data-stu-id="0cc06-136">Remove the installed CLI files.</span></span>

  ```bash
  rm -r <install location>/lib/azure-cli
  rm <install location>/bin/az
  ```
2. <span data-ttu-id="0cc06-137">Modifique o arquivo `$HOME/.bash_profile` para remover a seguinte linha:</span><span class="sxs-lookup"><span data-stu-id="0cc06-137">Modify your `$HOME/.bash_profile` file to remove the following line:</span></span>

  ```
  <install location>/lib/azure-cli/az.completion
  ```

3. <span data-ttu-id="0cc06-138">Se usar `bash` ou `zsh`, recarregue o cache de comando do shell.</span><span class="sxs-lookup"><span data-stu-id="0cc06-138">If using `bash` or `zsh`, reload your shell's command cache.</span></span>

  ```bash
  hash -r
  ```
