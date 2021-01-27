---
title: Extensões disponíveis para a CLI do Azure
description: Uma lista completa das extensões com suporte oficial para a CLI do Azure.
author: haroldrandom
ms.author: jianzen
manager: yonzhan,yungezz
ms.date: 01/01/2021
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 0dd2dbcf6d290e2a1309e150da5a37e57bc99f78
ms.sourcegitcommit: 2a0ae2ffc14ce325f9adb9c09d6b5eac534df8a6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2021
ms.locfileid: "98887062"
---
# <a name="available-extensions-for-the-azure-cli"></a>Extensões disponíveis para a CLI do Azure

Este artigo é uma lista completa das extensões disponíveis para a CLI do Azure que têm suporte da Microsoft.

A lista de extensões também está disponível na CLI. Para obtê-la, execute [az extension list-available](/cli/azure/extension#az-extension-list-available):

```azurecli-interactive
az extension list-available --output table
```

| Nome | Versão | Resumo | Visualização |
|------|---------|---------|---------|
| [conta](https://github.com/Azure/azure-cli-extensions/tree/master/src/account) | 0.2.1 | Extensão SubscriptionClient das ferramentas de linha de comando do Microsoft Azure |  |
| [aem](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Gerenciar Extensões de Monitoramento Aprimorado do Azure para SAP |  |
| [ai-examples](https://github.com/Azure/azure-cli-extensions/tree/master/src/ai-examples) | 0.2.5 | Adicione exemplos de IA fornecidos ao conteúdo da ajuda. | Sim |
| [versão prévia do aks](https://github.com/Azure/azure-cli-extensions/tree/master/src/aks-preview) | 0.4.71 | Fornece uma versão prévia para futuros recursos do AKS | Sim |
| [alertsmanagement](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Extensão de alertas das ferramentas de linha de comando do Microsoft Azure |  |
| [alias](https://github.com/Azure/azure-cli-extensions) | 0.5.2 | Suporte para aliases de comando | Sim |
| [application-insights](https://github.com/Azure/azure-cli-extensions/tree/master/src/application-insights) | 0.1.13 | Suporte para gerenciar componentes do Application Insights e consultar as métricas, os eventos e os logs de tais componentes. | Sim |
| [attestation](https://github.com/Azure/azure-cli-extensions/tree/master/src/attestation) | 0.2.0 | Extensão AttestationManagementClient das ferramentas de linha de comando do Microsoft Azure |  |
| [automation](https://github.com/Azure/azure-cli-extensions/tree/master/src/automation) | 0.1.0 | Extensão AutomationClient das ferramentas de linha de comando do Microsoft Azure |  |
| [azure-batch-cli-extensions](https://github.com/Azure/azure-batch-cli-extensions) | 6.0.0 | Comandos adicionais para trabalhar com o serviço de Lote do Azure |  |
| [azure-cli-iot-ext](https://github.com/azure/azure-iot-cli-extension) | 0.8.10 | Preterido: remova a “azure-cli-iot-ext” e instale a extensão “azure-iot” no lugar dela. A extensão herdada “azure-cli-iot-ext” está agendada para remoção após 15/09/2020. |  |
| [azure-cli-ml](/python/api/overview/azure/ml/?view=azure-ml-py) | 1.19.0 | Módulo de Comando do AzureML para as Ferramentas da Linha de Comando do Microsoft Azure |  |
| [azure-devops](https://github.com/Microsoft/azure-devops-cli-extension) | 0.18.0 | Ferramentas para gerenciar o Azure DevOps. |  |
| [azure-firewall](https://github.com/Azure/azure-cli-extensions/tree/master/src/azure-firewall) | 0.8.0 | Gerenciar recursos do Firewall do Azure. | Sim |
| [azure-iot](https://github.com/azure/azure-iot-cli-extension) | 0.10.8 | A extensão de IoT do Azure para a CLI do Azure. |  |
| [baremetal-infrastructure](https://github.com/Azure/azure-baremetalinfrastructure-cli-extension) | 0.0.2 | Comandos adicionais para trabalhar com instâncias de BareMetal. |  |
| [blockchain](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Extensão BlockchainManagementClient das ferramentas de linha de comando do Microsoft Azure |  |
| [blueprint](https://github.com/Azure/azure-cli-extensions/tree/master/src/blueprint) | 0.2.1 | Extensão Blueprint das Ferramentas de Linha de Comando do Microsoft Azure |  |
| [cli-translator](https://github.com/Azure/azure-cli-extensions/tree/master/src/cli-translator) | 0.3.0 | Converta o modelo do ARM em scripts da CLI do Azure executáveis. |  |
| [codespaces](https://github.com/Azure/azure-cli-extensions) | 0.3.0 | A extensão Codespaces da CLI do Azure | Sim |
| [communication](https://github.com/Azure/azure-cli-extensions/tree/master/src/communication) | 0.1.0 | Extensão CommunicationServiceManagementClient das ferramentas de linha de comando do Microsoft Azure |  |
| [connectedk8s](https://github.com/Azure/azure-cli-extensions/tree/master/src/connectedk8s) | 0.2.8 | Extensão connectedk8s das ferramentas de linha de comando do Microsoft Azure | Sim |
| [connectedmachine](https://github.com/Azure/azure-cli-extensions/tree/master/src/connectedmachine) | 0.3.0 | Extensão ConnectedMachine das ferramentas de linha de comando do Microsoft Azure |  |
| [connection-monitor-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/connection-monitor-preview) | 0.1.0 | Extensão Monitor de Conexão de Linha de Comando do Microsoft Azure V2 | Sim |
| [costmanagement](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Extensão CostManagementClient das Ferramentas de Linha de Comando do Microsoft Azure |  |
| [csvmware](https://github.com/Azure/az-vmware-cli) | 0.3.0 | Gerencie a Solução VMware da CloudSimple no Azure. | Sim |
| [custom-providers](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Extensão personalizada dos provedores das ferramentas de linha de comando do Microsoft Azure |  |
| [databox](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Extensão DataBox das ferramentas de linha de comando do Microsoft Azure |  |
| [databricks](https://github.com/Azure/azure-cli-extensions) | 0.7.0 | Extensão DatabricksClient das Ferramentas de Linha de Comando do Microsoft Azure |  |
| [datafactory](https://github.com/Azure/azure-cli-extensions/tree/master/src/datafactory) | 0.2.0 | Extensão DataFactoryManagementClient das Ferramentas de Linha de Comando do Microsoft Azure |  |
| [datashare](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Extensão DataShareManagementClient das ferramentas de linha de comando do Microsoft Azure |  |
| [db-up](https://github.com/Azure/azure-cli-extensions/tree/master/src/db-up) | 0.2.0 | Comandos adicionais para simplificar os fluxos de trabalho do Banco de Dados do Azure. | Sim |
| [deploy-to-azure](https://github.com/Azure/deploy-to-azure-cli-extension) | 0.2.0 | Implante no Azure com o Github Actions. | Sim |
| [desktopvirtualization](https://github.com/Azure/azure-cli-extensions/tree/master/src/desktopvirtualization) | 0.1.0 | Extensão DesktopVirtualizationAPIClient das ferramentas de linha de comando do Microsoft Azure |  |
| [dev-spaces](https://github.com/Azure/azure-cli-extensions/tree/master/src/dev-spaces) | 1.0.6 | Os Espaços de Desenvolvimento fornecem uma experiência de desenvolvimento Kubernetes rápida e iterativa para equipes. |  |
| [dev-spaces-preview](https://github.com/Azure/azure-cli-extensions) | 0.1.6 | Os Espaços de Desenvolvimento fornecem uma experiência de desenvolvimento Kubernetes rápida e iterativa para equipes. | Sim |
| [dms-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/dms-preview) | 0.12.0 | Suporte para novos cenários do Serviço de Migração de Banco de Dados. | Sim |
| [eventgrid](https://github.com/Azure/azure-cli-extensions) | 0.4.9 | Módulo de Comando do EventGrid para as Ferramentas da Linha de Comando do Microsoft Azure. | Sim |
| [express-route](https://github.com/Azure/azure-cli-extensions/tree/master/src/express-route) | 0.1.3 | Gerenciar ExpressRoute com versão prévia dos recursos. | Sim |
| [express-route-cross-connection](https://github.com/Azure/azure-cli-extensions/tree/master/src/express-route-cross-connection) | 0.1.1 | Gerencie os circuitos do ExpressRoute de cliente usando uma conexão cruzada do ExpressRoute. |  |
| [footprint](https://github.com/Azure/azure-cli-extensions/tree/master/src/footprint) | 1.0.0 | Extensão FootprintMonitoringManagementClient das ferramentas de linha de comando do Microsoft Azure |  |
| [front-door](https://github.com/Azure/azure-cli-extensions/tree/master/src/front-door) | 1.0.9 | Gerenciar FrontDoors de rede. |  |
| [fzf](https://github.com/phealy/azure-cli-fzf) | 1.0.2 | Extensão fzf das ferramentas de linha de comando do Microsoft Azure |  |
| [guestconfig](https://github.com/Azure/azure-cli-extensions/tree/master/src/guestconfig) | 0.1.0 | Extensão GuestConfigurationClient de ferramentas de linha de comando do Microsoft Azure |  |
| [hack](https://github.com/Azure/azure-cli-extensions/tree/master/src/hack) | 0.4.3 | Extensão Hack das Ferramentas de Linha de Comando do Microsoft Azure | Sim |
| [hardware-security-modules](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Extensão AzureDedicatedHSMResourceProvider das Ferramentas de Linha de Comando do Microsoft Azure |  |
| [healthcareapis](https://github.com/Azure/azure-cli-extensions/tree/master/src/healthcareapis) | 0.3.0 | Extensão HealthcareApisManagementClient das ferramentas de linha de comando do Microsoft Azure |  |
| [hpc-cache](https://github.com/Azure/azure-cli-extensions/tree/master/src/hpc-cache) | 0.1.2 | Extensão StorageCache das ferramentas de linha de comando do Microsoft Azure | Sim |
| [image-copy-extension](https://github.com/Azure/azure-cli-extensions/tree/master/src/image-copy) | 0.2.8 | Suporte para copiar imagens de vm gerenciadas entre regiões |  |
| [import-export](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Extensão StorageImportExport das ferramentas de linha de comando do Microsoft Azure |  |
| [interativo](https://github.com/Azure/azure-cli) | 0.4.4 | Shell interativo de linha de comando do Microsoft Azure | Sim |
| [internet-analyzer](https://github.com/Azure/azure-cli-extensions) | 0.1.0rc5 | Extensão Analisador de Internet das Ferramentas de Linha de Comando do Microsoft Azure | Sim |
| [ip-group](https://github.com/Azure/azure-cli-extensions) | 0.1.2 | Extensão IpGroup das Ferramentas de Linha de Comando do Microsoft Azure | Sim |
| [k8sconfiguration](https://github.com/Azure/azure-cli-extensions/tree/master/src/k8sconfiguration) | 0.2.2 | Extensão k8sconfiguration das ferramentas de linha de comando do Microsoft Azure | Sim |
| [keyvault-preview](https://github.com/Azure/azure-keyvault-cli-extension) | 0.1.3 | Visualizar comandos do Azure Key Vault. | Sim |
| [kusto](https://github.com/Azure/azure-cli-extensions/tree/master/src/kusto) | 0.2.0 | Extensão KustoManagementClient das ferramentas de linha de comando do Microsoft Azure |  |
| [log-analytics](https://github.com/Azure/azure-cli-extensions/tree/master/src/log-analytics) | 0.2.1 | Suporte para recursos de consulta do Log Analytics do Azure. | Sim |
| [log-analytics-solution](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Suporte para Solução Log Analytics do Azure |  |
| [logic](https://github.com/Azure/azure-cli-extensions/tree/master/src/logic) | 0.1.2 | Extensão LogicManagementClient das ferramentas de linha de comando do Microsoft Azure |  |
| [manutenção](https://github.com/Azure/azure-cli-extensions/tree/master/src/maintenance) | 1.1.0 | Extensão MaintenanceClient das ferramentas de linha de comando do Microsoft Azure | Sim |
| [managementpartner](https://github.com/Azure/azure-cli-extensions) | 0.1.3 | Suporte à versão prévia de Parceiro de Gerenciamento |  |
| [malha](https://github.com/Azure/azure-cli-extensions) | 0.10.6 | Suporte para a Malha do Microsoft Azure Service Fabric - Visualização Pública | Sim |
| [mixed-reality](https://github.com/Azure/azure-cli-extensions) | 0.0.2 | Extensão da CLI da Realidade Misturada do Azure. | Sim |
| [netappfiles-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/netappfiles-preview) | 0.3.2 | Fornece uma versão prévia para os futuros recursos do ANF (Azure NetApp Files). | Sim |
| [notification-hub](https://github.com/Azure/azure-cli-extensions) | 0.2.0 | Extensão Hub de Notificações de Ferramentas de Linha de Comando do Microsoft Azure |  |
| [peering](https://github.com/Azure/azure-cli-extensions) | 0.2.0 | Extensão PeeringManagementClient das ferramentas de linha de comando do Microsoft Azure |  |
| [portal](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Extensão do portal das ferramentas de linha de comando do Microsoft Azure |  |
| [powerbidedicated](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Extensão PowerBIDedicated das Ferramentas da Linha de Comando do Microsoft Azure | Sim |
| [privatedns](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Comandos para gerenciar zonas DNS privadas | Sim |
| [resource-graph](https://github.com/Azure/azure-cli-extensions/tree/master/src/resource-graph) | 1.1.0 | Suporte para consultar recursos do Azure com o Resource Graph. | Sim |
| [sap-hana](https://github.com/Azure/azure-hanaonazure-cli-extension) | 0.6.4 | Comandos adicionais para trabalhar com instâncias do SAP HanaOnAzure. |  |
| [scheduled-query](https://github.com/Azure/azure-cli-extensions) | 0.2.0 | Extensão Scheduled_query das ferramentas de linha de comando do Microsoft Azure | Sim |
| [sentinel](https://github.com/Azure/azure-cli-extensions/tree/master/src/sentinel) | 0.1.0 | Extensão SecurityInsights das ferramentas de linha de comando do Microsoft Azure |  |
| [spring-cloud](https://github.com/Azure/azure-cli-extensions/tree/master/src/spring-cloud) | 2.1.0 | Extensão spring-cloud das Ferramentas de Linha de Comando do Microsoft Azure |  |
| [ssh](https://github.com/Azure/azure-cli-extensions/tree/master/src/ssh) | 0.1.0 | SSH em VMs | Sim |
| [stack-hci](https://github.com/Azure/azure-cli-extensions/tree/master/src/stack-hci) | 0.1.1 | Extensão AzureStackHCIClient das ferramentas de linha de comando do Microsoft Azure |  |
| [storage-blob-preview](https://github.com/Azure/azure-cli-extensions) | 0.4.0 | Extensão Storage-blob-preview das ferramentas da linha de comando do Microsoft Azure | Sim |
| [storage-or-preview](https://github.com/Azure/azure-cli-extensions) | 0.4.0 | Extensão storage-ors-preview das ferramentas da linha de comando do Microsoft Azure | Sim |
| [storage-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/storage-preview) | 0.7.0 | Fornece uma visualização para recursos de armazenamento futuras. | Sim |
| [storagesync](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Extensão MicrosoftStorageSync das ferramentas de linha de comando do Microsoft Azure |  |
| [stream-analytics](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Extensão stream-analytics das ferramentas de linha de comando do Microsoft Azure |  |
| [subscription](https://github.com/Azure/azure-cli-extensions) | 0.1.4 | Suporte à versão prévia de gerenciamento de assinatura. | Sim |
| [support](https://github.com/azure/azure-cli-extensions/tree/master/src/support) | 1.0.2 | Extensão Suporte das Ferramentas de Linha de Comando do Microsoft Azure |  |
| [synapse](https://github.com/Azure/azure-cli-extensions) | 0.3.0 | Extensão do Synapse das Ferramentas da Linha de Comando do Microsoft Azure | Sim |
| [timeseriesinsights](https://github.com/Azure/azure-cli-extensions/src/timeseriesinsights) | 0.1.3 | Extensão TimeSeriesInsightsClient das ferramentas de linha de comando do Microsoft Azure |  |
| [virtual-network-tap](https://github.com/Azure/azure-cli-extensions/tree/master/src/virtual-network-tap) | 0.1.0 | Gerenciar TAPs de rede virtual (VTAP). | Sim |
| [virtual-wan](https://github.com/Azure/azure-cli-extensions/tree/master/src/virtual-wan) | 0.2.3 | Gerencie WAN virtual, hubs, gateways de VPN e sites VPN. | Sim |
| [vm-repair](https://github.com/Azure/azure-cli-extensions/tree/master/src/vm-repair) | 0.3.4 | Comandos de reparo automático para corrigir as VMs. |  |
| [vmware](https://github.com/Azure/az-vmware-cli) | 1.0.0 | Comandos da Solução VMware no Azure. |  |
| [webapp](https://github.com/Azure/azure-cli-extensions/tree/master/src/webapp) | 0.2.24 | Comandos adicionais para o Serviço de Aplicativo do Azure. | Sim |