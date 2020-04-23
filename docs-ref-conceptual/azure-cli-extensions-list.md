---
title: Extensões disponíveis para a CLI do Azure
description: Uma lista completa das extensões com suporte oficial para a CLI do Azure.
author: haroldrandom
ms.author: jianzen
manager: yonzhan,yungezz
ms.date: 04/16/2020
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 531ea056b276cc12d5807ed62baa4d3c6044c26e
ms.sourcegitcommit: 89ec9fa7ebd2170b55201cd51fb386fd9351d7ca
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2020
ms.locfileid: "81728570"
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
| [ai-examples](https://github.com/Azure/azure-cli-extensions/tree/master/src/ai-examples) | 0.2.0 | Adicione exemplos de IA fornecidos ao conteúdo da ajuda. | Sim |
| [versão prévia do aks](https://github.com/Azure/azure-cli-extensions/tree/master/src/aks-preview) | 0.4.43 | Fornece uma versão prévia para futuros recursos do AKS | Sim |
| [alertsmanagement](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Extensão de alertas das ferramentas de linha de comando do Microsoft Azure |  |
| [alias](https://github.com/Azure/azure-cli-extensions) | 0.5.2 | Suporte para aliases de comando | Sim |
| [application-insights](https://github.com/Azure/azure-cli-extensions/tree/master/src/application-insights) | 0.1.6 | Suporte para gerenciar componentes do Application Insights e consultar as métricas, os eventos e os logs de tais componentes. | Sim |
| [azure-batch-cli-extensions](https://github.com/Azure/azure-batch-cli-extensions) | 5.0.1 | Comandos adicionais para trabalhar com o serviço de Lote do Azure |  |
| [azure-cli-iot-ext](https://github.com/azure/azure-iot-cli-extension) | 0.8.9 | A extensão de IoT do Azure para a CLI do Azure. |  |
| [azure-cli-ml](https://docs.microsoft.com/azure/machine-learning/service/) | 1.3.0 | Módulo de Comando do AzureML para as Ferramentas da Linha de Comando do Microsoft Azure |  |
| [azure-devops](https://github.com/Microsoft/azure-devops-cli-extension) | 0.18.0 | Ferramentas para gerenciar o Azure DevOps. |  |
| [azure-firewall](https://github.com/Azure/azure-cli-extensions/tree/master/src/azure-firewall) | 0.3.1 | Gerenciar recursos do Firewall do Azure. | Sim |
| [azure-iot](https://github.com/azure/azure-iot-cli-extension) | 0.9.1 | A extensão de IoT do Azure para a CLI do Azure. |  |
| [blueprint](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Extensão Blueprint das Ferramentas de Linha de Comando do Microsoft Azure |  |
| [connectedmachine](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Extensão Connectedmachine das Ferramentas de Linha de Comando do Microsoft Azure | Sim |
| [connection-monitor-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/connection-monitor-preview) | 0.1.0 | Extensão Monitor de Conexão de Linha de Comando do Microsoft Azure V2 | Sim |
| [csvmware](https://github.com/Azure/az-vmware-cli) | 0.3.0 | Gerencie a Solução VMware da CloudSimple no Azure. | Sim |
| [databox](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Extensão DataBox das ferramentas de linha de comando do Microsoft Azure |  |
| [databricks](https://github.com/Azure/azure-cli-extensions) | 0.2.0 | Extensão DatabricksClient das Ferramentas de Linha de Comando do Microsoft Azure |  |
| [db-up](https://github.com/Azure/azure-cli-extensions/tree/master/src/db-up) | 0.1.13 | Comandos adicionais para simplificar os fluxos de trabalho do Banco de Dados do Azure. | Sim |
| [deploy-to-azure](https://github.com/Azure/deploy-to-azure-cli-extension) | 0.2.0 | Implante no Azure com o Github Actions. | Sim |
| [dev-spaces](https://github.com/Azure/azure-cli-extensions) | 1.0.5 | Os Espaços de Desenvolvimento fornecem uma experiência de desenvolvimento Kubernetes rápida e iterativa para equipes. |  |
| [dev-spaces-preview](https://github.com/Azure/azure-cli-extensions) | 0.1.6 | Os Espaços de Desenvolvimento fornecem uma experiência de desenvolvimento Kubernetes rápida e iterativa para equipes. | Sim |
| [dms-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/dms-preview) | 0.11.0 | Suporte para novos cenários do Serviço de Migração de Banco de Dados. | Sim |
| [eventgrid](https://github.com/Azure/azure-cli-extensions) | 0.4.7 | Módulo de Comando do EventGrid para as Ferramentas da Linha de Comando do Microsoft Azure. | Sim |
| [express-route](https://github.com/Azure/azure-cli-extensions/tree/master/src/express-route) | 0.1.3 | Gerenciar ExpressRoute com versão prévia dos recursos. | Sim |
| [express-route-cross-connection](https://github.com/Azure/azure-cli-extensions/tree/master/src/express-route-cross-connection) | 0.1.1 | Gerencie os circuitos do ExpressRoute de cliente usando uma conexão cruzada do ExpressRoute. |  |
| [front-door](https://github.com/Azure/azure-cli-extensions/tree/master/src/front-door) | 1.0.6 | Gerenciar FrontDoors de rede. |  |
| [hack](https://github.com/Azure/azure-cli-extensions) | 0.4.2 | Extensão Hack das Ferramentas de Linha de Comando do Microsoft Azure | Sim |
| [healthcareapis](https://github.com/Azure/azure-cli-extensions) | 0.1.3 | Extensão HealthCareApis das Ferramentas de Linha de Comando do Microsoft Azure |  |
| [hpc-cache](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Extensão StorageCache das ferramentas de linha de comando do Microsoft Azure | Sim |
| [image-copy-extension](https://github.com/Azure/azure-cli-extensions) | 0.2.3 | Suporte para copiar imagens de vm gerenciadas entre regiões |  |
| [interativo](https://github.com/Azure/azure-cli) | 0.4.4 | Shell interativo de linha de comando do Microsoft Azure | Sim |
| [internet-analyzer](https://github.com/Azure/azure-cli-extensions) | 0.1.0rc5 | Extensão Analisador de Internet das Ferramentas de Linha de Comando do Microsoft Azure | Sim |
| [ip-group](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Extensão IpGroup das Ferramentas de Linha de Comando do Microsoft Azure |  |
| [keyvault-preview](https://github.com/Azure/azure-keyvault-cli-extension) | 0.1.3 | Visualizar comandos do Azure Key Vault. | Sim |
| [log-analytics](https://github.com/Azure/azure-cli-extensions/tree/master/src/log-analytics) | 0.1.4 | Suporte para recursos de consulta do Log Analytics do Azure. | Sim |
| [manutenção](https://github.com/Azure/azure-cli-extensions) | 1.0.1 | Suporte para o gerenciamento de manutenção do Azure. |  |
| [managementpartner](https://github.com/Azure/azure-cli-extensions) | 0.1.2 | Suporte à versão prévia de Parceiro de Gerenciamento |  |
| [malha](https://github.com/Azure/azure-cli-extensions) | 0.10.6 | Suporte para a Malha do Microsoft Azure Service Fabric - Visualização Pública | Sim |
| [mixed-reality](https://github.com/Azure/azure-cli-extensions) | 0.0.1 | Extensão da CLI da Realidade Misturada do Azure. |  |
| [netappfiles-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/netappfiles-preview) | 0.3.2 | Fornece uma versão prévia para os futuros recursos do ANF (Azure NetApp Files). | Sim |
| [notification-hub](https://github.com/Azure/azure-cli-extensions) | 0.2.0 | Extensão Hub de Notificações de Ferramentas de Linha de Comando do Microsoft Azure |  |
| [peering](https://github.com/Azure/azure-cli-extensions) | 0.1.0rc2 | Extensão de Emparelhamento das Ferramentas de Linha de Comando do Microsoft Azure | Sim |
| [powerbidedicated](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Extensão PowerBIDedicated das Ferramentas da Linha de Comando do Microsoft Azure | Sim |
| [privatedns](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Comandos para gerenciar zonas DNS privadas | Sim |
| [resource-graph](https://github.com/Azure/azure-cli-extensions/tree/master/src/resource-graph) | 1.1.0 | Suporte para consultar recursos do Azure com o Resource Graph. | Sim |
| [sap-hana](https://github.com/Azure/azure-hanaonazure-cli-extension) | 0.5.9 | Comandos adicionais para trabalhar com instâncias do SAP HanaOnAzure. |  |
| [spring-cloud](https://github.com/Azure/azure-cli-extensions) | 0.2.2 | Extensão spring-cloud das Ferramentas de Linha de Comando do Microsoft Azure | Sim |
| [storage-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/storage-preview) | 0.2.10 | Fornece uma visualização para recursos de armazenamento futuras. | Sim |
| [storagesync](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Extensão MicrosoftStorageSync das ferramentas de linha de comando do Microsoft Azure |  |
| [stream-analytics](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Extensão stream-analytics das ferramentas de linha de comando do Microsoft Azure |  |
| [subscription](https://github.com/Azure/azure-cli-extensions) | 0.1.3 | Suporte à versão prévia de gerenciamento de assinatura. |  |
| [support](https://github.com/azure/azure-cli-extensions/tree/master/src/support) | 1.0.1 | Extensão Suporte das Ferramentas de Linha de Comando do Microsoft Azure |  |
| [synapse](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Extensão do Synapse das Ferramentas da Linha de Comando do Microsoft Azure | Sim |
| [virtual-network-tap](https://github.com/Azure/azure-cli-extensions/tree/master/src/virtual-network-tap) | 0.1.0 | Gerenciar TAPs de rede virtual (VTAP). | Sim |
| [virtual-wan](https://github.com/Azure/azure-cli-extensions/tree/master/src/virtual-wan) | 0.1.3 | Gerencie WAN virtual, hubs, gateways de VPN e sites VPN. | Sim |
| [vm-repair](https://github.com/Azure/azure-cli-extensions/tree/master/src/vm-repair) | 0.2.6 | Comandos de reparo automático para corrigir as VMs. |  |
| [vmware](https://github.com/virtustream/azure-vmware-virtustream-cli-extension) | 0.5.5 | Versão prévia dos comandos da Solução Azure VMware da Virtustream. | Sim |
| [webapp](https://github.com/Azure/azure-cli-extensions/tree/master/src/webapp) | 0.2.24 | Comandos adicionais para o Serviço de Aplicativo do Azure. | Sim |