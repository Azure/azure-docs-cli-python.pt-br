---
ms.topic: include
ms.date: 09/10/2020
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.custom: devx-track-azurecli
ms.openlocfilehash: 4835cc399942fba3cbf7408b1309480cd2bcc152
ms.sourcegitcommit: bd2dbc80328936dadd211764d25c32a14fc58083
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/04/2021
ms.locfileid: "100631155"
---
## <a name="prerequisites"></a><span data-ttu-id="3876c-101">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3876c-101">Prerequisites</span></span>

- <span data-ttu-id="3876c-102">Use o [Azure Cloud Shell](/azure/cloud-shell/quickstart) usando o ambiente bash.</span><span class="sxs-lookup"><span data-stu-id="3876c-102">Use [Azure Cloud Shell](/azure/cloud-shell/quickstart) using the bash environment.</span></span>

   <span data-ttu-id="3876c-103">[![Inserir inicialização](https://shell.azure.com/images/launchcloudshell.png "Iniciar o Azure Cloud Shell")](https://shell.azure.com)</span><span class="sxs-lookup"><span data-stu-id="3876c-103">[![Embed launch](https://shell.azure.com/images/launchcloudshell.png "Launch Azure Cloud Shell")](https://shell.azure.com)</span></span>   
- <span data-ttu-id="3876c-104">Se preferir, [instale](../install-azure-cli.md) a CLI do Azure para executar comandos de referência da CLI.</span><span class="sxs-lookup"><span data-stu-id="3876c-104">If you prefer, [install](../install-azure-cli.md) the Azure CLI to run CLI reference commands.</span></span>
   - <span data-ttu-id="3876c-105">Se estiver usando uma instalação local, entre com a CLI do Azure usando o comando [az login](/cli/azure/reference-index#az_login).</span><span class="sxs-lookup"><span data-stu-id="3876c-105">If you're using a local install, sign in with Azure CLI by using the [az login](/cli/azure/reference-index#az_login) command.</span></span>  <span data-ttu-id="3876c-106">Para concluir o processo de autenticação, siga as etapas exibidas no terminal.</span><span class="sxs-lookup"><span data-stu-id="3876c-106">To finish the authentication process, follow the steps displayed in your terminal.</span></span>  <span data-ttu-id="3876c-107">Confira [Entrar com a CLI do Azure](../authenticate-azure-cli.md) para obter outras opções de entrada.</span><span class="sxs-lookup"><span data-stu-id="3876c-107">See [Sign in with Azure CLI](../authenticate-azure-cli.md) for additional sign-in options.</span></span>
  - <span data-ttu-id="3876c-108">Quando solicitado, instale as extensões da CLI do Azure no primeiro uso.</span><span class="sxs-lookup"><span data-stu-id="3876c-108">When you're prompted, install Azure CLI extensions on first use.</span></span>  <span data-ttu-id="3876c-109">Para obter mais informações sobre extensões, confira [Usar extensões com a CLI do Azure](../azure-cli-extensions-overview.md).</span><span class="sxs-lookup"><span data-stu-id="3876c-109">For more information about extensions, see [Use extensions with Azure CLI](../azure-cli-extensions-overview.md).</span></span>
  - <span data-ttu-id="3876c-110">Execute [az version](/cli/azure/reference-index#az_version) para localizar a versão e as bibliotecas dependentes que estão instaladas.</span><span class="sxs-lookup"><span data-stu-id="3876c-110">Run [az version](/cli/azure/reference-index#az_version) to find the version and dependent libraries that are installed.</span></span> <span data-ttu-id="3876c-111">Para fazer a atualização para a versão mais recente, execute [az upgrade](/cli/azure/reference-index#az_upgrade).</span><span class="sxs-lookup"><span data-stu-id="3876c-111">To upgrade to the latest version, run [az upgrade](/cli/azure/reference-index#az_upgrade).</span></span>
