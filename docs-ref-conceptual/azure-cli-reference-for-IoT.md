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
ms.openlocfilehash: b3042b569267233f00a2bc1ea4b65089dae9cae5
ms.sourcegitcommit: b9b310407d99662296998b6e23d3903d61cc3756
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/14/2020
ms.locfileid: "88216537"
---
# <a name="azure-cli-for-azure-iot"></a>CLI do Azure para o Azure IoT

A [CLI do Azure](/cli/azure/what-is-azure-cli) (Interface de Linha de Comando do Azure) é um conjunto de comandos usados para criar e gerenciar recursos do Azure.  Ela está disponível em muitos serviços do Azure, incluindo o Azure IoT.  Há mais de 100 referências do Azure IoT, que possibilitam que você trabalhe de maneira eficaz com os serviços de IoT usando uma linha de comando.

## <a name="references-for-iot"></a>Referências de IoT

A experiência da CLI do Azure IoT é composta por duas partes: A CLI do Azure (também chamada de CLI **principal**) e a **extensão** da CLI do Azure IoT.

A funcionalidade de IoT na CLI do Azure **principal** tem como foco o gerenciamento e a configuração da infraestrutura. Operações de CRUD do Hub IoT, ou a configuração de rotas de mensagens do Hub IoT, são casos de uso típicos dos comandos principais.

A extensão de **IoT** traz recursos e funcionalidades avançadas para gerenciar, manipular e interagir com os dados, entidades e objetos na própria infraestrutura. Por exemplo, o gerenciamento de frotas de dispositivos, o monitoramento de eventos de dispositivo para nuvem e a invocação de métodos da nuvem para o dispositivo são habilitados por meio da extensão de IoT. A extensão do Azure IoT para a CLI do Azure desbloqueia o uso de tecnologias experimentais ou em pré-lançamento que contribuem para sua versatilidade em diversos cenários e casos de uso.

### <a name="core-reference-commands"></a>Comandos de referência principais

| Referência | Tem uma extensão | Descrição
|-|-|-|
| [az iot](/cli/azure/iot) | sim  | Todos os comandos principais da CLI do Azure disponíveis para o Azure IoT.
| [az iot central](/cli/azure/iot/central) | sim | Gerenciar ativos do IoT Central.
| [az iot dps](/en-us/cli/azure/iot/dps) | sim | Gerenciar o Serviço de Provisionamento de Dispositivos no Hub IoT do Azure.
| [az iot hub](/cli/azure/iot/hub) | sim | Gerenciar a infraestrutura do Hub IoT do Azure.

### <a name="extension-reference-commands"></a>Comandos de referência de extensão

| Referência | Tem um comando principal | Descrição
|-|-|-|
| [az iot](/cli/azure/ext/azure-iot/iot) | sim | Todos os comandos de extensão da CLI do Azure disponíveis para o Azure IoT.
| [az iot central](/cli/azure/ext/azure-iot/iot/central) | sim | Gerenciar soluções e a infraestrutura do Azure Central (IoT Central).
| [az iot device](/cli/azure/ext/azure-iot/iot/device) | | Utilizar os recursos de mensagens de dispositivo para nuvem e nuvem para dispositivo.
| [az dt](/cli/azure/ext/azure-iot/dt) | | Gerenciar soluções e a infraestrutura dos Gêmeos Digitais do Azure.
| [az iot dps](/cli/azure/ext/azure-iot/iot/dps) | sim | Gerenciar entidades em um Serviço de Provisionamento de Dispositivos no Hub IoT do Azure.
| [az iot edge](/cli/azure/ext/azure-iot/iot/edge) | | Gerenciar soluções de IoT no Edge.
| [az iot hub](/cli/azure/ext/azure-iot/iot/hub) | sim | Gerenciar entidades em um Hub IoT do Azure.
| [az iot pnp](/cli/azure/ext/azure-iot/iot/pnp) | | Gerenciar entidades de um repositório de modelos de IoT Plug and Play.

### <a name="additional-cli-commands-for-azure-services-used-by-iot"></a>Comandos adicionais da CLI para serviços do Azure usados pela IoT

| Referência | Type | Descrição
|-|-|-|
| [az maps](/cli/azure/maps) | core | Gerenciar o Azure Mapas.
| [az timeseriesinsights](/cli/azure/ext/timeseriesinsights/timeseriesinsights) | extensão | Gerenciar o Azure Time Series Insights.

### <a name="extension-reference-installation"></a>Instalação de referência de extensão

As referências de extensão da CLI do Azure devem ser instaladas antes do uso.  Use o comando [az extension add](/cli/azure/azure-cli-extensions-overview) para instalar uma referência de extensão por nome.  Saiba mais sobre as referências de extensão em [Usar extensões com a CLI do Azure](/cli/azure/azure-cli-extensions-overview).

```azurecli
# install the Azure CLI extension reference for Azure IoT
az extension add --name azure-iot
```

## <a name="popular-iot-articles-using-the-azure-cli"></a>Artigos populares sobre IoT em que a CLI do Azure é usada

- [Criar um hub IoT](/azure/iot-hub/iot-hub-create-using-cli)
- [Gerenciar o IoT Central](/azure/iot-central/core/howto-manage-iot-central-from-cli)
- [Tutoriais de dispositivos controlados pela CLI usando o Azure RTOS](/azure/rtos/getting-started?branch=master)
- [Usar a extensão de IoT para gerenciamento de dispositivo do Hub IoT do Azure](/azure/iot-hub/iot-hub-device-management-iot-extension-azure-cli-2-0)
- [Implantar e monitorar módulos do IoT Edge em escala usando a extensão da CLI do Azure para IoT](/azure/iot-edge/how-to-deploy-cli-at-scale)
- [Enviar telemetria para um dispositivo e monitorá-lo com a extensão da CLI do Azure para IoT](/azure/iot-hub/quickstart-send-telemetry-cli)
- [Usar a CLI do Azure para configurar o roteamento de mensagens do Hub IoT](/azure/iot-hub/tutorial-routing-config-message-routing-cli)
- [Gerenciar interfaces em um repositório de modelos Plug and Play](/azure/iot-pnp/howto-install-pnp-cli#manage-interfaces-in-a-model-repository)

## <a name="azure-cli-reference-examples"></a>Exemplos de referência da CLI do Azure

São fornecidos exemplos com todas as referências da CLI do Azure. Embora você também possa concluir essas tarefas no portal do Azure, usar a CLI do Azure requer uma só linha de comando.  Veja alguns blocos de código para ter uma ideia de como é fácil usar a CLI do Azure.

Para trabalhar com o Azure IoT, primeiro você precisará de um grupo de recursos.  Os grupos de recursos do Azure são simples de criar e gerenciar com a CLI do Azure.  

```azurecli
#create a resource group
az group create -location westus -name MyResourceGroup
```

```azurecli
#get a list of resource groups for a subscription
az group list --subscription MySubscription --output table
```

É tão simples quanto criar um Hub IoT do Azure na região '''westus''' com o tipo de preço Standard.

```azurecli
#create an Azure IoT hub
az iot hub create --resource-group MyResourceGroup --name MyIotHub --location westus
```

## <a name="see-also"></a>Confira também

- [Introdução à CLI do Azure](/cli/azure/get-started-with-azure-cli) para saber mais sobre a instalação e a conexão.

- Descubra referências adicionais [lançadas](/cli/azure/reference-index) e de [extensão](/cli/azure/azure-cli-extensions-list) na documentação da CLI do Azure.
