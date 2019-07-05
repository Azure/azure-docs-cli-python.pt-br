---
title: Extensões disponíveis para a CLI do Azure
description: Uma lista completa das extensões com suporte oficial para a CLI do Azure.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 06/30/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 63d50a46a81482e260307cdc44adfea6aa4499f1
ms.sourcegitcommit: e06d34682710e77840b0c51f4718184101bd8a03
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "67527340"
---
# <a name="available-extensions-for-the-azure-cli"></a>Extensões disponíveis para a CLI do Azure

Este artigo é uma lista completa das extensões disponíveis para a CLI do Azure que têm suporte da Microsoft.

A lista de extensões também está disponível na CLI. Para obtê-la, execute [az extension list-available](/cli/azure/extension?view=azure-cli-latest#az-extension-list-available):

```azurecli-interactive
az extension list-available --output table
```

| NOME | Versão | Resumo | Visualização |
|------|---------|---------|---------|
| [aem](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Gerenciar Extensões de Monitoramento Aprimorado do Azure para SAP |  |
| [versão prévia do aks](https://github.com/Azure/azure-cli-extensions/tree/master/src/aks-preview) | 0.4.5 | Fornece uma versão prévia para futuros recursos do AKS | Sim |
| [alias](https://github.com/Azure/azure-cli-extensions) | 0.5.2 | Suporte para aliases de comando | Sim |
| [appconfig](https://github.com/Azure/azure-cli-extensions) | 0.5.0 | Fornece uma versão prévia para os futuros recursos de Configuração do Aplicativo. | Sim |
| [application-insights](https://github.com/Azure/azure-cli-extensions/tree/master/src/application-insights) | 0.1.1 | Suporte para gerenciar componentes do Application Insights e consultar as métricas, os eventos e os logs de tais componentes. | Sim |
| [azure-batch-cli-extensions](https://github.com/Azure/azure-batch-cli-extensions) | 3.0.4 | Comandos adicionais para trabalhar com o serviço de Lote do Azure |  |
| [azure-cli-iot-ext](https://github.com/azure/azure-iot-cli-extension) | 0.7.1 | Fornece a camada de comandos do plano de dados para o Azure Hub IoT, IoT Edge e o Serviço de Provisionamento de Dispositivos |  |
| [azure-cli-ml](https://docs.microsoft.com/en-us/azure/machine-learning/service/) | 1.0.45.1 | Módulo de Comando do AzureML para as Ferramentas da Linha de Comando do Microsoft Azure |  |
| [azure-devops](https://github.com/Microsoft/azure-devops-cli-extension) | 0.11.0 | Ferramentas para gerenciar o Azure DevOps. |  |
| [azure-firewall](https://github.com/Azure/azure-cli-extensions/tree/master/src/azure-firewall) | 0.1.3 | Gerenciar recursos do Firewall do Azure. | Sim |
| [db-up](https://github.com/Azure/azure-cli-extensions/tree/master/src/db-up) | 0.1.13 | Comandos adicionais para simplificar os fluxos de trabalho do Banco de Dados do Azure. | Sim |
| [dev-spaces](https://github.com/Azure/azure-cli-extensions) | 1.0.3 | Os Espaços de Desenvolvimento fornecem uma experiência de desenvolvimento Kubernetes rápida e iterativa para equipes. |  |
| [dev-spaces-preview](https://github.com/Azure/azure-cli-extensions) | 0.1.6 | Os Espaços de Desenvolvimento fornecem uma experiência de desenvolvimento Kubernetes rápida e iterativa para equipes. | Sim |
| [dms-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/dms-preview) | 0.8.1 | Suporte para novos cenários do Serviço de Migração de Banco de Dados. | Sim |
| [dns](https://github.com/Azure/azure-cli-extensions) | 0.0.2 | Uma extensão da CLI do Azure para zonas DNS |  |
| [eventgrid](https://github.com/Azure/azure-cli-extensions) | 0.4.3 | Módulo de Comando do EventGrid para as Ferramentas da Linha de Comando do Microsoft Azure. | Sim |
| [express-route](https://github.com/Azure/azure-cli-extensions/tree/master/src/express-route) | 0.1.3 | Gerenciar ExpressRoute com versão prévia dos recursos. | Sim |
| [express-route-cross-connection](https://github.com/Azure/azure-cli-extensions/tree/master/src/express-route-cross-connection) | 0.1.1 | Gerencie os circuitos do ExpressRoute de cliente usando uma conexão cruzada do ExpressRoute. |  |
| [find](https://github.com/Azure/azure-cli-extensions/tree/master/src/find) | 0.3.0 | Consultas inteligentes para obter informações de CLI. | Sim |
| [front-door](https://github.com/Azure/azure-cli-extensions/tree/master/src/front-door) | 0.1.8 | Gerenciar FrontDoors de rede. | Sim |
| [image-copy-extension](https://github.com/Azure/azure-cli-extensions) | 0.2.1 | Suporte para copiar imagens de vm gerenciadas entre regiões |  |
| [interativo](https://github.com/Azure/azure-cli) | 0.4.3 | Shell interativo de linha de comando do Microsoft Azure | Sim |
| [keyvault-preview](https://github.com/Azure/azure-keyvault-cli-extension) | 0.1.3 | Visualizar comandos do Azure Key Vault. | Sim |
| [log-analytics](https://github.com/Azure/azure-cli-extensions/tree/master/src/log-analytics) | 0.1.3 | Suporte para recursos de consulta do Log Analytics do Azure. | Sim |
| [managementgroups](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Uma extensão da CLI do Azure para grupos de gerenciamento |  |
| [managementpartner](https://github.com/Azure/azure-cli-extensions) | 0.1.2 | Suporte à versão prévia de Parceiro de Gerenciamento |  |
| [malha](https://github.com/Azure/azure-cli-extensions) | 0.10.6 | Suporte para a Malha do Microsoft Azure Service Fabric - Visualização Pública | Sim |
| [mixed-reality](https://github.com/Azure/azure-cli-extensions) | 0.0.1 | Extensão da CLI da Realidade Misturada do Azure. |  |
| [netappfiles-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/netappfiles-preview) | 0.3.2 | Fornece uma versão prévia para os futuros recursos do ANF (Azure NetApp Files). | Sim |
| [privatedns](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Comandos para gerenciar zonas DNS privadas | Sim |
| [resource-graph](https://github.com/Azure/azure-cli-extensions/tree/master/src/resource-graph) | 0.1.11 | Suporte para consultar recursos do Azure com o Resource Graph. | Sim |
| [sap-hana](https://github.com/Azure/azure-hanaonazure-cli-extension) | 0.4.1 | Comandos adicionais para trabalhar com instâncias do SAP HanaOnAzure. |  |
| [storage-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/storage-preview) | 0.2.7 | Fornece uma visualização para recursos de armazenamento futuras. | Sim |
| [subscription](https://github.com/Azure/azure-cli-extensions) | 0.1.3 | Suporte à versão prévia de gerenciamento de assinatura. |  |
| [virtual-network-tap](https://github.com/Azure/azure-cli-extensions/tree/master/src/virtual-network-tap) | 0.1.0 | Gerenciar TAPs de rede virtual (VTAP). | Sim |
| [virtual-wan](https://github.com/Azure/azure-cli-extensions/tree/master/src/virtual-wan) | 0.1.0 | Gerencie WAN virtual, hubs, gateways de VPN e sites VPN. | Sim |
| [vm-repair](https://github.com/Azure/azure-cli-extensions/tree/master/src/vm-repair) | 0.1.1 | Comandos de reparo automático para corrigir as VMs. |  |
| [webapp](https://github.com/Azure/azure-cli-extensions/tree/master/src/webapp) | 0.2.19 | Comandos adicionais para o Serviço de Aplicativo do Azure. | Sim |