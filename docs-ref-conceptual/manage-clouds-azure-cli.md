---
title: Gerenciar várias nuvens com a CLI do Azure 2.0
description: Criar, fazer logon e gerenciar várias nuvens com a CLI do Azure 2.0.
author: sptramer
manager: routlaw
ms.author: sttramer
ms.date: 10/20/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.openlocfilehash: c17506cc81adc859ff5778b109c1832c857764e6
ms.sourcegitcommit: c9da729f4a42a839f13106f7589deaa0ca19cc4e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/06/2018
---
# <a name="managing-multiple-clouds-with-azure-cli-20"></a>Gerenciar várias nuvens com a CLI do Azure 2.0

Se você trabalha em regiões diferentes ou usa o [Azure Stack](https://docs.microsoft.com/azure/azure-stack/user/), talvez precise usar mais de uma nuvem. A Microsoft fornece nuvens para a conformidade com as leis regionais, que estão disponíveis seu uso. Este artigo mostra como obter informações sobre as nuvens disponíveis para sua conta, alterar a nuvem atual e registrar ou cancelar o registro de novas nuvens para usar com o Azure Stack.

## <a name="listing-clouds"></a>Listagem de nuvens

Você pode listar as nuvens disponíveis com o comando [az cloud list](/cli/azure/cloud#az-cloud-list). Isso informará qual nuvem está ativa no momento, qual é seu perfil atual e dará informações sobre os nomes de host e sufixos regionais.

Para obter a nuvem ativa e uma lista de todas as nuvens disponíveis:

```azurecli
az cloud list --output table
```

```output
IsActive    Name               Profile
----------  -----------------  ---------
True        AzureCloud         latest
            AzureChinaCloud    latest
            AzureUSGovernment  latest
            AzureGermanCloud   latest
```

A nuvem ativa no momento possui `True` na coluna `IsActive`. Somente uma nuvem pode estar ativa em determinado momento. Para obter informações mais detalhadas sobre uma nuvem, incluindo os pontos de extremidade que ela utiliza para os serviços do Azure, use o comando `cloud show`:

```azurecli
az cloud show --name AzureChinaCloud --output json
```

```output
{
  "endpoints": {
    "activeDirectory": "https://login.chinacloudapi.cn",
    "activeDirectoryDataLakeResourceId": null,
    "activeDirectoryGraphResourceId": "https://graph.chinacloudapi.cn/",
    "activeDirectoryResourceId": "https://management.core.chinacloudapi.cn/",
    "batchResourceId": "https://batch.chinacloudapi.cn/",
    "gallery": "https://gallery.chinacloudapi.cn/",
    "management": "https://management.core.chinacloudapi.cn/",
    "resourceManager": "https://management.chinacloudapi.cn",
    "sqlManagement": "https://management.core.chinacloudapi.cn:8443/",
    "vmImageAliasDoc": "https://raw.githubusercontent.com/Azure/azure-rest-api-specs/master/arm-compute/quickstart-templates/aliases.json"
  },
  "isActive": false,
  "name": "AzureChinaCloud",
  "profile": "latest",
  "suffixes": {
    "azureDatalakeAnalyticsCatalogAndJobEndpoint": null,
    "azureDatalakeStoreFileSystemEndpoint": null,
    "keyvaultDns": ".vault.azure.cn",
    "sqlServerHostname": ".database.chinacloudapi.cn",
    "storageEndpoint": "core.chinacloudapi.cn"
  }
}
```

## <a name="switching-the-active-cloud"></a>Alternar a nuvem ativa

Para trocar a nuvem ativa no momento, execute o comando [az cloud set](/cli/azure/cloud#az-cloud-set). Esse comando usa um argumento necessário, o nome da nuvem.

```azurecli
az cloud set --name AzureChinaCloud
```

> [!IMPORTANT]
> Se a autenticação para a nuvem ativada tiver expirado, você precisará autenticar novamente antes de realizar outras tarefas de CLI. Se esta for a primeira vez em que troca para a nova nuvem, você também precisará definir a assinatura ativa.
> Para obter instruções sobre autenticação, consulte [Fazer logon com a CLI do Azure 2.0](authenticate-azure-cli.md). Para obter informações sobre o gerenciamento de assinaturas, confira [Gerenciar assinaturas do Azure com a CLI do Azure 2.0](manage-azure-subscriptions-azure-cli.md)

## <a name="register-a-cloud"></a>Registrar uma nuvem

Registre uma nova nuvem se tiver seus próprios pontos de extremidade do Azure Stack. Uma nuvem é criada com o comando [az cloud register](/cli/azure/cloud#az-cloud-register). Este comando requer um nome e um conjunto de recursos com pontos de extremidade associados. Para saber como registrar uma nuvem para usar com o Azure Stack, confira [Instalar e configurar a CLI para usar com o Azure Stack](/azure/azure-stack/user/azure-stack-connect-cli#connect-to-azure-stack).

Você não precisa registrar sua própria nuvem para regiões na China, Governo dos EUA ou Alemanha. São gerenciadas pela Microsoft e ficam disponíveis por padrão.  Para obter mais informações sobre todas as configurações do ponto de extremidade disponíveis, confira a [documentação para `az cloud register`](/cli/azure/cloud#az-cloud-register).

Registrar uma nuvem não troca automaticamente para ela. Use o comando `az cloud set` para selecionar a nuvem recém-criada, conforme descrito acima.

## <a name="update-an-existing-cloud"></a>Atualizar uma nuvem existente

Se você tiver permissões, também poderá atualizar uma nuvem existente. Faça isso quando precisar trocar para um perfil diferente do Azure, adicionar ou alterar um ponto de extremidade.
Você faz isso com o comando [az cloud update](/cli/azure/cloud#az-cloud-update), que tem os mesmos argumentos de `az cloud register`.

## <a name="unregister-a-cloud"></a>Cancelar o registro de uma nuvem

Se você não precisar de uma nuvem registrada, o registro poderá ser cancelado com o comando [az cloud unregister](/cli/azure/cloud#az-cloud-unregister):

```azurecli
az cloud unregister --name MyCloud
```
