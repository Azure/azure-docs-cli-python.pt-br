---
title: Gerenciar as assinaturas do Azure com a CLI do Azure
description: Gerenciar as assinaturas do Azure com a CLI do Azure.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 06/15/2018
ms.topic: conceptual
ms.produdct: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.service: active-directory
ms.openlocfilehash: fdc8ffca38a6a581ae63b0518df72f6e09110d07
ms.sourcegitcommit: 1a38729d6ae93c49137b3d49b6a9ec8a75eff190
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2018
ms.locfileid: "36262702"
---
# <a name="manage-multiple-azure-subscriptions"></a>Gerenciar várias assinaturas do Azure

A maioria dos usuários do Azure terá somente uma assinatura. No entanto, se você fizer parte de várias organizações ou sua organização tiver um acesso dividido a certos recursos em agrupamentos, poderá ter várias assinaturas no Azure. Várias assinaturas podem ser facilmente gerenciadas com a CLI definindo uma assinatura global para todos os comandos, ou selecionando uma assinatura em uma base por comando.

## <a name="tenants-users-and-subscriptions"></a>Locatários, usuários e assinaturas

Talvez você tenha alguma confusão sobre a diferença entre locatários, usuários e assinaturas no Azure. Um _locatário_ é a entidade do Azure Active Directory que abrange toda a organização. Esse locatário tem pelo menos uma _assinatura_ e _usuário_. Um usuário é um indivíduo e é associado a somente um locatário: a organização à qual pertence. Os usuários são as contas que fazem logon no Azure para provisionar e usar os recursos.
Um usuário pode ter acesso a várias _assinaturas_, que são contratos com a Microsoft para usar os serviços de nuvem, incluindo o Azure. Cada recurso é associado a uma assinatura.

Para saber mais sobre as diferenças entre locatários, usuários e assinaturas, confira o [dicionário de terminologia de nuvem do Azure](/azure/azure-glossary-cloud-terminology).  Para saber como adicionar uma nova assinatura ao seu locatário do Azure Active Directory, confira [Como adicionar uma assinatura do Azure ao Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).
Ao trabalhar com vários locatários, talvez seja necessário entrar em um locatário específico. Para isso, confira [Entrar com a CLI do Azure](/cli/azure/authenticate-azure-cli).

## <a name="work-with-multiple-subscriptions"></a>Como trabalhar com várias assinaturas

Para acessar os recursos contidos em uma assinatura, você precisa trocar sua assinatura ativa. A alternância de sua assinatura pode ser feita para todos os comandos da CLI do Azure com [az account set](/cli/azure/account#az-account-set), ou feita por uma base por comando usando o argumento `--subscription`.

Para começar, você precisará de uma lista de suas assinaturas disponíveis. Para obter, use o comando [az account list](/cli/azure/account#az-account-list):

```azurecli-interactive
az account list --output table
```

Para alterar a assinatura ativa globalmente, use `az account set` junto com a ID da assinatura ou o nome da assinatura:

```azurecli-interactive
az account set --subscription "My Demos"
```

Para usar uma assinatura específica para um comando, use o argumento `--subscription`. Esse argumento tem uma ID da assinatura ou o nome da assinatura:

```azurecli-interactive
az vm create --subscription "My Demos" --resource-group MyGroup --name NewVM --image Ubuntu
```
