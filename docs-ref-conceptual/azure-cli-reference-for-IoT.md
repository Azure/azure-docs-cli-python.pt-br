---
title: Referências da CLI do Azure para o Azure IoT
description: Página de aterrissagem da referência da CLI do Azure para o Azure IoT
author: dbradish-microsoft
manager: barbkess
ms.devlang: azurecli
ms.topic: reference
ms.date: 06/05/2020
ms.author: dbradish
ms.service: azure-cli
ms.reviewer: paymaun.heidari
ms.custom: devx-track-azurecli
ms.openlocfilehash: 9190140c64f6a9863666329206839bb2553ffe79
ms.sourcegitcommit: 2da241715d25407ed22c1065c0c793acfd865996
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/09/2020
ms.locfileid: "89562780"
---
# <a name="azure-cli-for-azure-iot"></a><span data-ttu-id="43edd-103">CLI do Azure para o Azure IoT</span><span class="sxs-lookup"><span data-stu-id="43edd-103">Azure CLI for Azure IoT</span></span>

<span data-ttu-id="43edd-104">A [CLI do Azure](/cli/azure/what-is-azure-cli) (Interface de Linha de Comando do Azure) é um conjunto de comandos usados para criar e gerenciar recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="43edd-104">The Azure Command Line Interface ([Azure CLI](/cli/azure/what-is-azure-cli)) is a set of commands used to create and manage Azure resources.</span></span>  <span data-ttu-id="43edd-105">Ela está disponível em muitos serviços do Azure, incluindo o Azure IoT.</span><span class="sxs-lookup"><span data-stu-id="43edd-105">It is available across many Azure services including Azure IoT.</span></span>  <span data-ttu-id="43edd-106">Há mais de 100 referências do Azure IoT, que possibilitam que você trabalhe de maneira eficaz com os serviços de IoT usando uma linha de comando.</span><span class="sxs-lookup"><span data-stu-id="43edd-106">There are over 100 references for Azure IoT giving you the ability to work effectively with IoT services from a command line.</span></span>

## <a name="references-for-iot"></a><span data-ttu-id="43edd-107">Referências de IoT</span><span class="sxs-lookup"><span data-stu-id="43edd-107">References for IoT</span></span>

<span data-ttu-id="43edd-108">A experiência da CLI do Azure IoT é composta por duas partes: A CLI do Azure (também chamada de CLI **principal**) e a **extensão** da CLI do Azure IoT.</span><span class="sxs-lookup"><span data-stu-id="43edd-108">The Azure IoT CLI experience is composed of two parts: Azure CLI (commonly referred to as CLI **core**) and the Azure IoT CLI **extension**.</span></span>

<span data-ttu-id="43edd-109">A funcionalidade de IoT na CLI do Azure **principal** tem como foco o gerenciamento e a configuração da infraestrutura.</span><span class="sxs-lookup"><span data-stu-id="43edd-109">IoT functionality in Azure CLI **core** is focused on infrastructure management and configuration.</span></span> <span data-ttu-id="43edd-110">Operações de CRUD do Hub IoT, ou a configuração de rotas de mensagens do Hub IoT, são casos de uso típicos dos comandos principais.</span><span class="sxs-lookup"><span data-stu-id="43edd-110">IoT Hub CRUD operations, or configuring IoT Hub message routes are typical use cases for core commands.</span></span>

<span data-ttu-id="43edd-111">A extensão de **IoT** traz recursos e funcionalidades avançadas para gerenciar, manipular e interagir com os dados, entidades e objetos na própria infraestrutura.</span><span class="sxs-lookup"><span data-stu-id="43edd-111">The IoT **extension** introduces rich features and functionality to manage, manipulate and interact with the data, entities and objects on the infrastructure itself.</span></span> <span data-ttu-id="43edd-112">Por exemplo, o gerenciamento de frotas de dispositivos, o monitoramento de eventos de dispositivo para nuvem e a invocação de métodos da nuvem para o dispositivo são habilitados por meio da extensão de IoT.</span><span class="sxs-lookup"><span data-stu-id="43edd-112">For example managing fleets of devices, monitoring device-to-cloud events and invoking cloud to device methods are all enabled via the IoT extension.</span></span> <span data-ttu-id="43edd-113">A extensão do Azure IoT para a CLI do Azure desbloqueia o uso de tecnologias experimentais ou em pré-lançamento que contribuem para sua versatilidade em diversos cenários e casos de uso.</span><span class="sxs-lookup"><span data-stu-id="43edd-113">The Azure IoT extension for Azure CLI unlocks the use of experimental or pre-release technology contributing to its versatility in a variety of scenarios and use cases.</span></span>

### <a name="core-reference-commands"></a><span data-ttu-id="43edd-114">Comandos de referência principais</span><span class="sxs-lookup"><span data-stu-id="43edd-114">Core reference commands</span></span>

| <span data-ttu-id="43edd-115">Referência</span><span class="sxs-lookup"><span data-stu-id="43edd-115">Reference</span></span> | <span data-ttu-id="43edd-116">Tem uma extensão</span><span class="sxs-lookup"><span data-stu-id="43edd-116">Has extension</span></span> | <span data-ttu-id="43edd-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="43edd-117">Description</span></span>
|-|-|-|
| [<span data-ttu-id="43edd-118">az iot</span><span class="sxs-lookup"><span data-stu-id="43edd-118">az iot</span></span>](/cli/azure/iot) | <span data-ttu-id="43edd-119">sim</span><span class="sxs-lookup"><span data-stu-id="43edd-119">yes</span></span>  | <span data-ttu-id="43edd-120">Todos os comandos principais da CLI do Azure disponíveis para o Azure IoT.</span><span class="sxs-lookup"><span data-stu-id="43edd-120">All available Azure CLI core commands for Azure IoT.</span></span>
| [<span data-ttu-id="43edd-121">az iot central</span><span class="sxs-lookup"><span data-stu-id="43edd-121">az iot central</span></span>](/cli/azure/iot/central) | <span data-ttu-id="43edd-122">sim</span><span class="sxs-lookup"><span data-stu-id="43edd-122">yes</span></span> | <span data-ttu-id="43edd-123">Gerenciar ativos do IoT Central.</span><span class="sxs-lookup"><span data-stu-id="43edd-123">Manage IoT Central assets.</span></span>
| [<span data-ttu-id="43edd-124">az iot dps</span><span class="sxs-lookup"><span data-stu-id="43edd-124">az iot dps</span></span>](/en-us/cli/azure/iot/dps) | <span data-ttu-id="43edd-125">sim</span><span class="sxs-lookup"><span data-stu-id="43edd-125">yes</span></span> | <span data-ttu-id="43edd-126">Gerenciar o Serviço de Provisionamento de Dispositivos no Hub IoT do Azure.</span><span class="sxs-lookup"><span data-stu-id="43edd-126">Manage Azure IoT Hub Device Provisioning Service.</span></span>
| [<span data-ttu-id="43edd-127">az iot hub</span><span class="sxs-lookup"><span data-stu-id="43edd-127">az iot hub</span></span>](/cli/azure/iot/hub) | <span data-ttu-id="43edd-128">sim</span><span class="sxs-lookup"><span data-stu-id="43edd-128">yes</span></span> | <span data-ttu-id="43edd-129">Gerenciar a infraestrutura do Hub IoT do Azure.</span><span class="sxs-lookup"><span data-stu-id="43edd-129">Manage Azure IoT Hub infrastructure.</span></span>

### <a name="extension-reference-commands"></a><span data-ttu-id="43edd-130">Comandos de referência de extensão</span><span class="sxs-lookup"><span data-stu-id="43edd-130">Extension reference commands</span></span>

| <span data-ttu-id="43edd-131">Referência</span><span class="sxs-lookup"><span data-stu-id="43edd-131">Reference</span></span> | <span data-ttu-id="43edd-132">Tem um comando principal</span><span class="sxs-lookup"><span data-stu-id="43edd-132">Has core</span></span> | <span data-ttu-id="43edd-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="43edd-133">Description</span></span>
|-|-|-|
| [<span data-ttu-id="43edd-134">az iot</span><span class="sxs-lookup"><span data-stu-id="43edd-134">az iot</span></span>](/cli/azure/ext/azure-iot/iot) | <span data-ttu-id="43edd-135">sim</span><span class="sxs-lookup"><span data-stu-id="43edd-135">yes</span></span> | <span data-ttu-id="43edd-136">Todos os comandos de extensão da CLI do Azure disponíveis para o Azure IoT.</span><span class="sxs-lookup"><span data-stu-id="43edd-136">All available Azure CLI extension commands for Azure IoT.</span></span>
| [<span data-ttu-id="43edd-137">az iot central</span><span class="sxs-lookup"><span data-stu-id="43edd-137">az iot central</span></span>](/cli/azure/ext/azure-iot/iot/central) | <span data-ttu-id="43edd-138">sim</span><span class="sxs-lookup"><span data-stu-id="43edd-138">yes</span></span> | <span data-ttu-id="43edd-139">Gerenciar soluções e a infraestrutura do Azure Central (IoT Central).</span><span class="sxs-lookup"><span data-stu-id="43edd-139">Manage Azure Central (IoT Central) solutions & infrastructure.</span></span>
| [<span data-ttu-id="43edd-140">az iot device</span><span class="sxs-lookup"><span data-stu-id="43edd-140">az iot device</span></span>](/cli/azure/ext/azure-iot/iot/device) | | <span data-ttu-id="43edd-141">Utilizar os recursos de mensagens de dispositivo para nuvem e nuvem para dispositivo.</span><span class="sxs-lookup"><span data-stu-id="43edd-141">Leverage device-to-cloud and cloud-to-device messaging capabilities.</span></span>
| [<span data-ttu-id="43edd-142">az dt</span><span class="sxs-lookup"><span data-stu-id="43edd-142">az dt</span></span>](/cli/azure/ext/azure-iot/dt) | | <span data-ttu-id="43edd-143">Gerenciar soluções e a infraestrutura dos Gêmeos Digitais do Azure.</span><span class="sxs-lookup"><span data-stu-id="43edd-143">Manage Azure Digital Twins solutions & infrastructure.</span></span>
| [<span data-ttu-id="43edd-144">az iot dps</span><span class="sxs-lookup"><span data-stu-id="43edd-144">az iot dps</span></span>](/cli/azure/ext/azure-iot/iot/dps) | <span data-ttu-id="43edd-145">sim</span><span class="sxs-lookup"><span data-stu-id="43edd-145">yes</span></span> | <span data-ttu-id="43edd-146">Gerenciar entidades em um Serviço de Provisionamento de Dispositivos no Hub IoT do Azure.</span><span class="sxs-lookup"><span data-stu-id="43edd-146">Manage entities in an Azure IoT Hub Device Provisioning Service.</span></span>
| [<span data-ttu-id="43edd-147">az iot edge</span><span class="sxs-lookup"><span data-stu-id="43edd-147">az iot edge</span></span>](/cli/azure/ext/azure-iot/iot/edge) | | <span data-ttu-id="43edd-148">Gerenciar soluções de IoT no Edge.</span><span class="sxs-lookup"><span data-stu-id="43edd-148">Manage IoT solutions on the Edge.</span></span>
| [<span data-ttu-id="43edd-149">az iot hub</span><span class="sxs-lookup"><span data-stu-id="43edd-149">az iot hub</span></span>](/cli/azure/ext/azure-iot/iot/hub) | <span data-ttu-id="43edd-150">sim</span><span class="sxs-lookup"><span data-stu-id="43edd-150">yes</span></span> | <span data-ttu-id="43edd-151">Gerenciar entidades em um Hub IoT do Azure.</span><span class="sxs-lookup"><span data-stu-id="43edd-151">Manage entities in an Azure IoT Hub.</span></span>
| [<span data-ttu-id="43edd-152">az iot pnp</span><span class="sxs-lookup"><span data-stu-id="43edd-152">az iot pnp</span></span>](/cli/azure/ext/azure-iot/iot/pnp) | | <span data-ttu-id="43edd-153">Gerenciar entidades de um repositório de modelos de IoT Plug and Play.</span><span class="sxs-lookup"><span data-stu-id="43edd-153">Manage entities of an IoT Plug and Play model repository.</span></span>

### <a name="additional-cli-commands-for-azure-services-used-by-iot"></a><span data-ttu-id="43edd-154">Comandos adicionais da CLI para serviços do Azure usados pela IoT</span><span class="sxs-lookup"><span data-stu-id="43edd-154">Additional CLI commands for Azure services used by IoT</span></span>

| <span data-ttu-id="43edd-155">Referência</span><span class="sxs-lookup"><span data-stu-id="43edd-155">Reference</span></span> | <span data-ttu-id="43edd-156">Type</span><span class="sxs-lookup"><span data-stu-id="43edd-156">Type</span></span> | <span data-ttu-id="43edd-157">Descrição</span><span class="sxs-lookup"><span data-stu-id="43edd-157">Description</span></span>
|-|-|-|
| [<span data-ttu-id="43edd-158">az maps</span><span class="sxs-lookup"><span data-stu-id="43edd-158">az maps</span></span>](/cli/azure/maps) | <span data-ttu-id="43edd-159">core</span><span class="sxs-lookup"><span data-stu-id="43edd-159">core</span></span> | <span data-ttu-id="43edd-160">Gerenciar o Azure Mapas.</span><span class="sxs-lookup"><span data-stu-id="43edd-160">Manage Azure Maps.</span></span>
| [<span data-ttu-id="43edd-161">az timeseriesinsights</span><span class="sxs-lookup"><span data-stu-id="43edd-161">az timeseriesinsights</span></span>](/cli/azure/ext/timeseriesinsights/timeseriesinsights) | <span data-ttu-id="43edd-162">extensão</span><span class="sxs-lookup"><span data-stu-id="43edd-162">extension</span></span> | <span data-ttu-id="43edd-163">Gerenciar o Azure Time Series Insights.</span><span class="sxs-lookup"><span data-stu-id="43edd-163">Manage Azure Time Series Insights.</span></span>

### <a name="extension-reference-installation"></a><span data-ttu-id="43edd-164">Instalação de referência de extensão</span><span class="sxs-lookup"><span data-stu-id="43edd-164">Extension reference installation</span></span>

<span data-ttu-id="43edd-165">As referências de extensão da CLI do Azure devem ser instaladas antes do uso.</span><span class="sxs-lookup"><span data-stu-id="43edd-165">Azure CLI extension references must be installed prior to use.</span></span>  <span data-ttu-id="43edd-166">Use o comando [az extension add](/cli/azure/azure-cli-extensions-overview) para instalar uma referência de extensão por nome.</span><span class="sxs-lookup"><span data-stu-id="43edd-166">Use the [az extension add](/cli/azure/azure-cli-extensions-overview) command to install an extension reference by name.</span></span>  <span data-ttu-id="43edd-167">Saiba mais sobre as referências de extensão em [Usar extensões com a CLI do Azure](/cli/azure/azure-cli-extensions-overview).</span><span class="sxs-lookup"><span data-stu-id="43edd-167">Find out more about extension references in [Use extensions with Azure CLI](/cli/azure/azure-cli-extensions-overview).</span></span>

```azurecli
# install the Azure CLI extension reference for Azure IoT
az extension add --name azure-iot
```

## <a name="popular-iot-articles-using-the-azure-cli"></a><span data-ttu-id="43edd-168">Artigos populares sobre IoT em que a CLI do Azure é usada</span><span class="sxs-lookup"><span data-stu-id="43edd-168">Popular IoT articles using the Azure CLI</span></span>

- [<span data-ttu-id="43edd-169">Criar um hub IoT</span><span class="sxs-lookup"><span data-stu-id="43edd-169">Create an IoT hub</span></span>](/azure/iot-hub/iot-hub-create-using-cli)
- [<span data-ttu-id="43edd-170">Gerenciar o IoT Central</span><span class="sxs-lookup"><span data-stu-id="43edd-170">Manage IoT Central</span></span>](/azure/iot-central/core/howto-manage-iot-central-from-cli)
- [<span data-ttu-id="43edd-171">Tutoriais de dispositivos controlados pela CLI usando o Azure RTOS</span><span class="sxs-lookup"><span data-stu-id="43edd-171">CLI driven device tutorials using Azure RTOS</span></span>](/azure/rtos/getting-started?branch=master)
- [<span data-ttu-id="43edd-172">Usar a extensão de IoT para gerenciamento de dispositivo do Hub IoT do Azure</span><span class="sxs-lookup"><span data-stu-id="43edd-172">Use the IoT extension for Azure IoT Hub device management</span></span>](/azure/iot-hub/iot-hub-device-management-iot-extension-azure-cli-2-0)
- [<span data-ttu-id="43edd-173">Implantar e monitorar módulos do IoT Edge em escala usando a extensão da CLI do Azure para IoT</span><span class="sxs-lookup"><span data-stu-id="43edd-173">Deploy and monitor IoT Edge modules at scale with the Azure CLI extension for IoT</span></span>](/azure/iot-edge/how-to-deploy-cli-at-scale)
- [<span data-ttu-id="43edd-174">Enviar telemetria para um dispositivo e monitorá-lo com a extensão da CLI do Azure para IoT</span><span class="sxs-lookup"><span data-stu-id="43edd-174">Send Telemetry to a device and monitor it with the Azure CLI extension for IoT</span></span>](/azure/iot-hub/quickstart-send-telemetry-cli)
- [<span data-ttu-id="43edd-175">Usar a CLI do Azure para configurar o roteamento de mensagens do Hub IoT</span><span class="sxs-lookup"><span data-stu-id="43edd-175">Use the Azure CLI to configure IoT Hub message routing</span></span>](/azure/iot-hub/tutorial-routing-config-message-routing-cli)
- [<span data-ttu-id="43edd-176">Gerenciar interfaces em um repositório de modelos Plug and Play</span><span class="sxs-lookup"><span data-stu-id="43edd-176">Manage interfaces in a Plug and Play model repository</span></span>](/azure/iot-pnp/howto-install-pnp-cli#manage-interfaces-in-a-model-repository)

## <a name="azure-cli-reference-examples"></a><span data-ttu-id="43edd-177">Exemplos de referência da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="43edd-177">Azure CLI reference examples</span></span>

<span data-ttu-id="43edd-178">São fornecidos exemplos com todas as referências da CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="43edd-178">Examples are provided with every Azure CLI reference.</span></span> <span data-ttu-id="43edd-179">Embora você também possa concluir essas tarefas no portal do Azure, usar a CLI do Azure requer uma só linha de comando.</span><span class="sxs-lookup"><span data-stu-id="43edd-179">Although you can also complete these tasks through the Azure portal, using the Azure CLI requires a single command line.</span></span>  <span data-ttu-id="43edd-180">Veja alguns blocos de código para ter uma ideia de como é fácil usar a CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="43edd-180">Here are a few code blocks to give you an idea of how easy it is to use the Azure CLI.</span></span>

<span data-ttu-id="43edd-181">Para trabalhar com o Azure IoT, primeiro você precisará de um grupo de recursos.</span><span class="sxs-lookup"><span data-stu-id="43edd-181">To work with Azure IoT, you'll first need a resource group.</span></span>  <span data-ttu-id="43edd-182">Os grupos de recursos do Azure são simples de criar e gerenciar com a CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="43edd-182">Azure resource groups are simple to create and manage with the Azure CLI.</span></span>  

```azurecli
#create a resource group
az group create -location westus -name MyResourceGroup
```

```azurecli
#get a list of resource groups for a subscription
az group list --subscription MySubscription --output table
```

<span data-ttu-id="43edd-183">É tão simples quanto criar um Hub IoT do Azure na região '''westus''' com o tipo de preço Standard.</span><span class="sxs-lookup"><span data-stu-id="43edd-183">It is as straightforward to create an Azure IoT Hub in the '''westus''' region in the standard pricing tier.</span></span>

```azurecli
#create an Azure IoT hub
az iot hub create --resource-group MyResourceGroup --name MyIotHub --location westus
```

## <a name="see-also"></a><span data-ttu-id="43edd-184">Confira também</span><span class="sxs-lookup"><span data-stu-id="43edd-184">See also</span></span>

- <span data-ttu-id="43edd-185">[Introdução à CLI do Azure](/cli/azure/get-started-with-azure-cli) para saber mais sobre a instalação e a conexão.</span><span class="sxs-lookup"><span data-stu-id="43edd-185">[Get started with Azure CLI](/cli/azure/get-started-with-azure-cli) to learn about installation and sign in.</span></span>

- <span data-ttu-id="43edd-186">Descubra referências adicionais [lançadas](/cli/azure/reference-index) e de [extensão](/cli/azure/azure-cli-extensions-list) na documentação da CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="43edd-186">Discover additional [released](/cli/azure/reference-index) and [extension](/cli/azure/azure-cli-extensions-list) references in the Azure CLI documentation.</span></span>
