---
title: Execute a CLI do Azure 2.0 em um Contêiner do Docker
description: Como executar um contêiner do Docker hospedando a CLI do Azure 2.0
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 01/29/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: d88dbcec947372aa154bce939edd99f65cd9480f
ms.sourcegitcommit: ae72b6c8916aeb372a92188090529037e63930ba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2018
---
# <a name="run-azure-cli-20-in-a-docker-container"></a>Executar a CLI do Azure 2.0 em um contêiner do Docker

Você pode usar o Docker para executar um contêiner do Linux autônomo com a CLI do Azure 2.0 pré-instalada. O Docker permite que você inicie rapidamente com um ambiente no qual você pode experimentar a CLI para decidir se é ideal para você ou usar nossa imagem como uma base para sua própria implantação.

## <a name="run-in-a-docker-container"></a>Executar em um contêiner do Docker

Instalar a CLI usando `docker run`.

   ```bash
   docker run -it microsoft/azure-cli
   ```

A CLI está instalada na imagem como o comando `az` no `/usr/local/bin`. Para fazer logon, execute o comando `az login`.

```azurecli
az login
```

Para saber mais sobre os métodos de logon diferente, consulte [Fazer logon com a CLI do Azure 2.0](authenticate-azure-cli.md).

> [!NOTE]
> Se você quiser acompanhar as chaves SSH do seu ambiente de usuário, use `-v ${HOME}:/root` para montar $HOME como `/root`.

> ```bash
> docker run -it -v ${HOME}:/root microsoft/azure-cli
> ```

## <a name="update-docker-image"></a>Atualizar imagem do Docker

Atualizar com o Docker requer obter a nova imagem e recriar qualquer contêiner existente. Por esse motivo, você deve evitar o uso de um contêiner que hospeda a CLI como um armazenamento de dados.

Atualizar sua imagem local com `docker pull`.

```bash
docker pull microsoft/azure-cli
```

## <a name="uninstall-docker-image"></a>Desinstalar imagem do Docker

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

Depois de parar qualquer contêiner executando a imagem da CLI, remova-o.

```bash
docker rmi microsoft/azure-cli
```
