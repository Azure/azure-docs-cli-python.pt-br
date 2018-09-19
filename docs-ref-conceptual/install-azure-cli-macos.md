---
title: Instalar a CLI do Azure para macOS
description: Como instalar a CLI do Azure 2.0 no macOS
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: fd829c6ff9162b660a889d3e08615a76f42aeb97
ms.sourcegitcommit: 0e688704889fc88b91588bb6678a933c2d54f020
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/11/2018
ms.locfileid: "44388466"
---
# <a name="install-azure-cli-20-on-macos"></a>Instalar CLI do Azure 2.0 no macOS

Para a plataforma macOS, você pode instalar a CLI do Azure com o [gerenciador de pacotes homebrew](https://brew.sh). O Homebrew torna mais fácil manter a instalação da CLI atualizada. O pacote da CLI foi testado em versões do macOS 10.9 e posteriores.

## <a name="install"></a>Instalar

O homebrew é a maneira mais fácil de gerenciar a instalação da CLI. Ele fornece maneiras convenientes de instalar, atualizar e desinstalar.
Se você não tiver o homebrew disponível em seu sistema, [instale-o](https://docs.brew.sh/Installation.html) antes de continuar.

Você pode instalar a CLI atualizando suas informações de repositório brew e executando o comando `install`:

```bash
brew update && brew install azure-cli
```

É possível executar a CLI do Azure com o comando `az`. Para entrar, use o comando [az login](/cli/azure/reference-index#az-login).

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Para saber mais sobre os diferentes métodos de autenticação, consulte [Conectar com a CLI do Azure 2.0](authenticate-azure-cli.md).

## <a name="troubleshooting"></a>solução de problemas

Se você encontrar um problema ao instalar a CLI através do Homebrew, aqui estão alguns erros comuns. Se você tiver um problema não abordado aqui, [arquive um problema no github](https://github.com/Azure/azure-cli/issues).

### <a name="unable-to-find-python-or-installed-packages"></a>Não é possível localizar o Python ou os pacotes instalados

Pode haver uma pequena incompatibilidade de versão ou outro problema durante a instalação do homebrew. A CLI não usa um ambiente virtual Python, portanto, ela se baseia em localizar a versão instalada do Python. Uma possível correção é instalar e revincular a dependência `python3` do Homebrew.

```bash
brew update && brew install python3 && brew upgrade python3
brew link --overwrite python3
```

### <a name="cli-version-1x-is-installed"></a>A versão 1.x da CLI está instalada

Se tiver sido instalada uma versão desatualizada, pode ser devido a um cache de homebrew obsoleto. Siga as instruções de [atualização](#Update).

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
