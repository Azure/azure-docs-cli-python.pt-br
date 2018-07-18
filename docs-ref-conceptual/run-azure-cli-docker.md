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
ms.openlocfilehash: 65d8140bd12a260c127efa2adb064c2f9294810b
ms.sourcegitcommit: 64f2c628e83d687d0e172c01f13d71c8c39a8040
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/11/2018
ms.locfileid: "38967768"
---
# <a name="run-azure-cli-20-in-a-docker-container"></a>Executar a CLI do Azure 2.0 em um contêiner do Docker

Você pode usar o Docker para executar um contêiner do Linux autônomo com a CLI do Azure 2.0 pré-instalada. O Docker permite que você inicie rapidamente com um ambiente no qual você pode experimentar a CLI para decidir se é ideal para você ou usar nossa imagem como uma base para sua própria implantação.

## <a name="run-in-a-docker-container"></a>Executar em um contêiner do Docker

Instalar a CLI usando `docker run`.

   ```bash
   docker run -it microsoft/azure-cli
   ```

> [!NOTE]
> Se você quiser acompanhar as chaves SSH do seu ambiente de usuário, use `-v ${HOME}:/root` para montar $HOME como `/root`.
>
> ```bash
> docker run -it -v ${HOME}:/root microsoft/azure-cli
> ```

A CLI está instalada na imagem como o comando `az` no `/usr/local/bin`. Para entrar, execute o comando [az login](/cli/azure/reference-index#az-login).

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Para saber mais sobre os diferentes métodos de autenticação, consulte [Conectar com a CLI do Azure 2.0](authenticate-azure-cli.md).

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
