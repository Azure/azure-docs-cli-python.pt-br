---
title: Gerenciar assinaturas do Azure com a CLI do Azure
description: Saiba mais sobre locatários, usuários e assinaturas do Azure. Use a CLI do Azure para gerenciar suas assinaturas, criar grupos de gerenciamento e bloquear assinaturas.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 01/29/2021
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 6a980c45627c79c9e3f8c6c920944cc3dc62281f
ms.sourcegitcommit: 3e79897e0aeca4d74bc8ff0410121b011b5884ec
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2021
ms.locfileid: "99495220"
---
# <a name="use-azure-subscriptions-with-azure-cli"></a>Usar assinaturas do Azure com a CLI do Azure

Você pode ter várias assinaturas no Azure. Você pode fazer parte de mais de uma organização ou sua organização pode dividir o acesso a determinados recursos entre agrupamentos. A CLI do Azure dá suporte à seleção de uma assinatura globalmente e por comando.

Para obter informações detalhadas sobre assinaturas, cobrança e gerenciamento de custos, confira a [documentação sobre cobrança e gerenciamento de custos](/azure/billing/).

## <a name="tenants-users-and-subscriptions"></a>Locatários, usuários e assinaturas

Um _locatário_ é a entidade do Azure Active Directory que abrange toda a organização. Um locatário tem uma ou mais _assinaturas_ e _usuários_. Um usuário é um indivíduo e é associado a somente um locatário: a organização à qual pertence. Os usuários são as contas que se conectam ao Azure para criar, gerenciar e usar recursos. Um usuário pode ter acesso a várias _assinaturas_, que são contratos com a Microsoft para usar os serviços de nuvem, incluindo o Azure. Cada recurso é associado a uma assinatura.

* Para saber mais sobre as diferenças entre locatários, usuários e assinaturas, confira o [dicionário de terminologia de nuvem do Azure](/azure/azure-glossary-cloud-terminology).
* Para saber como adicionar uma nova assinatura ao seu locatário do Azure Active Directory, confira [Como associar ou adicionar uma assinatura do Azure ao locatário do Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).
* Para saber como entrar em um locatário específico, confira [Entrar com a CLI do Azure](./authenticate-azure-cli.md).

## <a name="commands-in-a-subscription"></a>Comandos em uma assinatura

Muitos comandos da CLI do Azure funcionam em uma assinatura. Você sempre pode especificar em qual assinatura deseja trabalhar usando o parâmetro **subscription** no comando. Esse parâmetro é opcional. Se você não especificar uma assinatura, o comando usará sua assinatura ativa atual.

Para ver a assinatura que você está usando no momento, execute o comando [az account show](/cli/azure/account#az_account_show):

```azurecli
az account show --output table
```

> [!TIP]
> O parâmetro `--output` é um parâmetro global, disponível para todos os comandos. O valor **table** apresenta a saída em um formato amigável. Para obter mais informações, confira [Formatos de saída para comandos da CLI do Azure](/cli/azure/format-output-azure-cli).

As assinaturas contêm grupos de recursos. Um grupo de recursos do Azure é um contêiner que mantém os recursos relacionados a uma solução do Azure. Se o comando funcionar com os recursos na sua assinatura ativa, você não precisará especificar `--subscription`.

Esse comando cria uma conta de armazenamento no grupo de recursos especificado:

```azurecli
az storage account create --resource-group StorageGroups --name storage136 \
    --location eastus --sku Standard_LRS
```

Se o grupo de armazenamento não fizer parte da sua assinatura ativa atual, esse comando falhará.

Se necessário, altere a assinatura ativa, conforme descrito na próxima seção, ou especifique a assinatura no comando:

```azurecli
az storage account create --resource-group StorageGroups --subscription "My Demos" \
    --name storage136 --location eastus --sku Standard_LRS
```

## <a name="change-the-active-subscription"></a>Alterar a assinatura ativa

Altere sua assinatura ativa usando o comando [az account set](/cli/azure/account#az-account-set).

Obtenha a lista de assinaturas usando o comando [az account list](/cli/azure/account#az-account-list):

```azurecli
az account list --output table
```

Esse comando lista todas as assinaturas que você pode acessar. Sua assinatura ativa é marcada como `True` na coluna `IsDefault`. Se você não vir uma assinatura esperada, adicione o parâmetro `--refresh` para obter a lista mais atual de assinaturas.

Para alternar para outra assinatura, use [az account set](/cli/azure/account#az-account-set) com a ID da assinatura ou o nome para o qual deseja alternar.

```azurecli
az account set --subscription "My Demos"
```

Suas assinaturas têm um nome e uma ID, que é um GUID. Você pode usar um desses comandos. Se você usar um nome que inclua espaços, use aspas.

Se você executar o comando [az account list](/cli/azure/account#az-account-list) novamente, a coluna `IsDefault` mostrará sua assinatura ativa atual.

## <a name="create-management-groups"></a>Criar grupos de gerenciamento

Os grupos de gerenciamento do Azure contêm assinaturas. Os grupos de gerenciamento fornecem uma forma de gerenciar o acesso, as políticas e a conformidade para essas assinaturas. Para obter mais informações, confira [O que são grupos de gerenciamento do Azure](/azure/governance/management-groups/overview).

Use os comandos [az account management-group](/cli/azure/account/management-group) para criar e gerenciar os grupos de gerenciamento do Azure.

Crie um grupo de gerenciamento para várias das suas assinaturas usando o comando [az account management-group create](/cli/azure/account/management-group#az_account_management_group_create):

```azurecli
az account management-group create --name Contoso01
```

Para ver todos os seus grupos de gerenciamento, use o comando [az account management-group list](/cli/azure/account/management-group#az_account_management_group_list):

```azurecli
az account management-group list
```

Adicione assinaturas ao novo grupo usando o comando [az account management-group subscription add](/cli/azure/account/management-group/subscription#az_account_management_group_subscription_add):

```azurecli
az account management-group subscription add --name Contoso01 --subscription "My Demos"
az account management-group subscription add --name Contoso01 --subscription "My Second Demos"
```

Para remover uma assinatura, use o comando [az account management-group subscription remove](/cli/azure/account/management-group/subscription#az_account_management_group_subscription_remove):

```azurecli
az account management-group subscription remove --name Contoso01 --subscription "My Demos"
```

Para remover um grupo de gerenciamento, execute o comando [az account management-group delete](/cli/azure/account/management-group#az_account_management_group_delete):

```azurecli
az account management-group delete --name Contoso01
```

A remoção de uma assinatura ou a exclusão de um grupo de gerenciamento não exclui nem desativa uma assinatura.

## <a name="set-a-subscription-lock"></a>Definir um bloqueio de assinatura

Como administrador, você poderá precisar bloquear uma assinatura para impedir que os usuários a excluam ou modifiquem. Para obter mais informações, confira [Bloquear recursos para impedir alterações inesperadas](/azure/azure-resource-manager/management/lock-resources).

Na CLI do Azure, use os comandos [az account lock](/cli/azure/account/lock). Por exemplo, o comando [az account lock create](/cli/azure/account/lock#az_account_lock_create) pode impedir que os usuários excluam uma assinatura:

```azurecli
az account lock create --name "Cannot delete subscription" --lock-type CanNotDelete
```

> [!NOTE]
> Você precisa ter as permissões apropriadas para criar ou alterar os bloqueios.

Para ver os bloqueios atuais na sua assinatura, use o comando [az account lock list](/cli/azure/account/lock#az_account_lock_list):

```azurecli
az account lock list --output table
```

Se você tornar uma conta somente leitura, o resultado será semelhante a atribuir permissões da função Leitor a todos os usuários. Para saber mais sobre como definir permissões para funções e usuários individuais, confira [Adicionar ou remover atribuições de função do Azure usando a CLI do Azure](/azure/role-based-access-control/role-assignments-cli).

Para ver os detalhes de um bloqueio, use o comando [az account lock show](/cli/azure/account/lock#az_account_lock_show):

```azurecli
az account lock show --name "Cannot delete subscription"
```

Você pode remover um bloqueio usando o comando [az account lock delete](/cli/azure/account/lock#az_account_lock_delete):

```azurecli
az account lock delete --name "Cannot delete subscription"
```

## <a name="see-also"></a>Confira também

* [Dicionário de terminologia de nuvem do Azure](/azure/azure-glossary-cloud-terminology)
* [Associar ou adicionar uma assinatura do Azure ao seu locatário do Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory)
* [Entrar com a CLI do Azure](./authenticate-azure-cli.md)
