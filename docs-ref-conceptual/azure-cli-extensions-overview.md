---
title: Extensões da CLI 2.0 do Azure
description: Usar extensões com a CLI 2.0 do Azure
keywords: CLI do Azure, Extensões
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 8df4c82253e958fdad37ef1551c051f3d17fb191
ms.sourcegitcommit: 0e688704889fc88b91588bb6678a933c2d54f020
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/11/2018
ms.locfileid: "44388534"
---
# <a name="use-extensions-with-azure-cli-20"></a><span data-ttu-id="81cf4-104">Usar extensões com a CLI do Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="81cf4-104">Use extensions with Azure CLI 2.0</span></span>

<span data-ttu-id="81cf4-105">A CLI do Azure 2.0 oferece a capacidade de carregar extensões.</span><span class="sxs-lookup"><span data-stu-id="81cf4-105">The Azure CLI 2.0 offers the capability to load extensions.</span></span> <span data-ttu-id="81cf4-106">As extensões são arquivos wheel Python que não são enviadas como parte da CLI, mas executadas como comandos da CLI.</span><span class="sxs-lookup"><span data-stu-id="81cf4-106">Extensions are Python wheels that aren't shipped as part of the CLI but run as CLI commands.</span></span>
<span data-ttu-id="81cf4-107">Com as extensões, você recebe acesso a comandos experimentais e de pré-lançamento, juntamente com a capacidade de escrever suas próprias interfaces de CLI.</span><span class="sxs-lookup"><span data-stu-id="81cf4-107">With extensions, you gain access to experimental and pre-release commands along with the ability to write your own CLI interfaces.</span></span> <span data-ttu-id="81cf4-108">Este artigo aborda como gerenciar extensões e responde a perguntas comuns sobre seu uso.</span><span class="sxs-lookup"><span data-stu-id="81cf4-108">This article covers how to manage extensions and answers common questions about their use.</span></span>

## <a name="find-extensions"></a><span data-ttu-id="81cf4-109">Localizar extensões</span><span class="sxs-lookup"><span data-stu-id="81cf4-109">Find extensions</span></span>

<span data-ttu-id="81cf4-110">Para ver as extensões fornecidas e mantidas pela Microsoft, use o comando [az extension list-available](/cli/azure/extension#az-extension-list-available).</span><span class="sxs-lookup"><span data-stu-id="81cf4-110">To see the extensions provided and maintained by Microsoft, use the [az extension list-available](/cli/azure/extension#az-extension-list-available) command.</span></span>

```azurecli-interactive
az extension list-available --output table
```

<span data-ttu-id="81cf4-111">Também hospedamos uma [lista de extensões](azure-cli-extensions-list.md) no site de documentação.</span><span class="sxs-lookup"><span data-stu-id="81cf4-111">We also host a [list of extensions](azure-cli-extensions-list.md) on the documentation site.</span></span>

## <a name="install-extensions"></a><span data-ttu-id="81cf4-112">Instalar extensões</span><span class="sxs-lookup"><span data-stu-id="81cf4-112">Install extensions</span></span>

<span data-ttu-id="81cf4-113">Depois de encontrar uma extensão para instalar, use [az extension add](https://docs.microsoft.com/cli/azure/extension#az-extension-add) para obtê-la.</span><span class="sxs-lookup"><span data-stu-id="81cf4-113">Once you have found an extension to install, use [az extension add](https://docs.microsoft.com/cli/azure/extension#az-extension-add) to get it.</span></span> <span data-ttu-id="81cf4-114">Se a extensão estiver listada em `az extension list-available`, é possível instalar a extensão pelo nome.</span><span class="sxs-lookup"><span data-stu-id="81cf4-114">If the extension is listed in `az extension list-available`, you can install the extension by name.</span></span>

```azurecli-interactive
az extension add --name <extension-name>
```

<span data-ttu-id="81cf4-115">Se a extensão for de um recurso externo ou se você tiver um link direto para ela, forneça a URL de origem ou o caminho local.</span><span class="sxs-lookup"><span data-stu-id="81cf4-115">If the extension is from an external resource or you have a direct link to it, provide the source URL or local path.</span></span> <span data-ttu-id="81cf4-116">A extensão _deve_ ser um arquivo wheel Python compilado.</span><span class="sxs-lookup"><span data-stu-id="81cf4-116">The extension _must_ be a compiled Python wheel file.</span></span>

```azurecli-interactive
az extension add --source <URL-or-path>
```

<span data-ttu-id="81cf4-117">Depois de instalada, a extensão pode ser encontrada no valor da variável do shell `$AZURE_EXTENSION_DIR`.</span><span class="sxs-lookup"><span data-stu-id="81cf4-117">Once an extension is installed, it's found under the value of the `$AZURE_EXTENSION_DIR` shell variable.</span></span> <span data-ttu-id="81cf4-118">Se essa variável tiver sua definição removida, por padrão, o valor é `$HOME/.azure/cliextensions` no Linux e macOS e `%USERPROFILE%\.azure\cliextensions` no Windows.</span><span class="sxs-lookup"><span data-stu-id="81cf4-118">If this variable is unset, by default the value is `$HOME/.azure/cliextensions` on Linux and macOS, and `%USERPROFILE%\.azure\cliextensions` on Windows.</span></span>

## <a name="update-extensions"></a><span data-ttu-id="81cf4-119">Atualizar extensões</span><span class="sxs-lookup"><span data-stu-id="81cf4-119">Update extensions</span></span>

<span data-ttu-id="81cf4-120">Se uma extensão tiver sido instalada pelo nome, atualize-a usando [az extension update](https://docs.microsoft.com/cli/azure/extension#az-extension-update).</span><span class="sxs-lookup"><span data-stu-id="81cf4-120">If an extension was installed by name, update it using [az extension update](https://docs.microsoft.com/cli/azure/extension#az-extension-update).</span></span>

```azurecli-interactive
az extension update --name <extension-name>
```

<span data-ttu-id="81cf4-121">Caso contrário, uma extensão poderá ser atualizada a partir da origem seguindo as instruções em [Instalar extensões](#install-extensions).</span><span class="sxs-lookup"><span data-stu-id="81cf4-121">Otherwise, an extension can be updated from source by following the [Install extensions](#install-extensions) instructions.</span></span>

<span data-ttu-id="81cf4-122">Se o nome de uma extensão não puder ser resolvido pela CLI, desinstale-a e tente reinstalá-la.</span><span class="sxs-lookup"><span data-stu-id="81cf4-122">If an extension name can't be resolved by the CLI, uninstall it and attempt to reinstall.</span></span> <span data-ttu-id="81cf4-123">A extensão também pode ter se tornado parte da CLI base.</span><span class="sxs-lookup"><span data-stu-id="81cf4-123">The extension could also have become part of the base CLI.</span></span>
<span data-ttu-id="81cf4-124">Tente atualizar a CLI, conforme descrito em [Instalar a CLI do Azure 2.0](install-azure-cli.md) e verifique se os comandos da extensão foram adicionados.</span><span class="sxs-lookup"><span data-stu-id="81cf4-124">Try updating the CLI as described in [Install the Azure CLI 2.0](install-azure-cli.md) and see if the extension's commands were added.</span></span>

## <a name="uninstall-extensions"></a><span data-ttu-id="81cf4-125">Desinstalar as extensões</span><span class="sxs-lookup"><span data-stu-id="81cf4-125">Uninstall extensions</span></span>

<span data-ttu-id="81cf4-126">Se você já não precisar de uma extensão, remova-a com [az extension remove](https://docs.microsoft.com/cli/azure/extension#az-extension-remove).</span><span class="sxs-lookup"><span data-stu-id="81cf4-126">If you no longer need an extension, remove it with [az extension remove](https://docs.microsoft.com/cli/azure/extension#az-extension-remove).</span></span>

```azurecli-interactive
az extension remove --name <extension-name>
```

<span data-ttu-id="81cf4-127">Também é possível remover uma extensão manualmente, excluindo-a do local onde foi instalada.</span><span class="sxs-lookup"><span data-stu-id="81cf4-127">You can also remove an extension manually by deleting it from the location where it was installed.</span></span> <span data-ttu-id="81cf4-128">A variável do shell `$AZURE_EXTENSION_DIR` define onde os módulos são instalados.</span><span class="sxs-lookup"><span data-stu-id="81cf4-128">The `$AZURE_EXTENSION_DIR` shell variable defines where modules are installed.</span></span>
<span data-ttu-id="81cf4-129">Se essa variável tiver sua definição removida, por padrão, o valor é `$HOME/.azure/cliextensions` no Linux e macOS e `%USERPROFILE%\.azure\cliextensions` no Windows.</span><span class="sxs-lookup"><span data-stu-id="81cf4-129">If this variable is unset, by default the value is `$HOME/.azure/cliextensions` on Linux and macOS, and `%USERPROFILE%\.azure\cliextensions` on Windows.</span></span>

```bash
rm -rf $AZURE_EXTENSION_DIR/<extension-name>
```

## <a name="faq"></a><span data-ttu-id="81cf4-130">Perguntas frequentes</span><span class="sxs-lookup"><span data-stu-id="81cf4-130">FAQ</span></span>

<span data-ttu-id="81cf4-131">Aqui estão algumas respostas para outras perguntas comuns sobre extensões da CLI.</span><span class="sxs-lookup"><span data-stu-id="81cf4-131">Here are some answers to other common questions about CLI extensions.</span></span>

### <a name="what-file-formats-are-allowed-for-installation"></a><span data-ttu-id="81cf4-132">Quais formatos de arquivo são permitidos para instalação?</span><span class="sxs-lookup"><span data-stu-id="81cf4-132">What file formats are allowed for installation?</span></span>

<span data-ttu-id="81cf4-133">Atualmente, apenas wheels compilados do Python podem ser instalados como extensões.</span><span class="sxs-lookup"><span data-stu-id="81cf4-133">Currently, only compiled Python wheels can be installed as extensions.</span></span>

### <a name="can-extensions-replace-existing-commands"></a><span data-ttu-id="81cf4-134">As extensões podem substituir os comandos existentes?</span><span class="sxs-lookup"><span data-stu-id="81cf4-134">Can extensions replace existing commands?</span></span>

<span data-ttu-id="81cf4-135">Sim.</span><span class="sxs-lookup"><span data-stu-id="81cf4-135">Yes.</span></span> <span data-ttu-id="81cf4-136">As extensões podem substituir os comandos existentes, mas antes de executar um comando que foi substituído, a CLI emitirá um aviso.</span><span class="sxs-lookup"><span data-stu-id="81cf4-136">Extensions may replace existing commands, but before running a command that has been replaced the CLI will issue a warning.</span></span>

### <a name="how-can-i-tell-if-an-extension-is-in-pre-release"></a><span data-ttu-id="81cf4-137">Como posso saber se uma extensão está em pré-lançamento?</span><span class="sxs-lookup"><span data-stu-id="81cf4-137">How can I tell if an extension is in pre-release?</span></span>

<span data-ttu-id="81cf4-138">O controle de versão e a documentação de uma extensão mostrará se ela está em pré-lançamento.</span><span class="sxs-lookup"><span data-stu-id="81cf4-138">An extension's documentation and versioning will show if it's in pre-release.</span></span> <span data-ttu-id="81cf4-139">Geralmente, a Microsoft lança comandos de visualização como extensões da CLI, com a opção de movê-los para o produto principal da CLI posteriormente.</span><span class="sxs-lookup"><span data-stu-id="81cf4-139">Microsoft often releases preview commands as CLI extensions, with the option of moving them into the main CLI product later.</span></span> <span data-ttu-id="81cf4-140">Quando os comandos são removidos das extensões, a extensão antiga deve ser desinstalada.</span><span class="sxs-lookup"><span data-stu-id="81cf4-140">When commands are moved out of extensions, the old extension should be uninstalled.</span></span> 

### <a name="can-extensions-depend-upon-each-other"></a><span data-ttu-id="81cf4-141">As extensões podem depender umas das outras?</span><span class="sxs-lookup"><span data-stu-id="81cf4-141">Can extensions depend upon each other?</span></span>

<span data-ttu-id="81cf4-142">Não.</span><span class="sxs-lookup"><span data-stu-id="81cf4-142">No.</span></span> <span data-ttu-id="81cf4-143">Como a CLI não garante uma ordem de carga, as dependências não poderão ser atendidas.</span><span class="sxs-lookup"><span data-stu-id="81cf4-143">Since the CLI doesn't guarantee a load order, dependencies might not be satisfied.</span></span> <span data-ttu-id="81cf4-144">Remover uma extensão não afetará outras extensões.</span><span class="sxs-lookup"><span data-stu-id="81cf4-144">Removing an extension won't affect any others.</span></span>

### <a name="are-extensions-updated-along-with-the-cli"></a><span data-ttu-id="81cf4-145">As extensões são atualizadas juntamente com a CLI?</span><span class="sxs-lookup"><span data-stu-id="81cf4-145">Are extensions updated along with the CLI?</span></span>

<span data-ttu-id="81cf4-146">Não.</span><span class="sxs-lookup"><span data-stu-id="81cf4-146">No.</span></span> <span data-ttu-id="81cf4-147">As extensões devem ser atualizadas separadamente, conforme descrito em [Atualizar extensões](#update-extensions).</span><span class="sxs-lookup"><span data-stu-id="81cf4-147">Extensions must be updated separately, as described in [Update extensions](#update-extensions).</span></span>
