---
title: Entrar com a CLI do Azure 2.0
description: "Faça logon com a CLI do Azure 2.0 interativamente ou com credenciais locais"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 02/13/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 92c96b7e969de686689ef02bf068392b9f565698
ms.sourcegitcommit: 29d7366a0902488f4f4d39c2cb0e89368d5186ea
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2018
---
# <a name="log-in-with-azure-cli-20"></a>Entrar com a CLI do Azure 2.0

Há várias maneiras de fazer logon e autenticar com a CLI do Azure. A maneira mais simples de começar é fazendo logon interativamente no navegador por meio do Azure Cloud Shell ou do comando `az login`.
A abordagem recomendada é usar entidades de serviço, que são contas restritas a permissões. Ao conceder apenas as permissões apropriadas necessárias para uma entidade de serviço, você pode garantir que seus scripts de automação fiquem ainda mais seguros.

Nenhuma informação de credencial privada é armazenada localmente. Em vez disso, um token de autenticação é gerado pelo Azure e armazenado. Após o logon, seu token de logon local fica válido até passar 14 dias sem ser usado. Depois disso, você precisará autenticar novamente.

Após o logon, os comandos da CLI são executados em sua assinatura padrão. Caso tenha mais de uma assinatura, é possível [alterar sua assinatura padrão](manage-azure-subscriptions-azure-cli.md).

## <a name="interactive-log-in"></a>Logon Interativo

Faça logon interativamente usando seu navegador da Web.

[!INCLUDE [interactive_login](includes/interactive-login.md)]

## <a name="command-line"></a>Linha de comando

Forneça suas credenciais na linha de comando.

> [!Note]
> Essa abordagem não funciona com contas da Microsoft ou contas que tenham a autenticação de dois fatores habilitada.

```azurecli
az login -u <username> -p <password>
```

## <a name="log-in-with-a-specific-tenant"></a>Faça logon com um locatário específico

Caso trabalhe com vários locatários, é possível selecionar seu locatário para fazer logon em com o argumento `--tenant`. O valor desse argumento pode tanto ser um domínio `.onmicrosoft.com` como a ID de objeto do Azure para o locatário. É possível fazer logon interativamente ou fornecer suas credenciais com os argumentos `--user` e `--password`. 

```
az login --tenant <tenant>
```

## <a name="logging-in-with-a-service-principal"></a>Como fazer logon com uma entidade de serviço

Entidades de serviço são contas que não estão associadas a nenhum usuário específico, as quais podem ter permissões atribuídas por meio de funções predefinidas. Autenticar com uma entidade de serviço é a melhor maneira de gravar scripts seguros ou programas, permitindo a aplicação de restrições de permissões e informações de credenciais estáticas armazenadas localmente. Para saber mais sobre entidades de serviço, consulte [Criar uma entidade de serviço do Azure com a CLI do Azure](create-an-azure-service-principal-azure-cli.md).

Para fazer logon com uma entidade de serviço, você fornece o nome de usuário, senha ou arquivo do certificado PEM e o locatário associado à entidade de serviço:

```azurecli
az login --service-principal -u <user> -p <password-or-cert> --tenant <tenant>
```

O valor do locatário é um locatário do Azure Active Directory associado à entidade de serviço. Pode tanto ser um domínio `.onmicrosoft.com` como a ID de objeto do Azure para o locatário.
Você pode obter a ID de objeto do locatário para seu logon atual usando o seguinte comando:

```azurecli
az account show --query 'tenantId' -o tsv
```
