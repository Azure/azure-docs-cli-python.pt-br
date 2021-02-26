---
title: Criar uma solicitação de suporte do Azure na CLI do Azure
description: Saiba como usar os comandos az support da CLI do Azure para criar, atualizar e gerenciar as solicitações de suporte do Azure.
author: dbradish-microsoft
ms.author: dbradish
ms.service: azure-supportability
ms.topic: how-to
ms.date: 02/12/2021
ms.custom: template-how-to
ms.openlocfilehash: 446fe0d3a6d7c726167d07e8eb5f4cfa2321d9b7
ms.sourcegitcommit: 594e9c620a6f74f5eaedf91a7f6a791e03a64c74
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2021
ms.locfileid: "100631156"
---
# <a name="create-an-azure-support-request-in-azure-cli"></a>Criar uma solicitação de suporte do Azure na CLI do Azure

A CLI do Azure permite que você crie e gerencie tíquetes de suporte do Azure.

- Abrir um tíquete de suporte técnico, de cobrança, de gerenciamento de assinatura ou de limites de serviço e de assinatura (cota).
- Obter uma lista de tíquetes de suporte e informações detalhadas sobre cada um deles. Limitar a pesquisa por tíquetes de suporte por status ou data de criação.
- Atualizar a gravidade, o status do tíquete e as informações de contato de um tíquete de suporte.
- Acrescentar uma nova comunicação a um tíquete de suporte ou obter uma lista de todas as comunicações de um tíquete de suporte. Limitar a pesquisa por listas de comunicação pela data de criação ou pelo tipo de comunicação.

Para criar uma solicitação de suporte, você precisa ser [Proprietário](/azure/role-based-access-control/built-in-roles#owner), [Colaborador](/azure/role-based-access-control/built-in-roles#contributor) ou ser atribuído à função [Colaborador de Solicitação de Suporte](/azure/role-based-access-control/built-in-roles#support-request-contributor) no nível da assinatura. Para criar uma solicitação de suporte sem uma assinatura, como o cenário do Azure Active Directory, você precisa ser um [Administrador](/azure/active-directory/roles/permissions-reference).

[!INCLUDE [azure-cli-prepare-your-environment.md](includes/azure-cli-prepare-your-environment.md)]

## <a name="create-a-support-ticket"></a>Criar um tíquete de suporte

1. Para obter uma lista de serviços, use o comando [az support services list](/cli/azure/ext/support/support/services#ext_support_az_support_services_list):

   ```azurecli
   az support services list --output table
   ```

   Neste exemplo, localize o valor da **Máquina Virtual que executa o Windows**, que é **6f16735c-b0ae-b275-ad3a-03479cfa1396**.

1. Para obter o tipo e o subtipo que descrevem o seu problema, execute o comando [az support services problem-classifications list](/cli/azure/ext/support/support/services/problem-classifications#ext_support_az_support_services_problem_classifications_list):

   ```azurecli
   az support services problem-classifications list --service-name 6f16735c-b0ae-b275-ad3a-03479cfa1396 --output table
   ```

   Neste exemplo, localize **Não consigo me conectar à minha VM/tenho um problema com meu IP**. Esse tipo tem um valor de **e5c307e3-50ff-5dc9-c8ae-7d35051f88c9**.

1. Crie um tíquete usando o comando [az support tickets create](/cli/azure/ext/support/support/tickets#ext_support_az_support_tickets_create):

   ```azurecli
   az support tickets create --ticket-name "VM012" --title "Issue with public IP" \
      --description "This ticket involves a public IP address of a VM." \
      --problem-classification e5c307e3-50ff-5dc9-c8ae-7d35051f88c9 \
      --severity minimal --contact-first-name Kenneth --contact-last-name Liew \
      --contact-method email --contact-email Kenneth.Liew@Contoso.com \
      --contact-country US --contact-language English --contact-timezone "Pacific Standard Time"
   ```

Um engenheiro de suporte vai entrar em contato com você usando o método indicado. Para obter informações sobre os tempos de resposta iniciais, confira [Escopo de suporte e capacidade de resposta](/support/plans/response/).

## <a name="manage-support-tickets"></a>Gerenciar tíquetes de suporte

Para ver os tíquetes de suporte da sua assinatura atual, execute o comando [az support tickets list](/cli/azure/ext/support/support/tickets#ext_support_az_support_tickets_list):

```azurecli
az support tickets list
```

Para ver os tíquetes de suporte em outra assinatura, execute o comando [az account set](/cli/azure/account#az_account_set) para alterar a sua assinatura atual e, em seguida, execute o comando de visualização.

Você também pode atualizar um tíquete usando o comando [az support tickets update](/cli/azure/ext/support/support/tickets#ext_support_az_support_tickets_update):

```azurecli
az support tickets update --ticket-name VM012 --severity moderate
```

## <a name="communicate-about-your-ticket"></a>Comunicar-se sobre o seu tíquete

Não é possível excluir um tíquete de suporte criado usando a CLI do Azure. Em vez disso, envie uma mensagem para fechar um tíquete. Se você precisar reabrir uma solicitação de suporte fechada, crie uma mensagem, que reabrirá automaticamente a solicitação.

Para se comunicar sobre o seu tíquete, execute o comando [az support tickets communications create](/cli/azure/ext/support/support/tickets/communications#ext_support_az_support_tickets_communications_create):

```azurecli
az support tickets communications create --ticket-name VM012 \
    --communication-name "VM Delay" \
    --communication-body "Delaying VM fixes due to scheduling on our end." \
    --communication-subject "Delaying VM fixes due to scheduling on our end."
```

Para ver todas as comunicações de um tíquete, use o comando [az support tickets communications list](/cli/azure/ext/support/support/tickets/communications#ext_support_az_support_tickets_communications_list):

```azurecli
az support tickets communications list --ticket-name VM012
```

Esse comando oferece um parâmetro `--filters` para restringir as suas respostas.

```azurecli
az support tickets communications list --ticket-name VM012 \
    --filters "communicationType eq 'Web'"
```

## <a name="next-steps"></a>Próximas etapas

- [Perguntas frequentes do Suporte do Azure](/support/faq/)
- [Gravidade e níveis do Azure](/support/plans/response/)
- [Como criar um tíquete de suporte no portal do Azure](/azure/azure-portal/supportability/how-to-create-azure-support-request)
