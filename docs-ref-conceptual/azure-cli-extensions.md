---
title: "Extensões da CLI 2.0 do Azure"
description: "Usar extensões com a CLI 2.0 do Azure"
keywords: "CLI do Azure, Extensões"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 02/13/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 548c06c64cc98598a2bd24bcc5959e59bffb4930
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/15/2018
---
# <a name="using-extensions-with-the-azure-cli-20"></a><span data-ttu-id="be0d1-104">Usar extensões com a CLI 2.0 do Azure</span><span class="sxs-lookup"><span data-stu-id="be0d1-104">Using extensions with the Azure CLI 2.0</span></span>

<span data-ttu-id="be0d1-105">Extensões são módulos individuais não enviados com a CLI do Azure em si, o que adiciona funcionalidades por meio de novos comandos.</span><span class="sxs-lookup"><span data-stu-id="be0d1-105">Extensions are individual modules not shipped with the Azure CLI itself that add functionality through new commands.</span></span> <span data-ttu-id="be0d1-106">Podem ser ofertas experimentais ou de pré-lançamento, ferramentas especializadas da Microsoft ou recursos personalizados que você escreve por conta própria.</span><span class="sxs-lookup"><span data-stu-id="be0d1-106">These might be experimental or pre-release offerings, specialized tools from Microsoft, or custom features you write yourself.</span></span> <span data-ttu-id="be0d1-107">As extensões possibilitam um nível de flexibilidade com a CLI que permite modificá-la conforme as suas necessidades, sem ter de enviar uma grande quantidade de pacotes adicionais que não são considerados parte do conjunto de recursos principais.</span><span class="sxs-lookup"><span data-stu-id="be0d1-107">Extensions allow for a degree of flexibility with the CLI that let you modify it to your own needs, without having to ship a lot of additional packages that aren't considered part of the core feature set.</span></span>

<span data-ttu-id="be0d1-108">Este artigo ajuda a entender como instalar, atualizar e remover extensões da CLI.</span><span class="sxs-lookup"><span data-stu-id="be0d1-108">This article helps you understand how to install, update, and remove extensions for the CLI.</span></span> <span data-ttu-id="be0d1-109">Ele também deve responder a perguntas comuns sobre o comportamento das extensões.</span><span class="sxs-lookup"><span data-stu-id="be0d1-109">It should also answer common questions about extension behavior.</span></span>

## <a name="finding-extensions"></a><span data-ttu-id="be0d1-110">Encontrar extensões</span><span class="sxs-lookup"><span data-stu-id="be0d1-110">Finding extensions</span></span>

<span data-ttu-id="be0d1-111">Para saber quais extensões estão disponíveis, é possível usar [az extension list-available](/cli/azure/extension?view=azure-cli-latest#az_extension_list_available).</span><span class="sxs-lookup"><span data-stu-id="be0d1-111">In order to know what extensions are available, you can use [az extension list-available](/cli/azure/extension?view=azure-cli-latest#az_extension_list_available).</span></span> <span data-ttu-id="be0d1-112">Esse comando lista as extensões oficiais disponíveis, que são fornecidas e com suporte pela Microsoft.</span><span class="sxs-lookup"><span data-stu-id="be0d1-112">This command lists the available, official extensions which are provided and supported by Microsoft.</span></span>

## <a name="installing-extensions"></a><span data-ttu-id="be0d1-113">Instalar extensões</span><span class="sxs-lookup"><span data-stu-id="be0d1-113">Installing extensions</span></span>

<span data-ttu-id="be0d1-114">Depois de encontrar uma extensão para instalar, use [az extension add](https://docs.microsoft.com/en-us/cli/azure/extension?view=azure-cli-latest#az_extension_add) para obtê-la.</span><span class="sxs-lookup"><span data-stu-id="be0d1-114">Once you have found an extension to install, use [az extension add](https://docs.microsoft.com/en-us/cli/azure/extension?view=azure-cli-latest#az_extension_add) to get it.</span></span> <span data-ttu-id="be0d1-115">Se a extensão estiver listada em `az extension list-available`, é possível instalar a extensão pelo nome.</span><span class="sxs-lookup"><span data-stu-id="be0d1-115">If the extension is listed in `az extension list-available`, you can install the extension by name.</span></span>

```azurecli
az extension add --name <extension-name>
```

<span data-ttu-id="be0d1-116">Se a extensão for de um recurso externo ou se você tiver um link direto a ela, é possível fornecer a URL de origem ou o caminho local.</span><span class="sxs-lookup"><span data-stu-id="be0d1-116">If the extension is from an external resource or you have a direct link to it, you can provide the source URL or local path.</span></span> <span data-ttu-id="be0d1-117">Ela _deve_ ser um arquivo wheel Python compilado.</span><span class="sxs-lookup"><span data-stu-id="be0d1-117">This _must_ be a compiled Python wheel file.</span></span>

```azurecli
az extension add --source <URL-or-path>
```

<span data-ttu-id="be0d1-118">Depois de instalada, a extensão pode ser encontrada no valor da variável do shell `$AZURE_EXTENSION_DIR`.</span><span class="sxs-lookup"><span data-stu-id="be0d1-118">Once an extension is installed, it can be found under the value of the `$AZURE_EXTENSION_DIR` shell variable.</span></span> <span data-ttu-id="be0d1-119">Se essa variável tiver sua definição removida, por padrão, o valor é `$HOME/.azure/cliextensions` no Linux e macOS e `%USERPROFILE%\.azure\cliextensions` no Windows.</span><span class="sxs-lookup"><span data-stu-id="be0d1-119">If this variable is unset, by default the value is `$HOME/.azure/cliextensions` on Linux and macOS, and `%USERPROFILE%\.azure\cliextensions` on Windows.</span></span>

## <a name="updating-extensions"></a><span data-ttu-id="be0d1-120">Atualizar extensões</span><span class="sxs-lookup"><span data-stu-id="be0d1-120">Updating extensions</span></span>

<span data-ttu-id="be0d1-121">Extensões só podem ser atualizadas por nome, usando [az extension update](https://docs.microsoft.com/en-us/cli/azure/extension?view=azure-cli-latest#az_extension_update).</span><span class="sxs-lookup"><span data-stu-id="be0d1-121">Extensions can only be updated by name, using [az extension update](https://docs.microsoft.com/en-us/cli/azure/extension?view=azure-cli-latest#az_extension_update).</span></span>

```azurecli
az extension update --name <extension-name>
```

<span data-ttu-id="be0d1-122">Se o nome de uma extensão não pode ser resolvido pela CLI por qualquer motivo, reinstale a extensão para atualizá-lo.</span><span class="sxs-lookup"><span data-stu-id="be0d1-122">If an extension name cannot be resolved by the CLI for whatever reason, reinstall the extension to update it.</span></span> <span data-ttu-id="be0d1-123">Também há a possibilidade da extensão ter sido movida do modo de versão prévia e ter se tornado um comando interno da CLI.</span><span class="sxs-lookup"><span data-stu-id="be0d1-123">There is also the possibility that the extension was moved out of preview and became a built-in command for the CLI.</span></span> <span data-ttu-id="be0d1-124">Nesse caso, atualize a CLI e desinstale a extensão.</span><span class="sxs-lookup"><span data-stu-id="be0d1-124">In that case, update the CLI and uninstall the extension.</span></span>

## <a name="uninstalling-extensions"></a><span data-ttu-id="be0d1-125">Desinstalar extensões</span><span class="sxs-lookup"><span data-stu-id="be0d1-125">Uninstalling extensions</span></span>

<span data-ttu-id="be0d1-126">Caso você não precise mais de uma extensão, ela pode ser removida com [az extension remove](https://docs.microsoft.com/en-us/cli/azure/extension?view=azure-cli-latest#az_extension_remove).</span><span class="sxs-lookup"><span data-stu-id="be0d1-126">If you no longer need an extension, it can be removed with [az extension remove](https://docs.microsoft.com/en-us/cli/azure/extension?view=azure-cli-latest#az_extension_remove).</span></span>

```azurecli
az extension remove --name <extension-name>
```

<span data-ttu-id="be0d1-127">Também é possível remover uma extensão manualmente, excluindo-a do local onde foi instalada.</span><span class="sxs-lookup"><span data-stu-id="be0d1-127">You can also remove an extension manually by deleting it from the location where it was installed.</span></span> <span data-ttu-id="be0d1-128">Esse será o valor de variável do shell `$AZURE_EXTENSION_DIR`.</span><span class="sxs-lookup"><span data-stu-id="be0d1-128">This will be the value of the `$AZURE_EXTENSION_DIR` shell variable.</span></span> <span data-ttu-id="be0d1-129">Se essa variável tiver sua definição removida, por padrão, o valor é `$HOME/.azure/cliextensions` no Linux e macOS e `%USERPROFILE%\.azure\cliextensions` no Windows.</span><span class="sxs-lookup"><span data-stu-id="be0d1-129">If this variable is unset, by default the value is `$HOME/.azure/cliextensions` on Linux and macOS, and `%USERPROFILE%\.azure\cliextensions` on Windows.</span></span>

```bash
rm -rf $AZURE_EXTENSION_DIR/<extension-name>
```

<span data-ttu-id="be0d1-130">Recomenda-se fazer a desinstalação usando `az extension remove`.</span><span class="sxs-lookup"><span data-stu-id="be0d1-130">It is recommended that you uninstall using `az extension remove`.</span></span>

## <a name="faq"></a><span data-ttu-id="be0d1-131">Perguntas frequentes</span><span class="sxs-lookup"><span data-stu-id="be0d1-131">FAQ</span></span>

<span data-ttu-id="be0d1-132">Aqui estão algumas respostas para outras perguntas comuns sobre extensões da CLI.</span><span class="sxs-lookup"><span data-stu-id="be0d1-132">Here are some answers to other common questions about CLI extensions.</span></span>

### <a name="what-file-formats-are-allowed-for-installation"></a><span data-ttu-id="be0d1-133">Quais formatos de arquivo são permitidos para instalação?</span><span class="sxs-lookup"><span data-stu-id="be0d1-133">What file formats are allowed for installation?</span></span>

<span data-ttu-id="be0d1-134">Atualmente, apenas wheels compilados do Python podem ser instalados como extensões.</span><span class="sxs-lookup"><span data-stu-id="be0d1-134">Currently, only compiled Python wheels can be installed as extensions.</span></span>

### <a name="can-extensions-replace-existing-commands"></a><span data-ttu-id="be0d1-135">As extensões podem substituir os comandos existentes?</span><span class="sxs-lookup"><span data-stu-id="be0d1-135">Can extensions replace existing commands?</span></span>

<span data-ttu-id="be0d1-136">Sim.</span><span class="sxs-lookup"><span data-stu-id="be0d1-136">Yes.</span></span> <span data-ttu-id="be0d1-137">As extensões podem substituir os comandos existentes, mas antes de executar um comando que foi substituído, a CLI emitirá um aviso.</span><span class="sxs-lookup"><span data-stu-id="be0d1-137">Extensions may replace existing commands, but before running a command that has been replaced the CLI will issue a warning.</span></span>

### <a name="how-can-i-tell-if-an-extension-is-in-pre-release"></a><span data-ttu-id="be0d1-138">Como posso saber se uma extensão está em pré-lançamento?</span><span class="sxs-lookup"><span data-stu-id="be0d1-138">How can I tell if an extension is in pre-release?</span></span>

<span data-ttu-id="be0d1-139">Uma extensão deve indicar, por meio de sua própria documentação e controle de versão, se está em pré-lançamento.</span><span class="sxs-lookup"><span data-stu-id="be0d1-139">An extension should indicate through its own documentation and versioning if it is in pre-release.</span></span> <span data-ttu-id="be0d1-140">Também é comum a Microsoft lançar comandos de versão prévia para a CLI como extensões, com planos para movê-las para a interface principal da CLI assim que o produto estiver fora da versão prévia.</span><span class="sxs-lookup"><span data-stu-id="be0d1-140">It is also common for Microsoft to release preview commands for the CLI as extensions, with plans to move them into the main CLI interface once the product is out of preview.</span></span>

### <a name="can-extensions-depend-upon-each-other"></a><span data-ttu-id="be0d1-141">As extensões podem depender umas das outras?</span><span class="sxs-lookup"><span data-stu-id="be0d1-141">Can extensions depend upon each other?</span></span>

<span data-ttu-id="be0d1-142">Nº</span><span class="sxs-lookup"><span data-stu-id="be0d1-142">No.</span></span> <span data-ttu-id="be0d1-143">As extensões devem ser pacotes individuais que não dependem um do outro.</span><span class="sxs-lookup"><span data-stu-id="be0d1-143">Extensions must be individual packages which do not rely on one another.</span></span> <span data-ttu-id="be0d1-144">Isso porque a CLI não oferece nenhuma garantia sobre quando as extensões são carregadas. Assim, não se pode garantir que as dependências sejam atendidas.</span><span class="sxs-lookup"><span data-stu-id="be0d1-144">This is because the CLI gives no guarantee about when extensions are loaded, so dependencies could not be guaranteed to be satisfied.</span></span> <span data-ttu-id="be0d1-145">Ao instalar uma extensão, apenas essa extensão é instalada e ela deve continuar a funcionar mesmo que outras extensões sejam removidas.</span><span class="sxs-lookup"><span data-stu-id="be0d1-145">Installing an extension installs that extension only, and it should continue to work even if you remove other extensions.</span></span>

### <a name="are-extensions-updated-along-with-the-cli"></a><span data-ttu-id="be0d1-146">As extensões são atualizadas juntamente com a CLI?</span><span class="sxs-lookup"><span data-stu-id="be0d1-146">Are extensions updated along with the CLI?</span></span>

<span data-ttu-id="be0d1-147">Nº</span><span class="sxs-lookup"><span data-stu-id="be0d1-147">No.</span></span> <span data-ttu-id="be0d1-148">As extensões devem ser atualizadas separadamente, conforme descrito na seção [Atualizar extensões](#updating-extensions).</span><span class="sxs-lookup"><span data-stu-id="be0d1-148">Extensions must be updated separately, as described in the [Updating extensions](#updating-extensions) section.</span></span>
