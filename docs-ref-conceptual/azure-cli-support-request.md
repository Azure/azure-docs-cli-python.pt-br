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
# <a name="create-an-azure-support-request-in-azure-cli"></a><span data-ttu-id="650d7-103">Criar uma solicitação de suporte do Azure na CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="650d7-103">Create an Azure support request in Azure CLI</span></span>

<span data-ttu-id="650d7-104">A CLI do Azure permite que você crie e gerencie tíquetes de suporte do Azure.</span><span class="sxs-lookup"><span data-stu-id="650d7-104">The Azure CLI enables you to create and manage Azure support tickets.</span></span>

- <span data-ttu-id="650d7-105">Abrir um tíquete de suporte técnico, de cobrança, de gerenciamento de assinatura ou de limites de serviço e de assinatura (cota).</span><span class="sxs-lookup"><span data-stu-id="650d7-105">Open a technical, billing, subscription management, or subscription and service limits (quota) support ticket.</span></span>
- <span data-ttu-id="650d7-106">Obter uma lista de tíquetes de suporte e informações detalhadas sobre cada um deles.</span><span class="sxs-lookup"><span data-stu-id="650d7-106">Get a list of support tickets and detailed information about each ticket.</span></span> <span data-ttu-id="650d7-107">Limitar a pesquisa por tíquetes de suporte por status ou data de criação.</span><span class="sxs-lookup"><span data-stu-id="650d7-107">Narrow your search for support tickets by status or created date.</span></span>
- <span data-ttu-id="650d7-108">Atualizar a gravidade, o status do tíquete e as informações de contato de um tíquete de suporte.</span><span class="sxs-lookup"><span data-stu-id="650d7-108">Update severity, ticket status, and contact information for a support ticket.</span></span>
- <span data-ttu-id="650d7-109">Acrescentar uma nova comunicação a um tíquete de suporte ou obter uma lista de todas as comunicações de um tíquete de suporte.</span><span class="sxs-lookup"><span data-stu-id="650d7-109">Add a new communication to a support ticket or get a list of all communications for a support ticket.</span></span> <span data-ttu-id="650d7-110">Limitar a pesquisa por listas de comunicação pela data de criação ou pelo tipo de comunicação.</span><span class="sxs-lookup"><span data-stu-id="650d7-110">Narrow your search of communication lists by created date or communication type.</span></span>

<span data-ttu-id="650d7-111">Para criar uma solicitação de suporte, você precisa ser [Proprietário](/azure/role-based-access-control/built-in-roles#owner), [Colaborador](/azure/role-based-access-control/built-in-roles#contributor) ou ser atribuído à função [Colaborador de Solicitação de Suporte](/azure/role-based-access-control/built-in-roles#support-request-contributor) no nível da assinatura.</span><span class="sxs-lookup"><span data-stu-id="650d7-111">To create a support request, you must be an [Owner](/azure/role-based-access-control/built-in-roles#owner) or [Contributor](/azure/role-based-access-control/built-in-roles#contributor), or be assigned to the [Support Request Contributor](/azure/role-based-access-control/built-in-roles#support-request-contributor) role at the subscription level.</span></span> <span data-ttu-id="650d7-112">Para criar uma solicitação de suporte sem uma assinatura, como o cenário do Azure Active Directory, você precisa ser um [Administrador](/azure/active-directory/roles/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="650d7-112">To create a support request without a subscription, such as an Azure Active Directory scenario, you must be an [Admin](/azure/active-directory/roles/permissions-reference).</span></span>

[!INCLUDE [azure-cli-prepare-your-environment.md](includes/azure-cli-prepare-your-environment.md)]

## <a name="create-a-support-ticket"></a><span data-ttu-id="650d7-113">Criar um tíquete de suporte</span><span class="sxs-lookup"><span data-stu-id="650d7-113">Create a support ticket</span></span>

1. <span data-ttu-id="650d7-114">Para obter uma lista de serviços, use o comando [az support services list](/cli/azure/ext/support/support/services#ext_support_az_support_services_list):</span><span class="sxs-lookup"><span data-stu-id="650d7-114">To obtain a list of services, use the [az support services list](/cli/azure/ext/support/support/services#ext_support_az_support_services_list) command:</span></span>

   ```azurecli
   az support services list --output table
   ```

   <span data-ttu-id="650d7-115">Neste exemplo, localize o valor da **Máquina Virtual que executa o Windows**, que é **6f16735c-b0ae-b275-ad3a-03479cfa1396**.</span><span class="sxs-lookup"><span data-stu-id="650d7-115">For this example, find the value for **Virtual Machine running Windows**, which is **6f16735c-b0ae-b275-ad3a-03479cfa1396**.</span></span>

1. <span data-ttu-id="650d7-116">Para obter o tipo e o subtipo que descrevem o seu problema, execute o comando [az support services problem-classifications list](/cli/azure/ext/support/support/services/problem-classifications#ext_support_az_support_services_problem_classifications_list):</span><span class="sxs-lookup"><span data-stu-id="650d7-116">To get the problem type and problem subtype that describes your problem, run the [az support services problem-classifications list](/cli/azure/ext/support/support/services/problem-classifications#ext_support_az_support_services_problem_classifications_list) command:</span></span>

   ```azurecli
   az support services problem-classifications list --service-name 6f16735c-b0ae-b275-ad3a-03479cfa1396 --output table
   ```

   <span data-ttu-id="650d7-117">Neste exemplo, localize **Não consigo me conectar à minha VM/tenho um problema com meu IP**.</span><span class="sxs-lookup"><span data-stu-id="650d7-117">For this example, find **Cannot connect to my VM / I have an issue with my public IP**.</span></span> <span data-ttu-id="650d7-118">Esse tipo tem um valor de **e5c307e3-50ff-5dc9-c8ae-7d35051f88c9**.</span><span class="sxs-lookup"><span data-stu-id="650d7-118">That type has a value of **e5c307e3-50ff-5dc9-c8ae-7d35051f88c9**.</span></span>

1. <span data-ttu-id="650d7-119">Crie um tíquete usando o comando [az support tickets create](/cli/azure/ext/support/support/tickets#ext_support_az_support_tickets_create):</span><span class="sxs-lookup"><span data-stu-id="650d7-119">Create a ticket by using the [az support tickets create](/cli/azure/ext/support/support/tickets#ext_support_az_support_tickets_create) command:</span></span>

   ```azurecli
   az support tickets create --ticket-name "VM012" --title "Issue with public IP" \
      --description "This ticket involves a public IP address of a VM." \
      --problem-classification e5c307e3-50ff-5dc9-c8ae-7d35051f88c9 \
      --severity minimal --contact-first-name Kenneth --contact-last-name Liew \
      --contact-method email --contact-email Kenneth.Liew@Contoso.com \
      --contact-country US --contact-language English --contact-timezone "Pacific Standard Time"
   ```

<span data-ttu-id="650d7-120">Um engenheiro de suporte vai entrar em contato com você usando o método indicado.</span><span class="sxs-lookup"><span data-stu-id="650d7-120">A support engineer will contact you using the method you indicated.</span></span> <span data-ttu-id="650d7-121">Para obter informações sobre os tempos de resposta iniciais, confira [Escopo de suporte e capacidade de resposta](/support/plans/response/).</span><span class="sxs-lookup"><span data-stu-id="650d7-121">For information about initial response times, see [Support scope and responsiveness](/support/plans/response/).</span></span>

## <a name="manage-support-tickets"></a><span data-ttu-id="650d7-122">Gerenciar tíquetes de suporte</span><span class="sxs-lookup"><span data-stu-id="650d7-122">Manage support tickets</span></span>

<span data-ttu-id="650d7-123">Para ver os tíquetes de suporte da sua assinatura atual, execute o comando [az support tickets list](/cli/azure/ext/support/support/tickets#ext_support_az_support_tickets_list):</span><span class="sxs-lookup"><span data-stu-id="650d7-123">To see your support tickets for your current subscription, run the [az support tickets list](/cli/azure/ext/support/support/tickets#ext_support_az_support_tickets_list) command:</span></span>

```azurecli
az support tickets list
```

<span data-ttu-id="650d7-124">Para ver os tíquetes de suporte em outra assinatura, execute o comando [az account set](/cli/azure/account#az_account_set) para alterar a sua assinatura atual e, em seguida, execute o comando de visualização.</span><span class="sxs-lookup"><span data-stu-id="650d7-124">To see support tickets in another subscription, run the [az account set](/cli/azure/account#az_account_set) command to change your current subscription, and then run the command.</span></span>

<span data-ttu-id="650d7-125">Você também pode atualizar um tíquete usando o comando [az support tickets update](/cli/azure/ext/support/support/tickets#ext_support_az_support_tickets_update):</span><span class="sxs-lookup"><span data-stu-id="650d7-125">You can also update a ticket by using the [az support tickets update](/cli/azure/ext/support/support/tickets#ext_support_az_support_tickets_update) command:</span></span>

```azurecli
az support tickets update --ticket-name VM012 --severity moderate
```

## <a name="communicate-about-your-ticket"></a><span data-ttu-id="650d7-126">Comunicar-se sobre o seu tíquete</span><span class="sxs-lookup"><span data-stu-id="650d7-126">Communicate about your ticket</span></span>

<span data-ttu-id="650d7-127">Não é possível excluir um tíquete de suporte criado usando a CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="650d7-127">You can't delete a support ticket created by using Azure CLI.</span></span> <span data-ttu-id="650d7-128">Em vez disso, envie uma mensagem para fechar um tíquete.</span><span class="sxs-lookup"><span data-stu-id="650d7-128">Instead, send a message to close a ticket.</span></span> <span data-ttu-id="650d7-129">Se você precisar reabrir uma solicitação de suporte fechada, crie uma mensagem, que reabrirá automaticamente a solicitação.</span><span class="sxs-lookup"><span data-stu-id="650d7-129">If you need to reopen a closed support request, create a new message, which automatically reopens the request.</span></span>

<span data-ttu-id="650d7-130">Para se comunicar sobre o seu tíquete, execute o comando [az support tickets communications create](/cli/azure/ext/support/support/tickets/communications#ext_support_az_support_tickets_communications_create):</span><span class="sxs-lookup"><span data-stu-id="650d7-130">To communicate about your ticket, run the [az support tickets communications create](/cli/azure/ext/support/support/tickets/communications#ext_support_az_support_tickets_communications_create) command:</span></span>

```azurecli
az support tickets communications create --ticket-name VM012 \
    --communication-name "VM Delay" \
    --communication-body "Delaying VM fixes due to scheduling on our end." \
    --communication-subject "Delaying VM fixes due to scheduling on our end."
```

<span data-ttu-id="650d7-131">Para ver todas as comunicações de um tíquete, use o comando [az support tickets communications list](/cli/azure/ext/support/support/tickets/communications#ext_support_az_support_tickets_communications_list):</span><span class="sxs-lookup"><span data-stu-id="650d7-131">To see all the communications for a ticket, use the [az support tickets communications list](/cli/azure/ext/support/support/tickets/communications#ext_support_az_support_tickets_communications_list) command:</span></span>

```azurecli
az support tickets communications list --ticket-name VM012
```

<span data-ttu-id="650d7-132">Esse comando oferece um parâmetro `--filters` para restringir as suas respostas.</span><span class="sxs-lookup"><span data-stu-id="650d7-132">This command offers a `--filters` parameter to narrow your responses.</span></span>

```azurecli
az support tickets communications list --ticket-name VM012 \
    --filters "communicationType eq 'Web'"
```

## <a name="next-steps"></a><span data-ttu-id="650d7-133">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="650d7-133">Next steps</span></span>

- [<span data-ttu-id="650d7-134">Perguntas frequentes do Suporte do Azure</span><span class="sxs-lookup"><span data-stu-id="650d7-134">Azure Support FAQs</span></span>](/support/faq/)
- [<span data-ttu-id="650d7-135">Gravidade e níveis do Azure</span><span class="sxs-lookup"><span data-stu-id="650d7-135">Azure severity and levels</span></span>](/support/plans/response/)
- [<span data-ttu-id="650d7-136">Como criar um tíquete de suporte no portal do Azure</span><span class="sxs-lookup"><span data-stu-id="650d7-136">How to create a support ticket via Azure portal</span></span>](/azure/azure-portal/supportability/how-to-create-azure-support-request)
