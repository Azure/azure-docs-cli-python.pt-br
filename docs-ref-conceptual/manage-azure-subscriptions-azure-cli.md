---
title: Gerenciar as assinaturas do Azure com a CLI do Azure 2.0
description: Gerencie as assinaturas do Azure com a CLI 2.0 no Linux, Mac ou Windows.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 10/30/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: b0c0b3f5e4d9bc651ad4781cb0906dc98d8531a3
ms.sourcegitcommit: 29d7366a0902488f4f4d39c2cb0e89368d5186ea
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2018
---
# <a name="manage-multiple-azure-subscriptions"></a>Gerenciar várias assinaturas do Azure

A maioria dos usuários do Azure terá somente uma assinatura. No entanto, se você fizer parte de várias organizações ou sua organização tiver um acesso dividido a certos recursos em agrupamentos, poderá ter várias assinaturas no Azure. Várias assinaturas podem ser facilmente gerenciadas com a CLI e as operações podem ser executadas selecionando uma assinatura.

## <a name="tenants-users-and-subscriptions"></a>Locatários, usuários e assinaturas

Talvez você tenha alguma confusão sobre a diferença entre locatários, usuários e assinaturas no Azure. Em geral, um _locatário_ é a entidade do Azure Active Directory que abrange toda a organização. Esse locatário tem pelo menos uma _assinatura_ e _usuário_. Um usuário é um indivíduo e é associado a somente um locatário, a organização à qual pertence. Os usuários são as contas que fazem logon no Azure para provisionar e usar os recursos. Um usuário pode ter acesso a várias _assinaturas_, que são contratos com a Microsoft para usar os serviços de nuvem, incluindo o Azure. Cada recurso é associado a uma assinatura.

Para saber mais sobre as diferenças entre locatários, usuários e assinaturas, confira o [dicionário de terminologia de nuvem do Azure](/azure/azure-glossary-cloud-terminology).
Para saber como adicionar uma nova assinatura ao seu locatário do Azure Active Directory, confira [Como adicionar uma assinatura do Azure ao Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).
Ao trabalhar com vários locatários, talvez seja necessário fazer logon em um locatário específico. Para isso, consulte [Fazer logon com a CLI do Azure 2.0](/cli/azure/authenticate-azure-cli).

## <a name="working-with-multiple-subscriptions"></a>Trabalhando com várias assinaturas

Para acessar os recursos contidos em uma assinatura, você precisa trocar sua assinatura ativa. Todo o trabalho com assinaturas é feito por meio do comando `az account`, que se refere ao contrato de serviço que representa uma assinatura, não à conta individual.

[!INCLUDE [cloud-shell-try-it.md](includes/cloud-shell-try-it.md)]

Para começar a trabalhar com suas assinaturas disponíveis, obtenha uma lista das disponíveis em sua conta:

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

Para alterar a assinatura ativa, você pode usar `az account set`:

```azurecli-interactive
az account set --subscription "My Demos"
```

É possível pode usar a ID da assinatura ou o nome da assinatura para selecioná-la.
