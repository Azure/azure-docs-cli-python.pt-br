---
title: Gerenciar grupos de recursos do Azure com a CLI do Azure
description: Saiba mais sobre os grupos de recursos do Azure e o uso da CLI do Azure para gerenciá-los. Saiba mais sobre os grupos de recursos persistentes e padrão.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 01/15/2021
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 22167bf3d0e1d3356ebf4a1a9854bab9d5476051
ms.sourcegitcommit: 3e79897e0aeca4d74bc8ff0410121b011b5884ec
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2021
ms.locfileid: "99496074"
---
# <a name="working-with-resource-groups-in-azure-cli"></a>Como trabalhar com grupos de recursos na CLI do Azure

Um grupo de recursos do Azure é um contêiner que mantém os recursos relacionados a uma solução do Azure. Um grupo de recursos pode conter armazenamento, máquinas virtuais, aplicativos, painéis, serviços ou quase tudo o que você usa no Azure.

## <a name="create-a-resource-group"></a>Criar um grupo de recursos

Para criar um grupo de recursos, use o comando [az group create](/cli/azure/group#az_group_create):

```azurecli
az group create --name MyResourceGroup --location eastus
```

Um grupo de recursos pertence a uma só localização. Para ver todas as localizações com suporte na sua assinatura atual, execute o comando [az account list-locations](/cli/azure/account#az_account_list_locations):

```azurecli
az account list-locations
```

Para ver todos os grupos de recursos para a sua assinatura atual, use o comando [az group list](/cli/azure/group#az_group_list):

```azurecli
az group list --output table
```

> [!TIP]
> O parâmetro `--output` é um parâmetro global, disponível para todos os comandos. O valor **table** apresenta a saída em um formato amigável. Para obter mais informações, confira [Formatos de saída para comandos da CLI do Azure](/cli/azure/format-output-azure-cli).

Ao criar um recurso, você o cria em um grupo de recursos. O seguinte exemplo mostra a criação de uma conta de armazenamento com o comando [az storage account create](/cli/azure/storage/account#az_storage_account_create):

```azurecli
az storage account create --resource-group MyResourceGroup --name storage134 --location eastus --sku Standard_LRS
```

Para remover um grupo de recursos, execute o comando [az group delete](/cli/azure/group#az_group_delete):

```azurecli
az group delete --name MyResourceGroup
```

Ao remover um grupo de recursos, você exclui todos os recursos que pertencem a ele. Não há nenhuma opção para restaurar os recursos. Se você testar um dos comandos deste artigo, a exclusão dos grupos de recursos criados limpará a sua conta.

## <a name="persist-a-resource-group"></a>Persistir um grupo de recursos

A persistência de parâmetro permite que você reutilize valores para determinados parâmetros, incluindo grupos de recursos.

Primeiro, ative o recurso de persistência usando o comando [az config param-persist on](/cli/azure/config/param-persist#az_config_param_persist_on):

```azurecli
az config param-persist on
```

Depois de ativar a persistência, crie outro grupo de recursos:

 ```azurecli
az group create --name OtherResourceGroup --location eastus
```

Desde que a persistência esteja ativada, você poderá deixar o parâmetro `--resource-group` fora dos comandos futuros. O seguinte comando cria uma conta de armazenamento no grupo **OtherResourceGroup**:

```azurecli
az storage account create --name storage135 --location eastus --sku Standard_LRS
```

Se você especificar um grupo de recursos no comando, isso terá precedência. O seguinte comando cria um grupo de armazenamento em um grupo de recursos chamado **StorageGroups**:

```azurecli
az storage account create --resource-group StorageGroups --name storage136 --location eastus --sku Standard_LRS
```

No entanto, depois que você especificar outro grupo de recursos como um valor, a CLI do Azure redefinirá o valor persistente. Os novos comandos usam **StorageGroups** como o grupo de recursos. Você poderá ver os valores persistentes usando o comando [az config param-persist show](/cli/azure/config/param-persist#az_config_param_persist_show):

```azurecli
az config param-persist show
```

Esse comando mostra os valores persistentes atuais. Esses valores são armazenados em um arquivo chamado *local_context_\<username>* em um diretório oculto chamado *.azure*. A CLI do Azure cria o diretório na sua localização atual quando você cria um valor persistente pela primeira vez.

Quando você terminar de usar parâmetros persistentes, execute o comando [az config param-persist off](/cli/azure/config/param-persist#az_config_param_persist_off):

```azurecli
az config param-persist off
```

A CLI do Azure salvará os valores persistentes. Você poderá vê-los no arquivo de contexto local. Se você ativar a persistência de parâmetro novamente, esses valores já estarão definidos.

Para obter mais informações sobre como usar os comandos [az config param-persist](/cli/azure/config/param-persist), confira [Usar parâmetros persistentes para simplificar os comandos sequenciais da CLI do Azure](/cli/azure/param-persist-tutorial).

## <a name="set-a-default-resource-group"></a>Definir um grupo de recursos padrão

Você pode definir um grupo de recursos padrão para todos os comandos executados da CLI do Azure local ou do Azure Cloud Shell. A CLI do Azure armazena essa configuração localmente em um arquivo *config*. Para ver a configuração atual, execute o comando [az config get](/cli/azure/config#az_config_get):

```azurecli
az config get
```

O resultado mostra os grupos de recursos padrão e outros valores padrão. Se você estiver usando a CLI do Azure pela primeira vez, os resultados poderão estar vazios.

Para definir um grupo de recursos padrão para a instalação da CLI do Azure, execute o comando [az config set](/cli/azure/config#az_config_set):

```azurecli
az config set defaults.group=MyResourceGroup
```

O comando define um valor para uma chave especificada, neste caso, `defaults.group`. Para obter as opções de configuração disponíveis, confira [Configuração da CLI do Azure](/cli/azure/azure-cli-configuration).

> [!NOTE]
> O comando [az config set](/cli/azure/config#az_config_set) não valida a existência do grupo de recursos inserido. O comando apenas armazena o par chave-valor.

Depois que você executar o comando, os dois seguintes comandos fornecerão o mesmo resultado:

```azurecli
az storage account create --resource-group MyResourceGroup --name storage01  --location eastus --sku Standard_LRS
az storage account create --name storage01 --location eastus --sku Standard_LRS
```

Um grupo de recursos pertence a uma assinatura. Se a sua organização tiver mais de uma assinatura, você precisará definir essa assinatura antes de trabalhar com um grupo de recursos na assinatura. Se o valor padrão de um grupo de recursos não pertencer à sua assinatura atual, ocorrerá um erro. Para obter mais informações sobre o uso de várias assinaturas, confira [Usar várias assinaturas do Azure](manage-azure-subscriptions-azure-cli.md).

Você não precisa redefinir o padrão para usar outros grupos de recursos. Em vez disso, especifique o grupo de recursos:

```azurecli
az group create --name OtherResourceGroup --location eastus
az storage account create --resource-group StorageGroups --name storage03  --location westus --sku Standard_LRS
```

O valor padrão destina-se apenas a você. Ele não afetará outros usuários ou as alterações feitas por meio do portal do Azure.

Se você estiver usando valores de parâmetros persistentes, conforme descrito neste artigo, esses valores terão precedência sobre os padrões definidos no arquivo *config*.

## <a name="clean-up-resources"></a>Limpar os recursos

Se você testou um dos comandos deste artigo, remova todos os recursos criados com o comando [az group delete](/cli/azure/group#az_group_delete):

```azurecli
az group delete --name MyResourceGroup
az group delete --name OtherResourceGroup
az group delete --name StorageGroups
```

Esse comando remove o grupo e todos os recursos que ele contém ao mesmo tempo.

Remova os parâmetros persistentes executando o comando [az config param-persist delete](/cli/azure/config/param-persist#az_config_param_persist_delete):

```azurecli
az config param-persist delete --all
```

## <a name="see-also"></a>Confira também

[Configuração da CLI do Azure](/cli/azure/azure-cli-configuration)

[Tutorial: usar parâmetros persistentes para simplificar comandos sequenciais da CLI do Azure](/cli/azure/param-persist-tutorial)

[Usar várias assinaturas do Azure](manage-azure-subscriptions-azure-cli.md)
