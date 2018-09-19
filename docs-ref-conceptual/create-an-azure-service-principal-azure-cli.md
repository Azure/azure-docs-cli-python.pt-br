---
title: Usar entidades de serviço do Azure com a CLI do Azure 2.0
description: Saiba como criar e usar uma entidade de serviço com a CLI do Azure 2.0.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.technology: azure-cli
ms.devlang: azure-cli
ms.service: role-based-access-control
ms.openlocfilehash: 5f98fd8d3897b11a9b37eefa6295b8b25b2b1c95
ms.sourcegitcommit: 0e688704889fc88b91588bb6678a933c2d54f020
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/11/2018
ms.locfileid: "44388432"
---
# <a name="create-an-azure-service-principal-with-azure-cli-20"></a><span data-ttu-id="dfb10-103">Criar uma entidade de serviço do Azure com a CLI do Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="dfb10-103">Create an Azure service principal with Azure CLI 2.0</span></span>

<span data-ttu-id="dfb10-104">Caso queira criar uma conexão separada com restrições de acesso, é possível fazer isso com uma entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="dfb10-104">If you want to create a separate sign-in with access restrictions, you can do so through a service principal.</span></span> <span data-ttu-id="dfb10-105">Entidades de serviço são identidades separadas que podem ser associadas a uma conta.</span><span class="sxs-lookup"><span data-stu-id="dfb10-105">Service principals are separate identities that can be associated with an account.</span></span> <span data-ttu-id="dfb10-106">Entidades de serviço são úteis para trabalhar com aplicativos e tarefas que devem ser automatizadas.</span><span class="sxs-lookup"><span data-stu-id="dfb10-106">Service principals are useful for working with applications and tasks that must be automated.</span></span> <span data-ttu-id="dfb10-107">Este artigo guia você pelas etapas de criação de uma entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="dfb10-107">This article runs you through the steps for creating a service principal.</span></span>

## <a name="create-the-service-principal"></a><span data-ttu-id="dfb10-108">Criar a entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="dfb10-108">Create the service principal</span></span>

<span data-ttu-id="dfb10-109">Use o comando [az ad sp create-for-rbac](/cli/azure/ad/sp#az-ad-sp-create-for-rbac) para criar uma entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="dfb10-109">Use the [az ad sp create-for-rbac](/cli/azure/ad/sp#az-ad-sp-create-for-rbac) command to create a service principal.</span></span> <span data-ttu-id="dfb10-110">O nome da entidade de serviço não está vinculado a nenhum aplicativo ou nome de usuário existente.</span><span class="sxs-lookup"><span data-stu-id="dfb10-110">The Service Principal's name isn't tied to any existing application or user name.</span></span> <span data-ttu-id="dfb10-111">Você pode criar uma entidade de serviço com a escolha do tipo de autenticação.</span><span class="sxs-lookup"><span data-stu-id="dfb10-111">You can create a service principal with your choice of authentication type.</span></span>

* <span data-ttu-id="dfb10-112">`--password` é usado para autenticação baseada em senha.</span><span class="sxs-lookup"><span data-stu-id="dfb10-112">`--password` is used for password-based authentication.</span></span> <span data-ttu-id="dfb10-113">Verifique se você criou uma senha forte, seguindo as [regras e restrições de senha do Azure Active Directory](/azure/active-directory/active-directory-passwords-policy).</span><span class="sxs-lookup"><span data-stu-id="dfb10-113">Make sure that you create a strong password by following the [Azure Active Directory password rules and restrictions](/azure/active-directory/active-directory-passwords-policy).</span></span> <span data-ttu-id="dfb10-114">Caso não especifique uma senha, uma será criada para você.</span><span class="sxs-lookup"><span data-stu-id="dfb10-114">If you don't specify a password, one is created for you.</span></span>

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --password PASSWORD
  ```

* <span data-ttu-id="dfb10-115">`--cert` é usado para autenticação baseada em certificado para um certificado existente, como uma cadeia de caracteres pública PEM ou DER, ou `@{file}` para carregar um arquivo.</span><span class="sxs-lookup"><span data-stu-id="dfb10-115">`--cert` is used for certificate-based authentication for an existing certificate, either as a PEM or DER public string, or `@{file}` to load a file.</span></span>

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --cert {CertStringOrFile}
  ```

  <span data-ttu-id="dfb10-116">O argumento `--keyvault` pode ser adicionado para indicar que o certificado está armazenado no Azure Key Vault.</span><span class="sxs-lookup"><span data-stu-id="dfb10-116">The `--keyvault` argument can be added to indicate the cert is stored in Azure Key Vault.</span></span> <span data-ttu-id="dfb10-117">Nesse caso, o valor `--cert` se refere ao nome do certificado no Key Vault.</span><span class="sxs-lookup"><span data-stu-id="dfb10-117">In this case, the `--cert` value refers to the name of the certificate in Key Vault.</span></span>

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --cert CertName --keyvault VaultName
  ```

* <span data-ttu-id="dfb10-118">`--create-cert` cria um certificado _autoassinado_ para autenticação.</span><span class="sxs-lookup"><span data-stu-id="dfb10-118">`--create-cert` creates a _self-signed_ certificate for authentication.</span></span> <span data-ttu-id="dfb10-119">Se o argumento `--cert` não for fornecido, será gerado um nome de certificado aleatório.</span><span class="sxs-lookup"><span data-stu-id="dfb10-119">If the `--cert` argument isn't provided, a random certificate name is generated.</span></span>

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --create-cert
  ```

  <span data-ttu-id="dfb10-120">O argumento `--keyvault` pode ser adicionado para armazenar o certificado no Azure Key Vault.</span><span class="sxs-lookup"><span data-stu-id="dfb10-120">The `--keyvault` argument can be added to store the certificate in Azure Key Vault.</span></span> <span data-ttu-id="dfb10-121">Ao usar `--keyvault`, o argumento `--cert` também é necessário.</span><span class="sxs-lookup"><span data-stu-id="dfb10-121">When using `--keyvault`, the `--cert` argument is also required.</span></span>

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --create-cert --cert CertName --keyvault VaultName
  ```

<span data-ttu-id="dfb10-122">Se um argumento que indica o tipo de autenticação não for incluído, `--password` é usado por padrão.</span><span class="sxs-lookup"><span data-stu-id="dfb10-122">If an argument indicating the authentication type isn't included, `--password` is used by default.</span></span>

<span data-ttu-id="dfb10-123">A saída do comando `create-for-rbac` está neste formato:</span><span class="sxs-lookup"><span data-stu-id="dfb10-123">The output of the `create-for-rbac` command is in the following format:</span></span>

```json
{
  "appId": "APP_ID",
  "displayName": "ServicePrincipalName",
  "name": "http://ServicePrincipalName",
  "password": ...,
  "tenant": "XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"
}
```

<span data-ttu-id="dfb10-124">Os valores `appId`, `tenant` e `password` são usados para autenticação.</span><span class="sxs-lookup"><span data-stu-id="dfb10-124">The `appId`, `tenant`, and `password` values are used for authentication.</span></span> <span data-ttu-id="dfb10-125">O `displayName` é usado ao procurar por uma entidade de serviço existente.</span><span class="sxs-lookup"><span data-stu-id="dfb10-125">The `displayName` is used when searching for an existing service principal.</span></span>

> [!NOTE]
> <span data-ttu-id="dfb10-126">Se sua conta não tem permissões suficientes para criar um serviço principal, você verá uma mensagem de erro contendo “Privilégios insuficientes para concluir a operação”.</span><span class="sxs-lookup"><span data-stu-id="dfb10-126">If your account does not have sufficient permissions to create a service principal, you see an error message containing "Insufficient privileges to complete the operation."</span></span> <span data-ttu-id="dfb10-127">Entre em contato com o administrador do Azure Active Directory para criar uma entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="dfb10-127">Contact your Azure Active Directory admin to create a service principal.</span></span>

## <a name="manage-service-principal-roles"></a><span data-ttu-id="dfb10-128">Gerenciar funções da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="dfb10-128">Manage service principal roles</span></span>

<span data-ttu-id="dfb10-129">A CLI do Azure 2.0 fornece os comandos a seguir para gerenciar atribuições de função.</span><span class="sxs-lookup"><span data-stu-id="dfb10-129">The Azure CLI 2.0 provides the following commands to manage role assignments.</span></span>

* [<span data-ttu-id="dfb10-130">az role assignment list</span><span class="sxs-lookup"><span data-stu-id="dfb10-130">az role assignment list</span></span>](/cli/azure/role/assignment#az-role-assignment-list)
* [<span data-ttu-id="dfb10-131">az role assignment create</span><span class="sxs-lookup"><span data-stu-id="dfb10-131">az role assignment create</span></span>](/cli/azure/role/assignment#az-role-assignment-create)
* [<span data-ttu-id="dfb10-132">az role assignment delete</span><span class="sxs-lookup"><span data-stu-id="dfb10-132">az role assignment delete</span></span>](/cli/azure/role/assignment#az-role-assignment-delete)

<span data-ttu-id="dfb10-133">A função padrão para uma entidade de serviço é **Colaborador**.</span><span class="sxs-lookup"><span data-stu-id="dfb10-133">The default role for a service principal is **Contributor**.</span></span> <span data-ttu-id="dfb10-134">Essa função tem permissões completas para ler e gravar em uma conta do Azure e não é adequada para aplicativos.</span><span class="sxs-lookup"><span data-stu-id="dfb10-134">This role has full permissions to read and write to an Azure account, and is not appropriate for applications.</span></span> <span data-ttu-id="dfb10-135">A função **Leitor** é mais restritiva, oferecendo acesso somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dfb10-135">The **Reader** role is more restrictive, providing read-only access.</span></span>  <span data-ttu-id="dfb10-136">Para obter mais informações sobre Controle de acesso baseado em função (RBAC) e funções, consulte [RBAC: funções internas](/azure/active-directory/role-based-access-built-in-roles).</span><span class="sxs-lookup"><span data-stu-id="dfb10-136">For more information on Role-Based Access Control (RBAC) and roles, see [RBAC: Built-in roles](/azure/active-directory/role-based-access-built-in-roles).</span></span>

<span data-ttu-id="dfb10-137">Esse exemplo adiciona a função **Leitor** e exclui a de **Colaborador**.</span><span class="sxs-lookup"><span data-stu-id="dfb10-137">This example adds the **Reader** role and deletes the **Contributor** one.</span></span>

```azurecli-interactive
az role assignment create --assignee APP_ID --role Reader
az role assignment delete --assignee APP_ID --role Contributor
```

<span data-ttu-id="dfb10-138">Adicionar uma função _não_ altera as permissões atribuídas anteriormente.</span><span class="sxs-lookup"><span data-stu-id="dfb10-138">Adding a role does _not_ change any previously assigned permissions.</span></span> <span data-ttu-id="dfb10-139">Ao restringir as permissões da entidade de serviço, a função __Colaborador__ sempre deve ser removida.</span><span class="sxs-lookup"><span data-stu-id="dfb10-139">When restricting a service principal's permissions, the __Contributor__ role should always be removed.</span></span>

<span data-ttu-id="dfb10-140">As alterações podem ser verificadas, listando as funções atribuídas.</span><span class="sxs-lookup"><span data-stu-id="dfb10-140">The changes can be verified by listing the assigned roles.</span></span>

```azurecli-interactive
az role assignment list --assignee APP_ID
```

> [!NOTE]
> <span data-ttu-id="dfb10-141">Caso sua conta não tiver permissões suficientes para atribuir uma função, você verá uma mensagem de erro informando que sua conta “não tem autorização para executar a ação ‘Microsoft.Authorization/roleAssignments/write' over scope '/subscriptions/{guid}’”. Entre em contato com o administrador do Azure Active Directory para gerenciar funções.</span><span class="sxs-lookup"><span data-stu-id="dfb10-141">If your account doesn't have the permissions to assign a role, you see an error message that your account "does not have authorization to perform action 'Microsoft.Authorization/roleAssignments/write' over scope '/subscriptions/{guid}'." Contact your Azure Active Directory admin to manage roles.</span></span>

## <a name="sign-in-using-the-service-principal"></a><span data-ttu-id="dfb10-142">Entrar usando a entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="dfb10-142">Sign in using the service principal</span></span>

<span data-ttu-id="dfb10-143">Você pode testar as credenciais e as permissões e da nova entidade de serviço conectando na CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="dfb10-143">You can test the new service principal's credentials and permissions by signing in under it within the Azure CLI.</span></span> <span data-ttu-id="dfb10-144">Entre como a nova entidade de serviço usando os valores `appId`, `tenant` e de credenciais.</span><span class="sxs-lookup"><span data-stu-id="dfb10-144">Sign in as the new service principal using the `appId`, `tenant`, and credentials values.</span></span> <span data-ttu-id="dfb10-145">Use o tipo de autenticação criado com a entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="dfb10-145">Use the authentication type that the service principal was created with.</span></span>

<span data-ttu-id="dfb10-146">Para entrar com uma senha, forneça-a como um parâmetro de argumento.</span><span class="sxs-lookup"><span data-stu-id="dfb10-146">To sign in with a password, provide it as an argument parameter.</span></span>

```azurecli-interactive
az login --service-principal --username APP_ID --password PASSWORD --tenant TENANT_ID
```

<span data-ttu-id="dfb10-147">Para entrar com um certificado, ele deve estar disponível localmente como um arquivo PEM ou DER.</span><span class="sxs-lookup"><span data-stu-id="dfb10-147">To sign in with a certificate, it must be available locally as a PEM or DER file.</span></span>

```azurecli-interactive
az login --service-principal --username APP_ID --tenant TENANT_ID --password PATH_TO_CERT
```

## <a name="reset-credentials"></a><span data-ttu-id="dfb10-148">Redefinir credenciais</span><span class="sxs-lookup"><span data-stu-id="dfb10-148">Reset credentials</span></span>

<span data-ttu-id="dfb10-149">Caso esqueça as credenciais de uma entidade de serviço, elas podem ser redefinidas com o comando [az ad sp credential reset](/cli/azure/ad/sp/credential#az-ad-sp-credential-reset).</span><span class="sxs-lookup"><span data-stu-id="dfb10-149">In the event that you forget the credentials for a service principal, they can be reset with the [az ad sp credential reset](/cli/azure/ad/sp/credential#az-ad-sp-credential-reset) command.</span></span> <span data-ttu-id="dfb10-150">As mesmas restrições e opções para criar uma nova entidade de serviço também se aplicam aqui.</span><span class="sxs-lookup"><span data-stu-id="dfb10-150">The same restrictions and options for creating a new service principal also apply here.</span></span>

```azurecli-interactive
az ad sp credential reset --name APP_ID --password NEW_PASSWORD
```
