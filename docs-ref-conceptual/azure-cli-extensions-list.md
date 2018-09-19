---
title: Extensões disponíveis para a CLI do Azure 2.0
description: Uma lista completa das extensões com suporte oficial para a CLI do Azure 2.0.
author: derekbekoe
ms.author: debekoe
manager: routlaw
ms.date: 09/06/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 24134d9769f7e89afe82f74490c6b49c81c7883f
ms.sourcegitcommit: 46d4040eae1923c59caaac22aedab303b3116dad
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/06/2018
ms.locfileid: "44048741"
---
# <a name="available-extensions-for-the-azure-cli-20"></a>Extensões disponíveis para a CLI do Azure 2.0

Este artigo é uma lista completa das extensões disponíveis para a CLI do Azure 2.0 que são oferecidas e têm suporte da Microsoft.

A lista de extensões também está disponível diretamente na CLI. Para obtê-la, execute [az extension list-available](/cli/azure/extension?view=azure-cli-latest#az-extension-list-available):

```azurecli
az extension list-available --output table
```

| NOME | Versão | Resumo | Visualização |
|------|---------|---------|---------|
| [aem](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Gerenciar Extensões de Monitoramento Aprimorado do Azure para SAP |  |
| [alias](https://github.com/Azure/azure-cli-extensions) | 0.5.1 | Suporte para aliases de comando | SIM |
| [azure-batch-cli-extensions](https://github.com/Azure/azure-batch-cli-extensions) | 2.4.1 | Comandos adicionais para trabalhar com o serviço de Lote do Azure |  |
| [azure-cli-iot-ext](https://github.com/azure/azure-iot-cli-extension) | 0.5.2 | Fornece a camada de comandos do plano de dados para o Azure Hub IoT, IoT Edge e o Serviço de Provisionamento de Dispositivos |  |
| [botservice](https://github.com/Azure/azure-cli-extensions) | 0.4.0 | Correções de bug para problemas no módulo de comando de CLI do botservice nativo. | SIM |
| [dev-spaces-preview](https://github.com/Azure/azure-cli-extensions) | 0.1.6 | Os Espaços de Desenvolvimento fornecem uma experiência de desenvolvimento Kubernetes rápida e iterativa para equipes. | SIM |
| [dns](https://github.com/Azure/azure-cli-extensions) | 0.0.2 | Uma extensão da CLI do Azure para zonas DNS |  |
| [eventgrid](https://github.com/Azure/azure-cli-extensions) | 0.2.1 | Suporte para recursos do Azure EventGrid 2018-05-01-preview | SIM |
| [express-route-cross-connection](https://github.com/Azure/azure-cli-extensions/tree/master/src/express-route-cross-connection) | 0.1.0 | Gerencie os circuitos do ExpressRoute de cliente usando uma conexão cruzada do ExpressRoute. |  |
| [find](https://github.com/Azure/azure-cli-extensions/tree/master/src/find) | 0.1.0 | Consultas inteligentes para obter informações de CLI. | SIM |
| [image-copy-extension](https://github.com/Azure/azure-cli-extensions) | 0.0.8 | Suporte para copiar imagens de vm gerenciadas entre regiões |  |
| [keyvault-preview](https://github.com/Azure/azure-keyvault-cli-extension) | 0.1.3 | Visualizar comandos do Azure Key Vault. | SIM |
| [log-analytics](https://github.com/Azure/azure-cli-extensions/tree/master/src/log-analytics) | 0.1.2 | Suporte para recursos de consulta do Log Analytics do Azure. | SIM |
| [managementgroups](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Uma extensão da CLI do Azure para grupos de gerenciamento |  |
| [managementpartner](https://github.com/Azure/azure-cli-extensions) | 0.1.2 | Suporte à versão prévia de Parceiro de Gerenciamento |  |
| [malha](https://github.com/Azure/azure-cli-extensions) | 0.9.1 | Suporte para a Malha do Microsoft Azure Service Fabric - Visualização Pública | SIM |
| [rdbms-vnet](https://github.com/Azure/azure-cli-extensions) | 10.0.0 | Suporte para regras de Rede Virtual no Azure MySQL e recursos do Azure PostgreSQL |  |
| [signalr](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Suporte à versão prévia de gerenciamento de signalr. | SIM |
| [storage-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/storage-preview) | 0.1.4 | Fornece uma visualização para recursos de armazenamento futuras. | SIM |
| [subscription](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Suporte à versão prévia de gerenciamento de assinatura. |  |
| [webapp](https://github.com/Azure/azure-cli-extensions) | 0.2.8 | Uma extensão da CLI do Azure para gerenciar recursos de appservice | SIM |
