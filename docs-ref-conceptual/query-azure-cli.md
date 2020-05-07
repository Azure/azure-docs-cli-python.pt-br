---
title: Resultados de comando de consulta com a CLI do Azure
description: Saiba como realizar consultas JMESPath na saída dos comandos da CLI do Azure.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/23/2019
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: c9f0afdd626ac8d9af027db02275e5a553595473
ms.sourcegitcommit: ee64dc738cfe689a2a479e32a87bf420f96c31c8
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2020
ms.locfileid: "79060451"
---
# <a name="query-azure-cli-command-output"></a><span data-ttu-id="25879-103">Consultar a saída do comando da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="25879-103">Query Azure CLI command output</span></span>

<span data-ttu-id="25879-104">A CLI do Azure usa o argumento `--query` para executar uma [consulta JMESPath](http://jmespath.org) nos resultados dos comandos.</span><span class="sxs-lookup"><span data-stu-id="25879-104">The Azure CLI uses the `--query` argument to execute a [JMESPath query](http://jmespath.org) on the results of commands.</span></span> <span data-ttu-id="25879-105">JMESPath é uma linguagem de consulta do JSON, permitindo que você selecione e modifique os dados na saída da CLI.</span><span class="sxs-lookup"><span data-stu-id="25879-105">JMESPath is a query language for JSON, giving you the ability to select and modify data from CLI output.</span></span> <span data-ttu-id="25879-106">As consultas são executadas na saída do JSON antes de qualquer formatação da exibição.</span><span class="sxs-lookup"><span data-stu-id="25879-106">Queries are executed on the JSON output before any display formatting.</span></span>

<span data-ttu-id="25879-107">O argumento `--query` tem suporte de todos os comandos na CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="25879-107">The `--query` argument is supported by all commands in the Azure CLI.</span></span> <span data-ttu-id="25879-108">Este artigo aborda como usar os recursos do JMESPath com uma série de exemplos pequenos e simples.</span><span class="sxs-lookup"><span data-stu-id="25879-108">This article covers how to use the features of JMESPath with a series of small, simple examples.</span></span>

## <a name="dictionary-and-list-cli-results"></a><span data-ttu-id="25879-109">Dicionário e lista dos resultados da CLI</span><span class="sxs-lookup"><span data-stu-id="25879-109">Dictionary and list CLI results</span></span>

<span data-ttu-id="25879-110">Mesmo ao usar um formato de saída diferente do JSON, os resultados do comando da CLI são tratados primeiro como JSON para consultas.</span><span class="sxs-lookup"><span data-stu-id="25879-110">Even when using an output format other than JSON, CLI command results are first treated as JSON for queries.</span></span> <span data-ttu-id="25879-111">Os resultados da CLI são uma matriz JSON ou um dicionário.</span><span class="sxs-lookup"><span data-stu-id="25879-111">CLI results are either a JSON array or dictionary.</span></span> <span data-ttu-id="25879-112">Matrizes são sequências de objetos que podem ser indexados, e dicionários são objetos não ordenados acessados com chaves.</span><span class="sxs-lookup"><span data-stu-id="25879-112">Arrays are sequences of objects that can be indexed, and dictionaries are unordered objects accessed with keys.</span></span> <span data-ttu-id="25879-113">Os comandos que _poderiam_ retornar mais de um objeto retornam uma matriz, e os comandos que _sempre_ retornam _apenas_ um objeto retornam um dicionário.</span><span class="sxs-lookup"><span data-stu-id="25879-113">Commands that _could_ return more than one object return an array, and commands that _always_ return _only_ a single object return a dictionary.</span></span>

## <a name="get-properties-in-a-dictionary"></a><span data-ttu-id="25879-114">Obter propriedades em um dicionário</span><span class="sxs-lookup"><span data-stu-id="25879-114">Get properties in a dictionary</span></span>

<span data-ttu-id="25879-115">Trabalhando com os resultados do dicionário, você pode acessar as propriedades no nível superior com apenas a chave.</span><span class="sxs-lookup"><span data-stu-id="25879-115">Working with dictionary results, you can access properties from the top level with just the key.</span></span> <span data-ttu-id="25879-116">O caractere `.` (__subexpressão__) é usado para acessar as propriedades dos dicionários aninhados.</span><span class="sxs-lookup"><span data-stu-id="25879-116">The `.` (__subexpression__) character is used to access properties of nested dictionaries.</span></span> <span data-ttu-id="25879-117">Antes de apresentar as consultas, examine a saída não modificada do comando `az vm show`:</span><span class="sxs-lookup"><span data-stu-id="25879-117">Before introducing queries, take a look at the unmodified output of the `az vm show` command:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM -o json
```

<span data-ttu-id="25879-118">O comando produzirá um dicionário.</span><span class="sxs-lookup"><span data-stu-id="25879-118">The command will output a dictionary.</span></span> <span data-ttu-id="25879-119">Parte do conteúdo foi omitida.</span><span class="sxs-lookup"><span data-stu-id="25879-119">Some content has been omitted.</span></span>

```json
{
  "additionalCapabilities": null,
  "availabilitySet": null,
  "diagnosticsProfile": {
    "bootDiagnostics": {
      "enabled": true,
      "storageUri": "https://xxxxxx.blob.core.windows.net/"
    }
  },
  ...
  "osProfile": {
    "adminPassword": null,
    "adminUsername": "azureuser",
    "allowExtensionOperations": true,
    "computerName": "TestVM",
    "customData": null,
    "linuxConfiguration": {
      "disablePasswordAuthentication": true,
      "provisionVmAgent": true,
      "ssh": {
        "publicKeys": [
          {
            "keyData": "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDMobZNJTqgjWn/IB5xlilvE4Y+BMYpqkDnGRUcA0g9BYPgrGSQquCES37v2e3JmpfDPHFsaR+CPKlVr2GoVJMMHeRcMJhj50ZWq0hAnkJBhlZVWy8S7dwdGAqPyPmWM2iJDCVMVrLITAJCno47O4Ees7RCH6ku7kU86b1NOanvrNwqTHr14wtnLhgZ0gQ5GV1oLWvMEVg1YFMIgPRkTsSQKWCG5lLqQ45aU/4NMJoUxGyJTL9i8YxMavaB1Z2npfTQDQo9+womZ7SXzHaIWC858gWNl9e5UFyHDnTEDc14hKkf1CqnGJVcCJkmSfmrrHk/CkmF0ZT3whTHO1DhJTtV stramer@contoso",
            "path": "/home/azureuser/.ssh/authorized_keys"
          }
        ]
      }
    },
    "secrets": [],
    "windowsConfiguration": null
  },
  ....
}
```

<span data-ttu-id="25879-120">O comando a seguir obtém as chaves SSH públicas autorizadas para conectar a VM adicionando uma consulta:</span><span class="sxs-lookup"><span data-stu-id="25879-120">The following command gets the SSH public keys authorized to connect to the VM by adding a query:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query osProfile.linuxConfiguration.ssh.publicKeys -o json
```

```json
[
  {
    "keyData": "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDMobZNJTqgjWn/IB5xlilvE4Y+BMYpqkDnGRUcA0g9BYPgrGSQquCES37v2e3JmpfDPHFsaR+CPKlVr2GoVJMMHeRcMJhj50ZWq0hAnkJBhlZVWy8S7dwdGAqPyPmWM2iJDCVMVrLITAJCno47O4Ees7RCH6ku7kU86b1NOanvrNwqTHr14wtnLhgZ0gQ5GV1oLWvMEVg1YFMIgPRkTsSQKWCG5lLqQ45aU/4NMJoUxGyJTL9i8YxMavaB1Z2npfTQDQo9+womZ7SXzHaIWC858gWNl9e5UFyHDnTEDc14hKkf1CqnGJVcCJkmSfmrrHk/CkmF0ZT3whTHO1DhJTtV stramer@contoso",
    "path": "/home/azureuser/.ssh/authorized_keys"
  }
]
```

## <a name="get-a-single-value"></a><span data-ttu-id="25879-121">Obter um valor único</span><span class="sxs-lookup"><span data-stu-id="25879-121">Get a single value</span></span>

<span data-ttu-id="25879-122">Um caso comum é precisar obter somente _um_ valor de um comando da CLI, como uma ID do recurso do Azure, um nome de recurso, um nome de usuário ou uma senha.</span><span class="sxs-lookup"><span data-stu-id="25879-122">A common case is that you need to only get _one_ value out of a CLI command, such as an Azure resource ID, a resource name, a username, or a password.</span></span> <span data-ttu-id="25879-123">Nesse caso, muitas vezes você também quer armazenar o valor em uma variável de ambiente local.</span><span class="sxs-lookup"><span data-stu-id="25879-123">In that case, you also often want to store the value in a local environment variable.</span></span> <span data-ttu-id="25879-124">Para obter uma propriedade única, primeiro, verifique se você está recebendo somente uma propriedade da consulta.</span><span class="sxs-lookup"><span data-stu-id="25879-124">To get a single property, first make sure that you're only getting one property out of the query.</span></span> <span data-ttu-id="25879-125">Ao modificar o último exemplo para obter somente o nome de usuário do administrador:</span><span class="sxs-lookup"><span data-stu-id="25879-125">Modifying the last example to get only the admin username:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'osProfile.adminUsername' -o json
```

```JSON
"azureuser"
```

<span data-ttu-id="25879-126">Parece um valor único válido, mas observe que os caracteres `"` são retornados como parte da saída.</span><span class="sxs-lookup"><span data-stu-id="25879-126">This looks like a valid single value, but note that the `"` characters are returned as part of the output.</span></span> <span data-ttu-id="25879-127">Isso indica que o objeto é uma cadeia de caracteres JSON.</span><span class="sxs-lookup"><span data-stu-id="25879-127">This indicates that the object is a JSON string.</span></span> <span data-ttu-id="25879-128">É importante observar que ao atribuir esse valor diretamente à variável de ambiente como saída do comando, as aspas podem __não__ ser interpretadas pelo shell:</span><span class="sxs-lookup"><span data-stu-id="25879-128">It's important to note that when you assign this value directly as output from the command to an environment variable, the quotes may __not__ be interpreted by the shell:</span></span>

```bash
USER=$(az vm show -g QueryDemo -n TestVM --query 'osProfile.adminUsername' -o json)
echo $USER
```

```output
"azureuser"
```

<span data-ttu-id="25879-129">Certamente, isso não é desejado.</span><span class="sxs-lookup"><span data-stu-id="25879-129">This is almost certainly not what you want.</span></span> <span data-ttu-id="25879-130">Nesse caso, você quer usar um formato de saída que não inclua os valores retornados com as informações de tipo.</span><span class="sxs-lookup"><span data-stu-id="25879-130">In this case, you want to use an output format which doesn't enclose returned values with type information.</span></span> <span data-ttu-id="25879-131">A melhor opção de saída oferecida pela CLI para este fim é `tsv`, valores separados por tabulações.</span><span class="sxs-lookup"><span data-stu-id="25879-131">The best output option that the CLI offers for this purpose is `tsv`, tab-separated values.</span></span> <span data-ttu-id="25879-132">Em especial, ao recuperar um valor que é somente um valor único (e não um dicionário ou uma lista), garante-se que a saída `tsv` não tenha aspas.</span><span class="sxs-lookup"><span data-stu-id="25879-132">In particular, when retrieving a value that's only a single value (not a dictionary or list), `tsv` output is guaranteed to be unquoted.</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'osProfile.adminUsername' -o tsv
```

```output
azureuser
```

<span data-ttu-id="25879-133">Para saber mais sobre o formato de saída `tsv`, confira [Formatos de saída – Formato de saída TSV](format-output-azure-cli.md#tsv-output-format)</span><span class="sxs-lookup"><span data-stu-id="25879-133">For more information about the `tsv` output format, see [Output formats - TSV output format](format-output-azure-cli.md#tsv-output-format)</span></span>

## <a name="get-multiple-values"></a><span data-ttu-id="25879-134">Obter vários valores</span><span class="sxs-lookup"><span data-stu-id="25879-134">Get multiple values</span></span>

<span data-ttu-id="25879-135">Para obter mais de uma propriedade, coloque as expressões entre colchetes `[ ]` (uma __lista de seleção múltipla__), como uma lista separada por vírgulas.</span><span class="sxs-lookup"><span data-stu-id="25879-135">To get more than one property, put expressions in square brackets  `[ ]` (a __multiselect list__) as a comma-separated list.</span></span> <span data-ttu-id="25879-136">Para obter o nome da VM, o usuário administrador e a chave SSH juntos, use o comando:</span><span class="sxs-lookup"><span data-stu-id="25879-136">To get the VM name, admin user, and SSH key all at once use the command:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query '[name, osProfile.adminUsername, osProfile.linuxConfiguration.ssh.publicKeys[0].keyData]' -o json
```

```json
[
  "TestVM",
  "azureuser",
  "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDMobZNJTqgjWn/IB5xlilvE4Y+BMYpqkDnGRUcA0g9BYPgrGSQquCES37v2e3JmpfDPHFsaR+CPKlVr2GoVJMMHeRcMJhj50ZWq0hAnkJBhlZVWy8S7dwdGAqPyPmWM2iJDCVMVrLITAJCno47O4Ees7RCH6ku7kU86b1NOanvrNwqTHr14wtnLhgZ0gQ5GV1oLWvMEVg1YFMIgPRkTsSQKWCG5lLqQ45aU/4NMJoUxGyJTL9i8YxMavaB1Z2npfTQDQo9+womZ7SXzHaIWC858gWNl9e5UFyHDnTEDc14hKkf1CqnGJVcCJkmSfmrrHk/CkmF0ZT3whTHO1DhJTtV stramer@contoso"
]
```

<span data-ttu-id="25879-137">Esses valores são listados na matriz de resultados na ordem em que foram fornecidos na consulta.</span><span class="sxs-lookup"><span data-stu-id="25879-137">These values are listed in the result array in the order they were given in the query.</span></span> <span data-ttu-id="25879-138">Como o resultado é uma matriz, não há nenhuma chave associada a ele.</span><span class="sxs-lookup"><span data-stu-id="25879-138">Since the result is an array, there are no keys associated with the results.</span></span>

## <a name="rename-properties-in-a-query"></a><span data-ttu-id="25879-139">Renomear as propriedades em uma consulta</span><span class="sxs-lookup"><span data-stu-id="25879-139">Rename properties in a query</span></span>

<span data-ttu-id="25879-140">Para obter um dicionário, em vez de uma matriz, ao consultar diversos valores, use o operador `{ }` (__hash de seleção múltipla__).</span><span class="sxs-lookup"><span data-stu-id="25879-140">To get a dictionary instead of an array when querying for multiple values, use the `{ }` (__multiselect hash__) operator.</span></span>
<span data-ttu-id="25879-141">O formato de um hash de seleção múltipla é `{displayName:JMESPathExpression, ...}`.</span><span class="sxs-lookup"><span data-stu-id="25879-141">The format for a multiselect hash is `{displayName:JMESPathExpression, ...}`.</span></span>
<span data-ttu-id="25879-142">`displayName` será a cadeia de caracteres mostrada na saída e `JMESPathExpression` é a expressão do JMESPath a avaliar.</span><span class="sxs-lookup"><span data-stu-id="25879-142">`displayName` will be the string shown in output, and `JMESPathExpression` is the JMESPath expression to evaluate.</span></span> <span data-ttu-id="25879-143">Modificando o exemplo da seção anterior alterando a lista de seleção múltipla para um hash:</span><span class="sxs-lookup"><span data-stu-id="25879-143">Modifying the example from the last section by changing the multiselect list to a hash:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query '{VMName:name, admin:osProfile.adminUsername, sshKey:osProfile.linuxConfiguration.ssh.publicKeys[0].keyData }' -o json
```

```json
{
  "VMName": "TestVM",
  "admin": "azureuser",
  "ssh-key": "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDMobZNJTqgjWn/IB5xlilvE4Y+BMYpqkDnGRUcA0g9BYPgrGSQquCES37v2e3JmpfDPHFsaR+CPKlVr2GoVJMMHeRcMJhj50ZWq0hAnkJBhlZVWy8S7dwdGAqPyPmWM2iJDCVMVrLITAJCno47O4Ees7RCH6ku7kU86b1NOanvrNwqTHr14wtnLhgZ0gQ5GV1oLWvMEVg1YFMIgPRkTsSQKWCG5lLqQ45aU/4NMJoUxGyJTL9i8YxMavaB1Z2npfTQDQo9+womZ7SXzHaIWC858gWNl9e5UFyHDnTEDc14hKkf1CqnGJVcCJkmSfmrrHk/CkmF0ZT3whTHO1DhJTtV stramer@contoso"
}
```

## <a name="get-properties-in-an-array"></a><span data-ttu-id="25879-144">Obter propriedades em uma matriz</span><span class="sxs-lookup"><span data-stu-id="25879-144">Get properties in an array</span></span>

<span data-ttu-id="25879-145">Uma matriz não tem nenhuma propriedade, mas pode ser indexada.</span><span class="sxs-lookup"><span data-stu-id="25879-145">An array has no properties of its own, but it can be indexed.</span></span> <span data-ttu-id="25879-146">Esse recurso é mostrado no último exemplo com a expressão `publicKeys[0]`, que obtém o primeiro elemento da matriz `publicKeys`.</span><span class="sxs-lookup"><span data-stu-id="25879-146">This feature is shown in the last example with the expression `publicKeys[0]`, which gets the first element of the `publicKeys` array.</span></span> <span data-ttu-id="25879-147">Não há nenhuma garantia de que a CLI de saída será ordenada, portanto, evite usar a indexação, a menos que tenha certeza da ordem ou não se importe com o elemento obtido.</span><span class="sxs-lookup"><span data-stu-id="25879-147">There's no guarantee CLI output is ordered, so avoid using indexing unless you're sure of the order or don't care what element you get.</span></span> <span data-ttu-id="25879-148">Para acessar as propriedades dos elementos em uma matriz, execute uma das duas operações: _nivelamento_ e _filtragem_.</span><span class="sxs-lookup"><span data-stu-id="25879-148">To access the properties of elements in an array, you do one of two operations: _flattening_ and _filtering_.</span></span> <span data-ttu-id="25879-149">Esta seção aborda como nivelar uma matriz.</span><span class="sxs-lookup"><span data-stu-id="25879-149">This section covers how to flatten an array.</span></span>

<span data-ttu-id="25879-150">O nivelamento de uma matriz é feito com o operador `[]` do JMESPath.</span><span class="sxs-lookup"><span data-stu-id="25879-150">Flattening an array is done with the `[]` JMESPath operator.</span></span> <span data-ttu-id="25879-151">Todas as expressões após o operador `[]` são aplicadas em cada elemento na matriz atual.</span><span class="sxs-lookup"><span data-stu-id="25879-151">All expressions after the `[]` operator are applied to each element in the current array.</span></span>
<span data-ttu-id="25879-152">Se `[]` aparecer no início da consulta, ele nivelará o resultado do comando da CLI.</span><span class="sxs-lookup"><span data-stu-id="25879-152">If `[]` appears at the start of the query, it flattens the CLI command result.</span></span> <span data-ttu-id="25879-153">Os resultados de `az vm list` podem ser examinados com esse recurso.</span><span class="sxs-lookup"><span data-stu-id="25879-153">The results of `az vm list` can be inspected with this feature.</span></span>
<span data-ttu-id="25879-154">Para obter o nome, o SO e o nome do administrador de cada VM em um grupo de recursos:</span><span class="sxs-lookup"><span data-stu-id="25879-154">To get the name, OS, and administrator name for each VM in a resource group:</span></span>

```azurecli-interactive
az vm list -g QueryDemo --query '[].{Name:name, OS:storageProfile.osDisk.osType, admin:osProfile.adminUsername}' -o json
```

```json
[
  {
    "Name": "Test-2",
    "OS": "Linux",
    "admin": "sttramer"
  },
  {
    "Name": "TestVM",
    "OS": "Linux",
    "admin": "azureuser"
  },
  {
    "Name": "WinTest",
    "OS": "Windows",
    "admin": "winadmin"
  }
]
```

<span data-ttu-id="25879-155">Quando combinados com o formato de saída `--output table`, os nomes de colunas correspondem ao valor `displayKey` do hash de seleção múltipla:</span><span class="sxs-lookup"><span data-stu-id="25879-155">When combined with the `--output table` output format, the column names match up with the `displayKey` value of the multiselect hash:</span></span>

```azurecli-interactive
az vm list -g QueryDemo --query '[].{Name:name, OS:storageProfile.osDisk.osType, Admin:osProfile.adminUsername}' --output table
```

```output
Name     OS       Admin
-------  -------  ---------
Test-2   Linux    sttramer
TestVM   Linux    azureuser
WinTest  Windows  winadmin
```

> [!NOTE]
>
> <span data-ttu-id="25879-156">Algumas chaves são filtradas e não são impressas na exibição da tabela.</span><span class="sxs-lookup"><span data-stu-id="25879-156">Certain keys are filtered out and not printed in the table view.</span></span> <span data-ttu-id="25879-157">Essas chaves são `id`, `type` e `etag`.</span><span class="sxs-lookup"><span data-stu-id="25879-157">These keys are `id`, `type`, and `etag`.</span></span> <span data-ttu-id="25879-158">Para ver esses valores, você pode alterar o nome da chave em um hash de seleção múltipla.</span><span class="sxs-lookup"><span data-stu-id="25879-158">To see these values, you can change the key name in a multiselect hash.</span></span>
>
> ```azurecli-interactive
> az vm show -g QueryDemo -n TestVM --query "{objectID:id}" -o table
> ```

<span data-ttu-id="25879-159">Qualquer matriz pode ser nivelada, não apenas o resultado de alto nível retornado pelo comando.</span><span class="sxs-lookup"><span data-stu-id="25879-159">Any array can be flattened, not just the top-level result returned by the command.</span></span> <span data-ttu-id="25879-160">Na última seção, a expressão `osProfile.linuxConfiguration.ssh.publicKeys[0].keyData` foi usada para obter a chave SSH pública para entrar.</span><span class="sxs-lookup"><span data-stu-id="25879-160">In the last section, the expression `osProfile.linuxConfiguration.ssh.publicKeys[0].keyData` was used to get the SSH public key for sign-in.</span></span> <span data-ttu-id="25879-161">Para obter _cada_ chave SSH pública, a expressão pode ser escrita como `osProfile.linuxConfiguration.ssh.publicKeys[].keyData`.</span><span class="sxs-lookup"><span data-stu-id="25879-161">To get _every_ SSH public key, the expression could instead be written as `osProfile.linuxConfiguration.ssh.publicKeys[].keyData`.</span></span>
<span data-ttu-id="25879-162">Esta expressão de consulta nivela a matriz `osProfile.linuxConfiguration.ssh.publicKeys` e executa a expressão `keyData` em cada elemento:</span><span class="sxs-lookup"><span data-stu-id="25879-162">This query expression flattens the `osProfile.linuxConfiguration.ssh.publicKeys` array, and then runs the `keyData` expression on each element:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query '{VMName:name, admin:osProfile.adminUsername, sshKeys:osProfile.linuxConfiguration.ssh.publicKeys[].keyData }' -o json
```

```json
{
  "VMName": "TestVM",
  "admin": "azureuser",
  "sshKeys": [
    "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDMobZNJTqgjWn/IB5xlilvE4Y+BMYpqkDnGRUcA0g9BYPgrGSQquCES37v2e3JmpfDPHFsaR+CPKlVr2GoVJMMHeRcMJhj50ZWq0hAnkJBhlZVWy8S7dwdGAqPyPmWM2iJDCVMVrLITAJCno47O4Ees7RCH6ku7kU86b1NOanvrNwqTHr14wtnLhgZ0gQ5GV1oLWvMEVg1YFMIgPRkTsSQKWCG5lLqQ45aU/4NMJoUxGyJTL9i8YxMavaB1Z2npfTQDQo9+womZ7SXzHaIWC858gWNl9e5UFyHDnTEDc14hKkf1CqnGJVcCJkmSfmrrHk/CkmF0ZT3whTHO1DhJTtV stramer@contoso\n"
  ]
}
```

## <a name="filter-arrays"></a><span data-ttu-id="25879-163">Filtrar matrizes</span><span class="sxs-lookup"><span data-stu-id="25879-163">Filter arrays</span></span>

<span data-ttu-id="25879-164">A outra operação usada para obter dados de uma matriz é a _filtragem_.</span><span class="sxs-lookup"><span data-stu-id="25879-164">The other operation used to get data from an array is _filtering_.</span></span> <span data-ttu-id="25879-165">A filtragem é feita com o operador `[?...]` do JMESPath.</span><span class="sxs-lookup"><span data-stu-id="25879-165">Filtering is done with the `[?...]` JMESPath operator.</span></span>
<span data-ttu-id="25879-166">Esse operador usa um predicado como conteúdo.</span><span class="sxs-lookup"><span data-stu-id="25879-166">This operator takes a predicate as its contents.</span></span> <span data-ttu-id="25879-167">Um predicado é qualquer instrução que pode ser avaliada como `true` ou `false`.</span><span class="sxs-lookup"><span data-stu-id="25879-167">A predicate is any statement that can be evaluated to either `true` or `false`.</span></span> <span data-ttu-id="25879-168">As expressões em que o predicado é avaliado como `true` são incluídas na saída.</span><span class="sxs-lookup"><span data-stu-id="25879-168">Expressions where the predicate evaluates to `true` are included in the output.</span></span>

<span data-ttu-id="25879-169">JMESPath oferece a comparação padrão e os operadores lógicos.</span><span class="sxs-lookup"><span data-stu-id="25879-169">JMESPath offers the standard comparison and logical operators.</span></span> <span data-ttu-id="25879-170">Eles incluem `<`, `<=`, `>`, `>=`, `==` e `!=`.</span><span class="sxs-lookup"><span data-stu-id="25879-170">These include `<`, `<=`, `>`, `>=`, `==`, and `!=`.</span></span>
<span data-ttu-id="25879-171">JMESPath também dá suporte às operações lógicas e (`&&`) ou (`||`), e não (`!`).</span><span class="sxs-lookup"><span data-stu-id="25879-171">JMESPath also supports logical and (`&&`), or (`||`), and not (`!`).</span></span> <span data-ttu-id="25879-172">Expressões podem ser agrupadas entre parênteses, permitindo expressões de predicado mais complexas.</span><span class="sxs-lookup"><span data-stu-id="25879-172">Expressions can be grouped within parenthesis, allowing for more complex predicate expressions.</span></span> <span data-ttu-id="25879-173">Para obter mais detalhes sobre predicados e operações lógicas, confira a [especificação do JMESPath](http://jmespath.org/specification.html).</span><span class="sxs-lookup"><span data-stu-id="25879-173">For the full details on predicates and logical operations, see the [JMESPath specification](http://jmespath.org/specification.html).</span></span>

<span data-ttu-id="25879-174">Na última seção, nivelamos uma matriz para obter a lista completa de todas as VMs em um grupo de recursos.</span><span class="sxs-lookup"><span data-stu-id="25879-174">In the last section, we flattened an array to get the complete list of all VMs in a resource group.</span></span> <span data-ttu-id="25879-175">Usando filtros, essa saída pode ser restrita apenas às VMs do Linux:</span><span class="sxs-lookup"><span data-stu-id="25879-175">Using filters, this output can be restricted to only Linux VMs:</span></span>

```azurecli-interactive
az vm list -g QueryDemo --query "[?storageProfile.osDisk.osType=='Linux'].{Name:name,  admin:osProfile.adminUsername}" --output table
```

```output
Name    Admin
------  ---------
Test-2  sttramer
TestVM  azureuser
```

> [!IMPORTANT]
>
> <span data-ttu-id="25879-176">No JMESPath, as cadeias de caracteres sempre ficam entre aspas simples (`'`).</span><span class="sxs-lookup"><span data-stu-id="25879-176">In JMESPath, strings are always surrounded by single quotes (`'`).</span></span> <span data-ttu-id="25879-177">Se você usar aspas duplas como parte de uma cadeia de caracteres em um predicado de filtro, obterá uma saída vazia.</span><span class="sxs-lookup"><span data-stu-id="25879-177">If you use double quotes as part of a string in a filter predicate, you'll get empty output.</span></span>

<span data-ttu-id="25879-178">O JMESPath também tem funções internas que podem ajudar na filtragem.</span><span class="sxs-lookup"><span data-stu-id="25879-178">JMESPath also has built-in functions that can help with filtering.</span></span> <span data-ttu-id="25879-179">Uma dessas funções é `contains(string, substring)`, que verifica se uma cadeia de caracteres contém uma subcadeia.</span><span class="sxs-lookup"><span data-stu-id="25879-179">One such function is `contains(string, substring)`, which checks to see if a string contains a substring.</span></span> <span data-ttu-id="25879-180">As expressões são avaliadas antes de chamar a função, portanto, o primeiro argumento pode ser uma expressão completa do JMESPath.</span><span class="sxs-lookup"><span data-stu-id="25879-180">Expressions are evaluated before calling the function, so the first argument can be a full JMESPath expression.</span></span> <span data-ttu-id="25879-181">O exemplo a seguir localiza todas as VMs usando o armazenamento SSD para seu disco do SO:</span><span class="sxs-lookup"><span data-stu-id="25879-181">The next example finds all VMs using SSD storage for their OS disk:</span></span>

```azurecli-interactive
az vm list -g QueryDemo --query "[?contains(storageProfile.osDisk.managedDisk.storageAccountType,'SSD')].{Name:name, Storage:storageProfile.osDisk.managedDisk.storageAccountType}" -o json
```

```json
[
  {
    "Name": "TestVM",
    "Storage": "StandardSSD_LRS"
  },
  {
    "Name": "WinTest",
    "Storage": "StandardSSD_LRS"
  }
]
```

<span data-ttu-id="25879-182">Essa consulta é um pouco longa.</span><span class="sxs-lookup"><span data-stu-id="25879-182">This query is a little long.</span></span> <span data-ttu-id="25879-183">A chave `storageProfile.osDisk.managedDisk.storageAccountType` é mencionada duas vezes e rechaveada na saída.</span><span class="sxs-lookup"><span data-stu-id="25879-183">The `storageProfile.osDisk.managedDisk.storageAccountType` key is mentioned twice, and rekeyed in the output.</span></span> <span data-ttu-id="25879-184">Uma maneira de reduzi-la é aplicar o filtro depois de nivelar e selecionar os dados.</span><span class="sxs-lookup"><span data-stu-id="25879-184">One way to shorten it is to apply the filter after flattening and selecting data.</span></span>

```azurecli-interactive
az vm list -g QueryDemo --query "[].{Name:name, Storage:storageProfile.osDisk.managedDisk.storageAccountType}[?contains(Storage,'SSD')]" -o json
```

```json
[
  {
    "Name": "TestVM",
    "Storage": "StandardSSD_LRS"
  },
  {
    "Name": "WinTest",
    "Storage": "StandardSSD_LRS"
  }
]
```

<span data-ttu-id="25879-185">Para matrizes grandes, pode ser mais rápido aplicar o filtro antes de selecionar os dados.</span><span class="sxs-lookup"><span data-stu-id="25879-185">For large arrays, it may be faster to apply the filter before selecting data.</span></span>

<span data-ttu-id="25879-186">Confira a [Especificação do JMESPath - Funções Internas](http://jmespath.org/specification.html#built-in-functions) para obter a lista completa de funções.</span><span class="sxs-lookup"><span data-stu-id="25879-186">See the [JMESPath specification - Built-in Functions](http://jmespath.org/specification.html#built-in-functions) for the full list of functions.</span></span>

## <a name="change-output"></a><span data-ttu-id="25879-187">Alterar a saída</span><span class="sxs-lookup"><span data-stu-id="25879-187">Change output</span></span>

<span data-ttu-id="25879-188">As funções do JMESPath também têm outra finalidade, que é operar nos resultados de uma consulta.</span><span class="sxs-lookup"><span data-stu-id="25879-188">JMESPath functions also have another purpose, which is to operate on the results of a query.</span></span> <span data-ttu-id="25879-189">Qualquer função que retorna um valor não booliano altera o resultado de uma expressão.</span><span class="sxs-lookup"><span data-stu-id="25879-189">Any function that returns a non-boolean value changes the result of an expression.</span></span>
<span data-ttu-id="25879-190">Por exemplo, você pode classificar os dados por um valor de propriedade com `sort_by(array, &sort_expression)`.</span><span class="sxs-lookup"><span data-stu-id="25879-190">For example, you can sort data by a property value with `sort_by(array, &sort_expression)`.</span></span> <span data-ttu-id="25879-191">O JMESPath usa um operador especial, `&`, para as expressões que devem ser avaliadas posteriormente como parte de uma função.</span><span class="sxs-lookup"><span data-stu-id="25879-191">JMESPath uses a special operator, `&`, for expressions that should be evaluated later as part of a function.</span></span> <span data-ttu-id="25879-192">O exemplo a seguir mostra como classificar uma lista de VMs pelo tamanho de disco do SO:</span><span class="sxs-lookup"><span data-stu-id="25879-192">The next example shows how to sort a VM list by OS disk size:</span></span>

```azurecli-interactive
az vm list -g QueryDemo --query "sort_by([].{Name:name, Size:storageProfile.osDisk.diskSizeGb}, &Size)" --output table
```

```output
Name     Size
-------  ------
TestVM   30
Test-2   32
WinTest  127
```

<span data-ttu-id="25879-193">Confira a [Especificação do JMESPath - Funções Internas](http://jmespath.org/specification.html#built-in-functions) para obter a lista completa de funções.</span><span class="sxs-lookup"><span data-stu-id="25879-193">See the [JMESPath specification - Built-in Functions](http://jmespath.org/specification.html#built-in-functions) for the full list of functions.</span></span>

## <a name="experiment-with-queries-interactively"></a><span data-ttu-id="25879-194">Experimentar consultas interativamente</span><span class="sxs-lookup"><span data-stu-id="25879-194">Experiment with queries interactively</span></span>

<span data-ttu-id="25879-195">Para começar a experimentar o JMESPath, o pacote [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) do Python oferece um ambiente interativo para trabalhar com as consultas.</span><span class="sxs-lookup"><span data-stu-id="25879-195">To start experimenting with JMESPath, the [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) Python package offers an interactive environment to work with queries.</span></span> <span data-ttu-id="25879-196">Os dados são transferidos como entrada e as consultas são gravadas e executadas no editor.</span><span class="sxs-lookup"><span data-stu-id="25879-196">Data is piped as input, and then queries are written and run in the editor.</span></span>

```bash
pip install jmespath-terminal
az vm list --output json | jpterm
```
