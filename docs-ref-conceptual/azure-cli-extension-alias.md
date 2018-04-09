---
title: Extensão de alias da CLI do Azure 2.0
description: Como usar a extensão de alias da CLI do Azure 2.0
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 03/14/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: e457d78b1009fe573554df36db18f525516e0b4a
ms.sourcegitcommit: 335c11e6c34f7907e61a43507745ba84ed4e7469
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/05/2018
---
# <a name="the-azure-cli-20-alias-extension"></a><span data-ttu-id="7843a-103">A extensão de alias da CLI do Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="7843a-103">The Azure CLI 2.0 alias extension</span></span>

<span data-ttu-id="7843a-104">A extensão de alias permite que os usuários definam comandos personalizados para a CLI do Azure usando comandos existentes.</span><span class="sxs-lookup"><span data-stu-id="7843a-104">The alias extension allows users to define custom commands for the Azure CLI by using existing commands.</span></span> <span data-ttu-id="7843a-105">Aliases ajudam a manter seu fluxo de trabalho simples e conciso permitindo atalhos e fornecendo a capacidade de usar argumentos posicionais.</span><span class="sxs-lookup"><span data-stu-id="7843a-105">Aliases help keep your workflow concise and simple by allowing shortcuts and giving you the ability to use positional arguments.</span></span> <span data-ttu-id="7843a-106">Como os aliases são ativados pelo mecanismo do modelo Jinja2, eles oferecem até mesmo o processamento avançado de argumento.</span><span class="sxs-lookup"><span data-stu-id="7843a-106">Since aliases are powered by the Jinja2 template engine, they even offer advanced argument processing.</span></span>

> [!NOTE]
> <span data-ttu-id="7843a-107">A Extensão do Alias está em versão prévia pública.</span><span class="sxs-lookup"><span data-stu-id="7843a-107">The Alias Extension is in public preview.</span></span> <span data-ttu-id="7843a-108">Os recursos e o formato do arquivo de configuração podem mudar.</span><span class="sxs-lookup"><span data-stu-id="7843a-108">The features and configuration file format may change.</span></span>

## <a name="install-the-alias-extension"></a><span data-ttu-id="7843a-109">Instalar a extensão do alias</span><span class="sxs-lookup"><span data-stu-id="7843a-109">Install the alias extension</span></span>

<span data-ttu-id="7843a-110">A versão mínima necessária da CLI do Azure para usar a extensão de alias é **2.0.28**.</span><span class="sxs-lookup"><span data-stu-id="7843a-110">The minimum required Azure CLI version to use the alias extension is **2.0.28**.</span></span> <span data-ttu-id="7843a-111">Para verificar sua versão da CLI, execute `az --version`.</span><span class="sxs-lookup"><span data-stu-id="7843a-111">To check your CLI version, run `az --version`.</span></span> <span data-ttu-id="7843a-112">Se você precisa atualizar sua instalação, siga as instruções em [Instalar a CLI do Azure 2.0](./install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="7843a-112">If you need to update your installation,  follow the instructions in [Install the Azure CLI 2.0](./install-azure-cli.md).</span></span>

<span data-ttu-id="7843a-113">Instalar a extensão com o comando [az extension add](/cli/azure/extension#az-extension-add).</span><span class="sxs-lookup"><span data-stu-id="7843a-113">Install the extension with the [az extension add](/cli/azure/extension#az-extension-add) command.</span></span>

```azurecli
az extension add --name alias
```

<span data-ttu-id="7843a-114">Verifique a instalação da extensão com [az extension list](/cli/azure/extension#az-extension-list).</span><span class="sxs-lookup"><span data-stu-id="7843a-114">Verify the installation of the extension with [az extension list](/cli/azure/extension#az-extension-list).</span></span> <span data-ttu-id="7843a-115">Se a extensão de alias tiver sido instalada corretamente, estará relacionada na saída do comando.</span><span class="sxs-lookup"><span data-stu-id="7843a-115">If the alias extension was installed properly, it's listed in the command output.</span></span>

```azurecli
az extension list --output table
```

```output
ExtensionType    Name                       Version
---------------  -------------------------  ---------
whl              alias                      0.2.0
```

## <a name="keep-the-extension-up-to-date"></a><span data-ttu-id="7843a-116">Manter a extensão atualizada</span><span class="sxs-lookup"><span data-stu-id="7843a-116">Keep the extension up to date</span></span>

<span data-ttu-id="7843a-117">A extensão do alias está em desenvolvimento ativo, e novas versões são lançadas regularmente.</span><span class="sxs-lookup"><span data-stu-id="7843a-117">The alias extension is under active development and new versions are released regularly.</span></span> <span data-ttu-id="7843a-118">Quando você atualiza a CLI, as novas versões não são instaladas automaticamente.</span><span class="sxs-lookup"><span data-stu-id="7843a-118">New versions are not automatically installed whenever you update the CLI.</span></span> <span data-ttu-id="7843a-119">Instale as atualizações para a extensão com [az extension update](/cli/azure/extension#az-extension-update).</span><span class="sxs-lookup"><span data-stu-id="7843a-119">Install the updates for the extension with [az extension update](/cli/azure/extension#az-extension-update).</span></span>

```azurecli
az extension update --name alias
```

## <a name="alias-commands-file-format"></a><span data-ttu-id="7843a-120">Formato de arquivo de comandos do alias</span><span class="sxs-lookup"><span data-stu-id="7843a-120">Alias commands file format</span></span>

<span data-ttu-id="7843a-121">As definições de comando do alias são gravadas em um arquivo de configuração localizado em `$AZURE_USER_CONFIG/alias`.</span><span class="sxs-lookup"><span data-stu-id="7843a-121">Alias command definitions are written into a configuration file, located at `$AZURE_USER_CONFIG/alias`.</span></span> <span data-ttu-id="7843a-122">O valor padrão de `AZURE_USER_CONFIG` é `$HOME/.azure` no Linux e macOS, e `%USERPROFILE%\.azure` no Windows.</span><span class="sxs-lookup"><span data-stu-id="7843a-122">The default value of `AZURE_USER_CONFIG` is `$HOME/.azure` on macOS and Linux, and `%USERPROFILE%\.azure` on Windows.</span></span> <span data-ttu-id="7843a-123">O arquivo de configuração do alias é gravado no formato de arquivo de configuração INI.</span><span class="sxs-lookup"><span data-stu-id="7843a-123">The alias configuration file is written in the INI configuration file format.</span></span> <span data-ttu-id="7843a-124">O formato geral para comandos de alias é:</span><span class="sxs-lookup"><span data-stu-id="7843a-124">The general format for alias commands is:</span></span>

```
[command_name]
command = invoked_commands
```

<span data-ttu-id="7843a-125">Não inclua `az` como parte do comando.</span><span class="sxs-lookup"><span data-stu-id="7843a-125">Don't include `az` as part of the command.</span></span>

## <a name="create-simple-alias-commands"></a><span data-ttu-id="7843a-126">Criar comandos simples de alias</span><span class="sxs-lookup"><span data-stu-id="7843a-126">Create simple alias commands</span></span>

<span data-ttu-id="7843a-127">Uma das utilidades dos aliases é encurtar grupos de comando ou nomes de comando existentes.</span><span class="sxs-lookup"><span data-stu-id="7843a-127">One use of aliases is for shortening existing command groups or command names.</span></span> <span data-ttu-id="7843a-128">Por exemplo, você pode encurtar o grupo de comandos `group` para `rg` e o comando `list` para `ls`.</span><span class="sxs-lookup"><span data-stu-id="7843a-128">For example, you can shorten the `group` command group to `rg` and the `list` command to `ls`.</span></span>

```
[rg]
command = group

[ls]
command = list
```

<span data-ttu-id="7843a-129">Agora, esses aliases recém-definidos podem ser usados nos mesmos lugares que suas definições.</span><span class="sxs-lookup"><span data-stu-id="7843a-129">These newly defined aliases can now be used anywhere that their definition would be.</span></span>

```azurecli
az rg list
az rg ls
az vm ls
```

<span data-ttu-id="7843a-130">Aliases também podem ser atalhos para comandos completos.</span><span class="sxs-lookup"><span data-stu-id="7843a-130">Aliases can also be shortcuts for complete commands.</span></span> <span data-ttu-id="7843a-131">O exemplo a seguir lista os grupos de recursos disponíveis e suas localizações na saída da tabela:</span><span class="sxs-lookup"><span data-stu-id="7843a-131">The next example lists available resource groups and their locations in table output:</span></span>

```
[ls-groups]
command = group list --query '[].{Name:name, Location:location}' --output table
```

<span data-ttu-id="7843a-132">Agora, `ls-groups` pode ser executado como qualquer outro comando da CLI.</span><span class="sxs-lookup"><span data-stu-id="7843a-132">Now `ls-groups` can be run like any other CLI command.</span></span>

```azurecli
az ls-groups
```

## <a name="create-an-alias-command-with-arguments"></a><span data-ttu-id="7843a-133">Criar um comando de alias com argumentos</span><span class="sxs-lookup"><span data-stu-id="7843a-133">Create an alias command with arguments</span></span>

<span data-ttu-id="7843a-134">Você também pode adicionar argumentos posicionais para um comando de alias incluindo-os como `{{ arg_name }}` no nome do alias.</span><span class="sxs-lookup"><span data-stu-id="7843a-134">You can also add positional arguments to an alias command by including them as `{{ arg_name }}` in the alias name.</span></span> <span data-ttu-id="7843a-135">O espaço em branco entre as chaves é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7843a-135">The whitespace inside the braces is required.</span></span>

```
[alias_name {{ arg1 }} {{ arg2 }} ...]
command = invoke_including_args
```

<span data-ttu-id="7843a-136">O exemplo de alias seguinte mostra como usar argumentos posicionais para obter o endereço IP público de uma VM.</span><span class="sxs-lookup"><span data-stu-id="7843a-136">The next example alias shows how to use positional arguments to get the public IP address for a VM.</span></span>

```
[get-vm-ip {{ resourceGroup }} {{ vmName }}]
command = vm list-ip-addresses --resource-group {{ resourceGroup }} --name {{ vmName }} --query [0].virtualMachine.network.publicIpAddresses[0].ipAddress
```

<span data-ttu-id="7843a-137">Ao executar esse comando, você fornece valores para os argumentos posicionais.</span><span class="sxs-lookup"><span data-stu-id="7843a-137">When running this command, you give values to the positional arguments.</span></span>

```azurecli
az get-vm-ip MyResourceGroup MyVM
```

<span data-ttu-id="7843a-138">Você também pode usar variáveis de ambiente em comandos invocados pelo aliases, as quais são avaliadas em tempo de execução.</span><span class="sxs-lookup"><span data-stu-id="7843a-138">You can also use environment variables in commands invoked by aliases, which are evaluated at runtime.</span></span> <span data-ttu-id="7843a-139">O exemplo a seguir adiciona o alias `create-rg`, que cria um grupo de recursos em `eastus` e adiciona uma marca `owner`.</span><span class="sxs-lookup"><span data-stu-id="7843a-139">The next example adds the `create-rg` alias, which creates a resource group in `eastus` and adds an `owner` tag.</span></span> <span data-ttu-id="7843a-140">Essa marca recebe o valor da variável de ambiente local `USER`.</span><span class="sxs-lookup"><span data-stu-id="7843a-140">This tag is assigned the value of the local environment variable `USER`.</span></span>

```
[create-rg {{ groupName }}]
command = group create --name {{ groupName }} --location eastus --tags owner=$USER
```

## <a name="process-arguments-using-jinja2-templates"></a><span data-ttu-id="7843a-141">Processar argumentos usando modelos Jinja2</span><span class="sxs-lookup"><span data-stu-id="7843a-141">Process arguments using Jinja2 templates</span></span>

<span data-ttu-id="7843a-142">A substituição de argumento na extensão de alias é executada por [Jinja2](http://jinja.pocoo.org/docs/2.10/), e fornece acesso completo aos recursos do mecanismo do modelo Jinja2.</span><span class="sxs-lookup"><span data-stu-id="7843a-142">Argument substitution in the alias extension is performed by [Jinja2](http://jinja.pocoo.org/docs/2.10/), giving you full access to the capabilities of the Jinja2 template engine.</span></span> <span data-ttu-id="7843a-143">Os modelos permitem que você execute ações como extração de dados e substituição em cadeias de caracteres.</span><span class="sxs-lookup"><span data-stu-id="7843a-143">Templates allow you to perform actions like data extraction and substitution on strings.</span></span>

<span data-ttu-id="7843a-144">Com modelos Jinja2, você pode escrever aliases que aceitam tipos diferentes de argumentos em comparação com o comando subjacente.</span><span class="sxs-lookup"><span data-stu-id="7843a-144">With Jinja2 templates, you can write aliases which take different types of arguments than the underlying command.</span></span> <span data-ttu-id="7843a-145">Por exemplo, você pode criar um alias que usa uma URL de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="7843a-145">For example, you can make an alias which takes a storage URL.</span></span> <span data-ttu-id="7843a-146">Em seguida, essa URL é analisada para passar os nomes de conta e do contêiner para o comando de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="7843a-146">Then this URL is parsed to pass the account and container names to the storage command.</span></span>

```
[storage-ls {{ url }}]
command = storage blob list --account-name {{ url.replace('https://', '').split('.')[0] }} --container-name {{ url.replace('https://', '').split('/')[1] }}
```

<span data-ttu-id="7843a-147">Para saber mais sobre o mecanismo de modelo Jinja2, confira a [documentação do Jinja2](http://jinja.pocoo.org/docs/2.10/templates/).</span><span class="sxs-lookup"><span data-stu-id="7843a-147">To learn about the Jinja2 template engine, see [the Jinja2 documentation](http://jinja.pocoo.org/docs/2.10/templates/).</span></span>

## <a name="uninstall-the-alias-extension"></a><span data-ttu-id="7843a-148">Desinstalar a extensão do alias</span><span class="sxs-lookup"><span data-stu-id="7843a-148">Uninstall the alias extension</span></span>

<span data-ttu-id="7843a-149">Para desinstalar a extensão, use o comando [az extension remove](/cli/azure/extension#az-extension-remove).</span><span class="sxs-lookup"><span data-stu-id="7843a-149">To uninstall the extension, use the [az extension remove](/cli/azure/extension#az-extension-remove) command.</span></span>

```azurecli
az extension remove --name alias
```

<span data-ttu-id="7843a-150">Se você desinstalou devido a um bug ou outros problemas com a extensão, [arquive um problema do GitHub](https://github.com/Azure/azure-cli-extensions/issues) para que possamos fornecer uma correção.</span><span class="sxs-lookup"><span data-stu-id="7843a-150">If you uninstalled due to a bug or other problem with the extension, please [file a GitHub issue](https://github.com/Azure/azure-cli-extensions/issues) so that we can provide a fix.</span></span>
