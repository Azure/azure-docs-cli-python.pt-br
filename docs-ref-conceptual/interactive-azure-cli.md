---
title: Modo interativo da CLI 2.0 do Azure
description: Use a CLI 2.0 do Azure no modo interativo.
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 04/06/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 0d32b7a1e754ba28ec1722fe4bf80e5f36b031e2
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/15/2018
---
# <a name="interactive-azure-cli-20"></a>CLI 2.0 interativa do Azure

É possível usar a CLI 2.0 do Azure no modo interativo executando o comando `az interactive`.
Isso coloca você em um shell interativo, no qual os comandos são preenchidos automaticamente e você tem acesso a descrições de comandos e a seus parâmetros e exemplos de comando.

![modo interativo](./media/interactive-azure-cli/webapp-create.png)

> [!NOTE]
> Não estamos usando o estilo padrão aqui, que não apresenta boa legibilidade em uma tela de fundo preta.

Caso você ainda não esteja conectado à sua conta, use o comando `login` para fazer isso.

## <a name="configure"></a>Configurar

Opcionalmente, o modo interativo exibe descrições de comando, descrições de parâmetro e exemplos de comando.
É possível ativar/desativar as descrições e os exemplos usando `F1`.

![descrições e exemplos](./media/interactive-azure-cli/descriptions-and-examples.png)

É possível ativar/desativar os padrões de parâmetro usando `F2`.

![padrões](./media/interactive-azure-cli/defaults.png)

`F3` ativa/desativa a exibição de alguns dos principais gestos.

![gestos](./media/interactive-azure-cli/gestures.png)

## <a name="scope"></a>Escopo

É possível definir o escopo do modo interativo para um grupo específico de comandos como `vm` ou `vm image`.
Quando você fizer isso, todos os comandos serão interpretados nesse escopo.
Será uma abreviação excelente se você estiver fazendo todo o trabalho nesse grupo de comandos.

Em vez de digitar estes comandos:

```azurecli
az>> vm create -n myVM -g myRG --image UbuntuLTS
az>> vm list -o table
```

É possível definir o escopo para o grupo de comandos da VM e digitar estes comandos:

```azurecli
az>> %%vm
az vm>> create -n myVM -g myRG --image UbuntuLTS
az vm>>list -o table
```

Também é possível definir o escopo para grupos de comandos de nível inferior.
É possível definir o escopo para `vm image` usando `%%vm image`.
Nesse caso, como já definimos o escopo para `vm`, usaremos `%%image`.

```azurecli
az vm>> %%image
az vm image>>
```

Nesse ponto, podemos mostrar o escopo novamente para `vm` usando `%%..` ou definir o escopo para a raiz com apenas `%%`.

```azurecli
az vm image>> %%
az>>
```

## <a name="query"></a>Consultar

É possível executar uma consulta JMESPath nos resultados do último comando executado.
Por exemplo, depois de criar uma VM, garanta que ela foi totalmente provisionada.

```azurecli
az>> vm create --name myVM --resource-group myRG --image UbuntuLTS --no-wait
az>> ? [*].provisioningState
```

```
[
  "Creating"
]
```

Para saber mais sobre como consultar os resultados dos comandos, consulte [Consultar os resultados de comandos com o Azure 2.0](query-azure-cli.md).

## <a name="bash-commands"></a>Comandos Bash

É possível executar comandos do Shell sem sair do modo interativo usando `#[cmd]`.

```azurecli
az>> #dir
```

## <a name="examples"></a>Exemplos

Alguns comandos trazem vários exemplos.
Role para a próxima página de exemplos usando `CTRL-N` e para a página anterior usando `CTRL-Y`.

![exemplos](./media/interactive-azure-cli/examples.png)

Também examine um exemplo específico usando `::#`.

```azurecli
az>> vm create ::8
```
