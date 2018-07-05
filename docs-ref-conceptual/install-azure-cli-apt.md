---
title: Instalar a CLI do Azure 2.0 no Linux com apt
description: Como instalar a CLI do Azure 2.0 com o gerenciador de pacotes apt
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/24/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: abbffb1c474d752130dfffa8e60937b3d632fa14
ms.sourcegitcommit: c6c3058254974b3a1d5d2fa2cd231a900c53d321
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2018
ms.locfileid: "37126575"
---
# <a name="install-azure-cli-20-with-apt"></a>Instalar CLI do Azure 2.0 com o apt

Se você estiver executando uma distribuição que venha com o `apt`, como o Ubuntu ou Debian, há um pacote 64-bit disponível para a CLI do Azure. Esse pacote foi testado com:

* Ubuntu trusty, xenial, artful e bionic
* Debian wheezy, jessie e stretch

## <a name="install"></a>Instalar

1. <a name="install-step-1"/> Modifique sua lista de fontes:

    ```bash
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
    ```

2. <a name="signingKey"></a>Obtenha a chave de assinatura da Microsoft:

   ```bash
   curl -L https://packages.microsoft.com/keys/microsoft.asc | sudo apt-key add -
   ```

3. Instalar a CLI:

   ```bash
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

   > [!WARNING]
   > A chave de assinatura foi atualizada em maio de 2018 e foi substituída. Se você receber erros de chave de assinatura, confirme se você [adquiriu a chave de assinatura mais recente](#signingKey).

É possível executar a CLI do Azure com o comando `az`. Para fazer logon, execute o comando `az login`.

```azurecli
az login
```

Para saber mais sobre os métodos de logon diferente, consulte [Fazer logon com a CLI do Azure 2.0](authenticate-azure-cli.md).

## <a name="troubleshooting"></a>solução de problemas

Aqui estão alguns problemas comuns vistos durante a instalação com `apt`. Se o problema não estiver listado aqui, [registre um problema no github](https://github.com/Azure/azure-cli/issues).

### <a name="lsbrelease-fails-with-command-not-found"></a>lsb_release falha com "Command não encontrado"

Ao executar o comando `lsb_release`, pode ser que você veja uma saída semelhante ao seguinte erro:

```output
-bash: lsb_release: command not found
```

O erro ocorre devido a lsb_release não estar sendo instalado. Você pode resolver isso instalando o pacote `lsb-release`.

```bash
sudo apt-get install lsb-release
```

### <a name="lsbrelease-does-not-return-the-base-distribution-version"></a>lsb_release não retorna a versão de distribuição de base

Algumas distribuições derivadas de Ubuntu ou Debian, como o Linux Mint, podem não retornar o nome da versão correta do `lsb_release`. Esse valor é usado no processo de instalação para determinar o pacote de instalação. Se souber o nome da versão da qual sua distribuição é derivada, você pode definir o valor `AZ_REPO` manualmente em [instalar etapa 1](#install-step-1). Caso contrário, procure informações para a sua distribuição sobre como determinar o nome da base de distribuição e defina `AZ_REPO` para o valor correto.

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

### <a name="apt-key-hangs"></a>A apt-key trava

Quando atrás de um firewall bloqueando as conexões de saída para a porta 11371, o comando `apt-key` pode travar indefinidamente. O firewall pode exigir o uso de um proxy HTTP para conexões de saída:

```bash
sudo apt-key adv --keyserver-options http-proxy=http://<USER>:<PASSWORD>@<PROXY-HOST>:<PROXY-PORT>/ --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
```

Se você não souber se tem um proxy, entre em contato com o administrador do sistema. Se o proxy não precisar de um login, deixe usuário, senha e o token `@` de fora.

## <a name="update"></a>Atualizar

Use `apt-get upgrade` para atualizar o pacote da CLI.

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!WARNING]
> A chave de assinatura foi atualizada em maio de 2018 e foi substituída. Se você receber erros de chave de assinatura, confirme se você [adquiriu a chave de assinatura mais recente](#signingKey).
   
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
