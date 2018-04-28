---
title: Extensão de alias da CLI do Azure 2.0
description: Como usar a extensão de alias da CLI do Azure 2.0
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 03/14/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 40a43f5013a5dd0d7bb65b21140bb4fc82769267
ms.sourcegitcommit: ae72b6c8916aeb372a92188090529037e63930ba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2018
---
# <a name="the-azure-cli-20-alias-extension"></a><span data-ttu-id="df4c3-103">A extensão de alias da CLI do Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="df4c3-103">The Azure CLI 2.0 alias extension</span></span>

<span data-ttu-id="df4c3-104">A extensão de alias permite que os usuários definam comandos personalizados para a CLI do Azure usando comandos existentes.</span><span class="sxs-lookup"><span data-stu-id="df4c3-104">The alias extension allows users to define custom commands for the Azure CLI by using existing commands.</span></span> <span data-ttu-id="df4c3-105">Aliases ajudam a manter seu fluxo de trabalho simples e conciso permitindo atalhos e fornecendo a capacidade de usar argumentos posicionais.</span><span class="sxs-lookup"><span data-stu-id="df4c3-105">Aliases help keep your workflow concise and simple by allowing shortcuts and giving you the ability to use positional arguments.</span></span> <span data-ttu-id="df4c3-106">Como os aliases são ativados pelo mecanismo do modelo Jinja2, eles oferecem até mesmo o processamento avançado de argumento.</span><span class="sxs-lookup"><span data-stu-id="df4c3-106">Since aliases are powered by the Jinja2 template engine, they even offer advanced argument processing.</span></span>

> [!NOTE]
> <span data-ttu-id="df4c3-107">A Extensão do Alias está em versão prévia pública.</span><span class="sxs-lookup"><span data-stu-id="df4c3-107">The Alias Extension is in public preview.</span></span> <span data-ttu-id="df4c3-108">Os recursos e o formato do arquivo de configuração podem mudar.</span><span class="sxs-lookup"><span data-stu-id="df4c3-108">The features and configuration file format may change.</span></span>

## <a name="install-the-alias-extension"></a><span data-ttu-id="df4c3-109">Instalar a extensão do alias</span><span class="sxs-lookup"><span data-stu-id="df4c3-109">Install the alias extension</span></span>

<span data-ttu-id="df4c3-110">A versão mínima necessária da CLI do Azure para usar a extensão de alias é **2.0.28**.</span><span class="sxs-lookup"><span data-stu-id="df4c3-110">The minimum required Azure CLI version to use the alias extension is **2.0.28**.</span></span> <span data-ttu-id="df4c3-111">Para verificar sua versão da CLI, execute `az --version`.</span><span class="sxs-lookup"><span data-stu-id="df4c3-111">To check your CLI version, run `az --version`.</span></span> <span data-ttu-id="df4c3-112">Se você precisa atualizar sua instalação, siga as instruções em [Instalar a CLI do Azure 2.0](./install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="df4c3-112">If you need to update your installation,  follow the instructions in [Install the Azure CLI 2.0](./install-azure-cli.md).</span></span>

<span data-ttu-id="df4c3-113">Instalar a extensão com o comando [az extension add](/cli/azure/extension#az-extension-add).</span><span class="sxs-lookup"><span data-stu-id="df4c3-113">Install the extension with the [az extension add](/cli/azure/extension#az-extension-add) command.</span></span>

```azurecli
az extension add --name alias
```

<span data-ttu-id="df4c3-114">Verifique a instalação da extensão com [az extension list](/cli/azure/extension#az-extension-list).</span><span class="sxs-lookup"><span data-stu-id="df4c3-114">Verify the installation of the extension with [az extension list](/cli/azure/extension#az-extension-list).</span></span> <span data-ttu-id="df4c3-115">Se a extensão de alias tiver sido instalada corretamente, estará relacionada na saída do comando.</span><span class="sxs-lookup"><span data-stu-id="df4c3-115">If the alias extension was installed properly, it's listed in the command output.</span></span>

```azurecli
az extension list --output table --query '[].{Name:name}'
```

```output
Name
------
alias
```


## <a name="keep-the-extension-up-to-date"></a><span data-ttu-id="df4c3-116">Manter a extensão atualizada</span><span class="sxs-lookup"><span data-stu-id="df4c3-116">Keep the extension up to date</span></span>

<span data-ttu-id="df4c3-117">A extensão do alias está em desenvolvimento ativo, e novas versões são lançadas regularmente.</span><span class="sxs-lookup"><span data-stu-id="df4c3-117">The alias extension is under active development and new versions are released regularly.</span></span> <span data-ttu-id="df4c3-118">Quando você atualiza a CLI, as novas versões não são instaladas automaticamente.</span><span class="sxs-lookup"><span data-stu-id="df4c3-118">New versions are not automatically installed whenever you update the CLI.</span></span> <span data-ttu-id="df4c3-119">Instale as atualizações para a extensão com [az extension update](/cli/azure/extension#az-extension-update).</span><span class="sxs-lookup"><span data-stu-id="df4c3-119">Install the updates for the extension with [az extension update](/cli/azure/extension#az-extension-update).</span></span>

```azurecli
az extension update --name alias
```


## <a name="manage-aliases-for-the-azure-cli"></a><span data-ttu-id="df4c3-120">Gerenciar aliases para a CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="df4c3-120">Manage aliases for the Azure CLI</span></span>

<span data-ttu-id="df4c3-121">A extensão de alias fornece comandos familiares e convenientes para gerenciar aliases.</span><span class="sxs-lookup"><span data-stu-id="df4c3-121">The alias extension provides convenient and familiar commands to manage aliases.</span></span> <span data-ttu-id="df4c3-122">Para exibir todos os comandos disponíveis e os detalhes de parâmetros, invoque o comando de alias com `--help`.</span><span class="sxs-lookup"><span data-stu-id="df4c3-122">To view all the available commands and parameter details, invoke the alias command with `--help`.</span></span>

```azurecli
az alias --help
```


## <a name="create-simple-alias-commands"></a><span data-ttu-id="df4c3-123">Criar comandos simples de alias</span><span class="sxs-lookup"><span data-stu-id="df4c3-123">Create simple alias commands</span></span>

<span data-ttu-id="df4c3-124">Uma das utilidades dos aliases é encurtar grupos de comando ou nomes de comando existentes.</span><span class="sxs-lookup"><span data-stu-id="df4c3-124">One use of aliases is for shortening existing command groups or command names.</span></span> <span data-ttu-id="df4c3-125">Por exemplo, você pode encurtar o grupo de comandos `group` para `rg` e o comando `list` para `ls`.</span><span class="sxs-lookup"><span data-stu-id="df4c3-125">For example, you can shorten the `group` command group to `rg` and the `list` command to `ls`.</span></span>

```azurecli
az alias create --name rg --command group
az alias create --name ls --command list
```

<span data-ttu-id="df4c3-126">Agora, esses aliases recém-definidos podem ser usados nos mesmos lugares que suas definições.</span><span class="sxs-lookup"><span data-stu-id="df4c3-126">These newly defined aliases can now be used anywhere that their definition would be.</span></span>

```azurecli
az rg list
az rg ls
az vm ls
```

<span data-ttu-id="df4c3-127">Não inclua `az` como parte do comando.</span><span class="sxs-lookup"><span data-stu-id="df4c3-127">Do not include `az` as part of the command.</span></span>

<span data-ttu-id="df4c3-128">Aliases também podem ser atalhos para comandos completos.</span><span class="sxs-lookup"><span data-stu-id="df4c3-128">Aliases can also be shortcuts for complete commands.</span></span> <span data-ttu-id="df4c3-129">O exemplo a seguir lista os grupos de recursos disponíveis e suas localizações na saída da tabela:</span><span class="sxs-lookup"><span data-stu-id="df4c3-129">The next example lists available resource groups and their locations in table output:</span></span>

```azurecli
az alias create --name ls-groups --command "group list --query '[].{Name:name, Location:location}' --output table"
```

<span data-ttu-id="df4c3-130">Agora, `ls-groups` pode ser executado como qualquer outro comando da CLI.</span><span class="sxs-lookup"><span data-stu-id="df4c3-130">Now `ls-groups` can be run like any other CLI command.</span></span>

```azurecli
az ls-groups
```


## <a name="create-an-alias-command-with-arguments"></a><span data-ttu-id="df4c3-131">Criar um comando de alias com argumentos</span><span class="sxs-lookup"><span data-stu-id="df4c3-131">Create an alias command with arguments</span></span>

<span data-ttu-id="df4c3-132">Você também pode adicionar argumentos posicionais para um comando de alias incluindo-os como `{{ arg_name }}` no nome do alias.</span><span class="sxs-lookup"><span data-stu-id="df4c3-132">You can also add positional arguments to an alias command by including them as `{{ arg_name }}` in the alias name.</span></span> <span data-ttu-id="df4c3-133">O espaço em branco entre as chaves é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df4c3-133">The whitespace inside the braces is required.</span></span>

```azurecli
az alias create --name "alias_name {{ arg1 }} {{ arg2 }} ..." --command "invoke_including_args"
```

<span data-ttu-id="df4c3-134">O exemplo de alias seguinte mostra como usar argumentos posicionais para obter o endereço IP público de uma VM.</span><span class="sxs-lookup"><span data-stu-id="df4c3-134">The next example alias shows how to use positional arguments to get the public IP address for a VM.</span></span>

```azurecli
az alias create \
    --name "get-vm-ip {{ resourceGroup }} {{ vmName }}" \
    --command "vm list-ip-addresses --resource-group {{ resourceGroup }} --name {{ vmName }}
        --query [0].virtualMachine.network.publicIpAddresses[0].ipAddress"
```

<span data-ttu-id="df4c3-135">Ao executar esse comando, você fornece valores para os argumentos posicionais.</span><span class="sxs-lookup"><span data-stu-id="df4c3-135">When running this command, you give values to the positional arguments.</span></span>

```azurecli
az get-vm-ip MyResourceGroup MyVM
```

<span data-ttu-id="df4c3-136">Você também pode usar variáveis de ambiente em comandos invocados pelo aliases, as quais são avaliadas em tempo de execução.</span><span class="sxs-lookup"><span data-stu-id="df4c3-136">You can also use environment variables in commands invoked by aliases, which are evaluated at runtime.</span></span> <span data-ttu-id="df4c3-137">O exemplo a seguir adiciona o alias `create-rg`, que cria um grupo de recursos em `eastus` e adiciona uma marca `owner`.</span><span class="sxs-lookup"><span data-stu-id="df4c3-137">The next example adds the `create-rg` alias, which creates a resource group in `eastus` and adds an `owner` tag.</span></span> <span data-ttu-id="df4c3-138">Essa marca recebe o valor da variável de ambiente local `USER`.</span><span class="sxs-lookup"><span data-stu-id="df4c3-138">This tag is assigned the value of the local environment variable `USER`.</span></span>

```azurecli
az alias create \
    --name "create-rg {{ groupName }}" \
    --command "group create --name {{ groupName }} --location eastus --tags owner=\$USER"
```

<span data-ttu-id="df4c3-139">Para registrar as variáveis de ambiente no comando de alias, o sinal de cifrão `$` deve ser precedido de um caractere de escape.</span><span class="sxs-lookup"><span data-stu-id="df4c3-139">To register the environment variables inside the command of the alias, the dollar sign `$` must be escaped.</span></span>


## <a name="process-arguments-using-jinja2-templates"></a><span data-ttu-id="df4c3-140">Processar argumentos usando modelos Jinja2</span><span class="sxs-lookup"><span data-stu-id="df4c3-140">Process arguments using Jinja2 templates</span></span>

<span data-ttu-id="df4c3-141">A substituição de argumento na extensão de alias é executada por [Jinja2](http://jinja.pocoo.org/docs/2.10/), e fornece acesso completo aos recursos do mecanismo do modelo Jinja2.</span><span class="sxs-lookup"><span data-stu-id="df4c3-141">Argument substitution in the alias extension is performed by [Jinja2](http://jinja.pocoo.org/docs/2.10/), giving you full access to the capabilities of the Jinja2 template engine.</span></span> <span data-ttu-id="df4c3-142">Os modelos permitem que você execute ações como extração de dados e substituição em cadeias de caracteres.</span><span class="sxs-lookup"><span data-stu-id="df4c3-142">Templates allow you to perform actions like data extraction and substitution on strings.</span></span>

<span data-ttu-id="df4c3-143">Com modelos Jinja2, você pode escrever aliases que aceitam tipos diferentes de argumentos em comparação com o comando subjacente.</span><span class="sxs-lookup"><span data-stu-id="df4c3-143">With Jinja2 templates, you can write aliases which take different types of arguments than the underlying command.</span></span> <span data-ttu-id="df4c3-144">Por exemplo, você pode criar um alias que usa uma URL de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="df4c3-144">For example, you can make an alias which takes a storage URL.</span></span> <span data-ttu-id="df4c3-145">Em seguida, essa URL é analisada para passar os nomes de conta e do contêiner para o comando de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="df4c3-145">Then this URL is parsed to pass the account and container names to the storage command.</span></span>

```azurecli
az alias create \
    --name 'storage-ls {{ url }}' \
    --command "storage blob list
        --account-name {{ url.replace('https://', '').split('.')[0] }}
        --container-name {{ url.replace('https://', '').split('/')[1] }}"
```

<span data-ttu-id="df4c3-146">Para saber mais sobre o mecanismo de modelo Jinja2, confira a [documentação do Jinja2](http://jinja.pocoo.org/docs/2.10/templates/).</span><span class="sxs-lookup"><span data-stu-id="df4c3-146">To learn about the Jinja2 template engine, see [the Jinja2 documentation](http://jinja.pocoo.org/docs/2.10/templates/).</span></span>


## <a name="alias-configuration-file"></a><span data-ttu-id="df4c3-147">Arquivo de configuração de alias</span><span class="sxs-lookup"><span data-stu-id="df4c3-147">Alias configuration file</span></span>

<span data-ttu-id="df4c3-148">Outra maneira de criar e modificar aliases é alterando o arquivo de configuração de alias.</span><span class="sxs-lookup"><span data-stu-id="df4c3-148">Another way to create and modify aliases is to alter the alias configuration file.</span></span> <span data-ttu-id="df4c3-149">As definições de comando do alias são gravadas em um arquivo de configuração localizado em `$AZURE_USER_CONFIG/alias`.</span><span class="sxs-lookup"><span data-stu-id="df4c3-149">Alias command definitions are written into a configuration file, located at `$AZURE_USER_CONFIG/alias`.</span></span> <span data-ttu-id="df4c3-150">O valor padrão de `AZURE_USER_CONFIG` é `$HOME/.azure` no Linux e macOS, e `%USERPROFILE%\.azure` no Windows.</span><span class="sxs-lookup"><span data-stu-id="df4c3-150">The default value of `AZURE_USER_CONFIG` is `$HOME/.azure` on macOS and Linux, and `%USERPROFILE%\.azure` on Windows.</span></span> <span data-ttu-id="df4c3-151">O arquivo de configuração do alias é gravado no formato de arquivo de configuração INI.</span><span class="sxs-lookup"><span data-stu-id="df4c3-151">The alias configuration file is written in the INI configuration file format.</span></span> <span data-ttu-id="df4c3-152">O formato para comandos de alias é:</span><span class="sxs-lookup"><span data-stu-id="df4c3-152">The format for alias commands is:</span></span>

```ini
[alias_name]
command = invoked_commands
```

<span data-ttu-id="df4c3-153">Para aliases que contêm argumentos posicionais, o formato para os comandos de alias é:</span><span class="sxs-lookup"><span data-stu-id="df4c3-153">For aliases that contain positional arguments, the format for alias commands is:</span></span>

```ini
[alias_name {{ arg1 }} {{ arg2 }} ...]
command = invoked_commands_including_args
```


## <a name="create-an-alias-command-with-arguments-via-the-alias-configuration-file"></a><span data-ttu-id="df4c3-154">Criar um comando de alias com argumentos por meio do arquivo de configuração do alias</span><span class="sxs-lookup"><span data-stu-id="df4c3-154">Create an alias command with arguments via the alias configuration file</span></span>

<span data-ttu-id="df4c3-155">Abaixo há um arquivo de configuração de alias que contém um comando de alias de exemplo com argumentos, o qual obtém o endereço IP público para uma VM.</span><span class="sxs-lookup"><span data-stu-id="df4c3-155">Below is an alias configuration file that contains an example alias command with arguments, which gets the public IP address for a VM.</span></span> <span data-ttu-id="df4c3-156">Verifique se o comando invocado está em uma única linha e contém os mesmos argumentos definidos no alias.</span><span class="sxs-lookup"><span data-stu-id="df4c3-156">Ensure that the invoked command is in a single line, and contains the same arguments defined in the alias.</span></span>

```ini
[get-vm-ip {{ resourceGroup }} {{ vmName }}]
command = vm list-ip-addresses --resource-group {{ resourceGroup }} --name {{ vmName }} --query [0].virtualMachine.network.publicIpAddresses[0].ipAddress
```


## <a name="uninstall-the-alias-extension"></a><span data-ttu-id="df4c3-157">Desinstalar a extensão do alias</span><span class="sxs-lookup"><span data-stu-id="df4c3-157">Uninstall the alias extension</span></span>

<span data-ttu-id="df4c3-158">Para desinstalar a extensão, use o comando [az extension remove](/cli/azure/extension#az-extension-remove).</span><span class="sxs-lookup"><span data-stu-id="df4c3-158">To uninstall the extension, use the [az extension remove](/cli/azure/extension#az-extension-remove) command.</span></span>

```azurecli
az extension remove --name alias
```

<span data-ttu-id="df4c3-159">Se você desinstalou devido a um bug ou outros problemas com a extensão, [arquive um problema do GitHub](https://github.com/Azure/azure-cli-extensions/issues) para que possamos fornecer uma correção.</span><span class="sxs-lookup"><span data-stu-id="df4c3-159">If you uninstalled due to a bug or other problem with the extension, please [file a GitHub issue](https://github.com/Azure/azure-cli-extensions/issues) so that we can provide a fix.</span></span>
