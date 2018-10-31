---
title: Extensões disponíveis para a CLI do Azure
description: Uma lista completa das extensões com suporte oficial para a CLI do Azure.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 10/25/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: bf6af6cd42f8a2f7f6db6fd0e561020c1fac6c01
ms.sourcegitcommit: cc9def8719d9dfaba409493c2be1619c21b8c899
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/26/2018
ms.locfileid: "50132496"
---
# <a name="available-extensions-for-the-azure-cli"></a>Extensões disponíveis para a CLI do Azure

Este artigo é uma lista completa das extensões disponíveis para a CLI do Azure que têm suporte da Microsoft.

A lista de extensões também está disponível na CLI. Para obtê-la, execute [az extension list-available](/cli/azure/extension?view=azure-cli-latest#az-extension-list-available):

```azurecli
az extension list-available --output table
```

| NOME | Versão | Resumo | Visualização |
|------|---------|---------|---------|
| [aem](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Gerenciar Extensões de Monitoramento Aprimorado do Azure para SAP |  |
| [alias](https://github.com/Azure/azure-cli-extensions) | 0.5.1 | Suporte para aliases de comando | SIM |
| [azure-batch-cli-extensions](https://github.com/Azure/azure-batch-cli-extensions) | 2.5.1 | Comandos adicionais para trabalhar com o serviço de Lote do Azure |  |
| [azure-cli-iot-ext](https://github.com/azure/azure-iot-cli-extension) | 0.6.0 | Fornece a camada de comandos do plano de dados para o Azure Hub IoT, IoT Edge e o Serviço de Provisionamento de Dispositivos |  |
| [azure-firewall](https://github.com/Azure/azure-cli-extensions/tree/master/src/azure-firewall) | 0.1.0 | Gerenciar recursos do Firewall do Azure. | SIM |
| [botservice](https://github.com/Azure/azure-cli-extensions) | 0.4.1 | Correções de bug para problemas no módulo de comando de CLI do botservice nativo. | SIM |
| [dev-spaces-preview](https://github.com/Azure/azure-cli-extensions) | 0.1.6 | Os Espaços de Desenvolvimento fornecem uma experiência de desenvolvimento Kubernetes rápida e iterativa para equipes. | SIM |
| [dms-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/dms-preview) | 0.5.0 | Suporte para novos cenários do Serviço de Migração de Banco de Dados. | SIM |
| [dns](https://github.com/Azure/azure-cli-extensions) | 0.0.2 | Uma extensão da CLI do Azure para zonas DNS |  |
| [eventgrid](https://github.com/Azure/azure-cli-extensions) | 0.2.1 | Suporte para recursos do Azure EventGrid 2018-05-01-preview | SIM |
| [express-route](https://github.com/Azure/azure-cli-extensions/tree/master/src/express-route) | 0.1.3 | Gerenciar ExpressRoute com versão prévia dos recursos. | SIM |
| [express-route-cross-connection](https://github.com/Azure/azure-cli-extensions/tree/master/src/express-route-cross-connection) | 0.1.0 | Gerencie os circuitos do ExpressRoute de cliente usando uma conexão cruzada do ExpressRoute. |  |
| [find](https://github.com/Azure/azure-cli-extensions/tree/master/src/find) | 0.2.0 | Consultas inteligentes para obter informações de CLI. | SIM |
| [front-door](https://github.com/Azure/azure-cli-extensions/tree/master/src/front-door) | 0.1.1 | Gerenciar FrontDoors de rede. | SIM |
| [image-copy-extension](https://github.com/Azure/azure-cli-extensions) | 0.0.8 | Suporte para copiar imagens de vm gerenciadas entre regiões |  |
| [interativo](https://github.com/Azure/azure-cli) | 0.4.0 | Shell interativo de linha de comando do Microsoft Azure | SIM |
| [keyvault-preview](https://github.com/Azure/azure-keyvault-cli-extension) | 0.1.3 | Visualizar comandos do Azure Key Vault. | SIM |
| [log-analytics](https://github.com/Azure/azure-cli-extensions/tree/master/src/log-analytics) | 0.1.3 | Suporte para recursos de consulta do Log Analytics do Azure. | SIM |
| [managementgroups](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Uma extensão da CLI do Azure para grupos de gerenciamento |  |
| [managementpartner](https://github.com/Azure/azure-cli-extensions) | 0.1.2 | Suporte à versão prévia de Parceiro de Gerenciamento |  |
| [malha](https://github.com/Azure/azure-cli-extensions) | 0.9.3 | Suporte para a Malha do Microsoft Azure Service Fabric - Visualização Pública | SIM |
| [rdbms-vnet](https://github.com/Azure/azure-cli-extensions) | 10.0.0 | Suporte para regras de Rede Virtual no Azure MySQL e recursos do Azure PostgreSQL |  |
| [resource-graph](https://github.com/Azure/azure-cli-extensions/tree/master/src/resource-graph) | 0.1.8 | Suporte para consultar recursos do Azure com o Resource Graph. | SIM |
| [sap-hana](https://github.com/Azure/azure-hanaonazure-cli-extension) | 0.1.6 | Comandos adicionais para trabalhar com instâncias do SAP HanaOnAzure. |  |
| [signalr](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Suporte à versão prévia de gerenciamento de signalr. | SIM |
| [storage-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/storage-preview) | 0.1.6 | Fornece uma visualização para recursos de armazenamento futuras. | SIM |
| [subscription](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Suporte à versão prévia de gerenciamento de assinatura. |  |
| [virtual-network-tap](https://github.com/Azure/azure-cli-extensions/tree/master/src/virtual-network-tap) | 0.1.0 | Gerenciar TAPs de rede virtual (VTAP). | SIM |
| [virtual-wan](https://github.com/Azure/azure-cli-extensions/tree/master/src/virtual-wan) | 0.1.0 | Gerencie WAN virtual, hubs, gateways de VPN e sites VPN. | SIM |
| [webapp](https://github.com/Azure/azure-cli-extensions) | 0.2.12 | Comandos adicionais para o Serviço de Aplicativo do Azure. | SIM |