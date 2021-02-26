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
ms.openlocfilehash: 6b64a8f781907977d6123561d91fb8266a0ebe08
ms.sourcegitcommit: 594e9c620a6f74f5eaedf91a7f6a791e03a64c74
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2021
ms.locfileid: "100631060"
---
# <a name="create-an-azure-service-principal-with-the-azure-cli"></a><span data-ttu-id="0e944-103">Criar uma entidade de serviço do Azure com a CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="0e944-103">Create an Azure service principal with the Azure CLI</span></span>

<span data-ttu-id="0e944-104">Ferramentas automatizadas que usam os serviços do Azure devem sempre ter permissões restritas.</span><span class="sxs-lookup"><span data-stu-id="0e944-104">Automated tools that use Azure services should always have restricted permissions.</span></span> <span data-ttu-id="0e944-105">Em vez de os aplicativos entrarem como um usuário com privilégio total, o Azure oferece as entidades de serviço.</span><span class="sxs-lookup"><span data-stu-id="0e944-105">Instead of having applications sign in as a fully privileged user, Azure offers service principals.</span></span>

<span data-ttu-id="0e944-106">Uma entidade de serviço do Azure é uma identidade criada para uso com aplicativos, serviços hospedados e ferramentas automatizadas para acessar os recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="0e944-106">An Azure service principal is an identity created for use with applications, hosted services, and automated tools to access Azure resources.</span></span> <span data-ttu-id="0e944-107">Esse acesso é restrito pelas funções atribuídas à entidade de serviço, oferecendo a você o controle sobre quais recursos poderão ser acessados e em qual nível.</span><span class="sxs-lookup"><span data-stu-id="0e944-107">This access is restricted by the roles assigned to the service principal, giving you control over which resources can be accessed and at which level.</span></span> <span data-ttu-id="0e944-108">Por motivos de segurança, é sempre recomendado usar entidades de serviço com ferramentas automatizadas em vez de permitir a entrada com uma identidade de usuário.</span><span class="sxs-lookup"><span data-stu-id="0e944-108">For security reasons, it's always recommended to use service principals with automated tools rather than allowing them to log in with a user identity.</span></span>

<span data-ttu-id="0e944-109">Este artigo mostra as etapas para criar, obter informações e redefinir uma entidade de serviço com a CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="0e944-109">This article shows you the steps for creating, getting information about, and resetting a service principal with the Azure CLI.</span></span>

## <a name="create-a-service-principal"></a><span data-ttu-id="0e944-110">Criar uma entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="0e944-110">Create a service principal</span></span>

<span data-ttu-id="0e944-111">Crie uma entidade de serviço com o comando [az ad sp create-for-rbac](/cli/azure/ad/sp#az-ad-sp-create-for-rbac).</span><span class="sxs-lookup"><span data-stu-id="0e944-111">Create a service principal with the [az ad sp create-for-rbac](/cli/azure/ad/sp#az-ad-sp-create-for-rbac) command.</span></span> <span data-ttu-id="0e944-112">Ao criar uma entidade de serviço, você pode escolher o tipo de autenticação de entrada usada.</span><span class="sxs-lookup"><span data-stu-id="0e944-112">When creating a service principal, you choose the type of sign-in authentication it uses.</span></span>

<span data-ttu-id="0e944-113">Há dois tipos de autenticação disponíveis para as entidades de serviço: A autenticação baseada em senha e em certificado.</span><span class="sxs-lookup"><span data-stu-id="0e944-113">There are two types of authentication available for service principals: Password-based authentication, and certificate-based authentication.</span></span>

> [!NOTE]
>
> <span data-ttu-id="0e944-114">Se sua conta não tiver permissão para criar uma entidade de serviço, `az ad sp create-for-rbac` mostrará uma mensagem de erro “Privilégios insuficientes para concluir a operação”.</span><span class="sxs-lookup"><span data-stu-id="0e944-114">If your account doesn't have permission to create a service principal, `az ad sp create-for-rbac` will return an error message containing "Insufficient privileges to complete the operation."</span></span> <span data-ttu-id="0e944-115">Entre em contato com o administrador do Azure Active Directory para criar uma entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="0e944-115">Contact your Azure Active Directory admin to create a service principal.</span></span>

> [!WARNING]
> <span data-ttu-id="0e944-116">Quando você cria uma entidade de serviço usando o comando `az ad sp create-for-rbac`, a saída inclui as credenciais que você precisa proteger.</span><span class="sxs-lookup"><span data-stu-id="0e944-116">When you create a service principal using the `az ad sp create-for-rbac` command, the output includes credentials that you must protect.</span></span> <span data-ttu-id="0e944-117">Lembre-se de não incluir essas credenciais em seu código ou de verificar as credenciais em seu controle do código-fonte.</span><span class="sxs-lookup"><span data-stu-id="0e944-117">Be sure that you do not include these credentials in your code or check the credentials into your source control.</span></span> <span data-ttu-id="0e944-118">Como alternativa, considere usar as [identidades gerenciadas](/azure/active-directory/managed-identities-azure-resources/overview), se estiverem disponíveis, para evitar a necessidade de usar credenciais.</span><span class="sxs-lookup"><span data-stu-id="0e944-118">As an alternative, consider using [managed identities](/azure/active-directory/managed-identities-azure-resources/overview) if available to avoid the need to use credentials.</span></span>
>
> <span data-ttu-id="0e944-119">Por padrão, `az ad sp create-for-rbac` atribui a função [Colaborador](/azure/role-based-access-control/built-in-roles#contributor) à entidade de serviço no escopo da assinatura.</span><span class="sxs-lookup"><span data-stu-id="0e944-119">By default, `az ad sp create-for-rbac` assigns the [Contributor](/azure/role-based-access-control/built-in-roles#contributor) role to the service principal at the subscription scope.</span></span> <span data-ttu-id="0e944-120">Para reduzir o risco de uma entidade de serviço comprometida, atribua uma função mais específica e restrinja o escopo a um recurso ou grupo de recursos.</span><span class="sxs-lookup"><span data-stu-id="0e944-120">To reduce your risk of a compromised service principal, assign a more specific role and narrow the scope to a resource or resource group.</span></span> <span data-ttu-id="0e944-121">Confira [Etapas para adicionar uma atribuição de função](/azure/role-based-access-control/role-assignments-steps) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="0e944-121">See [Steps to add a role assignment](/azure/role-based-access-control/role-assignments-steps) for more information.</span></span>
>
> <span data-ttu-id="0e944-122">Em uma versão futura, `az ad sp create-for-rbac` NÃO criará uma atribuição de função de **Colaborador** por padrão.</span><span class="sxs-lookup"><span data-stu-id="0e944-122">In a future release, `az ad sp create-for-rbac` will NOT create a **Contributor** role assignment by default.</span></span> <span data-ttu-id="0e944-123">Se necessário, use o argumento `--role` para criar explicitamente uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="0e944-123">If needed, use the `--role` argument to explicitly create a role assignment.</span></span>

### <a name="password-based-authentication"></a><span data-ttu-id="0e944-124">Autenticação baseada em senha</span><span class="sxs-lookup"><span data-stu-id="0e944-124">Password-based authentication</span></span>

<span data-ttu-id="0e944-125">Sem parâmetros de autenticação, a autenticação baseada em senha é usada com uma senha aleatória criada para você.</span><span class="sxs-lookup"><span data-stu-id="0e944-125">Without any authentication parameters, password-based authentication is used with a random password created for you.</span></span>

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName
  ```

> [!IMPORTANT]
> <span data-ttu-id="0e944-126">Desde a CLI do Azure 2.0.68, o parâmetro `--password` para criar uma entidade de serviço com uma senha definida pelo usuário __não tem mais suporte__ para evitar o uso acidental de senhas fracas.</span><span class="sxs-lookup"><span data-stu-id="0e944-126">As of Azure CLI 2.0.68, the `--password` parameter to create a service principal with a user-defined password is __no longer supported__ to prevent the accidental use of weak passwords.</span></span>

<span data-ttu-id="0e944-127">A saída para uma entidade de serviço com a autenticação por senha inclui a chave `password`.</span><span class="sxs-lookup"><span data-stu-id="0e944-127">The output for a service principal with password authentication includes the `password` key.</span></span> <span data-ttu-id="0e944-128">__Certifique-se de__ que tenha copiado esse valor já que não será possível recuperá-lo posteriormente.</span><span class="sxs-lookup"><span data-stu-id="0e944-128">__Make sure__ you copy this value - it can't be retrieved.</span></span> <span data-ttu-id="0e944-129">Se você esquecer a senha, [redefina as credenciais da entidade de serviço](#reset-credentials).</span><span class="sxs-lookup"><span data-stu-id="0e944-129">If you forget the password, [reset the service principal credentials](#reset-credentials).</span></span>

<span data-ttu-id="0e944-130">As chaves `appId` e `tenant` aparecem na saída do `az ad sp create-for-rbac` e são usadas na autenticação da entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="0e944-130">The `appId` and `tenant` keys appear in the output of `az ad sp create-for-rbac` and are used in service principal authentication.</span></span>
<span data-ttu-id="0e944-131">Registre seus valores, mas eles podem ser recuperados a qualquer momento com o comando [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).</span><span class="sxs-lookup"><span data-stu-id="0e944-131">Record their values, but they can be retrieved at any point with [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).</span></span>

### <a name="certificate-based-authentication"></a><span data-ttu-id="0e944-132">Autenticação baseada em certificado</span><span class="sxs-lookup"><span data-stu-id="0e944-132">Certificate-based authentication</span></span>

<span data-ttu-id="0e944-133">Para a autenticação baseada em certificado, use o argumento `--cert`.</span><span class="sxs-lookup"><span data-stu-id="0e944-133">For certificate-based authentication, use the `--cert` argument.</span></span> <span data-ttu-id="0e944-134">Esse argumento exige que você mantenha um certificado existente.</span><span class="sxs-lookup"><span data-stu-id="0e944-134">This argument requires that you hold an existing certificate.</span></span> <span data-ttu-id="0e944-135">Certifique-se de que todas as ferramentas que usam essa entidade de serviço tenham acesso à chave privada do certificado.</span><span class="sxs-lookup"><span data-stu-id="0e944-135">Make sure any tool that uses this service principal has access to the certificate's private key.</span></span> <span data-ttu-id="0e944-136">Os certificados devem estar no formato ASCII, como PEM, CER ou DER.</span><span class="sxs-lookup"><span data-stu-id="0e944-136">Certificates should be in an ASCII format such as PEM, CER, or DER.</span></span> <span data-ttu-id="0e944-137">Transmita o certificado como uma cadeia de caracteres ou use o formato `@path` para carregar o certificado de um arquivo.</span><span class="sxs-lookup"><span data-stu-id="0e944-137">Pass the certificate as a string, or use the `@path` format to load the certificate from a file.</span></span>

> [!NOTE]
> <span data-ttu-id="0e944-138">Ao usar um arquivo PEM, o **CERTIFICADO** precisa ser anexado à **CHAVE PRIVADA** dentro do arquivo.</span><span class="sxs-lookup"><span data-stu-id="0e944-138">When using a PEM file, the **CERTIFICATE** must be appended to the **PRIVATE KEY** within the file.</span></span>

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --cert "-----BEGIN CERTIFICATE-----
...
-----END CERTIFICATE-----"
```

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --cert @/path/to/cert.pem
```

<span data-ttu-id="0e944-139">O argumento `--keyvault` pode ser adicionado para usar o certificado no Azure Key Vault.</span><span class="sxs-lookup"><span data-stu-id="0e944-139">The `--keyvault` argument can be added to use a certificate in Azure Key Vault.</span></span> <span data-ttu-id="0e944-140">Nesse caso, o valor `--cert` é o nome do certificado.</span><span class="sxs-lookup"><span data-stu-id="0e944-140">In this case, the `--cert` value is the name of the certificate.</span></span>

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --cert CertName --keyvault VaultName
```

<span data-ttu-id="0e944-141">Para criar um certificado _autoassinado_ para autenticação, use o argumento `--create-cert`:</span><span class="sxs-lookup"><span data-stu-id="0e944-141">To create a _self-signed_ certificate for authentication, use the `--create-cert` argument:</span></span>

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --create-cert
```

<span data-ttu-id="0e944-142">Saída do console:</span><span class="sxs-lookup"><span data-stu-id="0e944-142">Console output:</span></span>

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

<span data-ttu-id="0e944-143">Conteúdo do novo arquivo PEM:</span><span class="sxs-lookup"><span data-stu-id="0e944-143">Contents of the new PEM file:</span></span>
```
-----BEGIN PRIVATE KEY-----
myPrivateKeyValue
-----END PRIVATE KEY-----
-----BEGIN CERTIFICATE-----
myCertificateValue
-----END CERTIFICATE-----
```

> [!NOTE]
> <span data-ttu-id="0e944-144">O comando `az ad sp create-for-rbac --create-cert` cria a entidade de serviço e um arquivo PEM.</span><span class="sxs-lookup"><span data-stu-id="0e944-144">The `az ad sp create-for-rbac --create-cert` command creates the service principal and a PEM file.</span></span> <span data-ttu-id="0e944-145">O arquivo PEM contém uma **CHAVE PRIVADA** e um **CERTIFICADO** formatados corretamente.</span><span class="sxs-lookup"><span data-stu-id="0e944-145">The PEM file contains a correctly formatted **PRIVATE KEY** and **CERTIFICATE**.</span></span>

<span data-ttu-id="0e944-146">O argumento `--keyvault` pode ser adicionado para armazenar o certificado no Azure Key Vault.</span><span class="sxs-lookup"><span data-stu-id="0e944-146">The `--keyvault` argument can be added to store the certificate in Azure Key Vault.</span></span> <span data-ttu-id="0e944-147">Ao usar `--keyvault`, o argumento `--cert` também será __necessário__.</span><span class="sxs-lookup"><span data-stu-id="0e944-147">When using `--keyvault`, the `--cert` argument is __required__.</span></span>

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --create-cert --cert CertName --keyvault VaultName
```

<span data-ttu-id="0e944-148">A menos que você armazene o certificado no cofre de chaves, a saída incluirá a chave `fileWithCertAndPrivateKey`.</span><span class="sxs-lookup"><span data-stu-id="0e944-148">Unless you store the certificate in Key Vault, the output includes the `fileWithCertAndPrivateKey` key.</span></span> <span data-ttu-id="0e944-149">O valor dessa chave informa onde o certificado gerado é armazenado.</span><span class="sxs-lookup"><span data-stu-id="0e944-149">This key's value tells you where the generated certificate is stored.</span></span>
<span data-ttu-id="0e944-150">__Certifique-se__ de copiar o certificado para um local seguro ou não será possível entrar com essa entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="0e944-150">__Make sure__ that you copy the certificate to a secure location, or you can't sign in with this service principal.</span></span>

<span data-ttu-id="0e944-151">Para certificados armazenados no Key Vault, recupere a chave privada do certificado com o comando [az keyvault secret show](/cli/azure/keyvault/secret#az-keyvault-secret-show).</span><span class="sxs-lookup"><span data-stu-id="0e944-151">For certificates stored in Key Vault, retrieve the certificate's private key with [az keyvault secret show](/cli/azure/keyvault/secret#az-keyvault-secret-show).</span></span> <span data-ttu-id="0e944-152">No Key Vault, o nome do segredo do certificado é igual ao nome do certificado.</span><span class="sxs-lookup"><span data-stu-id="0e944-152">In Key Vault, the name of the certificate's secret is the same as the certificate name.</span></span> <span data-ttu-id="0e944-153">Se você perder o acesso à chave privada de um certificado, [redefina as credenciais da entidade de serviço](#reset-credentials).</span><span class="sxs-lookup"><span data-stu-id="0e944-153">If you lose access to a certificate's private key, [reset the service principal credentials](#reset-credentials).</span></span>

<span data-ttu-id="0e944-154">As chaves `appId` e `tenant` aparecem na saída do `az ad sp create-for-rbac` e são usadas na autenticação da entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="0e944-154">The `appId` and `tenant` keys appear in the output of `az ad sp create-for-rbac` and are used in service principal authentication.</span></span>
<span data-ttu-id="0e944-155">Registre seus valores, mas eles podem ser recuperados a qualquer momento com o comando [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).</span><span class="sxs-lookup"><span data-stu-id="0e944-155">Record their values, but they can be retrieved at any point with [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).</span></span>

## <a name="get-an-existing-service-principal"></a><span data-ttu-id="0e944-156">Obter uma entidade de serviço existente</span><span class="sxs-lookup"><span data-stu-id="0e944-156">Get an existing service principal</span></span>

<span data-ttu-id="0e944-157">Uma lista das entidades de serviço em um locatário pode ser recuperada com o comando [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).</span><span class="sxs-lookup"><span data-stu-id="0e944-157">A list of the service principals in a tenant can be retrieved with [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).</span></span> <span data-ttu-id="0e944-158">Por padrão, esse comando retorna as 100 primeiras entidades de serviço do locatário.</span><span class="sxs-lookup"><span data-stu-id="0e944-158">By default this command returns the first 100 service principals for your tenant.</span></span> <span data-ttu-id="0e944-159">Para obter todas as entidades de serviço de um locatário, use o argumento `--all`.</span><span class="sxs-lookup"><span data-stu-id="0e944-159">To get all of a tenant's service principals, use the `--all` argument.</span></span> <span data-ttu-id="0e944-160">Obter essa lista pode levar muito tempo, portanto, é recomendável que você filtre a lista com um dos argumentos a seguir:</span><span class="sxs-lookup"><span data-stu-id="0e944-160">Getting this list can take a long time, so it's recommended that you filter the list with one of the following arguments:</span></span>

* <span data-ttu-id="0e944-161">`--display-name` envia solicitações às entidades de serviço que têm um _prefixo_ que corresponda ao nome fornecido.</span><span class="sxs-lookup"><span data-stu-id="0e944-161">`--display-name` requests service principals that have a _prefix_ that match the provided name.</span></span> <span data-ttu-id="0e944-162">O nome de exibição de uma entidade de serviço é o valor definido com o parâmetro `--name` durante a criação.</span><span class="sxs-lookup"><span data-stu-id="0e944-162">The display name of a service principal is the value set with the `--name` parameter during creation.</span></span> <span data-ttu-id="0e944-163">Se você não definiu `--name` durante a criação da entidade de serviço, o prefixo do nome será `azure-cli-`.</span><span class="sxs-lookup"><span data-stu-id="0e944-163">If you didn't set `--name` during service principal creation, the name prefix is `azure-cli-`.</span></span>
* <span data-ttu-id="0e944-164">`--spn` filtra a correspondência do nome exato da entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="0e944-164">`--spn` filters on exact service principal name matching.</span></span> <span data-ttu-id="0e944-165">O nome da entidade de serviço sempre começa com `https://`.</span><span class="sxs-lookup"><span data-stu-id="0e944-165">The service principal name always starts with `https://`.</span></span>
  <span data-ttu-id="0e944-166">se o valor usado para `--name` não era um URI, esse valor é `https://` seguido do nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="0e944-166">if the value you used for `--name` wasn't a URI, this value is `https://` followed by the display name.</span></span>
* <span data-ttu-id="0e944-167">`--show-mine` só envia solicitações às entidades de serviço criadas pelo usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="0e944-167">`--show-mine` requests only service principals created by the signed-in user.</span></span>
* <span data-ttu-id="0e944-168">`--filter` usa um filtro OData e realiza a filtragem _do lado do servidor_.</span><span class="sxs-lookup"><span data-stu-id="0e944-168">`--filter` takes an OData filter, and performs _server-side_ filtering.</span></span> <span data-ttu-id="0e944-169">Esse método é recomendado para a filtragem do lado do cliente com o argumento `--query` da CLI.</span><span class="sxs-lookup"><span data-stu-id="0e944-169">This method is recommended over filtering client-side with the CLI's `--query` argument.</span></span> <span data-ttu-id="0e944-170">Para saber mais sobre os filtros do OData, confira [Sintaxe de expressão do OData para filtros](/rest/api/searchservice/odata-expression-syntax-for-azure-search).</span><span class="sxs-lookup"><span data-stu-id="0e944-170">To learn about OData filters, see [OData expression syntax for filters](/rest/api/searchservice/odata-expression-syntax-for-azure-search).</span></span>

<span data-ttu-id="0e944-171">As informações retornadas para objetos da entidade de serviço são detalhadas.</span><span class="sxs-lookup"><span data-stu-id="0e944-171">The information returned for service principal objects is verbose.</span></span> <span data-ttu-id="0e944-172">Para obter apenas as informações necessárias para entrar, use a cadeia de consulta `[].{id:appId, tenant:appOwnerTenantId}`.</span><span class="sxs-lookup"><span data-stu-id="0e944-172">To get only the information necessary for sign-in, use the query string `[].{id:appId, tenant:appOwnerTenantId}`.</span></span> <span data-ttu-id="0e944-173">Por exemplo, para obter as informações de logon para todas as entidades de serviço criadas pelo usuário conectado no momento:</span><span class="sxs-lookup"><span data-stu-id="0e944-173">For example, to get the sign-in information for all service principals created by the currently logged in user:</span></span>

```azurecli-interactive
az ad sp list --show-mine --query "[].{id:appId, tenant:appOwnerTenantId}"
```

> [!IMPORTANT]
>
> <span data-ttu-id="0e944-174">`az ad sp list` ou [az ad sp show](/cli/azure/ad/sp#az-ad-sp-show) obtêm o usuário e o locatário, mas não os segredos de autenticação _nem_ o método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="0e944-174">`az ad sp list` or [az ad sp show](/cli/azure/ad/sp#az-ad-sp-show) get the user and tenant, but not any authentication secrets _or_ the authentication method.</span></span>
> <span data-ttu-id="0e944-175">Os segredos para certificados no Key Vault podem ser recuperados com o comando [az keyvault secret show](/cli/azure/keyvault/secret#az-keyvault-secret-show), mas, por padrão, nenhum outro segredo será armazenado.</span><span class="sxs-lookup"><span data-stu-id="0e944-175">Secrets for certificates in Key Vault can be retrieved with [az keyvault secret show](/cli/azure/keyvault/secret#az-keyvault-secret-show), but no other secrets are stored by default.</span></span>
> <span data-ttu-id="0e944-176">Se você esquecer o método de autenticação ou o segredo, [redefina as credenciais da entidade de serviço](#reset-credentials).</span><span class="sxs-lookup"><span data-stu-id="0e944-176">If you forget an authentication method or secret, [reset the service principal credentials](#reset-credentials).</span></span>

## <a name="manage-service-principal-roles"></a><span data-ttu-id="0e944-177">Gerenciar funções da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="0e944-177">Manage service principal roles</span></span>

<span data-ttu-id="0e944-178">A CLI do Azure oferece os seguintes comandos para gerenciar as atribuições de função:</span><span class="sxs-lookup"><span data-stu-id="0e944-178">The Azure CLI has the following commands to manage role assignments:</span></span>

* [<span data-ttu-id="0e944-179">az role assignment list</span><span class="sxs-lookup"><span data-stu-id="0e944-179">az role assignment list</span></span>](/cli/azure/role/assignment#az-role-assignment-list)
* [<span data-ttu-id="0e944-180">az role assignment create</span><span class="sxs-lookup"><span data-stu-id="0e944-180">az role assignment create</span></span>](/cli/azure/role/assignment#az-role-assignment-create)
* [<span data-ttu-id="0e944-181">az role assignment delete</span><span class="sxs-lookup"><span data-stu-id="0e944-181">az role assignment delete</span></span>](/cli/azure/role/assignment#az-role-assignment-delete)

<span data-ttu-id="0e944-182">A função padrão para uma entidade de serviço é **Colaborador**.</span><span class="sxs-lookup"><span data-stu-id="0e944-182">The default role for a service principal is **Contributor**.</span></span> <span data-ttu-id="0e944-183">Essa função tem permissões completas para ler e gravar em uma conta do Azure.</span><span class="sxs-lookup"><span data-stu-id="0e944-183">This role has full permissions to read and write to an Azure account.</span></span> <span data-ttu-id="0e944-184">A função **Leitor** é mais restritiva, com acesso somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0e944-184">The **Reader** role is more restrictive, with read-only access.</span></span>  <span data-ttu-id="0e944-185">Para obter mais informações sobre o Controle de Acesso Baseado em Função (RBAC) e funções, confira [RBAC: funções internas](/azure/active-directory/role-based-access-built-in-roles).</span><span class="sxs-lookup"><span data-stu-id="0e944-185">For more information on Role-Based Access Control (RBAC) and roles, see [RBAC: Built-in roles](/azure/active-directory/role-based-access-built-in-roles).</span></span>

<span data-ttu-id="0e944-186">Esse exemplo adiciona a função **Leitor** e exclui a função **Colaborador**:</span><span class="sxs-lookup"><span data-stu-id="0e944-186">This example adds the **Reader** role and removes the **Contributor** one:</span></span>

```azurecli-interactive
az role assignment create --assignee APP_ID --role Reader
az role assignment delete --assignee APP_ID --role Contributor
```

> [!NOTE]
> <span data-ttu-id="0e944-187">Caso sua conta não tenha permissão para atribuir uma função, você verá uma mensagem de erro informando que sua conta “não tem autorização para executar a ação ‘Microsoft.Authorization/roleAssignments/write’”. Entre em contato com o administrador do Azure Active Directory para gerenciar funções.</span><span class="sxs-lookup"><span data-stu-id="0e944-187">If your account doesn't have permission to assign a role, you see an error message that your account "does not have authorization to perform action 'Microsoft.Authorization/roleAssignments/write'." Contact your Azure Active Directory admin to manage roles.</span></span>

<span data-ttu-id="0e944-188">Adicionar uma função _não_ restringe as permissões atribuídas anteriormente.</span><span class="sxs-lookup"><span data-stu-id="0e944-188">Adding a role _doesn't_ restrict previously assigned permissions.</span></span> <span data-ttu-id="0e944-189">Ao restringir as permissões da entidade de serviço, a função __Colaborador__ deverá ser removida.</span><span class="sxs-lookup"><span data-stu-id="0e944-189">When restricting a service principal's permissions, the __Contributor__ role should be removed.</span></span>

<span data-ttu-id="0e944-190">Para verificar as alterações, liste as funções atribuídas:</span><span class="sxs-lookup"><span data-stu-id="0e944-190">The changes can be verified by listing the assigned roles:</span></span>

```azurecli-interactive
az role assignment list --assignee APP_ID
```

## <a name="sign-in-using-a-service-principal"></a><span data-ttu-id="0e944-191">Entrar usando uma entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="0e944-191">Sign in using a service principal</span></span>

<span data-ttu-id="0e944-192">Teste as novas credenciais e permissões da entidade de serviço iniciando a sessão.</span><span class="sxs-lookup"><span data-stu-id="0e944-192">Test the new service principal's credentials and permissions by signing in.</span></span> <span data-ttu-id="0e944-193">Para entrar com uma entidade de serviço, você precisa de `appId`, `tenant` e das credenciais.</span><span class="sxs-lookup"><span data-stu-id="0e944-193">To sign in with a service principal, you need the `appId`, `tenant`, and credentials.</span></span>

<span data-ttu-id="0e944-194">Para entrar com uma entidade de serviço usando a senha:</span><span class="sxs-lookup"><span data-stu-id="0e944-194">To sign in with a service principal using a password:</span></span>

```azurecli-interactive
az login --service-principal --username APP_ID --password PASSWORD --tenant TENANT_ID
```

<span data-ttu-id="0e944-195">Para entrar com um certificado, ele precisa estar disponível localmente como um arquivo PEM ou DER, no formato ASCII.</span><span class="sxs-lookup"><span data-stu-id="0e944-195">To sign in with a certificate, it must be available locally as a PEM or DER file, in ASCII format.</span></span> <span data-ttu-id="0e944-196">Ao usar um arquivo PEM, a **CHAVE PRIVADA** e o **CERTIFICADO** precisam ser anexados juntos dentro do arquivo.</span><span class="sxs-lookup"><span data-stu-id="0e944-196">When using a PEM file, the **PRIVATE KEY** and **CERTIFICATE** must be appended together within the file.</span></span>

```azurecli-interactive
az login --service-principal --username APP_ID --tenant TENANT_ID --password /path/to/cert
```

<span data-ttu-id="0e944-197">Para saber mais sobre como entrar com uma entidade de serviço, confira [Entrar com a CLI do Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="0e944-197">To learn more about signing in with a service principal, see [Sign in with the Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="create-a-resource-using-service-principal"></a><span data-ttu-id="0e944-198">Criar um recurso usando a entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="0e944-198">Create a resource using service principal</span></span>

<span data-ttu-id="0e944-199">A seção a seguir fornece um exemplo de como criar um recurso do [Armazenamento do Azure](/azure/storage/) com uma entidade de serviço usando os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="0e944-199">The following section provides an example of how to create an resource for [Azure Storage](/azure/storage/) with a service principal, using the following commands:</span></span>

* [<span data-ttu-id="0e944-200">az login</span><span class="sxs-lookup"><span data-stu-id="0e944-200">az login</span></span>](/cli/azure/reference-index#az_login)
* [<span data-ttu-id="0e944-201">az group create</span><span class="sxs-lookup"><span data-stu-id="0e944-201">az group create</span></span>](/cli/azure/group#az_group_create)
* [<span data-ttu-id="0e944-202">az storage account create</span><span class="sxs-lookup"><span data-stu-id="0e944-202">az storage account create</span></span>](/cli/azure/storage/account#az_storage_account_create)
* [<span data-ttu-id="0e944-203">az storage account keys list</span><span class="sxs-lookup"><span data-stu-id="0e944-203">az storage account keys list</span></span>](/cli/azure/storage/account/keys#az_storage_account_keys_list)

<span data-ttu-id="0e944-204">Para entrar com uma entidade de serviço, você precisa dos valores de `appId`, `tenant` e `password` retornados como resposta quando você [criou a entidade de serviço](#sign-in-using-a-service-principal).</span><span class="sxs-lookup"><span data-stu-id="0e944-204">To sign in with a service principal, you need the `appId`, `tenant`, and `password` returned as the response when you [created your service principal](#sign-in-using-a-service-principal).</span></span>

1. <span data-ttu-id="0e944-205">Faça logon como a entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="0e944-205">Log in as the service principal.</span></span>

    ```azurecli-interactive
    az login --service-principal --username APP_ID --password PASSWORD --tenant TENANT_ID
    ```

1. <span data-ttu-id="0e944-206">Crie um grupo de recursos para manter todos os recursos usados para o mesmo projeto de início rápido, tutorial ou desenvolvimento.</span><span class="sxs-lookup"><span data-stu-id="0e944-206">Create a resource group to hold all resources used for the same quickstart, tutorial, or development project.</span></span>

    ```azurecli-interactive
    az group create --location WESTUS --name MY_RESOURCE_GROUP
    ```

1. <span data-ttu-id="0e944-207">Crie um recurso para um serviço do Azure.</span><span class="sxs-lookup"><span data-stu-id="0e944-207">Create a resource to an Azure service.</span></span> <span data-ttu-id="0e944-208">Substitua `<SERVICENAME>` pelo nome do serviço do Azure.</span><span class="sxs-lookup"><span data-stu-id="0e944-208">Replace `<SERVICENAME>` with the name of the Azure service.</span></span>

    <span data-ttu-id="0e944-209">Para o Armazenamento do Azure, os valores válidos para o parâmetro `<KIND>` são:</span><span class="sxs-lookup"><span data-stu-id="0e944-209">For Azure Storage, valid values for the `<KIND>` parameter are:</span></span>

    * <span data-ttu-id="0e944-210">BlobStorage</span><span class="sxs-lookup"><span data-stu-id="0e944-210">BlobStorage</span></span>
    * <span data-ttu-id="0e944-211">BlockBlobStorage</span><span class="sxs-lookup"><span data-stu-id="0e944-211">BlockBlobStorage</span></span>
    * <span data-ttu-id="0e944-212">FileStorage</span><span class="sxs-lookup"><span data-stu-id="0e944-212">FileStorage</span></span>
    * <span data-ttu-id="0e944-213">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="0e944-213">Storage</span></span>
    * <span data-ttu-id="0e944-214">StorageV2</span><span class="sxs-lookup"><span data-stu-id="0e944-214">StorageV2</span></span>

    ```azurecli-interactive
    az storage account create --name MY_RESOURCE_<SERVICENAME> --resource-group MY_RESOURCE_GROUP --kind <KIND> --sku F0 --location WESTUS --yes
    ```

1. <span data-ttu-id="0e944-215">Obtenha as chaves de recurso para o novo recurso, que você usa em seu código para se autenticar no serviço do Azure.</span><span class="sxs-lookup"><span data-stu-id="0e944-215">Get resource keys for the new resource, which you use in your code to authenticate to the Azure service.</span></span>

    ```azurecli-interactive
    az storage account keys list --name MY_RESOURCE_<SERVICENAME> --resource-group MY_RESOURCE_GROUP
    ```

## <a name="reset-credentials"></a><span data-ttu-id="0e944-216">Redefinir credenciais</span><span class="sxs-lookup"><span data-stu-id="0e944-216">Reset credentials</span></span>

<span data-ttu-id="0e944-217">Se você esquecer as credenciais de uma entidade de serviço, use o comando [az ad sp credencial reset](/cli/azure/ad/sp/credential#az-ad-sp-credential-reset).</span><span class="sxs-lookup"><span data-stu-id="0e944-217">If you forget the credentials for a service principal, use [az ad sp credential reset](/cli/azure/ad/sp/credential#az-ad-sp-credential-reset).</span></span> <span data-ttu-id="0e944-218">O comando reset tem os mesmos argumentos que `az ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="0e944-218">The reset command takes the same arguments as `az ad sp create-for-rbac`.</span></span>

```azurecli-interactive
az ad sp credential reset --name APP_ID
```

## <a name="see-also"></a><span data-ttu-id="0e944-219">Confira também</span><span class="sxs-lookup"><span data-stu-id="0e944-219">See also</span></span>

* [<span data-ttu-id="0e944-220">Objetos de entidade de serviço e aplicativo no Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="0e944-220">Application and service principal objects in Azure Active Directory</span></span>](/azure/active-directory/develop/app-objects-and-service-principals)
* [<span data-ttu-id="0e944-221">Como gerenciar entidades de serviço</span><span class="sxs-lookup"><span data-stu-id="0e944-221">How to manage service principals</span></span>](/azure/developer/python/how-to-manage-service-principals)
