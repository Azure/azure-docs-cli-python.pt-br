---
title: Entrar com a CLI do Azure
description: Entrar com a CLI do Azure interativamente ou com as credenciais locais
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.technology: azure-cli
ms.devlang: azurecli
ms.component: authentication
ms.openlocfilehash: 05a4ef87fcf23af21ec6dc1d6cd9daa82369d5b9
ms.sourcegitcommit: 0d6b08048b5b35bf0bb3d7b91ff567adbaab2a8b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/07/2018
ms.locfileid: "51222439"
---
# <a name="sign-in-with-azure-cli"></a>Entrar com a CLI do Azure 

Há vários tipos de autenticação para a CLI do Azure. A maneira mais fácil de começar é com o [Azure Cloud Shell](/azure/cloud-shell/overview) que conecta você automaticamente.
Localmente, você pode entrar no modo interativo pelo navegador com o comando [az login](/cli/azure/reference-index#az-login). Ao escrever scripts, a abordagem recomendada é usar entidades de serviço. Ao conceder apenas as permissões apropriadas necessárias para uma entidade de serviço, você mantém sua automação segura.

Nenhuma das suas informações de entrada é armazenada pela CLI. Em vez disso, um [token de atualização de autenticação](https://docs.microsoft.com/en-us/azure/active-directory/develop/v1-id-and-access-tokens#refresh-tokens) é gerado pelo Azure e depois é armazenado. A partir de agosto de 2018, esse token será revogado após 90 dias de inatividade, mas esse valor poderá ser alterado pela Microsoft ou seu administrador de locatários. Depois que o token for revogado, você receberá uma mensagem da CLI dizendo que você precisa entrar novamente.

Após a conexão, os comandos da CLI são executados em sua assinatura padrão. Caso tenha várias assinaturas, é possível [alterar sua assinatura padrão](manage-azure-subscriptions-azure-cli.md).

## <a name="sign-in-interactively"></a>Entrar no modo interativo

O método de autenticação padrão da CLI do Azure usa um navegador da Web e token de acesso para entrar.

[!INCLUDE [interactive_login](includes/interactive-login.md)]

## <a name="sign-in-with-credentials-on-the-command-line"></a>Entrar com credenciais na linha de comando

Forneça suas credenciais de usuário do Azure na linha de comando.

> [!Note]
> Essa abordagem não funciona com contas da Microsoft ou contas que tenham a autenticação de dois fatores habilitada.

```azurecli-interactive
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

## <a name="sign-in-with-a-service-principal"></a>Entrar com uma entidade de serviço

Entidades de serviço são contas que não estão associadas a nenhum usuário específico, as quais podem ter permissões atribuídas por meio de funções predefinidas. Autenticar com uma entidade de serviço é a melhor maneira de gravar scripts seguros ou programas, permitindo a aplicação de restrições de permissões e informações de credenciais estáticas armazenadas localmente. Para saber mais sobre entidades de serviço, consulte [Criar uma entidade de serviço do Azure com a CLI do Azure](create-an-azure-service-principal-azure-cli.md).

Para entrar com uma entidade de serviço, você precisa:

* Da URL ou nome associado à entidade de serviço
* A senha da entidade de serviço ou o certificado X509 usado para criar a entidade de serviço em formato PEM
* O locatário associado à entidade de serviço, como um domínio `.onmicrosoft.com` ou ID de objeto do Azure

```azurecli-interactive
az login --service-principal -u <app-url> -p <password-or-cert> --tenant <tenant>
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

## <a name="sign-in-with-a-different-tenant"></a>Entrar com um locatário diferente

Você pode selecionar um locatário para entrar com o argumento `--tenant`. O valor desse argumento pode tanto ser um domínio `.onmicrosoft.com` como a ID de objeto do Azure para o locatário. Os dois métodos de entrada, interativo e com linha de comando, funcionam com `--tenant`.

```azurecli-interactive
az login --tenant <tenant>
```

## <a name="sign-in-with-a-managed-identity"></a>Entrar com uma identidade gerenciada

Nos recursos configurados para identidades gerenciadas em recursos do Azure, você pode entrar usando a identidade gerenciada. A entrada com a identidade do recurso é feito por meio do sinalizador `--identity`.

```azurecli-interactive
az login --identity
```

Para saber mais sobre identidades gerenciadas em recursos do Azure, confira [Configurar identidades gerenciadas em recursos do Azure](https://docs.microsoft.com/en-us/azure/active-directory/managed-identities-azure-resources/qs-configure-cli-windows-vm) e [Usar identidades gerenciadas em recursos do Azure para fazer logon](https://docs.microsoft.com/en-us/azure/active-directory/managed-identities-azure-resources/how-to-use-vm-sign-in).
