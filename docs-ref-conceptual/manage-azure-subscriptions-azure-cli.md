---
title: Gerenciar assinaturas do Azure com a CLI do Azure
description: Gerencie as assinaturas do Azure com a CLI do Azure.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.produdct: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 27f094b68812cb68a6a33a6977d4fd58e4178731
ms.sourcegitcommit: f40bd067ece4e6ec13e259782ed8db3e33b61a75
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "53593652"
---
# <a name="use-multiple-azure-subscriptions"></a>Usar várias assinaturas do Azure

A maioria dos usuários do Azure terá somente uma assinatura. No entanto, se você fizer parte de mais de uma organização ou se sua organização tiver dividido o acesso a determinados recursos nos agrupamentos, poderá ter várias assinaturas no Azure. A CLI é compatível com a escolha de uma assinatura globalmente e por comando.

## <a name="tenants-users-and-subscriptions"></a>Locatários, usuários e assinaturas

Talvez você tenha alguma confusão sobre a diferença entre locatários, usuários e assinaturas no Azure. Um _locatário_ é a entidade do Azure Active Directory que abrange toda a organização. Esse locatário tem pelo menos uma _assinatura_ e _usuário_. Um usuário é um indivíduo e é associado a somente um locatário: a organização à qual pertence. Os usuários são as contas que se conectam ao Azure para criar, gerenciar e usar recursos.
Um usuário pode ter acesso a várias _assinaturas_, que são contratos com a Microsoft para usar os serviços de nuvem, incluindo o Azure. Cada recurso é associado a uma assinatura.

Para saber mais sobre as diferenças entre locatários, usuários e assinaturas, confira o [dicionário de terminologia de nuvem do Azure](/azure/azure-glossary-cloud-terminology).  Para saber como adicionar uma nova assinatura ao seu locatário do Azure Active Directory, confira [Como adicionar uma assinatura do Azure ao Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).
Para saber como entrar em um locatário específico, confira [Entrar com a CLI do Azure](/cli/azure/authenticate-azure-cli).

## <a name="change-the-active-subscription"></a>Alterar a assinatura ativa 

Para acessar os recursos de uma assinatura, você precisa trocar sua assinatura ativa ou usar o argumento `--subscription`. A troca da assinatura de todos os comandos é feita com [az account set](/cli/azure/account#az-account-set).

Para trocar sua assinatura ativa:

1. Obtenha a lista de assinaturas usando o comando [az account list](/cli/azure/account#az-account-list):

    ```azurecli-interactive
    az account list --output table
    ```
2. Use `az account set` com a ID da assinatura ou nome para o qual você deseja alterar.

    ```azurecli-interactive
    az account set --subscription "My Demos"
    ```

Para executar apenas um único comando com uma assinatura diferente, use o argumento `--subscription`. Esse argumento tem uma ID da assinatura ou o nome da assinatura:

```azurecli-interactive
az vm create --subscription "My Demos" --resource-group MyGroup --name NewVM --image Ubuntu
```
