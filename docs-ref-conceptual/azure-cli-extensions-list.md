---
title: Extensões disponíveis para a CLI do Azure
description: Uma lista completa das extensões com suporte oficial para a CLI do Azure.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 02/05/2020
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: c11f43f2cabd0b7d2cef41cdecfead24791661e8
ms.sourcegitcommit: c332e9d6eeb4c0a8fbf587bd750002086f8ff0db
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2020
ms.locfileid: "77038219"
---
# <a name="available-extensions-for-the-azure-cli"></a>Extensões disponíveis para a CLI do Azure

Este artigo é uma lista completa das extensões disponíveis para a CLI do Azure que têm suporte da Microsoft.

A lista de extensões também está disponível na CLI. Para obtê-la, execute [az extension list-available](/cli/azure/extension?view=azure-cli-latest#az-extension-list-available):

```azurecli-interactive
az extension list-available --output table
```

| Nome | Versão | Resumo | Visualização |
|------|---------|---------|---------|
| [aem](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Gerenciar Extensões de Monitoramento Aprimorado do Azure para SAP |  |
| [versão prévia do aks](https://github.com/Azure/azure-cli-extensions/tree/master/src/aks-preview) | 0.4.27 | Fornece uma versão prévia para futuros recursos do AKS | Sim |
| [alias](https://github.com/Azure/azure-cli-extensions) | 0.5.2 | Suporte para aliases de comando | Sim |
| [appconfig](https://github.com/Azure/azure-cli-extensions) | 0.5.0 | Fornece uma versão prévia para os futuros recursos de Configuração do Aplicativo. | Sim |
| [application-insights](https://github.com/Azure/azure-cli-extensions/tree/master/src/application-insights) | 0.1.3 | Suporte para gerenciar componentes do Application Insights e consultar as métricas, os eventos e os logs de tais componentes. | Sim |
| [azure-batch-cli-extensions](https://github.com/Azure/azure-batch-cli-extensions) | 5.0.0 | Comandos adicionais para trabalhar com o serviço de Lote do Azure |  |
| [azure-cli-iot-ext](https://github.com/azure/azure-iot-cli-extension) | 0.8.9 | A extensão de IoT do Azure para a CLI do Azure. |  |
| [azure-cli-ml](https://docs.microsoft.com/azure/machine-learning/service/) | 1.0.85 | Módulo de Comando do AzureML para as Ferramentas da Linha de Comando do Microsoft Azure |  |
| [azure-devops](https://github.com/Microsoft/azure-devops-cli-extension) | 0.17.0 | Ferramentas para gerenciar o Azure DevOps. |  |
| [azure-firewall](https://github.com/Azure/azure-cli-extensions/tree/master/src/azure-firewall) | 0.1.9 | Gerenciar recursos do Firewall do Azure. | Sim |
| [connectedmachine](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Extensão Connectedmachine das Ferramentas de Linha de Comando do Microsoft Azure | Sim |
| [connection-monitor-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/connection-monitor-preview) | 0.1.0 | Extensão Monitor de Conexão de Linha de Comando do Microsoft Azure V2 | Sim |
| [db-up](https://github.com/Azure/azure-cli-extensions/tree/master/src/db-up) | 0.1.13 | Comandos adicionais para simplificar os fluxos de trabalho do Banco de Dados do Azure. | Sim |
| [dev-spaces](https://github.com/Azure/azure-cli-extensions) | 1.0.4 | Os Espaços de Desenvolvimento fornecem uma experiência de desenvolvimento Kubernetes rápida e iterativa para equipes. |  |
| [dev-spaces-preview](https://github.com/Azure/azure-cli-extensions) | 0.1.6 | Os Espaços de Desenvolvimento fornecem uma experiência de desenvolvimento Kubernetes rápida e iterativa para equipes. | Sim |
| [dms-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/dms-preview) | 0.9.0 | Suporte para novos cenários do Serviço de Migração de Banco de Dados. | Sim |
| [eventgrid](https://github.com/Azure/azure-cli-extensions) | 0.4.4 | Módulo de Comando do EventGrid para as Ferramentas da Linha de Comando do Microsoft Azure. | Sim |
| [express-route](https://github.com/Azure/azure-cli-extensions/tree/master/src/express-route) | 0.1.3 | Gerenciar ExpressRoute com versão prévia dos recursos. | Sim |
| [express-route-cross-connection](https://github.com/Azure/azure-cli-extensions/tree/master/src/express-route-cross-connection) | 0.1.1 | Gerencie os circuitos do ExpressRoute de cliente usando uma conexão cruzada do ExpressRoute. |  |
| [find](https://github.com/Azure/azure-cli-extensions/tree/master/src/find) | 0.3.0 | Consultas inteligentes para obter informações de CLI. | Sim |
| [front-door](https://github.com/Azure/azure-cli-extensions/tree/master/src/front-door) | 1.0.2 | Gerenciar FrontDoors de rede. |  |
| [hack](https://github.com/Azure/azure-cli-extensions) | 0.4.1 | Extensão Hack das Ferramentas de Linha de Comando do Microsoft Azure | Sim |
| [healthcareapis](https://github.com/Azure/azure-cli-extensions) | 0.1.2 | Extensão HealthCareApis das Ferramentas de Linha de Comando do Microsoft Azure |  |
| [image-copy-extension](https://github.com/Azure/azure-cli-extensions) | 0.2.3 | Suporte para copiar imagens de vm gerenciadas entre regiões |  |
| [interativo](https://github.com/Azure/azure-cli) | 0.4.3 | Shell interativo de linha de comando do Microsoft Azure | Sim |
| [internet-analyzer](https://github.com/Azure/azure-cli-extensions) | 0.1.0rc4 | Extensão Analisador de Internet das Ferramentas de Linha de Comando do Microsoft Azure | Sim |
| [ip-group](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Extensão IpGroup das Ferramentas de Linha de Comando do Microsoft Azure |  |
| [keyvault-preview](https://github.com/Azure/azure-keyvault-cli-extension) | 0.1.3 | Visualizar comandos do Azure Key Vault. | Sim |
| [log-analytics](https://github.com/Azure/azure-cli-extensions/tree/master/src/log-analytics) | 0.1.4 | Suporte para recursos de consulta do Log Analytics do Azure. | Sim |
| [manutenção](https://github.com/Azure/azure-cli-extensions) | 1.0.0 | Suporte para a versão prévia de gerenciamento de manutenção do Azure. | Sim |
| [managementgroups](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Uma extensão da CLI do Azure para grupos de gerenciamento |  |
| [managementpartner](https://github.com/Azure/azure-cli-extensions) | 0.1.2 | Suporte à versão prévia de Parceiro de Gerenciamento |  |
| [malha](https://github.com/Azure/azure-cli-extensions) | 0.10.6 | Suporte para a Malha do Microsoft Azure Service Fabric - Visualização Pública | Sim |
| [mixed-reality](https://github.com/Azure/azure-cli-extensions) | 0.0.1 | Extensão da CLI da Realidade Misturada do Azure. |  |
| [netappfiles-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/netappfiles-preview) | 0.3.2 | Fornece uma versão prévia para os futuros recursos do ANF (Azure NetApp Files). | Sim |
| [notification-hub](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Extensão Hub de Notificações de Ferramentas de Linha de Comando do Microsoft Azure | Sim |
| [peering](https://github.com/Azure/azure-cli-extensions) | 0.1.0rc1 | Extensão de Emparelhamento das Ferramentas de Linha de Comando do Microsoft Azure | Sim |
| [privatedns](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Comandos para gerenciar zonas DNS privadas | Sim |
| [resource-graph](https://github.com/Azure/azure-cli-extensions/tree/master/src/resource-graph) | 1.0.0 | Suporte para consultar recursos do Azure com o Resource Graph. |  |
| [sap-hana](https://github.com/Azure/azure-hanaonazure-cli-extension) | 0.5.5 | Comandos adicionais para trabalhar com instâncias do SAP HanaOnAzure. |  |
| [spring-cloud](https://github.com/Azure/azure-cli-extensions) | 0.2.0 | Extensão spring-cloud das Ferramentas de Linha de Comando do Microsoft Azure | Sim |
| [storage-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/storage-preview) | 0.2.10 | Fornece uma visualização para recursos de armazenamento futuras. | Sim |
| [subscription](https://github.com/Azure/azure-cli-extensions) | 0.1.3 | Suporte à versão prévia de gerenciamento de assinatura. |  |
| [support](https://github.com/azure/azure-cli-extensions/tree/master/src/support) | 0.1.0 | Extensão Suporte das Ferramentas de Linha de Comando do Microsoft Azure | Sim |
| [virtual-network-tap](https://github.com/Azure/azure-cli-extensions/tree/master/src/virtual-network-tap) | 0.1.0 | Gerenciar TAPs de rede virtual (VTAP). | Sim |
| [virtual-wan](https://github.com/Azure/azure-cli-extensions/tree/master/src/virtual-wan) | 0.1.2 | Gerencie WAN virtual, hubs, gateways de VPN e sites VPN. | Sim |
| [vm-repair](https://github.com/Azure/azure-cli-extensions/tree/master/src/vm-repair) | 0.2.5 | Comandos de reparo automático para corrigir as VMs. |  |
| [vmware-cs](https://github.com/Azure/az-vmware-cli) | 0.2.0 | Gerenciar a solução VMware no Azure. | Sim |
| [webapp](https://github.com/Azure/azure-cli-extensions/tree/master/src/webapp) | 0.2.24 | Comandos adicionais para o Serviço de Aplicativo do Azure. | Sim |