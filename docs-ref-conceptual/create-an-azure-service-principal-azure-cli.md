---
title: "Criar uma entidade de serviço do Azure com a CLI do Azure 2.0"
description: "Saiba como criar uma entidade de serviço para seu aplicativo ou serviço com a CLI do Azure 2.0."
keywords: CLI do Azure 2.0, Azure Active Directory, Azure Active directory, AD, RBAC
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: fab89cb8-dac1-4e21-9d34-5eadd5213c05
ms.openlocfilehash: 10a168ae0c33207905d58b7b57ac9ad76d8d9bf4
ms.sourcegitcommit: 73a73c8a17d95b116d33eee3287d938addc5c0ac
ms.translationtype: HT
ms.contentlocale: pt-BR
---
# <a name="create-an-azure-service-principal-with-azure-cli-20"></a>Criar uma entidade de serviço do Azure com a CLI do Azure 2.0

Se você planeja gerenciar seu aplicativo ou serviço com a CLI do Azure 2.0, execute-a em uma entidade de serviço do Azure Active Directory (AAD) em vez de suas próprias credenciais.
Esse tópico orienta você pela criação de uma entidade de segurança com a CLI do Azure 2.0.

> [!NOTE]
> Você também pode criar uma entidade de serviço por meio do Portal do Azure.
> Leia [Usar o portal para criar um aplicativo e entidade de serviço do Active Directory que pode acessar recursos](/azure/azure-resource-manager/resource-group-create-service-principal-portal) para obter mais detalhes.

## <a name="what-is-a-service-principal"></a>O que é uma entidade de serviço?

Uma entidade de serviço do Azure é uma identidade de segurança usada por aplicativos criados pelo usuário, serviços e ferramentas de automação para acessar recursos específicos do Azure. Pense nela como uma 'identidade de usuário' (login e senha ou certificado) com uma função específica e permissões de acesso aos seus recursos rigidamente controladas. Ela só precisa ser capaz de fazer coisas específicas, ao contrário de uma identidade de usuário geral. A segurança aumenta se você só conceder a ela o nível mínimo de permissões necessárias para realizar suas tarefas de gerenciamento. 

Atualmente, a CLI do Azure 2.0 só suporta a criação de credenciais de autenticação baseadas em senha. Nesse tópico, abordaremos a criação de uma entidade de serviço com uma senha específica e, opcionalmente, a atribuição de funções específicas a ela.

## <a name="verify-your-own-permission-level"></a>Verificar seu próprio nível de permissão

Primeiro, você deve ter permissões suficientes no Azure Active Directory e em sua assinatura do Azure. Especificamente, você deve ser capaz de criar um aplicativo no Active Directory e atribuir uma função à entidade de serviço. 

A maneira mais fácil de verificar se a sua conta tem as permissões adequadas é por meio do portal. Consulte [Verificar permissão necessária no portal](/azure/azure-resource-manager/resource-group-create-service-principal-portal.md#required-permissions).

## <a name="create-a-service-principal-for-your-application"></a>Crie uma entidade de serviço para seu aplicativo

Você deve ter um dos itens a seguir para identificar o aplicativo para o qual você deseja criar uma entidade de serviço:

  * o nome exclusivo ou URI do seu aplicativo implantado (como "MyDemoWebApp" nos exemplos) ou
  * a ID do Aplicativo, o GUID exclusivo associado ao aplicativo, serviço ou objeto implantado

Esses valores identificam seu aplicativo durante a criação de uma entidade de serviço.

### <a name="get-information-about-your-application"></a>Obter informações sobre seu aplicativo

Obtenha informações sobre seu aplicativo com a `az ad app list`.

```azurecli
az ad app list --display-name MyDemoWebApp
```

```json
{
    "appId": "a487e0c1-82af-47d9-9a0b-af184eb87646d",
    "appPermissions": null,
    "availableToOtherTenants": false,
    "displayName": "MyDemoWebApp",
    "homepage": "http://MyDemoWebApp.azurewebsites.net",
    "identifierUris": [
      "http://MyDemoWebApp"
    ],
    "objectId": "bd07205b-629f-4a2e-945e-1ee5dadf610b9",
    "objectType": "Application",
    "replyUrls": []
  }
```

O opção `--display-name` filtra a lista retornada de aplicativos para mostrá-los com o `displayName` começando com MyDemoWebApp.

### <a name="create-the-service-principal"></a>Criar a entidade de serviço

Use [az ad sp create-for-rbac](/cli/azure/ad/sp#create-for-rbac) para criar a entidade de serviço. 

```azurecli
az ad sp create-for-rbac --name {appId} --password "{strong password}" 
``` 

```json
{
  "appId": "a487e0c1-82af-47d9-9a0b-af184eb87646d",
  "displayName": "MyDemoWebApp",
  "name": "http://MyDemoWebApp",
  "password": {strong password},
  "tenant": "XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"
}
```

 > [!WARNING] 
 > Não crie uma senha não segura.  Execute a orientação [Restrições e regras de senha do Azure AD](/azure/active-directory/active-directory-passwords-policy).

### <a name="get-information-about-the-service-principal"></a>Obter informações sobre a entidade de serviço

```azurecli
az ad sp show --id a487e0c1-82af-47d9-9a0b-af184eb87646d
```

```json
{
  "appId": "a487e0c1-82af-47d9-9a0b-af184eb87646d",
  "displayName": "MyDemoWebApp",
  "objectId": "0ceae62e-1a1a-446f-aa56-2300d176659bde",
  "objectType": "ServicePrincipal",
  "servicePrincipalNames": [
    "http://MyDemoWebApp",
    "a487e0c1-82af-47d9-9a0b-af184eb87646d"
  ]
}
```

### <a name="sign-in-using-the-service-principal"></a>Entrar usando a entidade de serviço

Agora você pode entrar como a nova entidade de serviço para seu aplicativo usando a *appId* e a *senha* de `az ad sp show`.  Forneça o valor *tenant* dos resultados de `az ad sp create-for-rbac`.

```azurecli
az login --service-principal -u a487e0c1-82af-47d9-9a0b-af184eb87646d --password {password} --tenant {tenant}
``` 

Você verá essa saída após um logon bem-sucedido:

```json
[
  {
    "cloudName": "AzureCloud",
    "id": "a487e0c1-82af-47d9-9a0b-af184eb87646d",
    "isDefault": true,
    "state": "Enabled",
    "tenantId": "XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX",
    "user": {
      "name": "https://MyDemoWebApp",
      "type": "servicePrincipal"
    }
  }
]
```

Use os valores `id`, `password` e `tenant` valores como as credenciais para a execução de seu aplicativo. 

## <a name="managing-roles"></a>Gerenciamento de funções 

> [!NOTE]
> O RBAC (Controle de Acesso do Azure Baseado em Função) é um modelo para definir e gerenciar funções para entidades de usuário e de serviço.
> As funções têm conjuntos de permissões associados a elas, que determinam os recursos que uma entidade pode ler, acessar, gravar ou gerenciar.
> Para saber mais sobre funções e RBAC, consulte [RBAC: funções internas](/azure/active-directory/role-based-access-built-in-roles).

A CLI do Azure 2.0 fornece os seguintes comandos para gerenciar atribuições de função:

* [az role assignment list](/cli/azure/role/assignment#list)
* [az role assignment create](/cli/azure/role/assignment#create)
* [az role assignment delete](/cli/azure/role/assignment#delete)

A função padrão para uma entidade de serviço é **Colaborador**. Pode não ser a melhor opção para interações do aplicativo com os serviços do Azure, dadas suas permissões amplas. A função **Leitor** é mais restritiva e é uma boa opção para acesso somente leitura. Você pode exibir detalhes sobre as permissões específicas de função ou criar conectores personalizados por meio do portal do Azure.

Nesse exemplo, adicionamos a função **Leitor** ao nosso exemplo anterior e excluímos a função **Colaborador**:

```azurecli
az role assignment create --assignee a487e0c1-82af-47d9-9a0b-af184eb87646d --role Reader
az role assignment delete --assignee a487e0c1-82af-47d9-9a0b-af184eb87646d --role Contributor
```

Verifique as alterações listando as funções atribuídas no momento:

```azurecli
az role assignment list --assignee a487e0c1-82af-47d9-9a0b-af184eb87646d
```

```json
{
    "id": "/subscriptions/34345f33-0398-4a99-a42b-f6613d1664ac/providers/Microsoft.Authorization/roleAssignments/c27f78a7-9d3b-404b-ab59-47818f9af9ac",
    "name": "c27f78a7-9d3b-404b-ab59-47818f9af9ac",
    "properties": {
      "principalId": "790525226-46f9-4051-b439-7079e41dfa31",
      "principalName": "http://MyDemoWebApp",
      "roleDefinitionId": "/subscriptions/34345f33-0398-4a99-a42b-f6613d1664ac/providers/Microsoft.Authorization/roleDefinitions/acdd72a7-3385-48ef-bd42-f606fba81ae7",
      "roleDefinitionName": "Reader",
      "scope": "/subscriptions/34345f33-0398-4a99-a42b-f6613d1664ac"
    },
    "type": "Microsoft.Authorization/roleAssignments"
}
```

> [!NOTE] 
> Se sua conta não tiver permissões suficientes para atribuir uma função, verá uma mensagem de erro.
> A mensagem informa que sua conta “não tem autorização para executar a ação 'Microsoft.Authorization/roleAssignments/write' no escopo '/subscriptions/{guid}'”.
   
## <a name="change-the-credentials-of-a-security-principal"></a>Alterar as credenciais de uma entidade de segurança

É uma boa prática de segurança examinar as permissões e atualizar as senhas regularmente. Talvez você também queira gerenciar e modificar as credenciais de segurança à medida que seu aplicativo muda.

### <a name="reset-a-service-principal-password"></a>Redefinir uma senha da entidade de serviço

Use `az ad sp reset-credentials` para redefinir a senha atual da entidade de serviço.

```azurecli
az ad sp reset-credentials --name 20bce7de-3cd7-49f4-ab64-bb5b443838c3 --password {new-password}
```

```json
{
  "appId": "a487e0c1-82af-47d9-9a0b-af184eb87646d",
  "name": "a487e0c1-82af-47d9-9a0b-af184eb87646d",
  "password": {new-password},
  "tenant": "XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"
}
```

A CLI gera uma senha segura se você deixar a opção `--password` de fora.