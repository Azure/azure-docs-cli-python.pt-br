---
title: Instalar a CLI do Azure 2.0 no Linux com zypper
description: Como instalar a CLI do Azure 2.0 com o zypper
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 01/29/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 3a1e82dc666cd034d0cc4320a8b99dd6a9a14b6d
ms.sourcegitcommit: ae72b6c8916aeb372a92188090529037e63930ba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2018
---
# <a name="install-azure-cli-20-with-zypper"></a>Instalar CLI do Azure 2.0 com zypper

Se você estiver executando uma distribuição que vem com `zypper`, como o openSUSE ou SLES, há um pacote disponível para a CLI do Azure. Este pacote foi testado com openSUSE 42.2 e SLES 12 SP 2.

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a>Instalar

1. Instale `curl`:

   ```bash
   sudo zypper refresh
   sudo zypper install -y curl
   ```

2. Importe a chave de repositório da Microsoft:

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

3. Crie informações sobre o repositório do `azure-cli` local:

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ntype=rpm-md\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/zypp/repos.d/azure-cli.repo'
   ```

4. Atualize o índice de pacote do `zypper` e instale:

   ```bash
   sudo zypper refresh
   sudo zypper install -y azure-cli
   ```

É possível executar a CLI do Azure com o comando `az`. Para fazer logon, execute o comando `az login`.

```azurecli
az login
```

Para saber mais sobre os métodos de logon diferente, consulte [Fazer logon com a CLI do Azure 2.0](authenticate-azure-cli.md).

## <a name="update"></a>Atualizar

Você pode atualizar o pacote com o comando `zypper update`.

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

## <a name="uninstall"></a>Desinstalar

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. Remova o pacote do seu sistema.

    ```bash
    sudo zypper remove -y azure-cli
    ```

2. Se você não pretende reinstalar a CLI, remova as informações do repositório.

  ```bash
  sudo rm /etc/zypp/repos.d/azure-cli.repo
  ```

3. Se você removeu as informações do repositório, remova também a chave de assinatura do Microsoft GPG.

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```

