---
title: Instalar a CLI do Azure 2.0
description: "Documentos de referência para a instalação da CLI do Azure 2.0"
keywords: "CLI do Azure, Instalar a CLI do Azure, Azure Python CLI, Referência da CLI do Azure"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 11/01/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: ea5c0ee1-c530-4a1e-a83f-e1be71f6d416
ms.openlocfilehash: 22c92aae5b836599d2f29b9f03fbf88c0ca6c2b8
ms.sourcegitcommit: 905939cc44764b4d1cc79a9b36c0793f7055a686
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/20/2017
---
# <a name="install-azure-cli-20"></a>Instalar a CLI 2.0 do Azure

Instale hoje mesmo a nova versão da CLI do Azure!
Nós a aprimoramos e atualizamos para fornecer uma ótima experiência de linha de comando nativa para gerenciar os recursos do Azure.
Ela pode ser usada em Windows, Linux e macOS.
Para saber mais sobre a versão mais recente, veja as [notas de versão](release-notes-azure-cli.md).

> [!NOTE]
> Se você precisa da versão anterior da CLI do Azure, veja como [instalar a CLI do Azure 1.0](/azure/cli-install-nodejs).

## <a name="a-namemacosinstall-on-macos"></a><a name="macOS"/>Instalar no macOS

No macOS, é possível instalar qualquer um com [Homebrew](https://brew.sh/) ou manualmente.

### <a name="install-with-homebrew"></a>Instalar com o Homebrew

1. Se não tiver feito já, instale o Homebrew seguindo as [instruções de instalação do Homebrew](https://docs.brew.sh/Installation.html).

2. Se você instalou anteriormente a CLI manualmente, siga as instruções de [desinstalação manual](#UninstallManually).

3. Atualize seus repositórios locais do Homebrew.

   ```bash
   brew update
   ```

4. Instale o pacote `azure-cli`.

  ```bash
  brew install azure-cli
  ```

> [!NOTE]
> Se você instalou anteriormente a CLI do Azure 1.0 com o Homebrew, em vez de instalar com o pacote, pode obter a CLI 2.0 pelo processo de atualização regular do Homebrew.
>
> ```bash
> brew upgrade
> ```

### <a name="install-manually"></a>Instalar manualmente

1. Instale a CLI do Azure 2.0 com `curl`.

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

2. Talvez você precise reiniciar o shell para que algumas alterações entrem em vigor.

   ```bash
   exec -l $SHELL
   ```
   
3. Execute a CLI no prompt de comando com o comando `az`.

## <a name="install-on-windows"></a>Instalar no Windows

### <a name="install-with-msi-for-the-windows-command-line"></a>Instalar com MSI para a linha de comando do Windows 

Para instalar a CLI no Windows e usá-la na linha de comando do Windows, baixe e execute o [Instalador da CLI do Azure (MSI)](https://aka.ms/InstallAzureCliWindows).

### <a name="install-with-apt-get-for-bash-on-ubuntu-on-windows"></a>Instalar com apt-get para Bash no Ubuntu no Windows

1. Se você não tiver o Bash no Windows, [instale-o](https://msdn.microsoft.com/commandline/wsl/install_guide).

2. Abra o shell do Bash.

3. Modifique sua lista de fontes.

   ```bash
   echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
   ```

4. Execute os comandos sudo a seguir:

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

5.  Execute a CLI no prompt de comando com o comando `az`.

## <a name="install-with-apt-package-manager"></a>Instalar com gerenciador de pacotes apt 

Para obter distribuições usando o gerenciador de pacote `apt` como Ubuntu ou Debian, você pode instalar a CLI do Azure 2.0 via `apt-get`.

> [!NOTE]
> Você deve ter o Python 2.7.x ou Python 3.x para usar a CLI. Se a distribuição não tiver um pacote para cada um, [instale o Python](https://www.python.org/downloads/).

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

3.  Execute a CLI no prompt de comando com o comando `az`.

## <a name="install-with-yum-package-manager"></a>Instalar com gerenciador de pacotes yum

Para as distribuições que usam o gerenciador de pacotes `yum` como Red Hat Enterprise Linux (RHEL), Fedora ou CentOS, você pode instalar o CLI do Azure 2.0 via `yum`.

> [!NOTE]
> Você deve ter o Python 2.7.x ou Python 3.x para usar a CLI. Se a distribuição não tiver um pacote para cada um, [instale o Python](https://www.python.org/downloads/).

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

4. Execute a CLI no prompt de comando com o comando `az`.

## <a name="install-with-zypper-package-manager"></a>Instalar com gerenciador de pacotes zypper

Para distribuições que usam o gerenciador de pacotes `zypper` como OpenSUSE ou SLE, instale a CLI do Azure 2.0 via `zypper`.

> [!NOTE]
> Você deve ter o Python 2.7.x ou Python 3.x para usar a CLI. Se a distribuição não tiver um pacote para cada um, [instale o Python](https://www.python.org/downloads/).

1. Importe a chave de repositório da Microsoft:

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. Crie informações sobre o repositório do `azure-cli` local:

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ntype=rpm-md\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/zypp/repos.d/azure-cli.repo'
   ```

3. Atualize o índice de pacote do `zypper` e instale:

   ```bash
   sudo zypper refresh
   sudo zypper install azure-cli
   ```

4. Execute a CLI no prompt de comando com o comando `az`.

## <a name="install-with-docker"></a>Instalar com o Docker

Vamos manter uma imagem de Docker pré-configurada com a CLI do Azure 2.0.

Instalar a CLI usando `docker run`.

   ```bash
   docker run -it azuresdk/azure-cli-python:<version>
   ```

Confira nossas [marcas do Docker](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/) para versões disponíveis.

A CLI está instalada na imagem como o comando `az` no `/usr/local/bin`.

> [!NOTE]
> Se você quiser acompanhar as chaves SSH do seu ambiente de usuário, use `-v ${HOME}:/root` para montar $HOME como `/root`.

> ```bash
> docker run -it -v ${HOME}:/root azuresdk/azure-cli-python:<version>
> ```

## <a name="a-namelinuxinstall-on-linux-without-a-package-manager"></a><a name="Linux"/>Instalar no Linux sem um gerenciador de pacotes

É recomendável que você instale a CLI com um gerenciador de pacotes, se for possível. Se você não quiser adicionar repositórios da Microsoft, ou estiver trabalhando com uma distribuição que não tem um pacote fornecido, você pode instalar manualmente a CLI.

1. Instale os pré-requisitos com base na sua distribuição do Linux.

   ```
   Platform              | Prerequisites
   ----------------------|---------------------------------------------
   Ubuntu 15.10 or 16.04 | sudo apt-get update && sudo apt-get install -y python libssl-dev libffi-dev python-dev build-essential
   Ubuntu 12.04 or 14.04 | sudo apt-get update && sudo apt-get install -y python libssl-dev libffi-dev python-dev
   Debian 8              | sudo apt-get update && sudo apt-get install -y python libssl-dev libffi-dev python-dev build-essential
   Debian 7              | sudo apt-get update && sudo apt-get install -y python libssl-dev libffi-dev python-dev
   CentOS 7.1 or 7.2     | sudo yum check-update; sudo yum install -y gcc python libffi-devel python-devel openssl-devel
   RedHat 7.2            | sudo yum check-update; sudo yum install -y gcc python libffi-devel python-devel openssl-devel
   SUSE OpenSUSE 13.2    | sudo zypper refresh && sudo zypper --non-interactive install curl gcc python python-xml libffi-devel python-devel openssl-devel
   ```

Se a distribuição não estiver listada acima, você precisará instalar o [Python 2.7 ou posterior](https://www.python.org/downloads/), [libffi](https://sourceware.org/libffi/) e [OpenSSL](https://www.openssl.org/source/).

2. Instalar a CLI com `curl`.

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

3. Talvez você precise reiniciar o shell para que algumas alterações entrem em vigor.

   ```bash
   exec -l $SHELL
   ```

4. Execute a CLI no prompt de comando com o comando `az`.

## <a name="troubleshooting"></a>Solucionar problemas

Se você encontrar um problema durante a instalação do CLI, verifique essa seção para ver se o seu caso específico é abordado. Se o problema não estiver aqui, [faça um registro do problema do Github](https://github.com/Azure/azure-cli/issues).

### <a name="curl-object-moved-error"></a>Erro "Objeto movido" de cURL

Se você receber um erro de `curl` relacionado ao parâmetro `-L` ou uma mensagem de erro incluindo o texto "Objeto movido", tente usar a URL completa em vez da `aka.ms` de redirecionamento:

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a>`az` comando não encontrado

Talvez seja necessário limpar o cache de hash de comando do shell. Executar

```bash
hash -r
```

e ver se o problema foi resolvido. O comando também pode não estar em seu `$PATH`. Verifique se `<install path>/bin` aparece em seu `$PATH` e reinicie o shell se necessário.

## <a name="uninstall-cli-1x-versions"></a>Desinstale as versões 1.x da CLI

Se você tiver uma versão anterior a 1.x da CLI disponível em seu sistema, você pode desinstalá-la com base no tipo de instalação usada.

### <a name="uninstall-with-npm"></a>Desinstalar com NPM

Remover a CLI mais antiga com `npm uninstall`.

  ```bash
  npm uninstall -g azure-cli
  ```

### <a name="uninstall-with-distributable"></a>Desinstalar com distribuível

Se você tiver instalado por meio do [Instalador da CLI do Azure (MSI)](http://aka.ms/webpi-azure-cli) ou de um [pacote de macOS](http://aka.ms/mac-azure-cli), use a mesma ferramenta para remover a instalação.

### <a name="uninstall-with-docker"></a>Desinstalar com o Docker

Se você instalou uma imagem do Docker para usar a versão anterior da CLI, remova a imagem e qualquer contêiner associado. Você pode criar os contêineres novamente depois de instalar a nova imagem do Docker, conforme descrito nas instruções de instalação.

  ```bash
  docker rmi -f microsoft/azure-cli
  ```

## <a name="update-the-cli"></a>Atualizar a CLI

Para atualizar a CLI do Azure, use o mesmo método que você usou para instalá-la.

### <a name="update-with-homebrew"></a>Atualizar com o Homebrew

1. Se você tiver instalado manualmente, siga as instruções para [instalar com o Homebrew](#macOS).

2. Atualize suas informações de repositório do Homebrew local.

   ```bash
   brew update
   ```

3. Atualize os seus pacotes instalados.

   ```bash
   brew upgrade
   ```

### <a name="update-with-msi"></a>Atualizar com MSI

Execute o [Instalador da CLI do Azure (MSI)](https://aka.ms/InstallAzureCliWindows) novamente.

### <a name="update-with-apt"></a>Atualizar com apt

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

### <a name="update-with-yum"></a>Atualizar com yum

Atualize a CLI do Azure com o comando `yum update`.

```bash
yum check-update
sudo yum update azure-cli
```

### <a name="update-with-zypper"></a>Atualizar com zypper

Você pode atualizar o pacote com o comando `zypper update`.

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

### <a name="update-with-docker"></a>Atualizar com o Docker

1. Atualizar sua imagem local com `docker pull`.

   ```bash
   docker pull azuresdk/azure-cli-python
   ```

2. Obter os contêineres atuais usando a imagem CLI.

   ```bash
   docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```

> [!NOTE]
> Se você instalou uma versão específica da imagem, você precisará adicionar `:<version>` ao final do nome da imagem.

3. Interromper e recriar os contêineres.

   ```bash
   docker stop inspiring_benz
   docker rm inspiring_benz
   docker run azuresdk/azure-cli-python
   ```

### <a name="update-manually"></a>Atualizar manualmente

Siga as instruções de instalação manual para [macOS](#macOS) ou [Linux](#Linux) para atualizar.

## <a name="uninstall"></a>Desinstalar

Se você decidir desinstalar a CLI, lamentamos a sua saída. Você deve desinstalar usando o mesmo método que você usou para instalar a CLI.

### <a name="uninstall-with-homebrew"></a>Desinstalar com o Homebrew

Desinstalar o pacote `azure-cli`.

   ```bash
   brew uninstall azure-cli
   ```

### <a name="uninstall-with-msi"></a>Desinstalar com MSI

Execute o [MSI](https://aka.ms/InstallAzureCliWindows) novamente e escolha Desinstalar.

### <a name="uninstall-with-apt"></a>Desinstalar com apt

Desinstalar através de `apt-get remove`:

  ```bash
  sudo apt-get remove -y azure-cli
  ```

### <a name="uninstall-with-yum"></a>Desinstalar com yum

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
  rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```

### <a name="uninstall-with-zypper"></a>Desinstalar com zypper

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
  rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```

### <a name="uninstall-with-docker"></a>Desinstalar com o Docker

Se você instalou uma imagem do Docker, será necessário remover qualquer contêiner que a estiver executando e, em seguida, excluir a imagem local.

1. Obtenha os contêineres que estão executando a imagem da CLI do Azure.

   ```bash
   docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```

2. Exclua todos os contêineres com a imagem da CLI.

   ```bash
   docker rm 34a868beb2ab
   ```

3. Remova a imagem da CLI instalada localmente.

   ```bash
   docker rmi azuresdk/azure-cli-python
   ```

> [!NOTE]
> Se você instalou uma versão específica da imagem, você precisará adicionar `:<version>` ao final do nome da imagem.

###<a name="a-nameuninstallmanuallyuninstall-manually"></a><a name="UninstallManually"/>Desinstalar manualmente

Se você usou o script em https://aka.ms/InstallAzureCli para instalar a CLI, é possível desinstalá-la com estas etapas.

1. Remova os arquivos instalados.

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. Exclua a linha `<install location>/lib/azure-cli/az.completion` de `<install location>/.bash_profile`.

3. Se o shell usa um cache de comando, recarregue-o.

   ```bash
   hash -r
   ```

> [!Note]
> O local de instalação padrão é `/Users/<username>` para o macOS e `/home/<username>` para o Linux.

## <a name="report-cli-issues-and-feedback"></a>Relatar comentários e problemas da CLI

Se você encontrar bugs na ferramenta, faça o registro do problema na seção [Problemas](https://github.com/Azure/azure-cli/issues) do nosso repositório do GitHub.
Para fornecer comentários na linha de comando, use o comando `az feedback`.
