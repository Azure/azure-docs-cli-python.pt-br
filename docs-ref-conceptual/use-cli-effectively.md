---
ms.openlocfilehash: 4794f1eb2fb45ca767f67de5270e232d6b68aede
ms.sourcegitcommit: 58d839589858acc1a7a9f114af7f4fce13d883ea
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "88601892"
---
# <a name="tips-for-using-azure-cli-effectively"></a><span data-ttu-id="ef2f4-101">Dicas para usar a CLI do Azure com eficácia</span><span class="sxs-lookup"><span data-stu-id="ef2f4-101">Tips for using Azure CLI effectively</span></span>

<span data-ttu-id="ef2f4-102">Para maior clareza, os scripts Bash são embutidos.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-102">For clarity, Bash scripts are used inline.</span></span> <span data-ttu-id="ef2f4-103">Os exemplos do PowerShell ou do lote do Windows são listados no apêndice, que pode ser usado para criar exemplos semelhantes.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-103">Windows batch or PowerShell examples are listed in the appendix, which you can use to build similar examples.</span></span>

## <a name="output-formatting-json-table-or-tsv"></a><span data-ttu-id="ef2f4-104">Formatação de saída (JSON, tabela ou TSV)</span><span class="sxs-lookup"><span data-stu-id="ef2f4-104">Output formatting (json, table, or tsv)</span></span>

1. <span data-ttu-id="ef2f4-105">O formato `json` é o padrão da CLI e destina-se a fornecer as informações mais abrangentes.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-105">`json` format is the CLI's default, and is intended to give you the most comprehensive information.</span></span> <span data-ttu-id="ef2f4-106">Se você preferir um formato diferente, use o argumento `--output` para substituir uma invocação de comando individual ou use `az configure` para atualizar o seu padrão global.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-106">If you prefer a different format, use the `--output` argument to override for an individual command invocation, or use `az configure` to update your global default.</span></span> <span data-ttu-id="ef2f4-107">Observe que o formato JSON preserva as aspas duplas, geralmente tornando-as inadequadas para fins de script.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-107">Note that JSON format preserves the double quotes, generally making in unsuitable for scripting purposes.</span></span>

2. <span data-ttu-id="ef2f4-108">O `table` é útil para obter um resumo das informações centralizadas, especialmente para comandos de lista.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-108">`table` is useful for getting a summary of focused information, particularly for list commands.</span></span> <span data-ttu-id="ef2f4-109">Se você não gostar dos campos no formato de tabela padrão (ou não houver um formato padrão), poderá usar `--output json` para ver todas as informações ou usar o `--query` para especificar o formato que deseja.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-109">If you do not like the fields in the default table format (or there isn't a default format), you can use `--output json` to see all information, or leverage `--query` to specify a format you like.</span></span>

    ```sh
    az vm show -g my_rg -n my_vm --query "{name: name, os:storageProfile.imageReference.offer}" -otable
    Name    Os
    ------  ------------
    my_vm   UbuntuServer
    ```

3. <span data-ttu-id="ef2f4-110">`tsv` é útil para fins de script e de saída concisos.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-110">`tsv` is useful for concise output and scripting purposes.</span></span> <span data-ttu-id="ef2f4-111">O TSV removerá aspas duplas que o formato JSON preserva.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-111">The tsv will strip double quotes that the JSON format preserves.</span></span> <span data-ttu-id="ef2f4-112">Para especificar o formato desejado para o TSV, use o argumento `--query`.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-112">To specify the format you want for TSV, use the `--query` argument.</span></span>

    ```sh
    export vm_ids=$(az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv)
    az vm stop --ids $vm_ids
    ```

## <a name="pass-values-from-one-command-to-another"></a><span data-ttu-id="ef2f4-113">Passar valores de um comando para o outro</span><span class="sxs-lookup"><span data-stu-id="ef2f4-113">Pass values from one command to another</span></span>

1. <span data-ttu-id="ef2f4-114">Se o valor for usado mais de uma vez, atribua-o a uma variável.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-114">If the value will be used more than once, assign it to a variable.</span></span> <span data-ttu-id="ef2f4-115">Observe o uso de `-o tsv` no seguinte exemplo:</span><span class="sxs-lookup"><span data-stu-id="ef2f4-115">Note the use of `-o tsv` in the following example:</span></span>

    ```sh
    running_vm_ids=$(az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv)
    ```
2. <span data-ttu-id="ef2f4-116">Se o valor for usado apenas uma vez, considere usar pipe:</span><span class="sxs-lookup"><span data-stu-id="ef2f4-116">If the value is used only once, consider piping:</span></span>
    ```sh
    az vm list --query "[?powerState=='VM running'].name" | grep my_vm
    ```
3. <span data-ttu-id="ef2f4-117">Para listas, considere as seguintes sugestões:</span><span class="sxs-lookup"><span data-stu-id="ef2f4-117">For lists consider the following suggestions:</span></span>

   <span data-ttu-id="ef2f4-118">Se você precisar de mais controles no resultado, use o loop "for":</span><span class="sxs-lookup"><span data-stu-id="ef2f4-118">If you need more controls on the result, use "for" loop:</span></span>
    ```sh
    #!/usr/bin/env bash
    for vm in $(az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv); do
        echo stopping $vm
        az vm stop --ids $vm
        if [ $? -ne 0 ]; then
            echo "Failed to stop $vm"
            exit 1
        fi
        echo $vm stopped
    done
    ```

    <span data-ttu-id="ef2f4-119">Como alternativa, use `xargs` e considere usar o sinalizador `-P` para executar as operações em paralelo para melhor desempenho:</span><span class="sxs-lookup"><span data-stu-id="ef2f4-119">Alternatively, use `xargs` and consider using the `-P` flag to run the operations in parallel for improved performance:</span></span>
    ```sh
    az vm list -d -g my_rg --query "[?powerState=='VM stopped'].id" -o tsv | xargs -I {} -P 10 az vm start --ids "{}"
    ```
    <span data-ttu-id="ef2f4-120">Por fim, a CLI do Azure tem suporte interno para processar comandos com vários `--ids` em paralelo de modo a obter o mesmo efeito de xargs.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-120">Finally, Azure CLI has built-in support to process commands with multiple `--ids` in parallel to achieve the same effect of xargs.</span></span> <span data-ttu-id="ef2f4-121">Observe que `@-` é usado para obter valores do pipe:</span><span class="sxs-lookup"><span data-stu-id="ef2f4-121">Note that `@-` is used to get values from the pipe:</span></span>
    ```sh
    az vm list -d -g my_rg --query "[?powerState=='VM stopped'].id" -o tsv | az vm start --ids @-
    ```

## <a name="async-operations"></a><span data-ttu-id="ef2f4-122">Operações assíncronas</span><span class="sxs-lookup"><span data-stu-id="ef2f4-122">Async operations</span></span>

<span data-ttu-id="ef2f4-123">Muitos comandos e grupos expõem sinalizadores `--no-wait` nas suas operações de execução prolongada, além de um comando `wait` dedicado.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-123">Many commands and group expose `--no-wait` flags on their long-running operations as well as a dedicated `wait` command.</span></span> <span data-ttu-id="ef2f4-124">Eles se tornam úteis para determinados cenários:</span><span class="sxs-lookup"><span data-stu-id="ef2f4-124">These become handy for certain scenarios:</span></span>

1. <span data-ttu-id="ef2f4-125">Limpar recursos quando você não depende da limpeza para uma operação subsequente, como excluir um grupo de recursos:</span><span class="sxs-lookup"><span data-stu-id="ef2f4-125">Cleaning up resources when you aren't relying on the clean up for some subsequent operation, such as deleting a resource group:</span></span>
    ```sh
    az group delete -n my_rg --no-wait
    ```
2. <span data-ttu-id="ef2f4-126">Quando você quiser criar vários recursos independentes em paralelo.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-126">When you want to create multiple independent resources in parallel.</span></span> <span data-ttu-id="ef2f4-127">Isso é semelhante a criar e unir threads:</span><span class="sxs-lookup"><span data-stu-id="ef2f4-127">This is similar to creating and joining threads:</span></span>

    ```sh
    az vm create -g my_rg -n vm1 --image centos --no-wait
    az vm create -g my_rg -n vm2 --image centos --no-wait

    subscription=$(az account show --query "id" -otsv)
    vm1_id="/subscriptions/$subscription/resourceGroups/my_rg/providers/Microsoft.Compute/virtualMachines/vm1"
    vm2_id="/subscriptions/$subscription/resourceGroups/my_rg/providers/Microsoft.Compute/virtualMachines/vm2"
    az vm wait --created --ids $vm1_id $vm2_id
    ```

## <a name="generic-update-arguments"></a><span data-ttu-id="ef2f4-128">Argumentos de atualização genéricos</span><span class="sxs-lookup"><span data-stu-id="ef2f4-128">Generic update arguments</span></span>

<span data-ttu-id="ef2f4-129">A maioria dos comandos de atualização no recurso de CLI têm os três argumentos genéricos: `--add`, `--set` e `--remove`.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-129">Most update commands in the CLI feature the three generic arguments: `--add`, `--set` and `--remove`.</span></span> <span data-ttu-id="ef2f4-130">Esses argumentos são poderosos, mas geralmente menos convenientes do que os argumentos fortemente tipados normalmente presentes em comandos de atualização.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-130">These arguments are powerful but often less convenient than the strongly-typed arguments typically featured in update commands.</span></span> <span data-ttu-id="ef2f4-131">A CLI fornece argumentos fortemente tipados nos cenários mais comuns para facilitar o uso, mas se a propriedade que você deseja definir não estiver listada, os argumentos de atualização genérica geralmente apresentarão um caminho de desbloqueio sem a necessidade de aguardar uma nova versão.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-131">The CLI provides strongly-typed arguments for most common scenarios for ease-of-use, but if the property you want to set isn't listed, the generic update arguments will often present a path forward to unblock you without having to wait for a new release.</span></span>

1. <span data-ttu-id="ef2f4-132">A sintaxe de atualização genérica não é muito amigável, portanto, ela exigirá paciência.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-132">The generic update syntax isn't the most user friendly, so it will require some patience.</span></span>
2. <span data-ttu-id="ef2f4-133">Verifique se o grupo `Generic Update Arguments` está exposto no comando de atualização.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-133">Verify whether the update command has the `Generic Update Arguments` group exposed.</span></span> <span data-ttu-id="ef2f4-134">Se não estiver, você precisará reportar um problema, mas se estiver, você poderá tentar o cenário usando-o.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-134">If not, you'll need to file an issue, but if they are you can attempt you scenario using them.</span></span>
3. <span data-ttu-id="ef2f4-135">Use o comando `show` no recurso que você está interessado para descobrir qual caminho você deve fornecer nos argumentos genéricos.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-135">Use the `show` command on the resource you are interested in to figure out what path you should supply in the generic arguments.</span></span> <span data-ttu-id="ef2f4-136">Por exemplo, antes de experimentar `az vm update`, execute `az vm show` para determinar o caminho correto.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-136">For example, before you try out `az vm update`, run `az vm show` to determine the right path.</span></span> <span data-ttu-id="ef2f4-137">De modo geral, você usará a sintaxe Dot para acessar as propriedades do dicionário e os colchetes para indexar em listas.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-137">Generally, you will use dot syntax to access dictionary properties and brackets to index into lists.</span></span>
4. <span data-ttu-id="ef2f4-138">Confira os exemplos de trabalho para começar.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-138">Check out working examples to get started.</span></span> <span data-ttu-id="ef2f4-139">`az vm update -h` tem bons exemplos.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-139">`az vm update -h` has good ones.</span></span>
5. <span data-ttu-id="ef2f4-140">`--set` e `--add` obtêm uma lista de pares chave-valor no formato de `<key1>=<value1> <key2>=<value2>`.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-140">`--set` and `--add` take a list of key value pairs in the format of `<key1>=<value1> <key2>=<value2>`.</span></span> <span data-ttu-id="ef2f4-141">Use-os para construir conteúdos não triviais.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-141">Use them to construct non- trivial payloads.</span></span> <span data-ttu-id="ef2f4-142">Se a sintaxe receber mensagens demais, considere usar uma cadeia de caracteres JSON.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-142">If the syntax gets too message, consider using a JSON string.</span></span> <span data-ttu-id="ef2f4-143">Por exemplo, para anexar um novo disco de dados a uma VM:</span><span class="sxs-lookup"><span data-stu-id="ef2f4-143">For example, to attach a new data disk to a VM:</span></span>
    ```sh
    az vm update -g my_rg -n my_vm --add storageProfile.dataDisks "{\"createOption\": \"Attach\", \"managedDisk\": {\"id\": \"/subscriptions/0b1f6471-1bf0-4dda-aec3-cb9272f09590/resourceGroups/yg/providers/Microsoft.Compute/disks/yg-disk\"}, \"lun\": 1}"
    ```
6. <span data-ttu-id="ef2f4-144">Talvez você ache mais útil use a convenção de `@{file}` da CLI, colocar o JSON em um arquivo e carregá-lo.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-144">You may find it more useful to leverage the CLI's `@{file}` convention, putting the JSON into a file and loading it.</span></span> <span data-ttu-id="ef2f4-145">Isso simplifica o comando acima para:</span><span class="sxs-lookup"><span data-stu-id="ef2f4-145">This simplifies the above command to:</span></span>
    ```sh
    az vm update -g my_rg -n my_vm --add storageProfile.dataDisks @~/my_disk.json
    ```

## <a name="generic-resource-commands---az-resource"></a><span data-ttu-id="ef2f4-146">Comandos de recurso genéricos – `az resource`</span><span class="sxs-lookup"><span data-stu-id="ef2f4-146">Generic resource commands - `az resource`</span></span>

<span data-ttu-id="ef2f4-147">Pode haver casos em que um serviço no qual você está interessado não tenha cobertura de comando da CLI.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-147">There may be cases where a service you are interested in does not have CLI command coverage.</span></span> <span data-ttu-id="ef2f4-148">Você pode usar os comandos `az resource create/show/list/delete/update/invoke-action` para trabalhar com esses recursos.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-148">You can use the `az resource create/show/list/delete/update/invoke-action` commands to work with these resources.</span></span> <span data-ttu-id="ef2f4-149">Veja algumas sugestões:</span><span class="sxs-lookup"><span data-stu-id="ef2f4-149">Here are a few suggestions:</span></span>
1. <span data-ttu-id="ef2f4-150">Se apenas `create/update` estiverem envolvidos, considere usar `az group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-150">If only `create/update` are involved, consider using `az group deployment create`.</span></span> <span data-ttu-id="ef2f4-151">Use os [Modelos de Início Rápido do Azure](https://github.com/Azure/azure-quickstart-templates) para obter exemplos de trabalho.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-151">Leverage [Azure Quickstart Templates](https://github.com/Azure/azure-quickstart-templates) for working examples.</span></span>
2. <span data-ttu-id="ef2f4-152">Confira a referência da API REST para obter o conteúdo de solicitação, a URL e a versão da API.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-152">Check out the Rest API reference for the request payload, URL and API version.</span></span> <span data-ttu-id="ef2f4-153">Como um exemplo, confira os comentários da comunidade em [como criar o AppInsights](https://github.com/Azure/azure-cli/issues/5543).</span><span class="sxs-lookup"><span data-stu-id="ef2f4-153">As an example, check out the community's comments on [how to create AppInsights](https://github.com/Azure/azure-cli/issues/5543).</span></span>

## <a name="rest-api-command---az-rest"></a><span data-ttu-id="ef2f4-154">Comando da API REST – `az rest`</span><span class="sxs-lookup"><span data-stu-id="ef2f4-154">REST API command - `az rest`</span></span>

<span data-ttu-id="ef2f4-155">Se nenhum argumento de atualização genérico nem `az resource` atender às suas necessidades, você poderá usar o comando `az rest` para chamar a API REST.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-155">If neither generic update arguments nor `az resource` meets your needs, you can use `az rest` command to call the REST API.</span></span> <span data-ttu-id="ef2f4-156">Ele é autenticado automaticamente usando a credencial conectada e define o cabeçalho `Content-Type: application/json`.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-156">It automatically authenticates using the logged-in credential and sets header `Content-Type: application/json`.</span></span>

<span data-ttu-id="ef2f4-157">Isso é extremamente útil para chamar a [API do Microsoft Graph](/graph/api/overview?toc=./ref/toc.json&view=graph-rest-1.0), o que não tem suporte atualmente nos comandos da CLI ([#12946](https://github.com/Azure/azure-cli/issues/12946)).</span><span class="sxs-lookup"><span data-stu-id="ef2f4-157">This is extremely useful for calling [Microsoft Graph API](/graph/api/overview?toc=./ref/toc.json&view=graph-rest-1.0) which is not currently supported by CLI commands ([#12946](https://github.com/Azure/azure-cli/issues/12946)).</span></span>

<span data-ttu-id="ef2f4-158">Por exemplo, para atualizar `redirectUris` para um [Aplicativo](/graph/api/resources/application?view=graph-rest-1.0), chamamos a API REST [Aplicativo de atualização](/graph/api/application-update?view=graph-rest-1.0&tabs=http) com:</span><span class="sxs-lookup"><span data-stu-id="ef2f4-158">For example, to update `redirectUris` for an [Application](/graph/api/resources/application?view=graph-rest-1.0), we call the [Update application](/graph/api/application-update?view=graph-rest-1.0&tabs=http) REST API with:</span></span>

```sh
# Line breaks for legibility only

# Get the application
az rest --method GET
        --url 'https://graph.microsoft.com/v1.0/applications/b4e4d2ab-e2cb-45d5-a31a-98eb3f364001'

# Update `redirectUris` for `web` property
az rest --method PATCH
        --url 'https://graph.microsoft.com/v1.0/applications/b4e4d2ab-e2cb-45d5-a31a-98eb3f364001'
        --body '{"web":{"redirectUris":["https://myapp.com"]}}'
```

<span data-ttu-id="ef2f4-159">Ao usar `--url-parameters` para solicitações no formato de OData, use o caractere de escape `$` em ambientes diferentes. No `Bash`, use o caractere escape `$` como `\$`; e no `PowerShell`, use-o em `$` como `` `$``</span><span class="sxs-lookup"><span data-stu-id="ef2f4-159">When using `--url-parameters` for requests in the form of OData, please make sure to escape `$` in different environments: in `Bash`, escape `$` as `\$` and in `PowerShell`, escape `$` as `` `$``</span></span>

## <a name="quoting-issues"></a><span data-ttu-id="ef2f4-160">Problemas com colocações de aspas</span><span class="sxs-lookup"><span data-stu-id="ef2f4-160">Quoting issues</span></span>

<span data-ttu-id="ef2f4-161">Isso é um problema porque quando o shell de comando (Bash, Zsh, Prompt de Comando do Windows, PowerShell etc.) analisa o comando da CLI, ele interpreta as aspas e os espaços.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-161">This becomes an issue because when the command shell (Bash, Zsh, Windows Command Prompt, PowerShell, etc) parses the CLI command, it will interpret the quotes and spaces.</span></span> <span data-ttu-id="ef2f4-162">Sempre consulte os documentos quando você não tiver certeza sobre o uso de um shell:</span><span class="sxs-lookup"><span data-stu-id="ef2f4-162">Always refer to the documents when you are uncertain about the usage of a shell:</span></span>

- <span data-ttu-id="ef2f4-163">Bash: [Colocação de aspas](https://www.gnu.org/software/bash/manual/html_node/Quoting.html)</span><span class="sxs-lookup"><span data-stu-id="ef2f4-163">Bash: [Quoting](https://www.gnu.org/software/bash/manual/html_node/Quoting.html)</span></span>
- <span data-ttu-id="ef2f4-164">PowerShell: [Sobre as regras de colocação de aspas](/powershell/module/microsoft.powershell.core/about/about_quoting_rules)</span><span class="sxs-lookup"><span data-stu-id="ef2f4-164">PowerShell: [About Quoting Rules](/powershell/module/microsoft.powershell.core/about/about_quoting_rules)</span></span>
    - <span data-ttu-id="ef2f4-165">Devido ao problema conhecido [#1995](https://github.com/PowerShell/PowerShell/issues/1995) do PowerShell, algumas regras extras de escape se aplicam.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-165">Due to a known issue [#1995](https://github.com/PowerShell/PowerShell/issues/1995) of PowerShell, some extra escaping rules apply.</span></span> <span data-ttu-id="ef2f4-166">Consulte [Problemas com colocações de aspas no PowerShell](https://github.com/Azure/azure-cli/blob/dev/doc/quoting-issues-with-powershell.md) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-166">See [Quoting issues with PowerShell](https://github.com/Azure/azure-cli/blob/dev/doc/quoting-issues-with-powershell.md) for more information.</span></span>
- <span data-ttu-id="ef2f4-167">Prompt de Comando do Windows: [Instruções: caracteres de escape, delimitadores e aspas na linha de comando do Windows](https://ss64.com/nt/syntax-esc.html)</span><span class="sxs-lookup"><span data-stu-id="ef2f4-167">Windows Command Prompt: [How-to: Escape Characters, Delimiters and Quotes at the Windows command line](https://ss64.com/nt/syntax-esc.html)</span></span>

<span data-ttu-id="ef2f4-168">Para evitar resultados inesperados, veja algumas sugestões:</span><span class="sxs-lookup"><span data-stu-id="ef2f4-168">To avoid unanticipated results, here are a few suggestions:</span></span>

1. <span data-ttu-id="ef2f4-169">Se o valor contiver espaço em branco, você precisará colocá-lo em aspas.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-169">If the value contains whitespace, you must wrap it in quotes.</span></span>
2. <span data-ttu-id="ef2f4-170">No Bash ou no Windows PowerShell, as aspas simples e duplas serão interpretadas, enquanto no Prompt de Comando do Windows, apenas aspas duplas serão manipuladas, o que significa que as aspas simples serão interpretadas como parte do valor.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-170">In bash or Windows PowerShell, both single and double quotes will be interpreted, while in Windows Command Prompt, only double quotes are handled which means single quotes will be interpreted as a part of the value.</span></span>
3. <span data-ttu-id="ef2f4-171">Se o comando é executado somente no Bash (ou Zsh), o uso de aspas simples tem a vantagem delimitar o conteúdo.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-171">If your command only runs on Bash (or Zsh), using single quotes has the benefit of preserving the content inside.</span></span> <span data-ttu-id="ef2f4-172">Isso pode ser muito útil ao fornecer JSON embutido.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-172">This can be very helpful when supplying inline JSON.</span></span> <span data-ttu-id="ef2f4-173">Por exemplo, isto funciona no Bash: `'{"foo": "bar"}'`</span><span class="sxs-lookup"><span data-stu-id="ef2f4-173">For example this works in bash: `'{"foo": "bar"}'`</span></span>
4. <span data-ttu-id="ef2f4-174">Se o comando for executado no Prompt de Comando do Windows, você precisará usar exclusivamente aspas duplas.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-174">If your command will run on Windows Command Prompt, you must use double quotes exclusively.</span></span> <span data-ttu-id="ef2f4-175">Se o valor contiver aspas duplas, você precisará usar o caractere de escape: `"i like to use \" a lot"`.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-175">If the value contains double quotes, you must escape it: `"i like to use \" a lot"`.</span></span> <span data-ttu-id="ef2f4-176">O equivalente do Prompt de Comando do exemplo acima seria: `"{\"foo\": \"bar\"}"`</span><span class="sxs-lookup"><span data-stu-id="ef2f4-176">The Command Prompt equivalent of the above would be: `"{\"foo\": \"bar\"}"`</span></span>
5. <span data-ttu-id="ef2f4-177">Variáveis exportadas no Bash dentro de aspas duplas serão avaliadas.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-177">Exported variables in bash inside double quotes will be evaluated.</span></span> <span data-ttu-id="ef2f4-178">Se isso não for o que você deseja, use novamente `\ ` para colocar o caractere de escape `"\$var"` ou use aspas simples `'$var'`.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-178">If this is not what you want, again use `\ ` to escape it like `"\$var"` or use single quotes `'$var'`.</span></span>
6. <span data-ttu-id="ef2f4-179">Alguns argumentos de CLI, incluindo os argumentos de atualização genéricos, tem uma lista de valores separados por espaços, como `<key1>=<value1> <key2>=<value2>`.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-179">A few CLI arguments, including the generic update arguments, take a list of space-separated values, like `<key1>=<value1> <key2>=<value2>`.</span></span> <span data-ttu-id="ef2f4-180">Como o valor e o nome da chave podem usar uma cadeia de caracteres arbitrária que pode conter espaços em branco, será necessário usar aspas.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-180">Since the key name and value can take arbitrary string which might contain whitespace, using quotes will be necessary.</span></span> <span data-ttu-id="ef2f4-181">Encapsule o par, não a chave ou o valor individual.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-181">Wrap the pair, not individual key or value.</span></span> <span data-ttu-id="ef2f4-182">Portanto, `"my name"=john` está errado.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-182">So `"my name"=john` is wrong.</span></span> <span data-ttu-id="ef2f4-183">Em vez disso, use `"my name=john"`.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-183">Instead, use `"my name=john"`.</span></span> <span data-ttu-id="ef2f4-184">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="ef2f4-184">For example:</span></span>
    ```sh
    az webapp config appsettings set -g my_rg -n my_web --settings "client id=id1" "my name=john"
    ```
7. <span data-ttu-id="ef2f4-185">Use a convenção de `@<file>` da CLI para carregar de um arquivo de modo a ignorar os mecanismos de interpretação do shell:</span><span class="sxs-lookup"><span data-stu-id="ef2f4-185">Use CLI's `@<file>` convention to load from a file so to bypass the shell's interpretation mechanisms:</span></span>
    ```sh
    az ad app create --display-name my-native --native-app --required-resource-accesses @manifest.json
    ```
8. <span data-ttu-id="ef2f4-186">Quando um argumento da CLI aceita uma lista separada por espaços, estes são os formatos aceitos:</span><span class="sxs-lookup"><span data-stu-id="ef2f4-186">When a CLI argument says it accepts a space-separated list, these are the formats accepted:</span></span>
    - <span data-ttu-id="ef2f4-187">`--arg foo bar`: OK.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-187">`--arg foo bar`: OK.</span></span> <span data-ttu-id="ef2f4-188">Lista separada por espaços sem aspas</span><span class="sxs-lookup"><span data-stu-id="ef2f4-188">Unquoted, space-separated list</span></span>
    - <span data-ttu-id="ef2f4-189">`--arg "foo" "bar"`: OK: Lista separada por espaços com aspas</span><span class="sxs-lookup"><span data-stu-id="ef2f4-189">`--arg "foo" "bar"`: OK: Quoted, space-separated list</span></span>
    - <span data-ttu-id="ef2f4-190">`--arg "foo bar"`: INVÁLIDO.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-190">`--arg "foo bar"`: BAD.</span></span> <span data-ttu-id="ef2f4-191">Essa é uma cadeia de caracteres com um espaço, não uma lista separada por espaços.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-191">This is a string with a space in it, not a space-separated list.</span></span>
9. <span data-ttu-id="ef2f4-192">Ao executar comandos da CLI do Azure no PowerShell, ocorrerão erros de análise se os argumentos contiverem caracteres especiais do PowerShell, como em `@`.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-192">When running Azure CLI commands in PowerShell, parsing errors will occur when the arguments contain special characters of PowerShell, such as at `@`.</span></span> <span data-ttu-id="ef2f4-193">Você pode resolver esse problema adicionando `` ` `` antes do caractere especial para usar o caractere de escape ou colocando o argumento em aspas simples ou duplas `'`/`"`.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-193">You can solve this problem by adding `` ` `` before the special character to escape it, or by enclosing the argument with single or double quotes `'`/`"`.</span></span> <span data-ttu-id="ef2f4-194">Por exemplo, `az group deployment create --parameters @parameters.json` não funciona no PowerShell porque `@` é analisado como um [símbolo de nivelamento](/powershell/module/microsoft.powershell.core/about/about_splatting).</span><span class="sxs-lookup"><span data-stu-id="ef2f4-194">For example, `az group deployment create --parameters @parameters.json` doesn't work in PowerShell because `@` is parsed as a [splatting symbol](/powershell/module/microsoft.powershell.core/about/about_splatting).</span></span> <span data-ttu-id="ef2f4-195">Para corrigir isso, você pode alterar o argumento para `` `@parameters.json`` ou `'@parameters.json'`.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-195">To fix this, you may change the argument to `` `@parameters.json`` or `'@parameters.json'`.</span></span>
10. <span data-ttu-id="ef2f4-196">Ao usar `--query` com um comando, alguns caracteres de [JMESPath](https://jmespath.org/specification.html) precisam usar o caractere de escape no shell.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-196">When using `--query` with a command, some characters of [JMESPath](https://jmespath.org/specification.html) need to be escaped in the shell.</span></span> <span data-ttu-id="ef2f4-197">Por exemplo, no Bash:</span><span class="sxs-lookup"><span data-stu-id="ef2f4-197">For example, in Bash:</span></span>
    ```sh
    # Wrong, as the dash needs to be quoted in a JMESPath query
    $ az version --query azure-cli
    az version: error: argument --query: invalid jmespath_type value: 'azure-cli'

    # Wrong, as the dash needs to be quoted in a JMESPath query, but quotes are interpreted by Bash
    $ az version --query "azure-cli"
    az version: error: argument --query: invalid jmespath_type value: 'azure-cli'

    # Correct
    $ az version --query '"azure-cli"'
    "2.5.1"

    $ az version --query \"azure-cli\"
    "2.5.1"

    $ az version --query "\"azure-cli\""
    "2.5.1"
    ```

    <span data-ttu-id="ef2f4-198">No Prompt de Comando:</span><span class="sxs-lookup"><span data-stu-id="ef2f4-198">In Command Prompt:</span></span>
    ```cmd
    > az version --query "\"azure-cli\""
    "2.5.1"

    > az version --query \"azure-cli\"
    "2.5.1"
    ```

    <span data-ttu-id="ef2f4-199">No PowerShell (é necessário um escape extra):</span><span class="sxs-lookup"><span data-stu-id="ef2f4-199">In PowerShell (extra escaping is needed):</span></span>
    ```powershell
    > az version --query '\"azure-cli\"'
    "2.5.1"

    > az version --query "\`"azure-cli\`""
    "2.5.1"

    > az version --query "\""azure-cli\"""
    "2.5.1"

    > az --% version --query "\"azure-cli\""
    "2.5.1"

    > az --% version --query \"azure-cli\"
    "2.5.1"
    ```

11. <span data-ttu-id="ef2f4-200">A melhor maneira de solucionar um problema de colocação de aspas é executar o comando com o sinalizador `--debug`.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-200">The best way to troubleshoot a quoting issue is to run the command with `--debug` flag.</span></span> <span data-ttu-id="ef2f4-201">Ele revela os argumentos reais recebidos pela CLI na [sintaxe do Python](https://docs.python.org/3/tutorial/introduction.html#strings).</span><span class="sxs-lookup"><span data-stu-id="ef2f4-201">It reveals the actual arguments received by CLI in [Python's syntax](https://docs.python.org/3/tutorial/introduction.html#strings).</span></span> <span data-ttu-id="ef2f4-202">Por exemplo, no Bash:</span><span class="sxs-lookup"><span data-stu-id="ef2f4-202">For example, in Bash:</span></span>

    ```sh
    # Wrong, as quotes and spaces are interpreted by Bash
    $ az {"key": "value"} --debug
    Command arguments: ['{key:', 'value}', '--debug']

    # Wrong, as quotes are interpreted by Bash
    $ az {"key":"value"} --debug
    Command arguments: ['{key:value}', '--debug']

    # Correct
    $ az '{"key":"value"}' --debug
    Command arguments: ['{"key":"value"}', '--debug']

    # Correct
    $ az "{\"key\":\"value\"}" --debug
    Command arguments: ['{"key":"value"}', '--debug']
    ```

## <a name="work-behind-a-proxy"></a><span data-ttu-id="ef2f4-203">Trabalhar usando um proxy</span><span class="sxs-lookup"><span data-stu-id="ef2f4-203">Work behind a proxy</span></span>

<span data-ttu-id="ef2f4-204">O uso do proxy é comum em redes corporativas ou é introduzido por ferramentas de rastreamento como Fiddler, mitmproxy etc. Se o proxy usar certificados autoassinados, a biblioteca de [Solicitações](https://github.com/kennethreitz/requests) do Python usada pela CLI vai gerar `SSLError("bad handshake: Error([('SSL routines', 'tls_process_server_certificate', 'certificate verify failed')],)",)`.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-204">Proxy is common behind corporate network or introduced by tracing tools like Fiddler, mitmproxy, etc. If the proxy uses self-signed certificates, the Python [Requests](https://github.com/kennethreitz/requests) library which CLI uses will throw `SSLError("bad handshake: Error([('SSL routines', 'tls_process_server_certificate', 'certificate verify failed')],)",)`.</span></span> <span data-ttu-id="ef2f4-205">Há dois modos de lidar com esse erro:</span><span class="sxs-lookup"><span data-stu-id="ef2f4-205">There are 2 ways to handle this error:</span></span>

1. <span data-ttu-id="ef2f4-206">Defina a variável de ambiente `REQUESTS_CA_BUNDLE` como o caminho do arquivo de certificado do pacote de AC no formato PEM.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-206">Set environment variable `REQUESTS_CA_BUNDLE` to the path of CA bundle certificate file in PEM format.</span></span> <span data-ttu-id="ef2f4-207">Isso será recomendado se você usar a CLI com frequência em um proxy corporativo.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-207">This is recommended if you use CLI frequently behind a corporate proxy.</span></span> <span data-ttu-id="ef2f4-208">O pacote de AC padrão que a CLI usa está localizado em `C:\Program Files (x86)\Microsoft SDKs\Azure\CLI2\Lib\site-packages\certifi\cacert.pem` no Windows e em ` /opt/az/lib/python3.6/site-packages/certifi/cacert.pem` no Linux.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-208">The default CA bundle which CLI uses is located at `C:\Program Files (x86)\Microsoft SDKs\Azure\CLI2\Lib\site-packages\certifi\cacert.pem` on Windows and ` /opt/az/lib/python3.6/site-packages/certifi/cacert.pem` on Linux.</span></span> <span data-ttu-id="ef2f4-209">Você pode acrescentar o certificado do servidor proxy nesse arquivo ou copiar o conteúdo para outro arquivo de certificado e, em seguida, definir ele como `REQUESTS_CA_BUNDLE`.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-209">You may append the proxy server's certificate to this file or copy the contents to another certificate file, then set `REQUESTS_CA_BUNDLE` to it.</span></span> <span data-ttu-id="ef2f4-210">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="ef2f4-210">For example:</span></span>

    ```
    <Original cacert.pem>

    -----BEGIN CERTIFICATE-----
    <Your proxy's certificate here>
    -----END CERTIFICATE-----
    ```

   <span data-ttu-id="ef2f4-211">Uma pergunta frequente é se as variáveis de ambiente `HTTP_PROXY` ou `HTTPS_PROXY` devem ou não ser definidas e a resposta é: depende.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-211">A frequent ask is whether or not `HTTP_PROXY` or `HTTPS_PROXY` environment variables should be set, the answer is it depends.</span></span> <span data-ttu-id="ef2f4-212">Por padrão, para o Fiddler no Windows ele atua como um proxy do sistema ao iniciar, você não precisa definir nada.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-212">For Fiddler on Windows, by default it acts as system proxy on start, you don't need to set anything.</span></span> <span data-ttu-id="ef2f4-213">Se a opção estiver desativada ou usando outras ferramentas que não funcionam como proxy do sistema, você deverá defini-las.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-213">If the option is off or using other tools which don't work as system proxy, you should set them.</span></span> <span data-ttu-id="ef2f4-214">Como quase todo o tráfego da CLI é baseado em SSL, somente `HTTPS_PROXY` deve ser definido.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-214">Since almost all traffic from CLI is SSL-based, only `HTTPS_PROXY` should be set.</span></span> <span data-ttu-id="ef2f4-215">Se você não tiver certeza, basta defini-las, mas lembre-se de remover a definição depois que o proxy for desligado.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-215">If you are not sure, just set them, but do remember to unset it after the proxy is shut down.</span></span> <span data-ttu-id="ef2f4-216">Para o Fiddler, o valor padrão é `http://localhost:8888`.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-216">For fiddler, the default value is `http://localhost:8888`.</span></span>

   <span data-ttu-id="ef2f4-217">Para obter outros detalhes, confira o [blog do Stefan](https://blog.jhnr.ch/2018/05/16/working-with-azure-cli-behind-ssl-intercepting-proxy-server/).</span><span class="sxs-lookup"><span data-stu-id="ef2f4-217">For other details, check out [Stefan's blog](https://blog.jhnr.ch/2018/05/16/working-with-azure-cli-behind-ssl-intercepting-proxy-server/).</span></span>

2. <span data-ttu-id="ef2f4-218">Desabilite a verificação de certificado na CLI do Azure definindo a variável de ambiente `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION=1`.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-218">Disable the certificate check across Azure CLI by setting environment variable `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION=1`.</span></span> <span data-ttu-id="ef2f4-219">Isso não é seguro, mas pode ser usado por um curto período, por exemplo, para capturar um rastreamento de rede para um comando específico e desligá-lo imediatamente quando terminar.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-219">This is not safe, but good for a short period like capturing a network trace for a specific command and promptly turning it off when finished.</span></span> <span data-ttu-id="ef2f4-220">Isso pode não funcionar para alguns comandos de plano de dados devido a limitações do SDK subjacentes.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-220">This may not work for some data-plane commands due to underlying SDK limitations.</span></span>

## <a name="concurrent-builds"></a><span data-ttu-id="ef2f4-221">Builds simultâneos</span><span class="sxs-lookup"><span data-stu-id="ef2f4-221">Concurrent builds</span></span>

<span data-ttu-id="ef2f4-222">Se você estiver usando o AZ em um computador de build e vários trabalhos puderem ser executados em paralelo, haverá um risco de que os tokens de logon que são compartilhados entre dois trabalhos de build sejam os trabalhos executados como o mesmo usuário do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-222">If you are using az on a build machine, and multiple jobs can be run in parallel, then there is a risk that the login tokens are shared between two build jobs is the jobs run as the same OS user.</span></span>  <span data-ttu-id="ef2f4-223">Para evitar erros como esse, defina AZURE_CONFIG_DIR como um diretório no qual os tokens de logon devem ser armazenados.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-223">To avoid mix ups like this, set AZURE_CONFIG_DIR to a directory where the login tokens should be stored.</span></span>  <span data-ttu-id="ef2f4-224">Pode ser uma pasta criada aleatoriamente ou apenas o nome do workspace do Jenkins, como este ```AZURE_CONFIG_DIR=.```</span><span class="sxs-lookup"><span data-stu-id="ef2f4-224">It could be a randomly created folder, or just the name of the jenkins workspace, like this ```AZURE_CONFIG_DIR=.```</span></span>

## <a name="appendix"></a><span data-ttu-id="ef2f4-225">Apêndice</span><span class="sxs-lookup"><span data-stu-id="ef2f4-225">Appendix</span></span>

### <a name="windows-batch-scripts-for-saving-to-variables-and-using-it-later"></a><span data-ttu-id="ef2f4-226">Scripts de lote do Windows para salvar em variáveis e usar mais tarde</span><span class="sxs-lookup"><span data-stu-id="ef2f4-226">Windows batch scripts for saving to variables and using it later</span></span>

```batch
ECHO OFF
SETLOCAL
FOR /F "tokens=* USEBACKQ" %%F IN (`az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv`) DO (
    SET "vm_ids=%%F %vm_ids%"  :: construct the id list
)
az vm stop --ids %vm_ids% :: CLI stops all VMs in parallel
```

### <a name="windows-powershell-scripts-for-saving-to-variables-and-using-it-later"></a><span data-ttu-id="ef2f4-227">Scripts do Windows PowerShell para salvar em variáveis e usar mais tarde</span><span class="sxs-lookup"><span data-stu-id="ef2f4-227">Windows PowerShell scripts for saving to variables and using it later</span></span>

```powershell
$vm_ids=(az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv)
az vm stop --ids $vm_ids # CLI stops all VMs in parallel
```

### <a name="windows-batch-scripts-to-loop-through-a-list"></a><span data-ttu-id="ef2f4-228">Scripts de lote do Windows para executar um loop em uma lista</span><span class="sxs-lookup"><span data-stu-id="ef2f4-228">Windows batch scripts to loop through a list</span></span>
```batch
ECHO OFF
SETLOCAL
FOR /F "tokens=* USEBACKQ" %%F IN (`az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv`) DO (
    ECHO Stopping %%F
    az vm stop --ids %%F
)
```

### <a name="windows-powershell-scripts-to-loop-through-a-list"></a><span data-ttu-id="ef2f4-229">Scripts do Windows PowerShell para executar em loop em uma lista</span><span class="sxs-lookup"><span data-stu-id="ef2f4-229">Windows PowerShell scripts to loop through a list</span></span>
```powershell
$vm_ids=(az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv)
foreach ($vm_id in $vm_ids) {
    Write-Output "Stopping $vm_id"
    az vm stop --ids $vm_id
}
```

### <a name="cli-environment-variables"></a><span data-ttu-id="ef2f4-230">Variáveis de ambiente da CLI</span><span class="sxs-lookup"><span data-stu-id="ef2f4-230">CLI Environment Variables</span></span>

|  <span data-ttu-id="ef2f4-231">Variável de ambiente</span><span class="sxs-lookup"><span data-stu-id="ef2f4-231">Environment Variable</span></span>          | <span data-ttu-id="ef2f4-232">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef2f4-232">Description</span></span>            |
|--------------------------------|------------------------|
| <span data-ttu-id="ef2f4-233">**AZURE_CONFIG_DIR**</span><span class="sxs-lookup"><span data-stu-id="ef2f4-233">**AZURE_CONFIG_DIR**</span></span>           | <span data-ttu-id="ef2f4-234">Diretório de configuração global para arquivos de configuração, logs e telemetria.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-234">Global config directory for config files, logs and telemetry.</span></span> <span data-ttu-id="ef2f4-235">Se não for especificado, o padrão será `~/.azure`.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-235">If unspecified, defaults to `~/.azure`.</span></span> |
| <span data-ttu-id="ef2f4-236">**AZURE_EXTENSION_DIR**</span><span class="sxs-lookup"><span data-stu-id="ef2f4-236">**AZURE_EXTENSION_DIR**</span></span>        | <span data-ttu-id="ef2f4-237">O diretório de instalação das extensões.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-237">Extensions' installation directory.</span></span> <span data-ttu-id="ef2f4-238">Se não for especificado, o padrão será o diretório `cliextensions` no diretório de configuração global.</span><span class="sxs-lookup"><span data-stu-id="ef2f4-238">If unspecified, defaults to `cliextensions` directory within the global config directory.</span></span> |
