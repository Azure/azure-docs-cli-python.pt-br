---
title: Extensões da CLI 2.0 do Azure
description: Usar extensões com a CLI 2.0 do Azure
keywords: CLI do Azure, Extensões
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/16/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 1b983faef4c1678763b3483192e94a6c96e24f32
ms.sourcegitcommit: 80189ff103c91f8c47ab8ebf586df815fff5dd5d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/07/2018
ms.locfileid: "34479462"
---
# <a name="using-extensions-with-the-azure-cli-20"></a><span data-ttu-id="46632-104">Usar extensões com a CLI 2.0 do Azure</span><span class="sxs-lookup"><span data-stu-id="46632-104">Using extensions with the Azure CLI 2.0</span></span>

<span data-ttu-id="46632-105">Extensões são módulos individuais não enviados com a CLI do Azure em si, o que adiciona funcionalidades por meio de novos comandos.</span><span class="sxs-lookup"><span data-stu-id="46632-105">Extensions are individual modules not shipped with the Azure CLI itself that add functionality through new commands.</span></span> <span data-ttu-id="46632-106">Podem ser ofertas experimentais ou de pré-lançamento, ferramentas especializadas da Microsoft ou recursos personalizados que você escreve por conta própria.</span><span class="sxs-lookup"><span data-stu-id="46632-106">These might be experimental or pre-release offerings, specialized tools from Microsoft, or custom features you write yourself.</span></span> <span data-ttu-id="46632-107">As extensões possibilitam um nível de flexibilidade com a CLI que permite modificá-la conforme as suas necessidades, sem ter de enviar uma grande quantidade de pacotes adicionais que não são considerados parte do conjunto de recursos principais.</span><span class="sxs-lookup"><span data-stu-id="46632-107">Extensions allow for a degree of flexibility with the CLI that let you modify it to your own needs, without having to ship a lot of additional packages that aren't considered part of the core feature set.</span></span>

<span data-ttu-id="46632-108">Este artigo ajuda a entender como instalar, atualizar e remover extensões da CLI.</span><span class="sxs-lookup"><span data-stu-id="46632-108">This article helps you understand how to install, update, and remove extensions for the CLI.</span></span> <span data-ttu-id="46632-109">Também responde a perguntas comuns sobre o comportamento das extensões.</span><span class="sxs-lookup"><span data-stu-id="46632-109">It also answers common questions about extension behavior.</span></span>

## <a name="find-extensions"></a><span data-ttu-id="46632-110">Localizar extensões</span><span class="sxs-lookup"><span data-stu-id="46632-110">Find extensions</span></span>

<span data-ttu-id="46632-111">Para saber quais extensões estão disponíveis, é possível usar [az extension list-available](/cli/azure/extension#az-extension-list-available).</span><span class="sxs-lookup"><span data-stu-id="46632-111">In order to know what extensions are available, you can use [az extension list-available](/cli/azure/extension#az-extension-list-available).</span></span> <span data-ttu-id="46632-112">Este comando lista as extensões oficiais fornecidas e mantidas pela Microsoft.</span><span class="sxs-lookup"><span data-stu-id="46632-112">This command lists the official extensions provided and maintained by Microsoft.</span></span>

```azurecli-interactive
az extension list-available --output table
```

<span data-ttu-id="46632-113">Também hospedamos uma [lista de extensões da Microsoft](azure-cli-extensions-list.md) no site de documentação.</span><span class="sxs-lookup"><span data-stu-id="46632-113">We also host a [list of Microsoft extensions](azure-cli-extensions-list.md) on the documentation site.</span></span>

## <a name="install-extensions"></a><span data-ttu-id="46632-114">Instalar extensões</span><span class="sxs-lookup"><span data-stu-id="46632-114">Install extensions</span></span>

<span data-ttu-id="46632-115">Depois de encontrar uma extensão para instalar, use [az extension add](https://docs.microsoft.com/cli/azure/extension#az-extension-add) para obtê-la.</span><span class="sxs-lookup"><span data-stu-id="46632-115">Once you have found an extension to install, use [az extension add](https://docs.microsoft.com/cli/azure/extension#az-extension-add) to get it.</span></span> <span data-ttu-id="46632-116">Se a extensão estiver listada em `az extension list-available`, é possível instalar a extensão pelo nome.</span><span class="sxs-lookup"><span data-stu-id="46632-116">If the extension is listed in `az extension list-available`, you can install the extension by name.</span></span>

```azurecli-interactive
az extension add --name <extension-name>
```

<span data-ttu-id="46632-117">Se a extensão for de um recurso externo ou se você tiver um link direto a ela, é possível fornecer a URL de origem ou o caminho local.</span><span class="sxs-lookup"><span data-stu-id="46632-117">If the extension is from an external resource or you have a direct link to it, you can provide the source URL or local path.</span></span> <span data-ttu-id="46632-118">Ela _deve_ ser um arquivo wheel Python compilado.</span><span class="sxs-lookup"><span data-stu-id="46632-118">This _must_ be a compiled Python wheel file.</span></span>

```azurecli-interactive
az extension add --source <URL-or-path>
```

<span data-ttu-id="46632-119">Depois de instalada, a extensão pode ser encontrada no valor da variável do shell `$AZURE_EXTENSION_DIR`.</span><span class="sxs-lookup"><span data-stu-id="46632-119">Once an extension is installed, it can be found under the value of the `$AZURE_EXTENSION_DIR` shell variable.</span></span> <span data-ttu-id="46632-120">Se essa variável tiver sua definição removida, por padrão, o valor é `$HOME/.azure/cliextensions` no Linux e macOS e `%USERPROFILE%\.azure\cliextensions` no Windows.</span><span class="sxs-lookup"><span data-stu-id="46632-120">If this variable is unset, by default the value is `$HOME/.azure/cliextensions` on Linux and macOS, and `%USERPROFILE%\.azure\cliextensions` on Windows.</span></span>

## <a name="update-extensions"></a><span data-ttu-id="46632-121">Atualizar extensões</span><span class="sxs-lookup"><span data-stu-id="46632-121">Update extensions</span></span>

<span data-ttu-id="46632-122">Se uma extensão tiver sido instalada pelo nome, ela poderá ser atualizada usando [az extension update](https://docs.microsoft.com/cli/azure/extension#az-extension-update).</span><span class="sxs-lookup"><span data-stu-id="46632-122">If an extension was installed by name, it can be updated using [az extension update](https://docs.microsoft.com/cli/azure/extension#az-extension-update).</span></span>

```azurecli-interactive
az extension update --name <extension-name>
```

<span data-ttu-id="46632-123">Caso contrário, uma extensão poderá ser atualizada a partir da origem seguindo as instruções em [Instalar extensões](#install-extensions).</span><span class="sxs-lookup"><span data-stu-id="46632-123">Otherwise, an extension can be updated from source by following the [Install extensions](#install-extensions) instructions.</span></span>

<span data-ttu-id="46632-124">Se um nome de extensão não puder ser resolvido pela CLI, desinstalá-a e tente reinstalá-la.</span><span class="sxs-lookup"><span data-stu-id="46632-124">If an extension name cannot be resolved by the CLI, uninstall it and attempt to reinstall.</span></span> <span data-ttu-id="46632-125">Também há a possibilidade da extensão ter sido movida do modo de versão prévia e ter se tornado um comando interno da CLI.</span><span class="sxs-lookup"><span data-stu-id="46632-125">There's also the possibility that the extension was moved out of preview and became a built-in command for the CLI.</span></span> <span data-ttu-id="46632-126">Tente atualizar a CLI, conforme descrito em [Instalar a CLI do Azure 2.0](install-azure-cli.md) e verifique se os comandos da extensão foram adicionados.</span><span class="sxs-lookup"><span data-stu-id="46632-126">Try updating the CLI as described in [Install the Azure CLI 2.0](install-azure-cli.md) and see if the extension's commands were added.</span></span> 

## <a name="uninstall-extensions"></a><span data-ttu-id="46632-127">Desinstalar as extensões</span><span class="sxs-lookup"><span data-stu-id="46632-127">Uninstall extensions</span></span>

<span data-ttu-id="46632-128">Caso você não precise mais de uma extensão, ela pode ser removida com [az extension remove](https://docs.microsoft.com/cli/azure/extension#az-extension-remove).</span><span class="sxs-lookup"><span data-stu-id="46632-128">If you no longer need an extension, it can be removed with [az extension remove](https://docs.microsoft.com/cli/azure/extension#az-extension-remove).</span></span>

```azurecli-interactive
az extension remove --name <extension-name>
```

<span data-ttu-id="46632-129">Também é possível remover uma extensão manualmente, excluindo-a do local onde foi instalada.</span><span class="sxs-lookup"><span data-stu-id="46632-129">You can also remove an extension manually by deleting it from the location where it was installed.</span></span> <span data-ttu-id="46632-130">Esse será o valor de variável do shell `$AZURE_EXTENSION_DIR`.</span><span class="sxs-lookup"><span data-stu-id="46632-130">This will be the value of the `$AZURE_EXTENSION_DIR` shell variable.</span></span> <span data-ttu-id="46632-131">Se essa variável tiver sua definição removida, por padrão, o valor é `$HOME/.azure/cliextensions` no Linux e macOS e `%USERPROFILE%\.azure\cliextensions` no Windows.</span><span class="sxs-lookup"><span data-stu-id="46632-131">If this variable is unset, by default the value is `$HOME/.azure/cliextensions` on Linux and macOS, and `%USERPROFILE%\.azure\cliextensions` on Windows.</span></span>

```bash
rm -rf $AZURE_EXTENSION_DIR/<extension-name>
```

<span data-ttu-id="46632-132">Recomenda-se fazer a desinstalação usando `az extension remove`.</span><span class="sxs-lookup"><span data-stu-id="46632-132">It is recommended that you uninstall using `az extension remove`.</span></span>

## <a name="faq"></a><span data-ttu-id="46632-133">Perguntas frequentes</span><span class="sxs-lookup"><span data-stu-id="46632-133">FAQ</span></span>

<span data-ttu-id="46632-134">Aqui estão algumas respostas para outras perguntas comuns sobre extensões da CLI.</span><span class="sxs-lookup"><span data-stu-id="46632-134">Here are some answers to other common questions about CLI extensions.</span></span>

### <a name="what-file-formats-are-allowed-for-installation"></a><span data-ttu-id="46632-135">Quais formatos de arquivo são permitidos para instalação?</span><span class="sxs-lookup"><span data-stu-id="46632-135">What file formats are allowed for installation?</span></span>

<span data-ttu-id="46632-136">Atualmente, apenas wheels compilados do Python podem ser instalados como extensões.</span><span class="sxs-lookup"><span data-stu-id="46632-136">Currently, only compiled Python wheels can be installed as extensions.</span></span>

### <a name="can-extensions-replace-existing-commands"></a><span data-ttu-id="46632-137">As extensões podem substituir os comandos existentes?</span><span class="sxs-lookup"><span data-stu-id="46632-137">Can extensions replace existing commands?</span></span>

<span data-ttu-id="46632-138">Sim.</span><span class="sxs-lookup"><span data-stu-id="46632-138">Yes.</span></span> <span data-ttu-id="46632-139">As extensões podem substituir os comandos existentes, mas antes de executar um comando que foi substituído, a CLI emitirá um aviso.</span><span class="sxs-lookup"><span data-stu-id="46632-139">Extensions may replace existing commands, but before running a command that has been replaced the CLI will issue a warning.</span></span>

### <a name="how-can-i-tell-if-an-extension-is-in-pre-release"></a><span data-ttu-id="46632-140">Como posso saber se uma extensão está em pré-lançamento?</span><span class="sxs-lookup"><span data-stu-id="46632-140">How can I tell if an extension is in pre-release?</span></span>

<span data-ttu-id="46632-141">Uma extensão deve indicar, por meio de sua própria documentação e controle de versão, se está em pré-lançamento.</span><span class="sxs-lookup"><span data-stu-id="46632-141">An extension should indicate through its own documentation and versioning if it is in pre-release.</span></span> <span data-ttu-id="46632-142">Também é comum a Microsoft lançar comandos de versão prévia para a CLI como extensões, com planos para movê-las para a interface principal da CLI assim que o produto estiver fora da versão prévia.</span><span class="sxs-lookup"><span data-stu-id="46632-142">It is also common for Microsoft to release preview commands for the CLI as extensions, with plans to move them into the main CLI interface once the product is out of preview.</span></span>

### <a name="can-extensions-depend-upon-each-other"></a><span data-ttu-id="46632-143">As extensões podem depender umas das outras?</span><span class="sxs-lookup"><span data-stu-id="46632-143">Can extensions depend upon each other?</span></span>

<span data-ttu-id="46632-144">Nº</span><span class="sxs-lookup"><span data-stu-id="46632-144">No.</span></span> <span data-ttu-id="46632-145">As extensões devem ser pacotes individuais que não dependem um do outro.</span><span class="sxs-lookup"><span data-stu-id="46632-145">Extensions must be individual packages which do not rely on one another.</span></span> <span data-ttu-id="46632-146">Isso porque a CLI não oferece nenhuma garantia sobre quando as extensões são carregadas. Assim, não se pode garantir que as dependências sejam atendidas.</span><span class="sxs-lookup"><span data-stu-id="46632-146">This is because the CLI gives no guarantee about when extensions are loaded, so dependencies could not be guaranteed to be satisfied.</span></span> <span data-ttu-id="46632-147">Ao instalar uma extensão, apenas essa extensão é instalada e ela deve continuar a funcionar mesmo que outras extensões sejam removidas.</span><span class="sxs-lookup"><span data-stu-id="46632-147">Installing an extension installs that extension only, and it should continue to work even if you remove other extensions.</span></span>

### <a name="are-extensions-updated-along-with-the-cli"></a><span data-ttu-id="46632-148">As extensões são atualizadas juntamente com a CLI?</span><span class="sxs-lookup"><span data-stu-id="46632-148">Are extensions updated along with the CLI?</span></span>

<span data-ttu-id="46632-149">Nº</span><span class="sxs-lookup"><span data-stu-id="46632-149">No.</span></span> <span data-ttu-id="46632-150">As extensões devem ser atualizadas separadamente, conforme descrito em [Atualizar extensões](#update-extensions).</span><span class="sxs-lookup"><span data-stu-id="46632-150">Extensions must be updated separately, as described in [Update extensions](#update-extensions).</span></span>
