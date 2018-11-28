---
title: Usar entidades de serviço do Azure com a CLI do Azure
description: Saiba como criar e usar uma entidade de serviço com a CLI do Azure.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 40ff3b54cdd1f4908b59479e317092ee62b05bb0
ms.sourcegitcommit: f92d5b3ccd409be126f1e7c06b9f1adc98dad78b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/20/2018
ms.locfileid: "52159364"
---
# <a name="create-an-azure-service-principal-with-azure-cli"></a>Criar uma entidade de serviço do Azure com a CLI do Azure

Caso queira criar uma conexão separada com restrições de acesso, é possível fazer isso com uma entidade de serviço. Entidades de serviço são identidades separadas que podem ser associadas a uma conta. Entidades de serviço são úteis para trabalhar com aplicativos e tarefas que devem ser automatizadas. Este artigo guia você pelas etapas de criação de uma entidade de serviço.

## <a name="create-the-service-principal"></a>Criar a entidade de serviço

Use o comando [az ad sp create-for-rbac](/cli/azure/ad/sp#az-ad-sp-create-for-rbac) para criar uma entidade de serviço. O nome da entidade de serviço não está vinculado a nenhum aplicativo ou nome de usuário existente. Você pode criar uma entidade de serviço com a escolha do tipo de autenticação.

* `--password` é usado para autenticação baseada em senha. Verifique se você criou uma senha forte, seguindo as [regras e restrições de senha do Azure Active Directory](/azure/active-directory/active-directory-passwords-policy). Caso não especifique uma senha, uma será criada para você.

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --password PASSWORD
  ```

* `--cert` é usado para autenticação baseada em certificado para um certificado existente, como uma cadeia de caracteres pública PEM ou DER, ou `@{file}` para carregar um arquivo.

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --cert {CertStringOrFile}
  ```

  O argumento `--keyvault` pode ser adicionado para indicar que o certificado está armazenado no Azure Key Vault. Nesse caso, o valor `--cert` se refere ao nome do certificado no Key Vault.

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --cert CertName --keyvault VaultName
  ```

* `--create-cert` cria um certificado _autoassinado_ para autenticação. Se o argumento `--cert` não for fornecido, será gerado um nome de certificado aleatório.

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --create-cert
  ```

  O argumento `--keyvault` pode ser adicionado para armazenar o certificado no Azure Key Vault. Ao usar `--keyvault`, o argumento `--cert` também é necessário.

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --create-cert --cert CertName --keyvault VaultName
  ```

Se um argumento que indica o tipo de autenticação não for incluído, `--password` é usado por padrão.

A saída JSON do comando `create-for-rbac` está no seguinte formato:

```json
{
  "appId": "APP_ID",
  "displayName": "ServicePrincipalName",
  "name": "http://ServicePrincipalName",
  "password": ...,
  "tenant": "XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"
}
```

Os valores `appId`, `tenant` e `password` são usados para autenticação. O `displayName` é usado ao procurar por uma entidade de serviço existente.

> [!NOTE]
> Se sua conta não tem permissões suficientes para criar um serviço principal, você verá uma mensagem de erro contendo “Privilégios insuficientes para concluir a operação”. Entre em contato com o administrador do Azure Active Directory para criar uma entidade de serviço.

## <a name="manage-service-principal-roles"></a>Gerenciar funções da entidade de serviço

A CLI do Azure fornece os comandos a seguir para gerenciar atribuições de função.

* [az role assignment list](/cli/azure/role/assignment#az-role-assignment-list)
* [az role assignment create](/cli/azure/role/assignment#az-role-assignment-create)
* [az role assignment delete](/cli/azure/role/assignment#az-role-assignment-delete)

A função padrão para uma entidade de serviço é **Colaborador**. Essa função tem permissões completas para ler e gravar em uma conta do Azure e não é adequada para aplicativos. A função **Leitor** é mais restritiva, oferecendo acesso somente leitura.  Para obter mais informações sobre Controle de acesso baseado em função (RBAC) e funções, consulte [RBAC: funções internas](/azure/active-directory/role-based-access-built-in-roles).

Esse exemplo adiciona a função **Leitor** e exclui a de **Colaborador**.

```azurecli-interactive
az role assignment create --assignee APP_ID --role Reader
az role assignment delete --assignee APP_ID --role Contributor
```

Adicionar uma função _não_ altera as permissões atribuídas anteriormente. Ao restringir as permissões da entidade de serviço, a função __Colaborador__ sempre deve ser removida.

As alterações podem ser verificadas, listando as funções atribuídas.

```azurecli-interactive
az role assignment list --assignee APP_ID
```

> [!NOTE]
> Caso sua conta não tiver permissões suficientes para atribuir uma função, você verá uma mensagem de erro informando que sua conta “não tem autorização para executar a ação ‘Microsoft.Authorization/roleAssignments/write' over scope '/subscriptions/{guid}’”. Entre em contato com o administrador do Azure Active Directory para gerenciar funções.

## <a name="sign-in-using-the-service-principal"></a>Entrar usando a entidade de serviço

Você pode testar as credenciais e as permissões e da nova entidade de serviço conectando na CLI do Azure. Entre como a nova entidade de serviço usando os valores `appId`, `tenant` e de credenciais. Use o tipo de autenticação criado com a entidade de serviço.

Para entrar com uma senha, forneça-a como um parâmetro de argumento.

```azurecli-interactive
az login --service-principal --username APP_ID --password PASSWORD --tenant TENANT_ID
```

Para entrar com um certificado, ele deve estar disponível localmente como um arquivo PEM ou DER.

```azurecli-interactive
az login --service-principal --username APP_ID --tenant TENANT_ID --password PATH_TO_CERT
```

## <a name="reset-credentials"></a>Redefinir credenciais

Caso esqueça as credenciais de uma entidade de serviço, elas podem ser redefinidas com o comando [az ad sp credential reset](/cli/azure/ad/sp/credential#az-ad-sp-credential-reset). As mesmas restrições e opções para criar uma nova entidade de serviço também se aplicam aqui.

```azurecli-interactive
az ad sp credential reset --name APP_ID --password NEW_PASSWORD
```
