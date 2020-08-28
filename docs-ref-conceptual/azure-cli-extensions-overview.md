---
title: Extensões da CLI do Azure
description: Usando extensões com a CLI do Azure
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 08/06/2020
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 72e5ca67f9d1d7a754dae098d89f2eb76d108b0b
ms.sourcegitcommit: fd8c3e32f0f50feb6fea33ead636a80a050bcf2a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2020
ms.locfileid: "88713087"
---
# <a name="use-extensions-with-azure-cli"></a><span data-ttu-id="09a5e-103">Usar extensões com a CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="09a5e-103">Use extensions with Azure CLI</span></span> 

<span data-ttu-id="09a5e-104">A CLI do Azure oferece a capacidade de carregar extensões.</span><span class="sxs-lookup"><span data-stu-id="09a5e-104">The Azure CLI offers the capability to load extensions.</span></span> <span data-ttu-id="09a5e-105">As extensões são arquivos wheel Python que não são enviadas como parte da CLI, mas executadas como comandos da CLI.</span><span class="sxs-lookup"><span data-stu-id="09a5e-105">Extensions are Python wheels that aren't shipped as part of the CLI but run as CLI commands.</span></span>
<span data-ttu-id="09a5e-106">Com as extensões, você recebe acesso a comandos experimentais e de pré-lançamento, juntamente com a capacidade de escrever suas próprias interfaces de CLI.</span><span class="sxs-lookup"><span data-stu-id="09a5e-106">With extensions, you gain access to experimental and pre-release commands along with the ability to write your own CLI interfaces.</span></span> <span data-ttu-id="09a5e-107">Este artigo aborda como gerenciar extensões e responde a perguntas comuns sobre seu uso.</span><span class="sxs-lookup"><span data-stu-id="09a5e-107">This article covers how to manage extensions and answers common questions about their use.</span></span>

## <a name="find-extensions"></a><span data-ttu-id="09a5e-108">Localizar extensões</span><span class="sxs-lookup"><span data-stu-id="09a5e-108">Find extensions</span></span>

<span data-ttu-id="09a5e-109">Para ver as extensões fornecidas e mantidas pela Microsoft, use o comando [az extension list-available](/cli/azure/extension#az-extension-list-available).</span><span class="sxs-lookup"><span data-stu-id="09a5e-109">To see the extensions provided and maintained by Microsoft, use the [az extension list-available](/cli/azure/extension#az-extension-list-available) command.</span></span>

```azurecli-interactive
az extension list-available --output table
```

<span data-ttu-id="09a5e-110">Também hospedamos uma [lista de extensões](azure-cli-extensions-list.md) no site de documentação.</span><span class="sxs-lookup"><span data-stu-id="09a5e-110">We also host a [list of extensions](azure-cli-extensions-list.md) on the documentation site.</span></span>

## <a name="install-extensions"></a><span data-ttu-id="09a5e-111">Instalar extensões</span><span class="sxs-lookup"><span data-stu-id="09a5e-111">Install extensions</span></span>

### <a name="install-extensions-manually"></a><span data-ttu-id="09a5e-112">Instalar extensões manualmente</span><span class="sxs-lookup"><span data-stu-id="09a5e-112">Install extensions manually</span></span>

<span data-ttu-id="09a5e-113">Depois de encontrar uma extensão para instalar, use [az extension add](https://docs.microsoft.com/cli/azure/extension#az-extension-add) para obtê-la.</span><span class="sxs-lookup"><span data-stu-id="09a5e-113">Once you have found an extension to install, use [az extension add](https://docs.microsoft.com/cli/azure/extension#az-extension-add) to get it.</span></span> <span data-ttu-id="09a5e-114">Se a extensão estiver listada em `az extension list-available`, é possível instalar a extensão pelo nome.</span><span class="sxs-lookup"><span data-stu-id="09a5e-114">If the extension is listed in `az extension list-available`, you can install the extension by name.</span></span>

```azurecli-interactive
az extension add --name <extension-name>
```

<span data-ttu-id="09a5e-115">Se a extensão for de um recurso externo ou se você tiver um link direto para ela, forneça a URL de origem ou o caminho local.</span><span class="sxs-lookup"><span data-stu-id="09a5e-115">If the extension is from an external resource or you have a direct link to it, provide the source URL or local path.</span></span> <span data-ttu-id="09a5e-116">A extensão _deve_ ser um arquivo wheel Python compilado.</span><span class="sxs-lookup"><span data-stu-id="09a5e-116">The extension _must_ be a compiled Python wheel file.</span></span>

```azurecli-interactive
az extension add --source <URL-or-path>
```

<span data-ttu-id="09a5e-117">Depois de instalada, a extensão pode ser encontrada no valor da variável do shell `$AZURE_EXTENSION_DIR`.</span><span class="sxs-lookup"><span data-stu-id="09a5e-117">Once an extension is installed, it's found under the value of the `$AZURE_EXTENSION_DIR` shell variable.</span></span> <span data-ttu-id="09a5e-118">Se essa variável tiver sua definição removida, por padrão, o valor é `$HOME/.azure/cliextensions` no Linux e macOS e `%USERPROFILE%\.azure\cliextensions` no Windows.</span><span class="sxs-lookup"><span data-stu-id="09a5e-118">If this variable is unset, by default the value is `$HOME/.azure/cliextensions` on Linux and macOS, and `%USERPROFILE%\.azure\cliextensions` on Windows.</span></span>

### <a name="install-extensions-automatically"></a><span data-ttu-id="09a5e-119">Instalar extensões automaticamente</span><span class="sxs-lookup"><span data-stu-id="09a5e-119">Install extensions automatically</span></span>

<span data-ttu-id="09a5e-120">Quando você executa um comando de extensão que não está instalado, a CLI do Azure pode reconhecer o comando executado e instalar automaticamente a extensão para você da versão `2.10.0` em diante.</span><span class="sxs-lookup"><span data-stu-id="09a5e-120">When you run an extension command that is not installed, the Azure CLI can recognize the command you run, and automatically install the extension for you starting from version `2.10.0`.</span></span> <span data-ttu-id="09a5e-121">Esse recurso, conhecido como **instalação dinâmica**, é habilitado por meio de configuração.</span><span class="sxs-lookup"><span data-stu-id="09a5e-121">This feature, referred to as **dynamic install**, is enabled through configuration.</span></span>
```azurecli-interactive
az config set extension.use_dynamic_install=yes_prompt
```

<span data-ttu-id="09a5e-122">Use o comando de configuração a seguir para habilitar a instalação dinâmica sem um prompt.</span><span class="sxs-lookup"><span data-stu-id="09a5e-122">Use the following configuration command to enable dynamic install without a prompt.</span></span>
```azurecli-interactive
az config set extension.use_dynamic_install=yes_without_prompt
```

<span data-ttu-id="09a5e-123">Use o comando de configuração a seguir para desligar o recurso de instalação dinâmica e reverter para o comportamento padrão.</span><span class="sxs-lookup"><span data-stu-id="09a5e-123">Use the following configuration command to turn off the dynamic install feature to revert to the default behavior.</span></span> <span data-ttu-id="09a5e-124">O comando de extensão retornará um erro de comando não encontrado se a extensão não estiver instalada.</span><span class="sxs-lookup"><span data-stu-id="09a5e-124">The extension command will return a command-not-found error if the extension is not installed.</span></span>
```azurecli-interactive
az config set extension.use_dynamic_install=no
```

<span data-ttu-id="09a5e-125">Por padrão, um comando de extensão que solicita a instalação dinâmica não continuará sendo executado.</span><span class="sxs-lookup"><span data-stu-id="09a5e-125">By default, an extension command that prompts dynamic install will not continue to run.</span></span> <span data-ttu-id="09a5e-126">Definindo a propriedade `run_after_dynamic_install` como `yes`, altere o comportamento padrão e faça o comando continuar.</span><span class="sxs-lookup"><span data-stu-id="09a5e-126">You can change the default behavior and make the command continue by setting the `run_after_dynamic_install` property to `yes`.</span></span>
```azurecli-interactive
az config set extension.run_after_dynamic_install=yes
```

## <a name="update-extensions"></a><span data-ttu-id="09a5e-127">Atualizar extensões</span><span class="sxs-lookup"><span data-stu-id="09a5e-127">Update extensions</span></span>

<span data-ttu-id="09a5e-128">Se uma extensão tiver sido instalada pelo nome, atualize-a usando [az extension update](https://docs.microsoft.com/cli/azure/extension#az-extension-update).</span><span class="sxs-lookup"><span data-stu-id="09a5e-128">If an extension was installed by name, update it using [az extension update](https://docs.microsoft.com/cli/azure/extension#az-extension-update).</span></span>

```azurecli-interactive
az extension update --name <extension-name>
```

<span data-ttu-id="09a5e-129">Caso contrário, uma extensão poderá ser atualizada a partir da origem seguindo as instruções em [Instalar extensões](#install-extensions).</span><span class="sxs-lookup"><span data-stu-id="09a5e-129">Otherwise, an extension can be updated from source by following the [Install extensions](#install-extensions) instructions.</span></span>

<span data-ttu-id="09a5e-130">Se o nome de uma extensão não puder ser resolvido pela CLI, desinstale-a e tente reinstalá-la.</span><span class="sxs-lookup"><span data-stu-id="09a5e-130">If an extension name can't be resolved by the CLI, uninstall it and attempt to reinstall.</span></span> <span data-ttu-id="09a5e-131">A extensão também pode ter se tornado parte da CLI base.</span><span class="sxs-lookup"><span data-stu-id="09a5e-131">The extension could also have become part of the base CLI.</span></span>
<span data-ttu-id="09a5e-132">Tente atualizar a CLI conforme descrito em [Instalar a CLI do Azure](install-azure-cli.md) e verifique se os comandos da extensão foram adicionados.</span><span class="sxs-lookup"><span data-stu-id="09a5e-132">Try updating the CLI as described in [Install the Azure CLI](install-azure-cli.md) and see if the extension's commands were added.</span></span>

## <a name="uninstall-extensions"></a><span data-ttu-id="09a5e-133">Desinstalar as extensões</span><span class="sxs-lookup"><span data-stu-id="09a5e-133">Uninstall extensions</span></span>

<span data-ttu-id="09a5e-134">Se você já não precisar de uma extensão, remova-a com [az extension remove](https://docs.microsoft.com/cli/azure/extension#az-extension-remove).</span><span class="sxs-lookup"><span data-stu-id="09a5e-134">If you no longer need an extension, remove it with [az extension remove](https://docs.microsoft.com/cli/azure/extension#az-extension-remove).</span></span>

```azurecli-interactive
az extension remove --name <extension-name>
```

<span data-ttu-id="09a5e-135">Também é possível remover uma extensão manualmente, excluindo-a do local onde foi instalada.</span><span class="sxs-lookup"><span data-stu-id="09a5e-135">You can also remove an extension manually by deleting it from the location where it was installed.</span></span> <span data-ttu-id="09a5e-136">A variável do shell `$AZURE_EXTENSION_DIR` define onde os módulos são instalados.</span><span class="sxs-lookup"><span data-stu-id="09a5e-136">The `$AZURE_EXTENSION_DIR` shell variable defines where modules are installed.</span></span>
<span data-ttu-id="09a5e-137">Se essa variável tiver sua definição removida, por padrão, o valor é `$HOME/.azure/cliextensions` no Linux e macOS e `%USERPROFILE%\.azure\cliextensions` no Windows.</span><span class="sxs-lookup"><span data-stu-id="09a5e-137">If this variable is unset, by default the value is `$HOME/.azure/cliextensions` on Linux and macOS, and `%USERPROFILE%\.azure\cliextensions` on Windows.</span></span>

```bash
rm -rf $AZURE_EXTENSION_DIR/<extension-name>
```

## <a name="faq"></a><span data-ttu-id="09a5e-138">Perguntas frequentes</span><span class="sxs-lookup"><span data-stu-id="09a5e-138">FAQ</span></span>

<span data-ttu-id="09a5e-139">Aqui estão algumas respostas para outras perguntas comuns sobre extensões da CLI.</span><span class="sxs-lookup"><span data-stu-id="09a5e-139">Here are some answers to other common questions about CLI extensions.</span></span>

### <a name="what-file-formats-are-allowed-for-installation"></a><span data-ttu-id="09a5e-140">Quais formatos de arquivo são permitidos para instalação?</span><span class="sxs-lookup"><span data-stu-id="09a5e-140">What file formats are allowed for installation?</span></span>

<span data-ttu-id="09a5e-141">Atualmente, apenas wheels compilados do Python podem ser instalados como extensões.</span><span class="sxs-lookup"><span data-stu-id="09a5e-141">Currently, only compiled Python wheels can be installed as extensions.</span></span>

### <a name="can-extensions-replace-existing-commands"></a><span data-ttu-id="09a5e-142">As extensões podem substituir os comandos existentes?</span><span class="sxs-lookup"><span data-stu-id="09a5e-142">Can extensions replace existing commands?</span></span>

<span data-ttu-id="09a5e-143">Sim.</span><span class="sxs-lookup"><span data-stu-id="09a5e-143">Yes.</span></span> <span data-ttu-id="09a5e-144">As extensões podem substituir os comandos existentes, mas antes de executar um comando que foi substituído, a CLI emitirá um aviso.</span><span class="sxs-lookup"><span data-stu-id="09a5e-144">Extensions may replace existing commands, but before running a command that has been replaced the CLI will issue a warning.</span></span>

### <a name="how-can-i-tell-if-an-extension-is-in-pre-release"></a><span data-ttu-id="09a5e-145">Como posso saber se uma extensão está em pré-lançamento?</span><span class="sxs-lookup"><span data-stu-id="09a5e-145">How can I tell if an extension is in pre-release?</span></span>

<span data-ttu-id="09a5e-146">O controle de versão e a documentação de uma extensão mostrará se ela está em pré-lançamento.</span><span class="sxs-lookup"><span data-stu-id="09a5e-146">An extension's documentation and versioning will show if it's in pre-release.</span></span> <span data-ttu-id="09a5e-147">Geralmente, a Microsoft lança comandos de visualização como extensões da CLI, com a opção de movê-los para o produto principal da CLI posteriormente.</span><span class="sxs-lookup"><span data-stu-id="09a5e-147">Microsoft often releases preview commands as CLI extensions, with the option of moving them into the main CLI product later.</span></span> <span data-ttu-id="09a5e-148">Quando os comandos são removidos das extensões, a extensão antiga deve ser desinstalada.</span><span class="sxs-lookup"><span data-stu-id="09a5e-148">When commands are moved out of extensions, the old extension should be uninstalled.</span></span> 

### <a name="can-extensions-depend-upon-each-other"></a><span data-ttu-id="09a5e-149">As extensões podem depender umas das outras?</span><span class="sxs-lookup"><span data-stu-id="09a5e-149">Can extensions depend upon each other?</span></span>

<span data-ttu-id="09a5e-150">Não.</span><span class="sxs-lookup"><span data-stu-id="09a5e-150">No.</span></span> <span data-ttu-id="09a5e-151">Como a CLI não garante uma ordem de carga, as dependências não poderão ser atendidas.</span><span class="sxs-lookup"><span data-stu-id="09a5e-151">Since the CLI doesn't guarantee a load order, dependencies might not be satisfied.</span></span> <span data-ttu-id="09a5e-152">Remover uma extensão não afetará outras extensões.</span><span class="sxs-lookup"><span data-stu-id="09a5e-152">Removing an extension won't affect any others.</span></span>

### <a name="are-extensions-updated-along-with-the-cli"></a><span data-ttu-id="09a5e-153">As extensões são atualizadas juntamente com a CLI?</span><span class="sxs-lookup"><span data-stu-id="09a5e-153">Are extensions updated along with the CLI?</span></span>

<span data-ttu-id="09a5e-154">Não.</span><span class="sxs-lookup"><span data-stu-id="09a5e-154">No.</span></span> <span data-ttu-id="09a5e-155">As extensões devem ser atualizadas separadamente, conforme descrito em [Atualizar extensões](#update-extensions).</span><span class="sxs-lookup"><span data-stu-id="09a5e-155">Extensions must be updated separately, as described in [Update extensions](#update-extensions).</span></span>

### <a name="how-to-develop-our-own-extension"></a><span data-ttu-id="09a5e-156">Como desenvolver sua própria extensão?</span><span class="sxs-lookup"><span data-stu-id="09a5e-156">How to develop our own extension?</span></span>
<span data-ttu-id="09a5e-157">Confira o repositório oficial para receber mais ajuda.</span><span class="sxs-lookup"><span data-stu-id="09a5e-157">Please refer to the official repository for more help.</span></span> [<span data-ttu-id="09a5e-158">Azure/azure-cli-extensions</span><span class="sxs-lookup"><span data-stu-id="09a5e-158">Azure/azure-cli-extensions</span></span>](https://github.com/Azure/azure-cli/tree/master/doc/extensions)
