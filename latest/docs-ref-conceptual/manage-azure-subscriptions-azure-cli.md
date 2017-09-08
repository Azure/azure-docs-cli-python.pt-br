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
ms.sourcegitcommit: f107cf927ea1ef51de181d87fc4bc078e9288e47
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2017
---
# <a name="manage-multiple-azure-subscriptions"></a>Gerenciar várias assinaturas do Azure

Se você for novo no Azure, provavelmente tem apenas uma única assinatura.
Mas se você já usa o Azure por algum tempo, poderá criar várias assinaturas do Azure.
Se esse for o caso, configure a CLI do Azure 2.0 para executar comandos em uma assinatura específica.

[!INCLUDE [cloud-shell-try-it.md](includes/cloud-shell-try-it.md)]

1. Obtenha uma lista de todas as assinaturas em sua conta.

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

1. Defina o padrão.
 
   ```azurecli-interactive
   az account set --subscription "My Demos"
   ```

   > [!NOTE]
   > O parâmetro `--subscription` fica com o nome da assinatura ou com a ID da assinatura.

Verifique a alteração ao executar o comando `az account list --output table` novamente.

Após configurar sua assinatura padrão, todos os comandos subsequentes da CLI do Azure serão executados nessa assinatura.