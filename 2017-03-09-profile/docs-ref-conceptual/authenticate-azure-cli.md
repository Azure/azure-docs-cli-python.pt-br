---
title: Entrar com a CLI do Azure 2.0
description: Entre com a CLI do Azure 2.0 no Linux, Mac ou Windows.
keywords: CLI do Azure 2.0, Linux, Mac, Windows, OS X, Ubuntu, Debian, CentOS, RHEL, SUSE, CoreOS, Docker, Windows, Python, PIP
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 65becd3a-9d69-4415-8a30-777d13a0e7aa
ms.openlocfilehash: 3ba1dd840102c738ccd9eb62a0b9db612cec48d1
ms.sourcegitcommit: 5cfbea569fef193044da712708bc6957d3fb557c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2017
---
# <a name="log-in-with-azure-cli-20"></a>Entrar com a CLI do Azure 2.0

Há várias maneiras de fazer logon e autenticar com a CLI do Azure. É a maneira mais simples para começar é fazer logon interativamente no navegador ou na linha de comando. A abordagem recomendada é usar entidades de serviço que fornecem uma maneira para que você crie contas não-interativas para manipular os recursos. Ao conceder apenas as permissões apropriadas necessárias para uma entidade de serviço, você pode garantir que seus scripts de automação fiquem ainda mais seguros. 

Nenhuma informação de credencial privada é armazenada localmente. Em vez disso, um token de autenticação é gerado pelo Azure e armazenado. Após o logon, seu token de logon local é válido até ficar 14 dias sem ser usado. Nesse ponto, você precisará autenticar novamente.

Comandos que são executados com a CLI são executados em sua assinatura padrão.  Se você tiver mais de uma assinatura, convém [confirmar sua assinatura padrão](manage-azure-subscriptions-azure-cli.md) e alterá-la adequadamente.

## <a name="interactive-log-in"></a>Logon Interativo

Faça logon interativamente usando seu navegador da Web.

[!INCLUDE [interactive_login](includes/interactive-login.md)]

## <a name="command-line"></a>Linha de comando

Forneça suas credenciais na linha de comando.

> [!Note]
> Essa abordagem não funciona com contas da Microsoft ou contas que tenham a autenticação de dois fatores habilitada.

```azurecli-interactive
az login -u <username> -p <password>
```

## <a name="logging-in-with-a-service-principal"></a>Como fazer logon com uma entidade de serviço

As entidades de serviço são como as contas de usuário às quais você pode aplicar regras usando o Azure Active Directory.
Autenticar com uma entidade de serviço é a melhor maneira de proteger o uso de seus recursos do Azure dos scripts ou aplicativos que manipulam recursos.
Você define as funções que deseja que os usuários tenham por meio do conjunto de comandos do `az role`.
Você pode saber mais e ver exemplos de funções de entidade de serviço em nossos [artigos de referência de função az](https://docs.microsoft.com/cli/azure/role.md).

1. Se você ainda não tiver uma entidade de serviço, [crie uma](create-an-azure-service-principal-azure-cli.md).

1. Faça logon com uma entidade de serviço.

   ```azurecli-interactive
   az login --service-principal -u "http://my-app" -p <password> --tenant <tenant>
   ```

   Para obter o locatário, faça logon interativamente e obtenha a TenantId da sua assinatura.

   ```azurecli
   az account show
   ```

   ```json
   {
       "environmentName": "AzureCloud",
       "id": "********-****-****-****-************",
       "isDefault": true,
       "name": "Pay-As-You-Go",
       "state": "Enabled",
       "tenantId": "********-****-****-****-************",
       "user": {
       "name": "********",
       "type": "user"
       }
   }
   ```
