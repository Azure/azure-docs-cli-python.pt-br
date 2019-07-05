---
title: Usar entidades de serviço do Azure com a CLI do Azure
description: Saiba como criar e usar entidades de serviço com a CLI do Azure.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 02/15/2019
ms.topic: conceptual
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 6d88400b8d7070cf2f9dba2f3e124edfe2e3163d
ms.sourcegitcommit: e06d34682710e77840b0c51f4718184101bd8a03
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "67527332"
---
# <a name="create-an-azure-service-principal-with-azure-cli"></a><span data-ttu-id="d99cd-103">Criar uma entidade de serviço do Azure com a CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="d99cd-103">Create an Azure service principal with Azure CLI</span></span>

<span data-ttu-id="d99cd-104">Ferramentas automatizadas que usam os serviços do Azure devem sempre ter permissões restritas.</span><span class="sxs-lookup"><span data-stu-id="d99cd-104">Automated tools that use Azure services should always have restricted permissions.</span></span> <span data-ttu-id="d99cd-105">Em vez de os aplicativos entrarem como um usuário com privilégio total, o Azure oferece as entidades de serviço.</span><span class="sxs-lookup"><span data-stu-id="d99cd-105">Instead of having applications sign in as a fully privileged user, Azure offers service principals.</span></span>

<span data-ttu-id="d99cd-106">Uma entidade de serviço do Azure é uma identidade criada para uso com aplicativos, serviços hospedados e ferramentas automatizadas para acessar os recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="d99cd-106">An Azure service principal is an identity created for use with applications, hosted services, and automated tools to access Azure resources.</span></span> <span data-ttu-id="d99cd-107">Esse acesso é restrito pelas funções atribuídas à entidade de serviço, oferecendo a você o controle sobre quais recursos poderão ser acessados e em qual nível.</span><span class="sxs-lookup"><span data-stu-id="d99cd-107">This access is restricted by the roles assigned to the service principal, giving you control over which resources can be accessed and at which level.</span></span> <span data-ttu-id="d99cd-108">Por motivos de segurança, é sempre recomendado usar entidades de serviço com ferramentas automatizadas em vez de permitir a entrada com uma identidade de usuário.</span><span class="sxs-lookup"><span data-stu-id="d99cd-108">For security reasons, it's always recommended to use service principals with automated tools rather than allowing them to log in with a user identity.</span></span>

<span data-ttu-id="d99cd-109">Este artigo mostra as etapas para criar, obter informações e redefinir uma entidade de serviço com a CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="d99cd-109">This article shows you the steps for creating, getting information about, and resetting a service principal with the Azure CLI.</span></span>

## <a name="create-a-service-principal"></a><span data-ttu-id="d99cd-110">Criar uma entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="d99cd-110">Create a service principal</span></span>

<span data-ttu-id="d99cd-111">Crie uma entidade de serviço com o comando [az ad sp create-for-rbac](/cli/azure/ad/sp#az-ad-sp-create-for-rbac).</span><span class="sxs-lookup"><span data-stu-id="d99cd-111">Create a service principal with the [az ad sp create-for-rbac](/cli/azure/ad/sp#az-ad-sp-create-for-rbac) command.</span></span> <span data-ttu-id="d99cd-112">Ao criar uma entidade de serviço, você pode escolher o tipo de autenticação de entrada usada.</span><span class="sxs-lookup"><span data-stu-id="d99cd-112">When creating a service principal, you choose the type of sign-in authentication it uses.</span></span> 

> [!NOTE]
>
> <span data-ttu-id="d99cd-113">Se sua conta não tiver permissão para criar uma entidade de serviço, `az ad sp create-for-rbac` mostrará uma mensagem de erro “Privilégios insuficientes para concluir a operação”.</span><span class="sxs-lookup"><span data-stu-id="d99cd-113">If your account doesn't have permission to create a service principal, `az ad sp create-for-rbac` will return an error message containing "Insufficient privileges to complete the operation."</span></span> <span data-ttu-id="d99cd-114">Entre em contato com o administrador do Azure Active Directory para criar uma entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="d99cd-114">Contact your Azure Active Directory admin to create a service principal.</span></span>

<span data-ttu-id="d99cd-115">Há dois tipos de autenticação disponíveis para as entidades de serviço: A autenticação baseada em senha e em certificado.</span><span class="sxs-lookup"><span data-stu-id="d99cd-115">There are two types of authentication available for service principals: Password-based authentication, and certificate-based authentication.</span></span>

### <a name="password-based-authentication"></a><span data-ttu-id="d99cd-116">Autenticação baseada em senha</span><span class="sxs-lookup"><span data-stu-id="d99cd-116">Password-based authentication</span></span>

<span data-ttu-id="d99cd-117">Sem parâmetros de autenticação, a autenticação baseada em senha é usada com uma senha aleatória criada para você.</span><span class="sxs-lookup"><span data-stu-id="d99cd-117">Without any authentication parameters, password-based authentication is used with a random password created for you.</span></span>

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName
  ```

> [!IMPORTANT]
> <span data-ttu-id="d99cd-118">Desde a CLI do Azure 2.0.68, o parâmetro `--password` para criar uma entidade de serviço com uma senha definida pelo usuário __não tem mais suporte__ para evitar o uso acidental de senhas fracas.</span><span class="sxs-lookup"><span data-stu-id="d99cd-118">As of Azure CLI 2.0.68, the `--password` parameter to create a service principal with a user-defined password is __no longer supported__ to prevent the accidental use of weak passwords.</span></span>

<span data-ttu-id="d99cd-119">A saída para uma entidade de serviço com a autenticação por senha inclui a chave `password`.</span><span class="sxs-lookup"><span data-stu-id="d99cd-119">The output for a service principal with password authentication includes the `password` key.</span></span> <span data-ttu-id="d99cd-120">__Certifique-se de__ que tenha copiado esse valor já que não será possível recuperá-lo posteriormente.</span><span class="sxs-lookup"><span data-stu-id="d99cd-120">__Make sure__ you copy this value - it can't be retrieved.</span></span> <span data-ttu-id="d99cd-121">Se você esquecer a senha, [redefina as credenciais da entidade de serviço](#reset-credentials).</span><span class="sxs-lookup"><span data-stu-id="d99cd-121">If you forget the password, [reset the service principal credentials](#reset-credentials).</span></span>

<span data-ttu-id="d99cd-122">As chaves `appId` e `tenant` aparecem na saída do `az ad sp create-for-rbac` e são usadas na autenticação da entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="d99cd-122">The `appId` and `tenant` keys appear in the output of `az ad sp create-for-rbac` and are used in service principal authentication.</span></span>
<span data-ttu-id="d99cd-123">Registre seus valores, mas eles podem ser recuperados a qualquer momento com o comando [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).</span><span class="sxs-lookup"><span data-stu-id="d99cd-123">Record their values, but they can be retrieved at any point with [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).</span></span>

### <a name="certificate-based-authentication"></a><span data-ttu-id="d99cd-124">Autenticação baseada em certificado</span><span class="sxs-lookup"><span data-stu-id="d99cd-124">Certificate-based authentication</span></span>

<span data-ttu-id="d99cd-125">Para a autenticação baseada em certificado, use o argumento `--cert`.</span><span class="sxs-lookup"><span data-stu-id="d99cd-125">For certificate-based authentication, use the `--cert` argument.</span></span> <span data-ttu-id="d99cd-126">Esse argumento exige que você mantenha um certificado existente.</span><span class="sxs-lookup"><span data-stu-id="d99cd-126">This argument requires that you hold an existing certificate.</span></span> <span data-ttu-id="d99cd-127">Certifique-se de que todas as ferramentas que usam essa entidade de serviço tenham acesso à chave privada do certificado.</span><span class="sxs-lookup"><span data-stu-id="d99cd-127">Make sure any tool that uses this service principal has access to the certificate's private key.</span></span> <span data-ttu-id="d99cd-128">Os certificados devem estar no formato ASCII, como PEM, CER ou DER.</span><span class="sxs-lookup"><span data-stu-id="d99cd-128">Certificates should be in an ASCII format such as PEM, CER, or DER.</span></span> <span data-ttu-id="d99cd-129">Transmita o certificado como uma cadeia de caracteres ou use o formato `@path` para carregar o certificado de um arquivo.</span><span class="sxs-lookup"><span data-stu-id="d99cd-129">Pass the certificate as a string, or use the `@path` format to load the certificate from a file.</span></span>

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --cert "-----BEGIN CERTIFICATE-----
...
-----END CERTIFICATE-----"
```

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --cert @/path/to/cert.pem
```

<span data-ttu-id="d99cd-130">O argumento `--keyvault` pode ser adicionado para usar o certificado no Azure Key Vault.</span><span class="sxs-lookup"><span data-stu-id="d99cd-130">The `--keyvault` argument can be added to use a certificate in Azure Key Vault.</span></span> <span data-ttu-id="d99cd-131">Nesse caso, o valor `--cert` é o nome do certificado.</span><span class="sxs-lookup"><span data-stu-id="d99cd-131">In this case, the `--cert` value is the name of the certificate.</span></span>

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --cert CertName --keyvault VaultName
```

<span data-ttu-id="d99cd-132">Para criar um certificado _autoassinado_ para autenticação, use o argumento `--create-cert`:</span><span class="sxs-lookup"><span data-stu-id="d99cd-132">To create a _self-signed_ certificate for authentication, use the `--create-cert` argument:</span></span>

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --create-cert
```

<span data-ttu-id="d99cd-133">O argumento `--keyvault` pode ser adicionado para armazenar o certificado no Azure Key Vault.</span><span class="sxs-lookup"><span data-stu-id="d99cd-133">The `--keyvault` argument can be added to store the certificate in Azure Key Vault.</span></span> <span data-ttu-id="d99cd-134">Ao usar `--keyvault`, o argumento `--cert` também será __necessário__.</span><span class="sxs-lookup"><span data-stu-id="d99cd-134">When using `--keyvault`, the `--cert` argument is __required__.</span></span>

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --create-cert --cert CertName --keyvault VaultName
```

<span data-ttu-id="d99cd-135">A menos que você armazene o certificado no cofre de chaves, a saída incluirá a chave `fileWithCertAndPrivateKey`.</span><span class="sxs-lookup"><span data-stu-id="d99cd-135">Unless you store the certificate in Key Vault, the output includes the `fileWithCertAndPrivateKey` key.</span></span> <span data-ttu-id="d99cd-136">O valor dessa chave informa onde o certificado gerado é armazenado.</span><span class="sxs-lookup"><span data-stu-id="d99cd-136">This key's value tells you where the generated certificate is stored.</span></span>
<span data-ttu-id="d99cd-137">__Certifique-se__ de copiar o certificado para um local seguro ou não será possível entrar com essa entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="d99cd-137">__Make sure__ that you copy the certificate to a secure location, or you can't sign in with this service principal.</span></span>

<span data-ttu-id="d99cd-138">Para certificados armazenados no Key Vault, recupere a chave privada do certificado com o comando [az keyvault secret show](/cli/azure/keyvault/secret#az-keyvault-secret-show).</span><span class="sxs-lookup"><span data-stu-id="d99cd-138">For certificates stored in Key Vault, retrieve the certificate's private key with [az keyvault secret show](/cli/azure/keyvault/secret#az-keyvault-secret-show).</span></span> <span data-ttu-id="d99cd-139">No Key Vault, o nome do segredo do certificado é igual ao nome do certificado.</span><span class="sxs-lookup"><span data-stu-id="d99cd-139">In Key Vault, the name of the certificate's secret is the same as the certificate name.</span></span> <span data-ttu-id="d99cd-140">Se você perder o acesso à chave privada de um certificado, [redefina as credenciais da entidade de serviço](#reset-credentials).</span><span class="sxs-lookup"><span data-stu-id="d99cd-140">If you lose access to a certificate's private key, [reset the service principal credentials](#reset-credentials).</span></span>

<span data-ttu-id="d99cd-141">As chaves `appId` e `tenant` aparecem na saída do `az ad sp create-for-rbac` e são usadas na autenticação da entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="d99cd-141">The `appId` and `tenant` keys appear in the output of `az ad sp create-for-rbac` and are used in service principal authentication.</span></span>
<span data-ttu-id="d99cd-142">Registre seus valores, mas eles podem ser recuperados a qualquer momento com o comando [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).</span><span class="sxs-lookup"><span data-stu-id="d99cd-142">Record their values, but they can be retrieved at any point with [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).</span></span>

## <a name="get-an-existing-service-principal"></a><span data-ttu-id="d99cd-143">Obter uma entidade de serviço existente</span><span class="sxs-lookup"><span data-stu-id="d99cd-143">Get an existing service principal</span></span>

<span data-ttu-id="d99cd-144">Uma lista das entidades de serviço em um locatário pode ser recuperada com o comando [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).</span><span class="sxs-lookup"><span data-stu-id="d99cd-144">A list of the service principals in a tenant can be retrieved with [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).</span></span> <span data-ttu-id="d99cd-145">Por padrão, esse comando retorna as 100 primeiras entidades de serviço do locatário.</span><span class="sxs-lookup"><span data-stu-id="d99cd-145">By default this command returns the first 100 service principals for your tenant.</span></span> <span data-ttu-id="d99cd-146">Para obter todas as entidades de serviço de um locatário, use o argumento `--all`.</span><span class="sxs-lookup"><span data-stu-id="d99cd-146">To get all of a tenant's service principals, use the `--all` argument.</span></span> <span data-ttu-id="d99cd-147">Obter essa lista pode levar muito tempo, portanto, é recomendável que você filtre a lista com um dos argumentos a seguir:</span><span class="sxs-lookup"><span data-stu-id="d99cd-147">Getting this list can take a long time, so it's recommended that you filter the list with one of the following arguments:</span></span>

* <span data-ttu-id="d99cd-148">`--display-name` envia solicitações às entidades de serviço que têm um _prefixo_ que corresponda ao nome fornecido.</span><span class="sxs-lookup"><span data-stu-id="d99cd-148">`--display-name` requests service principals that have a _prefix_ that match the provided name.</span></span> <span data-ttu-id="d99cd-149">O nome de exibição de uma entidade de serviço é o valor definido com o parâmetro `--name` durante a criação.</span><span class="sxs-lookup"><span data-stu-id="d99cd-149">The display name of a service principal is the value set with the `--name` parameter during creation.</span></span> <span data-ttu-id="d99cd-150">Se você não definiu `--name` durante a criação da entidade de serviço, o prefixo do nome será `azure-cli-`.</span><span class="sxs-lookup"><span data-stu-id="d99cd-150">If you didn't set `--name` during service principal creation, the name prefix is `azure-cli-`.</span></span>
* <span data-ttu-id="d99cd-151">`--spn` filtra a correspondência do nome exato da entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="d99cd-151">`--spn` filters on exact service principal name matching.</span></span> <span data-ttu-id="d99cd-152">O nome da entidade de serviço sempre começa com `https://`.</span><span class="sxs-lookup"><span data-stu-id="d99cd-152">The service principal name always starts with `https://`.</span></span>
  <span data-ttu-id="d99cd-153">se o valor usado para `--name` não era um URI, esse valor é `https://` seguido do nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="d99cd-153">if the value you used for `--name` wasn't a URI, this value is `https://` followed by the display name.</span></span>
* <span data-ttu-id="d99cd-154">`--show-mine` só envia solicitações às entidades de serviço criadas pelo usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="d99cd-154">`--show-mine` requests only service principals created by the signed-in user.</span></span>
* <span data-ttu-id="d99cd-155">`--filter` usa um filtro OData e realiza a filtragem _do lado do servidor_.</span><span class="sxs-lookup"><span data-stu-id="d99cd-155">`--filter` takes an OData filter, and performs _server-side_ filtering.</span></span> <span data-ttu-id="d99cd-156">Esse método é recomendado para a filtragem do lado do cliente com o argumento `--query` da CLI.</span><span class="sxs-lookup"><span data-stu-id="d99cd-156">This method is recommended over filtering client-side with the CLI's `--query` argument.</span></span> <span data-ttu-id="d99cd-157">Para saber mais sobre os filtros do OData, confira [Sintaxe de expressão do OData para filtros](/rest/api/searchservice/odata-expression-syntax-for-azure-search).</span><span class="sxs-lookup"><span data-stu-id="d99cd-157">To learn about OData filters, see [OData expression syntax for filters](/rest/api/searchservice/odata-expression-syntax-for-azure-search).</span></span>

<span data-ttu-id="d99cd-158">As informações retornadas para objetos da entidade de serviço são detalhadas.</span><span class="sxs-lookup"><span data-stu-id="d99cd-158">The information returned for service principal objects is verbose.</span></span> <span data-ttu-id="d99cd-159">Para obter apenas as informações necessárias para entrar, use a cadeia de consulta `[].{"id":"appId", "tenant":"appOwnerTenantId"}`.</span><span class="sxs-lookup"><span data-stu-id="d99cd-159">To get only the information necessary for sign-in, use the query string `[].{"id":"appId", "tenant":"appOwnerTenantId"}`.</span></span> <span data-ttu-id="d99cd-160">Por exemplo, para obter as informações de logon para todas as entidades de serviço criadas pelo usuário conectado no momento:</span><span class="sxs-lookup"><span data-stu-id="d99cd-160">For example, to get the sign-in information for all service principals created by the currently logged in user:</span></span>

```azurecli-interactive
az ad sp list --show-mine --query '[].{"id":"appId", "tenant":"appOwnerTenantId"}'
```

> [!IMPORTANT]
>
> <span data-ttu-id="d99cd-161">`az ad sp list` ou [az ad sp show](/cli/azure/ad/sp#az-ad-sp-show) obtêm o usuário e o locatário, mas não os segredos de autenticação _nem_ o método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="d99cd-161">`az ad sp list` or [az ad sp show](/cli/azure/ad/sp#az-ad-sp-show) get the user and tenant, but not any authentication secrets _or_ the authentication method.</span></span>
> <span data-ttu-id="d99cd-162">Os segredos para certificados no Key Vault podem ser recuperados com o comando [az keyvault secret show](/cli/azure/keyvault/secret#az-keyvault-secret-show), mas, por padrão, nenhum outro segredo será armazenado.</span><span class="sxs-lookup"><span data-stu-id="d99cd-162">Secrets for certificates in Key Vault can be retrieved with [az keyvault secret show](/cli/azure/keyvault/secret#az-keyvault-secret-show), but no other secrets are stored by default.</span></span>
> <span data-ttu-id="d99cd-163">Se você esquecer o método de autenticação ou o segredo, [redefina as credenciais da entidade de serviço](#reset-credentials).</span><span class="sxs-lookup"><span data-stu-id="d99cd-163">If you forget an authentication method or secret, [reset the service principal credentials](#reset-credentials).</span></span>

## <a name="manage-service-principal-roles"></a><span data-ttu-id="d99cd-164">Gerenciar funções da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="d99cd-164">Manage service principal roles</span></span>

<span data-ttu-id="d99cd-165">A CLI do Azure oferece os seguintes comandos para gerenciar as atribuições de função:</span><span class="sxs-lookup"><span data-stu-id="d99cd-165">The Azure CLI has the following commands to manage role assignments:</span></span>

* [<span data-ttu-id="d99cd-166">az role assignment list</span><span class="sxs-lookup"><span data-stu-id="d99cd-166">az role assignment list</span></span>](/cli/azure/role/assignment#az-role-assignment-list)
* [<span data-ttu-id="d99cd-167">az role assignment create</span><span class="sxs-lookup"><span data-stu-id="d99cd-167">az role assignment create</span></span>](/cli/azure/role/assignment#az-role-assignment-create)
* [<span data-ttu-id="d99cd-168">az role assignment delete</span><span class="sxs-lookup"><span data-stu-id="d99cd-168">az role assignment delete</span></span>](/cli/azure/role/assignment#az-role-assignment-delete)

<span data-ttu-id="d99cd-169">A função padrão para uma entidade de serviço é **Colaborador**.</span><span class="sxs-lookup"><span data-stu-id="d99cd-169">The default role for a service principal is **Contributor**.</span></span> <span data-ttu-id="d99cd-170">Essa função tem permissões completas para ler e gravar em uma conta do Azure.</span><span class="sxs-lookup"><span data-stu-id="d99cd-170">This role has full permissions to read and write to an Azure account.</span></span> <span data-ttu-id="d99cd-171">A função **Leitor** é mais restritiva, com acesso somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d99cd-171">The **Reader** role is more restrictive, with read-only access.</span></span>  <span data-ttu-id="d99cd-172">Para obter mais informações sobre o Controle de Acesso Baseado em Função (RBAC) e funções, confira [RBAC: funções internas](/azure/active-directory/role-based-access-built-in-roles).</span><span class="sxs-lookup"><span data-stu-id="d99cd-172">For more information on Role-Based Access Control (RBAC) and roles, see [RBAC: Built-in roles](/azure/active-directory/role-based-access-built-in-roles).</span></span>

<span data-ttu-id="d99cd-173">Esse exemplo adiciona a função **Leitor** e exclui a função **Colaborador**:</span><span class="sxs-lookup"><span data-stu-id="d99cd-173">This example adds the **Reader** role and removes the **Contributor** one:</span></span>

```azurecli-interactive
az role assignment create --assignee APP_ID --role Reader
az role assignment delete --assignee APP_ID --role Contributor
```

> [!NOTE]
> <span data-ttu-id="d99cd-174">Caso sua conta não tenha permissão para atribuir uma função, você verá uma mensagem de erro informando que sua conta “não tem autorização para executar a ação ‘Microsoft.Authorization/roleAssignments/write’”. Entre em contato com o administrador do Azure Active Directory para gerenciar funções.</span><span class="sxs-lookup"><span data-stu-id="d99cd-174">If your account doesn't have permission to assign a role, you see an error message that your account "does not have authorization to perform action 'Microsoft.Authorization/roleAssignments/write'." Contact your Azure Active Directory admin to manage roles.</span></span>

<span data-ttu-id="d99cd-175">Adicionar uma função _não_ restringe as permissões atribuídas anteriormente.</span><span class="sxs-lookup"><span data-stu-id="d99cd-175">Adding a role _doesn't_ restrict previously assigned permissions.</span></span> <span data-ttu-id="d99cd-176">Ao restringir as permissões da entidade de serviço, a função __Colaborador__ deverá ser removida.</span><span class="sxs-lookup"><span data-stu-id="d99cd-176">When restricting a service principal's permissions, the __Contributor__ role should be removed.</span></span>

<span data-ttu-id="d99cd-177">Para verificar as alterações, liste as funções atribuídas:</span><span class="sxs-lookup"><span data-stu-id="d99cd-177">The changes can be verified by listing the assigned roles:</span></span>

```azurecli-interactive
az role assignment list --assignee APP_ID
```

## <a name="sign-in-using-a-service-principal"></a><span data-ttu-id="d99cd-178">Entrar usando uma entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="d99cd-178">Sign in using a service principal</span></span>

<span data-ttu-id="d99cd-179">Teste as novas credenciais e permissões da entidade de serviço iniciando a sessão.</span><span class="sxs-lookup"><span data-stu-id="d99cd-179">Test the new service principal's credentials and permissions by signing in.</span></span> <span data-ttu-id="d99cd-180">Para entrar com uma entidade de serviço, você precisa de `appId`, `tenant` e das credenciais.</span><span class="sxs-lookup"><span data-stu-id="d99cd-180">To sign in with a service prinicpal, you need the `appId`, `tenant`, and credentials.</span></span>

<span data-ttu-id="d99cd-181">Para entrar com uma entidade de serviço usando a senha:</span><span class="sxs-lookup"><span data-stu-id="d99cd-181">To sign in with a service principal using a password:</span></span>

```azurecli-interactive
az login --service-principal --username APP_ID --password PASSWORD --tenant TENANT_ID
```

<span data-ttu-id="d99cd-182">Para entrar com um certificado, ele deve estar disponível localmente como um arquivo PEM ou DER, no formato ASCII:</span><span class="sxs-lookup"><span data-stu-id="d99cd-182">To sign in with a certificate, it must be available locally as a PEM or DER file, in ASCII format:</span></span>

```azurecli-interactive
az login --service-principal --username APP_ID --tenant TENANT_ID --password /path/to/cert
```

<span data-ttu-id="d99cd-183">Para saber mais sobre como entrar com uma entidade de serviço, confira [Entrar com a CLI do Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="d99cd-183">To learn more about signing in with a service principal, see [Sign in with the Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="reset-credentials"></a><span data-ttu-id="d99cd-184">Redefinir credenciais</span><span class="sxs-lookup"><span data-stu-id="d99cd-184">Reset credentials</span></span>

<span data-ttu-id="d99cd-185">Se você esquecer as credenciais de uma entidade de serviço, use o comando [az ad sp credencial reset](/cli/azure/ad/sp/credential#az-ad-sp-credential-reset).</span><span class="sxs-lookup"><span data-stu-id="d99cd-185">If you forget the credentials for a service principal, use [az ad sp credential reset](/cli/azure/ad/sp/credential#az-ad-sp-credential-reset).</span></span> <span data-ttu-id="d99cd-186">O comando reset tem os mesmos argumentos que `az ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="d99cd-186">The reset command takes the same arguments as `az ad sp create-for-rbac`.</span></span>

```azurecli-interactive
az ad sp credential reset --name APP_ID
```
