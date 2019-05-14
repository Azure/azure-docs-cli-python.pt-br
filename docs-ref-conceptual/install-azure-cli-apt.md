---
title: Instalar a CLI do Azure no Linux com apt
description: Como instalar a CLI do Azure com o gerenciador de pacotes apt
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/08/2019
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: af82eea3fd549cbca85699a3030a19bc82574b73
ms.sourcegitcommit: c65c69bd08fd6b7632ba60dc7c8e9f2b57a9d0b7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2019
ms.locfileid: "65476269"
---
# <a name="install-azure-cli-with-apt"></a>Instalar CLI do Azure com o apt

Se você estiver executando uma distribuição fornecida com `apt`, como Ubuntu ou Debian, há um pacote x86_64 disponível para a CLI do Azure. Este pacote foi testado e é compatível com:

* Ubuntu trusty, xenial, artful, bionic e disco
* Debian wheezy, jessie e stretch

[!INCLUDE [current-version](includes/current-version.md)]

> [!NOTE]
>
> O pacote para a CLI do Azure instala seu próprio interpretador de Python e não usa o Python do sistema.

## <a name="install"></a>Instalar

Oferecemos duas maneiras de instalar a CLI do Azure com distribuições que dão suporte a `apt`: Como um script tudo-em-um que executa os comandos de instalação para você, e instruções que podem ser executadas como um processo passo a passo por conta própria.

### <a name="install-with-one-command"></a>Instalar com um comando

Oferecemos e mantemos um script que executa todos os comandos de instalação em uma única etapa. Executá-lo usando `curl` e redirecione diretamente para `bash`, ou baixe o script para um arquivo e inspecione-o antes da execução.

> [!IMPORTANT]
> Esse script é verificado somente para o Ubuntu 16.04+ e Debian 8+. Ele pode não funcionar em outras distribuições.
> Se você estiver usando uma distribuição derivada como Linux Mint, siga as instruções de instalação manual e execute qualquer solução de problemas necessária.

```bash
curl -sL https://aka.ms/InstallAzureCLIDeb | sudo bash
```

### <a name="manual-install-instructions"></a>Instruções para instalação manual

Se você não quiser executar um script como superusuário, siga estas etapas manuais para instalar a CLI do Azure.

1. Obtenha os pacotes necessários para o processo de instalação:

    ```bash
    sudo apt-get update
    sudo apt-get install curl apt-transport-https lsb-release gnupg
    ```

2. Baixe e instale a chave de autenticação da Microsoft:

    ```bash
    curl -sL https://packages.microsoft.com/keys/microsoft.asc | \
        gpg --dearmor | \
        sudo tee /etc/apt/trusted.gpg.d/microsoft.asc.gpg > /dev/null
    ```

3. <div id="set-release"/>Adicione o repositório de software da CLI do Azure:

    ```bash
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
    ```

4. Atualize as informações do repositório e instale o pacote `azure-cli`:

    ```bash
    sudo apt-get update
    sudo apt-get install azure-cli
    ```

Execute a CLI do Azure com o comando `az`. Para entrar, use o comando [az login](/cli/azure/reference-index#az-login).

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Para saber mais sobre os diferentes métodos de autenticação, confira [Entrar com a CLI do Azure](authenticate-azure-cli.md).

## <a name="troubleshooting"></a>solução de problemas

Aqui estão alguns problemas comuns vistos durante a instalação com `apt`. Se você tiver um problema não abordado aqui, [arquive um problema no github](https://github.com/Azure/azure-cli/issues).

### <a name="lsbrelease-does-not-return-the-correct-base-distribution-version"></a>lsb_release não retorna a versão correta da distribuição de base

Algumas distribuições derivadas do Ubuntu ou do Debian, como o Linux Mint, podem não retornar o nome correto da versão de `lsb_release`. Esse valor é usado no processo de instalação para determinar o pacote de instalação. Se você souber o nome do código da versão do Ubuntu ou do Debian da qual sua distribuição é derivada, poderá definir o valor de `AZ_REPO` manualmente ao [adicionar o repositório](#set-release). Caso contrário, procure informações para sua distribuição sobre como determinar o nome do código da distribuição de base e defina `AZ_REPO` com o valor correto.

### <a name="no-package-for-your-distribution"></a>Nenhum pacote para distribuição

Às vezes, um pacote da CLI do Azure pode ser disponibilizado somente um tempo depois do lançamento da distribuição. A CLI do Azure é projetada para ser resiliente em relação a versões futuras das dependências e precisam da menor quantidade possível delas. Se não houver pacotes disponíveis para sua distribuição de base, tente um pacote de uma distribuição anterior.

Para isso, defina o valor de `AZ_REPO` manualmente ao [adicionar o repositório](#set-release). Para as distribuições do Ubuntu, use o repositório `disco`; para as distribuições do Debian, use `stretch`. Não há suporte para as distribuições lançadas antes do Ubuntu Trusty e do Debian Wheezy.

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a>Atualizar

Use `apt-get upgrade` para atualizar o pacote da CLI.

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
    sudo rm /etc/apt/trusted.gpg.d/microsoft.asc.gpg
    ```

4. Remova quaisquer pacotes desnecessários:

   ```bash
   sudo apt autoremove
   ```

## <a name="next-steps"></a>Próximas etapas

Agora que você instalou a CLI do Azure, faça um tour breve de seus recursos e comandos comuns.

> [!div class="nextstepaction"]
> [Introdução à CLI do Azure](get-started-with-azure-cli.md)
