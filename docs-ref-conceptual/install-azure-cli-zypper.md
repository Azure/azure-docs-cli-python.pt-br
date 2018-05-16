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
ms.sourcegitcommit: 15d6dfaee2075d0abceb2aa2423f0b6ef7b2ac9b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2018
---

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
   sudo zypper install --from azure-cli -y azure-cli
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

