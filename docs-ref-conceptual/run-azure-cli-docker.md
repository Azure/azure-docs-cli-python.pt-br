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
ms.openlocfilehash: 7a50682d549f6383e68128f2c2aef02dc2877a8e
ms.sourcegitcommit: 83826ca154c9f32c6091c63ce4b3e480694ba8d1
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/09/2018
ms.locfileid: "43144896"
---
# <a name="run-azure-cli-20-in-a-docker-container"></a><span data-ttu-id="d8770-103">Executar a CLI do Azure 2.0 em um contêiner do Docker</span><span class="sxs-lookup"><span data-stu-id="d8770-103">Run Azure CLI 2.0 in a Docker container</span></span>

<span data-ttu-id="d8770-104">Você pode usar o Docker para executar um contêiner do Linux autônomo com a CLI do Azure 2.0 pré-instalada.</span><span class="sxs-lookup"><span data-stu-id="d8770-104">You can use Docker to run a standalone Linux container with the Azure CLI 2.0 pre-installed.</span></span> <span data-ttu-id="d8770-105">O Docker permite que você inicie rapidamente com um ambiente no qual você pode experimentar a CLI para decidir se é ideal para você ou usar nossa imagem como uma base para sua própria implantação.</span><span class="sxs-lookup"><span data-stu-id="d8770-105">Docker lets you get started quickly with an environment where you can try out the CLI to decide if it's right for you, or use our image as a base for your own deployment.</span></span>

## <a name="run-in-a-docker-container"></a><span data-ttu-id="d8770-106">Executar em um contêiner do Docker</span><span class="sxs-lookup"><span data-stu-id="d8770-106">Run in a Docker container</span></span>

<span data-ttu-id="d8770-107">Instalar a CLI usando `docker run`.</span><span class="sxs-lookup"><span data-stu-id="d8770-107">Install the CLI using `docker run`.</span></span>

   ```bash
   docker run -it microsoft/azure-cli
   ```

> [!NOTE]
> <span data-ttu-id="d8770-108">Se você quiser acompanhar as chaves SSH do seu ambiente de usuário, você pode usar `-v ${HOME}/.ssh:/root/.ssh` para montar suas chaves SSH no ambiente.</span><span class="sxs-lookup"><span data-stu-id="d8770-108">If you want to pick up the SSH keys from your user environment, you can use `-v ${HOME}/.ssh:/root/.ssh` to mount your SSH keys in the environment.</span></span>
>
> ```bash
> docker run -it -v ${HOME}/.ssh:/root/.ssh microsoft/azure-cli
> ```

<span data-ttu-id="d8770-109">A CLI está instalada na imagem como o comando `az` no `/usr/local/bin`.</span><span class="sxs-lookup"><span data-stu-id="d8770-109">The CLI is installed on the image as the `az` command in `/usr/local/bin`.</span></span> <span data-ttu-id="d8770-110">Para entrar, execute o comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="d8770-110">To sign in, run the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="d8770-111">Para saber mais sobre os diferentes métodos de autenticação, consulte [Conectar com a CLI do Azure 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="d8770-111">To learn more about different authentication methods, see [Sign in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="update-docker-image"></a><span data-ttu-id="d8770-112">Atualizar imagem do Docker</span><span class="sxs-lookup"><span data-stu-id="d8770-112">Update Docker image</span></span>

<span data-ttu-id="d8770-113">Atualizar com o Docker requer obter a nova imagem e recriar qualquer contêiner existente.</span><span class="sxs-lookup"><span data-stu-id="d8770-113">Updating with Docker requires both pulling the new image and re-creating any existing containers.</span></span> <span data-ttu-id="d8770-114">Por esse motivo, você deve evitar o uso de um contêiner que hospeda a CLI como um armazenamento de dados.</span><span class="sxs-lookup"><span data-stu-id="d8770-114">For this reason you should try to avoid using a container that hosts the CLI as a data store.</span></span>

<span data-ttu-id="d8770-115">Atualizar sua imagem local com `docker pull`.</span><span class="sxs-lookup"><span data-stu-id="d8770-115">Update your local image with `docker pull`.</span></span>

```bash
docker pull microsoft/azure-cli
```

## <a name="uninstall-docker-image"></a><span data-ttu-id="d8770-116">Desinstalar imagem do Docker</span><span class="sxs-lookup"><span data-stu-id="d8770-116">Uninstall Docker image</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="d8770-117">Depois de parar qualquer contêiner executando a imagem da CLI, remova-o.</span><span class="sxs-lookup"><span data-stu-id="d8770-117">After halting any containers running the CLI image, remove it.</span></span>

```bash
docker rmi microsoft/azure-cli
```
