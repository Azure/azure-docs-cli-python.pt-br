---
title: Instalar a CLI do Azure 2.0 no Linux com yum
description: Como instalar a CLI do Azure 2.0 com o yum
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 4b92499d2cb81f64bfbb13215428365711b07874
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/15/2018
---
# <a name="install-azure-cli-20-with-yum"></a>Instalar CLI do Azure 2.0 com o yum

Se você estiver executando uma distribuição que vem com `yum`, como RHEL, Fedora ou CentOS, há um pacote disponível para a CLI do Azure. Este pacote foi testado com RHEL 7, Fedora 19 e posterior e CentOS 7.

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a>Instalar

1. Importe a chave de repositório da Microsoft:

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. Crie informações sobre o repositório do `azure-cli` local:

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. Atualize o índice de pacote do `yum` e instale:

   ```bash
   yum check-update
   sudo yum install azure-cli
   ```

Execute a CLI do Azure com o comando `az`.

## <a name="update"></a>Atualizar

Atualize a CLI do Azure com o comando `yum update`.

```bash
yum check-update
sudo yum update azure-cli
```

## <a name="uninstall"></a>Desinstalar

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. Remova o pacote do seu sistema.

   ```bash
   sudo yum remove azure-cli
   ```

2. Se você não pretende reinstalar a CLI, remova as informações do repositório.

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. Se você removeu as informações do repositório, remova também a chave de assinatura do Microsoft GPG.

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```
