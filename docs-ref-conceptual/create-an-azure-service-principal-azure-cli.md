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
ms.openlocfilehash: 7ead12b35cefd7cba9e06f7905c9267c569d98dd
ms.sourcegitcommit: 014d89aa21f90561eb69792ad01947e481ea640a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/23/2019
ms.locfileid: "56741710"
---
# <a name="create-an-azure-service-principal-with-azure-cli"></a><span data-ttu-id="bafb7-103">Criar uma entidade de serviço do Azure com a CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="bafb7-103">Create an Azure service principal with Azure CLI</span></span>

<span data-ttu-id="bafb7-104">Ferramentas automatizadas que usam os serviços do Azure devem sempre ter permissões restritas.</span><span class="sxs-lookup"><span data-stu-id="bafb7-104">Automated tools that use Azure services should always have restricted permissions.</span></span> <span data-ttu-id="bafb7-105">Em vez de os aplicativos entrarem como um usuário com privilégio total, o Azure oferece as entidades de serviço.</span><span class="sxs-lookup"><span data-stu-id="bafb7-105">Instead of having applications sign in as a fully privileged user, Azure offers service principals.</span></span>

<span data-ttu-id="bafb7-106">Uma entidade de serviço do Azure é uma identidade criada para uso com aplicativos, serviços hospedados e ferramentas automatizadas para acessar os recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="bafb7-106">An Azure service principal is an identity created for use with applications, hosted services, and automated tools to access Azure resources.</span></span> <span data-ttu-id="bafb7-107">Esse acesso é restrito pelas funções atribuídas à entidade de serviço, oferecendo a você o controle sobre quais recursos poderão ser acessados e em qual nível.</span><span class="sxs-lookup"><span data-stu-id="bafb7-107">This access is restricted by the roles assigned to the service principal, giving you control over which resources can be accessed and at which level.</span></span> <span data-ttu-id="bafb7-108">Por motivos de segurança, é sempre recomendado usar entidades de serviço com ferramentas automatizadas em vez de permitir a entrada com uma identidade de usuário.</span><span class="sxs-lookup"><span data-stu-id="bafb7-108">For security reasons, it's always recommended to use service principals with automated tools rather than allowing them to log in with a user identity.</span></span>

<span data-ttu-id="bafb7-109">Este artigo mostra as etapas para criar, obter informações e redefinir uma entidade de serviço com a CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="bafb7-109">This article shows you the steps for creating, getting information about, and resetting a service principal with the Azure CLI.</span></span>

## <a name="create-a-service-principal"></a><span data-ttu-id="bafb7-110">Criar uma entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="bafb7-110">Create a service principal</span></span>

<span data-ttu-id="bafb7-111">Crie uma entidade de serviço com o comando [az ad sp create-for-rbac](/cli/azure/ad/sp#az-ad-sp-create-for-rbac).</span><span class="sxs-lookup"><span data-stu-id="bafb7-111">Create a service principal with the [az ad sp create-for-rbac](/cli/azure/ad/sp#az-ad-sp-create-for-rbac) command.</span></span> <span data-ttu-id="bafb7-112">Ao criar uma entidade de serviço, você pode escolher o tipo de autenticação de entrada usada.</span><span class="sxs-lookup"><span data-stu-id="bafb7-112">When creating a service principal, you choose the type of sign-in authentication it uses.</span></span> 

> [!NOTE]
>
> <span data-ttu-id="bafb7-113">Se sua conta não tiver permissão para criar uma entidade de serviço, `az ad sp create-for-rbac` mostrará uma mensagem de erro “Privilégios insuficientes para concluir a operação”.</span><span class="sxs-lookup"><span data-stu-id="bafb7-113">If your account doesn't have permission to create a service principal, `az ad sp create-for-rbac` will return an error message containing "Insufficient privileges to complete the operation."</span></span> <span data-ttu-id="bafb7-114">Entre em contato com o administrador do Azure Active Directory para criar uma entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="bafb7-114">Contact your Azure Active Directory admin to create a service principal.</span></span>

<span data-ttu-id="bafb7-115">Há dois tipos de autenticação disponíveis para as entidades de serviço: A autenticação baseada em senha e em certificado.</span><span class="sxs-lookup"><span data-stu-id="bafb7-115">There are two types of authentication available for service principals: Password-based authentication, and certificate-based authentication.</span></span>

### <a name="password-based-authentication"></a><span data-ttu-id="bafb7-116">Autenticação baseada em senha</span><span class="sxs-lookup"><span data-stu-id="bafb7-116">Password-based authentication</span></span>

<span data-ttu-id="bafb7-117">Sem parâmetros de autenticação, a autenticação baseada em senha é usada com uma senha aleatória criada para você.</span><span class="sxs-lookup"><span data-stu-id="bafb7-117">Without any authentication parameters, password-based authentication is used with a random password created for you.</span></span> <span data-ttu-id="bafb7-118">Caso queira uma autenticação baseada em senha, esse método é recomendado.</span><span class="sxs-lookup"><span data-stu-id="bafb7-118">If you want password-based authentication, this method is recommended.</span></span>

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName
  ```

<span data-ttu-id="bafb7-119">Para uma senha fornecida pelo usuário, use o argumento `--password`.</span><span class="sxs-lookup"><span data-stu-id="bafb7-119">For a user-supplied password, use the `--password` argument.</span></span> <span data-ttu-id="bafb7-120">Quando criar uma senha, certifique-se de seguir as [Regras e restrições de senha do Azure Active Directory](/azure/active-directory/active-directory-passwords-policy).</span><span class="sxs-lookup"><span data-stu-id="bafb7-120">When creating a password, make sure you follow the [Azure Active Directory password rules and restrictions](/azure/active-directory/active-directory-passwords-policy).</span></span> <span data-ttu-id="bafb7-121">Não use uma senha fraca, nem reutilize uma senha.</span><span class="sxs-lookup"><span data-stu-id="bafb7-121">Don't use a weak password or reuse a password.</span></span>

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --password <Choose a strong password>
  ```

  > [!IMPORTANT]
  >
  > <span data-ttu-id="bafb7-122">Por motivos de segurança, o argumento `--password` para a criação da entidade de serviço será preterido em uma versão futura.</span><span class="sxs-lookup"><span data-stu-id="bafb7-122">For security reasons, the `--password` argument for service principal creation will be deprecated in a future release.</span></span> <span data-ttu-id="bafb7-123">Se você quiser usar a autenticação baseada em senha, evite `--password` e deixe a CLI gerar uma senha segura para você.</span><span class="sxs-lookup"><span data-stu-id="bafb7-123">If you want to use password-based authentication, avoid `--password` and let the CLI generate a secure password for you.</span></span>

<span data-ttu-id="bafb7-124">A saída para uma entidade de serviço com a autenticação por senha inclui a chave `password`.</span><span class="sxs-lookup"><span data-stu-id="bafb7-124">The output for a service principal with password authentication includes the `password` key.</span></span> <span data-ttu-id="bafb7-125">__Certifique-se de__ que tenha copiado esse valor já que não será possível recuperá-lo posteriormente.</span><span class="sxs-lookup"><span data-stu-id="bafb7-125">__Make sure__ you copy this value - it can't be retrieved.</span></span> <span data-ttu-id="bafb7-126">Se você esquecer a senha, [redefina as credenciais da entidade de serviço](#reset-credentials).</span><span class="sxs-lookup"><span data-stu-id="bafb7-126">If you forget the password, [reset the service principal credentials](#reset-credentials).</span></span>

<span data-ttu-id="bafb7-127">As chaves `appId` e `tenant` aparecem na saída do `az ad sp create-for-rbac` e são usadas na autenticação da entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="bafb7-127">The `appId` and `tenant` keys appear in the output of `az ad sp create-for-rbac` and are used in service principal authentication.</span></span>
<span data-ttu-id="bafb7-128">Registre seus valores, mas eles podem ser recuperados a qualquer momento com o comando [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).</span><span class="sxs-lookup"><span data-stu-id="bafb7-128">Record their values, but they can be retrieved at any point with [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).</span></span>

### <a name="certificate-based-authentication"></a><span data-ttu-id="bafb7-129">Autenticação baseada em certificado</span><span class="sxs-lookup"><span data-stu-id="bafb7-129">Certificate-based authentication</span></span>

<span data-ttu-id="bafb7-130">Para a autenticação baseada em certificado, use o argumento `--cert`.</span><span class="sxs-lookup"><span data-stu-id="bafb7-130">For certificate-based authentication, use the `--cert` argument.</span></span> <span data-ttu-id="bafb7-131">Esse argumento exige que você mantenha um certificado existente.</span><span class="sxs-lookup"><span data-stu-id="bafb7-131">This argument requires that you hold an existing certificate.</span></span> <span data-ttu-id="bafb7-132">Certifique-se de que todas as ferramentas que usam essa entidade de serviço tenham acesso à chave privada do certificado.</span><span class="sxs-lookup"><span data-stu-id="bafb7-132">Make sure any tool that uses this service principal has access to the certificate's private key.</span></span> <span data-ttu-id="bafb7-133">Os certificados devem estar no formato ASCII, como PEM, CER ou DER.</span><span class="sxs-lookup"><span data-stu-id="bafb7-133">Certificates should be in an ASCII format such as PEM, CER, or DER.</span></span> <span data-ttu-id="bafb7-134">Transmita o certificado como uma cadeia de caracteres ou use o formato `@path` para carregar o certificado de um arquivo.</span><span class="sxs-lookup"><span data-stu-id="bafb7-134">Pass the certificate as a string, or use the `@path` format to load the certificate from a file.</span></span>

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --cert "-----BEGIN CERTIFICATE-----
...
-----END CERTIFICATE-----"
```

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --cert @/path/to/cert.pem
```

<span data-ttu-id="bafb7-135">O argumento `--keyvault` pode ser adicionado para usar o certificado no Azure Key Vault.</span><span class="sxs-lookup"><span data-stu-id="bafb7-135">The `--keyvault` argument can be added to use a certificate in Azure Key Vault.</span></span> <span data-ttu-id="bafb7-136">Nesse caso, o valor `--cert` é o nome do certificado.</span><span class="sxs-lookup"><span data-stu-id="bafb7-136">In this case, the `--cert` value is the name of the certificate.</span></span>

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --cert CertName --keyvault VaultName
```

<span data-ttu-id="bafb7-137">Para criar um certificado _autoassinado_ para autenticação, use o argumento `--create-cert`:</span><span class="sxs-lookup"><span data-stu-id="bafb7-137">To create a _self-signed_ certificate for authentication, use the `--create-cert` argument:</span></span>

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --create-cert
```

<span data-ttu-id="bafb7-138">O argumento `--keyvault` pode ser adicionado para armazenar o certificado no Azure Key Vault.</span><span class="sxs-lookup"><span data-stu-id="bafb7-138">The `--keyvault` argument can be added to store the certificate in Azure Key Vault.</span></span> <span data-ttu-id="bafb7-139">Ao usar `--keyvault`, o argumento `--cert` também será __necessário__.</span><span class="sxs-lookup"><span data-stu-id="bafb7-139">When using `--keyvault`, the `--cert` argument is __required__.</span></span>

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --create-cert --cert CertName --keyvault VaultName
```

<span data-ttu-id="bafb7-140">A menos que você armazene o certificado no cofre de chaves, a saída incluirá a chave `fileWithCertAndPrivateKey`.</span><span class="sxs-lookup"><span data-stu-id="bafb7-140">Unless you store the certificate in Key Vault, the output includes the `fileWithCertAndPrivateKey` key.</span></span> <span data-ttu-id="bafb7-141">O valor dessa chave informa onde o certificado gerado é armazenado.</span><span class="sxs-lookup"><span data-stu-id="bafb7-141">This key's value tells you where the generated certificate is stored.</span></span>
<span data-ttu-id="bafb7-142">__Certifique-se__ de copiar o certificado para um local seguro ou não será possível entrar com essa entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="bafb7-142">__Make sure__ that you copy the certificate to a secure location, or you can't sign in with this service principal.</span></span>

<span data-ttu-id="bafb7-143">Para certificados armazenados no Key Vault, recupere a chave privada do certificado com o comando [az keyvault secret show](/cli/azure/keyvault/secret#az-keyvault-secret-show).</span><span class="sxs-lookup"><span data-stu-id="bafb7-143">For certificates stored in Key Vault, retrieve the certificate's private key with [az keyvault secret show](/cli/azure/keyvault/secret#az-keyvault-secret-show).</span></span> <span data-ttu-id="bafb7-144">No Key Vault, o nome do segredo do certificado é igual ao nome do certificado.</span><span class="sxs-lookup"><span data-stu-id="bafb7-144">In Key Vault, the name of the certificate's secret is the same as the certificate name.</span></span> <span data-ttu-id="bafb7-145">Se você perder o acesso à chave privada de um certificado, [redefina as credenciais da entidade de serviço](#reset-credentials).</span><span class="sxs-lookup"><span data-stu-id="bafb7-145">If you lose access to a certificate's private key, [reset the service principal credentials](#reset-credentials).</span></span>

<span data-ttu-id="bafb7-146">As chaves `appId` e `tenant` aparecem na saída do `az ad sp create-for-rbac` e são usadas na autenticação da entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="bafb7-146">The `appId` and `tenant` keys appear in the output of `az ad sp create-for-rbac` and are used in service principal authentication.</span></span>
<span data-ttu-id="bafb7-147">Registre seus valores, mas eles podem ser recuperados a qualquer momento com o comando [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).</span><span class="sxs-lookup"><span data-stu-id="bafb7-147">Record their values, but they can be retrieved at any point with [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).</span></span>

## <a name="get-an-existing-service-principal"></a><span data-ttu-id="bafb7-148">Obter uma entidade de serviço existente</span><span class="sxs-lookup"><span data-stu-id="bafb7-148">Get an existing service principal</span></span>

<span data-ttu-id="bafb7-149">Uma lista das entidades de serviço em um locatário pode ser recuperada com o comando [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).</span><span class="sxs-lookup"><span data-stu-id="bafb7-149">A list of the service principals in a tenant can be retrieved with [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).</span></span> <span data-ttu-id="bafb7-150">Por padrão, esse comando retorna as 100 primeiras entidades de serviço do locatário.</span><span class="sxs-lookup"><span data-stu-id="bafb7-150">By default this command returns the first 100 service principals for your tenant.</span></span> <span data-ttu-id="bafb7-151">Para obter todas as entidades de serviço de um locatário, use o argumento `--all`.</span><span class="sxs-lookup"><span data-stu-id="bafb7-151">To get all of a tenant's service principals, use the `--all` argument.</span></span> <span data-ttu-id="bafb7-152">Obter essa lista pode levar muito tempo, portanto, é recomendável que você filtre a lista com um dos argumentos a seguir:</span><span class="sxs-lookup"><span data-stu-id="bafb7-152">Getting this list can take a long time, so it's recommended that you filter the list with one of the following arguments:</span></span>

* <span data-ttu-id="bafb7-153">`--display-name` envia solicitações às entidades de serviço que têm um _prefixo_ que corresponda ao nome fornecido.</span><span class="sxs-lookup"><span data-stu-id="bafb7-153">`--display-name` requests service principals that have a _prefix_ that match the provided name.</span></span> <span data-ttu-id="bafb7-154">O nome de exibição de uma entidade de serviço é o valor definido com o parâmetro `--name` durante a criação.</span><span class="sxs-lookup"><span data-stu-id="bafb7-154">The display name of a service principal is the value set with the `--name` parameter during creation.</span></span> <span data-ttu-id="bafb7-155">Se você não definiu `--name` durante a criação da entidade de serviço, o prefixo do nome será `azure-cli-`.</span><span class="sxs-lookup"><span data-stu-id="bafb7-155">If you didn't set `--name` during service principal creation, the name prefix is `azure-cli-`.</span></span>
* <span data-ttu-id="bafb7-156">`--spn` filtra a correspondência do nome exato da entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="bafb7-156">`--spn` filters on exact service principal name matching.</span></span> <span data-ttu-id="bafb7-157">O nome da entidade de serviço sempre começa com `https://`.</span><span class="sxs-lookup"><span data-stu-id="bafb7-157">The service principal name always starts with `https://`.</span></span>
  <span data-ttu-id="bafb7-158">se o valor usado para `--name` não era um URI, esse valor é `https://` seguido do nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="bafb7-158">if the value you used for `--name` wasn't a URI, this value is `https://` followed by the display name.</span></span>
* <span data-ttu-id="bafb7-159">`--show-mine` só envia solicitações às entidades de serviço criadas pelo usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="bafb7-159">`--show-mine` requests only service principals created by the signed-in user.</span></span>
* <span data-ttu-id="bafb7-160">`--filter` usa um filtro OData e realiza a filtragem _do lado do servidor_.</span><span class="sxs-lookup"><span data-stu-id="bafb7-160">`--filter` takes an OData filter, and performs _server-side_ filtering.</span></span> <span data-ttu-id="bafb7-161">Esse método é recomendado para a filtragem do lado do cliente com o argumento `--query` da CLI.</span><span class="sxs-lookup"><span data-stu-id="bafb7-161">This method is recommended over filtering client-side with the CLI's `--query` argument.</span></span> <span data-ttu-id="bafb7-162">Para saber mais sobre os filtros do OData, confira [Sintaxe de expressão do OData para filtros](/rest/api/searchservice/odata-expression-syntax-for-azure-search).</span><span class="sxs-lookup"><span data-stu-id="bafb7-162">To learn about OData filters, see [OData expression syntax for filters](/rest/api/searchservice/odata-expression-syntax-for-azure-search).</span></span>

<span data-ttu-id="bafb7-163">As informações retornadas para objetos da entidade de serviço são detalhadas.</span><span class="sxs-lookup"><span data-stu-id="bafb7-163">The information returned for service principal objects is verbose.</span></span> <span data-ttu-id="bafb7-164">Para obter apenas as informações necessárias para entrar, use a cadeia de consulta `[].{"id":"appId", "tenant":"appOwnerTenantId"}`.</span><span class="sxs-lookup"><span data-stu-id="bafb7-164">To get only the information necessary for sign-in, use the query string `[].{"id":"appId", "tenant":"appOwnerTenantId"}`.</span></span> <span data-ttu-id="bafb7-165">Por exemplo, para obter as informações de logon para todas as entidades de serviço criadas pelo usuário conectado no momento:</span><span class="sxs-lookup"><span data-stu-id="bafb7-165">For example, to get the sign-in information for all service principals created by the currently logged in user:</span></span>

```azurecli-interactive
az ad sp list --show-mine --query '[].{"id":"appId", "tenant":"appOwnerTenantId"}'
```

> [!IMPORTANT]
>
> <span data-ttu-id="bafb7-166">`az ad sp list` ou [az ad sp show](/cli/azure/ad/sp#az-ad-sp-show) obtêm o usuário e o locatário, mas não os segredos de autenticação _nem_ o método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="bafb7-166">`az ad sp list` or [az ad sp show](/cli/azure/ad/sp#az-ad-sp-show) get the user and tenant, but not any authentication secrets _or_ the authentication method.</span></span>
> <span data-ttu-id="bafb7-167">Os segredos para certificados no Key Vault podem ser recuperados com o comando [az keyvault secret show](/cli/azure/keyvault/secret#az-keyvault-secret-show), mas, por padrão, nenhum outro segredo será armazenado.</span><span class="sxs-lookup"><span data-stu-id="bafb7-167">Secrets for certificates in Key Vault can be retrieved with [az keyvault secret show](/cli/azure/keyvault/secret#az-keyvault-secret-show), but no other secrets are stored by default.</span></span>
> <span data-ttu-id="bafb7-168">Se você esquecer o método de autenticação ou o segredo, [redefina as credenciais da entidade de serviço](#reset-credentials).</span><span class="sxs-lookup"><span data-stu-id="bafb7-168">If you forget an authentication method or secret, [reset the service principal credentials](#reset-credentials).</span></span>

## <a name="manage-service-principal-roles"></a><span data-ttu-id="bafb7-169">Gerenciar funções da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="bafb7-169">Manage service principal roles</span></span>

<span data-ttu-id="bafb7-170">A CLI do Azure oferece os seguintes comandos para gerenciar as atribuições de função:</span><span class="sxs-lookup"><span data-stu-id="bafb7-170">The Azure CLI has the following commands to manage role assignments:</span></span>

* [<span data-ttu-id="bafb7-171">az role assignment list</span><span class="sxs-lookup"><span data-stu-id="bafb7-171">az role assignment list</span></span>](/cli/azure/role/assignment#az-role-assignment-list)
* [<span data-ttu-id="bafb7-172">az role assignment create</span><span class="sxs-lookup"><span data-stu-id="bafb7-172">az role assignment create</span></span>](/cli/azure/role/assignment#az-role-assignment-create)
* [<span data-ttu-id="bafb7-173">az role assignment delete</span><span class="sxs-lookup"><span data-stu-id="bafb7-173">az role assignment delete</span></span>](/cli/azure/role/assignment#az-role-assignment-delete)

<span data-ttu-id="bafb7-174">A função padrão para uma entidade de serviço é **Colaborador**.</span><span class="sxs-lookup"><span data-stu-id="bafb7-174">The default role for a service principal is **Contributor**.</span></span> <span data-ttu-id="bafb7-175">Essa função tem permissões completas para ler e gravar em uma conta do Azure.</span><span class="sxs-lookup"><span data-stu-id="bafb7-175">This role has full permissions to read and write to an Azure account.</span></span> <span data-ttu-id="bafb7-176">A função **Leitor** é mais restritiva, com acesso somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bafb7-176">The **Reader** role is more restrictive, with read-only access.</span></span>  <span data-ttu-id="bafb7-177">Para obter mais informações sobre o Controle de Acesso Baseado em Função (RBAC) e funções, confira [RBAC: funções internas](/azure/active-directory/role-based-access-built-in-roles).</span><span class="sxs-lookup"><span data-stu-id="bafb7-177">For more information on Role-Based Access Control (RBAC) and roles, see [RBAC: Built-in roles](/azure/active-directory/role-based-access-built-in-roles).</span></span>

<span data-ttu-id="bafb7-178">Esse exemplo adiciona a função **Leitor** e exclui a função **Colaborador**:</span><span class="sxs-lookup"><span data-stu-id="bafb7-178">This example adds the **Reader** role and removes the **Contributor** one:</span></span>

```azurecli-interactive
az role assignment create --assignee APP_ID --role Reader
az role assignment delete --assignee APP_ID --role Contributor
```

> [!NOTE]
> <span data-ttu-id="bafb7-179">Caso sua conta não tenha permissão para atribuir uma função, você verá uma mensagem de erro informando que sua conta “não tem autorização para executar a ação ‘Microsoft.Authorization/roleAssignments/write’”. Entre em contato com o administrador do Azure Active Directory para gerenciar funções.</span><span class="sxs-lookup"><span data-stu-id="bafb7-179">If your account doesn't have permission to assign a role, you see an error message that your account "does not have authorization to perform action 'Microsoft.Authorization/roleAssignments/write'." Contact your Azure Active Directory admin to manage roles.</span></span>

<span data-ttu-id="bafb7-180">Adicionar uma função _não_ restringe as permissões atribuídas anteriormente.</span><span class="sxs-lookup"><span data-stu-id="bafb7-180">Adding a role _doesn't_ restrict previously assigned permissions.</span></span> <span data-ttu-id="bafb7-181">Ao restringir as permissões da entidade de serviço, a função __Colaborador__ deverá ser removida.</span><span class="sxs-lookup"><span data-stu-id="bafb7-181">When restricting a service principal's permissions, the __Contributor__ role should be removed.</span></span>

<span data-ttu-id="bafb7-182">Para verificar as alterações, liste as funções atribuídas:</span><span class="sxs-lookup"><span data-stu-id="bafb7-182">The changes can be verified by listing the assigned roles:</span></span>

```azurecli-interactive
az role assignment list --assignee APP_ID
```

## <a name="sign-in-using-a-service-principal"></a><span data-ttu-id="bafb7-183">Entrar usando uma entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="bafb7-183">Sign in using a service principal</span></span>

<span data-ttu-id="bafb7-184">Teste as novas credenciais e permissões da entidade de serviço iniciando a sessão.</span><span class="sxs-lookup"><span data-stu-id="bafb7-184">Test the new service principal's credentials and permissions by signing in.</span></span> <span data-ttu-id="bafb7-185">Para entrar com uma entidade de serviço, você precisa de `appId`, `tenant` e das credenciais.</span><span class="sxs-lookup"><span data-stu-id="bafb7-185">To sign in with a service prinicpal, you need the `appId`, `tenant`, and credentials.</span></span>

<span data-ttu-id="bafb7-186">Para entrar com uma entidade de serviço usando a senha:</span><span class="sxs-lookup"><span data-stu-id="bafb7-186">To sign in with a service principal using a password:</span></span>

```azurecli-interactive
az login --service-principal --username APP_ID --password PASSWORD --tenant TENANT_ID
```

<span data-ttu-id="bafb7-187">Para entrar com um certificado, ele deve estar disponível localmente como um arquivo PEM ou DER, no formato ASCII:</span><span class="sxs-lookup"><span data-stu-id="bafb7-187">To sign in with a certificate, it must be available locally as a PEM or DER file, in ASCII format:</span></span>

```azurecli-interactive
az login --service-principal --username APP_ID --tenant TENANT_ID --password /path/to/cert
```

<span data-ttu-id="bafb7-188">Para saber mais sobre como entrar com uma entidade de serviço, confira [Entrar com a CLI do Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="bafb7-188">To learn more about signing in with a service principal, see [Sign in with the Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="reset-credentials"></a><span data-ttu-id="bafb7-189">Redefinir credenciais</span><span class="sxs-lookup"><span data-stu-id="bafb7-189">Reset credentials</span></span>

<span data-ttu-id="bafb7-190">Se você esquecer as credenciais de uma entidade de serviço, use o comando [az ad sp credencial reset](/cli/azure/ad/sp/credential#az-ad-sp-credential-reset).</span><span class="sxs-lookup"><span data-stu-id="bafb7-190">If you forget the credentials for a service principal, use [az ad sp credential reset](/cli/azure/ad/sp/credential#az-ad-sp-credential-reset).</span></span> <span data-ttu-id="bafb7-191">O comando reset tem os mesmos argumentos que `az ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="bafb7-191">The reset command takes the same arguments as `az ad sp create-for-rbac`.</span></span>

```azurecli-interactive
az ad sp credential reset --name APP_ID
```
