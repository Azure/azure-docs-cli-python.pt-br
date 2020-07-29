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
ms.openlocfilehash: aa4653ceaba41709cd54a098f649a9c922e93fa8
ms.sourcegitcommit: 05ef6cb6cf049d8c8eb54dd408f56cb145fb5905
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/29/2020
ms.locfileid: "87374381"
---
# <a name="azure-cli-for-azure-iot"></a><span data-ttu-id="0ca77-103">CLI do Azure para o Azure IoT</span><span class="sxs-lookup"><span data-stu-id="0ca77-103">Azure CLI for Azure IoT</span></span>

<span data-ttu-id="0ca77-104">A [CLI do Azure](/cli/azure/what-is-azure-cli) (Interface de Linha de Comando do Azure) é um conjunto de comandos usados para criar e gerenciar recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="0ca77-104">The Azure Command Line Interface ([Azure CLI](/cli/azure/what-is-azure-cli)) is a set of commands used to create and manage Azure resources.</span></span>  <span data-ttu-id="0ca77-105">Ela está disponível em muitos serviços do Azure, incluindo o Azure IoT.</span><span class="sxs-lookup"><span data-stu-id="0ca77-105">It is available across many Azure services including Azure IoT.</span></span>  <span data-ttu-id="0ca77-106">Há mais de 100 referências do Azure IoT, que possibilitam que você trabalhe de maneira eficaz com os serviços de IoT usando uma linha de comando.</span><span class="sxs-lookup"><span data-stu-id="0ca77-106">There are over 100 references for Azure IoT giving you the ability to work effectively with IoT services from a command line.</span></span>

## <a name="references-for-iot"></a><span data-ttu-id="0ca77-107">Referências de IoT</span><span class="sxs-lookup"><span data-stu-id="0ca77-107">References for IoT</span></span>

<span data-ttu-id="0ca77-108">A experiência da CLI do Azure IoT é composta por duas partes: A CLI do Azure (também chamada de CLI **principal**) e a **extensão** da CLI do Azure IoT.</span><span class="sxs-lookup"><span data-stu-id="0ca77-108">The Azure IoT CLI experience is composed of two parts: Azure CLI (commonly referred to as CLI **core**) and the Azure IoT CLI **extension**.</span></span>

<span data-ttu-id="0ca77-109">A funcionalidade de IoT na CLI do Azure **principal** tem como foco o gerenciamento e a configuração da infraestrutura.</span><span class="sxs-lookup"><span data-stu-id="0ca77-109">IoT functionality in Azure CLI **core** is focused on infrastructure management and configuration.</span></span> <span data-ttu-id="0ca77-110">Operações de CRUD do Hub IoT, ou a configuração de rotas de mensagens do Hub IoT, são casos de uso típicos dos comandos principais.</span><span class="sxs-lookup"><span data-stu-id="0ca77-110">IoT Hub CRUD operations, or configuring IoT Hub message routes are typical use cases for core commands.</span></span>

<span data-ttu-id="0ca77-111">A extensão de **IoT** traz recursos e funcionalidades avançadas para gerenciar, manipular e interagir com os dados, entidades e objetos na própria infraestrutura.</span><span class="sxs-lookup"><span data-stu-id="0ca77-111">The IoT **extension** introduces rich features and functionality to manage, manipulate and interact with the data, entities and objects on the infrastructure itself.</span></span> <span data-ttu-id="0ca77-112">Por exemplo, o gerenciamento de frotas de dispositivos, o monitoramento de eventos de dispositivo para nuvem e a invocação de métodos da nuvem para o dispositivo são habilitados por meio da extensão de IoT.</span><span class="sxs-lookup"><span data-stu-id="0ca77-112">For example managing fleets of devices, monitoring device-to-cloud events and invoking cloud to device methods are all enabled via the IoT extension.</span></span> <span data-ttu-id="0ca77-113">A extensão do Azure IoT para a CLI do Azure desbloqueia o uso de tecnologias experimentais ou em pré-lançamento que contribuem para sua versatilidade em diversos cenários e casos de uso.</span><span class="sxs-lookup"><span data-stu-id="0ca77-113">The Azure IoT extension for Azure CLI unlocks the use of experimental or pre-release technology contributing to its versatility in a variety of scenarios and use cases.</span></span>

### <a name="core-reference-commands"></a><span data-ttu-id="0ca77-114">Comandos de referência principais</span><span class="sxs-lookup"><span data-stu-id="0ca77-114">Core reference commands</span></span>

| <span data-ttu-id="0ca77-115">Referência</span><span class="sxs-lookup"><span data-stu-id="0ca77-115">Reference</span></span> | <span data-ttu-id="0ca77-116">Tem uma extensão</span><span class="sxs-lookup"><span data-stu-id="0ca77-116">Has extension</span></span> | <span data-ttu-id="0ca77-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ca77-117">Description</span></span>
|-|-|-|
| [<span data-ttu-id="0ca77-118">az iot</span><span class="sxs-lookup"><span data-stu-id="0ca77-118">az iot</span></span>](/cli/azure/iot) | <span data-ttu-id="0ca77-119">sim</span><span class="sxs-lookup"><span data-stu-id="0ca77-119">yes</span></span>  | <span data-ttu-id="0ca77-120">Todos os comandos principais da CLI do Azure disponíveis para o Azure IoT.</span><span class="sxs-lookup"><span data-stu-id="0ca77-120">All available Azure CLI core commands for Azure IoT.</span></span>
| [<span data-ttu-id="0ca77-121">az iot central</span><span class="sxs-lookup"><span data-stu-id="0ca77-121">az iot central</span></span>](/cli/azure/iot/central) | <span data-ttu-id="0ca77-122">sim</span><span class="sxs-lookup"><span data-stu-id="0ca77-122">yes</span></span> | <span data-ttu-id="0ca77-123">Gerenciar ativos do IoT Central.</span><span class="sxs-lookup"><span data-stu-id="0ca77-123">Manage IoT Central assets.</span></span>
| [<span data-ttu-id="0ca77-124">az iot dps</span><span class="sxs-lookup"><span data-stu-id="0ca77-124">az iot dps</span></span>](/en-us/cli/azure/iot/dps) | <span data-ttu-id="0ca77-125">sim</span><span class="sxs-lookup"><span data-stu-id="0ca77-125">yes</span></span> | <span data-ttu-id="0ca77-126">Gerenciar o Serviço de Provisionamento de Dispositivos no Hub IoT do Azure.</span><span class="sxs-lookup"><span data-stu-id="0ca77-126">Manage Azure IoT Hub Device Provisioning Service.</span></span>
| [<span data-ttu-id="0ca77-127">az iot hub</span><span class="sxs-lookup"><span data-stu-id="0ca77-127">az iot hub</span></span>](/cli/azure/iot/hub) | <span data-ttu-id="0ca77-128">sim</span><span class="sxs-lookup"><span data-stu-id="0ca77-128">yes</span></span> | <span data-ttu-id="0ca77-129">Gerenciar a infraestrutura do Hub IoT do Azure.</span><span class="sxs-lookup"><span data-stu-id="0ca77-129">Manage Azure IoT Hub infrastructure.</span></span>

### <a name="extension-reference-commands"></a><span data-ttu-id="0ca77-130">Comandos de referência de extensão</span><span class="sxs-lookup"><span data-stu-id="0ca77-130">Extension reference commands</span></span>

| <span data-ttu-id="0ca77-131">Referência</span><span class="sxs-lookup"><span data-stu-id="0ca77-131">Reference</span></span> | <span data-ttu-id="0ca77-132">Tem um comando principal</span><span class="sxs-lookup"><span data-stu-id="0ca77-132">Has core</span></span> | <span data-ttu-id="0ca77-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ca77-133">Description</span></span>
|-|-|-|
| [<span data-ttu-id="0ca77-134">az iot</span><span class="sxs-lookup"><span data-stu-id="0ca77-134">az iot</span></span>](/cli/azure/ext/azure-iot/iot) | <span data-ttu-id="0ca77-135">sim</span><span class="sxs-lookup"><span data-stu-id="0ca77-135">yes</span></span> | <span data-ttu-id="0ca77-136">Todos os comandos de extensão da CLI do Azure disponíveis para o Azure IoT.</span><span class="sxs-lookup"><span data-stu-id="0ca77-136">All available Azure CLI extension commands for Azure IoT.</span></span>
| [<span data-ttu-id="0ca77-137">az iot central</span><span class="sxs-lookup"><span data-stu-id="0ca77-137">az iot central</span></span>](/cli/azure/ext/azure-iot/iot/central) | <span data-ttu-id="0ca77-138">sim</span><span class="sxs-lookup"><span data-stu-id="0ca77-138">yes</span></span> | <span data-ttu-id="0ca77-139">Gerenciar soluções e a infraestrutura do Azure Central (IoT Central).</span><span class="sxs-lookup"><span data-stu-id="0ca77-139">Manage Azure Central (IoT Central) solutions & infrastructure.</span></span>
| [<span data-ttu-id="0ca77-140">az iot device</span><span class="sxs-lookup"><span data-stu-id="0ca77-140">az iot device</span></span>](/cli/azure/ext/azure-iot/iot/device) | | <span data-ttu-id="0ca77-141">Utilizar os recursos de mensagens de dispositivo para nuvem e nuvem para dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0ca77-141">Leverage device-to-cloud and cloud-to-device messaging capabilities.</span></span>
| [<span data-ttu-id="0ca77-142">az dt</span><span class="sxs-lookup"><span data-stu-id="0ca77-142">az dt</span></span>](/cli/azure/ext/azure-iot/dt) | | <span data-ttu-id="0ca77-143">Gerenciar soluções e a infraestrutura dos Gêmeos Digitais do Azure.</span><span class="sxs-lookup"><span data-stu-id="0ca77-143">Manage Azure Digital Twins solutions & infrastructure.</span></span>
| [<span data-ttu-id="0ca77-144">az iot dps</span><span class="sxs-lookup"><span data-stu-id="0ca77-144">az iot dps</span></span>](/cli/azure/ext/azure-iot/iot/dps) | <span data-ttu-id="0ca77-145">sim</span><span class="sxs-lookup"><span data-stu-id="0ca77-145">yes</span></span> | <span data-ttu-id="0ca77-146">Gerenciar entidades em um Serviço de Provisionamento de Dispositivos no Hub IoT do Azure.</span><span class="sxs-lookup"><span data-stu-id="0ca77-146">Manage entities in an Azure IoT Hub Device Provisioning Service.</span></span>
| [<span data-ttu-id="0ca77-147">az iot edge</span><span class="sxs-lookup"><span data-stu-id="0ca77-147">az iot edge</span></span>](/cli/azure/ext/azure-iot/iot/edge) | | <span data-ttu-id="0ca77-148">Gerenciar soluções de IoT no Edge.</span><span class="sxs-lookup"><span data-stu-id="0ca77-148">Manage IoT solutions on the Edge.</span></span>
| [<span data-ttu-id="0ca77-149">az iot hub</span><span class="sxs-lookup"><span data-stu-id="0ca77-149">az iot hub</span></span>](/cli/azure/ext/azure-iot/iot/hub) | <span data-ttu-id="0ca77-150">sim</span><span class="sxs-lookup"><span data-stu-id="0ca77-150">yes</span></span> | <span data-ttu-id="0ca77-151">Gerenciar entidades em um Hub IoT do Azure.</span><span class="sxs-lookup"><span data-stu-id="0ca77-151">Manage entities in an Azure IoT Hub.</span></span>
| [<span data-ttu-id="0ca77-152">az iot pnp</span><span class="sxs-lookup"><span data-stu-id="0ca77-152">az iot pnp</span></span>](/cli/azure/ext/azure-iot/iot/pnp) | <span data-ttu-id="0ca77-153">sim</span><span class="sxs-lookup"><span data-stu-id="0ca77-153">yes</span></span> | <span data-ttu-id="0ca77-154">Gerenciar entidades de um repositório de modelos de IoT Plug and Play.</span><span class="sxs-lookup"><span data-stu-id="0ca77-154">Manage entities of an IoT Plug and Play model repository.</span></span>

### <a name="additional-cli-commands-for-azure-services-used-by-iot"></a><span data-ttu-id="0ca77-155">Comandos adicionais da CLI para serviços do Azure usados pela IoT</span><span class="sxs-lookup"><span data-stu-id="0ca77-155">Additional CLI commands for Azure services used by IoT</span></span>

| <span data-ttu-id="0ca77-156">Referência</span><span class="sxs-lookup"><span data-stu-id="0ca77-156">Reference</span></span> | <span data-ttu-id="0ca77-157">Type</span><span class="sxs-lookup"><span data-stu-id="0ca77-157">Type</span></span> | <span data-ttu-id="0ca77-158">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ca77-158">Description</span></span>
|-|-|-|
| [<span data-ttu-id="0ca77-159">az maps</span><span class="sxs-lookup"><span data-stu-id="0ca77-159">az maps</span></span>](/cli/azure/maps) | <span data-ttu-id="0ca77-160">core</span><span class="sxs-lookup"><span data-stu-id="0ca77-160">core</span></span> | <span data-ttu-id="0ca77-161">Gerenciar o Azure Mapas.</span><span class="sxs-lookup"><span data-stu-id="0ca77-161">Manage Azure Maps.</span></span>
| [<span data-ttu-id="0ca77-162">az timeseriesinsights</span><span class="sxs-lookup"><span data-stu-id="0ca77-162">az timeseriesinsights</span></span>](/cli/azure/ext/timeseriesinsights/timeseriesinsights) | <span data-ttu-id="0ca77-163">extensão</span><span class="sxs-lookup"><span data-stu-id="0ca77-163">extension</span></span> | <span data-ttu-id="0ca77-164">Gerenciar o Azure Time Series Insights.</span><span class="sxs-lookup"><span data-stu-id="0ca77-164">Manage Azure Time Series Insights.</span></span>

### <a name="extension-reference-installation"></a><span data-ttu-id="0ca77-165">Instalação de referência de extensão</span><span class="sxs-lookup"><span data-stu-id="0ca77-165">Extension reference installation</span></span>

<span data-ttu-id="0ca77-166">As referências de extensão da CLI do Azure devem ser instaladas antes do uso.</span><span class="sxs-lookup"><span data-stu-id="0ca77-166">Azure CLI extension references must be installed prior to use.</span></span>  <span data-ttu-id="0ca77-167">Use o comando [az extension add](/cli/azure/azure-cli-extensions-overview) para instalar uma referência de extensão por nome.</span><span class="sxs-lookup"><span data-stu-id="0ca77-167">Use the [az extension add](/cli/azure/azure-cli-extensions-overview) command to install an extension reference by name.</span></span>  <span data-ttu-id="0ca77-168">Saiba mais sobre as referências de extensão em [Usar extensões com a CLI do Azure](/cli/azure/azure-cli-extensions-overview).</span><span class="sxs-lookup"><span data-stu-id="0ca77-168">Find out more about extension references in [Use extensions with Azure CLI](/cli/azure/azure-cli-extensions-overview).</span></span>

```azurecli
# install the Azure CLI extension reference for Azure IoT
az extension add --name azure-iot
```

## <a name="popular-iot-articles-using-the-azure-cli"></a><span data-ttu-id="0ca77-169">Artigos populares sobre IoT em que a CLI do Azure é usada</span><span class="sxs-lookup"><span data-stu-id="0ca77-169">Popular IoT articles using the Azure CLI</span></span>

- [<span data-ttu-id="0ca77-170">Criar um hub IoT</span><span class="sxs-lookup"><span data-stu-id="0ca77-170">Create an IoT hub</span></span>](/azure/iot-hub/iot-hub-create-using-cli)
- [<span data-ttu-id="0ca77-171">Gerenciar o IoT Central</span><span class="sxs-lookup"><span data-stu-id="0ca77-171">Manage IoT Central</span></span>](/azure/iot-central/core/howto-manage-iot-central-from-cli)
- [<span data-ttu-id="0ca77-172">Tutoriais de dispositivos controlados pela CLI usando o Azure RTOS</span><span class="sxs-lookup"><span data-stu-id="0ca77-172">CLI driven device tutorials using Azure RTOS</span></span>](/azure/rtos/getting-started?branch=master)
- [<span data-ttu-id="0ca77-173">Usar a extensão de IoT para gerenciamento de dispositivo do Hub IoT do Azure</span><span class="sxs-lookup"><span data-stu-id="0ca77-173">Use the IoT extension for Azure IoT Hub device management</span></span>](/azure/iot-hub/iot-hub-device-management-iot-extension-azure-cli-2-0)
- [<span data-ttu-id="0ca77-174">Implantar e monitorar módulos do IoT Edge em escala usando a extensão da CLI do Azure para IoT</span><span class="sxs-lookup"><span data-stu-id="0ca77-174">Deploy and monitor IoT Edge modules at scale with the Azure CLI extension for IoT</span></span>](/azure/iot-edge/how-to-deploy-cli-at-scale)
- [<span data-ttu-id="0ca77-175">Enviar telemetria para um dispositivo e monitorá-lo com a extensão da CLI do Azure para IoT</span><span class="sxs-lookup"><span data-stu-id="0ca77-175">Send Telemetry to a device and monitor it with the Azure CLI extension for IoT</span></span>](/azure/iot-hub/quickstart-send-telemetry-cli)
- [<span data-ttu-id="0ca77-176">Usar a CLI do Azure para configurar o roteamento de mensagens do Hub IoT</span><span class="sxs-lookup"><span data-stu-id="0ca77-176">Use the Azure CLI to configure IoT Hub message routing</span></span>](/azure/iot-hub/tutorial-routing-config-message-routing-cli)
- [<span data-ttu-id="0ca77-177">Gerenciar interfaces em um repositório de modelos Plug and Play</span><span class="sxs-lookup"><span data-stu-id="0ca77-177">Manage interfaces in a Plug and Play model repository</span></span>](/azure/iot-pnp/howto-install-pnp-cli#manage-interfaces-in-a-model-repository)

## <a name="azure-cli-reference-examples"></a><span data-ttu-id="0ca77-178">Exemplos de referência da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="0ca77-178">Azure CLI reference examples</span></span>

<span data-ttu-id="0ca77-179">São fornecidos exemplos com todas as referências da CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="0ca77-179">Examples are provided with every Azure CLI reference.</span></span> <span data-ttu-id="0ca77-180">Embora você também possa concluir essas tarefas no portal do Azure, usar a CLI do Azure requer uma só linha de comando.</span><span class="sxs-lookup"><span data-stu-id="0ca77-180">Although you can also complete these tasks through the Azure portal, using the Azure CLI requires a single command line.</span></span>  <span data-ttu-id="0ca77-181">Veja alguns blocos de código para ter uma ideia de como é fácil usar a CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="0ca77-181">Here are a few code blocks to give you an idea of how easy it is to use the Azure CLI.</span></span>

<span data-ttu-id="0ca77-182">Para trabalhar com o Azure IoT, primeiro você precisará de um grupo de recursos.</span><span class="sxs-lookup"><span data-stu-id="0ca77-182">To work with Azure IoT, you'll first need a resource group.</span></span>  <span data-ttu-id="0ca77-183">Os grupos de recursos do Azure são simples de criar e gerenciar com a CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="0ca77-183">Azure resource groups are simple to create and manage with the Azure CLI.</span></span>  

```azurecli
#create a resource group
az group create -location westus -name MyResourceGroup
```

```azurecli
#get a list of resource groups for a subscription
az group list --subscription MySubscription --output table
```

<span data-ttu-id="0ca77-184">É tão simples quanto criar um Hub IoT do Azure na região '''westus''' com o tipo de preço Standard.</span><span class="sxs-lookup"><span data-stu-id="0ca77-184">It is as straightforward to create an Azure IoT Hub in the '''westus''' region in the standard pricing tier.</span></span>

```azurecli
#create an Azure IoT hub
az iot hub create --resource-group MyResourceGroup --name MyIotHub --location westus
```

## <a name="see-also"></a><span data-ttu-id="0ca77-185">Confira também</span><span class="sxs-lookup"><span data-stu-id="0ca77-185">See also</span></span>

- <span data-ttu-id="0ca77-186">[Introdução à CLI do Azure](/cli/azure/get-started-with-azure-cli) para saber mais sobre a instalação e a conexão.</span><span class="sxs-lookup"><span data-stu-id="0ca77-186">[Get started with Azure CLI](/cli/azure/get-started-with-azure-cli) to learn about installation and sign in.</span></span>

- <span data-ttu-id="0ca77-187">Descubra referências adicionais [lançadas](/cli/azure/reference-index) e de [extensão](/cli/azure/azure-cli-extensions-list) na documentação da CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="0ca77-187">Discover additional [released](/cli/azure/reference-index) and [extension](/cli/azure/azure-cli-extensions-list) references in the Azure CLI documentation.</span></span>
