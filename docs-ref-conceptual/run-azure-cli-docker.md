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
ms.openlocfilehash: 277d9d3423af4941fb7f7fb57130fa1b7af7d32e
ms.sourcegitcommit: 0e688704889fc88b91588bb6678a933c2d54f020
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/11/2018
ms.locfileid: "44388330"
---
# <a name="run-azure-cli-20-in-a-docker-container"></a>Executar a CLI do Azure 2.0 em um contêiner do Docker

Você pode usar o Docker para executar um contêiner do Linux autônomo com a CLI do Azure 2.0 pré-instalada. O Docker ajuda você a começar rapidamente com um ambiente isolado para executar a CLI. A imagem também pode ser usada como base para suas próprias implantações.

## <a name="run-in-a-docker-container"></a>Executar em um contêiner do Docker

Instalar a CLI usando `docker run`.

   ```bash
   docker run -it microsoft/azure-cli
   ```

> [!NOTE]
> Se você quiser acompanhar as chaves SSH do seu ambiente de usuário, use `-v ${HOME}/.ssh:/root/.ssh` para montar suas chaves SSH no ambiente.
>
> ```bash
> docker run -it -v ${HOME}/.ssh:/root/.ssh microsoft/azure-cli
> ```

A CLI está instalada na imagem como o comando `az` no `/usr/local/bin`. Para entrar, execute o comando [az login](/cli/azure/reference-index#az-login).

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Para saber mais sobre os diferentes métodos de autenticação, consulte [Conectar com a CLI do Azure 2.0](authenticate-azure-cli.md).

## <a name="update-docker-image"></a>Atualizar imagem do Docker

Atualizar com o Docker requer obter a nova imagem e recriar qualquer contêiner existente. Por esse motivo, você deve evitar o uso de um contêiner que hospede a CLI como um armazenamento de dados.

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
