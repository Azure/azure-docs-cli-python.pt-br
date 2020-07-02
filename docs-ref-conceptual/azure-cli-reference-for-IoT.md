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
ms.openlocfilehash: e3bf40eab68f09dfb94e14e59d8a746d87bb0766
ms.sourcegitcommit: 415c6ddcce1da133d96b8c700e6aa570e4746b3f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2020
ms.locfileid: "85765098"
---
# <a name="azure-cli-for-azure-iot"></a><span data-ttu-id="16d2a-103">CLI do Azure para o Azure IoT</span><span class="sxs-lookup"><span data-stu-id="16d2a-103">Azure CLI for Azure IoT</span></span>

<span data-ttu-id="16d2a-104">A [CLI do Azure](/cli/azure/what-is-azure-cli) (Interface de Linha de Comando do Azure) é um conjunto de comandos usados para criar e gerenciar recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="16d2a-104">The Azure Command Line Interface ([Azure CLI](/cli/azure/what-is-azure-cli)) is a set of commands used to create and manage Azure resources.</span></span>  <span data-ttu-id="16d2a-105">Ela está disponível em muitos serviços do Azure, incluindo o Azure IoT.</span><span class="sxs-lookup"><span data-stu-id="16d2a-105">It is available across many Azure services including Azure IoT.</span></span>  <span data-ttu-id="16d2a-106">Há mais de 100 referências do Azure IoT, que possibilitam que você trabalhe de maneira eficaz com os serviços de IoT usando uma linha de comando.</span><span class="sxs-lookup"><span data-stu-id="16d2a-106">There are over 100 references for Azure IoT giving you the ability to work effectively with IoT services from a command line.</span></span>

## <a name="references-for-iot"></a><span data-ttu-id="16d2a-107">Referências de IoT</span><span class="sxs-lookup"><span data-stu-id="16d2a-107">References for IoT</span></span>

<span data-ttu-id="16d2a-108">A experiência da CLI do Azure IoT é composta por duas partes: A CLI do Azure (também chamada de CLI **principal**) e a **extensão** da CLI do Azure IoT.</span><span class="sxs-lookup"><span data-stu-id="16d2a-108">The Azure IoT CLI experience is composed of two parts: Azure CLI (commonly referred to as CLI **core**) and the Azure IoT CLI **extension**.</span></span>

<span data-ttu-id="16d2a-109">A funcionalidade de IoT na CLI do Azure **principal** tem como foco o gerenciamento e a configuração da infraestrutura.</span><span class="sxs-lookup"><span data-stu-id="16d2a-109">IoT functionality in Azure CLI **core** is focused on infrastructure management and configuration.</span></span> <span data-ttu-id="16d2a-110">Operações de CRUD do Hub IoT, ou a configuração de rotas de mensagens do Hub IoT, são casos de uso típicos dos comandos principais.</span><span class="sxs-lookup"><span data-stu-id="16d2a-110">IoT Hub CRUD operations, or configuring IoT Hub message routes are typical use cases for core commands.</span></span>

<span data-ttu-id="16d2a-111">A extensão de **IoT** traz recursos e funcionalidades avançadas para gerenciar, manipular e interagir com os dados, entidades e objetos na própria infraestrutura.</span><span class="sxs-lookup"><span data-stu-id="16d2a-111">The IoT **extension** introduces rich features and functionality to manage, manipulate and interact with the data, entities and objects on the infrastructure itself.</span></span> <span data-ttu-id="16d2a-112">Por exemplo, o gerenciamento de frotas de dispositivos, o monitoramento de eventos de dispositivo para nuvem e a invocação de métodos da nuvem para o dispositivo são habilitados por meio da extensão de IoT.</span><span class="sxs-lookup"><span data-stu-id="16d2a-112">For example managing fleets of devices, monitoring device-to-cloud events and invoking cloud to device methods are all enabled via the IoT extension.</span></span> <span data-ttu-id="16d2a-113">A extensão do Azure IoT para a CLI do Azure desbloqueia o uso de tecnologias experimentais ou em pré-lançamento que contribuem para sua versatilidade em diversos cenários e casos de uso.</span><span class="sxs-lookup"><span data-stu-id="16d2a-113">The Azure IoT extension for Azure CLI unlocks the use of experimental or pre-release technology contributing to its versatility in a variety of scenarios and use cases.</span></span>

### <a name="core-reference-commands"></a><span data-ttu-id="16d2a-114">Comandos de referência principais</span><span class="sxs-lookup"><span data-stu-id="16d2a-114">Core reference commands</span></span>

| <span data-ttu-id="16d2a-115">Referência</span><span class="sxs-lookup"><span data-stu-id="16d2a-115">Reference</span></span> | <span data-ttu-id="16d2a-116">Tem uma extensão</span><span class="sxs-lookup"><span data-stu-id="16d2a-116">Has extension</span></span> | <span data-ttu-id="16d2a-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="16d2a-117">Description</span></span>
|-|-|-|
| [<span data-ttu-id="16d2a-118">az iot</span><span class="sxs-lookup"><span data-stu-id="16d2a-118">az iot</span></span>](/cli/azure/iot) | <span data-ttu-id="16d2a-119">sim</span><span class="sxs-lookup"><span data-stu-id="16d2a-119">yes</span></span>  | <span data-ttu-id="16d2a-120">Todos os comandos principais da CLI do Azure disponíveis para o Azure IoT.</span><span class="sxs-lookup"><span data-stu-id="16d2a-120">All available Azure CLI core commands for Azure IoT.</span></span>
| [<span data-ttu-id="16d2a-121">az iot central</span><span class="sxs-lookup"><span data-stu-id="16d2a-121">az iot central</span></span>](/cli/azure/iot/central) | <span data-ttu-id="16d2a-122">sim</span><span class="sxs-lookup"><span data-stu-id="16d2a-122">yes</span></span> | <span data-ttu-id="16d2a-123">Gerenciar ativos do IoT Central.</span><span class="sxs-lookup"><span data-stu-id="16d2a-123">Manage IoT Central assets.</span></span>
| [<span data-ttu-id="16d2a-124">az iot dps</span><span class="sxs-lookup"><span data-stu-id="16d2a-124">az iot dps</span></span>](/en-us/cli/azure/iot/dps) | <span data-ttu-id="16d2a-125">sim</span><span class="sxs-lookup"><span data-stu-id="16d2a-125">yes</span></span> | <span data-ttu-id="16d2a-126">Gerenciar o Serviço de Provisionamento de Dispositivos no Hub IoT do Azure.</span><span class="sxs-lookup"><span data-stu-id="16d2a-126">Manage Azure IoT Hub Device Provisioning Service.</span></span>
| [<span data-ttu-id="16d2a-127">az iot hub</span><span class="sxs-lookup"><span data-stu-id="16d2a-127">az iot hub</span></span>](/cli/azure/iot/hub) | <span data-ttu-id="16d2a-128">sim</span><span class="sxs-lookup"><span data-stu-id="16d2a-128">yes</span></span> | <span data-ttu-id="16d2a-129">Gerenciar a infraestrutura do Hub IoT do Azure.</span><span class="sxs-lookup"><span data-stu-id="16d2a-129">Manage Azure IoT Hub infrastructure.</span></span>
| [<span data-ttu-id="16d2a-130">az iot pnp</span><span class="sxs-lookup"><span data-stu-id="16d2a-130">az iot pnp</span></span>](/cli/azure/iot/pnp) | <span data-ttu-id="16d2a-131">sim</span><span class="sxs-lookup"><span data-stu-id="16d2a-131">yes</span></span> | <span data-ttu-id="16d2a-132">Gerenciar repositórios e chaves de acesso do repositório de IoT Plug and Play.</span><span class="sxs-lookup"><span data-stu-id="16d2a-132">Manage IoT Plug and Play repositories and repository access keys.</span></span>

### <a name="extension-reference-commands"></a><span data-ttu-id="16d2a-133">Comandos de referência de extensão</span><span class="sxs-lookup"><span data-stu-id="16d2a-133">Extension reference commands</span></span>

| <span data-ttu-id="16d2a-134">Referência</span><span class="sxs-lookup"><span data-stu-id="16d2a-134">Reference</span></span> | <span data-ttu-id="16d2a-135">Tem um comando principal</span><span class="sxs-lookup"><span data-stu-id="16d2a-135">Has core</span></span> | <span data-ttu-id="16d2a-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="16d2a-136">Description</span></span>
|-|-|-|
| [<span data-ttu-id="16d2a-137">az iot</span><span class="sxs-lookup"><span data-stu-id="16d2a-137">az iot</span></span>](/cli/azure/ext/azure-iot/iot) | <span data-ttu-id="16d2a-138">sim</span><span class="sxs-lookup"><span data-stu-id="16d2a-138">yes</span></span> | <span data-ttu-id="16d2a-139">Todos os comandos de extensão da CLI do Azure disponíveis para o Azure IoT.</span><span class="sxs-lookup"><span data-stu-id="16d2a-139">All available Azure CLI extension commands for Azure IoT.</span></span>
| [<span data-ttu-id="16d2a-140">az iot central</span><span class="sxs-lookup"><span data-stu-id="16d2a-140">az iot central</span></span>](/cli/azure/ext/azure-iot/iot/central) | <span data-ttu-id="16d2a-141">sim</span><span class="sxs-lookup"><span data-stu-id="16d2a-141">yes</span></span> | <span data-ttu-id="16d2a-142">Gerenciar soluções e a infraestrutura do Azure Central (IoT Central).</span><span class="sxs-lookup"><span data-stu-id="16d2a-142">Manage Azure Central (IoT Central) solutions & infrastructure.</span></span>
| [<span data-ttu-id="16d2a-143">az iot device</span><span class="sxs-lookup"><span data-stu-id="16d2a-143">az iot device</span></span>](/cli/azure/ext/azure-iot/iot/device) | | <span data-ttu-id="16d2a-144">Utilizar os recursos de mensagens de dispositivo para nuvem e nuvem para dispositivo.</span><span class="sxs-lookup"><span data-stu-id="16d2a-144">Leverage device-to-cloud and cloud-to-device messaging capabilities.</span></span>
| [<span data-ttu-id="16d2a-145">az dt</span><span class="sxs-lookup"><span data-stu-id="16d2a-145">az dt</span></span>](/cli/azure/ext/azure-iot/dt) | | <span data-ttu-id="16d2a-146">Gerenciar soluções e a infraestrutura dos Gêmeos Digitais do Azure.</span><span class="sxs-lookup"><span data-stu-id="16d2a-146">Manage Azure Digital Twins solutions & infrastructure.</span></span>
| [<span data-ttu-id="16d2a-147">az iot dps</span><span class="sxs-lookup"><span data-stu-id="16d2a-147">az iot dps</span></span>](/cli/azure/ext/azure-iot/iot/dps) | <span data-ttu-id="16d2a-148">sim</span><span class="sxs-lookup"><span data-stu-id="16d2a-148">yes</span></span> | <span data-ttu-id="16d2a-149">Gerenciar entidades em um Serviço de Provisionamento de Dispositivos no Hub IoT do Azure.</span><span class="sxs-lookup"><span data-stu-id="16d2a-149">Manage entities in an Azure IoT Hub Device Provisioning Service.</span></span>
| [<span data-ttu-id="16d2a-150">az iot edge</span><span class="sxs-lookup"><span data-stu-id="16d2a-150">az iot edge</span></span>](/cli/azure/ext/azure-iot/iot/edge) | | <span data-ttu-id="16d2a-151">Gerenciar soluções de IoT no Edge.</span><span class="sxs-lookup"><span data-stu-id="16d2a-151">Manage IoT solutions on the Edge.</span></span>
| [<span data-ttu-id="16d2a-152">az iot hub</span><span class="sxs-lookup"><span data-stu-id="16d2a-152">az iot hub</span></span>](/cli/azure/ext/azure-iot/iot/hub) | <span data-ttu-id="16d2a-153">sim</span><span class="sxs-lookup"><span data-stu-id="16d2a-153">yes</span></span> | <span data-ttu-id="16d2a-154">Gerenciar entidades em um Hub IoT do Azure.</span><span class="sxs-lookup"><span data-stu-id="16d2a-154">Manage entities in an Azure IoT Hub.</span></span>
| [<span data-ttu-id="16d2a-155">az iot pnp</span><span class="sxs-lookup"><span data-stu-id="16d2a-155">az iot pnp</span></span>](/cli/azure/ext/azure-iot/iot/pnp) | <span data-ttu-id="16d2a-156">sim</span><span class="sxs-lookup"><span data-stu-id="16d2a-156">yes</span></span> | <span data-ttu-id="16d2a-157">Gerenciar entidades de um repositório de modelos de IoT Plug and Play.</span><span class="sxs-lookup"><span data-stu-id="16d2a-157">Manage entities of an IoT Plug and Play model repository.</span></span>

### <a name="additional-cli-commands-for-azure-services-used-by-iot"></a><span data-ttu-id="16d2a-158">Comandos adicionais da CLI para serviços do Azure usados pela IoT</span><span class="sxs-lookup"><span data-stu-id="16d2a-158">Additional CLI commands for Azure services used by IoT</span></span>

| <span data-ttu-id="16d2a-159">Referência</span><span class="sxs-lookup"><span data-stu-id="16d2a-159">Reference</span></span> | <span data-ttu-id="16d2a-160">Type</span><span class="sxs-lookup"><span data-stu-id="16d2a-160">Type</span></span> | <span data-ttu-id="16d2a-161">Descrição</span><span class="sxs-lookup"><span data-stu-id="16d2a-161">Description</span></span>
|-|-|-|
| [<span data-ttu-id="16d2a-162">az maps</span><span class="sxs-lookup"><span data-stu-id="16d2a-162">az maps</span></span>](/cli/azure/maps) | <span data-ttu-id="16d2a-163">core</span><span class="sxs-lookup"><span data-stu-id="16d2a-163">core</span></span> | <span data-ttu-id="16d2a-164">Gerenciar o Azure Mapas.</span><span class="sxs-lookup"><span data-stu-id="16d2a-164">Manage Azure Maps.</span></span>
| [<span data-ttu-id="16d2a-165">az timeseriesinsights</span><span class="sxs-lookup"><span data-stu-id="16d2a-165">az timeseriesinsights</span></span>](/cli/azure/ext/timeseriesinsights/timeseriesinsights) | <span data-ttu-id="16d2a-166">extensão</span><span class="sxs-lookup"><span data-stu-id="16d2a-166">extension</span></span> | <span data-ttu-id="16d2a-167">Gerenciar o Azure Time Series Insights.</span><span class="sxs-lookup"><span data-stu-id="16d2a-167">Manage Azure Time Series Insights.</span></span>

## <a name="popular-iot-articles-using-the-azure-cli"></a><span data-ttu-id="16d2a-168">Artigos populares sobre IoT em que a CLI do Azure é usada</span><span class="sxs-lookup"><span data-stu-id="16d2a-168">Popular IoT articles using the Azure CLI</span></span>

- [<span data-ttu-id="16d2a-169">Criar um hub IoT</span><span class="sxs-lookup"><span data-stu-id="16d2a-169">Create an IoT hub</span></span>](/azure/iot-hub/iot-hub-create-using-cli)
- [<span data-ttu-id="16d2a-170">Gerenciar o IoT Central</span><span class="sxs-lookup"><span data-stu-id="16d2a-170">Manage IoT Central</span></span>](/azure/iot-central/core/howto-manage-iot-central-from-cli)
- [<span data-ttu-id="16d2a-171">Tutoriais de dispositivos controlados pela CLI usando o Azure RTOS</span><span class="sxs-lookup"><span data-stu-id="16d2a-171">CLI driven device tutorials using Azure RTOS</span></span>](/azure/rtos/getting-started?branch=master)
- [<span data-ttu-id="16d2a-172">Usar a extensão de IoT para gerenciamento de dispositivo do Hub IoT do Azure</span><span class="sxs-lookup"><span data-stu-id="16d2a-172">Use the IoT extension for Azure IoT Hub device management</span></span>](/azure/iot-hub/iot-hub-device-management-iot-extension-azure-cli-2-0)
- [<span data-ttu-id="16d2a-173">Implantar e monitorar módulos do IoT Edge em escala usando a extensão da CLI do Azure para IoT</span><span class="sxs-lookup"><span data-stu-id="16d2a-173">Deploy and monitor IoT Edge modules at scale with the Azure CLI extension for IoT</span></span>](/azure/iot-edge/how-to-deploy-cli-at-scale)
- [<span data-ttu-id="16d2a-174">Enviar telemetria para um dispositivo e monitorá-lo com a extensão da CLI do Azure para IoT</span><span class="sxs-lookup"><span data-stu-id="16d2a-174">Send Telemetry to a device and monitor it with the Azure CLI extension for IoT</span></span>](/azure/iot-hub/quickstart-send-telemetry-cli)
- [<span data-ttu-id="16d2a-175">Usar a CLI do Azure para configurar o roteamento de mensagens do Hub IoT</span><span class="sxs-lookup"><span data-stu-id="16d2a-175">Use the Azure CLI to configure IoT Hub message routing</span></span>](/azure/iot-hub/tutorial-routing-config-message-routing-cli)
- [<span data-ttu-id="16d2a-176">Gerenciar interfaces em um repositório de modelos Plug and Play</span><span class="sxs-lookup"><span data-stu-id="16d2a-176">Manage interfaces in a Plug and Play model repository</span></span>](/azure/iot-pnp/howto-install-pnp-cli#manage-interfaces-in-a-model-repository)

## <a name="azure-cli-reference-examples"></a><span data-ttu-id="16d2a-177">Exemplos de referência da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="16d2a-177">Azure CLI reference examples</span></span>

<span data-ttu-id="16d2a-178">São fornecidos exemplos com todas as referências da CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="16d2a-178">Examples are provided with every Azure CLI reference.</span></span> <span data-ttu-id="16d2a-179">Embora você também possa concluir essas tarefas no portal do Azure, usar a CLI do Azure requer uma só linha de comando.</span><span class="sxs-lookup"><span data-stu-id="16d2a-179">Although you can also complete these tasks through the Azure portal, using the Azure CLI requires a single command line.</span></span>  <span data-ttu-id="16d2a-180">Veja alguns blocos de código para ter uma ideia de como é fácil usar a CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="16d2a-180">Here are a few code blocks to give you an idea of how easy it is to use the Azure CLI.</span></span>

<span data-ttu-id="16d2a-181">Para trabalhar com o Azure IoT, primeiro você precisará de um grupo de recursos.</span><span class="sxs-lookup"><span data-stu-id="16d2a-181">To work with Azure IoT, you'll first need a resource group.</span></span>  <span data-ttu-id="16d2a-182">Os grupos de recursos do Azure são simples de criar e gerenciar com a CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="16d2a-182">Azure resource groups are simple to create and manage with the Azure CLI.</span></span>  

```azurecli
#create a resource group
az group create -location westus -name MyResourceGroup
```

```azurecli
#get a list of resource groups for a subscription
az group list --subscription MySubscription --output table
```

<span data-ttu-id="16d2a-183">É tão simples quanto criar um Hub IoT do Azure na região '''westus''' com o tipo de preço Standard.</span><span class="sxs-lookup"><span data-stu-id="16d2a-183">It is as straightforward to create an Azure IoT Hub in the '''westus''' region in the standard pricing tier.</span></span>

```azurecli
#create an Azure IoT hub
az iot hub create --resource-group MyResourceGroup --name MyIotHub --location westus
```

## <a name="see-also"></a><span data-ttu-id="16d2a-184">Confira também</span><span class="sxs-lookup"><span data-stu-id="16d2a-184">See also</span></span>

- <span data-ttu-id="16d2a-185">[Introdução à CLI do Azure](/cli/azure/get-started-with-azure-cli) para saber mais sobre a instalação e a conexão.</span><span class="sxs-lookup"><span data-stu-id="16d2a-185">[Get started with Azure CLI](/cli/azure/get-started-with-azure-cli) to learn about installation and sign in.</span></span>

- <span data-ttu-id="16d2a-186">Descubra referências adicionais [lançadas](/cli/azure/reference-index) e de [extensão](/cli/azure/azure-cli-extensions-list) na documentação da CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="16d2a-186">Discover additional [released](/cli/azure/reference-index) and [extension](/cli/azure/azure-cli-extensions-list) references in the Azure CLI documentation.</span></span>

- <span data-ttu-id="16d2a-187">Saiba mais sobre as referências de extensão em [Usar extensões com a CLI do Azure](/cli/azure/azure-cli-extensions-overview).</span><span class="sxs-lookup"><span data-stu-id="16d2a-187">Find out more about extension references in [Use extensions with Azure CLI](/cli/azure/azure-cli-extensions-overview).</span></span>
