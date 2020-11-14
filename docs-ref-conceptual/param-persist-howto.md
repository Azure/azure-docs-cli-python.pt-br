---
title: Opções de parâmetro persistente da CLI do Azure
description: Como usar o parâmetro persistente da CLI do Azure para armazenar valores de parâmetro reutilizáveis
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.prod: azure
ms.date: 10/30/2020
ms.topic: conceptual
ms.devlang: azurecli
ms.technology: azure-cli
ms.custom: devex-track-azurecli
ms.openlocfilehash: 47fb93c7f78af94c58d509a969bab70b814e6128
ms.sourcegitcommit: 8d514f4147d6edfc02d8d95d5a4243d100a7fcc9
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2020
ms.locfileid: "93423178"
---
# <a name="azure-cli-persisted-parameter"></a>Parâmetro persistente da CLI do Azure

A referência do [az config param-persist](/cli/azure/param-persist) da CLI do Azure fornece a capacidade de reter valores de parâmetros persistentes locais para os comandos da CLI do Azure.  Isso elimina a necessidade de redigitar com frequência os parâmetros comuns. Por exemplo, o local e o grupo de recursos são parâmetros obrigatórios em muitos comandos da CLI, mas que não contribuem para a _intenção_ do comando.  Ao armazenar valores de parâmetro por meio de parâmetros persistentes, você diminui a redundância e pode reduzir significativamente a sintaxe dos comandos da CLI.

Os valores da configuração usados pela CLI são avaliados na seguinte precedência, com os itens na parte superior da lista sendo prioridade.

1. Parâmetros de linha de comando
1. Valores do diretório de trabalho local definidos pelo **az config param-persist**
1. Variáveis de ambiente
1. Valores do arquivo de configuração ou definidos com o **az config**

[Instale a CLI do Azure](install-azure-cli.md) ou abra o [Azure Cloud Shell](https://shell.azure.com) para executar os scripts deste artigo.  Se você estiver usando uma instalação local da CLI do Azure, será necessário ter a versão 2.12.0 (ou posterior) para executar os comandos do **az config param-persist**.  Execute [az version](/cli/azure/reference-index?#az_version) para localizar a versão e as bibliotecas dependentes que estão instaladas. Para fazer a atualização para a versão mais recente, execute [az upgrade](/cli/azure/reference-index?#az_upgrade).  O Azure Cloud Shell sempre tem a última versão da CLI do Azure.

## <a name="persisted-parameter-data-file"></a>Arquivo de dados do parâmetro persistente

Os valores dos parâmetros persistentes são mantidos em um arquivo chamado **.param_persist** , armazenado no diretório de trabalho.  Se você estiver usando o [Azure Cloud Shell](https://shell.azure.com) para executar comandos da CLI do Azure, o diretório de trabalho estará na conta de armazenamento usada pela CLI do Azure.  Se você estiver usando uma [instalação local](/install-azure-cli) da CLI do Azure, o diretório de trabalho estará no computador local.  Seja em qualquer um dos locais, o arquivo **.param_persist** fica oculto e não deve ser atualizado manualmente.

## <a name="persisted-parameter-storage-and-support"></a>Armazenamento e suporte de parâmetros persistentes

Os parâmetros da CLI do Azure a seguir são compatíveis com parâmetros persistentes.  Os parâmetros **resource_group_name** e **location** são armazenados de maneira diferente, de modo que você pode adicioná-los a parâmetros persistentes _sem_ executar o comando create.

| Parâmetro persistente | Ação de armazenamento | Com suporte por
|-|-|-|
| local | Executar qualquer comando | Todas as referências da CLI do Azure
| resource_group_name | Executar qualquer comando | Todas as referências da CLI do Azure
| vnet_name | Executar um comando create | Somente Aplicativos Web do Azure
| storage_account_name | Executar um comando create |  Somente Aplicativos Web do Azure
| webapp_name | Executar um comando create | Somente Aplicativos Web do Azure
| function_app_name | Executar um comando create | Somente Azure Functions

## <a name="sample-script-using-persisted-parameters"></a>Script de exemplo usando parâmetros persistentes

Sem os parâmetros persistentes, os comandos sequenciais da CLI devem repetir os mesmos valores de parâmetro.  Com os parâmetros persistentes habilitados, os valores de parâmetros armazenados podem ser omitidos nos comandos sequenciais.  Neste exemplo, o **local** , o **nome do grupo de recursos** ou o **nome da conta de armazenamento** são repetidos nos comandos subsequentes.

```azurecli
# Reminder: function app and storage account names must be unique.

# turn persisted parameters on
az config param-persist on

# Create a resource group which will store "resource group" and "location" in persisted parameter.
az group create --name RGlocalContext --location westeurope

# Create an Azure storage account omitting location and resource group.
az storage account create \
  --name sa1localcontext \
  --sku Standard_LRS

# Create a serverless function app in the resource group omitting storage account and resource group.
az functionapp create \
  --name FAlocalContext \
  --consumption-plan-location westeurope \
  --functions-version 2

# See the stored parameter values
az config param-persist show
```

## <a name="persisted-parameter-and-global-variable-comparison"></a>Comparação entre o parâmetro persistente e a variável global

Há dois comandos da CLI do Azure que podem ser usados para valores de parâmetro padrão: o **az configure** e o **az config param-persist**.  Use o comando **az configure** para especificar _variáveis globais_ , como grupo, local ou Web.  Use **az param-persist** para especificar _valores padrão locais_ exclusivos para a carga de trabalho.  Os valores armazenados são usados pela CLI no lugar dos argumentos necessários.

> [!Important]
> Parâmetros persistentes substituem os valores de contexto global.
>

| Referência | Escopo | Definir | Use
|-|-|-|-|
[az configure](/cli/azure/reference-index#az_configure) | Com escopo global em toda a CLI | Definir explicitamente usando **az configure --defaults** | Usar para configurações como registro em log, coleta de dados e valores de argumento padrão
[az config param-persist](/cli/azure/config/param-persist) | Com escopo definido localmente para um diretório de trabalho específico | Definir automaticamente quando os parâmetros persistentes forem ativados | Use para comandos sequenciais de uma carga de trabalho individual.

### <a name="command-examples"></a>Exemplos de comando

Use o **az config param-persist** para definir uma variável global usada na criação de uma conta de armazenamento do Azure.

```azurecli
# set the global variable for resource group
az configure --defaults group=myGlobalVariableRG

# Create an Azure storage account omitting the resource group relying on the global variable value
# Substitute the storage account name parameter with a unique value
az storage account create \
  --name mystorageaccount1 \
  --location westeurope \
  --sku Standard_LRS
```

A saída do comando da CLI mostra que foi criada uma conta de armazenamento no grupo de recursos encontrado na variável global, 'myGlobalVariableRG'.

```output
...
},
  "primaryLocation": "westeurope",
  "privateEndpointConnections": [],
  "provisioningState": "Succeeded",
  "resourceGroup": "myGlobalVariableRG",
  "routingPreference": null,
  "secondaryEndpoints": null,
  "secondaryLocation": null,
  "sku": {
    "name": "Standard_LRS",
    "tier": "Standard"
},
...
```

Use o **az config param-persist** para definir parâmetros persistentes usados na criação de uma conta de armazenamento do Azure.  Se uma variável global for definida para o mesmo objeto, o parâmetro persistente substituirá a variável global.

```azurecli
# turn persisted parameter on
az config param-persist on

# Create a resource group in order to write to persisted parameter
az group create --name myParamPersistRG --location westeurope

# Create an Azure storage account omitting the resource group relying on the persisted parameter value
# Substitute the storage account name parameter with a unique value
az storage account create \
  --name mystorageaccount2 \
  --location westeurope \
  --sku Standard_LRS
```

Mesmo com uma variável global definida para o grupo de recursos com o valor `myGlobalVariableRG`, com os parâmetros persistentes ativados a nova conta de armazenamento foi criada com `myParamPersistRG`.

```output
...
},
  "primaryLocation": "westeurope",
  "privateEndpointConnections": [],
  "provisioningState": "Succeeded",
  "resourceGroup": "myParamPersistRG",
  "routingPreference": null,
  "secondaryEndpoints": null,
  "secondaryLocation": null,
  "sku": {
    "name": "Standard_LRS",
    "tier": "Standard"
},
...
```

## <a name="see-also"></a>Confira também

* [Tutorial: usar parâmetros persistentes com comandos sequenciais da CLI do Azure](param-persist-tutorial.md)
* [Configuração da CLI do Azure usando o az configure](azure-cli-configuration.md)

