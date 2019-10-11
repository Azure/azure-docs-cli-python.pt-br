---
title: Instalar a CLI do Azure para macOS
description: Como instalar a CLI do Azure no macOS
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/05/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 790c63a60a5d23863b48227dcc99462bbf950d80
ms.sourcegitcommit: b42ce26476b135bb2047c8d9d787580c858f8b6b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2019
ms.locfileid: "72163844"
---
# <a name="install-azure-cli-on-macos"></a>Instalar a CLI do Azure no macOS

Para a plataforma macOS, você pode instalar a CLI do Azure com o [gerenciador de pacotes homebrew](https://brew.sh). O Homebrew torna mais fácil manter a instalação da CLI atualizada. O pacote da CLI foi testado em versões do macOS 10.9 e posteriores.

[!INCLUDE [current-version](includes/current-version.md)]

## <a name="install-with-homebrew"></a>Instalar com o Homebrew

O homebrew é a maneira mais fácil de gerenciar a instalação da CLI. Ele fornece maneiras convenientes de instalar, atualizar e desinstalar.
Se você não tiver o homebrew disponível em seu sistema, [instale-o](https://docs.brew.sh/Installation.html) antes de continuar.

Você pode instalar a CLI atualizando suas informações de repositório brew e executando o comando `install`:

```bash
brew update && brew install azure-cli
```

> [!IMPORTANT]
>
> A CLI do Azure tem uma dependência no pacote `python3` do Homebrew, e a instalará.
> A CLI do Azure é certamente compatível com a versão mais recente do `python3` publicada no Homebrew.

É possível executar a CLI do Azure com o comando `az`. Para entrar, use o comando [az login](/cli/azure/reference-index#az-login).

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Para saber mais sobre os diferentes métodos de autenticação, confira [Entrar com a CLI do Azure](authenticate-azure-cli.md).

## <a name="troubleshooting"></a>solução de problemas

Se você encontrar um problema ao instalar a CLI através do Homebrew, aqui estão alguns erros comuns. Se você tiver um problema não abordado aqui, [arquive um problema no github](https://github.com/Azure/azure-cli/issues).

### <a name="unable-to-find-python-or-installed-packages"></a>Não é possível localizar o Python ou os pacotes instalados

Pode haver uma pequena incompatibilidade de versão ou outro problema durante a instalação do homebrew. A CLI não usa um ambiente virtual Python, portanto, ela se baseia em localizar a versão instalada do Python. Uma possível correção é instalar e revincular a dependência `python3` do Homebrew.

```bash
brew update && brew install python3 && brew upgrade python3
brew link --overwrite python3
```

### <a name="cli-version-1x-is-installed"></a>A versão 1.x da CLI está instalada

Se tiver sido instalada uma versão desatualizada, pode ser devido a um cache de homebrew obsoleto. Siga as instruções de [atualização](#update).

### <a name="proxy-blocks-connection"></a>Conexão de blocos de proxy

Talvez você não consiga obter recursos do Homebrew, a menos que o tenha configurado corretamente para usar seu proxy. Siga as [instruções de configuração de proxy do Homebrew](https://docs.brew.sh/Manpage#using-homebrew-behind-a-proxy).

> [!IMPORTANT]
> Se você estiver atrás de um proxy, as variáveis `HTTP_PROXY` e `HTTPS_PROXY` precisarão ser definidas para se conectarem aos serviços do Azure com a CLI.
> Se você não estiver usando a autenticação básica, é recomendável exportar as variáveis no arquivo `.bashrc`.
> Sempre siga as políticas de segurança da sua empresa e os requisitos do administrador do sistema.

Para obter os recursos de Bottle do Homebrew, o proxy precisa permitir conexões HTTPS com os seguintes endereços:

* `https://formulae.brew.sh`
* `https://homebrew.bintray.com`

## <a name="update"></a>Atualizar

A CLI é atualizada regularmente com correções de bugs, aprimoramentos, novos recursos e funcionalidade de visualização. Uma nova versão fica disponível aproximadamente a cada duas semanas. Atualize as informações do repositório local e atualize o pacote `azure-cli`.

```bash
brew update && brew upgrade azure-cli
```

## <a name="uninstall"></a>Desinstalar

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

Use o homebrew para desinstalar o pacote `azure-cli`.

```bash
brew uninstall azure-cli
```

## <a name="other-installation-methods"></a>Outros métodos de instalação

Se você não pode usar o Homebrew para instalar a CLI do Azure em seu ambiente, é possível usar as instruções manuais para o Linux. Observe que esse processo não é oficialmente mantido para ser compatível com o macOS. É sempre recomendável usar um gerenciador de pacotes, como o Homebrew. Somente use o método de instalação manual se não tiver nenhuma outra opção disponível.

Para as instruções de instalação manual, confira [Instalar manualmente a CLI do Azure no Linux](install-azure-cli-linux.md).

## <a name="next-steps"></a>Próximas etapas

Agora que você instalou a CLI do Azure, faça um tour breve de seus recursos e comandos comuns.

> [!div class="nextstepaction"]
> [Introdução à CLI do Azure](get-started-with-azure-cli.md)
