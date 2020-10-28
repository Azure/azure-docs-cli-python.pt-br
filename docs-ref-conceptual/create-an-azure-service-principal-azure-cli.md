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
ms.custom: devx-track-azurecli
ms.openlocfilehash: 17f550e2ce1df2e171d51c262d7a5e0428965039
ms.sourcegitcommit: 1187fb75b68426c46e84b3f294c509ee7b7da9be
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/27/2020
ms.locfileid: "92687005"
---
# <a name="create-an-azure-service-principal-with-the-azure-cli"></a><span data-ttu-id="6464a-103">Criar uma entidade de serviço do Azure com a CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="6464a-103">Create an Azure service principal with the Azure CLI</span></span>

<span data-ttu-id="6464a-104">Ferramentas automatizadas que usam os serviços do Azure devem sempre ter permissões restritas.</span><span class="sxs-lookup"><span data-stu-id="6464a-104">Automated tools that use Azure services should always have restricted permissions.</span></span> <span data-ttu-id="6464a-105">Em vez de os aplicativos entrarem como um usuário com privilégio total, o Azure oferece as entidades de serviço.</span><span class="sxs-lookup"><span data-stu-id="6464a-105">Instead of having applications sign in as a fully privileged user, Azure offers service principals.</span></span>

<span data-ttu-id="6464a-106">Uma entidade de serviço do Azure é uma identidade criada para uso com aplicativos, serviços hospedados e ferramentas automatizadas para acessar os recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="6464a-106">An Azure service principal is an identity created for use with applications, hosted services, and automated tools to access Azure resources.</span></span> <span data-ttu-id="6464a-107">Esse acesso é restrito pelas funções atribuídas à entidade de serviço, oferecendo a você o controle sobre quais recursos poderão ser acessados e em qual nível.</span><span class="sxs-lookup"><span data-stu-id="6464a-107">This access is restricted by the roles assigned to the service principal, giving you control over which resources can be accessed and at which level.</span></span> <span data-ttu-id="6464a-108">Por motivos de segurança, é sempre recomendado usar entidades de serviço com ferramentas automatizadas em vez de permitir a entrada com uma identidade de usuário.</span><span class="sxs-lookup"><span data-stu-id="6464a-108">For security reasons, it's always recommended to use service principals with automated tools rather than allowing them to log in with a user identity.</span></span>

<span data-ttu-id="6464a-109">Este artigo mostra as etapas para criar, obter informações e redefinir uma entidade de serviço com a CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="6464a-109">This article shows you the steps for creating, getting information about, and resetting a service principal with the Azure CLI.</span></span>

## <a name="create-a-service-principal"></a><span data-ttu-id="6464a-110">Criar uma entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="6464a-110">Create a service principal</span></span>

<span data-ttu-id="6464a-111">Crie uma entidade de serviço com o comando [az ad sp create-for-rbac](/cli/azure/ad/sp#az-ad-sp-create-for-rbac).</span><span class="sxs-lookup"><span data-stu-id="6464a-111">Create a service principal with the [az ad sp create-for-rbac](/cli/azure/ad/sp#az-ad-sp-create-for-rbac) command.</span></span> <span data-ttu-id="6464a-112">Ao criar uma entidade de serviço, você pode escolher o tipo de autenticação de entrada usada.</span><span class="sxs-lookup"><span data-stu-id="6464a-112">When creating a service principal, you choose the type of sign-in authentication it uses.</span></span>

> [!NOTE]
>
> <span data-ttu-id="6464a-113">Se sua conta não tiver permissão para criar uma entidade de serviço, `az ad sp create-for-rbac` mostrará uma mensagem de erro “Privilégios insuficientes para concluir a operação”.</span><span class="sxs-lookup"><span data-stu-id="6464a-113">If your account doesn't have permission to create a service principal, `az ad sp create-for-rbac` will return an error message containing "Insufficient privileges to complete the operation."</span></span> <span data-ttu-id="6464a-114">Entre em contato com o administrador do Azure Active Directory para criar uma entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="6464a-114">Contact your Azure Active Directory admin to create a service principal.</span></span>

<span data-ttu-id="6464a-115">Há dois tipos de autenticação disponíveis para as entidades de serviço: A autenticação baseada em senha e em certificado.</span><span class="sxs-lookup"><span data-stu-id="6464a-115">There are two types of authentication available for service principals: Password-based authentication, and certificate-based authentication.</span></span>

### <a name="password-based-authentication"></a><span data-ttu-id="6464a-116">Autenticação baseada em senha</span><span class="sxs-lookup"><span data-stu-id="6464a-116">Password-based authentication</span></span>

<span data-ttu-id="6464a-117">Sem parâmetros de autenticação, a autenticação baseada em senha é usada com uma senha aleatória criada para você.</span><span class="sxs-lookup"><span data-stu-id="6464a-117">Without any authentication parameters, password-based authentication is used with a random password created for you.</span></span>

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName
  ```

> [!IMPORTANT]
> <span data-ttu-id="6464a-118">Desde a CLI do Azure 2.0.68, o parâmetro `--password` para criar uma entidade de serviço com uma senha definida pelo usuário __não tem mais suporte__ para evitar o uso acidental de senhas fracas.</span><span class="sxs-lookup"><span data-stu-id="6464a-118">As of Azure CLI 2.0.68, the `--password` parameter to create a service principal with a user-defined password is __no longer supported__ to prevent the accidental use of weak passwords.</span></span>

<span data-ttu-id="6464a-119">A saída para uma entidade de serviço com a autenticação por senha inclui a chave `password`.</span><span class="sxs-lookup"><span data-stu-id="6464a-119">The output for a service principal with password authentication includes the `password` key.</span></span> <span data-ttu-id="6464a-120">__Certifique-se de__ que tenha copiado esse valor já que não será possível recuperá-lo posteriormente.</span><span class="sxs-lookup"><span data-stu-id="6464a-120">__Make sure__ you copy this value - it can't be retrieved.</span></span> <span data-ttu-id="6464a-121">Se você esquecer a senha, [redefina as credenciais da entidade de serviço](#reset-credentials).</span><span class="sxs-lookup"><span data-stu-id="6464a-121">If you forget the password, [reset the service principal credentials](#reset-credentials).</span></span>

<span data-ttu-id="6464a-122">As chaves `appId` e `tenant` aparecem na saída do `az ad sp create-for-rbac` e são usadas na autenticação da entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="6464a-122">The `appId` and `tenant` keys appear in the output of `az ad sp create-for-rbac` and are used in service principal authentication.</span></span>
<span data-ttu-id="6464a-123">Registre seus valores, mas eles podem ser recuperados a qualquer momento com o comando [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).</span><span class="sxs-lookup"><span data-stu-id="6464a-123">Record their values, but they can be retrieved at any point with [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).</span></span>

### <a name="certificate-based-authentication"></a><span data-ttu-id="6464a-124">Autenticação baseada em certificado</span><span class="sxs-lookup"><span data-stu-id="6464a-124">Certificate-based authentication</span></span>

<span data-ttu-id="6464a-125">Para a autenticação baseada em certificado, use o argumento `--cert`.</span><span class="sxs-lookup"><span data-stu-id="6464a-125">For certificate-based authentication, use the `--cert` argument.</span></span> <span data-ttu-id="6464a-126">Esse argumento exige que você mantenha um certificado existente.</span><span class="sxs-lookup"><span data-stu-id="6464a-126">This argument requires that you hold an existing certificate.</span></span> <span data-ttu-id="6464a-127">Certifique-se de que todas as ferramentas que usam essa entidade de serviço tenham acesso à chave privada do certificado.</span><span class="sxs-lookup"><span data-stu-id="6464a-127">Make sure any tool that uses this service principal has access to the certificate's private key.</span></span> <span data-ttu-id="6464a-128">Os certificados devem estar no formato ASCII, como PEM, CER ou DER.</span><span class="sxs-lookup"><span data-stu-id="6464a-128">Certificates should be in an ASCII format such as PEM, CER, or DER.</span></span> <span data-ttu-id="6464a-129">Transmita o certificado como uma cadeia de caracteres ou use o formato `@path` para carregar o certificado de um arquivo.</span><span class="sxs-lookup"><span data-stu-id="6464a-129">Pass the certificate as a string, or use the `@path` format to load the certificate from a file.</span></span>

> [!NOTE]
> <span data-ttu-id="6464a-130">Ao usar um arquivo PEM, o **CERTIFICADO** precisa ser anexado à **CHAVE PRIVADA** dentro do arquivo.</span><span class="sxs-lookup"><span data-stu-id="6464a-130">When using a PEM file, the **CERTIFICATE** must be appended to the **PRIVATE KEY** within the file.</span></span>

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --cert "-----BEGIN CERTIFICATE-----
...
-----END CERTIFICATE-----"
```

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --cert @/path/to/cert.pem
```

<span data-ttu-id="6464a-131">O argumento `--keyvault` pode ser adicionado para usar o certificado no Azure Key Vault.</span><span class="sxs-lookup"><span data-stu-id="6464a-131">The `--keyvault` argument can be added to use a certificate in Azure Key Vault.</span></span> <span data-ttu-id="6464a-132">Nesse caso, o valor `--cert` é o nome do certificado.</span><span class="sxs-lookup"><span data-stu-id="6464a-132">In this case, the `--cert` value is the name of the certificate.</span></span>

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --cert CertName --keyvault VaultName
```

<span data-ttu-id="6464a-133">Para criar um certificado _autoassinado_ para autenticação, use o argumento `--create-cert`:</span><span class="sxs-lookup"><span data-stu-id="6464a-133">To create a _self-signed_ certificate for authentication, use the `--create-cert` argument:</span></span>

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --create-cert
```

<span data-ttu-id="6464a-134">Saída do console:</span><span class="sxs-lookup"><span data-stu-id="6464a-134">Console output:</span></span>

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

<span data-ttu-id="6464a-135">Conteúdo do novo arquivo PEM:</span><span class="sxs-lookup"><span data-stu-id="6464a-135">Contents of the new PEM file:</span></span>
```
-----BEGIN PRIVATE KEY-----
myPrivateKeyValue
-----END PRIVATE KEY-----
-----BEGIN CERTIFICATE-----
myCertificateValue
-----END CERTIFICATE-----
```

> [!NOTE]
> <span data-ttu-id="6464a-136">O comando `az ad sp create-for-rbac --create-cert` cria a entidade de serviço e um arquivo PEM.</span><span class="sxs-lookup"><span data-stu-id="6464a-136">The `az ad sp create-for-rbac --create-cert` command creates the service principal and a PEM file.</span></span> <span data-ttu-id="6464a-137">O arquivo PEM contém uma **CHAVE PRIVADA** e um **CERTIFICADO** formatados corretamente.</span><span class="sxs-lookup"><span data-stu-id="6464a-137">The PEM file contains a correctly formatted **PRIVATE KEY** and **CERTIFICATE** .</span></span>

<span data-ttu-id="6464a-138">O argumento `--keyvault` pode ser adicionado para armazenar o certificado no Azure Key Vault.</span><span class="sxs-lookup"><span data-stu-id="6464a-138">The `--keyvault` argument can be added to store the certificate in Azure Key Vault.</span></span> <span data-ttu-id="6464a-139">Ao usar `--keyvault`, o argumento `--cert` também será __necessário__ .</span><span class="sxs-lookup"><span data-stu-id="6464a-139">When using `--keyvault`, the `--cert` argument is __required__ .</span></span>

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --create-cert --cert CertName --keyvault VaultName
```

<span data-ttu-id="6464a-140">A menos que você armazene o certificado no cofre de chaves, a saída incluirá a chave `fileWithCertAndPrivateKey`.</span><span class="sxs-lookup"><span data-stu-id="6464a-140">Unless you store the certificate in Key Vault, the output includes the `fileWithCertAndPrivateKey` key.</span></span> <span data-ttu-id="6464a-141">O valor dessa chave informa onde o certificado gerado é armazenado.</span><span class="sxs-lookup"><span data-stu-id="6464a-141">This key's value tells you where the generated certificate is stored.</span></span>
<span data-ttu-id="6464a-142">__Certifique-se__ de copiar o certificado para um local seguro ou não será possível entrar com essa entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="6464a-142">__Make sure__ that you copy the certificate to a secure location, or you can't sign in with this service principal.</span></span>

<span data-ttu-id="6464a-143">Para certificados armazenados no Key Vault, recupere a chave privada do certificado com o comando [az keyvault secret show](/cli/azure/keyvault/secret#az-keyvault-secret-show).</span><span class="sxs-lookup"><span data-stu-id="6464a-143">For certificates stored in Key Vault, retrieve the certificate's private key with [az keyvault secret show](/cli/azure/keyvault/secret#az-keyvault-secret-show).</span></span> <span data-ttu-id="6464a-144">No Key Vault, o nome do segredo do certificado é igual ao nome do certificado.</span><span class="sxs-lookup"><span data-stu-id="6464a-144">In Key Vault, the name of the certificate's secret is the same as the certificate name.</span></span> <span data-ttu-id="6464a-145">Se você perder o acesso à chave privada de um certificado, [redefina as credenciais da entidade de serviço](#reset-credentials).</span><span class="sxs-lookup"><span data-stu-id="6464a-145">If you lose access to a certificate's private key, [reset the service principal credentials](#reset-credentials).</span></span>

<span data-ttu-id="6464a-146">As chaves `appId` e `tenant` aparecem na saída do `az ad sp create-for-rbac` e são usadas na autenticação da entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="6464a-146">The `appId` and `tenant` keys appear in the output of `az ad sp create-for-rbac` and are used in service principal authentication.</span></span>
<span data-ttu-id="6464a-147">Registre seus valores, mas eles podem ser recuperados a qualquer momento com o comando [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).</span><span class="sxs-lookup"><span data-stu-id="6464a-147">Record their values, but they can be retrieved at any point with [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).</span></span>

## <a name="get-an-existing-service-principal"></a><span data-ttu-id="6464a-148">Obter uma entidade de serviço existente</span><span class="sxs-lookup"><span data-stu-id="6464a-148">Get an existing service principal</span></span>

<span data-ttu-id="6464a-149">Uma lista das entidades de serviço em um locatário pode ser recuperada com o comando [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).</span><span class="sxs-lookup"><span data-stu-id="6464a-149">A list of the service principals in a tenant can be retrieved with [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).</span></span> <span data-ttu-id="6464a-150">Por padrão, esse comando retorna as 100 primeiras entidades de serviço do locatário.</span><span class="sxs-lookup"><span data-stu-id="6464a-150">By default this command returns the first 100 service principals for your tenant.</span></span> <span data-ttu-id="6464a-151">Para obter todas as entidades de serviço de um locatário, use o argumento `--all`.</span><span class="sxs-lookup"><span data-stu-id="6464a-151">To get all of a tenant's service principals, use the `--all` argument.</span></span> <span data-ttu-id="6464a-152">Obter essa lista pode levar muito tempo, portanto, é recomendável que você filtre a lista com um dos argumentos a seguir:</span><span class="sxs-lookup"><span data-stu-id="6464a-152">Getting this list can take a long time, so it's recommended that you filter the list with one of the following arguments:</span></span>

* <span data-ttu-id="6464a-153">`--display-name` envia solicitações às entidades de serviço que têm um _prefixo_ que corresponda ao nome fornecido.</span><span class="sxs-lookup"><span data-stu-id="6464a-153">`--display-name` requests service principals that have a _prefix_ that match the provided name.</span></span> <span data-ttu-id="6464a-154">O nome de exibição de uma entidade de serviço é o valor definido com o parâmetro `--name` durante a criação.</span><span class="sxs-lookup"><span data-stu-id="6464a-154">The display name of a service principal is the value set with the `--name` parameter during creation.</span></span> <span data-ttu-id="6464a-155">Se você não definiu `--name` durante a criação da entidade de serviço, o prefixo do nome será `azure-cli-`.</span><span class="sxs-lookup"><span data-stu-id="6464a-155">If you didn't set `--name` during service principal creation, the name prefix is `azure-cli-`.</span></span>
* <span data-ttu-id="6464a-156">`--spn` filtra a correspondência do nome exato da entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="6464a-156">`--spn` filters on exact service principal name matching.</span></span> <span data-ttu-id="6464a-157">O nome da entidade de serviço sempre começa com `https://`.</span><span class="sxs-lookup"><span data-stu-id="6464a-157">The service principal name always starts with `https://`.</span></span>
  <span data-ttu-id="6464a-158">se o valor usado para `--name` não era um URI, esse valor é `https://` seguido do nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="6464a-158">if the value you used for `--name` wasn't a URI, this value is `https://` followed by the display name.</span></span>
* <span data-ttu-id="6464a-159">`--show-mine` só envia solicitações às entidades de serviço criadas pelo usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="6464a-159">`--show-mine` requests only service principals created by the signed-in user.</span></span>
* <span data-ttu-id="6464a-160">`--filter` usa um filtro OData e realiza a filtragem _do lado do servidor_ .</span><span class="sxs-lookup"><span data-stu-id="6464a-160">`--filter` takes an OData filter, and performs _server-side_ filtering.</span></span> <span data-ttu-id="6464a-161">Esse método é recomendado para a filtragem do lado do cliente com o argumento `--query` da CLI.</span><span class="sxs-lookup"><span data-stu-id="6464a-161">This method is recommended over filtering client-side with the CLI's `--query` argument.</span></span> <span data-ttu-id="6464a-162">Para saber mais sobre os filtros do OData, confira [Sintaxe de expressão do OData para filtros](/rest/api/searchservice/odata-expression-syntax-for-azure-search).</span><span class="sxs-lookup"><span data-stu-id="6464a-162">To learn about OData filters, see [OData expression syntax for filters](/rest/api/searchservice/odata-expression-syntax-for-azure-search).</span></span>

<span data-ttu-id="6464a-163">As informações retornadas para objetos da entidade de serviço são detalhadas.</span><span class="sxs-lookup"><span data-stu-id="6464a-163">The information returned for service principal objects is verbose.</span></span> <span data-ttu-id="6464a-164">Para obter apenas as informações necessárias para entrar, use a cadeia de consulta `[].{id:appId, tenant:appOwnerTenantId}`.</span><span class="sxs-lookup"><span data-stu-id="6464a-164">To get only the information necessary for sign-in, use the query string `[].{id:appId, tenant:appOwnerTenantId}`.</span></span> <span data-ttu-id="6464a-165">Por exemplo, para obter as informações de logon para todas as entidades de serviço criadas pelo usuário conectado no momento:</span><span class="sxs-lookup"><span data-stu-id="6464a-165">For example, to get the sign-in information for all service principals created by the currently logged in user:</span></span>

```azurecli-interactive
az ad sp list --show-mine --query "[].{id:appId, tenant:appOwnerTenantId}"
```

> [!IMPORTANT]
>
> <span data-ttu-id="6464a-166">`az ad sp list` ou [az ad sp show](/cli/azure/ad/sp#az-ad-sp-show) obtêm o usuário e o locatário, mas não os segredos de autenticação _nem_ o método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="6464a-166">`az ad sp list` or [az ad sp show](/cli/azure/ad/sp#az-ad-sp-show) get the user and tenant, but not any authentication secrets _or_ the authentication method.</span></span>
> <span data-ttu-id="6464a-167">Os segredos para certificados no Key Vault podem ser recuperados com o comando [az keyvault secret show](/cli/azure/keyvault/secret#az-keyvault-secret-show), mas, por padrão, nenhum outro segredo será armazenado.</span><span class="sxs-lookup"><span data-stu-id="6464a-167">Secrets for certificates in Key Vault can be retrieved with [az keyvault secret show](/cli/azure/keyvault/secret#az-keyvault-secret-show), but no other secrets are stored by default.</span></span>
> <span data-ttu-id="6464a-168">Se você esquecer o método de autenticação ou o segredo, [redefina as credenciais da entidade de serviço](#reset-credentials).</span><span class="sxs-lookup"><span data-stu-id="6464a-168">If you forget an authentication method or secret, [reset the service principal credentials](#reset-credentials).</span></span>

## <a name="manage-service-principal-roles"></a><span data-ttu-id="6464a-169">Gerenciar funções da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="6464a-169">Manage service principal roles</span></span>

<span data-ttu-id="6464a-170">A CLI do Azure oferece os seguintes comandos para gerenciar as atribuições de função:</span><span class="sxs-lookup"><span data-stu-id="6464a-170">The Azure CLI has the following commands to manage role assignments:</span></span>

* [<span data-ttu-id="6464a-171">az role assignment list</span><span class="sxs-lookup"><span data-stu-id="6464a-171">az role assignment list</span></span>](/cli/azure/role/assignment#az-role-assignment-list)
* [<span data-ttu-id="6464a-172">az role assignment create</span><span class="sxs-lookup"><span data-stu-id="6464a-172">az role assignment create</span></span>](/cli/azure/role/assignment#az-role-assignment-create)
* [<span data-ttu-id="6464a-173">az role assignment delete</span><span class="sxs-lookup"><span data-stu-id="6464a-173">az role assignment delete</span></span>](/cli/azure/role/assignment#az-role-assignment-delete)

<span data-ttu-id="6464a-174">A função padrão para uma entidade de serviço é **Colaborador** .</span><span class="sxs-lookup"><span data-stu-id="6464a-174">The default role for a service principal is **Contributor** .</span></span> <span data-ttu-id="6464a-175">Essa função tem permissões completas para ler e gravar em uma conta do Azure.</span><span class="sxs-lookup"><span data-stu-id="6464a-175">This role has full permissions to read and write to an Azure account.</span></span> <span data-ttu-id="6464a-176">A função **Leitor** é mais restritiva, com acesso somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6464a-176">The **Reader** role is more restrictive, with read-only access.</span></span>  <span data-ttu-id="6464a-177">Para obter mais informações sobre o Controle de Acesso Baseado em Função (RBAC) e funções, confira [RBAC: funções internas](/azure/active-directory/role-based-access-built-in-roles).</span><span class="sxs-lookup"><span data-stu-id="6464a-177">For more information on Role-Based Access Control (RBAC) and roles, see [RBAC: Built-in roles](/azure/active-directory/role-based-access-built-in-roles).</span></span>

<span data-ttu-id="6464a-178">Esse exemplo adiciona a função **Leitor** e exclui a função **Colaborador** :</span><span class="sxs-lookup"><span data-stu-id="6464a-178">This example adds the **Reader** role and removes the **Contributor** one:</span></span>

```azurecli-interactive
az role assignment create --assignee APP_ID --role Reader
az role assignment delete --assignee APP_ID --role Contributor
```

> [!NOTE]
> <span data-ttu-id="6464a-179">Caso sua conta não tenha permissão para atribuir uma função, você verá uma mensagem de erro informando que sua conta “não tem autorização para executar a ação ‘Microsoft.Authorization/roleAssignments/write’”. Entre em contato com o administrador do Azure Active Directory para gerenciar funções.</span><span class="sxs-lookup"><span data-stu-id="6464a-179">If your account doesn't have permission to assign a role, you see an error message that your account "does not have authorization to perform action 'Microsoft.Authorization/roleAssignments/write'." Contact your Azure Active Directory admin to manage roles.</span></span>

<span data-ttu-id="6464a-180">Adicionar uma função _não_ restringe as permissões atribuídas anteriormente.</span><span class="sxs-lookup"><span data-stu-id="6464a-180">Adding a role _doesn't_ restrict previously assigned permissions.</span></span> <span data-ttu-id="6464a-181">Ao restringir as permissões da entidade de serviço, a função __Colaborador__ deverá ser removida.</span><span class="sxs-lookup"><span data-stu-id="6464a-181">When restricting a service principal's permissions, the __Contributor__ role should be removed.</span></span>

<span data-ttu-id="6464a-182">Para verificar as alterações, liste as funções atribuídas:</span><span class="sxs-lookup"><span data-stu-id="6464a-182">The changes can be verified by listing the assigned roles:</span></span>

```azurecli-interactive
az role assignment list --assignee APP_ID
```

## <a name="sign-in-using-a-service-principal"></a><span data-ttu-id="6464a-183">Entrar usando uma entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="6464a-183">Sign in using a service principal</span></span>

<span data-ttu-id="6464a-184">Teste as novas credenciais e permissões da entidade de serviço iniciando a sessão.</span><span class="sxs-lookup"><span data-stu-id="6464a-184">Test the new service principal's credentials and permissions by signing in.</span></span> <span data-ttu-id="6464a-185">Para entrar com uma entidade de serviço, você precisa de `appId`, `tenant` e das credenciais.</span><span class="sxs-lookup"><span data-stu-id="6464a-185">To sign in with a service principal, you need the `appId`, `tenant`, and credentials.</span></span>

<span data-ttu-id="6464a-186">Para entrar com uma entidade de serviço usando a senha:</span><span class="sxs-lookup"><span data-stu-id="6464a-186">To sign in with a service principal using a password:</span></span>

```azurecli-interactive
az login --service-principal --username APP_ID --password PASSWORD --tenant TENANT_ID
```

<span data-ttu-id="6464a-187">Para entrar com um certificado, ele precisa estar disponível localmente como um arquivo PEM ou DER, no formato ASCII.</span><span class="sxs-lookup"><span data-stu-id="6464a-187">To sign in with a certificate, it must be available locally as a PEM or DER file, in ASCII format.</span></span> <span data-ttu-id="6464a-188">Ao usar um arquivo PEM, a **CHAVE PRIVADA** e o **CERTIFICADO** precisam ser anexados juntos dentro do arquivo.</span><span class="sxs-lookup"><span data-stu-id="6464a-188">When using a PEM file, the **PRIVATE KEY** and **CERTIFICATE** must be appended together within the file.</span></span>

```azurecli-interactive
az login --service-principal --username APP_ID --tenant TENANT_ID --password /path/to/cert
```

<span data-ttu-id="6464a-189">Para saber mais sobre como entrar com uma entidade de serviço, confira [Entrar com a CLI do Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="6464a-189">To learn more about signing in with a service principal, see [Sign in with the Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="create-a-resource-using-service-principal"></a><span data-ttu-id="6464a-190">Criar um recurso usando a entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="6464a-190">Create a resource using service principal</span></span>

<span data-ttu-id="6464a-191">A seção a seguir fornece um exemplo de como criar um recurso do [Armazenamento do Azure](/azure/storage/) com uma entidade de serviço usando os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="6464a-191">The following section provides an example of how to create an resource for [Azure Storage](/azure/storage/) with a service principal, using the following commands:</span></span>

* [<span data-ttu-id="6464a-192">az login</span><span class="sxs-lookup"><span data-stu-id="6464a-192">az login</span></span>](/cli/azure/reference-index?#az_login)
* [<span data-ttu-id="6464a-193">az group create</span><span class="sxs-lookup"><span data-stu-id="6464a-193">az group create</span></span>](/cli/azure/group#az_group_create)
* [<span data-ttu-id="6464a-194">az storage account create</span><span class="sxs-lookup"><span data-stu-id="6464a-194">az storage account create</span></span>](/cli/azure/storage/account#az_storage_account_create)
* [<span data-ttu-id="6464a-195">az storage account keys list</span><span class="sxs-lookup"><span data-stu-id="6464a-195">az storage account keys list</span></span>](/cli/azure/storage/account/keys#az_storage_account_keys_list)

<span data-ttu-id="6464a-196">Para entrar com uma entidade de serviço, você precisa dos valores de `appId`, `tenant` e `password` retornados como resposta quando você [criou a entidade de serviço](#sign-in-using-a-service-principal).</span><span class="sxs-lookup"><span data-stu-id="6464a-196">To sign in with a service principal, you need the `appId`, `tenant`, and `password` returned as the response when you [created your service principal](#sign-in-using-a-service-principal).</span></span>

1. <span data-ttu-id="6464a-197">Faça logon como a entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="6464a-197">Log in as the service principal.</span></span>

    ```azurecli-interactive
    az login --service-principal --username APP_ID --password PASSWORD --tenant TENANT_ID
    ```

1. <span data-ttu-id="6464a-198">Crie um grupo de recursos para manter todos os recursos usados para o mesmo projeto de início rápido, tutorial ou desenvolvimento.</span><span class="sxs-lookup"><span data-stu-id="6464a-198">Create a resource group to hold all resources used for the same quickstart, tutorial, or development project.</span></span>

    ```azurecli-interactive
    az group create --location WESTUS --name MY_RESOURCE_GROUP
    ```

1. <span data-ttu-id="6464a-199">Crie um recurso para um serviço do Azure.</span><span class="sxs-lookup"><span data-stu-id="6464a-199">Create a resource to an Azure service.</span></span> <span data-ttu-id="6464a-200">Substitua `<SERVICENAME>` pelo nome do serviço do Azure.</span><span class="sxs-lookup"><span data-stu-id="6464a-200">Replace `<SERVICENAME>` with the name of the Azure service.</span></span>

    <span data-ttu-id="6464a-201">Para o Armazenamento do Azure, os valores válidos para o parâmetro `<KIND>` são:</span><span class="sxs-lookup"><span data-stu-id="6464a-201">For Azure Storage, valid values for the `<KIND>` parameter are:</span></span>

    * <span data-ttu-id="6464a-202">BlobStorage</span><span class="sxs-lookup"><span data-stu-id="6464a-202">BlobStorage</span></span>
    * <span data-ttu-id="6464a-203">BlockBlobStorage</span><span class="sxs-lookup"><span data-stu-id="6464a-203">BlockBlobStorage</span></span>
    * <span data-ttu-id="6464a-204">FileStorage</span><span class="sxs-lookup"><span data-stu-id="6464a-204">FileStorage</span></span>
    * <span data-ttu-id="6464a-205">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="6464a-205">Storage</span></span>
    * <span data-ttu-id="6464a-206">StorageV2</span><span class="sxs-lookup"><span data-stu-id="6464a-206">StorageV2</span></span>

    ```azurecli-interactive
    az storage account create --name MY_RESOURCE_<SERVICENAME> --resource-group MY_RESOURCE_GROUP --kind <KIND> --sku F0 --location WESTUS --yes
    ```

1. <span data-ttu-id="6464a-207">Obtenha as chaves de recurso para o novo recurso, que você usa em seu código para se autenticar no serviço do Azure.</span><span class="sxs-lookup"><span data-stu-id="6464a-207">Get resource keys for the new resource, which you use in your code to authenticate to the Azure service.</span></span>

    ```azurecli-interactive
    az storage account keys list --name MY_RESOURCE_<SERVICENAME> --resource-group MY_RESOURCE_GROUP
    ```

## <a name="reset-credentials"></a><span data-ttu-id="6464a-208">Redefinir credenciais</span><span class="sxs-lookup"><span data-stu-id="6464a-208">Reset credentials</span></span>

<span data-ttu-id="6464a-209">Se você esquecer as credenciais de uma entidade de serviço, use o comando [az ad sp credencial reset](/cli/azure/ad/sp/credential#az-ad-sp-credential-reset).</span><span class="sxs-lookup"><span data-stu-id="6464a-209">If you forget the credentials for a service principal, use [az ad sp credential reset](/cli/azure/ad/sp/credential#az-ad-sp-credential-reset).</span></span> <span data-ttu-id="6464a-210">O comando reset tem os mesmos argumentos que `az ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="6464a-210">The reset command takes the same arguments as `az ad sp create-for-rbac`.</span></span>

```azurecli-interactive
az ad sp credential reset --name APP_ID
```

## <a name="see-also"></a><span data-ttu-id="6464a-211">Veja também</span><span class="sxs-lookup"><span data-stu-id="6464a-211">See also</span></span>

* [<span data-ttu-id="6464a-212">Aplicativo e objetos de entidade de serviço no Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="6464a-212">Application and service principal objects in Azure Active Directory</span></span>](/azure/active-directory/develop/app-objects-and-service-principals)
* [<span data-ttu-id="6464a-213">Como gerenciar entidades de serviço</span><span class="sxs-lookup"><span data-stu-id="6464a-213">How to manage service principals</span></span>](/azure/developer/python/how-to-manage-service-principals)
