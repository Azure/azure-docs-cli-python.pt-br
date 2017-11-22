---
title: Entrar com a CLI do Azure 2.0
description: Entre com a CLI do Azure 2.0 no Linux, Mac ou Windows.
keywords: "CLI do Azure 2.0, logon, CLI do Azure, autenticação, autorizar, logon"
author: sptramer
ms.author: stttramer
manager: routlaw
ms.date: 11/13/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 65becd3a-9d69-4415-8a30-777d13a0e7aa
ms.openlocfilehash: dd05868f7378673836f47e743ed4088f2efd3dca
ms.sourcegitcommit: 5db22de971cf3983785cb209d92cbed1bbd69ecf
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/14/2017
---
# <a name="log-in-with-azure-cli-20"></a>Entrar com a CLI do Azure 2.0

Há várias maneiras de fazer logon e autenticar com a CLI do Azure. É a maneira mais simples para começar é fazer logon interativamente no navegador ou na linha de comando. A abordagem recomendada é usar entidades de serviço que fornecem uma maneira para que você crie contas não-interativas para manipular os recursos. Ao conceder apenas as permissões apropriadas necessárias para uma entidade de serviço, você pode garantir que seus scripts de automação fiquem ainda mais seguros. 

Nenhuma informação de credencial privada é armazenada localmente. Em vez disso, um token de autenticação é gerado pelo Azure e armazenado. Após o logon, seu token de logon local é válido até ficar 14 dias sem ser usado. Nesse ponto, você precisará autenticar novamente.

Após o logon, os comandos da CLI são executados em sua assinatura padrão. Se você tiver mais de uma assinatura, poderá querer [altear sua assinatura padrão](manage-azure-subscriptions-azure-cli.md).

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
Autenticar com uma entidade de serviço é a melhor maneira de proteger o uso de seus recursos do Azure dos scripts ou aplicativos que manipulam recursos. Se você ainda não tem uma entidade de serviço disponível e gostaria de criar uma, confira [Criar uma entidade de serviço do Azure com a CLI do Azure](create-an-azure-service-principal-azure-cli.md).

Para fazer logon com uma entidade de serviço, você fornece o nome de usuário, senha ou arquivo do certificado PEM e o locatário associado à entidade de serviço:

```azurecli-interactive
az login --service-principal -u <user> -p <password-or-cert> --tenant <tenant>
```

O valor do locatário é um locatário do Azure Active Directory associado à entidade de serviço. Isso pode ser um domínio .onmicrosoft.com ou a ID de objeto do Azure para o locatário.
Você pode obter a ID de objeto do locatário para seu logon atual usando o seguinte comando:

```azurecli
az account show --query 'tenanatId' -o tsv
```

