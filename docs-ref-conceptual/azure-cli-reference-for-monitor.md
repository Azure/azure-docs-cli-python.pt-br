---
title: Referências da CLI do Azure para o Azure Monitor
description: Página de aterrissagem da referência da CLI do Azure para o Azure Monitor
author: dbradish-microsoft
manager: barbkess
ms.devlang: azurecli
ms.topic: reference
ms.date: 06/30/2020
ms.author: dbradish
ms.service: azure-cli
ms.reviewer: robb
ms.custom: devx-track-azurecli
ms.openlocfilehash: d16c745656b3d92942e66cfbcb6764d219d971ec
ms.sourcegitcommit: 5d29362589078b66d15f5cd494fe903a5195658d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/25/2020
ms.locfileid: "91225432"
---
# <a name="azure-cli-for-azure-monitor"></a>CLI do Azure para Azure Monitor

A [CLI do Azure](./what-is-azure-cli.md) (Interface de Linha de Comando do Azure) é um conjunto de comandos usados para criar e gerenciar recursos do Azure.  Ela está disponível em muitos serviços do Azure, incluindo o Azure Monitor.  Há mais de 100 referências para o Azure Monitor, que possibilitam que você trabalhe de maneira eficaz com os serviços de monitor usando uma linha de comando.

## <a name="references-for-azure-monitor"></a>Referências para o Azure Monitor

A experiência da CLI do [Azure Monitor](/azure/azure-monitor/) é composta por duas partes: A CLI do Azure (também chamada de CLI **principal**) e a **extensão** da CLI do Azure Monitor.  As referências de extensão da CLI do Azure devem ser instaladas antes do uso. O comando [az extension add](/cli/azure/extension?view=azure-cli-latest#az-extension-add) instala uma referência de extensão por nome.

> [!IMPORTANT]
>
> O Azure Monitor agora inclui o Application Insights e o Log Analytics. Dessa forma, você deve instalar as extensões para cada subárea ao trabalhar com a CLI do Azure Monitor.

### <a name="references"></a>Referências

| Referência | Instalar a extensão | Descrição | Para obter mais informações, consulte
|-|-|-|-|
| [az monitor](/cli/azure/monitor) | | O grupo de comandos de nível superior para todos os comandos da CLI do Azure para o Azure Monitor. | [Visão geral do Azure Monitor](/azure/azure-monitor/overview)
| [az monitor action-group](/cli/azure/monitor/action-group) | | Gerenciar grupos de ações, que se relacionam a notificações depois que um alerta é disparado. | [Alertas do Azure Monitor](/azure/azure-monitor/platform/alerts-overview)
| [az monitor activity-log](/cli/azure/monitor/activity-log) | | Gerenciar o log de atividades, incluindo alertas do log de atividades. | [Logs de atividades do Azure](/azure/azure-monitor/platform/activity-log)
| [az monitor alert](/cli/azure/monitor/alert) | | NÃO USE para uma nova implantação.  Esse comando gerencia as regras de alerta clássicas baseadas em métricas mais antigas que, exceto em alguns casos, foram migradas para os tipos de alertas de métrica mais recentes. Em vez disso, use [az monitor metrics alert](/cli/azure/monitor/metrics/alert). |
| [az monitor app-insights](/cli/azure/ext/application-insights/monitor/app-insights) | sim | Gerenciar o Application Insights para monitoramento de aplicativos. | [Visão geral do Application Insights](/azure/azure-monitor/app/app-insights-overview)
| [az monitor autoscale](/cli/azure/monitor/autoscale) | | Gerenciar configurações de dimensionamento automático. | [Visão geral do dimensionamento automático](/azure/azure-monitor/platform/autoscale-overview)
| [az monitor diagnostic-settings](/cli/azure/monitor/diagnostic-settings) | | Gerencie as configurações de diagnóstico do serviço, que configuram a coleta e o roteamento de muitos tipos de métricas e logs de plataforma. | [Criar configurações de diagnóstico](/azure/azure-monitor/platform/diagnostic-settings)
| [az monitor log-analytics](/cli/azure/monitor/log-analytics) | | Gerenciar clusters de log e workspaces. | [Criar sua implantação de Logs do Azure Monitor](/azure/azure-monitor/platform/design-logs-deployment)
| [az monitor log-analytics query](/cli/azure/ext/log-analytics/monitor/log-analytics#ext-log-analytics-az-monitor-log-analytics-query) | sim | Comandos para consultar dados em workspaces do Log Analytics.  | [Introdução às consultas do Log Analytics](/azure/azure-monitor/log-query/get-started-portal)
| [az monitor log-profiles](/cli/azure/monitor/log-profiles) | | NÃO USE para uma nova implantação.  Esse comando foi usado anteriormente para rotear logs de atividade para Log do Azure Monitor e para o Log Analytics.  Em vez disso, use [configuração de diagnóstico](/azure/azure-monitor/platform/diagnostic-settings).  | [Enviar o log de atividades para o workspace do Log Analytics](/azure/azure-monitor/platform/activity-log#send-to-log-analytics-workspace)
| [az monitor metrics](/cli/azure/monitor/metrics) | | Gerencie métricas de plataforma e regras de alerta de métrica quase em tempo real. | [Visão geral de métricas no Azure Monitor](/azure/azure-monitor/platform/data-platform-metrics) e [Entender como os alertas de métrica funcionam](/azure/azure-monitor/platform/alerts-metric-overview)
| [az monitor private-link-scope](/cli/azure/monitor/private-link-scope) | | Gerenciar o recurso do escopo de link privado do monitor. | [Usar o Link Privado do Azure para conectar redes com segurança ao Azure Monitor](/azure/azure-monitor/platform/private-link-security)

### <a name="installing-extension-references"></a>Instalar referências de extensão

As referências de extensão da CLI do Azure devem ser instaladas antes do uso.  O comando [az extension add](./azure-cli-extensions-overview.md) instala uma referência de extensão por nome.

```azurecli
# install the extension for az monitor app-insights
az extension add --name application-insights

# install the extension for az monitor log-analytics
az extension add --name log-analytics
```

## <a name="popular-monitor-articles-using-the-azure-cli"></a>Artigos populares do Monitor que usam a CLI do Azure

- [Exemplos de CLI do Azure Monitor](/azure/azure-monitor/samples/cli-samples)
- [Criar um workspace do Log Analytics com a CLI do Azure 2.0](/azure/azure-monitor/learn/quick-create-workspace-cli)

## <a name="azure-cli-reference-examples"></a>Exemplos de referência da CLI do Azure

São fornecidos exemplos com todas as referências da CLI do Azure. Embora você também possa concluir essas tarefas no portal do Azure, usar a CLI do Azure requer uma só linha de comando.  Veja alguns exemplos de código para ter uma ideia de como é fácil usar a CLI do Azure.

Para trabalhar com o Azure Monitor, primeiro você precisará de um grupo de recursos.  Os grupos de recursos do Azure são simples de criar e gerenciar com a CLI do Azure.  

```azurecli
#create a resource group
az group create -location westus -name MyResourceGroup

#get a list of resource groups for a subscription
az group list --subscription MySubscription --output table
```

Criar um alerta de log do Azure Monitor é muito simples.

```azurecli
#create an Azure Monitor activity log alert
az monitor activity-log alert create --name MyAlertName --resource-group MyResourceGroup
```

## <a name="see-also"></a>Confira também

- [Introdução à CLI do Azure](./get-started-with-azure-cli.md) para saber mais sobre a instalação e a conexão.

- Descubra referências adicionais [lançadas](/cli/azure/reference-index) e de [extensão](./azure-cli-extensions-list.md) na documentação da CLI do Azure.

- Saiba mais sobre as referências de extensão em [Usar extensões com a CLI do Azure](./azure-cli-extensions-overview.md).