---
title: Instalar a CLI do Azure 2.0 com o apt
description: Como instalar a CLI do Azure 2.0 com o gerenciador de pacotes apt
keywords: CLI do Azure, Instalar CLI do Azure, apt do azure, debian do azure, ubuntu do azure
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 11/01/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ROBOTS: NOINDEX,NOFOLLOW
ms.openlocfilehash: 75c531a13a4b730158cd2e874cb6c5d581a27598
ms.sourcegitcommit: 2e4d0bdd94c626e061434883032367b5619de4fe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2017
---
# <a name="install-azure-cli-20-with-apt"></a>Instalar CLI do Azure 2.0 com o apt

Se você estiver executando uma distribuição que vem com o `apt`, como o Ubuntu ou Debian, há um pacote disponível para a CLI do Azure que pode ser instalado em seu sistema.

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a>Instalar

1. Modifique sua lista de fontes:

   - sistema de 32 bits

     ```bash
     echo "deb https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

   - sistema de 64 bits

     ```bash
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. Execute os comandos sudo a seguir:

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

É possível executar a CLI do Azure com o comando `az`.

## <a name="update"></a>Atualização

Use `apt-get upgrade` para atualizar o pacote da CLI.

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> Isso atualizará todos os pacotes instalados no sistema que não tiveram uma alteração de dependência.
> Para atualizar somente a CLI, use `apt-get install`.
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

### <a name="uninstall"></a>Desinstalar

Se você decidiu desinstalar a CLI do Azure, lamentamos sua saída. Antes de desinstalar, use o comando `az feedback` para nos fornecer algumas razões por ter escolhido desinstalar e como poderíamos melhorar a experiência da CLI. Queremos assegurar que a CLI do Azure não tenha bugs e seja amigável o máximo possível. Você também pode [registrar um problema do github](https://github.com/Azure/azure-cli/issues).

1. Desinstalar com `apt-get remove`.

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. Se você não pretende reinstalar a CLI, remova as informações do repositório da CLI do Azure.

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. Remova quaisquer pacotes desnecessários.

   ```bash
   sudo apt autoremove
   ```
