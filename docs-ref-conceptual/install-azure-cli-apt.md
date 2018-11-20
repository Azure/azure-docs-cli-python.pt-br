---
title: Instalar a CLI do Azure no Linux com apt
description: Como instalar a CLI do Azure com o gerenciador de pacotes apt
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/12/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 0d4311e88fec9903c1aab1410cc71328f896dc65
ms.sourcegitcommit: 728a050f13d3682122be4a8993596cc4185a45ce
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/15/2018
ms.locfileid: "51680927"
---
# <a name="install-azure-cli-with-apt"></a>Instalar CLI do Azure com o apt

Se você estiver executando uma distribuição que vem com `apt`, como o Ubuntu ou o Debian, haverá um pacote de 64 bits disponível para a CLI do Azure. Esse pacote foi testado com:

* Ubuntu trusty, xenial, artful e bionic
* Debian wheezy, jessie e stretch

## <a name="install"></a>Instalar

1. <div id="install-step-1"/>Modifique sua lista de fontes:

    ```bash
    sudo apt-get install apt-transport-https lsb-release software-properties-common -y
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
    ```

2. <div id="signingKey"/>Obtenha a chave de assinatura da Microsoft:

   ```bash
   sudo apt-key --keyring /etc/apt/trusted.gpg.d/Microsoft.gpg adv \
        --keyserver packages.microsoft.com \
        --recv-keys BC528686B50D79E339D3721CEB3E94ADBE1229CF
   ```

3. Instalar a CLI:

   ```bash
   sudo apt-get update
   sudo apt-get install azure-cli
   ```

   > [!WARNING]
   > A chave de assinatura foi atualizada em maio de 2018 e foi substituída. Se você receber erros de autenticação, verifique se tem [a chave de autenticação mais recente](#signingKey).

É possível executar a CLI do Azure com o comando `az`. Para entrar, use o comando [az login](/cli/azure/reference-index#az-login).

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Para saber mais sobre os diferentes métodos de autenticação, confira [Entrar com a CLI do Azure](authenticate-azure-cli.md).

## <a name="troubleshooting"></a>solução de problemas

Aqui estão alguns problemas comuns vistos durante a instalação com `apt`. Se você tiver um problema não abordado aqui, [arquive um problema no github](https://github.com/Azure/azure-cli/issues).

### <a name="lsbrelease-does-not-return-the-base-distribution-version"></a>lsb_release não retorna a versão da distribuição de base

Algumas distribuições derivadas do Ubuntu ou do Debian, como o Linux Mint, podem não retornar o nome correto da versão de `lsb_release`. Esse valor é usado no processo de instalação para determinar o pacote de instalação. Se você souber o nome da versão da qual sua distribuição é derivada, poderá definir o `AZ_REPO` valor manualmente em [instalar etapa 1](#install-step-1). Caso contrário, procure informações para sua distribuição sobre como determinar o nome da distribuição de base e defina `AZ_REPO` para o valor correto.

### <a name="apt-key-fails-with-no-dirmngr"></a>apt-key falha com “Sem dirmngr”

Ao executar o comando `apt-key`, pode ser que você veja uma saída semelhante ao seguinte erro:

```output
gpg: failed to start the dirmngr '/usr/bin/dirmngr': No such file or directory
gpg: connecting dirmngr at '/tmp/apt-key-gpghome.kt5zo27tp1/S.dirmngr' failed: No such file or directory
gpg: keyserver receive failed: No dirmngr
```

O erro ocorre devido a um componente ausente requerido por `apt-key`. Você pode resolver isso instalando o pacote `dirmngr`.

```bash
sudo apt-get install dirmngr
```

### <a name="apt-key-hangs"></a>apt-key trava

Quando atrás de um firewall que bloqueia as conexões de saída para a porta 11371, o comando `apt-key` pode travar indefinidamente.
O firewall pode exigir um proxy HTTP para as conexões de saída:

```bash
sudo apt-key --keyring /etc/apt/trusted.gpg.d/Microsoft.gpg adv \
    --keyserver-options http-proxy=http://<USER>:<PASSWORD>@<PROXY-HOST>:<PROXY-PORT>/ \
    --keyserver packages.microsoft.com \
    --recv-keys BC528686B50D79E339D3721CEB3E94ADBE1229CF
```

Para determinar se você tem um proxy, entre em contato com o administrador do sistema. Se o proxy não precisar de logon, omita as informações sobre usuário e senha.

## <a name="update"></a>Atualizar

Use `apt-get upgrade` para atualizar o pacote da CLI.

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!WARNING]
> A chave de assinatura foi atualizada em maio de 2018 e foi substituída. Se você receber erros de autenticação, verifique se tem [a chave de autenticação mais recente](#signingKey).
>
> [!NOTE]
> Esse comando atualiza todos os pacotes instalados no sistema que não tiveram uma alteração de dependência.
> Para atualizar apenas a CLI, use `apt-get install`.
> 
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a>Desinstalar

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. Desinstalar com `apt-get remove`:

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. Se você não pretender reinstalar a CLI, remova as informações do repositório da CLI do Azure:

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. Remova a chave de autenticação:

    ```bash
    sudo rm /etc/apt/trusted.gpg.d/Microsoft.gpg
    ```

4. Remova quaisquer pacotes desnecessários:

   ```bash
   sudo apt autoremove
   ```

## <a name="next-steps"></a>Próximas etapas

Agora que você instalou a CLI do Azure, faça um tour breve de seus recursos e comandos comuns.

> [!div class="nextstepaction"]
> [Introdução à CLI do Azure](get-started-with-azure-cli.md)