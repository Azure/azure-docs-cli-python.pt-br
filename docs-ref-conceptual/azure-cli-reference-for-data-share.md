---
title: Referências da CLI do Azure para o Azure Data Share
description: Página de aterrissagem da referência da CLI do Azure para o Azure Data Share
services: data-share
author: dbradish-microsoft
manager: barbkess
ms.service: data-share
ms.devlang: azurecli
ms.topic: reference
ms.date: 05/27/2020
ms.author: dbradish
ms.openlocfilehash: 404022b13f44174e4b647f0430a58fac5eeb81df
ms.sourcegitcommit: c473377d1c08ac4efd2480bf852c30dbf1044a57
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2020
ms.locfileid: "86415547"
---
# <a name="azure-cli-for-azure-data-share"></a><span data-ttu-id="9ce28-103">CLI do Azure para o Azure Data Share</span><span class="sxs-lookup"><span data-stu-id="9ce28-103">Azure CLI for Azure Data Share</span></span>

<span data-ttu-id="9ce28-104">A [CLI do Azure](/cli/azure/what-is-azure-cli) (Interface de Linha de Comando do Azure) é um conjunto de comandos usados para criar e gerenciar recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="9ce28-104">The Azure Command Line Interface ([Azure CLI](/cli/azure/what-is-azure-cli)) is a set of commands used to create and manage Azure resources.</span></span>  <span data-ttu-id="9ce28-105">Ela está disponível em muitos serviços do Azure, incluindo o Azure Data Share.</span><span class="sxs-lookup"><span data-stu-id="9ce28-105">It is available across many Azure services including Azure Data Share.</span></span>  <span data-ttu-id="9ce28-106">Há mais de 65 comandos diferentes para o compartilhamento de dados.</span><span class="sxs-lookup"><span data-stu-id="9ce28-106">There are over 65 different commands for data share!</span></span>  <span data-ttu-id="9ce28-107">Esses comandos oferecem a capacidade de trabalhar com eficiência com o serviço de uma linha de comando.</span><span class="sxs-lookup"><span data-stu-id="9ce28-107">These commands give you the ability to work effectively with the service from a command line.</span></span>

## <a name="references-for-data-share"></a><span data-ttu-id="9ce28-108">Referências para o Data Share</span><span class="sxs-lookup"><span data-stu-id="9ce28-108">References for Data Share</span></span>

<span data-ttu-id="9ce28-109">Todos os comandos da CLI do Azure para o Azure Data Share são atualmente extensões para a CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="9ce28-109">All Azure CLI commands for Azure Data Share are currently extensions to the Azure CLI.</span></span>  <span data-ttu-id="9ce28-110">Uma extensão fornece acesso a comandos experimentais e de pré-lançamento.</span><span class="sxs-lookup"><span data-stu-id="9ce28-110">An extension gives you access to experimental and pre-release commands.</span></span>  <span data-ttu-id="9ce28-111">Saiba mais sobre as referências de extensão em [Usar extensões com a CLI do Azure](/cli/azure/azure-cli-extensions-overview).</span><span class="sxs-lookup"><span data-stu-id="9ce28-111">Find out more about extension references in [Use extensions with Azure CLI](/cli/azure/azure-cli-extensions-overview).</span></span>

|<span data-ttu-id="9ce28-112">Referência da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="9ce28-112">Azure CLI Reference</span></span> |<span data-ttu-id="9ce28-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ce28-113">Description</span></span>
|-|-|-|
| [<span data-ttu-id="9ce28-114">az datashare</span><span class="sxs-lookup"><span data-stu-id="9ce28-114">az datashare</span></span>](/cli/azure/ext/datashare/datashare) | <span data-ttu-id="9ce28-115">Todos os comandos para gerenciar o Azure Data Share.</span><span class="sxs-lookup"><span data-stu-id="9ce28-115">All commands to manage Azure Data Share.</span></span>
| [<span data-ttu-id="9ce28-116">az datashare account</span><span class="sxs-lookup"><span data-stu-id="9ce28-116">az datashare account</span></span>](/cli/azure/ext/datashare/datashare/account) | <span data-ttu-id="9ce28-117">Comandos para gerenciar as contas do Azure Data Share.</span><span class="sxs-lookup"><span data-stu-id="9ce28-117">Commands to manage Azure Data Share accounts.</span></span>
| [<span data-ttu-id="9ce28-118">az datashare consumer</span><span class="sxs-lookup"><span data-stu-id="9ce28-118">az datashare consumer</span></span>](/cli/azure/ext/datashare/datashare/consumer) | <span data-ttu-id="9ce28-119">Comandos para os consumidores gerenciarem o Azure Data Share.</span><span class="sxs-lookup"><span data-stu-id="9ce28-119">Commands for consumers to manage Azure Data Share.</span></span>
| [<span data-ttu-id="9ce28-120">az datashare dataset</span><span class="sxs-lookup"><span data-stu-id="9ce28-120">az datashare dataset</span></span>](/cli/azure/ext/datashare/datashare/dataset) | <span data-ttu-id="9ce28-121">Comandos para os provedores gerenciarem os conjuntos de dados do Azure Data Share.</span><span class="sxs-lookup"><span data-stu-id="9ce28-121">Commands for providers to manage Azure Data Share datasets.</span></span>
| [<span data-ttu-id="9ce28-122">az datashare invitation</span><span class="sxs-lookup"><span data-stu-id="9ce28-122">az datashare invitation</span></span>](/cli/azure/ext/datashare/datashare/invitation) | <span data-ttu-id="9ce28-123">Comandos para os consumidores gerenciarem convites do Azure Data Share.</span><span class="sxs-lookup"><span data-stu-id="9ce28-123">Commands for consumers to manage Azure Data Share invitations.</span></span>
| [<span data-ttu-id="9ce28-124">az datashare provider-share-subscription</span><span class="sxs-lookup"><span data-stu-id="9ce28-124">az datashare provider-share-subscription</span></span>](/cli/azure/ext/datashare/datashare/provider-share-subscription) | <span data-ttu-id="9ce28-125">Comandos para os provedores gerenciarem assinaturas do Azure Data Share.</span><span class="sxs-lookup"><span data-stu-id="9ce28-125">Commands for providers to manage Azure Data Share subscriptions.</span></span>
| [<span data-ttu-id="9ce28-126">az datashare synchronization</span><span class="sxs-lookup"><span data-stu-id="9ce28-126">az datashare synchronization</span></span>](/cli/azure/ext/datashare/datashare/synchronization)  | <span data-ttu-id="9ce28-127">Comandos para gerenciar a sincronização do Azure Data Share.</span><span class="sxs-lookup"><span data-stu-id="9ce28-127">Commands to manage Azure Data Share synchronization.</span></span>
| [<span data-ttu-id="9ce28-128">az datashare synchronization-setting</span><span class="sxs-lookup"><span data-stu-id="9ce28-128">az datashare synchronization-setting</span></span>](/cli/azure/ext/datashare/datashare/synchronization-setting)  | <span data-ttu-id="9ce28-129">Comandos para os provedores gerenciarem as configurações de sincronização do Azure Data Share.</span><span class="sxs-lookup"><span data-stu-id="9ce28-129">Commands for providers to manage Azure Data Share synchronization settings.</span></span>

## <a name="reference-examples"></a><span data-ttu-id="9ce28-130">Exemplos de referência</span><span class="sxs-lookup"><span data-stu-id="9ce28-130">Reference examples</span></span>

<span data-ttu-id="9ce28-131">São fornecidos exemplos com todas as referências da CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="9ce28-131">Examples are provided with every Azure CLI reference.</span></span> <span data-ttu-id="9ce28-132">Embora você também possa concluir essas tarefas no portal do Azure, usar a CLI do Azure requer uma só linha de comando.</span><span class="sxs-lookup"><span data-stu-id="9ce28-132">Although you can also complete these tasks through the Azure portal, using the Azure CLI requires a single command line.</span></span>  <span data-ttu-id="9ce28-133">Veja alguns blocos de código para ter uma ideia de como é fácil usar a CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="9ce28-133">Here are a few code blocks to give you an idea of how easy it is to use the Azure CLI.</span></span>

<span data-ttu-id="9ce28-134">Para trabalhar com o Azure Data Share, primeiro você precisará de um grupo de recursos.</span><span class="sxs-lookup"><span data-stu-id="9ce28-134">To work with Azure Data Share, you'll first need a resource group.</span></span>  <span data-ttu-id="9ce28-135">Os grupos de recursos do Azure são simples de criar e gerenciar com a CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="9ce28-135">Azure resource groups are simple to create and manage with the Azure CLI.</span></span>  

```azurecli
#create a resource group
az group create -location westus -name MyResourceGroup
```

```azurecli
#get a list of resource groups for a subscription
az group list --subscription MySubscription --output table
```

<span data-ttu-id="9ce28-136">É tão simples criar uma conta de compartilhamento de dados.</span><span class="sxs-lookup"><span data-stu-id="9ce28-136">It is as straightforward to create a data share account.</span></span>

```azurecli
#create a data share account
az datashare account create --location "West US 2" --tags tag1=Red tag2=White --name MyAccount --resource-group MyResourceGroup
```

## <a name="see-also"></a><span data-ttu-id="9ce28-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="9ce28-137">See also</span></span>

* <span data-ttu-id="9ce28-138">[Introdução à CLI do Azure](/cli/azure/get-started-with-azure-cli) para saber mais sobre a instalação e a conexão.</span><span class="sxs-lookup"><span data-stu-id="9ce28-138">[Get started with Azure CLI](/cli/azure/get-started-with-azure-cli) to learn about installation and sign in.</span></span>

* <span data-ttu-id="9ce28-139">Descubra referências adicionais de [núcleo](/cli/azure/reference-index) e de [extensão](/cli/azure/azure-cli-extensions-list) na documentação da CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="9ce28-139">Discover additional [core](/cli/azure/reference-index) and [extension](/cli/azure/azure-cli-extensions-list) references in the Azure CLI documentation.</span></span>
