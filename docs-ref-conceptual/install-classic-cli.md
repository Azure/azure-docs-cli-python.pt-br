---
title: Instalar a CLI clássica do Azure
description: Instalar a CLI clássica do Azure para Mac, Linux e Windows para começar a usar os serviços do Azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 06/11/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 68aa728b9b9324a53856008f05d8ce30eb61c76d
ms.sourcegitcommit: 6d9169ed547df151f99e5a3ac86578634486419a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2018
ms.locfileid: "49652474"
---
# <a name="install-the-azure-classic-cli"></a><span data-ttu-id="9647f-103">Instalar a CLI clássica do Azure</span><span class="sxs-lookup"><span data-stu-id="9647f-103">Install the Azure classic CLI</span></span>

> [!IMPORTANT]
> <span data-ttu-id="9647f-104">Este tópico descreve como instalar a CLI clássica do Azure.</span><span class="sxs-lookup"><span data-stu-id="9647f-104">This topic describes how to install the Azure classic CLI.</span></span> <span data-ttu-id="9647f-105">A CLI clássica foi preterida e só deve ser usada com o modelo de implantação clássico.</span><span class="sxs-lookup"><span data-stu-id="9647f-105">The classic CLI is deprecated and should only be used with the classic deployment model.</span></span>
> <span data-ttu-id="9647f-106">Para todas as outras implantações, use [a CLI do Azure](/cli/azure).</span><span class="sxs-lookup"><span data-stu-id="9647f-106">For all other deployments, use [the Azure CLI](/cli/azure).</span></span>

<span data-ttu-id="9647f-107">Instale rapidamente a CLI clássica do Azure para usar comandos de software livre baseados em shell a fim de criar e gerenciar recursos no Microsoft Azure.</span><span class="sxs-lookup"><span data-stu-id="9647f-107">Quickly install the Azure classic CLI to use a set of open-source shell-based commands for creating and managing resources in Microsoft Azure.</span></span> <span data-ttu-id="9647f-108">Você tem várias opções para instalar essas ferramentas de plataforma cruzada em seu computador:</span><span class="sxs-lookup"><span data-stu-id="9647f-108">You have several options to install these cross-platform tools on your computer:</span></span>

* <span data-ttu-id="9647f-109">**Pacote npm**: execute o npm (o gerenciador de pacotes para JavaScript) para instalar o pacote da CLI clássica do Azure em sua distribuição Linux ou sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="9647f-109">**npm package** - Run npm (the package manager for JavaScript) to install the Azure classic CLI package on your Linux distribution or OS.</span></span> <span data-ttu-id="9647f-110">Requer Node.js e npm.</span><span class="sxs-lookup"><span data-stu-id="9647f-110">Requires node.js and npm.</span></span>
* <span data-ttu-id="9647f-111">**Instalador**: baixe um instalador para facilitar a instalação no macOS ou no Windows.</span><span class="sxs-lookup"><span data-stu-id="9647f-111">**Installer** - Download an installer for easy installation on macOS or Windows.</span></span>
* <span data-ttu-id="9647f-112">**Contêiner do Docker**: comece a usar a CLI clássica em um contêiner do Docker pronto para ser executado.</span><span class="sxs-lookup"><span data-stu-id="9647f-112">**Docker container** - Start using the classic CLI in a ready-to-run Docker container.</span></span> <span data-ttu-id="9647f-113">Requer um host do Docker.</span><span class="sxs-lookup"><span data-stu-id="9647f-113">Requires a Docker host.</span></span>

<span data-ttu-id="9647f-114">Para obter mais opções e um histórico, consulte o repositório do projeto no [GitHub](https://github.com/azure/azure-xplat-cli).</span><span class="sxs-lookup"><span data-stu-id="9647f-114">For more options and background, see the project repository on [GitHub](https://github.com/azure/azure-xplat-cli).</span></span>

<span data-ttu-id="9647f-115">Quando a CLI clássica do Azure estiver instalada conecte-a com `azure login` e execute os comandos`azure` na interface de linha de comando (Bash, Terminal, Prompt de comando e assim por diante) para trabalhar com os recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="9647f-115">Once the Azure classic CLI is installed, connect with `azure login` and run the `azure` commands from your command-line interface (Bash, Terminal, Command prompt, and so on) to work with your Azure resources.</span></span>

## <a name="option-1-install-an-npm-package"></a><span data-ttu-id="9647f-116">Opção 1: Instalar um pacote npm</span><span class="sxs-lookup"><span data-stu-id="9647f-116">Option 1: Install an npm package</span></span>

<span data-ttu-id="9647f-117">Para instalar a CLI clássica de um pacote npm, você precisa baixar e instalar os [Node.js e npm mais recentes](https://nodejs.org/en/download/package-manager/).</span><span class="sxs-lookup"><span data-stu-id="9647f-117">To install the classic CLI from an npm package, make sure you have downloaded and installed the [latest Node.js and npm](https://nodejs.org/en/download/package-manager/).</span></span> <span data-ttu-id="9647f-118">Em seguida, execute `npm install` para instalar o pacote azure-cli:</span><span class="sxs-lookup"><span data-stu-id="9647f-118">Then, run `npm install` to install the azure-cli package:</span></span>

```bash
npm install -g azure-cli
```

<span data-ttu-id="9647f-119">Em distribuições Linux, talvez seja necessário usar `sudo` para executar o comando `npm` com êxito, da seguinte forma:</span><span class="sxs-lookup"><span data-stu-id="9647f-119">On Linux distributions, you might need to use `sudo` to successfully run the `npm` command, as follows:</span></span>

```bash
sudo npm install -g azure-cli
```

> [!NOTE]
> <span data-ttu-id="9647f-120">Se você precisa instalar ou atualizar o Node.js e o npm em seu sistema operacional, recomendamos que você instale o Node.js LTS versão 4.x ou posterior.</span><span class="sxs-lookup"><span data-stu-id="9647f-120">If you need to install or update Node.js and npm on your OS, we recommend that you install Node.js LTS version 4.x or later.</span></span> <span data-ttu-id="9647f-121">Se você usar uma versão mais antiga, poderá obter erros de instalação.</span><span class="sxs-lookup"><span data-stu-id="9647f-121">If you use an older version, you might get installation errors.</span></span>

<span data-ttu-id="9647f-122">Se preferir, você também poderá baixar um arquivo tar das [Versões do GitHub](https://github.com/Azure/azure-xplat-cli/releases).</span><span class="sxs-lookup"><span data-stu-id="9647f-122">If you prefer, you may also download a tar file from the [GitHub releases](https://github.com/Azure/azure-xplat-cli/releases).</span></span> <span data-ttu-id="9647f-123">Em seguida, instale o pacote npm baixado da seguinte maneira (em distribuições Linux, talvez seja necessário usar `sudo`):</span><span class="sxs-lookup"><span data-stu-id="9647f-123">Then, install the downloaded npm package as follows (on Linux distributions you might need to use `sudo`):</span></span>

```bash
npm install -g <path to downloaded tar file>
```

## <a name="option-2-use-an-installer"></a><span data-ttu-id="9647f-124">Opção 2: Usar um instalador</span><span class="sxs-lookup"><span data-stu-id="9647f-124">Option 2: Use an installer</span></span>

<span data-ttu-id="9647f-125">Se você usa um computador Windows ou Mac, há instaladores DMG e MSI disponíveis nas [Versões do GitHub](https://github.com/Azure/azure-xplat-cli/releases).</span><span class="sxs-lookup"><span data-stu-id="9647f-125">If you use a Mac or Windows computer, DMG and MSI installers are available from [GitHub releases](https://github.com/Azure/azure-xplat-cli/releases).</span></span>

> [!TIP]
> <span data-ttu-id="9647f-126">No Windows, você também pode baixar o [Web Platform Installer](https://go.microsoft.com/?linkid=9828653) para instalar a CLI clássica.</span><span class="sxs-lookup"><span data-stu-id="9647f-126">On Windows, you can also download the [Web Platform Installer](https://go.microsoft.com/?linkid=9828653) to install the classic CLI.</span></span> <span data-ttu-id="9647f-127">Esse instalador dá a opção de instalar o SDK do Azure e outras ferramentas de linha de comando.</span><span class="sxs-lookup"><span data-stu-id="9647f-127">This installer gives you the option to install additional Azure SDK and command-line tools.</span></span>

## <a name="option-3-use-a-docker-container"></a><span data-ttu-id="9647f-128">Opção 3: Usar um contêiner do Docker</span><span class="sxs-lookup"><span data-stu-id="9647f-128">Option 3: Use a Docker container</span></span>

<span data-ttu-id="9647f-129">Se você tiver configurado seu computador como um host do [Docker](https://docs.docker.com/engine/understanding-docker/), execute a CLI clássica do Azure em um contêiner do Docker.</span><span class="sxs-lookup"><span data-stu-id="9647f-129">If you have set up your computer as a [Docker](https://docs.docker.com/engine/understanding-docker/) host, you can run the Azure classic CLI in a Docker container.</span></span> <span data-ttu-id="9647f-130">Execute o seguinte comando (em distribuições Linux, talvez seja necessário usar `sudo`):</span><span class="sxs-lookup"><span data-stu-id="9647f-130">Run the following command (on Linux distributions you might need to use `sudo`):</span></span>

```bash
docker run -it microsoft/azure-cli:0.10.17
```

## <a name="run-azure-classic-cli-commands"></a><span data-ttu-id="9647f-131">Executar comandos da CLI clássica do Azure</span><span class="sxs-lookup"><span data-stu-id="9647f-131">Run Azure classic CLI commands</span></span>

<span data-ttu-id="9647f-132">Quando a CLI clássica do Azure estiver instalada, execute o comando `azure` na interface do usuário de linha de comando (Bash, Terminal, Prompt de comando e assim por diante).</span><span class="sxs-lookup"><span data-stu-id="9647f-132">After the classic CLI is installed, run the `azure` command from your command-line user interface (Bash, Terminal, Command prompt, and so on).</span></span> <span data-ttu-id="9647f-133">Por exemplo, para executar o comando de ajuda, digite o seguinte:</span><span class="sxs-lookup"><span data-stu-id="9647f-133">For example, to run the help command, type the following:</span></span>

```azurecli
azure help
```

> [!NOTE]
> <span data-ttu-id="9647f-134">Em algumas distribuições Linux, você poderá receber um erro semelhante a `/usr/bin/env: ‘node’: No such file or directory`.</span><span class="sxs-lookup"><span data-stu-id="9647f-134">On some Linux distributions, you may receive an error similar to `/usr/bin/env: ‘node’: No such file or directory`.</span></span> <span data-ttu-id="9647f-135">Esse erro ocorre quando instalações recentes do Node.js são instaladas em /usr/bin/nodejs.</span><span class="sxs-lookup"><span data-stu-id="9647f-135">This error comes from recent installations of Node.js being installed at /usr/bin/nodejs.</span></span> <span data-ttu-id="9647f-136">Para corrigi-lo, crie um link simbólico para /usr/bin/node executando este comando:</span><span class="sxs-lookup"><span data-stu-id="9647f-136">To fix it, create a symbolic link to /usr/bin/node by running this command:</span></span>

```bash
sudo ln -s /usr/bin/nodejs /usr/bin/node
```

<span data-ttu-id="9647f-137">Para ver a versão da CLI clássica do Azure que você instalou, digite o seguinte:</span><span class="sxs-lookup"><span data-stu-id="9647f-137">To see the version of the Azure classic CLI installed, type the following:</span></span>

```azurecli
azure --version
```

> [!NOTE]
> <span data-ttu-id="9647f-138">Ao usar a CLI clássica do Azure pela primeira vez, você verá uma mensagem perguntando se deseja permitir que a Microsoft colete informações de uso.</span><span class="sxs-lookup"><span data-stu-id="9647f-138">When you first use Azure classic CLI, you see a message asking if you want to allow Microsoft to collect usage information.</span></span> <span data-ttu-id="9647f-139">A participação é voluntária.</span><span class="sxs-lookup"><span data-stu-id="9647f-139">Participation is voluntary.</span></span> <span data-ttu-id="9647f-140">Se optar por participar, você poderá parar a qualquer momento executando `azure telemetry --disable`.</span><span class="sxs-lookup"><span data-stu-id="9647f-140">If you choose to participate, you can stop at any time by running `azure telemetry --disable`.</span></span> <span data-ttu-id="9647f-141">Para habilitar a participação a qualquer momento, execute `azure telemetry --enable`.</span><span class="sxs-lookup"><span data-stu-id="9647f-141">To enable participation at any time, run `azure telemetry --enable`.</span></span>

## <a name="update-the-classic-cli"></a><span data-ttu-id="9647f-142">Atualizar a CLI clássica</span><span class="sxs-lookup"><span data-stu-id="9647f-142">Update the classic CLI</span></span>

<span data-ttu-id="9647f-143">A Microsoft pode lançar versões atualizadas da CLI clássica do Azure.</span><span class="sxs-lookup"><span data-stu-id="9647f-143">Microsoft may release updated versions of the Azure classic CLI.</span></span> <span data-ttu-id="9647f-144">Reinstale a CLI clássica usando o instalador do seu sistema operacional ou executando o contêiner do Docker mais recente.</span><span class="sxs-lookup"><span data-stu-id="9647f-144">Reinstall the classic CLI using the installer for your operating system, or run the latest Docker container.</span></span> <span data-ttu-id="9647f-145">Ou, caso tenha o Node.js e o npm mais recentes instalados, atualize-os digitando o que é mostrado abaixo (em distribuições Linux, talvez seja necessário usar `sudo`).</span><span class="sxs-lookup"><span data-stu-id="9647f-145">Or, if you have the latest Node.js and npm installed, update by typing the following (on Linux distributions you might need to use `sudo`).</span></span>

```bash
npm update -g azure-cli
```

## <a name="enable-tab-completion"></a><span data-ttu-id="9647f-146">Ativar o recurso auto-completar com TAB</span><span class="sxs-lookup"><span data-stu-id="9647f-146">Enable tab completion</span></span>

<span data-ttu-id="9647f-147">Há suporte à conclusão de tabulação de comandos da CLI clássica para Mac e Linux.</span><span class="sxs-lookup"><span data-stu-id="9647f-147">Tab completion of classic CLI commands is supported for Mac and Linux.</span></span>

<span data-ttu-id="9647f-148">Para habilitá-lo no zsh, execute:</span><span class="sxs-lookup"><span data-stu-id="9647f-148">To enable it in zsh, run:</span></span>

```bash
echo '. <(azure --completion)' >> .zshrc
```

<span data-ttu-id="9647f-149">Para habilitá-lo no bash, execute:</span><span class="sxs-lookup"><span data-stu-id="9647f-149">To enable it in bash, run:</span></span>

```bash
azure --completion >> ~/azure.completion.sh
echo 'source ~/azure.completion.sh' >> ~/.bash_profile
```

## <a name="next-steps"></a><span data-ttu-id="9647f-150">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="9647f-150">Next steps</span></span>

* <span data-ttu-id="9647f-151">Para saber mais sobre a CLI clássica do Azure, baixar o código-fonte, relatar problemas ou colaborar com o projeto, visite o [Repositório GitHub para a CLI clássica do Azure](https://github.com/azure/azure-xplat-cli).</span><span class="sxs-lookup"><span data-stu-id="9647f-151">To learn more about the Azure classic CLI, download source code, report problems, or contribute to the project, visit the [GitHub repository for the Azure classic CLI](https://github.com/azure/azure-xplat-cli).</span></span>
