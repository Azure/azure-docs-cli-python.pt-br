---
title: Usar entidades de serviço do Azure com a CLI do Azure
description: Saiba como criar e usar entidades de serviço com a CLI do Azure.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 02/15/2019
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: c18adbee84fd3e5c73367b07bbd0b03ac61008cd
ms.sourcegitcommit: b5ecfc168489cd0d96462d6decf83e8b26a10194
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2020
ms.locfileid: "80417865"
---
# <a name="create-an-azure-service-principal-with-the-azure-cli"></a>Criar uma entidade de serviço do Azure com a CLI do Azure

Ferramentas automatizadas que usam os serviços do Azure devem sempre ter permissões restritas. Em vez de os aplicativos entrarem como um usuário com privilégio total, o Azure oferece as entidades de serviço.

Uma entidade de serviço do Azure é uma identidade criada para uso com aplicativos, serviços hospedados e ferramentas automatizadas para acessar os recursos do Azure. Esse acesso é restrito pelas funções atribuídas à entidade de serviço, oferecendo a você o controle sobre quais recursos poderão ser acessados e em qual nível. Por motivos de segurança, é sempre recomendado usar entidades de serviço com ferramentas automatizadas em vez de permitir a entrada com uma identidade de usuário.

Este artigo mostra as etapas para criar, obter informações e redefinir uma entidade de serviço com a CLI do Azure.

## <a name="create-a-service-principal"></a>Criar uma entidade de serviço

Crie uma entidade de serviço com o comando [az ad sp create-for-rbac](/cli/azure/ad/sp#az-ad-sp-create-for-rbac). Ao criar uma entidade de serviço, você pode escolher o tipo de autenticação de entrada usada.

> [!NOTE]
>
> Se sua conta não tiver permissão para criar uma entidade de serviço, `az ad sp create-for-rbac` mostrará uma mensagem de erro “Privilégios insuficientes para concluir a operação”. Entre em contato com o administrador do Azure Active Directory para criar uma entidade de serviço.

Há dois tipos de autenticação disponíveis para as entidades de serviço: A autenticação baseada em senha e em certificado.

### <a name="password-based-authentication"></a>Autenticação baseada em senha

Sem parâmetros de autenticação, a autenticação baseada em senha é usada com uma senha aleatória criada para você.

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName
  ```

> [!IMPORTANT]
> Desde a CLI do Azure 2.0.68, o parâmetro `--password` para criar uma entidade de serviço com uma senha definida pelo usuário __não tem mais suporte__ para evitar o uso acidental de senhas fracas.

A saída para uma entidade de serviço com a autenticação por senha inclui a chave `password`. __Certifique-se de__ que tenha copiado esse valor já que não será possível recuperá-lo posteriormente. Se você esquecer a senha, [redefina as credenciais da entidade de serviço](#reset-credentials).

As chaves `appId` e `tenant` aparecem na saída do `az ad sp create-for-rbac` e são usadas na autenticação da entidade de serviço.
Registre seus valores, mas eles podem ser recuperados a qualquer momento com o comando [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).

### <a name="certificate-based-authentication"></a>Autenticação baseada em certificado

Para a autenticação baseada em certificado, use o argumento `--cert`. Esse argumento exige que você mantenha um certificado existente. Certifique-se de que todas as ferramentas que usam essa entidade de serviço tenham acesso à chave privada do certificado. Os certificados devem estar no formato ASCII, como PEM, CER ou DER. Transmita o certificado como uma cadeia de caracteres ou use o formato `@path` para carregar o certificado de um arquivo.

> [!NOTE]
> Ao usar um arquivo PEM, o **CERTIFICADO** precisa ser anexado à **CHAVE PRIVADA** dentro do arquivo.

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --cert "-----BEGIN CERTIFICATE-----
...
-----END CERTIFICATE-----"
```

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --cert @/path/to/cert.pem
```

O argumento `--keyvault` pode ser adicionado para usar o certificado no Azure Key Vault. Nesse caso, o valor `--cert` é o nome do certificado.

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --cert CertName --keyvault VaultName
```

Para criar um certificado _autoassinado_ para autenticação, use o argumento `--create-cert`:

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --create-cert
```

Saída do console:

```
Creating a role assignment under the scope of "/subscriptions/myId"
Please copy C:\myPath\myNewFile.pem to a safe place.
When you run 'az login', provide the file path in the --password argument
{
  "appId": "myAppId",
  "displayName": "myDisplayName",
  "fileWithCertAndPrivateKey": "C:\\myPath\\myNewFile.pem",
  "name": "http://myName",
  "password": null,
  "tenant": "myTenantId"
}
```

Conteúdo do novo arquivo PEM:
```
-----BEGIN PRIVATE KEY-----
myPrivateKeyValue
-----END PRIVATE KEY-----
-----BEGIN CERTIFICATE-----
myCertificateValue
-----END CERTIFICATE-----
```

> [!NOTE]
> O comando `az ad sp create-for-rbac --create-cert` cria a entidade de serviço e um arquivo PEM. O arquivo PEM contém uma **CHAVE PRIVADA** e um **CERTIFICADO** formatados corretamente.

O argumento `--keyvault` pode ser adicionado para armazenar o certificado no Azure Key Vault. Ao usar `--keyvault`, o argumento `--cert` também será __necessário__.

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --create-cert --cert CertName --keyvault VaultName
```

A menos que você armazene o certificado no cofre de chaves, a saída incluirá a chave `fileWithCertAndPrivateKey`. O valor dessa chave informa onde o certificado gerado é armazenado.
__Certifique-se__ de copiar o certificado para um local seguro ou não será possível entrar com essa entidade de serviço.

Para certificados armazenados no Key Vault, recupere a chave privada do certificado com o comando [az keyvault secret show](/cli/azure/keyvault/secret#az-keyvault-secret-show). No Key Vault, o nome do segredo do certificado é igual ao nome do certificado. Se você perder o acesso à chave privada de um certificado, [redefina as credenciais da entidade de serviço](#reset-credentials).

As chaves `appId` e `tenant` aparecem na saída do `az ad sp create-for-rbac` e são usadas na autenticação da entidade de serviço.
Registre seus valores, mas eles podem ser recuperados a qualquer momento com o comando [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).

## <a name="get-an-existing-service-principal"></a>Obter uma entidade de serviço existente

Uma lista das entidades de serviço em um locatário pode ser recuperada com o comando [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list). Por padrão, esse comando retorna as 100 primeiras entidades de serviço do locatário. Para obter todas as entidades de serviço de um locatário, use o argumento `--all`. Obter essa lista pode levar muito tempo, portanto, é recomendável que você filtre a lista com um dos argumentos a seguir:

* `--display-name` envia solicitações às entidades de serviço que têm um _prefixo_ que corresponda ao nome fornecido. O nome de exibição de uma entidade de serviço é o valor definido com o parâmetro `--name` durante a criação. Se você não definiu `--name` durante a criação da entidade de serviço, o prefixo do nome será `azure-cli-`.
* `--spn` filtra a correspondência do nome exato da entidade de serviço. O nome da entidade de serviço sempre começa com `https://`.
  se o valor usado para `--name` não era um URI, esse valor é `https://` seguido do nome de exibição.
* `--show-mine` só envia solicitações às entidades de serviço criadas pelo usuário conectado.
* `--filter` usa um filtro OData e realiza a filtragem _do lado do servidor_. Esse método é recomendado para a filtragem do lado do cliente com o argumento `--query` da CLI. Para saber mais sobre os filtros do OData, confira [Sintaxe de expressão do OData para filtros](/rest/api/searchservice/odata-expression-syntax-for-azure-search).

As informações retornadas para objetos da entidade de serviço são detalhadas. Para obter apenas as informações necessárias para entrar, use a cadeia de consulta `[].{id:appId, tenant:appOwnerTenantId}`. Por exemplo, para obter as informações de logon para todas as entidades de serviço criadas pelo usuário conectado no momento:

```azurecli-interactive
az ad sp list --show-mine --query "[].{id:appId, tenant:appOwnerTenantId}"
```

> [!IMPORTANT]
>
> `az ad sp list` ou [az ad sp show](/cli/azure/ad/sp#az-ad-sp-show) obtêm o usuário e o locatário, mas não os segredos de autenticação _nem_ o método de autenticação.
> Os segredos para certificados no Key Vault podem ser recuperados com o comando [az keyvault secret show](/cli/azure/keyvault/secret#az-keyvault-secret-show), mas, por padrão, nenhum outro segredo será armazenado.
> Se você esquecer o método de autenticação ou o segredo, [redefina as credenciais da entidade de serviço](#reset-credentials).

## <a name="manage-service-principal-roles"></a>Gerenciar funções da entidade de serviço

A CLI do Azure oferece os seguintes comandos para gerenciar as atribuições de função:

* [az role assignment list](/cli/azure/role/assignment#az-role-assignment-list)
* [az role assignment create](/cli/azure/role/assignment#az-role-assignment-create)
* [az role assignment delete](/cli/azure/role/assignment#az-role-assignment-delete)

A função padrão para uma entidade de serviço é **Colaborador**. Essa função tem permissões completas para ler e gravar em uma conta do Azure. A função **Leitor** é mais restritiva, com acesso somente leitura.  Para obter mais informações sobre o Controle de Acesso Baseado em Função (RBAC) e funções, confira [RBAC: funções internas](/azure/active-directory/role-based-access-built-in-roles).

Esse exemplo adiciona a função **Leitor** e exclui a função **Colaborador**:

```azurecli-interactive
az role assignment create --assignee APP_ID --role Reader
az role assignment delete --assignee APP_ID --role Contributor
```

> [!NOTE]
> Caso sua conta não tenha permissão para atribuir uma função, você verá uma mensagem de erro informando que sua conta “não tem autorização para executar a ação ‘Microsoft.Authorization/roleAssignments/write’”. Entre em contato com o administrador do Azure Active Directory para gerenciar funções.

Adicionar uma função _não_ restringe as permissões atribuídas anteriormente. Ao restringir as permissões da entidade de serviço, a função __Colaborador__ deverá ser removida.

Para verificar as alterações, liste as funções atribuídas:

```azurecli-interactive
az role assignment list --assignee APP_ID
```

## <a name="sign-in-using-a-service-principal"></a>Entrar usando uma entidade de serviço

Teste as novas credenciais e permissões da entidade de serviço iniciando a sessão. Para entrar com uma entidade de serviço, você precisa de `appId`, `tenant` e das credenciais.

Para entrar com uma entidade de serviço usando a senha:

```azurecli-interactive
az login --service-principal --username APP_ID --password PASSWORD --tenant TENANT_ID
```

Para entrar com um certificado, ele precisa estar disponível localmente como um arquivo PEM ou DER, no formato ASCII. Ao usar um arquivo PEM, a **CHAVE PRIVADA** e o **CERTIFICADO** precisam ser anexados juntos dentro do arquivo.

```azurecli-interactive
az login --service-principal --username APP_ID --tenant TENANT_ID --password /path/to/cert
```

Para saber mais sobre como entrar com uma entidade de serviço, confira [Entrar com a CLI do Azure](authenticate-azure-cli.md).

## <a name="reset-credentials"></a>Redefinir credenciais

Se você esquecer as credenciais de uma entidade de serviço, use o comando [az ad sp credencial reset](/cli/azure/ad/sp/credential#az-ad-sp-credential-reset). O comando reset tem os mesmos argumentos que `az ad sp create-for-rbac`.

```azurecli-interactive
az ad sp credential reset --name APP_ID
```
