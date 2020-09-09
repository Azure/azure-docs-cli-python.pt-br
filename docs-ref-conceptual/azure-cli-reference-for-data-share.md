---
title: Referências da CLI do Azure para o Azure Data Share
description: Página de aterrissagem da referência da CLI do Azure para o Azure Data Share
services: data-share
author: dbradish-microsoft
manager: barbkess
ms.service: data-share
ms.devlang: azurecli
ms.topic: reference
ms.date: 05/27/2020
ms.author: dbradish
ms.custom: devx-track-azurecli
ms.openlocfilehash: e8d834864b2d967beb18e9cd304b922db859ef09
ms.sourcegitcommit: 2da241715d25407ed22c1065c0c793acfd865996
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/09/2020
ms.locfileid: "89562763"
---
# <a name="azure-cli-for-azure-data-share"></a>CLI do Azure para o Azure Data Share

A [CLI do Azure](/cli/azure/what-is-azure-cli) (Interface de Linha de Comando do Azure) é um conjunto de comandos usados para criar e gerenciar recursos do Azure.  Ela está disponível em muitos serviços do Azure, incluindo o Azure Data Share.  Há mais de 65 comandos diferentes para o compartilhamento de dados.  Esses comandos oferecem a capacidade de trabalhar com eficiência com o serviço de uma linha de comando.

## <a name="references-for-data-share"></a>Referências para o Data Share

Todos os comandos da CLI do Azure para o Azure Data Share são atualmente extensões para a CLI do Azure.  Uma extensão fornece acesso a comandos experimentais e de pré-lançamento.  Saiba mais sobre as referências de extensão em [Usar extensões com a CLI do Azure](/cli/azure/azure-cli-extensions-overview).

|Referência da CLI do Azure |Descrição
|-|-|-|
| [az datashare](/cli/azure/ext/datashare/datashare) | Todos os comandos para gerenciar o Azure Data Share.
| [az datashare account](/cli/azure/ext/datashare/datashare/account) | Comandos para gerenciar as contas do Azure Data Share.
| [az datashare consumer](/cli/azure/ext/datashare/datashare/consumer) | Comandos para os consumidores gerenciarem o Azure Data Share.
| [az datashare dataset](/cli/azure/ext/datashare/datashare/dataset) | Comandos para os provedores gerenciarem os conjuntos de dados do Azure Data Share.
| [az datashare invitation](/cli/azure/ext/datashare/datashare/invitation) | Comandos para os consumidores gerenciarem convites do Azure Data Share.
| [az datashare provider-share-subscription](/cli/azure/ext/datashare/datashare/provider-share-subscription) | Comandos para os provedores gerenciarem assinaturas do Azure Data Share.
| [az datashare synchronization](/cli/azure/ext/datashare/datashare/synchronization)  | Comandos para gerenciar a sincronização do Azure Data Share.
| [az datashare synchronization-setting](/cli/azure/ext/datashare/datashare/synchronization-setting)  | Comandos para os provedores gerenciarem as configurações de sincronização do Azure Data Share.

## <a name="reference-examples"></a>Exemplos de referência

São fornecidos exemplos com todas as referências da CLI do Azure. Embora você também possa concluir essas tarefas no portal do Azure, usar a CLI do Azure requer uma só linha de comando.  Veja alguns blocos de código para ter uma ideia de como é fácil usar a CLI do Azure.

Para trabalhar com o Azure Data Share, primeiro você precisará de um grupo de recursos.  Os grupos de recursos do Azure são simples de criar e gerenciar com a CLI do Azure.  

```azurecli
#create a resource group
az group create -location westus -name MyResourceGroup
```

```azurecli
#get a list of resource groups for a subscription
az group list --subscription MySubscription --output table
```

É tão simples criar uma conta de compartilhamento de dados.

```azurecli
#create a data share account
az datashare account create --location "West US 2" --tags tag1=Red tag2=White --name MyAccount --resource-group MyResourceGroup
```

## <a name="see-also"></a>Confira também

* [Introdução à CLI do Azure](/cli/azure/get-started-with-azure-cli) para saber mais sobre a instalação e a conexão.

* Descubra referências adicionais de [núcleo](/cli/azure/reference-index) e de [extensão](/cli/azure/azure-cli-extensions-list) na documentação da CLI do Azure.
