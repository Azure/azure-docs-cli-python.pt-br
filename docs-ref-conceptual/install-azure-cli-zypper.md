---
title: Instalar a CLI do Azure no Linux com zypper
description: Como instalar a CLI do Azure com o zypper
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/09/2018
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: b06d1f9b97bb4ad8b569f608175754020f548642
ms.sourcegitcommit: d056d09dd6268b8d70ca65303a3ebf640a8d4b26
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/03/2020
ms.locfileid: "85938124"
---
# <a name="install-azure-cli-with-zypper"></a>Instalar CLI do Azure com zypper

Para distribuições Linux com `zypper`, como o openSUSE ou SLES, há um pacote disponível para a CLI do Azure. Este pacote foi testado com openSUSE Leap 15.1 e SLES 15.

[!INCLUDE [current-version](includes/current-version.md)]

[!INCLUDE [rpm-warning](includes/rpm-warning.md)]

## <a name="install"></a>Instalar

1. Instale `curl`:

   ```bash
   sudo zypper install -y curl
   ```

2. Importe a chave de repositório da Microsoft:

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

3. Crie informações sobre o repositório do `azure-cli` local:

   ```bash
   sudo zypper addrepo --name 'Azure CLI' --check https://packages.microsoft.com/yumrepos/azure-cli azure-cli
   ```

4. Atualize o índice de pacote do `zypper` e instale:

   ```bash
   sudo zypper install --from azure-cli azure-cli
   ```
   Entrada 2 para continuar a instalar, ignorando algumas dependências.

É possível executar a CLI do Azure com o comando `az`. Para entrar, use o comando [az login](/cli/azure/reference-index#az-login).

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Para saber mais sobre os diferentes métodos de autenticação, confira [Entrar com a CLI do Azure](authenticate-azure-cli.md).

## <a name="troubleshooting"></a>Solução de problemas

Aqui estão alguns problemas comuns vistos durante a instalação com `zypper`. Se você tiver um problema não abordado aqui, [arquive um problema no github](https://github.com/Azure/azure-cli/issues).

### <a name="install-on-sles-12-or-other-systems-without-python-36"></a>Instalar no SLES 12 ou em sistemas sem o Python 3.6

No SLES 12, o pacote python3 padrão é 3.4 e não é compatível com a CLI do Azure. É possível criar primeiro uma versão superior do python3 da origem. Em seguida, você poderá baixar o pacote da CLI do Azure e instalá-lo sem dependência.
```bash
$ sudo zypper install -y gcc gcc-c++ make ncurses patch wget tar zlib-devel zlib openssl-devel
# Download Python source code
$ PYTHON_VERSION="3.6.9"
$ PYTHON_SRC_DIR=$(mktemp -d)
$ wget -qO- https://www.python.org/ftp/python/$PYTHON_VERSION/Python-$PYTHON_VERSION.tgz | tar -xz -C "$PYTHON_SRC_DIR"
# Build Python
$ $PYTHON_SRC_DIR/*/configure
$ make
$ sudo make install
#Download azure-cli package 
$ AZ_VERSION=$(zypper --no-refresh info azure-cli |grep Version | awk -F': ' '{print $2}' | awk '{$1=$1;print}')
$ wget https://packages.microsoft.com/yumrepos/azure-cli/azure-cli-$AZ_VERSION.x86_64.rpm
#Install without dependency
$ sudo rpm -ivh --nodeps azure-cli-$AZ_VERSION.x86_64.rpm
```

### <a name="proxy-blocks-connection"></a>Conexão de blocos de proxy

[!INCLUDE[configure-proxy](includes/configure-proxy.md)]

Talvez você queira configurar explicitamente `zypper` (por meio de `yast2`) para usar esse proxy sempre. Para fazer isso, execute o comando `yast2 proxy` como superusuário e preencha as informações apresentadas no formulário. Se você tiver um gerenciador de janelas disponível no sistema, também poderá usar o painel `Network Services > Proxy` no `YaST Control Center`.

Para configurações avançadas ou mais informações, confira a [documentação de configuração do Proxy do OpenSUSE](https://www.suse.com/documentation/slms1/book_slms/data/sec_wy_config_updates_proxy.html)

Para obter a chave de assinatura da Microsoft e o pacote do nosso repositório, o proxy precisa permitir conexões HTTPS com os seguintes endereços:

* `https://packages.microsoft.com`
* `https://download.opensuse.org`

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

### <a name="ssl-certificate-problem"></a>Problema com o certificado SSL

Quando um certificado é inválido ou está desatualizado em um computador, você pode receber um erro indicando que o cURL falhou ao verificar a legitimidade do servidor e, portanto, não foi possível estabelecer uma conexão segura.  Atualize o certificado para corrigir o problema.  

```bach
sudo zypper update-ca-certificates
```

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
   sudo zypper removerepo azure-cli
   ```

3. Se você não usa outros pacotes da Microsoft, remova a chave de assinatura da Microsoft.

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```

## <a name="next-steps"></a>Próximas etapas

Agora que você instalou a CLI do Azure, faça um tour breve de seus recursos e comandos comuns.

> [!div class="nextstepaction"]
> [Introdução à CLI do Azure](get-started-with-azure-cli.md)
