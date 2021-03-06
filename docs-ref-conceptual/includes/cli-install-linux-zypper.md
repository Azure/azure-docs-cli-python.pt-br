---
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 11/24/2020
ms.topic: include
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: d80970432a116656a33a3dc6c0d4909b4b92f312
ms.sourcegitcommit: d5f026468ea20bbd7ef35bdbf9852bcb2b812d83
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/23/2020
ms.locfileid: "97744590"
---
## <a name="overview"></a>Visão geral

Para distribuições Linux com `zypper`, como o openSUSE ou SLES, há um pacote disponível para a CLI do Azure. Este pacote foi testado com openSUSE Leap 15.1 e SLES 15.

[!INCLUDE [current-version](current-version.md)]

[!INCLUDE [rpm-warning](rpm-warning.md)]

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

[!INCLUDE [interactive-login](interactive-login.md)]

Para saber mais sobre os diferentes métodos de autenticação, confira [Entrar com a CLI do Azure](../authenticate-azure-cli.md).

## <a name="troubleshooting"></a>Solução de problemas

Aqui estão alguns problemas comuns vistos durante a instalação com `zypper`. Se você tiver um problema não abordado aqui, [arquive um problema no GitHub](https://github.com/Azure/azure-cli/issues).

### <a name="notimplementederror-on-opensuse-15-vm"></a>NotImplementedError na VM do OpenSUSE 15
A VM do OpenSUSE 15 tem uma CLI do Azure pré-instalada com a versão `2.0.45`, que está desatualizada e apresenta problemas com o comando `az login`. Remova-a junto com as dependências antes de seguir as instruções de [instalação](#install) para adicionar a última CLI do Azure:

```bash
sudo zypper rm -y --clean-deps azure-cli
```

Se você atualizou a CLI do Azure sem remover as dependências da versão `2.0.45`, as dependências antigas podem afetar a última versão da CLI do Azure. Você precisará adicionar novamente a versão antiga para vinculá-la às dependências e remover a `azure-cli` junto com as dependências:

```bash
# The package name may vary on different system version, run 'zypper --no-refresh info azure-cli' to check the source package format
sudo zypper install --oldpackage azure-cli-2.0.45-4.22.noarch

sudo zypper rm -y --clean-deps azure-cli
```

### <a name="install-on-sles-12-or-other-systems-without-python-36"></a>Instalar no SLES 12 ou em sistemas sem o Python 3.6

No SLES 12, o pacote `python3` padrão é `3.4` e não é compatível com a CLI do Azure. Primeiro, siga as etapas 1 a 3 das [instruções de instalação](#install) para adicionar o repositório da `azure-cli`. Em seguida, crie uma versão posterior do `python3` da origem. Por fim, você poderá baixar o pacote da CLI do Azure e instalá-lo sem nenhuma dependência.

Use o seguinte comando para instalar a CLI do Azure (lembre-se de que a versão existente do Python 3 será substituída pelo Python 3.6):

```bash
curl -sL https://azurecliprod.blob.core.windows.net/sles12_install.sh | sudo bash
```

Ou, então, faça isso passo a passo:

```bash
# !Please add azure-cli repository first following step 1-3 of the install instruction before running below commands
$ sudo zypper refresh
$ sudo zypper install -y gcc gcc-c++ make ncurses patch wget tar zlib-devel zlib openssl-devel
# Download Python source code
$ PYTHON_VERSION="3.6.9"
$ PYTHON_SRC_DIR=$(mktemp -d)
$ wget -qO- https://www.python.org/ftp/python/$PYTHON_VERSION/Python-$PYTHON_VERSION.tgz | tar -xz -C "$PYTHON_SRC_DIR"
# Build Python
# Please be aware that with --prefix=/usr, the command will override the existing Python 3 version
$ $PYTHON_SRC_DIR/*/configure --prefix=/usr
$ make
$ sudo make install
# Download azure-cli package 
$ AZ_VERSION=$(zypper --no-refresh info azure-cli |grep Version | awk -F': ' '{print $2}' | awk '{$1=$1;print}')
$ wget https://packages.microsoft.com/yumrepos/azure-cli/azure-cli-$AZ_VERSION.x86_64.rpm
# Install without dependency
$ sudo rpm -ivh --nodeps azure-cli-$AZ_VERSION.x86_64.rpm
```

### <a name="proxy-blocks-connection"></a>Conexão de blocos de proxy

[!INCLUDE[configure-proxy](configure-proxy.md)]

Talvez você queira configurar explicitamente `zypper` (por meio de `yast2`) para usar esse proxy sempre. Para fazer isso, execute o comando `yast2 proxy` como superusuário e preencha as informações apresentadas no formulário. Se você tiver um gerenciador de janelas disponível no sistema, também poderá usar o painel `Network Services > Proxy` no `YaST Control Center`.

Para configurações avançadas ou mais informações, confira a [documentação de configuração do Proxy do OpenSUSE](https://www.suse.com/documentation/slms1/book_slms/data/sec_wy_config_updates_proxy.html)

Para obter a chave de assinatura da Microsoft e o pacote do nosso repositório, o proxy precisa permitir conexões HTTPS com os seguintes endereços:

* `https://packages.microsoft.com`
* `https://download.opensuse.org`

[!INCLUDE[troubleshoot-wsl.md](troubleshoot-wsl.md)]

### <a name="ssl-certificate-problem"></a>Problema com o certificado SSL

Quando um certificado é inválido ou está desatualizado em um computador, você pode receber um erro indicando que o cURL falhou ao verificar a legitimidade do servidor e, portanto, não foi possível estabelecer uma conexão segura.  Atualize o certificado para corrigir o problema.  

```bach
sudo zypper update-ca-certificates
```

## <a name="update"></a>Atualizar

[!INCLUDE [az-upgrade](az-upgrade.md)]

Você também pode atualizar o pacote com o comando `zypper update`.

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

## <a name="uninstall"></a>Desinstalar

[!INCLUDE [uninstall-boilerplate.md](uninstall-boilerplate.md)]

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
