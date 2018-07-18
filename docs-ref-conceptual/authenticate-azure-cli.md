---
title: Entrar com a CLI do Azure 2.0
description: Entrar com a CLI do Azure 2.0 interativamente ou com as credenciais locais
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 07/09/2018
ms.topic: conceptual
ms.technology: azure-cli
ms.devlang: azurecli
ms.service: active-directory
ms.component: authentication
ms.openlocfilehash: a0e05b3306cc273486b1b5fc887ceedbf78cb779
ms.sourcegitcommit: 64f2c628e83d687d0e172c01f13d71c8c39a8040
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/11/2018
ms.locfileid: "38967751"
---
# <a name="sign-in-with-azure-cli-20"></a>Entrar com a CLI do Azure 2.0

Há várias maneiras de se autenticar com a CLI do Azure. A maneira mais fácil de começar é entrar interativamente no navegador por meio do Azure Cloud Shell ou do comando `az login`.
A abordagem recomendada é usar entidades de serviço, que são contas restritas a permissões. Ao conceder apenas as permissões apropriadas necessárias para uma entidade de serviço, você pode garantir que seus scripts de automação fiquem ainda mais seguros.

Nenhuma informação de credencial privada é armazenada localmente. Em vez disso, um token de autenticação é gerado pelo Azure e armazenado. Após a conexão, seu token de autenticação fica válido por até 14 dias sem ser usado. Depois disso, você precisará autenticar novamente.

Após a conexão, os Comandos da CLI são executados em sua assinatura padrão. Caso tenha mais de uma assinatura, é possível [alterar sua assinatura padrão](manage-azure-subscriptions-azure-cli.md).

## <a name="interactive-sign-in"></a>Entrada interativa

O método de autenticação padrão da CLI do Azure usa um navegador da Web e token de acesso para entrar.

[!INCLUDE [interactive_login](includes/interactive-login.md)]

## <a name="command-line"></a>Linha de comando

Forneça suas credenciais de usuário do Azure na linha de comando.

> [!Note]
> Essa abordagem não funciona com contas da Microsoft ou contas que tenham a autenticação de dois fatores habilitada.

```azurecli
az login -u <username> -p <password>
```

> [!IMPORTANT]
> Caso deseje evitar a exibição de sua senha no console e esteja usando `az login` interativamente, use o comando `read -s` em `bash`.
>
> ```bash
> read -sp "Azure password: " AZ_PASS && echo && az login -u <username> -p $AZ_PASS
> ```
>
> No PowerShell, use o cmdlet `Read-Host -AsSecureString` e proteja a conversão da cadeia de caracteres.
>
> ```powershell
> $securePass =  Read-Host "Azure password: " -AsSecureString;
> $AzPass = [Runtime.InteropServices.Marshal]::PtrToStringAuto([Runtime.InteropServices.Marshal]::SecureStringToBSTR($securePass));
> az login -u <username> -p $AzPass;
> $AzPass = ""
> ```

## <a name="sign-in-with-a-specific-tenant"></a>Entrar com um locatário específico

Se você trabalha com vários locatários, é possível selecionar seu locatário para entrar com o argumento `--tenant`. O valor desse argumento pode tanto ser um domínio `.onmicrosoft.com` como a ID de objeto do Azure para o locatário. É possível entrar interativamente ou fornecer suas credenciais com os argumentos `--user` e `--password`.

```azurecli
az login --tenant <tenant>
```

## <a name="sign-in-with-a-service-principal"></a>Entrar com uma entidade de serviço

Entidades de serviço são contas que não estão associadas a nenhum usuário específico, as quais podem ter permissões atribuídas por meio de funções predefinidas. Autenticar com uma entidade de serviço é a melhor maneira de gravar scripts seguros ou programas, permitindo a aplicação de restrições de permissões e informações de credenciais estáticas armazenadas localmente. Para saber mais sobre entidades de serviço, consulte [Criar uma entidade de serviço do Azure com a CLI do Azure](create-an-azure-service-principal-azure-cli.md).

Para entrar com uma entidade de serviço, você fornece o nome de usuário, senha ou arquivo PEM de certificado e o locatário associado à entidade de serviço:

```azurecli
az login --service-principal -u <app-url> -p <password-or-cert> --tenant <tenant>
```

O valor do locatário é um locatário do Azure Active Directory associado à entidade de serviço. Pode tanto ser um domínio `.onmicrosoft.com` como a ID de objeto do Azure para o locatário.
Você pode obter a ID de objeto do locatário para sua conta ativa atualmente usando o seguinte comando:

```azurecli-interactive
az account show --query 'tenantId' -o tsv
```

> [!IMPORTANT]
> Caso deseje evitar a exibição de sua senha no console e esteja usando `az login` interativamente, use o comando `read -s` em `bash`.
>
> ```bash
> read -sp "Azure password: " AZ_PASS && echo && az login --service-principal -u <app-url> -p $AZ_PASS --tenant <tenant>
> ```
>
> No PowerShell, use o cmdlet `Read-Host -AsSecureString` e proteja a conversão da cadeia de caracteres.
>
> ```powershell
> $securePass =  Read-Host "Azure password: " -AsSecureString;
> $AzPass = [Runtime.InteropServices.Marshal]::PtrToStringAuto([Runtime.InteropServices.Marshal]::SecureStringToBSTR($securePass));
> az login --service-principal -u <app-url> -p $AzPass --tenant <tenant>;
> $AzPass = ""
> ```
