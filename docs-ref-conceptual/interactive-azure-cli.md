---
title: Modo interativo da CLI do Azure
description: Use a CLI do Azure no modo interativo.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/09/2018
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 7b3ee1e284e7f771c661bb65bf8b8ab53dafd77f
ms.sourcegitcommit: 7caa6673f65e61deb8d6def6386e4eb9acdac923
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/28/2020
ms.locfileid: "77779509"
---
# <a name="azure-cli-interactive-mode"></a><span data-ttu-id="c1f05-103">Modo interativo da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="c1f05-103">Azure CLI interactive mode</span></span>

<span data-ttu-id="c1f05-104">É possível usar a CLI do Azure no modo interativo executando o comando `az interactive`.</span><span class="sxs-lookup"><span data-stu-id="c1f05-104">You can use Azure CLI in interactive mode by running the `az interactive` command.</span></span>
<span data-ttu-id="c1f05-105">Esse modo coloca você em um shell interativo com preenchimento automático, descrições de comando e exemplos.</span><span class="sxs-lookup"><span data-stu-id="c1f05-105">This mode places you in an interactive shell with auto-completion, command descriptions, and examples.</span></span>

![modo interativo](./media/interactive-azure-cli/webapp-create.png)

> [!NOTE]
> <span data-ttu-id="c1f05-107">Não estamos usando o estilo padrão aqui, que não apresenta boa legibilidade em uma tela de fundo preta.</span><span class="sxs-lookup"><span data-stu-id="c1f05-107">We're not using the default style here, which doesn't read as well on a black background.</span></span>

<span data-ttu-id="c1f05-108">Caso você ainda não esteja conectado à sua conta, use o comando `login`.</span><span class="sxs-lookup"><span data-stu-id="c1f05-108">If you're not already signed in to your account, use the `login` command.</span></span>

## <a name="configure"></a><span data-ttu-id="c1f05-109">Configurar</span><span class="sxs-lookup"><span data-stu-id="c1f05-109">Configure</span></span>

<span data-ttu-id="c1f05-110">Opcionalmente, o modo interativo exibe descrições de comando, descrições de parâmetro e exemplos de comando.</span><span class="sxs-lookup"><span data-stu-id="c1f05-110">Interactive mode optionally displays command descriptions, parameter descriptions, and command examples.</span></span>
<span data-ttu-id="c1f05-111">É possível ativar/desativar as descrições e os exemplos usando `F1`.</span><span class="sxs-lookup"><span data-stu-id="c1f05-111">Turn descriptions and examples on or off using `F1`.</span></span>

![descrições e exemplos](./media/interactive-azure-cli/descriptions-and-examples.png)

<span data-ttu-id="c1f05-113">É possível ativar/desativar os padrões de parâmetro usando `F2`.</span><span class="sxs-lookup"><span data-stu-id="c1f05-113">You can turn the display of parameter defaults on or off using `F2`.</span></span>

![padrões](./media/interactive-azure-cli/defaults.png)

<span data-ttu-id="c1f05-115">`F3` ativa/desativa a exibição de alguns dos principais gestos.</span><span class="sxs-lookup"><span data-stu-id="c1f05-115">`F3` toggles the display of some key gestures.</span></span>

![gestos](./media/interactive-azure-cli/gestures.png)

## <a name="scope"></a><span data-ttu-id="c1f05-117">Escopo</span><span class="sxs-lookup"><span data-stu-id="c1f05-117">Scope</span></span>

<span data-ttu-id="c1f05-118">É possível definir o escopo do modo interativo para um grupo específico de comandos como `vm` ou `vm image`.</span><span class="sxs-lookup"><span data-stu-id="c1f05-118">You can scope your interactive mode to a specific command group like `vm` or `vm image`.</span></span>
<span data-ttu-id="c1f05-119">Quando você fizer isso, todos os comandos serão interpretados nesse escopo.</span><span class="sxs-lookup"><span data-stu-id="c1f05-119">When you do, all commands are interpreted in that scope.</span></span>
<span data-ttu-id="c1f05-120">Será uma abreviação excelente se você estiver fazendo todo o trabalho nesse grupo de comandos.</span><span class="sxs-lookup"><span data-stu-id="c1f05-120">It's a great shorthand if you're doing all your work in that command group.</span></span>

<span data-ttu-id="c1f05-121">Em vez de digitar estes comandos:</span><span class="sxs-lookup"><span data-stu-id="c1f05-121">Instead of typing these commands:</span></span>

```azurecli
az>> vm create -n myVM -g myRG --image UbuntuLTS
az>> vm list -o table
```

<span data-ttu-id="c1f05-122">É possível definir o escopo para o grupo de comandos da VM e digitar estes comandos:</span><span class="sxs-lookup"><span data-stu-id="c1f05-122">You can scope to the vm command group and type these commands:</span></span>

```azurecli
az>> %%vm
az vm>> create -n myVM -g myRG --image UbuntuLTS
az vm>>list -o table
```

<span data-ttu-id="c1f05-123">Também é possível definir o escopo para grupos de comandos de nível inferior.</span><span class="sxs-lookup"><span data-stu-id="c1f05-123">You can scope to lower-level command groups as well.</span></span>
<span data-ttu-id="c1f05-124">É possível definir o escopo para `vm image` usando `%%vm image`.</span><span class="sxs-lookup"><span data-stu-id="c1f05-124">You could scope to `vm image` using `%%vm image`.</span></span>
<span data-ttu-id="c1f05-125">Nesse caso, como já definimos o escopo para `vm`, usaremos `%%image`.</span><span class="sxs-lookup"><span data-stu-id="c1f05-125">In this case, since we're already scoped to `vm`, we would use `%%image`.</span></span>

```azurecli
az vm>> %%image
az vm image>>
```

<span data-ttu-id="c1f05-126">Nesse ponto, podemos mostrar o escopo novamente para `vm` usando `%%..` ou definir o escopo para a raiz com apenas `%%`.</span><span class="sxs-lookup"><span data-stu-id="c1f05-126">At that point, we can pop the scope back up to `vm` using `%%..`, or we can scope to the root with just `%%`.</span></span>

```azurecli
az vm image>> %%
az>>
```

## <a name="query"></a><span data-ttu-id="c1f05-127">Consulta</span><span class="sxs-lookup"><span data-stu-id="c1f05-127">Query</span></span>

<span data-ttu-id="c1f05-128">É possível executar uma consulta JMESPath nos resultados do último comando executado usando `??` seguido de uma consulta JMESPath.</span><span class="sxs-lookup"><span data-stu-id="c1f05-128">You can execute a JMESPath query on the results of the last command that you executed by using `??`followed by a JMESPath query.</span></span>
<span data-ttu-id="c1f05-129">Por exemplo, depois de criar um grupo, você pode recuperar a ID do novo grupo.</span><span class="sxs-lookup"><span data-stu-id="c1f05-129">For example, after you created a group, you can retrieve the id of the new group.</span></span>

```azurecli
az>> group create -n myRG -l westEurope
az>> "?? id"
```

<span data-ttu-id="c1f05-130">Você também pode aproveitar essa sintaxe para usar o resultado do comando anterior como um argumento do próximo comando.\* Por exemplo, depois de ter listado todos os grupos, liste todos os recursos do tipo `virtualMachine` no primeiro grupo cuja localização seja westeurope.</span><span class="sxs-lookup"><span data-stu-id="c1f05-130">You can also use this syntax to use the result of the previous command as an argument for your next command.\* For instance after having listed all groups, list all the resources of type `virtualMachine`on the first group whose location is westeurope.</span></span> 

```azurecli
az>> vm create --name myVM --resource-group myRG --image UbuntuLTS --no-wait -o json
az>> group list -o json
az>> resource list -g "?? [?location=='westeurope'].name | [0]" --query "[?type=='Microsoft.Compute/virtualMachines'].name
```

<span data-ttu-id="c1f05-131">Para saber mais sobre como consultar os resultados dos comandos, confira [Consultar os resultados de comandos com a CLI do Azure](query-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="c1f05-131">To learn more about querying the results of your commands, see [Query command results with the Azure CLI](query-azure-cli.md).</span></span>

## <a name="bash-commands"></a><span data-ttu-id="c1f05-132">Comandos Bash</span><span class="sxs-lookup"><span data-stu-id="c1f05-132">Bash commands</span></span>

<span data-ttu-id="c1f05-133">É possível executar comandos do Shell sem sair do modo interativo usando `#[cmd]`.</span><span class="sxs-lookup"><span data-stu-id="c1f05-133">You can run shell commands without leaving interactive mode using `#[cmd]`.</span></span>

```azurecli
az>> #dir
```

## <a name="examples"></a><span data-ttu-id="c1f05-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c1f05-134">Examples</span></span>

<span data-ttu-id="c1f05-135">Alguns comandos trazem vários exemplos.</span><span class="sxs-lookup"><span data-stu-id="c1f05-135">Some commands have lots of examples.</span></span>
<span data-ttu-id="c1f05-136">Role para a próxima página de exemplos usando `CTRL-N` e para a página anterior usando `CTRL-Y`.</span><span class="sxs-lookup"><span data-stu-id="c1f05-136">You can scroll to the next page of examples using `CTRL-N` and the previous page using `CTRL-Y`.</span></span>

![exemplos](./media/interactive-azure-cli/examples.png)

<span data-ttu-id="c1f05-138">Também examine um exemplo específico usando `::#`.</span><span class="sxs-lookup"><span data-stu-id="c1f05-138">You can also look at a specific example using `::#`.</span></span>

```azurecli
az>> vm create ::8
```
