---
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 12/15/2020
ms.topic: include
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 2cba7031b3fe4c54edcb7c0dcef6f37b97d2f785
ms.sourcegitcommit: d5f026468ea20bbd7ef35bdbf9852bcb2b812d83
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/23/2020
ms.locfileid: "97744588"
---
## <a name="overview"></a><span data-ttu-id="e833d-101">Visão geral</span><span class="sxs-lookup"><span data-stu-id="e833d-101">Overview</span></span>

> [!NOTE]
> <span data-ttu-id="e833d-102">É altamente recomendável instalar a CLI com um gerenciador de pacotes.</span><span class="sxs-lookup"><span data-stu-id="e833d-102">It's strongly recommend to install the CLI with a package manager.</span></span> <span data-ttu-id="e833d-103">Um gerenciador de pacotes garante que você sempre obtenha as atualizações mais recentes, além da estabilidade dos componentes da CLI.</span><span class="sxs-lookup"><span data-stu-id="e833d-103">A package manager makes sure you always get the latest updates, and guarantees the stability of CLI components.</span></span> <span data-ttu-id="e833d-104">Verifique e veja se há um pacote de distribuição antes de instalar manualmente.</span><span class="sxs-lookup"><span data-stu-id="e833d-104">Check and see if there is a package for your distribution before installing manually.</span></span>

<span data-ttu-id="e833d-105">A CLI requer o seguinte software:</span><span class="sxs-lookup"><span data-stu-id="e833d-105">The CLI requires the following software:</span></span>

* <span data-ttu-id="e833d-106">[Python 3.6.x, 3.7.x ou 3.8.x](https://www.python.org/downloads/).</span><span class="sxs-lookup"><span data-stu-id="e833d-106">[Python 3.6.x, 3.7.x or 3.8.x](https://www.python.org/downloads/).</span></span>
* [<span data-ttu-id="e833d-107">libffi</span><span class="sxs-lookup"><span data-stu-id="e833d-107">libffi</span></span>](https://sourceware.org/libffi/)
* [<span data-ttu-id="e833d-108">OpenSSL 1.0.2</span><span class="sxs-lookup"><span data-stu-id="e833d-108">OpenSSL 1.0.2</span></span>](https://www.openssl.org/source/)

> [!IMPORTANT]
>
> <span data-ttu-id="e833d-109">A CLI não é mais compatível com o Python 2.7 desde a versão `2.1.0`.</span><span class="sxs-lookup"><span data-stu-id="e833d-109">The CLI has dropped support for Python 2.7 since version `2.1.0`.</span></span> <span data-ttu-id="e833d-110">Não há garantia de que as novas versões serão executadas com o Python 2.7 corretamente.</span><span class="sxs-lookup"><span data-stu-id="e833d-110">New versions no longer guarantee to run with Python 2.7 correctly.</span></span>

## <a name="install-or-update"></a><span data-ttu-id="e833d-111">Instalar ou atualizar</span><span class="sxs-lookup"><span data-stu-id="e833d-111">Install or update</span></span>

<span data-ttu-id="e833d-112">Instalar e atualizar a CLI exige executar novamente o script de instalação.</span><span class="sxs-lookup"><span data-stu-id="e833d-112">Both installing and updating the CLI requires re-running the install script.</span></span> <span data-ttu-id="e833d-113">Instale a CLI executando `curl`.</span><span class="sxs-lookup"><span data-stu-id="e833d-113">Install the CLI by running `curl`.</span></span>

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

<span data-ttu-id="e833d-114">O script também pode ser baixado e executado localmente.</span><span class="sxs-lookup"><span data-stu-id="e833d-114">The script can also be downloaded and run locally.</span></span> <span data-ttu-id="e833d-115">Talvez você precise reiniciar o shell para que as alterações entrem em vigor.</span><span class="sxs-lookup"><span data-stu-id="e833d-115">You may have to restart your shell in order for changes to take effect.</span></span>

<span data-ttu-id="e833d-116">É possível executar a CLI do Azure com o comando `az`.</span><span class="sxs-lookup"><span data-stu-id="e833d-116">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="e833d-117">Para entrar, use o comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="e833d-117">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](interactive-login.md)]

<span data-ttu-id="e833d-118">Para saber mais sobre os diferentes métodos de autenticação, confira [Entrar com a CLI do Azure](../authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="e833d-118">To learn more about different authentication methods, see [Sign in with Azure CLI](../authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="e833d-119">Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="e833d-119">Troubleshooting</span></span>

<span data-ttu-id="e833d-120">Aqui estão alguns problemas comuns observados durante uma instalação manual.</span><span class="sxs-lookup"><span data-stu-id="e833d-120">Here are some common problems seen during a manual installation.</span></span> <span data-ttu-id="e833d-121">Se você tiver um problema não abordado aqui, [arquive um problema no GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="e833d-121">If you experience a problem not covered here, [file an issue on GitHub](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="curl-object-moved-error"></a><span data-ttu-id="e833d-122">Erro "Objeto movido" de cURL</span><span class="sxs-lookup"><span data-stu-id="e833d-122">curl "Object Moved" error</span></span>

<span data-ttu-id="e833d-123">Se você receber um erro de `curl` relacionado ao parâmetro `-L` ou uma mensagem de erro incluindo o texto "Objeto movido", tente usar a URL completa em vez da `aka.ms` de redirecionamento:</span><span class="sxs-lookup"><span data-stu-id="e833d-123">If you get an error from `curl` related to the `-L` parameter, or an error message including the text "Object Moved", try using the full URL instead of the `aka.ms` redirect:</span></span>

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a><span data-ttu-id="e833d-124">`az` comando não encontrado</span><span class="sxs-lookup"><span data-stu-id="e833d-124">`az` command not found</span></span>

<span data-ttu-id="e833d-125">Se não conseguir executar o comando após a instalação e usar `bash` ou `zsh`, limpe o cache do hash de comando do shell.</span><span class="sxs-lookup"><span data-stu-id="e833d-125">If you can't run the command after installation and using `bash` or `zsh`, clear your shell's command hash cache.</span></span> <span data-ttu-id="e833d-126">Executar</span><span class="sxs-lookup"><span data-stu-id="e833d-126">Run</span></span>

```bash
hash -r
```

<span data-ttu-id="e833d-127">e verificar se o problema foi resolvido.</span><span class="sxs-lookup"><span data-stu-id="e833d-127">and check if the problem is resolved.</span></span>

<span data-ttu-id="e833d-128">O problema também pode ocorrer se você não reiniciou o shell após a instalação.</span><span class="sxs-lookup"><span data-stu-id="e833d-128">The issue can also occur if you didn't restart your shell after installation.</span></span> <span data-ttu-id="e833d-129">Verifique se o local do comando `az` está no `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="e833d-129">Make sure that the location of the `az` command is in your `$PATH`.</span></span> <span data-ttu-id="e833d-130">A localização do comando `az` é</span><span class="sxs-lookup"><span data-stu-id="e833d-130">The location of the `az` command is</span></span>

```bash
<install path>/bin
```

### <a name="proxy-blocks-connection"></a><span data-ttu-id="e833d-131">Conexão de blocos de proxy</span><span class="sxs-lookup"><span data-stu-id="e833d-131">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](configure-proxy.md)]

<span data-ttu-id="e833d-132">Para obter os scripts de instalação, o proxy precisa permitir conexões HTTPS com os seguintes endereços:</span><span class="sxs-lookup"><span data-stu-id="e833d-132">In order to get the installation scripts, your proxy needs to allow HTTPS connections to the following addresses:</span></span>

* `https://aka.ms/`
* `https://azurecliprod.blob.core.windows.net/`
* `https://pypi.python.org`
* <span data-ttu-id="e833d-133">Pontos de extremidade usados pelo gerenciador de pacotes da distribuição (se houver) para pacotes essenciais</span><span class="sxs-lookup"><span data-stu-id="e833d-133">Endpoints used by your distribution's package manager (if any) for core packages</span></span>

[!INCLUDE[troubleshoot-wsl.md](troubleshoot-wsl.md)]

## <a name="uninstall"></a><span data-ttu-id="e833d-134">Desinstalar</span><span class="sxs-lookup"><span data-stu-id="e833d-134">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](uninstall-boilerplate.md)]

<span data-ttu-id="e833d-135">Desinstale a CLI excluindo diretamente os arquivos do local escolhido no momento da instalação.</span><span class="sxs-lookup"><span data-stu-id="e833d-135">Uninstall the CLI by directly deleting the files from the location chosen at the time of installation.</span></span> <span data-ttu-id="e833d-136">O local de instalação padrão é `$HOME`.</span><span class="sxs-lookup"><span data-stu-id="e833d-136">The default install location is `$HOME`.</span></span>

1. <span data-ttu-id="e833d-137">Remova os arquivos da CLI instalados.</span><span class="sxs-lookup"><span data-stu-id="e833d-137">Remove the installed CLI files.</span></span>

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. <span data-ttu-id="e833d-138">Modifique o arquivo `$HOME/.bash_profile` para remover a seguinte linha:</span><span class="sxs-lookup"><span data-stu-id="e833d-138">Modify your `$HOME/.bash_profile` file to remove the following line:</span></span>

   ```text
   <install location>/lib/azure-cli/az.completion
   ```

3. <span data-ttu-id="e833d-139">Se usar `bash` ou `zsh`, recarregue o cache de comando do shell.</span><span class="sxs-lookup"><span data-stu-id="e833d-139">If using `bash` or `zsh`, reload your shell's command cache.</span></span>

   ```bash
   hash -r
   ```