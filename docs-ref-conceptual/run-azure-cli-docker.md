---
title: Execute a CLI do Azure 2.0 em um Contêiner do Docker
description: Como executar um contêiner do Docker hospedando a CLI do Azure 2.0
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 01/29/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 277d9d3423af4941fb7f7fb57130fa1b7af7d32e
ms.sourcegitcommit: 0e688704889fc88b91588bb6678a933c2d54f020
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/11/2018
ms.locfileid: "44388330"
---
# <a name="run-azure-cli-20-in-a-docker-container"></a><span data-ttu-id="985e2-103">Executar a CLI do Azure 2.0 em um contêiner do Docker</span><span class="sxs-lookup"><span data-stu-id="985e2-103">Run Azure CLI 2.0 in a Docker container</span></span>

<span data-ttu-id="985e2-104">Você pode usar o Docker para executar um contêiner do Linux autônomo com a CLI do Azure 2.0 pré-instalada.</span><span class="sxs-lookup"><span data-stu-id="985e2-104">You can use Docker to run a standalone Linux container with the Azure CLI 2.0 pre-installed.</span></span> <span data-ttu-id="985e2-105">O Docker ajuda você a começar rapidamente com um ambiente isolado para executar a CLI.</span><span class="sxs-lookup"><span data-stu-id="985e2-105">Docker gets you started quickly with an isolated environment to run the CLI in.</span></span> <span data-ttu-id="985e2-106">A imagem também pode ser usada como base para suas próprias implantações.</span><span class="sxs-lookup"><span data-stu-id="985e2-106">The image can also be used as a base for your own deployments.</span></span>

## <a name="run-in-a-docker-container"></a><span data-ttu-id="985e2-107">Executar em um contêiner do Docker</span><span class="sxs-lookup"><span data-stu-id="985e2-107">Run in a Docker container</span></span>

<span data-ttu-id="985e2-108">Instalar a CLI usando `docker run`.</span><span class="sxs-lookup"><span data-stu-id="985e2-108">Install the CLI using `docker run`.</span></span>

   ```bash
   docker run -it microsoft/azure-cli
   ```

> [!NOTE]
> <span data-ttu-id="985e2-109">Se você quiser acompanhar as chaves SSH do seu ambiente de usuário, use `-v ${HOME}/.ssh:/root/.ssh` para montar suas chaves SSH no ambiente.</span><span class="sxs-lookup"><span data-stu-id="985e2-109">If you want to pick up the SSH keys from your user environment, use `-v ${HOME}/.ssh:/root/.ssh` to mount your SSH keys in the environment.</span></span>
>
> ```bash
> docker run -it -v ${HOME}/.ssh:/root/.ssh microsoft/azure-cli
> ```

<span data-ttu-id="985e2-110">A CLI está instalada na imagem como o comando `az` no `/usr/local/bin`.</span><span class="sxs-lookup"><span data-stu-id="985e2-110">The CLI is installed on the image as the `az` command in `/usr/local/bin`.</span></span> <span data-ttu-id="985e2-111">Para entrar, execute o comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="985e2-111">To sign in, run the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="985e2-112">Para saber mais sobre os diferentes métodos de autenticação, consulte [Conectar com a CLI do Azure 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="985e2-112">To learn more about different authentication methods, see [Sign in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="update-docker-image"></a><span data-ttu-id="985e2-113">Atualizar imagem do Docker</span><span class="sxs-lookup"><span data-stu-id="985e2-113">Update Docker image</span></span>

<span data-ttu-id="985e2-114">Atualizar com o Docker requer obter a nova imagem e recriar qualquer contêiner existente.</span><span class="sxs-lookup"><span data-stu-id="985e2-114">Updating with Docker requires both pulling the new image and re-creating any existing containers.</span></span> <span data-ttu-id="985e2-115">Por esse motivo, você deve evitar o uso de um contêiner que hospede a CLI como um armazenamento de dados.</span><span class="sxs-lookup"><span data-stu-id="985e2-115">For this reason, you should try to avoid using a container that hosts the CLI as a data store.</span></span>

<span data-ttu-id="985e2-116">Atualizar sua imagem local com `docker pull`.</span><span class="sxs-lookup"><span data-stu-id="985e2-116">Update your local image with `docker pull`.</span></span>

```bash
docker pull microsoft/azure-cli
```

## <a name="uninstall-docker-image"></a><span data-ttu-id="985e2-117">Desinstalar imagem do Docker</span><span class="sxs-lookup"><span data-stu-id="985e2-117">Uninstall Docker image</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="985e2-118">Depois de parar qualquer contêiner executando a imagem da CLI, remova-o.</span><span class="sxs-lookup"><span data-stu-id="985e2-118">After halting any containers running the CLI image, remove it.</span></span>

```bash
docker rmi microsoft/azure-cli
```
