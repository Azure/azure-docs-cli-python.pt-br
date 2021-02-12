---
title: Tutorial sobre como usar parâmetros persistentes com a CLI do Azure
description: Tutorial sobre como usar o az config param-persist a fim de armazenar valores de parâmetro da CLI do Azure para uso recorrente
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.prod: azure
ms.date: 11/25/2020
ms.topic: conceptual
ms.devlang: azurecli
ms.technology: azure-cli
ms.custom: devex-track-azurecli
ms.openlocfilehash: 75833b18da0aea04dfc2aa33d9d7d18910525e98
ms.sourcegitcommit: 4c41593455b473c796735c73590403d9b6be87a2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/05/2021
ms.locfileid: "99572775"
---
# <a name="tutorial-use-persisted-parameters-to-simplify-sequential-azure-cli-commands"></a>Tutorial: usar parâmetros persistentes para simplificar comandos sequenciais da CLI do Azure

A CLI do Azure oferece os parâmetros persistentes que lhe permitem armazenar valores de parâmetro para uso contínuo.  Neste tutorial, você aprende a trabalhar com valores persistentes e a usar esses valores locais para executar com eficiência comandos sequenciais.

Neste tutorial, você aprenderá a:

> [!div class="checklist"]
> * Usar comandos de referência do `az config param-persist`
> * Executar comandos sequenciais usando os parâmetros persistentes

Este tutorial usa os comandos da CLI do Azure a seguir

- [az config param-persist delete](/cli/azure/config/param-persist#az_config_param_persist_delete)
- [az config param-persist off](/cli/azure/config/param-persist#az_config_param_persist_off)
- [az config param-persist on](/cli/azure/config/param-persist#az_config_param_persist_on)
- [az config param-persist show](/cli/azure/config/param-persist#az_config_param_persist_show)
- [az function app create](/cli/azure/functionapp#az_functionapp_create)
- [az group create](/cli/azure/group#az_group_create)
- [az storage account create](/cli/azure/storage/account#az_storage_account_create)


Se você não tiver uma assinatura do Azure, crie uma [conta gratuita](https://azure.microsoft.com/free/?WT.mc_id=A261C142F) antes de começar.

## <a name="prerequisites"></a>Pré-requisitos

1. [Instalar a CLI do Azure](install-azure-cli.md)

   Se preferir, você também pode usar o Azure Cloud Shell para concluir as etapas deste tutorial.  O Azure Cloud Shell é um ambiente de shell interativo usado por meio do navegador.  Inicie o Cloud Shell usando um destes métodos:

   - Abra o Cloud Shell acessando [https://shell.azure.com](https://shell.azure.com)

   - Selecione o botão **Cloud Shell** na barra de menus, no canto superior direito do [portal do Azure](https://portal.azure.com)

1. Se estiver usando uma instalação local da CLI do Azure, faça o seguinte:
   - Entre usando o comando [az login](/cli/azure/reference-index#az-login) e siga as etapas exibidas no terminal para concluir o processo de autenticação.

     ```azurecli
     az login
     ```
    - Este tutorial requer a versão 2.12.0 (ou posterior) da CLI do Azure.  Execute [az version](/cli/azure/reference-index#az_version) para localizar a versão e as bibliotecas dependentes que estão instaladas. Para fazer a atualização para a versão mais recente, execute [az upgrade](/cli/azure/reference-index#az_upgrade).

## <a name="1-determine-your-local-directory"></a>1. Determinar o diretório local

Os valores dos parâmetros persistentes são armazenados no diretório de trabalho da conta de armazenamento do Azure usada pelo Azure Cloud Shell.  Se você estiver usando uma instalação local da CLI do Azure, os valores serão armazenados no diretório de trabalho do computador.

Para localizar, criar ou alterar o diretório de trabalho que está sendo usado pela CLI do Azure, use estes comandos familiares da CLI.

```azurecli
# List directories
dir

# Make directory
mkdir azCLI

# Change directory
cd azCLI
```

## <a name="2-turn-on-persisted-parameters"></a>2. Ativar os parâmetros persistentes

Os [Parâmetros persistentes](/cli/azure/param-persist) devem ser ativados para que seja possível armazenar valores de parâmetros.  Você receberá um aviso até que `az config param-persist` saia da fase experimental.  Confira [Visão geral: tipos de referência e status da CLI do Azure](/cli/azure/reference-types-and-status) para saber mais sobre os tipos de referência, os status e os níveis de suporte da CLI do Azure.

```azurecli
az config param-persist on
```

## <a name="3-create-persisted-parameters"></a>3. Criar parâmetros persistentes

Para armazenar valores em parâmetros persistentes, execute o comando que preferir da CLI do Azure que contenha os parâmetros que você deseja armazenar.  Por exemplo, crie um grupo de recursos e os parâmetros `--location` e `--name` serão armazenados para uso futuro.

1. Armazene o local e o nome do grupo de recursos.
   ```azurecli
   # With persisted parameters turned on, create a resource group
   az group create --name RG1forTutorial --location eastus2

   # See new persisted parameters
   az config param-persist show
   ```

   ```output
   {
     "all": {
       "location": "eastus2",
       "resource_group_name": "RG1forTutorial"
     }
   }
   ```

1. Usando os novos parâmetros persistentes, crie uma conta de armazenamento.

   ```azurecli
   # Create a storage account
   az storage account create --name sa1fortutorial

   # See that storage_account_name has been added to persisted parameters
   az config param-persist show
   ```

   ```output
   {
     "all": {
       "location": "eastus2",
       "resource_group_name": "RG1forTutorial",
       "storage_account_name": "sa1fortutorial"
     }
   }
   ```

1. Crie um parâmetro persistente sem criar um recurso.

   Se você não quiser criar um recurso do Azure, os parâmetros `resource_group_name` e `location` poderão ser armazenados usando comandos que não são de criação, como o `show` ou `list`.   Confira [Parâmetros persistentes da CLI do Azure](/cli/azure/param-persist-howto#compare-parameter-persistence-and-global-variables) para obter uma lista completa dos parâmetros com suporte e a ação necessária para manter os valores.  Este exemplo também remove todos os valores de parâmetro usando o comando [az config param-persist delete](/cli/azure/config/param-persist#az-param-persist-delete).

   ```azurecli
   # Clear all persisted parameters for demonstration.
   az config param-persist delete --all

   # List all storage accounts which will create the `resource_group_name` stored parameter value.
   az storage account show --resource-group RG1forTutorial --name sa1fortutorial

   # See the new stored value created for resource group.  The storage account name is only stored with a 'create' command.
   az config param-persist show
   ```

   ```output
   {
     "all": {
       "resource_group_name": "RG1forTutorial"
     }
   }
   ```

## <a name="4-replace-persisted-parameters"></a>4. Substituir parâmetros persistentes

Substituir um valor de parâmetro armazenado é tão simples quanto executar um comando que contém um valor diferente.

1. Crie parâmetros persistentes.
   ```azurecli
   # Clear all persisted parameters for demonstration
   az config param-persist delete --all

   # Create a storage account placing "location", "resource_group_name", and "storage_account_name" into persisted parameters
   az storage account create --name sa1fortutorial --resource-group RG1forTutorial --location eastus2

   # See persisted parameters entries
   az config param-persist show
   ```

   ```output
   {
     "all": {
       "location": "eastus2",
       "resource_group_name": "RG1forTutorial",
       "storage_account_name": "sa1fortutorial"
     }
   }
   ```

1. Substitua os valores recém-armazenados.

   ```azurecli
   # Create a second storage account while changing both the "storage_account_name" and "location" persisted parameters
   az storage account create --name sa2fortutorial --location westeurope

   # See new persisted parameters
   az config param-persist show
   ```

   ```output
   {
     "all": {
       "location": "westeurope",
       "resource_group_name": "RG1forTutorial",
       "storage_account_name": "sa2fortutorial"
     }
   }
   ```

   > [!NOTE]
   >
   > Mesmo se os parâmetros persistentes estiverem ativados, você não precisará usá-los.  Você ainda pode executar os comandos com todos os valores de parâmetro especificados.  No entanto, lembre-se de que, com os parâmetros persistentes ativados, _você sempre criará parâmetros persistentes ou substituirá os parâmetros persistentes existentes._

## <a name="5-execute-sequential-commands"></a>5. Executar comandos sequenciais

Esses scripts criam um Aplicativo de funções do Azure usando o Plano de consumo.

### <a name="using-persisted-parameters"></a>[Usando parâmetros persistentes](#tab/azure-cli)

```azurecli
# Reminder: function app and storage account names must be unique.

# Turn persisted parameters on.
az config param-persist on

# Create a resource group.
az group create --name RG2forTutorial --location westeurope

# Create an Azure storage account in the resource group omitting "--location" and "--resource-group" parameters.
az storage account create \
  --name sa3fortutorial \
  --sku Standard_LRS

# Create a serverless function app in the resource group omitting "--storage-account" and "--resource-group" parameters.
az functionapp create \
  --name FAforTutorial \
  --consumption-plan-location westeurope \
  --functions-version 2

# See the stored parameter values.
az config param-persist show
```

### <a name="without-persisted-parameters"></a>[Sem parâmetros persistentes](#tab/azure-portal)

```azurecli
# Reminder: function app and storage account names must be unique.

# turn persisted parameters off
az config param-persist off

# Create a resource group.
az group create --name RG2forTutorial --location westeurope

# Create an Azure storage account in the resource group.
az storage account create \
  --name sa3fortutorial \
  --location westeurope \
  --resource-group RG2forTutorial \
  --sku Standard_LRS

# Create a serverless function app in the resource group.
az functionapp create \
  --name FAforTutorial \
  --storage-account sa3fortutorial \
  --consumption-plan-location westeurope \
  --resource-group RG2forTutorial \
  --functions-version 2
```

* * *

## <a name="6-delete-persisted-parameters"></a>6. Excluir parâmetros persistentes

Use o comando [az config param-persist delete](/cli/azure/param-persist#az-param-persist-delete) para remover entradas.

```azurecli
# Remove a single persisted parameters entry by specifying the name, not the value
az config param-persist delete resource_group_name

# Remove all persisted parameters entries and do not prompt for confirmation
az config param-persist delete --all --yes
```

> [!IMPORTANT]
>
> Os parâmetros persistentes não são atualizados quando um recurso do Azure é excluído.
>
> ```azurecli
> # delete a resource group
> az group delete --name RG1forTutorial
>
> # verify that the resource group no longer exists
> az group list --output table
>
> # See that the resource group name remains in persisted parameters
> az config param-persist show
> ```

## <a name="7-turn-persisted-parameters-off"></a>7. Desativar os parâmetros persistentes

Você pode desativar os parâmetros persistentes usando o comando [az config param-persist off](/cli/azure/param-persist#az-param-persist-off), mas os dados de parâmetros persistentes salvos não serão excluídos.

```azurecli
# Turn persisted parameters off
az config param-persist off

# See that your persisted parameters still exist
az config param-persist show

# Try to create a new resource relying on persisted parameters and receive error "...the following arguments are required:..."
az storage account create --name SA4inAzCLI --sku Standard_LRS
```

## <a name="8-clean-up-resources"></a>8. Limpar os recursos

Quando não forem mais necessários, use o comando [az group delete](/cli/azure/group) para remover o grupo de recursos e todos os recursos relacionados.

```azurecli
az group delete --name RG1forTutorial
```

## <a name="see-also"></a>Confira também

- [Como trabalhar com os parâmetros persistentes da CLI do Azure](param-persist-howto.md)
- [Configuração da CLI do Azure usando o az configure](/cli/azure/azure-cli-configuration)
