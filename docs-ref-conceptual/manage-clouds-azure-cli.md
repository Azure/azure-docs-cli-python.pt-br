---
title: Selecionar nuvens com a CLI do Azure
description: Crie, gerencie e conecte-se a várias nuvens com a CLI do Azure.
author: dbradish-microsoft
manager: barbkess
ms.author: dbradish
ms.date: 09/09/2018
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: b59da347069f0df61756eac958c6a0119a31be18
ms.sourcegitcommit: 5d29362589078b66d15f5cd494fe903a5195658d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/25/2020
ms.locfileid: "91225313"
---
# <a name="select-clouds-with-the-azure-cli"></a>Selecionar nuvens com a CLI do Azure

Se você trabalha em regiões diferentes ou usa o [Azure Stack](/azure/azure-stack/user/), talvez precise usar mais de uma nuvem. A Microsoft fornece nuvens para a conformidade com as leis regionais, que estão disponíveis seu uso. Este artigo mostra como obter informações sobre as nuvens, alterar a nuvem atual e registrar ou cancelar o registro de novas nuvens.

## <a name="list-available-clouds"></a>Listar nuvens disponíveis

Você pode listar as nuvens disponíveis com o comando [az cloud list](/cli/azure/cloud#az-cloud-list). Esse comando mostra qual nuvem está ativa no momento, qual é seu perfil atual e dará informações sobre os nomes de host e sufixos regionais.

Para obter a nuvem ativa e uma lista de todas as nuvens disponíveis:

```azurecli-interactive
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

```azurecli-interactive
az cloud show --name AzureChinaCloud --output json
```

```json
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

## <a name="switch-the-active-cloud"></a>Alternar a nuvem ativa

Para definir a nuvem padrão usando um arquivo de configuração, consulte [valores de configuração da CLI e variáveis de ambiente](./azure-cli-configuration.md?view=azure-cli-latest#cli-configuration-values-and-environment-variables).  Para alternar a nuvem ativa, execute o comando [az cloud set](/cli/azure/cloud#az-cloud-set). Esse comando usa um argumento necessário, o nome da nuvem.

```azurecli-interactive
az cloud set --name AzureChinaCloud
```

> [!IMPORTANT]
> Se a autenticação para a nuvem ativada tiver expirado, você precisará autenticar novamente antes de realizar outras tarefas de CLI. Se esta for a primeira vez em que troca para a nova nuvem, você também precisará definir a assinatura ativa.
> Para obter instruções sobre a autenticação, confira [Entrar com a CLI do Azure](authenticate-azure-cli.md). Para obter informações sobre o gerenciamento de assinaturas, confira [Gerenciar assinaturas do Azure com a CLI do Azure](manage-azure-subscriptions-azure-cli.md)

## <a name="register-a-new-cloud"></a>Registrar uma nova nuvem

Registre uma nova nuvem se tiver seus próprios pontos de extremidade do Azure Stack. Uma nuvem é criada com o comando [az cloud register](/cli/azure/cloud#az-cloud-register). Este comando requer um nome e um conjunto de pontos de extremidade de serviço. Para saber como registrar uma nuvem para usar com o Azure Stack, confira [Usar perfis de versão da API com a CLI do Azure no Azure Stack](/azure/azure-stack/user/azure-stack-version-profiles-azurecli2#connect-to-azure-stack).

Você não precisa registrar informações para regiões da Alemanha, China ou US Government. Essas nuvens são gerenciadas pela Microsoft e ficam disponíveis por padrão.  Para obter mais informações sobre todas as configurações do ponto de extremidade disponíveis, confira a [documentação para `az cloud register`](/cli/azure/cloud#az-cloud-register).

Você não é automaticamente migrado para uma nuvem ao registrá-la. Use o comando `az cloud set` para escolher a nuvem recém-criada.

## <a name="update-an-existing-cloud"></a>Atualizar uma nuvem existente

Se você tiver permissões, também poderá atualizar uma nuvem existente. A atualização de uma nuvem leva à mudança para um perfil de serviços do Azure diferente ou modifica os pontos de extremidade da conexão.
Atualize uma nuvem com o comando [az cloud update](/cli/azure/cloud#az-cloud-update), que tem os mesmos argumentos de `az cloud register`.

## <a name="unregister-a-cloud"></a>Cancelar o registro de uma nuvem

Se você já não precisar de uma nuvem criada, é possível remover seu registro com o comando [cloud unregister](/cli/azure/cloud#az-cloud-unregister):

```azurecli-interactive
az cloud unregister --name MyCloud
```