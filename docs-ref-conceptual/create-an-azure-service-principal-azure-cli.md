---
title: Usar entidades de serviço do Azure com a CLI do Azure
description: Saiba como criar e usar uma entidade de serviço com a CLI do Azure.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 6cce8fb47dd2b57180487441055333343fff8330
ms.sourcegitcommit: 614811ea63ceb0e71bd99323846dc1b754e15255
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/28/2018
ms.locfileid: "53805866"
---
# <a name="create-an-azure-service-principal-with-azure-cli"></a><span data-ttu-id="e82c0-103">Criar uma entidade de serviço do Azure com a CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="e82c0-103">Create an Azure service principal with Azure CLI</span></span>

<span data-ttu-id="e82c0-104">Caso queira criar uma conexão separada com restrições de acesso, é possível fazer isso com uma entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="e82c0-104">If you want to create a separate sign-in with access restrictions, you can do so through a service principal.</span></span> <span data-ttu-id="e82c0-105">Entidades de serviço são identidades separadas que podem ser associadas a uma conta.</span><span class="sxs-lookup"><span data-stu-id="e82c0-105">Service principals are separate identities that can be associated with an account.</span></span> <span data-ttu-id="e82c0-106">Entidades de serviço são úteis para trabalhar com aplicativos e tarefas que devem ser automatizadas.</span><span class="sxs-lookup"><span data-stu-id="e82c0-106">Service principals are useful for working with applications and tasks that must be automated.</span></span> <span data-ttu-id="e82c0-107">Este artigo guia você pelas etapas de criação de uma entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="e82c0-107">This article runs you through the steps for creating a service principal.</span></span>

## <a name="create-the-service-principal"></a><span data-ttu-id="e82c0-108">Criar a entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="e82c0-108">Create the service principal</span></span>

<span data-ttu-id="e82c0-109">Use o comando [az ad sp create-for-rbac](/cli/azure/ad/sp#az-ad-sp-create-for-rbac) para criar uma entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="e82c0-109">Use the [az ad sp create-for-rbac](/cli/azure/ad/sp#az-ad-sp-create-for-rbac) command to create a service principal.</span></span> <span data-ttu-id="e82c0-110">O nome da entidade de serviço não está vinculado a nenhum aplicativo ou nome de usuário existente.</span><span class="sxs-lookup"><span data-stu-id="e82c0-110">The Service Principal's name isn't tied to any existing application or user name.</span></span> <span data-ttu-id="e82c0-111">Você pode criar uma entidade de serviço com a escolha do tipo de autenticação.</span><span class="sxs-lookup"><span data-stu-id="e82c0-111">You can create a service principal with your choice of authentication type.</span></span>

* <span data-ttu-id="e82c0-112">`--password` é usado para autenticação baseada em senha.</span><span class="sxs-lookup"><span data-stu-id="e82c0-112">`--password` is used for password-based authentication.</span></span> <span data-ttu-id="e82c0-113">Se um argumento que indica o tipo de autenticação não for incluído, --senha é usada por padrão e uma é criada para você.</span><span class="sxs-lookup"><span data-stu-id="e82c0-113">If an argument indicating the authentication type isn't included, --password is used by default, and one is created for you.</span></span> <span data-ttu-id="e82c0-114">Se você quiser usar a autenticação baseada em senha, é recomendável usar esse comando, portanto, a senha é criada para você.</span><span class="sxs-lookup"><span data-stu-id="e82c0-114">If you want to use password-based authentication, we recommend using this command, so the password is created for you.</span></span>  

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName 
  ```
  <span data-ttu-id="e82c0-115">Se você quiser escolher a senha, em vez de ela ser criada para você (não recomendado, por motivos de segurança), você pode usar esse comando.</span><span class="sxs-lookup"><span data-stu-id="e82c0-115">If you want to choose the password, instead of it being created for you (which is not recommended, for security reasons), you can use this command.</span></span> <span data-ttu-id="e82c0-116">Verifique se você criou uma senha forte, seguindo as [regras e restrições de senha do Azure Active Directory](/azure/active-directory/active-directory-passwords-policy).</span><span class="sxs-lookup"><span data-stu-id="e82c0-116">Make sure that you create a strong password by following the [Azure Active Directory password rules and restrictions](/azure/active-directory/active-directory-passwords-policy).</span></span> <span data-ttu-id="e82c0-117">A opção de escolher senha deixa a chance de uma senha fraca ser escolhida ou da senha ser usada novamente.</span><span class="sxs-lookup"><span data-stu-id="e82c0-117">The option to choose password leaves the chance of a weak password being chosen or password being re-used.</span></span> <span data-ttu-id="e82c0-118">Essa opção está planejada para ser substituída em uma versão futura da CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="e82c0-118">This option is planned to be deprecated in a future version of Azure CLI.</span></span> 

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --password <Choose a strong password>
  ```

* <span data-ttu-id="e82c0-119">`--cert` é usado para autenticação baseada em certificado para um certificado existente, como uma cadeia de caracteres pública PEM ou DER, ou `@{file}` para carregar um arquivo.</span><span class="sxs-lookup"><span data-stu-id="e82c0-119">`--cert` is used for certificate-based authentication for an existing certificate, either as a PEM or DER public string, or `@{file}` to load a file.</span></span>

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --cert {CertStringOrFile}
  ```

  <span data-ttu-id="e82c0-120">O argumento `--keyvault` pode ser adicionado para indicar que o certificado está armazenado no Azure Key Vault.</span><span class="sxs-lookup"><span data-stu-id="e82c0-120">The `--keyvault` argument can be added to indicate the cert is stored in Azure Key Vault.</span></span> <span data-ttu-id="e82c0-121">Nesse caso, o valor `--cert` se refere ao nome do certificado no Key Vault.</span><span class="sxs-lookup"><span data-stu-id="e82c0-121">In this case, the `--cert` value refers to the name of the certificate in Key Vault.</span></span>

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --cert CertName --keyvault VaultName
  ```

* <span data-ttu-id="e82c0-122">`--create-cert` cria um certificado _autoassinado_ para autenticação.</span><span class="sxs-lookup"><span data-stu-id="e82c0-122">`--create-cert` creates a _self-signed_ certificate for authentication.</span></span> <span data-ttu-id="e82c0-123">Se o argumento `--cert` não for fornecido, será gerado um nome de certificado aleatório.</span><span class="sxs-lookup"><span data-stu-id="e82c0-123">If the `--cert` argument isn't provided, a random certificate name is generated.</span></span>

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --create-cert
  ```

  <span data-ttu-id="e82c0-124">O argumento `--keyvault` pode ser adicionado para armazenar o certificado no Azure Key Vault.</span><span class="sxs-lookup"><span data-stu-id="e82c0-124">The `--keyvault` argument can be added to store the certificate in Azure Key Vault.</span></span> <span data-ttu-id="e82c0-125">Ao usar `--keyvault`, o argumento `--cert` também é necessário.</span><span class="sxs-lookup"><span data-stu-id="e82c0-125">When using `--keyvault`, the `--cert` argument is also required.</span></span>

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --create-cert --cert CertName --keyvault VaultName
  ```

<span data-ttu-id="e82c0-126">Se um argumento que indica o tipo de autenticação não for incluído, `--password` é usado por padrão.</span><span class="sxs-lookup"><span data-stu-id="e82c0-126">If an argument indicating the authentication type isn't included, `--password` is used by default.</span></span>

<span data-ttu-id="e82c0-127">A saída JSON do comando `create-for-rbac` está no seguinte formato:</span><span class="sxs-lookup"><span data-stu-id="e82c0-127">The JSON output of the `create-for-rbac` command is in the following format:</span></span>

```json
{
  "appId": "APP_ID",
  "displayName": "ServicePrincipalName",
  "name": "http://ServicePrincipalName",
  "password": ...,
  "tenant": "XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"
}
```

<span data-ttu-id="e82c0-128">Os valores `appId`, `tenant` e `password` são usados para autenticação.</span><span class="sxs-lookup"><span data-stu-id="e82c0-128">The `appId`, `tenant`, and `password` values are used for authentication.</span></span> <span data-ttu-id="e82c0-129">O `displayName` é usado ao procurar por uma entidade de serviço existente.</span><span class="sxs-lookup"><span data-stu-id="e82c0-129">The `displayName` is used when searching for an existing service principal.</span></span>

> [!NOTE]
> <span data-ttu-id="e82c0-130">Se sua conta não tem permissões suficientes para criar um serviço principal, você verá uma mensagem de erro contendo “Privilégios insuficientes para concluir a operação”.</span><span class="sxs-lookup"><span data-stu-id="e82c0-130">If your account does not have sufficient permissions to create a service principal, you see an error message containing "Insufficient privileges to complete the operation."</span></span> <span data-ttu-id="e82c0-131">Entre em contato com o administrador do Azure Active Directory para criar uma entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="e82c0-131">Contact your Azure Active Directory admin to create a service principal.</span></span>

## <a name="manage-service-principal-roles"></a><span data-ttu-id="e82c0-132">Gerenciar funções da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="e82c0-132">Manage service principal roles</span></span>

<span data-ttu-id="e82c0-133">A CLI do Azure fornece os comandos a seguir para gerenciar atribuições de função.</span><span class="sxs-lookup"><span data-stu-id="e82c0-133">The Azure CLI provides the following commands to manage role assignments.</span></span>

* [<span data-ttu-id="e82c0-134">az role assignment list</span><span class="sxs-lookup"><span data-stu-id="e82c0-134">az role assignment list</span></span>](/cli/azure/role/assignment#az-role-assignment-list)
* [<span data-ttu-id="e82c0-135">az role assignment create</span><span class="sxs-lookup"><span data-stu-id="e82c0-135">az role assignment create</span></span>](/cli/azure/role/assignment#az-role-assignment-create)
* [<span data-ttu-id="e82c0-136">az role assignment delete</span><span class="sxs-lookup"><span data-stu-id="e82c0-136">az role assignment delete</span></span>](/cli/azure/role/assignment#az-role-assignment-delete)

<span data-ttu-id="e82c0-137">A função padrão para uma entidade de serviço é **Colaborador**.</span><span class="sxs-lookup"><span data-stu-id="e82c0-137">The default role for a service principal is **Contributor**.</span></span> <span data-ttu-id="e82c0-138">Essa função tem permissões completas para ler e gravar em uma conta do Azure e não é adequada para aplicativos.</span><span class="sxs-lookup"><span data-stu-id="e82c0-138">This role has full permissions to read and write to an Azure account, and is not appropriate for applications.</span></span> <span data-ttu-id="e82c0-139">A função **Leitor** é mais restritiva, oferecendo acesso somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e82c0-139">The **Reader** role is more restrictive, providing read-only access.</span></span>  <span data-ttu-id="e82c0-140">Para obter mais informações sobre o Controle de Acesso Baseado em Função (RBAC) e funções, confira [RBAC: funções internas](/azure/active-directory/role-based-access-built-in-roles).</span><span class="sxs-lookup"><span data-stu-id="e82c0-140">For more information on Role-Based Access Control (RBAC) and roles, see [RBAC: Built-in roles](/azure/active-directory/role-based-access-built-in-roles).</span></span>

<span data-ttu-id="e82c0-141">Esse exemplo adiciona a função **Leitor** e exclui a de **Colaborador**.</span><span class="sxs-lookup"><span data-stu-id="e82c0-141">This example adds the **Reader** role and deletes the **Contributor** one.</span></span>

```azurecli-interactive
az role assignment create --assignee APP_ID --role Reader
az role assignment delete --assignee APP_ID --role Contributor
```

<span data-ttu-id="e82c0-142">Adicionar uma função _não_ altera as permissões atribuídas anteriormente.</span><span class="sxs-lookup"><span data-stu-id="e82c0-142">Adding a role does _not_ change any previously assigned permissions.</span></span> <span data-ttu-id="e82c0-143">Ao restringir as permissões da entidade de serviço, a função __Colaborador__ sempre deve ser removida.</span><span class="sxs-lookup"><span data-stu-id="e82c0-143">When restricting a service principal's permissions, the __Contributor__ role should always be removed.</span></span>

<span data-ttu-id="e82c0-144">As alterações podem ser verificadas, listando as funções atribuídas.</span><span class="sxs-lookup"><span data-stu-id="e82c0-144">The changes can be verified by listing the assigned roles.</span></span>

```azurecli-interactive
az role assignment list --assignee APP_ID
```

> [!NOTE]
> <span data-ttu-id="e82c0-145">Caso sua conta não tiver permissões suficientes para atribuir uma função, você verá uma mensagem de erro informando que sua conta “não tem autorização para executar a ação ‘Microsoft.Authorization/roleAssignments/write' over scope '/subscriptions/{guid}’”. Entre em contato com o administrador do Azure Active Directory para gerenciar funções.</span><span class="sxs-lookup"><span data-stu-id="e82c0-145">If your account doesn't have the permissions to assign a role, you see an error message that your account "does not have authorization to perform action 'Microsoft.Authorization/roleAssignments/write' over scope '/subscriptions/{guid}'." Contact your Azure Active Directory admin to manage roles.</span></span>

## <a name="sign-in-using-the-service-principal"></a><span data-ttu-id="e82c0-146">Entrar usando a entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="e82c0-146">Sign in using the service principal</span></span>

<span data-ttu-id="e82c0-147">Você pode testar as credenciais e as permissões e da nova entidade de serviço conectando na CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="e82c0-147">You can test the new service principal's credentials and permissions by signing in under it within the Azure CLI.</span></span> <span data-ttu-id="e82c0-148">Entre como a nova entidade de serviço usando os valores `appId`, `tenant` e de credenciais.</span><span class="sxs-lookup"><span data-stu-id="e82c0-148">Sign in as the new service principal using the `appId`, `tenant`, and credentials values.</span></span> <span data-ttu-id="e82c0-149">Use o tipo de autenticação criado com a entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="e82c0-149">Use the authentication type that the service principal was created with.</span></span>

<span data-ttu-id="e82c0-150">Para entrar com uma senha, forneça-a como um parâmetro de argumento.</span><span class="sxs-lookup"><span data-stu-id="e82c0-150">To sign in with a password, provide it as an argument parameter.</span></span>

```azurecli-interactive
az login --service-principal --username APP_ID --password PASSWORD --tenant TENANT_ID
```

<span data-ttu-id="e82c0-151">Para entrar com um certificado, ele deve estar disponível localmente como um arquivo PEM ou DER.</span><span class="sxs-lookup"><span data-stu-id="e82c0-151">To sign in with a certificate, it must be available locally as a PEM or DER file.</span></span>

```azurecli-interactive
az login --service-principal --username APP_ID --tenant TENANT_ID --password PATH_TO_CERT
```

## <a name="reset-credentials"></a><span data-ttu-id="e82c0-152">Redefinir credenciais</span><span class="sxs-lookup"><span data-stu-id="e82c0-152">Reset credentials</span></span>

<span data-ttu-id="e82c0-153">Caso esqueça as credenciais de uma entidade de serviço, elas podem ser redefinidas com o comando [az ad sp credential reset](/cli/azure/ad/sp/credential#az-ad-sp-credential-reset).</span><span class="sxs-lookup"><span data-stu-id="e82c0-153">In the event that you forget the credentials for a service principal, they can be reset with the [az ad sp credential reset](/cli/azure/ad/sp/credential#az-ad-sp-credential-reset) command.</span></span> <span data-ttu-id="e82c0-154">As mesmas restrições e opções para criar uma nova entidade de serviço também se aplicam aqui.</span><span class="sxs-lookup"><span data-stu-id="e82c0-154">The same restrictions and options for creating a new service principal also apply here.</span></span>

```azurecli-interactive
az ad sp credential reset --name APP_ID 
```
