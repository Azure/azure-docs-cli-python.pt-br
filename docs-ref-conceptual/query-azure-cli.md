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
ms.custom: devx-track-azurecli
ms.openlocfilehash: 780fc2dc87f949a1f36228af7a49cd987cb10cf6
ms.sourcegitcommit: 753de7d5c45062d5138be86ced7eacddd5696ca3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/20/2020
ms.locfileid: "94976825"
---
# <a name="query-azure-cli-command-output"></a><span data-ttu-id="25051-103">Consultar a saída do comando da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="25051-103">Query Azure CLI command output</span></span>

<span data-ttu-id="25051-104">A CLI do Azure usa o argumento `--query` para executar uma [consulta JMESPath](http://jmespath.org) nos resultados dos comandos.</span><span class="sxs-lookup"><span data-stu-id="25051-104">The Azure CLI uses the `--query` argument to execute a [JMESPath query](http://jmespath.org) on the results of commands.</span></span> <span data-ttu-id="25051-105">JMESPath é uma linguagem de consulta do JSON, permitindo que você selecione e modifique os dados na saída da CLI.</span><span class="sxs-lookup"><span data-stu-id="25051-105">JMESPath is a query language for JSON, giving you the ability to select and modify data from CLI output.</span></span> <span data-ttu-id="25051-106">As consultas são executadas na saída do JSON antes de qualquer formatação da exibição.</span><span class="sxs-lookup"><span data-stu-id="25051-106">Queries are executed on the JSON output before any display formatting.</span></span>

<span data-ttu-id="25051-107">O argumento `--query` tem suporte de todos os comandos na CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="25051-107">The `--query` argument is supported by all commands in the Azure CLI.</span></span> <span data-ttu-id="25051-108">Este artigo aborda como usar os recursos do JMESPath com uma série de exemplos pequenos e simples.</span><span class="sxs-lookup"><span data-stu-id="25051-108">This article covers how to use the features of JMESPath with a series of small, simple examples.</span></span>

> [!NOTE]
>
> <span data-ttu-id="25051-109">Durante o uso da CLI do Azure no PowerShell no Windows, pode ser necessário um escape extra para o argumento de consulta.</span><span class="sxs-lookup"><span data-stu-id="25051-109">When using Azure CLI in PowerShell on Windows, some extra escaping may be necessary for the query argument.</span></span> <span data-ttu-id="25051-110">Confira [Problemas com colocações de aspas no PowerShell](https://github.com/Azure/azure-cli/blob/dev/doc/quoting-issues-with-powershell.md) para obter mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="25051-110">Please see [Quoting issues with PowerShell](https://github.com/Azure/azure-cli/blob/dev/doc/quoting-issues-with-powershell.md) for more detail.</span></span>

## <a name="dictionary-and-list-cli-results"></a><span data-ttu-id="25051-111">Dicionário e lista dos resultados da CLI</span><span class="sxs-lookup"><span data-stu-id="25051-111">Dictionary and list CLI results</span></span>

<span data-ttu-id="25051-112">Mesmo ao usar um formato de saída diferente do JSON, os resultados do comando da CLI são tratados primeiro como JSON para consultas.</span><span class="sxs-lookup"><span data-stu-id="25051-112">Even when using an output format other than JSON, CLI command results are first treated as JSON for queries.</span></span> <span data-ttu-id="25051-113">Os resultados da CLI são uma matriz JSON ou um dicionário.</span><span class="sxs-lookup"><span data-stu-id="25051-113">CLI results are either a JSON array or dictionary.</span></span> <span data-ttu-id="25051-114">Matrizes são sequências de objetos que podem ser indexados, e dicionários são objetos não ordenados acessados com chaves.</span><span class="sxs-lookup"><span data-stu-id="25051-114">Arrays are sequences of objects that can be indexed, and dictionaries are unordered objects accessed with keys.</span></span> <span data-ttu-id="25051-115">Os comandos que _poderiam_ retornar mais de um objeto retornam uma matriz, e os comandos que _sempre_ retornam _apenas_ um objeto retornam um dicionário.</span><span class="sxs-lookup"><span data-stu-id="25051-115">Commands that _could_ return more than one object return an array, and commands that _always_ return _only_ a single object return a dictionary.</span></span>

## <a name="get-properties-in-a-dictionary"></a><span data-ttu-id="25051-116">Obter propriedades em um dicionário</span><span class="sxs-lookup"><span data-stu-id="25051-116">Get properties in a dictionary</span></span>

<span data-ttu-id="25051-117">Trabalhando com os resultados do dicionário, você pode acessar as propriedades no nível superior com apenas a chave.</span><span class="sxs-lookup"><span data-stu-id="25051-117">Working with dictionary results, you can access properties from the top level with just the key.</span></span> <span data-ttu-id="25051-118">O caractere `.` (__subexpressão__) é usado para acessar as propriedades dos dicionários aninhados.</span><span class="sxs-lookup"><span data-stu-id="25051-118">The `.` (__subexpression__) character is used to access properties of nested dictionaries.</span></span> <span data-ttu-id="25051-119">Antes de apresentar as consultas, examine a saída não modificada do comando `az vm show`:</span><span class="sxs-lookup"><span data-stu-id="25051-119">Before introducing queries, take a look at the unmodified output of the `az vm show` command:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM -o json
```

<span data-ttu-id="25051-120">O comando produzirá um dicionário.</span><span class="sxs-lookup"><span data-stu-id="25051-120">The command will output a dictionary.</span></span> <span data-ttu-id="25051-121">Parte do conteúdo foi omitida.</span><span class="sxs-lookup"><span data-stu-id="25051-121">Some content has been omitted.</span></span>

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

<span data-ttu-id="25051-122">O comando a seguir obtém as chaves SSH públicas autorizadas para conectar a VM adicionando uma consulta:</span><span class="sxs-lookup"><span data-stu-id="25051-122">The following command gets the SSH public keys authorized to connect to the VM by adding a query:</span></span>

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

## <a name="get-a-single-value"></a><span data-ttu-id="25051-123">Obter um valor único</span><span class="sxs-lookup"><span data-stu-id="25051-123">Get a single value</span></span>

<span data-ttu-id="25051-124">Um caso comum é precisar obter somente _um_ valor de um comando da CLI, como uma ID do recurso do Azure, um nome de recurso, um nome de usuário ou uma senha.</span><span class="sxs-lookup"><span data-stu-id="25051-124">A common case is that you need to only get _one_ value out of a CLI command, such as an Azure resource ID, a resource name, a username, or a password.</span></span> <span data-ttu-id="25051-125">Nesse caso, muitas vezes você também quer armazenar o valor em uma variável de ambiente local.</span><span class="sxs-lookup"><span data-stu-id="25051-125">In that case, you also often want to store the value in a local environment variable.</span></span> <span data-ttu-id="25051-126">Para obter uma propriedade única, primeiro, verifique se você está recebendo somente uma propriedade da consulta.</span><span class="sxs-lookup"><span data-stu-id="25051-126">To get a single property, first make sure that you're only getting one property out of the query.</span></span> <span data-ttu-id="25051-127">Ao modificar o último exemplo para obter somente o nome de usuário do administrador:</span><span class="sxs-lookup"><span data-stu-id="25051-127">Modifying the last example to get only the admin username:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'osProfile.adminUsername' -o json
```

```JSON
"azureuser"
```

<span data-ttu-id="25051-128">Parece um valor único válido, mas observe que os caracteres `"` são retornados como parte da saída.</span><span class="sxs-lookup"><span data-stu-id="25051-128">This looks like a valid single value, but note that the `"` characters are returned as part of the output.</span></span> <span data-ttu-id="25051-129">Isso indica que o objeto é uma cadeia de caracteres JSON.</span><span class="sxs-lookup"><span data-stu-id="25051-129">This indicates that the object is a JSON string.</span></span> <span data-ttu-id="25051-130">É importante observar que ao atribuir esse valor diretamente à variável de ambiente como saída do comando, as aspas podem __não__ ser interpretadas pelo shell:</span><span class="sxs-lookup"><span data-stu-id="25051-130">It's important to note that when you assign this value directly as output from the command to an environment variable, the quotes may __not__ be interpreted by the shell:</span></span>

```bash
USER=$(az vm show -g QueryDemo -n TestVM --query 'osProfile.adminUsername' -o json)
echo $USER
```

```output
"azureuser"
```

<span data-ttu-id="25051-131">Certamente, isso não é desejado.</span><span class="sxs-lookup"><span data-stu-id="25051-131">This is almost certainly not what you want.</span></span> <span data-ttu-id="25051-132">Nesse caso, você quer usar um formato de saída que não inclua os valores retornados com as informações de tipo.</span><span class="sxs-lookup"><span data-stu-id="25051-132">In this case, you want to use an output format which doesn't enclose returned values with type information.</span></span> <span data-ttu-id="25051-133">A melhor opção de saída oferecida pela CLI para este fim é `tsv`, valores separados por tabulações.</span><span class="sxs-lookup"><span data-stu-id="25051-133">The best output option that the CLI offers for this purpose is `tsv`, tab-separated values.</span></span> <span data-ttu-id="25051-134">Em especial, ao recuperar um valor que é somente um valor único (e não um dicionário ou uma lista), garante-se que a saída `tsv` não tenha aspas.</span><span class="sxs-lookup"><span data-stu-id="25051-134">In particular, when retrieving a value that's only a single value (not a dictionary or list), `tsv` output is guaranteed to be unquoted.</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'osProfile.adminUsername' -o tsv
```

```output
azureuser
```

<span data-ttu-id="25051-135">Para saber mais sobre o formato de saída `tsv`, confira [Formatos de saída – Formato de saída TSV](format-output-azure-cli.md#tsv-output-format)</span><span class="sxs-lookup"><span data-stu-id="25051-135">For more information about the `tsv` output format, see [Output formats - TSV output format](format-output-azure-cli.md#tsv-output-format)</span></span>

## <a name="get-multiple-values"></a><span data-ttu-id="25051-136">Obter vários valores</span><span class="sxs-lookup"><span data-stu-id="25051-136">Get multiple values</span></span>

<span data-ttu-id="25051-137">Para obter mais de uma propriedade, coloque as expressões entre colchetes `[ ]` (uma __lista de seleção múltipla__), como uma lista separada por vírgulas.</span><span class="sxs-lookup"><span data-stu-id="25051-137">To get more than one property, put expressions in square brackets  `[ ]` (a __multiselect list__) as a comma-separated list.</span></span> <span data-ttu-id="25051-138">Para obter o nome da VM, o usuário administrador e a chave SSH juntos, use o comando:</span><span class="sxs-lookup"><span data-stu-id="25051-138">To get the VM name, admin user, and SSH key all at once use the command:</span></span>

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

<span data-ttu-id="25051-139">Esses valores são listados na matriz de resultados na ordem em que foram fornecidos na consulta.</span><span class="sxs-lookup"><span data-stu-id="25051-139">These values are listed in the result array in the order they were given in the query.</span></span> <span data-ttu-id="25051-140">Como o resultado é uma matriz, não há nenhuma chave associada a ele.</span><span class="sxs-lookup"><span data-stu-id="25051-140">Since the result is an array, there are no keys associated with the results.</span></span>

## <a name="rename-properties-in-a-query"></a><span data-ttu-id="25051-141">Renomear as propriedades em uma consulta</span><span class="sxs-lookup"><span data-stu-id="25051-141">Rename properties in a query</span></span>

<span data-ttu-id="25051-142">Para obter um dicionário, em vez de uma matriz, ao consultar diversos valores, use o operador `{ }` (__hash de seleção múltipla__).</span><span class="sxs-lookup"><span data-stu-id="25051-142">To get a dictionary instead of an array when querying for multiple values, use the `{ }` (__multiselect hash__) operator.</span></span>
<span data-ttu-id="25051-143">O formato de um hash de seleção múltipla é `{displayName:JMESPathExpression, ...}`.</span><span class="sxs-lookup"><span data-stu-id="25051-143">The format for a multiselect hash is `{displayName:JMESPathExpression, ...}`.</span></span>
<span data-ttu-id="25051-144">`displayName` será a cadeia de caracteres mostrada na saída e `JMESPathExpression` é a expressão do JMESPath a avaliar.</span><span class="sxs-lookup"><span data-stu-id="25051-144">`displayName` will be the string shown in output, and `JMESPathExpression` is the JMESPath expression to evaluate.</span></span> <span data-ttu-id="25051-145">Modificando o exemplo da seção anterior alterando a lista de seleção múltipla para um hash:</span><span class="sxs-lookup"><span data-stu-id="25051-145">Modifying the example from the last section by changing the multiselect list to a hash:</span></span>

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

## <a name="get-properties-in-an-array"></a><span data-ttu-id="25051-146">Obter propriedades em uma matriz</span><span class="sxs-lookup"><span data-stu-id="25051-146">Get properties in an array</span></span>

<span data-ttu-id="25051-147">Uma matriz não tem nenhuma propriedade, mas pode ser indexada.</span><span class="sxs-lookup"><span data-stu-id="25051-147">An array has no properties of its own, but it can be indexed.</span></span> <span data-ttu-id="25051-148">Esse recurso é mostrado no último exemplo com a expressão `publicKeys[0]`, que obtém o primeiro elemento da matriz `publicKeys`.</span><span class="sxs-lookup"><span data-stu-id="25051-148">This feature is shown in the last example with the expression `publicKeys[0]`, which gets the first element of the `publicKeys` array.</span></span> <span data-ttu-id="25051-149">Não há nenhuma garantia de que a CLI de saída será ordenada, portanto, evite usar a indexação, a menos que tenha certeza da ordem ou não se importe com o elemento obtido.</span><span class="sxs-lookup"><span data-stu-id="25051-149">There's no guarantee CLI output is ordered, so avoid using indexing unless you're sure of the order or don't care what element you get.</span></span> <span data-ttu-id="25051-150">Para acessar as propriedades dos elementos em uma matriz, execute uma das duas operações: _nivelamento_ e _filtragem_.</span><span class="sxs-lookup"><span data-stu-id="25051-150">To access the properties of elements in an array, you do one of two operations: _flattening_ and _filtering_.</span></span> <span data-ttu-id="25051-151">Esta seção aborda como nivelar uma matriz.</span><span class="sxs-lookup"><span data-stu-id="25051-151">This section covers how to flatten an array.</span></span>

<span data-ttu-id="25051-152">O nivelamento de uma matriz é feito com o operador `[]` do JMESPath.</span><span class="sxs-lookup"><span data-stu-id="25051-152">Flattening an array is done with the `[]` JMESPath operator.</span></span> <span data-ttu-id="25051-153">Todas as expressões após o operador `[]` são aplicadas em cada elemento na matriz atual.</span><span class="sxs-lookup"><span data-stu-id="25051-153">All expressions after the `[]` operator are applied to each element in the current array.</span></span>
<span data-ttu-id="25051-154">Se `[]` aparecer no início da consulta, ele nivelará o resultado do comando da CLI.</span><span class="sxs-lookup"><span data-stu-id="25051-154">If `[]` appears at the start of the query, it flattens the CLI command result.</span></span> <span data-ttu-id="25051-155">Os resultados de `az vm list` podem ser examinados com esse recurso.</span><span class="sxs-lookup"><span data-stu-id="25051-155">The results of `az vm list` can be inspected with this feature.</span></span>
<span data-ttu-id="25051-156">Para obter o nome, o SO e o nome do administrador de cada VM em um grupo de recursos:</span><span class="sxs-lookup"><span data-stu-id="25051-156">To get the name, OS, and administrator name for each VM in a resource group:</span></span>

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

<span data-ttu-id="25051-157">Quando combinados com o formato de saída `--output table`, os nomes de colunas correspondem ao valor `displayKey` do hash de seleção múltipla:</span><span class="sxs-lookup"><span data-stu-id="25051-157">When combined with the `--output table` output format, the column names match up with the `displayKey` value of the multiselect hash:</span></span>

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
> <span data-ttu-id="25051-158">Algumas chaves são filtradas e não são impressas na exibição da tabela.</span><span class="sxs-lookup"><span data-stu-id="25051-158">Certain keys are filtered out and not printed in the table view.</span></span> <span data-ttu-id="25051-159">Essas chaves são `id`, `type` e `etag`.</span><span class="sxs-lookup"><span data-stu-id="25051-159">These keys are `id`, `type`, and `etag`.</span></span> <span data-ttu-id="25051-160">Para ver esses valores, você pode alterar o nome da chave em um hash de seleção múltipla.</span><span class="sxs-lookup"><span data-stu-id="25051-160">To see these values, you can change the key name in a multiselect hash.</span></span>
>
> ```azurecli-interactive
> az vm show -g QueryDemo -n TestVM --query "{objectID:id}" -o table
> ```

<span data-ttu-id="25051-161">Qualquer matriz pode ser nivelada, não apenas o resultado de alto nível retornado pelo comando.</span><span class="sxs-lookup"><span data-stu-id="25051-161">Any array can be flattened, not just the top-level result returned by the command.</span></span> <span data-ttu-id="25051-162">Na última seção, a expressão `osProfile.linuxConfiguration.ssh.publicKeys[0].keyData` foi usada para obter a chave SSH pública para entrar.</span><span class="sxs-lookup"><span data-stu-id="25051-162">In the last section, the expression `osProfile.linuxConfiguration.ssh.publicKeys[0].keyData` was used to get the SSH public key for sign-in.</span></span> <span data-ttu-id="25051-163">Para obter _cada_ chave SSH pública, a expressão pode ser escrita como `osProfile.linuxConfiguration.ssh.publicKeys[].keyData`.</span><span class="sxs-lookup"><span data-stu-id="25051-163">To get _every_ SSH public key, the expression could instead be written as `osProfile.linuxConfiguration.ssh.publicKeys[].keyData`.</span></span>
<span data-ttu-id="25051-164">Esta expressão de consulta nivela a matriz `osProfile.linuxConfiguration.ssh.publicKeys` e executa a expressão `keyData` em cada elemento:</span><span class="sxs-lookup"><span data-stu-id="25051-164">This query expression flattens the `osProfile.linuxConfiguration.ssh.publicKeys` array, and then runs the `keyData` expression on each element:</span></span>

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

## <a name="filter-arrays"></a><span data-ttu-id="25051-165">Filtrar matrizes</span><span class="sxs-lookup"><span data-stu-id="25051-165">Filter arrays</span></span>

<span data-ttu-id="25051-166">A outra operação usada para obter dados de uma matriz é a _filtragem_.</span><span class="sxs-lookup"><span data-stu-id="25051-166">The other operation used to get data from an array is _filtering_.</span></span> <span data-ttu-id="25051-167">A filtragem é feita com o operador `[?...]` do JMESPath.</span><span class="sxs-lookup"><span data-stu-id="25051-167">Filtering is done with the `[?...]` JMESPath operator.</span></span>
<span data-ttu-id="25051-168">Esse operador usa um predicado como conteúdo.</span><span class="sxs-lookup"><span data-stu-id="25051-168">This operator takes a predicate as its contents.</span></span> <span data-ttu-id="25051-169">Um predicado é qualquer instrução que pode ser avaliada como `true` ou `false`.</span><span class="sxs-lookup"><span data-stu-id="25051-169">A predicate is any statement that can be evaluated to either `true` or `false`.</span></span> <span data-ttu-id="25051-170">As expressões em que o predicado é avaliado como `true` são incluídas na saída.</span><span class="sxs-lookup"><span data-stu-id="25051-170">Expressions where the predicate evaluates to `true` are included in the output.</span></span>

<span data-ttu-id="25051-171">JMESPath oferece a comparação padrão e os operadores lógicos.</span><span class="sxs-lookup"><span data-stu-id="25051-171">JMESPath offers the standard comparison and logical operators.</span></span> <span data-ttu-id="25051-172">Eles incluem `<`, `<=`, `>`, `>=`, `==` e `!=`.</span><span class="sxs-lookup"><span data-stu-id="25051-172">These include `<`, `<=`, `>`, `>=`, `==`, and `!=`.</span></span>
<span data-ttu-id="25051-173">JMESPath também dá suporte às operações lógicas e (`&&`) ou (`||`), e não (`!`).</span><span class="sxs-lookup"><span data-stu-id="25051-173">JMESPath also supports logical and (`&&`), or (`||`), and not (`!`).</span></span> <span data-ttu-id="25051-174">Expressões podem ser agrupadas entre parênteses, permitindo expressões de predicado mais complexas.</span><span class="sxs-lookup"><span data-stu-id="25051-174">Expressions can be grouped within parenthesis, allowing for more complex predicate expressions.</span></span> <span data-ttu-id="25051-175">Para obter mais detalhes sobre predicados e operações lógicas, confira a [especificação do JMESPath](http://jmespath.org/specification.html).</span><span class="sxs-lookup"><span data-stu-id="25051-175">For the full details on predicates and logical operations, see the [JMESPath specification](http://jmespath.org/specification.html).</span></span>

<span data-ttu-id="25051-176">Na última seção, nivelamos uma matriz para obter a lista completa de todas as VMs em um grupo de recursos.</span><span class="sxs-lookup"><span data-stu-id="25051-176">In the last section, we flattened an array to get the complete list of all VMs in a resource group.</span></span> <span data-ttu-id="25051-177">Usando filtros, essa saída pode ser restrita apenas às VMs do Linux:</span><span class="sxs-lookup"><span data-stu-id="25051-177">Using filters, this output can be restricted to only Linux VMs:</span></span>

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
> <span data-ttu-id="25051-178">No JMESPath, as cadeias de caracteres sempre ficam entre aspas simples (`'`).</span><span class="sxs-lookup"><span data-stu-id="25051-178">In JMESPath, strings are always surrounded by single quotes (`'`).</span></span> <span data-ttu-id="25051-179">Se você usar aspas duplas como parte de uma cadeia de caracteres em um predicado de filtro, obterá uma saída vazia.</span><span class="sxs-lookup"><span data-stu-id="25051-179">If you use double quotes as part of a string in a filter predicate, you'll get empty output.</span></span>

<span data-ttu-id="25051-180">O JMESPath também tem funções internas que podem ajudar na filtragem.</span><span class="sxs-lookup"><span data-stu-id="25051-180">JMESPath also has built-in functions that can help with filtering.</span></span> <span data-ttu-id="25051-181">Uma dessas funções é `contains(string, substring)`, que verifica se uma cadeia de caracteres contém uma subcadeia.</span><span class="sxs-lookup"><span data-stu-id="25051-181">One such function is `contains(string, substring)`, which checks to see if a string contains a substring.</span></span> <span data-ttu-id="25051-182">As expressões são avaliadas antes de chamar a função, portanto, o primeiro argumento pode ser uma expressão completa do JMESPath.</span><span class="sxs-lookup"><span data-stu-id="25051-182">Expressions are evaluated before calling the function, so the first argument can be a full JMESPath expression.</span></span> <span data-ttu-id="25051-183">O exemplo a seguir localiza todas as VMs usando o armazenamento SSD para seu disco do SO:</span><span class="sxs-lookup"><span data-stu-id="25051-183">The next example finds all VMs using SSD storage for their OS disk:</span></span>

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

<span data-ttu-id="25051-184">Essa consulta é um pouco longa.</span><span class="sxs-lookup"><span data-stu-id="25051-184">This query is a little long.</span></span> <span data-ttu-id="25051-185">A chave `storageProfile.osDisk.managedDisk.storageAccountType` é mencionada duas vezes e rechaveada na saída.</span><span class="sxs-lookup"><span data-stu-id="25051-185">The `storageProfile.osDisk.managedDisk.storageAccountType` key is mentioned twice, and rekeyed in the output.</span></span> <span data-ttu-id="25051-186">Uma maneira de reduzi-la é aplicar o filtro depois de nivelar e selecionar os dados.</span><span class="sxs-lookup"><span data-stu-id="25051-186">One way to shorten it is to apply the filter after flattening and selecting data.</span></span>

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

<span data-ttu-id="25051-187">Para matrizes grandes, pode ser mais rápido aplicar o filtro antes de selecionar os dados.</span><span class="sxs-lookup"><span data-stu-id="25051-187">For large arrays, it may be faster to apply the filter before selecting data.</span></span>

<span data-ttu-id="25051-188">Confira a [Especificação do JMESPath - Funções Internas](http://jmespath.org/specification.html#built-in-functions) para obter a lista completa de funções.</span><span class="sxs-lookup"><span data-stu-id="25051-188">See the [JMESPath specification - Built-in Functions](http://jmespath.org/specification.html#built-in-functions) for the full list of functions.</span></span>

## <a name="change-output"></a><span data-ttu-id="25051-189">Alterar a saída</span><span class="sxs-lookup"><span data-stu-id="25051-189">Change output</span></span>

<span data-ttu-id="25051-190">As funções do JMESPath também têm outra finalidade, que é operar nos resultados de uma consulta.</span><span class="sxs-lookup"><span data-stu-id="25051-190">JMESPath functions also have another purpose, which is to operate on the results of a query.</span></span> <span data-ttu-id="25051-191">Qualquer função que retorna um valor não booliano altera o resultado de uma expressão.</span><span class="sxs-lookup"><span data-stu-id="25051-191">Any function that returns a non-boolean value changes the result of an expression.</span></span>
<span data-ttu-id="25051-192">Por exemplo, você pode classificar os dados por um valor de propriedade com `sort_by(array, &sort_expression)`.</span><span class="sxs-lookup"><span data-stu-id="25051-192">For example, you can sort data by a property value with `sort_by(array, &sort_expression)`.</span></span> <span data-ttu-id="25051-193">O JMESPath usa um operador especial, `&`, para as expressões que devem ser avaliadas posteriormente como parte de uma função.</span><span class="sxs-lookup"><span data-stu-id="25051-193">JMESPath uses a special operator, `&`, for expressions that should be evaluated later as part of a function.</span></span> <span data-ttu-id="25051-194">O exemplo a seguir mostra como classificar uma lista de VMs pelo tamanho de disco do SO:</span><span class="sxs-lookup"><span data-stu-id="25051-194">The next example shows how to sort a VM list by OS disk size:</span></span>

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

<span data-ttu-id="25051-195">Confira a [Especificação do JMESPath - Funções Internas](http://jmespath.org/specification.html#built-in-functions) para obter a lista completa de funções.</span><span class="sxs-lookup"><span data-stu-id="25051-195">See the [JMESPath specification - Built-in Functions](http://jmespath.org/specification.html#built-in-functions) for the full list of functions.</span></span>

## <a name="experiment-with-queries-interactively"></a><span data-ttu-id="25051-196">Experimentar consultas interativamente</span><span class="sxs-lookup"><span data-stu-id="25051-196">Experiment with queries interactively</span></span>

<span data-ttu-id="25051-197">Para começar a experimentar o JMESPath, o pacote [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) do Python oferece um ambiente interativo para trabalhar com as consultas.</span><span class="sxs-lookup"><span data-stu-id="25051-197">To start experimenting with JMESPath, the [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) Python package offers an interactive environment to work with queries.</span></span> <span data-ttu-id="25051-198">Os dados são transferidos como entrada e as consultas são gravadas e executadas no editor.</span><span class="sxs-lookup"><span data-stu-id="25051-198">Data is piped as input, and then queries are written and run in the editor.</span></span>

```bash
pip install jmespath-terminal
az vm list --output json | jpterm
```
