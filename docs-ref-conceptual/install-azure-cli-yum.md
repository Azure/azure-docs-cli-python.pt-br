---
title: Instalar a CLI do Azure 2.0 no Linux com yum
description: Como instalar a CLI do Azure 2.0 com o yum
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 25eb473aa56d3ddd34f8e1808b84ebb5f6324f2b
ms.sourcegitcommit: d93b0a2bcfb0d164ef90d6d4618f0552609a8ea6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/20/2018
ms.locfileid: "46470007"
---
# <a name="install-azure-cli-20-with-yum"></a>Instalar CLI do Azure 2.0 com o yum

Para distribuições Linux com `yum`, como o RHEL, Fedora ou CentOS há um pacote para a CLI do Azure. Este pacote foi testado com RHEL 7, Fedora 19 e posterior e CentOS 7.

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a>Instalar

1. Importe a chave do repositório da Microsoft.

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. Crie informações sobre o repositório do local `azure-cli`.

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. Instale com o comando `yum install`.

   ```bash
   sudo yum install azure-cli
   ```

É possível executar a CLI do Azure com o comando `az`. Para entrar, use o comando [az login](/cli/azure/reference-index#az-login).

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Para saber mais sobre os diferentes métodos de autenticação, consulte [Conectar com a CLI do Azure 2.0](authenticate-azure-cli.md).

## <a name="update"></a>Atualizar

Atualize a CLI do Azure com o comando `yum update`.

```bash
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

## <a name="next-steps"></a>Próximas etapas

Agora que você instalou a CLI do Azure, faça um tour breve de seus recursos e comandos comuns.

> [!div class="nextstepaction"]
> [Introdução à CLI do Azure](get-started-with-azure-cli.md)
