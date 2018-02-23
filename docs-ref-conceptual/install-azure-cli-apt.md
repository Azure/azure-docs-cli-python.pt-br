---
title: Instalar a CLI do Azure 2.0 no Linux com apt
description: Como instalar a CLI do Azure 2.0 com o gerenciador de pacotes apt
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 02/06/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 4076fefb902a324f77f97bc042b9f5ba3e787734
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/15/2018
---
# <a name="install-azure-cli-20-with-apt"></a>Instalar CLI do Azure 2.0 com o apt

Se você estiver executando uma distribuição que venha com o `apt`, como o Ubuntu ou Debian, há um pacote 64-bit disponível para a CLI do Azure. Esse pacote foi testado com:

* Ubuntu wheezy, xenial e artful
* Debian wheezy, jessie e stretch

## <a name="install"></a>Instalar

1. Modifique sua lista de fontes:

     ```bash
     AZ_REPO=$(lsb_release -cs)
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. Execute os comandos sudo a seguir:

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

É possível executar a CLI do Azure com o comando `az`.

## <a name="troubleshooting"></a>solução de problemas

Aqui estão alguns problemas comuns vistos durante a instalação com `apt`. Se o problema não estiver listado aqui, [registre um problema no github](https://github.com/Azure/azure-cli/issues).

### <a name="apt-key-fails-with-no-dirmngr"></a>A apt-key falha com “Sem dirmngr”

Ao executar o comando `apt-key`, pode ser que você veja uma saída semelhante ao seguinte erro:

```output
gpg: failed to start the dirmngr '/usr/bin/dirmngr': No such file or directory
gpg: connecting dirmngr at '/tmp/apt-key-gpghome.kt5zo27tp1/S.dirmngr' failed: No such file or directory
gpg: keyserver receive failed: No dirmngr
```

O erro ocorre devido a um componente ausente exigido por `apt-key`. Você pode resolver isso instalando o pacote `dirmngr`.

```bash
sudo apt-get install dirmngr
```

## <a name="update"></a>Atualizar

Use `apt-get upgrade` para atualizar o pacote da CLI.

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> Esse comando atualiza todos os pacotes instalados no seu sistema que não tiveram uma alteração de dependência.
> Para atualizar apenas a CLI, use `apt-get install`.
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a>Desinstalar

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

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
