---
title: Instalar a CLI do Azure 2.0 no Linux com zypper
description: Como instalar a CLI do Azure 2.0 com o zypper
keywords: cli do azure, instalar cli do azure, zypper cli do azure, opensuse cli do azure, sle cli do azure
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/18
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: c0b566f96e47d34d20f7bf85db0fae32913ed596
ms.sourcegitcommit: 8606f36963e8daa6448d637393d1e4ef2c9859a0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/01/2018
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

É possível executar a CLI com o comando `az`.

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

