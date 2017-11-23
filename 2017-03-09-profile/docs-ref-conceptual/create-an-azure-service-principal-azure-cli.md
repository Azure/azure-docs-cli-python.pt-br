---
title: "Criar uma entidade de serviço do Azure com a CLI do Azure 2.0"
description: "Saiba como criar uma entidade de serviço para seu aplicativo ou serviço com a CLI do Azure 2.0."
keywords: CLI do Azure 2.0, Azure Active Directory, Azure Active directory, AD, RBAC
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 10/12/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: fab89cb8-dac1-4e21-9d34-5eadd5213c05
ms.openlocfilehash: a6ad5611f3e507b65e160122c87e22ec44546588
ms.sourcegitcommit: 0149f195a0d9f0ea9b7ff5c6e00ad4242223a1a8
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2017
---
# <a name="create-an-azure-service-principal-with-azure-cli-20"></a><span data-ttu-id="db3de-104">Criar uma entidade de serviço do Azure com a CLI do Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="db3de-104">Create an Azure service principal with Azure CLI 2.0</span></span>

<span data-ttu-id="db3de-105">Se você planeja gerenciar seu aplicativo ou serviço com a CLI do Azure 2.0, execute-a em uma entidade de serviço do Azure Active Directory (AAD) em vez de suas próprias credenciais.</span><span class="sxs-lookup"><span data-stu-id="db3de-105">If you plan to manage your app or service with Azure CLI 2.0, you should run it under an Azure Active Directory (AAD) service principal rather than your own credentials.</span></span>
<span data-ttu-id="db3de-106">Esse tópico orienta você pela criação de uma entidade de segurança com a CLI do Azure 2.0.</span><span class="sxs-lookup"><span data-stu-id="db3de-106">This topic steps you through creating a security principal with Azure CLI 2.0.</span></span>

> [!NOTE]
> <span data-ttu-id="db3de-107">Você também pode criar uma entidade de serviço por meio do Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="db3de-107">You can also create a service principal through the Azure portal.</span></span>
> <span data-ttu-id="db3de-108">Leia [Usar o portal para criar um aplicativo e entidade de serviço do Active Directory que pode acessar recursos](/azure/azure-resource-manager/resource-group-create-service-principal-portal) para obter mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="db3de-108">Read [Use portal to create Active Directory application and service principal that can access resources](/azure/azure-resource-manager/resource-group-create-service-principal-portal) for more details.</span></span>

## <a name="what-is-a-service-principal"></a><span data-ttu-id="db3de-109">O que é uma ‘entidade de serviço’?</span><span class="sxs-lookup"><span data-stu-id="db3de-109">What is a 'service principal'?</span></span>

<span data-ttu-id="db3de-110">Uma entidade de serviço do Azure é uma identidade de segurança usada por aplicativos criados pelo usuário, serviços e ferramentas de automação para acessar recursos específicos do Azure.</span><span class="sxs-lookup"><span data-stu-id="db3de-110">An Azure service principal is a security identity used by user-created apps, services, and automation tools to access specific Azure resources.</span></span> <span data-ttu-id="db3de-111">Pense nela como uma 'identidade de usuário' (login e senha ou certificado) com uma função específica e permissões de acesso aos seus recursos rigidamente controladas.</span><span class="sxs-lookup"><span data-stu-id="db3de-111">Think of it as a 'user identity' (login and password or certificate) with a specific role, and tightly controlled permissions to access your resources.</span></span> <span data-ttu-id="db3de-112">Ela só precisa ser capaz de fazer coisas específicas, ao contrário de uma identidade de usuário geral.</span><span class="sxs-lookup"><span data-stu-id="db3de-112">It only needs to be able to do specific things, unlike a general user identity.</span></span> <span data-ttu-id="db3de-113">A segurança aumenta se você só conceder a ela o nível mínimo de permissões necessárias para realizar suas tarefas de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="db3de-113">It improves security if you only grant it the minimum permissions level needed to perform its management tasks.</span></span> 

<span data-ttu-id="db3de-114">A CLI do Azure 2.0 oferece suporte à criação de credenciais de autenticação baseadas em senha e credenciais de certificado.</span><span class="sxs-lookup"><span data-stu-id="db3de-114">Azure CLI 2.0 supports the creation of password-based authentication credentials and certificate credentials.</span></span> <span data-ttu-id="db3de-115">Neste tópico, abordaremos os dois tipos de credenciais.</span><span class="sxs-lookup"><span data-stu-id="db3de-115">In this topic, we cover both types of credentials.</span></span>

## <a name="verify-your-own-permission-level"></a><span data-ttu-id="db3de-116">Verificar seu próprio nível de permissão</span><span class="sxs-lookup"><span data-stu-id="db3de-116">Verify your own permission level</span></span>

<span data-ttu-id="db3de-117">Primeiro, você deve ter permissões suficientes no Azure Active Directory e em sua assinatura do Azure.</span><span class="sxs-lookup"><span data-stu-id="db3de-117">First, you must have sufficient permissions in both your Azure Active Directory and your Azure subscription.</span></span> <span data-ttu-id="db3de-118">Especificamente, você deve ser capaz de criar um aplicativo no Active Directory e atribuir uma função à entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="db3de-118">Specifically, you must be able to create an app in the Active Directory, and assign a role to the service principal.</span></span> 

<span data-ttu-id="db3de-119">A maneira mais fácil de verificar se a sua conta tem as permissões adequadas é por meio do portal.</span><span class="sxs-lookup"><span data-stu-id="db3de-119">The easiest way to check whether your account has adequate permissions is through the portal.</span></span> <span data-ttu-id="db3de-120">Consulte [Verificar permissão necessária no portal](/azure/azure-resource-manager/resource-group-create-service-principal-portal#required-permissions).</span><span class="sxs-lookup"><span data-stu-id="db3de-120">See [Check required permission in portal](/azure/azure-resource-manager/resource-group-create-service-principal-portal#required-permissions).</span></span>

## <a name="create-a-service-principal-for-your-application"></a><span data-ttu-id="db3de-121">Crie uma entidade de serviço para seu aplicativo</span><span class="sxs-lookup"><span data-stu-id="db3de-121">Create a service principal for your application</span></span>

<span data-ttu-id="db3de-122">Você deve ter um dos itens a seguir para identificar o aplicativo para o qual você deseja criar uma entidade de serviço:</span><span class="sxs-lookup"><span data-stu-id="db3de-122">You must have one of the following to identify the app you want to create a service principal for:</span></span>

  * <span data-ttu-id="db3de-123">o nome exclusivo ou URI do seu aplicativo implantado (como "MyDemoWebApp" nos exemplos) ou</span><span class="sxs-lookup"><span data-stu-id="db3de-123">The unique name or URI of your deployed app (such as "MyDemoWebApp" in the examples), or</span></span>
  * <span data-ttu-id="db3de-124">a ID do Aplicativo, o GUID exclusivo associado ao aplicativo, serviço ou objeto implantado</span><span class="sxs-lookup"><span data-stu-id="db3de-124">the Application ID, the unique GUID associated with your deployed app, service, or object</span></span>

<span data-ttu-id="db3de-125">Esses valores identificam seu aplicativo durante a criação de uma entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="db3de-125">These values identify your application when creating a service principal.</span></span>

### <a name="get-information-about-your-application"></a><span data-ttu-id="db3de-126">Obter informações sobre seu aplicativo</span><span class="sxs-lookup"><span data-stu-id="db3de-126">Get information about your application</span></span>

<span data-ttu-id="db3de-127">Obtenha informações sobre seu aplicativo com a `az ad app list`.</span><span class="sxs-lookup"><span data-stu-id="db3de-127">Get identity information about your application with the `az ad app list`.</span></span>

[!INCLUDE [cloud-shell-try-it.md](includes/cloud-shell-try-it.md)]

```azurecli-interactive
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

<span data-ttu-id="db3de-128">O opção `--display-name` filtra a lista retornada de aplicativos para mostrá-los com o `displayName` começando com MyDemoWebApp.</span><span class="sxs-lookup"><span data-stu-id="db3de-128">The `--display-name` option filters the returned list of apps to show those with `displayName` starting with MyDemoWebApp.</span></span>

### <a name="create-a-service-principal-with-a-password"></a><span data-ttu-id="db3de-129">Criar uma entidade de serviço com uma senha</span><span class="sxs-lookup"><span data-stu-id="db3de-129">Create a service principal with a password</span></span>

<span data-ttu-id="db3de-130">Use [az ad sp create-for-rbac](/cli/azure/ad/sp#create-for-rbac) e o parâmetro `--password` para criar a entidade de serviço com uma senha.</span><span class="sxs-lookup"><span data-stu-id="db3de-130">Use [az ad sp create-for-rbac](/cli/azure/ad/sp#create-for-rbac) and the `--password` parameter to create the service principal with a password.</span></span> <span data-ttu-id="db3de-131">Quando você não fornece uma função ou escopo, o padrão é a função **Colaborador** para a assinatura atual.</span><span class="sxs-lookup"><span data-stu-id="db3de-131">When you do not provide a role or scope, it defaults to the **Contributor** role for the current subscription.</span></span> <span data-ttu-id="db3de-132">Se você criar uma entidade de serviço sem usar o parâmetro `--password` ou `--cert`, a autenticação de senha será usada e uma senha, gerada para você.</span><span class="sxs-lookup"><span data-stu-id="db3de-132">If you create a service principal without using either the `--password` or `--cert` parameter, password authentication is used and a password is generated for you.</span></span>

```azurecli-interactive
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
 > <span data-ttu-id="db3de-133">Não crie uma senha não segura.</span><span class="sxs-lookup"><span data-stu-id="db3de-133">Don't create an insecure password.</span></span>  <span data-ttu-id="db3de-134">Execute a orientação [Restrições e regras de senha do Azure AD](/azure/active-directory/active-directory-passwords-policy).</span><span class="sxs-lookup"><span data-stu-id="db3de-134">Follow the [Azure AD password rules and restrictions](/azure/active-directory/active-directory-passwords-policy) guidance.</span></span>

### <a name="create-a-service-principal-with-a-self-signed-certificate"></a><span data-ttu-id="db3de-135">Criar uma entidade de serviço com um certificado autoassinado</span><span class="sxs-lookup"><span data-stu-id="db3de-135">Create a service principal with a self-signed certificate</span></span>

<span data-ttu-id="db3de-136">Use [az ad sp create-for-rbac](/cli/azure/ad/sp#create-for-rbac) e o parâmetro `--create-cert` para criar um certificado autoassinado.</span><span class="sxs-lookup"><span data-stu-id="db3de-136">Use [az ad sp create-for-rbac](/cli/azure/ad/sp#create-for-rbac) and the `--create-cert` parameter to create a self-signed certificate.</span></span>

```azurecli-interactive
az ad sp create-for-rbac --name {appId} --create-cert
```

```json
{
  "appId": "c495db57-82e0-4e2e-9369-069dff176858",
  "displayName": "azure-cli-2017-10-12-22-15-38",
  "fileWithCertAndPrivateKey": "<path>/<file-name>.pem",
  "name": "http://MyDemoWebApp",
  "password": null,
  "tenant": "XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"
}
```

<span data-ttu-id="db3de-137">Copie o valor da resposta `fileWithCertAndPrivateKey`.</span><span class="sxs-lookup"><span data-stu-id="db3de-137">Copy the value of the `fileWithCertAndPrivateKey` response.</span></span> <span data-ttu-id="db3de-138">Este é o arquivo de certificado que será usado para a autenticação.</span><span class="sxs-lookup"><span data-stu-id="db3de-138">This is the certificate file which will be used for authentication.</span></span>

<span data-ttu-id="db3de-139">Para obter mais opções ao usar os certificados, consulte [az ad sp create-for-rbac](/cli/azure/ad/sp#create-for-rbac).</span><span class="sxs-lookup"><span data-stu-id="db3de-139">For more options when using certificates, see [az ad sp create-for-rbac](/cli/azure/ad/sp#create-for-rbac).</span></span>

### <a name="get-information-about-the-service-principal"></a><span data-ttu-id="db3de-140">Obter informações sobre a entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="db3de-140">Get information about the service principal</span></span>

```azurecli-interactive
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

### <a name="sign-in-using-the-service-principal"></a><span data-ttu-id="db3de-141">Entrar usando a entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="db3de-141">Sign in using the service principal</span></span>

<span data-ttu-id="db3de-142">Agora, você pode fazer logon como a nova entidade de serviço para seu aplicativo usando *appId* de `az ad sp show`e a *senha* ou o caminho para o certificado criado.</span><span class="sxs-lookup"><span data-stu-id="db3de-142">You can now log in as the new service principal for your app using the *appId* from `az ad sp show`, and either the *password* or the path to the created certificate.</span></span>  <span data-ttu-id="db3de-143">Forneça o valor *tenant* dos resultados de `az ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="db3de-143">Supply the *tenant* value from the results of `az ad sp create-for-rbac`.</span></span>

```azurecli-interactive
az login --service-principal -u a487e0c1-82af-47d9-9a0b-af184eb87646d --password {password-or-path-to-cert} --tenant {tenant}
``` 

<span data-ttu-id="db3de-144">Você verá essa saída após um logon bem-sucedido:</span><span class="sxs-lookup"><span data-stu-id="db3de-144">You will see this output after a successful sign-on:</span></span>

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

<span data-ttu-id="db3de-145">Use os valores `id`, `password` e `tenant` valores como as credenciais para a execução de seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="db3de-145">Use the `id`, `password`, and `tenant` values as the credentials for running your app.</span></span> 

## <a name="managing-roles"></a><span data-ttu-id="db3de-146">Gerenciamento de funções</span><span class="sxs-lookup"><span data-stu-id="db3de-146">Managing roles</span></span> 

> [!NOTE]
> <span data-ttu-id="db3de-147">O RBAC (Controle de Acesso do Azure Baseado em Função) é um modelo para definir e gerenciar funções para entidades de usuário e de serviço.</span><span class="sxs-lookup"><span data-stu-id="db3de-147">Azure Role-Based Access Control (RBAC) is a model for defining and managing roles for user and service principals.</span></span>
> <span data-ttu-id="db3de-148">As funções têm conjuntos de permissões associados a elas, que determinam os recursos que uma entidade pode ler, acessar, gravar ou gerenciar.</span><span class="sxs-lookup"><span data-stu-id="db3de-148">Roles have sets of permissions associated with them, which determine the resources a principal can read, access, write, or manage.</span></span>
> <span data-ttu-id="db3de-149">Para saber mais sobre funções e RBAC, consulte [RBAC: funções internas](/azure/active-directory/role-based-access-built-in-roles).</span><span class="sxs-lookup"><span data-stu-id="db3de-149">For more information on RBAC and roles, see [RBAC: Built-in roles](/azure/active-directory/role-based-access-built-in-roles).</span></span>

<span data-ttu-id="db3de-150">A CLI do Azure 2.0 fornece os seguintes comandos para gerenciar atribuições de função:</span><span class="sxs-lookup"><span data-stu-id="db3de-150">The Azure CLI 2.0 provides the following commands to manage role assignments:</span></span>

* [<span data-ttu-id="db3de-151">az role assignment list</span><span class="sxs-lookup"><span data-stu-id="db3de-151">az role assignment list</span></span>](/cli/azure/role/assignment#list)
* [<span data-ttu-id="db3de-152">az role assignment create</span><span class="sxs-lookup"><span data-stu-id="db3de-152">az role assignment create</span></span>](/cli/azure/role/assignment#create)
* [<span data-ttu-id="db3de-153">az role assignment delete</span><span class="sxs-lookup"><span data-stu-id="db3de-153">az role assignment delete</span></span>](/cli/azure/role/assignment#delete)

<span data-ttu-id="db3de-154">A função padrão para uma entidade de serviço é **Colaborador**.</span><span class="sxs-lookup"><span data-stu-id="db3de-154">The default role for a service principal is **Contributor**.</span></span> <span data-ttu-id="db3de-155">Pode não ser a melhor opção para interações do aplicativo com os serviços do Azure, dadas suas permissões amplas.</span><span class="sxs-lookup"><span data-stu-id="db3de-155">It may not be the best choice for an app's interactions with Azure services, given its broad permissions.</span></span> <span data-ttu-id="db3de-156">A função **Leitor** é mais restritiva e é uma boa opção para acesso somente leitura.</span><span class="sxs-lookup"><span data-stu-id="db3de-156">The **Reader** role is more restrictive and is a good choice for read-only access.</span></span> <span data-ttu-id="db3de-157">Você pode exibir detalhes sobre as permissões específicas de função ou criar conectores personalizados por meio do portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="db3de-157">You can view details on role-specific permissions or create custom ones through the Azure portal.</span></span>

<span data-ttu-id="db3de-158">Nesse exemplo, adicionamos a função **Leitor** ao nosso exemplo anterior e excluímos a função **Colaborador**:</span><span class="sxs-lookup"><span data-stu-id="db3de-158">In this example, add the **Reader** role to our prior example, and delete the **Contributor** one:</span></span>

```azurecli-interactive
az role assignment create --assignee a487e0c1-82af-47d9-9a0b-af184eb87646d --role Reader
az role assignment delete --assignee a487e0c1-82af-47d9-9a0b-af184eb87646d --role Contributor
```

<span data-ttu-id="db3de-159">Verifique as alterações listando as funções atribuídas no momento:</span><span class="sxs-lookup"><span data-stu-id="db3de-159">Verify the changes by listing the currently assigned roles:</span></span>

```azurecli-interactive
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
> <span data-ttu-id="db3de-160">Se sua conta não tiver permissões suficientes para atribuir uma função, verá uma mensagem de erro.</span><span class="sxs-lookup"><span data-stu-id="db3de-160">If your account does not have sufficient permissions to assign a role, you see an error message.</span></span>
> <span data-ttu-id="db3de-161">A mensagem informa que sua conta “não tem autorização para executar a ação 'Microsoft.Authorization/roleAssignments/write' no escopo '/subscriptions/{guid}'”.</span><span class="sxs-lookup"><span data-stu-id="db3de-161">The message states your account "does not have authorization to perform action 'Microsoft.Authorization/roleAssignments/write' over scope '/subscriptions/{guid}'."</span></span>
   
## <a name="change-the-credentials-of-a-security-principal"></a><span data-ttu-id="db3de-162">Alterar as credenciais de uma entidade de segurança</span><span class="sxs-lookup"><span data-stu-id="db3de-162">Change the credentials of a security principal</span></span>

<span data-ttu-id="db3de-163">É uma boa prática de segurança examinar as permissões e atualizar as senhas regularmente.</span><span class="sxs-lookup"><span data-stu-id="db3de-163">It's a good security practice to review permissions and update passwords regularly.</span></span> <span data-ttu-id="db3de-164">Talvez você também queira gerenciar e modificar as credenciais de segurança à medida que seu aplicativo muda.</span><span class="sxs-lookup"><span data-stu-id="db3de-164">You may also want to manage and modify the security credentials as your app changes.</span></span>

### <a name="reset-a-service-principal-password"></a><span data-ttu-id="db3de-165">Redefinir uma senha da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="db3de-165">Reset a service principal password</span></span>

<span data-ttu-id="db3de-166">Use `az ad sp reset-credentials` para redefinir a senha atual da entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="db3de-166">Use `az ad sp reset-credentials` to reset the current password for the service principal.</span></span>

```azurecli-interactive
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

<span data-ttu-id="db3de-167">A CLI gera uma senha segura se você deixar a opção `--password` de fora.</span><span class="sxs-lookup"><span data-stu-id="db3de-167">The CLI generates a secure password if you leave out the `--password` option.</span></span>
