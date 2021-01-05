---
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/29/2020
ms.topic: include
ms.custom: devx-track-azurecli
ms.openlocfilehash: caf16d07ba6bbf6010a3e8e01ef6b49108853566
ms.sourcegitcommit: bd2dbc80328936dadd211764d25c32a14fc58083
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/04/2021
ms.locfileid: "97858016"
---
## <a name="overview"></a>Visão geral

O gerenciador de pacotes `apt` contém um pacote x86_64 para a CLI do Azure que foi testado nas distribuições a seguir.

| Distribuição | Versão |
|:-------------|:--------|
| Ubuntu       | 14.04 LTS (Trusty Tahir), 16.04 LTS (Xenial Xerus), 18.04 LTS (Bionic Beaver), 19.10 (Eoan Ermine), 20.04 LTS (Focal Fossa) |
| Debian       | Debian 8 (Jessie), Debian 9 (Stretch), Debian 10 (Buster) |

> [!WARNING]
> Ubuntu 20.04 (Focal Fossa), inclui um pacote `azure-cli` com a versão `2.0.81` fornecido pelo repositório `focal/universe`. Esse pacote está desatualizado e não é recomendado. Se esse pacote estiver instalado, remova-o antes de continuar executando o comando `sudo apt remove azure-cli -y && sudo apt autoremove -y`.

## <a name="installation-options"></a>Opções de instalação

Há duas formas de instalar a CLI do Azure no seu sistema.  Primeiro, você pode executar um comando que vai baixar um script de instalação e executar os comandos de instalação.  Ou, se preferir, você pode executar os comandos de instalação por conta própria em um processo passo a passo.  Os dois métodos são apresentados abaixo.

## <a name="option-1-install-with-one-command"></a>Opção 1: Instalar com um comando

A equipe da CLI do Azure mantém um script para executar todos os comandos de instalação em uma etapa.  Esse script é baixado por meio de `curl` e encaminhado diretamente para `bash` a fim de instalar a CLI.

Se você quiser inspecionar o conteúdo do script por conta própria antes de executá-lo, basta baixar o script usando `curl` e inspecioná-lo no seu editor de texto favorito.

```bash
curl -sL https://aka.ms/InstallAzureCLIDeb | sudo bash
```

## <a name="option-2-step-by-step-installation-instructions"></a>Opção 2: Instruções de instalação passo a passo

Se você preferir um processo de instalação passo a passo, conclua as etapas a seguir para instalar a CLI do Azure.

1. Obtenha os pacotes necessários para o processo de instalação:

    ```bash
    sudo apt-get update
    sudo apt-get install ca-certificates curl apt-transport-https lsb-release gnupg
    ```

2. Baixe e instale a chave de autenticação da Microsoft:

    ```bash
    curl -sL https://packages.microsoft.com/keys/microsoft.asc |
        gpg --dearmor |
        sudo tee /etc/apt/trusted.gpg.d/microsoft.gpg > /dev/null
    ```

3. <div id="set-release"/>Adicione o repositório de software da CLI do Azure (pule esta etapa em distribuições do Linux ARM64):

    ```bash
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" |
        sudo tee /etc/apt/sources.list.d/azure-cli.list
    ```

4. Atualize as informações do repositório e instale o pacote `azure-cli`:

    ```bash
    sudo apt-get update
    sudo apt-get install azure-cli
    ```

## <a name="sign-in-to-azure-with-the-azure-cli"></a>Entrar no Azure com a CLI do Azure

Execute a CLI do Azure com o comando `az`. Para entrar, use o comando [az login](/cli/azure/reference-index#az-login).

[!INCLUDE [interactive-login](interactive-login.md)]

Para saber mais sobre os diferentes métodos de autenticação, confira [Entrar com a CLI do Azure](../authenticate-azure-cli.md).

## <a name="troubleshooting"></a>Solução de problemas

Aqui estão alguns problemas comuns vistos durante a instalação com `apt`. Se você tiver um problema não abordado aqui, [arquive um problema no github](https://github.com/Azure/azure-cli/issues).

### <a name="no-module-issue-on-ubuntu-2004-focalwsl"></a>Nenhum problema com o módulo no Ubuntu 20.04 (Focal)/WSL

Se você tiver instalado `azure-cli` em `Focal` sem adicionar o repositório de software da CLI do Azure na [etapa 3](#set-release) das instruções de instalação manual ou sem usar nosso [script](#option-1-install-with-one-command), poderá encontrar problemas indicando, por exemplo, que não há nenhum módulo chamado "decorator" ou "antlr4", já que o pacote instalado é o `azure-cli 2.0.81` desatualizado do repositório `focal/universe`. Remova-a primeiro executando `sudo apt remove azure-cli -y && sudo apt autoremove -y` e, em seguida, siga as [instruções](#install) acima para instalar o pacote `azure-cli` mais recente.

### <a name="lsb_release-does-not-return-the-correct-base-distribution-version"></a>lsb_release não retorna a versão correta da distribuição de base

Algumas distribuições derivadas do Ubuntu ou do Debian, como o Linux Mint, podem não retornar o nome correto da versão de `lsb_release`. Esse valor é usado no processo de instalação para determinar o pacote de instalação. Se você souber o nome do código da versão do Ubuntu ou do Debian da qual sua distribuição é derivada, poderá definir o valor de `AZ_REPO` manualmente ao [adicionar o repositório](#set-release). Caso contrário, procure informações para sua distribuição sobre como determinar o nome do código da distribuição de base e defina `AZ_REPO` com o valor correto.

### <a name="no-package-for-your-distribution"></a>Nenhum pacote para distribuição

Às vezes, um pacote da CLI do Azure pode ser disponibilizado somente um tempo depois do lançamento da distribuição. A CLI do Azure é projetada para ser resiliente em relação a versões futuras das dependências e precisam da menor quantidade possível delas. Se não houver pacotes disponíveis para sua distribuição de base, tente um pacote de uma distribuição anterior.

Para isso, defina o valor de `AZ_REPO` manualmente ao [adicionar o repositório](#set-release). Para as distribuições do Ubuntu, use o repositório `bionic`; para as distribuições do Debian, use `stretch`. Não há suporte para as distribuições lançadas antes do Ubuntu Trusty e do Debian Wheezy.

### <a name="elementary-os-eos-fails-to-install-the-azure-cli"></a>O EOS (SO elementar) falha ao instalar a CLI do Azure

O EOS não consegue instalar a CLI do Azure porque `lsb_release` retorna `HERA`, que é o nome da versão de EOS.  A solução é corrigir o arquivo `/etc/apt/sources.list.d/azure-cli.list` e alterar `hera main` para `bionic main`.

Conteúdo do arquivo original:

```
deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ hera main
```

Conteúdo do arquivo modificado

```
deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ bionic main
```

### <a name="proxy-blocks-connection"></a>Conexão de blocos de proxy

[!INCLUDE[configure-proxy](configure-proxy.md)]

Talvez você queira configurar explicitamente `apt` para usar esse proxy sempre. Verifique se as linhas a seguir aparecem em um arquivo de configuração `apt` em `/etc/apt/apt.conf.d/`. É recomendável usar o arquivo de configuração global existente, um arquivo de configuração de proxy existente, `40proxies` ou `99local`. No entanto, siga os requisitos de administração do sistema.

```apt.conf
Acquire {
    http::proxy "http://[username]:[password]@[proxy]:[port]";
    https::proxy "https://[username]:[password]@[proxy]:[port]";
}
```

Se o proxy não usar autenticação básica, __remova__ a parte `[username]:[password]@` do URI do proxy. Se você precisar de mais informações sobre a configuração do proxy, confira a documentação oficial do Ubuntu:

* [apt.conf manpage](http://manpages.ubuntu.com/manpages/bionic/en/man5/apt.conf.5.html)
* [Wiki do Ubuntu – apt-get howto](https://help.ubuntu.com/community/AptGet/Howto#Setting_up_apt-get_to_use_a_http-proxy)

Para obter a chave de assinatura da Microsoft e o pacote do nosso repositório, o proxy precisa permitir conexões HTTPS com o seguinte endereço:

* `https://packages.microsoft.com`

[!INCLUDE[troubleshoot-wsl.md](troubleshoot-wsl.md)]

## <a name="update"></a>Atualizar
[!INCLUDE [az-upgrade](az-upgrade.md)]

Você também pode usar `apt-get upgrade` para atualizar o pacote da CLI.

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> Esse comando atualiza todos os pacotes instalados no sistema que não tiveram uma alteração de dependência.
> Para atualizar apenas a CLI, use `apt-get install`.
>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a>Desinstalar

[!INCLUDE [uninstall-boilerplate.md](uninstall-boilerplate.md)]

1. Desinstalar com `apt-get remove`:

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. Se você não pretender reinstalar a CLI, remova as informações do repositório da CLI do Azure:

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. Se você não usa nenhum outro pacote da Microsoft, remova a chave de assinatura:

    ```bash
    sudo rm /etc/apt/trusted.gpg.d/microsoft.gpg
    ```

4. Remova quaisquer pacotes desnecessários:

   ```bash
   sudo apt autoremove
   ```
