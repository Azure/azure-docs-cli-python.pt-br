---
title: Gerenciar as assinaturas do Azure com a CLI do Azure 2.0
description: Gerencie as assinaturas do Azure com a CLI 2.0 no Linux, Mac ou Windows.
keywords: Assinatura da CLI do Azure 2.0, Linux, Mac, Windows, OS X
author: kamaljit
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 98fb955e-6dbf-47e2-80ac-170d6d95cb70
ms.openlocfilehash: 383fb6ebd90ac79f60869187b402d53d4f1791fd
ms.sourcegitcommit: 4fd631a58cf19c494162510d073fbbbdf0524d16
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/05/2017
---
# <a name="manage-multiple-azure-subscriptions"></a><span data-ttu-id="1de7a-104">Gerenciar várias assinaturas do Azure</span><span class="sxs-lookup"><span data-stu-id="1de7a-104">Manage multiple Azure subscriptions</span></span>

<span data-ttu-id="1de7a-105">Se você for novo no Azure, provavelmente tem apenas uma única assinatura.</span><span class="sxs-lookup"><span data-stu-id="1de7a-105">If you are brand new to Azure, you probably only have a single subscription.</span></span>
<span data-ttu-id="1de7a-106">Mas se você já usa o Azure por algum tempo, poderá criar várias assinaturas do Azure.</span><span class="sxs-lookup"><span data-stu-id="1de7a-106">But if you have been using Azure for a while, you may have created multiple Azure subscriptions.</span></span>
<span data-ttu-id="1de7a-107">Se esse for o caso, configure a CLI do Azure 2.0 para executar comandos em uma assinatura específica.</span><span class="sxs-lookup"><span data-stu-id="1de7a-107">If so, you can configure Azure CLI 2.0 to execute commands against a particular subscription.</span></span>

[!INCLUDE [cloud-shell-try-it.md](includes/cloud-shell-try-it.md)]

1. <span data-ttu-id="1de7a-108">Obtenha uma lista de todas as assinaturas em sua conta.</span><span class="sxs-lookup"><span data-stu-id="1de7a-108">Get a list of all subscriptions in your account.</span></span>

   ```azurecli-interactive
   az account list --output table
   ```

   ```Output
   Name                                         CloudName    SubscriptionId                        State     IsDefault
   -------------------------------------------  -----------  ------------------------------------  --------  -----------
   My Production Subscription                   AzureCloud   XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX  Enabled
   My DevTest Subscription                      AzureCloud   XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX  Enabled   True
   My Demos                                     AzureCloud   XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX  Enabled
   ```

1. <span data-ttu-id="1de7a-109">Defina o padrão.</span><span class="sxs-lookup"><span data-stu-id="1de7a-109">Set the default.</span></span>
 
   ```azurecli-interactive
   az account set --subscription "My Demos"
   ```

   > [!NOTE]
   > <span data-ttu-id="1de7a-110">O parâmetro `--subscription` fica com o nome da assinatura ou com a ID da assinatura.</span><span class="sxs-lookup"><span data-stu-id="1de7a-110">The `--subscription` parameter takes either the subscription name or the subscription ID.</span></span>

<span data-ttu-id="1de7a-111">Verifique a alteração ao executar o comando `az account list --output table` novamente.</span><span class="sxs-lookup"><span data-stu-id="1de7a-111">You can verify the change by running the `az account list --output table` command again.</span></span>

<span data-ttu-id="1de7a-112">Após configurar sua assinatura padrão, todos os comandos subsequentes da CLI do Azure serão executados nessa assinatura.</span><span class="sxs-lookup"><span data-stu-id="1de7a-112">Once you set your default subscription, all subsequent Azure CLI commands run against this subscription.</span></span>