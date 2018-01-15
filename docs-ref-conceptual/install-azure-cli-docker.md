---
title: Instalar a CLI do Azure com o Docker
description: "Como instalar um contêiner do Docker com a CLI do Azure 2.0"
keywords: CLI do Azure, Instalar CLI do Azure, docker do azure, imagem do docker do azure,
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 10/30/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ROBOTS: NOINDEX,NOFOLLOW
ms.openlocfilehash: 76ecf2c9cd0e6e694a31ac160112d1348863f118
ms.sourcegitcommit: 3eef136ae752eb90c67af604d4ddd298d70b1c9d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/06/2018
---
# <a name="install-azure-cli-20-with-docker"></a>Instalar CLI do Azure 2.0 com o Docker

Você pode usar o Docker para instalar um contêiner do Linux autônomo com a CLI do Azure 2.0 pré-instalada. Permite que você inicie rapidamente com um ambiente no qual pode experimentar a CLI para decidir se é ideal para você ou permite que use isso como uma imagem de base.

## <a name="install-with-docker"></a>Instalar com o Docker

Instalar a CLI usando `docker run`.

   ```bash
   docker run -it azuresdk/azure-cli-python:<version>
   ```

Confira nossas [marcas do Docker](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/) para versões disponíveis.

A CLI está instalada na imagem como o comando `az` no `/usr/local/bin`.

> [!NOTE]
> Se você quiser acompanhar as chaves SSH do seu ambiente de usuário, use `-v ${HOME}:/root` para montar $HOME como `/root`.

> ```bash
> docker run -it -v ${HOME}:/root azuresdk/azure-cli-python:<version>
> ```

### <a name="update-with-docker"></a>Atualizar com o Docker

Atualizar com o Docker requer obter a nova imagem e recriar qualquer contêiner existente. Por esse motivo, você deve evitar o uso de um contêiner que hospeda a CLI como um armazenamento de dados.

1. Atualizar sua imagem local com `docker pull`.

   ```bash
   docker pull azuresdk/azure-cli-python
   ```

2. Obter os contêineres atuais usando a imagem CLI.

   ```bash
   docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```

  > [!NOTE]
  > Se você instalou uma versão específica da imagem, você precisará adicionar `:<version>` ao final do nome da imagem.

3. Interromper e recriar os contêineres.

   ```bash
   docker stop inspiring_benz
   docker rm inspiring_benz
   docker run azuresdk/azure-cli-python
   ```

### <a name="uninstall-with-docker"></a>Desinstalar com o Docker

Se você decidiu desinstalar a CLI do Azure, lamentamos sua saída. Antes de desinstalar, use o comando `az feedback` para nos fornecer algumas razões por ter escolhido desinstalar e como poderíamos melhorar a experiência da CLI. Queremos assegurar que a CLI do Azure não tenha bugs e seja amigável o máximo possível. Você também pode [registrar um problema do github](https://github.com/Azure/azure-cli/issues).

Para desinstalar corretamente a imagem do Docker da CLI, precisará remover qualquer contêiner que o executa e excluir a imagem do local.

1. Obtenha os contêineres que executam a imagem azure-cli.

   ```bash
   docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```
  > [!NOTE]
  > Se você instalou uma versão específica da imagem, você precisará adicionar `:<version>` ao final do nome da imagem.

2. Exclua todos os contêineres com a imagem da CLI.

   ```bash
   docker rm 34a868beb2ab
   ```

3. Remova a imagem da CLI instalada localmente.

   ```bash
   docker rmi azuresdk/azure-cli-python
   ```

