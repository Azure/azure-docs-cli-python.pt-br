---
title: Modo interativo da CLI 2.0 do Azure
description: Use a CLI 2.0 do Azure no modo interativo.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: f07689a323314c076f1eb2a8844875d9543d4b2e
ms.sourcegitcommit: 0e688704889fc88b91588bb6678a933c2d54f020
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/11/2018
ms.locfileid: "44388568"
---
# <a name="interactive-azure-cli-20"></a><span data-ttu-id="c7d8d-103">CLI 2.0 interativa do Azure</span><span class="sxs-lookup"><span data-stu-id="c7d8d-103">Interactive Azure CLI 2.0</span></span>

<span data-ttu-id="c7d8d-104">É possível usar a CLI 2.0 do Azure no modo interativo executando o comando `az interactive`.</span><span class="sxs-lookup"><span data-stu-id="c7d8d-104">You can use Azure CLI 2.0 in interactive mode by running the `az interactive` command.</span></span>
<span data-ttu-id="c7d8d-105">Esse modo coloca você em um shell interativo com preenchimento automático, descrições de comando e exemplos.</span><span class="sxs-lookup"><span data-stu-id="c7d8d-105">This mode places you in an interactive shell with auto-completion, command descriptions, and examples.</span></span>

![modo interativo](./media/interactive-azure-cli/webapp-create.png)

> [!NOTE]
> <span data-ttu-id="c7d8d-107">Não estamos usando o estilo padrão aqui, que não apresenta boa legibilidade em uma tela de fundo preta.</span><span class="sxs-lookup"><span data-stu-id="c7d8d-107">We're not using the default style here, which doesn't read as well on a black background.</span></span>

<span data-ttu-id="c7d8d-108">Caso você ainda não esteja conectado à sua conta, use o comando `login`.</span><span class="sxs-lookup"><span data-stu-id="c7d8d-108">If you're not already signed in to your account, use the `login` command.</span></span>

## <a name="configure"></a><span data-ttu-id="c7d8d-109">Configurar</span><span class="sxs-lookup"><span data-stu-id="c7d8d-109">Configure</span></span>

<span data-ttu-id="c7d8d-110">Opcionalmente, o modo interativo exibe descrições de comando, descrições de parâmetro e exemplos de comando.</span><span class="sxs-lookup"><span data-stu-id="c7d8d-110">Interactive mode optionally displays command descriptions, parameter descriptions, and command examples.</span></span>
<span data-ttu-id="c7d8d-111">É possível ativar/desativar as descrições e os exemplos usando `F1`.</span><span class="sxs-lookup"><span data-stu-id="c7d8d-111">Turn descriptions and examples on or off using `F1`.</span></span>

![descrições e exemplos](./media/interactive-azure-cli/descriptions-and-examples.png)

<span data-ttu-id="c7d8d-113">É possível ativar/desativar os padrões de parâmetro usando `F2`.</span><span class="sxs-lookup"><span data-stu-id="c7d8d-113">You can turn the display of parameter defaults on or off using `F2`.</span></span>

![padrões](./media/interactive-azure-cli/defaults.png)

<span data-ttu-id="c7d8d-115">`F3` ativa/desativa a exibição de alguns dos principais gestos.</span><span class="sxs-lookup"><span data-stu-id="c7d8d-115">`F3` toggles the display of some key gestures.</span></span>

![gestos](./media/interactive-azure-cli/gestures.png)

## <a name="scope"></a><span data-ttu-id="c7d8d-117">Escopo</span><span class="sxs-lookup"><span data-stu-id="c7d8d-117">Scope</span></span>

<span data-ttu-id="c7d8d-118">É possível definir o escopo do modo interativo para um grupo específico de comandos como `vm` ou `vm image`.</span><span class="sxs-lookup"><span data-stu-id="c7d8d-118">You can scope your interactive mode to a specific command group like `vm` or `vm image`.</span></span>
<span data-ttu-id="c7d8d-119">Quando você fizer isso, todos os comandos serão interpretados nesse escopo.</span><span class="sxs-lookup"><span data-stu-id="c7d8d-119">When you do, all commands are interpreted in that scope.</span></span>
<span data-ttu-id="c7d8d-120">Será uma abreviação excelente se você estiver fazendo todo o trabalho nesse grupo de comandos.</span><span class="sxs-lookup"><span data-stu-id="c7d8d-120">It's a great shorthand if you're doing all your work in that command group.</span></span>

<span data-ttu-id="c7d8d-121">Em vez de digitar estes comandos:</span><span class="sxs-lookup"><span data-stu-id="c7d8d-121">Instead of typing these commands:</span></span>

```azurecli
az>> vm create -n myVM -g myRG --image UbuntuLTS
az>> vm list -o table
```

<span data-ttu-id="c7d8d-122">É possível definir o escopo para o grupo de comandos da VM e digitar estes comandos:</span><span class="sxs-lookup"><span data-stu-id="c7d8d-122">You can scope to the vm command group and type these commands:</span></span>

```azurecli
az>> %%vm
az vm>> create -n myVM -g myRG --image UbuntuLTS
az vm>>list -o table
```

<span data-ttu-id="c7d8d-123">Também é possível definir o escopo para grupos de comandos de nível inferior.</span><span class="sxs-lookup"><span data-stu-id="c7d8d-123">You can scope to lower-level command groups as well.</span></span>
<span data-ttu-id="c7d8d-124">É possível definir o escopo para `vm image` usando `%%vm image`.</span><span class="sxs-lookup"><span data-stu-id="c7d8d-124">You could scope to `vm image` using `%%vm image`.</span></span>
<span data-ttu-id="c7d8d-125">Nesse caso, como já definimos o escopo para `vm`, usaremos `%%image`.</span><span class="sxs-lookup"><span data-stu-id="c7d8d-125">In this case, since we're already scoped to `vm`, we would use `%%image`.</span></span>

```azurecli
az vm>> %%image
az vm image>>
```

<span data-ttu-id="c7d8d-126">Nesse ponto, podemos mostrar o escopo novamente para `vm` usando `%%..` ou definir o escopo para a raiz com apenas `%%`.</span><span class="sxs-lookup"><span data-stu-id="c7d8d-126">At that point, we can pop the scope back up to `vm` using `%%..`, or we can scope to the root with just `%%`.</span></span>

```azurecli
az vm image>> %%
az>>
```

## <a name="query"></a><span data-ttu-id="c7d8d-127">Consultar</span><span class="sxs-lookup"><span data-stu-id="c7d8d-127">Query</span></span>

<span data-ttu-id="c7d8d-128">É possível executar uma consulta JMESPath nos resultados do último comando executado.</span><span class="sxs-lookup"><span data-stu-id="c7d8d-128">You can execute a JMESPath query on the results of the last command that you executed.</span></span>
<span data-ttu-id="c7d8d-129">Por exemplo, depois de criar uma VM, garanta que ela foi totalmente provisionada.</span><span class="sxs-lookup"><span data-stu-id="c7d8d-129">For example, after you create a VM, you can make sure it has fully provisioned.</span></span>

```azurecli
az>> vm create --name myVM --resource-group myRG --image UbuntuLTS --no-wait
az>> ? [*].provisioningState
```

```output
[
  "Creating"
]
```

<span data-ttu-id="c7d8d-130">Para saber mais sobre como consultar os resultados dos comandos, consulte [Consultar os resultados de comandos com o Azure 2.0](query-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="c7d8d-130">To learn more about querying the results of your commands, see [Query command results with Azure 2.0](query-azure-cli.md).</span></span>

## <a name="bash-commands"></a><span data-ttu-id="c7d8d-131">Comandos Bash</span><span class="sxs-lookup"><span data-stu-id="c7d8d-131">Bash commands</span></span>

<span data-ttu-id="c7d8d-132">É possível executar comandos do Shell sem sair do modo interativo usando `#[cmd]`.</span><span class="sxs-lookup"><span data-stu-id="c7d8d-132">You can run shell commands without leaving interactive mode using `#[cmd]`.</span></span>

```azurecli
az>> #dir
```

## <a name="examples"></a><span data-ttu-id="c7d8d-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c7d8d-133">Examples</span></span>

<span data-ttu-id="c7d8d-134">Alguns comandos trazem vários exemplos.</span><span class="sxs-lookup"><span data-stu-id="c7d8d-134">Some commands have lots of examples.</span></span>
<span data-ttu-id="c7d8d-135">Role para a próxima página de exemplos usando `CTRL-N` e para a página anterior usando `CTRL-Y`.</span><span class="sxs-lookup"><span data-stu-id="c7d8d-135">You can scroll to the next page of examples using `CTRL-N` and the previous page using `CTRL-Y`.</span></span>

![exemplos](./media/interactive-azure-cli/examples.png)

<span data-ttu-id="c7d8d-137">Também examine um exemplo específico usando `::#`.</span><span class="sxs-lookup"><span data-stu-id="c7d8d-137">You can also look at a specific example using `::#`.</span></span>

```azurecli
az>> vm create ::8
```
