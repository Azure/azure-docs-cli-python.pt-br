---
title: Entrar com a CLI do Azure 2.0
description: Entre com a CLI do Azure 2.0 no Linux, Mac ou Windows.
keywords: CLI do Azure 2.0, Linux, Mac, Windows, OS X, Ubuntu, Debian, CentOS, RHEL, SUSE, CoreOS, Docker, Windows, Python, PIP
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 65becd3a-9d69-4415-8a30-777d13a0e7aa
ms.openlocfilehash: 4ab4f0de38614eff00f55bad96ea886bb007f3c0
ms.sourcegitcommit: 4fd631a58cf19c494162510d073fbbbdf0524d16
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/05/2017
---
# <a name="log-in-with-azure-cli-20"></a><span data-ttu-id="e182d-104">Entrar com a CLI do Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="e182d-104">Log in with Azure CLI 2.0</span></span>

<span data-ttu-id="e182d-105">Há várias maneiras de fazer logon e autenticar com a CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="e182d-105">There are several ways to log in and authenticate with the Azure CLI.</span></span> <span data-ttu-id="e182d-106">É a maneira mais simples para começar é fazer logon interativamente no navegador ou na linha de comando.</span><span class="sxs-lookup"><span data-stu-id="e182d-106">The simplest way to get started is to log in interactively through your browser, or to log in at the command line.</span></span> <span data-ttu-id="e182d-107">A abordagem recomendada é usar entidades de serviço que fornecem uma maneira para que você crie contas não-interativas para manipular os recursos.</span><span class="sxs-lookup"><span data-stu-id="e182d-107">Our recommended approach is to use service principals, which provide a way for you to create non-interactive accounts that you can use to manipulate resources.</span></span> <span data-ttu-id="e182d-108">Ao conceder apenas as permissões apropriadas necessárias para uma entidade de serviço, você pode garantir que seus scripts de automação fiquem ainda mais seguros.</span><span class="sxs-lookup"><span data-stu-id="e182d-108">By granting just the appropriate permissions needed to a service principal, you can ensure your automation scripts are even more secure.</span></span>

<span data-ttu-id="e182d-109">Comandos que são executados com a CLI são executados em sua assinatura padrão.</span><span class="sxs-lookup"><span data-stu-id="e182d-109">Commands that you run with the CLI are run against your default subscription.</span></span>  <span data-ttu-id="e182d-110">Se você tiver mais de uma assinatura, convém [confirmar sua assinatura padrão](manage-azure-subscriptions-azure-cli.md) e alterá-la adequadamente.</span><span class="sxs-lookup"><span data-stu-id="e182d-110">If you have more than one subscription, you may want to [confirm your default subscription](manage-azure-subscriptions-azure-cli.md) and change it appropriately.</span></span>

## <a name="interactive-log-in"></a><span data-ttu-id="e182d-111">Logon Interativo</span><span class="sxs-lookup"><span data-stu-id="e182d-111">Interactive log-in</span></span>

<span data-ttu-id="e182d-112">Faça logon interativamente usando seu navegador da Web.</span><span class="sxs-lookup"><span data-stu-id="e182d-112">Log in interactively from your web browser.</span></span>

[!INCLUDE [interactive_login](includes/interactive-login.md)]

## <a name="command-line"></a><span data-ttu-id="e182d-113">Linha de comando</span><span class="sxs-lookup"><span data-stu-id="e182d-113">Command line</span></span>

<span data-ttu-id="e182d-114">Forneça suas credenciais na linha de comando.</span><span class="sxs-lookup"><span data-stu-id="e182d-114">Provide your credentials on the command line.</span></span>

> [!Note]
> <span data-ttu-id="e182d-115">Essa abordagem não funciona com contas da Microsoft ou contas que tenham a autenticação de dois fatores habilitada.</span><span class="sxs-lookup"><span data-stu-id="e182d-115">This approach doesn't work with Microsoft accounts or accounts that have two-factor authentication enabled.</span></span>

```azurecli-interactive
az login -u <username> -p <password>
```

## <a name="logging-in-with-a-service-principal"></a><span data-ttu-id="e182d-116">Como fazer logon com uma entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="e182d-116">Logging in with a service principal</span></span>

<span data-ttu-id="e182d-117">As entidades de serviço são como as contas de usuário às quais você pode aplicar regras usando o Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e182d-117">Service principals are like user accounts to which you can apply rules using Azure Active Directory.</span></span>
<span data-ttu-id="e182d-118">Autenticar com uma entidade de serviço é a melhor maneira de proteger o uso de seus recursos do Azure dos scripts ou aplicativos que manipulam recursos.</span><span class="sxs-lookup"><span data-stu-id="e182d-118">Authenticating with a service principal is the best way to secure the usage of your Azure resources from either your scripts or applications that manipulate resources.</span></span>
<span data-ttu-id="e182d-119">Você define as funções que deseja que os usuários tenham por meio do conjunto de comandos do `az role`.</span><span class="sxs-lookup"><span data-stu-id="e182d-119">You define the roles you want your users to have via the `az role` set of commands.</span></span>
<span data-ttu-id="e182d-120">Você pode saber mais e ver exemplos de funções de entidade de serviço em nossos [artigos de referência de função az](https://docs.microsoft.com/cli/azure/role.md).</span><span class="sxs-lookup"><span data-stu-id="e182d-120">You can learn more and see examples of service principal roles in our [az role reference articles](https://docs.microsoft.com/cli/azure/role.md).</span></span>

1. <span data-ttu-id="e182d-121">Se você ainda não tiver uma entidade de serviço, [crie uma](create-an-azure-service-principal-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="e182d-121">If you don't already have a service principal, [create one](create-an-azure-service-principal-azure-cli.md).</span></span>

1. <span data-ttu-id="e182d-122">Faça logon com uma entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="e182d-122">Log in with the service principal.</span></span>

   ```azurecli-interactive
   az login --service-principal -u "http://my-app" -p <password> --tenant <tenant>
   ```

   <span data-ttu-id="e182d-123">Para obter o locatário, faça logon interativamente e obtenha a TenantId da sua assinatura.</span><span class="sxs-lookup"><span data-stu-id="e182d-123">To get your tenant, log in interactively and then get the tenantId from your subscription.</span></span>

   ```azurecli
   az account show
   ```

   ```json
   {
       "environmentName": "AzureCloud",
       "id": "********-****-****-****-************",
       "isDefault": true,
       "name": "Pay-As-You-Go",
       "state": "Enabled",
       "tenantId": "********-****-****-****-************",
       "user": {
       "name": "********",
       "type": "user"
       }
   }
   ```