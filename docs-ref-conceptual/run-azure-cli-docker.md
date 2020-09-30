---
title: Executar a CLI do Azure em um contêiner do Docker
description: Como executar um contêiner do Docker hospedando a CLI do Azure
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 01/29/2018
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 524eefb786fbe3029ea027acfdc2cdbb3dcb7040
ms.sourcegitcommit: 5d29362589078b66d15f5cd494fe903a5195658d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/25/2020
ms.locfileid: "91225772"
---
# <a name="run-azure-cli-in-a-docker-container"></a><span data-ttu-id="dff78-103">Executar a CLI do Azure em um contêiner do Docker</span><span class="sxs-lookup"><span data-stu-id="dff78-103">Run Azure CLI in a Docker container</span></span>

<span data-ttu-id="dff78-104">Você pode usar o Docker para executar um contêiner do Linux autônomo com a CLI do Azure pré-instalada.</span><span class="sxs-lookup"><span data-stu-id="dff78-104">You can use Docker to run a standalone Linux container with the Azure CLI pre-installed.</span></span> <span data-ttu-id="dff78-105">O Docker ajuda você a começar rapidamente com um ambiente isolado para executar a CLI.</span><span class="sxs-lookup"><span data-stu-id="dff78-105">Docker gets you started quickly with an isolated environment to run the CLI in.</span></span> <span data-ttu-id="dff78-106">A imagem também pode ser usada como base para suas próprias implantações.</span><span class="sxs-lookup"><span data-stu-id="dff78-106">The image can also be used as a base for your own deployments.</span></span>

## <a name="run-in-a-docker-container"></a><span data-ttu-id="dff78-107">Executar em um contêiner do Docker</span><span class="sxs-lookup"><span data-stu-id="dff78-107">Run in a Docker container</span></span>

> [!NOTE]
> <span data-ttu-id="dff78-108">A CLI do Azure migrou para o [Registro de Contêiner da Microsoft](https://azure.microsoft.com/services/container-registry).</span><span class="sxs-lookup"><span data-stu-id="dff78-108">The Azure CLI has migrated to [Microsoft Container Registry](https://azure.microsoft.com/services/container-registry).</span></span> <span data-ttu-id="dff78-109">Ainda há suporte para marcas existentes no Hub do Docker, mas as novas versões só estarão disponíveis como mcr.microsoft.com/azure-cli.</span><span class="sxs-lookup"><span data-stu-id="dff78-109">Existing tags on Docker Hub are still supported, but new releases will only be available as mcr.microsoft.com/azure-cli.</span></span>

<span data-ttu-id="dff78-110">Instalar a CLI usando `docker run`.</span><span class="sxs-lookup"><span data-stu-id="dff78-110">Install the CLI using `docker run`.</span></span>

   ```bash
   docker run -it mcr.microsoft.com/azure-cli
   ```

> [!NOTE]
> <span data-ttu-id="dff78-111">Se você quiser acompanhar as chaves SSH do seu ambiente de usuário, use `-v ${HOME}/.ssh:/root/.ssh` para montar suas chaves SSH no ambiente.</span><span class="sxs-lookup"><span data-stu-id="dff78-111">If you want to pick up the SSH keys from your user environment, use `-v ${HOME}/.ssh:/root/.ssh` to mount your SSH keys in the environment.</span></span>
>
> ```bash
> docker run -it -v ${HOME}/.ssh:/root/.ssh mcr.microsoft.com/azure-cli
> ```

<span data-ttu-id="dff78-112">A CLI está instalada na imagem como o comando `az` no `/usr/local/bin`.</span><span class="sxs-lookup"><span data-stu-id="dff78-112">The CLI is installed on the image as the `az` command in `/usr/local/bin`.</span></span> <span data-ttu-id="dff78-113">Para entrar, execute o comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="dff78-113">To sign in, run the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="dff78-114">Para saber mais sobre os diferentes métodos de autenticação, confira [Entrar com a CLI do Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="dff78-114">To learn more about different authentication methods, see [Sign in with the Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="update-docker-image"></a><span data-ttu-id="dff78-115">Atualizar imagem do Docker</span><span class="sxs-lookup"><span data-stu-id="dff78-115">Update Docker image</span></span>

<span data-ttu-id="dff78-116">Atualizar com o Docker requer obter a nova imagem e recriar qualquer contêiner existente.</span><span class="sxs-lookup"><span data-stu-id="dff78-116">Updating with Docker requires both pulling the new image and re-creating any existing containers.</span></span> <span data-ttu-id="dff78-117">Por esse motivo, você deve evitar o uso de um contêiner que hospede a CLI como um armazenamento de dados.</span><span class="sxs-lookup"><span data-stu-id="dff78-117">For this reason, you should try to avoid using a container that hosts the CLI as a data store.</span></span>

<span data-ttu-id="dff78-118">Atualizar sua imagem local com `docker pull`.</span><span class="sxs-lookup"><span data-stu-id="dff78-118">Update your local image with `docker pull`.</span></span>

```bash
docker pull mcr.microsoft.com/azure-cli
```

## <a name="uninstall-docker-image"></a><span data-ttu-id="dff78-119">Desinstalar imagem do Docker</span><span class="sxs-lookup"><span data-stu-id="dff78-119">Uninstall Docker image</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="dff78-120">Depois de parar qualquer contêiner executando a imagem da CLI, remova-o.</span><span class="sxs-lookup"><span data-stu-id="dff78-120">After halting any containers running the CLI image, remove it.</span></span>

```bash
docker rmi mcr.microsoft.com/azure-cli
```

## <a name="next-steps"></a><span data-ttu-id="dff78-121">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="dff78-121">Next Steps</span></span>

<span data-ttu-id="dff78-122">Agora que você pronto para usar a CLI do Azure, faça um tour breve de seus recursos e comandos comuns.</span><span class="sxs-lookup"><span data-stu-id="dff78-122">Now that you're ready to use the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="dff78-123">Introdução à CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="dff78-123">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)