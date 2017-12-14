---
title: Instalar a CLI do Azure 2.0 com o yum
description: Como instalar a CLI do Azure 2.0 com o yum
keywords: CLI do Azure, Instalar CLI do Azure, yum do azure, rhel do azure, fedora do azure, centos do azure
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
ms.openlocfilehash: f0d5effcd8315094b30050a35119e41eddf89961
ms.sourcegitcommit: 2e4d0bdd94c626e061434883032367b5619de4fe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2017
---
# <a name="install-azure-cli-20-with-yum"></a>Instalar CLI do Azure 2.0 com o yum

Se você estiver executando uma distribuição que vem com o `yum`, como o RHEL, Fedora ou CentOS, há um pacote disponível para a CLI do Azure que pode ser instalado em seu sistema.

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

## <a name="update"></a>Atualização

Atualize a CLI do Azure com o comando `yum update`.

```bash
yum check-update
sudo yum update azure-cli
```

## <a name="uninstall"></a>Desinstalar

Se você decidiu desinstalar a CLI do Azure, lamentamos sua saída. Antes de desinstalar, use o comando `az feedback` para nos fornecer algumas razões por ter escolhido desinstalar e como poderíamos melhorar a experiência da CLI. Queremos assegurar que a CLI do Azure não tenha bugs e seja amigável o máximo possível. Você também pode [registrar um problema do github](https://github.com/Azure/azure-cli/issues).

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
