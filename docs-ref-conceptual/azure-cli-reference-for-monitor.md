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
ms.openlocfilehash: 064ba33fb9c10043d7b68e472a53332f44ac1283
ms.sourcegitcommit: 857d0f19fd87d37d134efdf0dda0e7003260938b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "86308705"
---
# <a name="azure-cli-for-azure-monitor"></a><span data-ttu-id="08cc3-103">CLI do Azure para Azure Monitor</span><span class="sxs-lookup"><span data-stu-id="08cc3-103">Azure CLI for Azure Monitor</span></span>

<span data-ttu-id="08cc3-104">A [CLI do Azure](/cli/azure/what-is-azure-cli) (Interface de Linha de Comando do Azure) é um conjunto de comandos usados para criar e gerenciar recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="08cc3-104">The Azure Command Line Interface ([Azure CLI](/cli/azure/what-is-azure-cli)) is a set of commands used to create and manage Azure resources.</span></span>  <span data-ttu-id="08cc3-105">Ela está disponível em muitos serviços do Azure, incluindo o Azure Monitor.</span><span class="sxs-lookup"><span data-stu-id="08cc3-105">It is available across many Azure services including Azure Monitor.</span></span>  <span data-ttu-id="08cc3-106">Há mais de 100 referências para o Azure Monitor, que possibilitam que você trabalhe de maneira eficaz com os serviços de monitor usando uma linha de comando.</span><span class="sxs-lookup"><span data-stu-id="08cc3-106">There are over 100 references for Azure Monitor giving you the ability to work effectively with monitor services from a command line.</span></span>

## <a name="references-for-azure-monitor"></a><span data-ttu-id="08cc3-107">Referências para o Azure Monitor</span><span class="sxs-lookup"><span data-stu-id="08cc3-107">References for Azure Monitor</span></span>

<span data-ttu-id="08cc3-108">A experiência da CLI do [Azure Monitor](/azure/azure-monitor/) é composta por duas partes: A CLI do Azure (também chamada de CLI **principal**) e a **extensão** da CLI do Azure Monitor.</span><span class="sxs-lookup"><span data-stu-id="08cc3-108">The [Azure Monitor](/azure/azure-monitor/) CLI experience is composed of two parts: Azure CLI (commonly referred to as CLI **core**) and the Azure Monitor CLI **extension**.</span></span>  <span data-ttu-id="08cc3-109">As referências de extensão da CLI do Azure devem ser instaladas antes do uso.</span><span class="sxs-lookup"><span data-stu-id="08cc3-109">Azure CLI extension references must be installed prior to use.</span></span> <span data-ttu-id="08cc3-110">O comando [az extension add](/cli/azure/extension?view=azure-cli-latest#az-extension-add) instala uma referência de extensão por nome.</span><span class="sxs-lookup"><span data-stu-id="08cc3-110">The [az extension add](/cli/azure/extension?view=azure-cli-latest#az-extension-add) command installs an extension reference by name.</span></span>

> [!IMPORTANT]
>
> <span data-ttu-id="08cc3-111">O Azure Monitor agora inclui o Application Insights e o Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="08cc3-111">Azure Monitor now includes Application Insights and Log Analytics.</span></span> <span data-ttu-id="08cc3-112">Dessa forma, você deve instalar as extensões para cada subárea ao trabalhar com a CLI do Azure Monitor.</span><span class="sxs-lookup"><span data-stu-id="08cc3-112">As such, you must install the extensions for each sub-area when working with Azure Monitor CLI.</span></span>

### <a name="references"></a><span data-ttu-id="08cc3-113">Referências</span><span class="sxs-lookup"><span data-stu-id="08cc3-113">References</span></span>

| <span data-ttu-id="08cc3-114">Referência</span><span class="sxs-lookup"><span data-stu-id="08cc3-114">Reference</span></span> | <span data-ttu-id="08cc3-115">Instalar a extensão</span><span class="sxs-lookup"><span data-stu-id="08cc3-115">Install extension</span></span> | <span data-ttu-id="08cc3-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="08cc3-116">Description</span></span> | <span data-ttu-id="08cc3-117">Para obter mais informações, consulte</span><span class="sxs-lookup"><span data-stu-id="08cc3-117">For more information see</span></span>
|-|-|-|-|
| [<span data-ttu-id="08cc3-118">az monitor</span><span class="sxs-lookup"><span data-stu-id="08cc3-118">az monitor</span></span>](/cli/azure/monitor) | | <span data-ttu-id="08cc3-119">O grupo de comandos de nível superior para todos os comandos da CLI do Azure para o Azure Monitor.</span><span class="sxs-lookup"><span data-stu-id="08cc3-119">The top level command group for all Azure CLI commands for Azure Monitor.</span></span> | [<span data-ttu-id="08cc3-120">Visão geral do Azure Monitor</span><span class="sxs-lookup"><span data-stu-id="08cc3-120">Azure Monitor overview</span></span>](/azure/azure-monitor/overview)
| [<span data-ttu-id="08cc3-121">az monitor action-group</span><span class="sxs-lookup"><span data-stu-id="08cc3-121">az monitor action-group</span></span>](/cli/azure/monitor/action-group) | | <span data-ttu-id="08cc3-122">Gerenciar grupos de ações, que se relacionam a notificações depois que um alerta é disparado.</span><span class="sxs-lookup"><span data-stu-id="08cc3-122">Manage action groups, which relate to notifications once an alert has fired.</span></span> | [<span data-ttu-id="08cc3-123">Alertas do Azure Monitor</span><span class="sxs-lookup"><span data-stu-id="08cc3-123">Azure Monitor alerts</span></span>](/azure/azure-monitor/platform/alerts-overview)
| [<span data-ttu-id="08cc3-124">az monitor activity-log</span><span class="sxs-lookup"><span data-stu-id="08cc3-124">az monitor activity-log</span></span>](/cli/azure/monitor/activity-log) | | <span data-ttu-id="08cc3-125">Gerenciar o log de atividades, incluindo alertas do log de atividades.</span><span class="sxs-lookup"><span data-stu-id="08cc3-125">Manage activity log including activity log alerts.</span></span> | [<span data-ttu-id="08cc3-126">Logs de atividades do Azure</span><span class="sxs-lookup"><span data-stu-id="08cc3-126">Azure activity logs</span></span>](/azure/azure-monitor/platform/activity-log)
| [<span data-ttu-id="08cc3-127">az monitor alert</span><span class="sxs-lookup"><span data-stu-id="08cc3-127">az monitor alert</span></span>](/cli/azure/monitor/alert) | | <span data-ttu-id="08cc3-128">NÃO USE para uma nova implantação.</span><span class="sxs-lookup"><span data-stu-id="08cc3-128">DO NOT USE for new development.</span></span>  <span data-ttu-id="08cc3-129">Esse comando gerencia as regras de alerta clássicas baseadas em métricas mais antigas que, exceto em alguns casos, foram migradas para os tipos de alertas de métrica mais recentes.</span><span class="sxs-lookup"><span data-stu-id="08cc3-129">This command manages older classic metric-based alert rules, which in all but a few cases have been migrated to the newer metric alert types.</span></span> <span data-ttu-id="08cc3-130">Em vez disso, use [az monitor metrics alert](/cli/azure/monitor/metrics/alert).</span><span class="sxs-lookup"><span data-stu-id="08cc3-130">Use [az monitor metrics alert](/cli/azure/monitor/metrics/alert) instead.</span></span> |
| [<span data-ttu-id="08cc3-131">az monitor app-insights</span><span class="sxs-lookup"><span data-stu-id="08cc3-131">az monitor app-insights</span></span>](/cli/azure/ext/application-insights/monitor/app-insights) | <span data-ttu-id="08cc3-132">sim</span><span class="sxs-lookup"><span data-stu-id="08cc3-132">yes</span></span> | <span data-ttu-id="08cc3-133">Gerenciar o Application Insights para monitoramento de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="08cc3-133">Manage Application Insights for application monitoring.</span></span> | [<span data-ttu-id="08cc3-134">Visão geral do Application Insights</span><span class="sxs-lookup"><span data-stu-id="08cc3-134">Application insights overview</span></span>](/azure/azure-monitor/app/app-insights-overview)
| [<span data-ttu-id="08cc3-135">az monitor autoscale</span><span class="sxs-lookup"><span data-stu-id="08cc3-135">az monitor autoscale</span></span>](/cli/azure/monitor/autoscale) | | <span data-ttu-id="08cc3-136">Gerenciar configurações de dimensionamento automático.</span><span class="sxs-lookup"><span data-stu-id="08cc3-136">Manage autoscale settings.</span></span> | [<span data-ttu-id="08cc3-137">Visão geral do dimensionamento automático</span><span class="sxs-lookup"><span data-stu-id="08cc3-137">Autoscale overview</span></span>](/azure/azure-monitor/platform/autoscale-overview)
| [<span data-ttu-id="08cc3-138">az monitor diagnostic-settings</span><span class="sxs-lookup"><span data-stu-id="08cc3-138">az monitor diagnostic-settings</span></span>](/cli/azure/monitor/diagnostic-settings) | | <span data-ttu-id="08cc3-139">Gerencie as configurações de diagnóstico do serviço, que configuram a coleta e o roteamento de muitos tipos de métricas e logs de plataforma.</span><span class="sxs-lookup"><span data-stu-id="08cc3-139">Manage service diagnostic settings, which sets up collection and routing of many types of platform metrics and logs.</span></span> | [<span data-ttu-id="08cc3-140">Criar configurações de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="08cc3-140">Create diagnostic settings</span></span>](/azure/azure-monitor/platform/diagnostic-settings)
| [<span data-ttu-id="08cc3-141">az monitor log-analytics</span><span class="sxs-lookup"><span data-stu-id="08cc3-141">az monitor log-analytics</span></span>](/cli/azure/monitor/log-analytics) | | <span data-ttu-id="08cc3-142">Gerenciar clusters de log e workspaces.</span><span class="sxs-lookup"><span data-stu-id="08cc3-142">Manage log clusters and work spaces.</span></span> | [<span data-ttu-id="08cc3-143">Criar sua implantação de Logs do Azure Monitor</span><span class="sxs-lookup"><span data-stu-id="08cc3-143">Designing your Azure Monitor Logs deployment</span></span>](/azure/azure-monitor/platform/design-logs-deployment)
| [<span data-ttu-id="08cc3-144">az monitor log-analytics query</span><span class="sxs-lookup"><span data-stu-id="08cc3-144">az monitor log-analytics query</span></span>](/cli/azure/ext/log-analytics/monitor/log-analytics#ext-log-analytics-az-monitor-log-analytics-query) | <span data-ttu-id="08cc3-145">sim</span><span class="sxs-lookup"><span data-stu-id="08cc3-145">yes</span></span> | <span data-ttu-id="08cc3-146">Comandos para consultar dados em workspaces do Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="08cc3-146">Commands for querying data in Log Analytics workspaces.</span></span>  | [<span data-ttu-id="08cc3-147">Introdução às consultas do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="08cc3-147">Get started with Log Analytics queries</span></span>](/azure/azure-monitor/log-query/get-started-portal)
| [<span data-ttu-id="08cc3-148">az monitor log-profiles</span><span class="sxs-lookup"><span data-stu-id="08cc3-148">az monitor log-profiles</span></span>](/cli/azure/monitor/log-profiles) | | <span data-ttu-id="08cc3-149">NÃO USE para uma nova implantação.</span><span class="sxs-lookup"><span data-stu-id="08cc3-149">DO NOT USE for new development.</span></span>  <span data-ttu-id="08cc3-150">Esse comando foi usado anteriormente para rotear logs de atividade para Log do Azure Monitor e para o Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="08cc3-150">This command was previously used to route activity logs to Azure Monitor Logs and Log Analytics.</span></span>  <span data-ttu-id="08cc3-151">Em vez disso, use [configuração de diagnóstico](/azure/azure-monitor/platform/diagnostic-settings).</span><span class="sxs-lookup"><span data-stu-id="08cc3-151">Use [diagnostic settings](/azure/azure-monitor/platform/diagnostic-settings) instead.</span></span>  | [<span data-ttu-id="08cc3-152">Enviar o log de atividades para o workspace do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="08cc3-152">Send the Activity log to a Log Analytics workspace</span></span>](/azure/azure-monitor/platform/activity-log#send-to-log-analytics-workspace)
| [<span data-ttu-id="08cc3-153">az monitor metrics</span><span class="sxs-lookup"><span data-stu-id="08cc3-153">az monitor metrics</span></span>](/cli/azure/monitor/metrics) | | <span data-ttu-id="08cc3-154">Gerencie métricas de plataforma e regras de alerta de métrica quase em tempo real.</span><span class="sxs-lookup"><span data-stu-id="08cc3-154">Manage platform metrics and near-realtime metric alert rules.</span></span> | <span data-ttu-id="08cc3-155">[Visão geral de métricas no Azure Monitor](/azure/azure-monitor/platform/data-platform-metrics) e [Entender como os alertas de métrica funcionam](/azure/azure-monitor/platform/alerts-metric-overview)</span><span class="sxs-lookup"><span data-stu-id="08cc3-155">[Overview of metrics in Azure Monitor](/azure/azure-monitor/platform/data-platform-metrics) and [Understand how metric alerts work](/azure/azure-monitor/platform/alerts-metric-overview)</span></span>
| [<span data-ttu-id="08cc3-156">az monitor private-link-scope</span><span class="sxs-lookup"><span data-stu-id="08cc3-156">az monitor private-link-scope</span></span>](/cli/azure/monitor/private-link-scope) | | <span data-ttu-id="08cc3-157">Gerenciar o recurso do escopo de link privado do monitor.</span><span class="sxs-lookup"><span data-stu-id="08cc3-157">Manage monitor private link scope resource.</span></span> | [<span data-ttu-id="08cc3-158">Usar o Link Privado do Azure para conectar redes com segurança ao Azure Monitor</span><span class="sxs-lookup"><span data-stu-id="08cc3-158">Use Azure Private Link to securely connect networks to Azure Monitor</span></span>](/azure/azure-monitor/platform/private-link-security)

### <a name="installing-extension-references"></a><span data-ttu-id="08cc3-159">Instalar referências de extensão</span><span class="sxs-lookup"><span data-stu-id="08cc3-159">Installing extension references</span></span>

<span data-ttu-id="08cc3-160">As referências de extensão da CLI do Azure devem ser instaladas antes do uso.</span><span class="sxs-lookup"><span data-stu-id="08cc3-160">Azure CLI extension references must be installed prior to use.</span></span>  <span data-ttu-id="08cc3-161">O comando [az extension add](/cli/azure/azure-cli-extensions-overview) instala uma referência de extensão por nome.</span><span class="sxs-lookup"><span data-stu-id="08cc3-161">The [az extension add](/cli/azure/azure-cli-extensions-overview) command installs an extension reference by name.</span></span>

```azurecli
# install the extension for az monitor app-insights
az extension add --name application-insights

# install the extension for az monitor log-analytics
az extension add --name log-analytics
```

## <a name="popular-monitor-articles-using-the-azure-cli"></a><span data-ttu-id="08cc3-162">Artigos populares do Monitor que usam a CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="08cc3-162">Popular Monitor articles using the Azure CLI</span></span>

- [<span data-ttu-id="08cc3-163">Exemplos de CLI do Azure Monitor</span><span class="sxs-lookup"><span data-stu-id="08cc3-163">Azure Monitor CLI samples</span></span>](/azure/azure-monitor/samples/cli-samples)
- [<span data-ttu-id="08cc3-164">Criar um workspace do Log Analytics com a CLI do Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="08cc3-164">Create a Log Analytics workspace with Azure CLI 2.0</span></span>](/azure/azure-monitor/learn/quick-create-workspace-cli)

## <a name="azure-cli-reference-examples"></a><span data-ttu-id="08cc3-165">Exemplos de referência da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="08cc3-165">Azure CLI reference examples</span></span>

<span data-ttu-id="08cc3-166">São fornecidos exemplos com todas as referências da CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="08cc3-166">Examples are provided with every Azure CLI reference.</span></span> <span data-ttu-id="08cc3-167">Embora você também possa concluir essas tarefas no portal do Azure, usar a CLI do Azure requer uma só linha de comando.</span><span class="sxs-lookup"><span data-stu-id="08cc3-167">Although you can also complete these tasks through the Azure portal, using the Azure CLI requires a single command line.</span></span>  <span data-ttu-id="08cc3-168">Veja alguns exemplos de código para ter uma ideia de como é fácil usar a CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="08cc3-168">Here are a few code samples to give you an idea of how easy it is to use the Azure CLI.</span></span>

<span data-ttu-id="08cc3-169">Para trabalhar com o Azure Monitor, primeiro você precisará de um grupo de recursos.</span><span class="sxs-lookup"><span data-stu-id="08cc3-169">To work with Azure Monitor, you'll first need a resource group.</span></span>  <span data-ttu-id="08cc3-170">Os grupos de recursos do Azure são simples de criar e gerenciar com a CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="08cc3-170">Azure resource groups are simple to create and manage with the Azure CLI.</span></span>  

```azurecli
#create a resource group
az group create -location westus -name MyResourceGroup

#get a list of resource groups for a subscription
az group list --subscription MySubscription --output table
```

<span data-ttu-id="08cc3-171">Criar um alerta de log do Azure Monitor é muito simples.</span><span class="sxs-lookup"><span data-stu-id="08cc3-171">Creating an Azure Monitor log alert is just as straightforward.</span></span>

```azurecli
#create an Azure Monitor activity log alert
az monitor activity-log alert create --name MyAlertName --resource-group MyResourceGroup
```

## <a name="see-also"></a><span data-ttu-id="08cc3-172">Confira também</span><span class="sxs-lookup"><span data-stu-id="08cc3-172">See also</span></span>

- <span data-ttu-id="08cc3-173">[Introdução à CLI do Azure](/cli/azure/get-started-with-azure-cli) para saber mais sobre a instalação e a conexão.</span><span class="sxs-lookup"><span data-stu-id="08cc3-173">[Get started with Azure CLI](/cli/azure/get-started-with-azure-cli) to learn about installation and sign in.</span></span>

- <span data-ttu-id="08cc3-174">Descubra referências adicionais [lançadas](/cli/azure/reference-index) e de [extensão](/cli/azure/azure-cli-extensions-list) na documentação da CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="08cc3-174">Discover additional [released](/cli/azure/reference-index) and [extension](/cli/azure/azure-cli-extensions-list) references in the Azure CLI documentation.</span></span>

- <span data-ttu-id="08cc3-175">Saiba mais sobre as referências de extensão em [Usar extensões com a CLI do Azure](/cli/azure/azure-cli-extensions-overview).</span><span class="sxs-lookup"><span data-stu-id="08cc3-175">Learn more about extension references in [Use extensions with Azure CLI](/cli/azure/azure-cli-extensions-overview).</span></span>