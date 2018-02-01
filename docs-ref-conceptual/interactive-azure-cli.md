---
title: Modo interativo da CLI 2.0 do Azure
description: Use a CLI 2.0 do Azure no modo interativo.
keywords: CLI 2.0 do Azure, modo interativo
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 04/06/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 
ms.openlocfilehash: fb260d7385728acd0c699488ecb5b108afefd08c
ms.sourcegitcommit: dd5b2c7b0b56608ef9ea8730c7dc76e6c532d5ea
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2018
---
# <a name="interactive-azure-cli-20"></a><span data-ttu-id="43a01-104">CLI 2.0 interativa do Azure</span><span class="sxs-lookup"><span data-stu-id="43a01-104">Interactive Azure CLI 2.0</span></span>

<span data-ttu-id="43a01-105">É possível usar a CLI 2.0 do Azure no modo interativo executando o comando `az interactive`.</span><span class="sxs-lookup"><span data-stu-id="43a01-105">You can use Azure CLI 2.0 in interactive mode by running the `az interactive` command.</span></span>
<span data-ttu-id="43a01-106">Isso coloca você em um shell interativo, no qual os comandos são preenchidos automaticamente e você tem acesso a descrições de comandos e a seus parâmetros e exemplos de comando.</span><span class="sxs-lookup"><span data-stu-id="43a01-106">That places you in an interactive shell where your commands are auto-completed and you have access to descriptions of commands and their parameters and command examples.</span></span>

![modo interativo](./media/interactive-azure-cli/webapp-create.png)

> [!NOTE]
> <span data-ttu-id="43a01-108">Não estamos usando o estilo padrão aqui, que não apresenta boa legibilidade em uma tela de fundo preta.</span><span class="sxs-lookup"><span data-stu-id="43a01-108">We're not using the default style here, which doesn't read as well on a black background.</span></span>

<span data-ttu-id="43a01-109">Caso você ainda não esteja conectado à sua conta, use o comando `login` para fazer isso.</span><span class="sxs-lookup"><span data-stu-id="43a01-109">If you're not already logged in to your account, use the `login` command to do that.</span></span>

## <a name="configure"></a><span data-ttu-id="43a01-110">Configurar</span><span class="sxs-lookup"><span data-stu-id="43a01-110">Configure</span></span>

<span data-ttu-id="43a01-111">Opcionalmente, o modo interativo exibe descrições de comando, descrições de parâmetro e exemplos de comando.</span><span class="sxs-lookup"><span data-stu-id="43a01-111">Interactive mode optionally displays command descriptions, parameter descriptions, and command examples.</span></span>
<span data-ttu-id="43a01-112">É possível ativar/desativar as descrições e os exemplos usando `F1`.</span><span class="sxs-lookup"><span data-stu-id="43a01-112">You can turn descriptions and examples on or off using `F1`.</span></span>

![descrições e exemplos](./media/interactive-azure-cli/descriptions-and-examples.png)

<span data-ttu-id="43a01-114">É possível ativar/desativar os padrões de parâmetro usando `F2`.</span><span class="sxs-lookup"><span data-stu-id="43a01-114">You can turn the display of parameter defaults on or off using `F2`.</span></span>

![padrões](./media/interactive-azure-cli/defaults.png)

<span data-ttu-id="43a01-116">`F3` ativa/desativa a exibição de alguns dos principais gestos.</span><span class="sxs-lookup"><span data-stu-id="43a01-116">`F3` toggles the display of some key gestures.</span></span>

![gestos](./media/interactive-azure-cli/gestures.png)

## <a name="scope"></a><span data-ttu-id="43a01-118">Escopo</span><span class="sxs-lookup"><span data-stu-id="43a01-118">Scope</span></span>

<span data-ttu-id="43a01-119">É possível definir o escopo do modo interativo para um grupo específico de comandos como `vm` ou `vm image`.</span><span class="sxs-lookup"><span data-stu-id="43a01-119">You can scope your interactive mode to a specific command group like `vm` or `vm image`.</span></span>
<span data-ttu-id="43a01-120">Quando você fizer isso, todos os comandos serão interpretados nesse escopo.</span><span class="sxs-lookup"><span data-stu-id="43a01-120">When you do, all commands are interpreted in that scope.</span></span>
<span data-ttu-id="43a01-121">Será uma abreviação excelente se você estiver fazendo todo o trabalho nesse grupo de comandos.</span><span class="sxs-lookup"><span data-stu-id="43a01-121">It's a great shorthand if you're doing all your work in that command group.</span></span>

<span data-ttu-id="43a01-122">Em vez de digitar estes comandos:</span><span class="sxs-lookup"><span data-stu-id="43a01-122">Instead of typing these commands:</span></span>

```azurecli
az>> vm create -n myVM -g myRG --image UbuntuLTS
az>> vm list -o table
```

<span data-ttu-id="43a01-123">É possível definir o escopo para o grupo de comandos da VM e digitar estes comandos:</span><span class="sxs-lookup"><span data-stu-id="43a01-123">You can scope to the vm command group and type these commands:</span></span>

```azurecli
az>> %%vm
az vm>> create -n myVM -g myRG --image UbuntuLTS
az vm>>list -o table
```

<span data-ttu-id="43a01-124">Também é possível definir o escopo para grupos de comandos de nível inferior.</span><span class="sxs-lookup"><span data-stu-id="43a01-124">You can scope to lower-level command groups as well.</span></span>
<span data-ttu-id="43a01-125">É possível definir o escopo para `vm image` usando `%%vm image`.</span><span class="sxs-lookup"><span data-stu-id="43a01-125">You could scope to `vm image` using `%%vm image`.</span></span>
<span data-ttu-id="43a01-126">Nesse caso, como já definimos o escopo para `vm`, usaremos `%%image`.</span><span class="sxs-lookup"><span data-stu-id="43a01-126">In this case, since we're already scoped to `vm`, we would use `%%image`.</span></span>

```azurecli
az vm>> %%image
az vm image>>
```

<span data-ttu-id="43a01-127">Nesse ponto, podemos mostrar o escopo novamente para `vm` usando `%%..` ou definir o escopo para a raiz com apenas `%%`.</span><span class="sxs-lookup"><span data-stu-id="43a01-127">At that point, we can pop the scope back up to `vm` using `%%..`, or we can scope to the root with just `%%`.</span></span>

```azurecli
az vm image>> %%
az>>
```

## <a name="query"></a><span data-ttu-id="43a01-128">Consultar</span><span class="sxs-lookup"><span data-stu-id="43a01-128">Query</span></span>

<span data-ttu-id="43a01-129">É possível executar uma consulta JMESPath nos resultados do último comando executado.</span><span class="sxs-lookup"><span data-stu-id="43a01-129">You can execute a JMESPath query on the results of the last command that you executed.</span></span>
<span data-ttu-id="43a01-130">Por exemplo, depois de criar uma VM, garanta que ela foi totalmente provisionada.</span><span class="sxs-lookup"><span data-stu-id="43a01-130">For example, after you create a VM, you can make sure it has fully provisioned.</span></span>

```azurecli
az>> vm create --name myVM --resource-group myRG --image UbuntuLTS --no-wait
az>> ? [*].provisioningState
```

```
[
  "Creating"
]
```

<span data-ttu-id="43a01-131">Para saber mais sobre como consultar os resultados dos comandos, consulte [Consultar os resultados de comandos com o Azure 2.0](query-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="43a01-131">To learn more about querying the results of your commands, see [Query command results with Azure 2.0](query-azure-cli.md).</span></span>

## <a name="bash-commands"></a><span data-ttu-id="43a01-132">Comandos Bash</span><span class="sxs-lookup"><span data-stu-id="43a01-132">Bash commands</span></span>

<span data-ttu-id="43a01-133">É possível executar comandos do Shell sem sair do modo interativo usando `#[cmd]`.</span><span class="sxs-lookup"><span data-stu-id="43a01-133">You can run shell commands without leaving interactive mode using `#[cmd]`.</span></span>

```azurecli
az>> #dir
```

## <a name="examples"></a><span data-ttu-id="43a01-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="43a01-134">Examples</span></span>

<span data-ttu-id="43a01-135">Alguns comandos trazem vários exemplos.</span><span class="sxs-lookup"><span data-stu-id="43a01-135">Some commands have lots of examples.</span></span>
<span data-ttu-id="43a01-136">Role para a próxima página de exemplos usando `CTRL-N` e para a página anterior usando `CTRL-Y`.</span><span class="sxs-lookup"><span data-stu-id="43a01-136">You can scroll to the next page of examples using `CTRL-N` and the previous page using `CTRL-Y`.</span></span>

![exemplos](./media/interactive-azure-cli/examples.png)

<span data-ttu-id="43a01-138">Também examine um exemplo específico usando `::#`.</span><span class="sxs-lookup"><span data-stu-id="43a01-138">You can also look at a specific example using `::#`.</span></span>

```azurecli
az>> vm create ::8
```
