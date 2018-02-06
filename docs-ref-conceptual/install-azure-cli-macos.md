---
title: Instalar a CLI do Azure para macOS
description: Como instalar a CLI do Azure 2.0 no macOS
keywords: CLI do Azure, Instalar CLI do Azure, macos do azure, macos instalar azure
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/18
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 36fd2604677db0b7f820ee11884bf790fb1d75cb
ms.sourcegitcommit: 8606f36963e8daa6448d637393d1e4ef2c9859a0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/01/2018
---
# <a name="install-azure-cli-20-on-macos"></a>Instalar CLI do Azure 2.0 no macOS

Para a plataforma macOS, você pode instalar a CLI do Azure usando o [gerenciador de pacotes homebrew](http://brew.sh). O Homebrew torna mais fácil manter a instalação da CLI atualizada. O pacote da CLI foi testado em versões do macOS 10.9 e posteriores.

## <a name="install"></a>Instalar

O homebrew é a maneira mais fácil de gerenciar a instalação da CLI. Ele fornece maneiras convenientes de instalar, atualizar e desinstalar. Se você não tiver o homebrew disponível em seu sistema, [instale-o](https://docs.brew.sh/Installation.html) antes de continuar.

Você pode instalar a CLI atualizando suas informações de repositório brew e executando o comando `install`:

```bash
brew update && brew install azure-cli
```

É possível executar a CLI do Azure com o comando `az`.

## <a name="troubleshooting"></a>solução de problemas

Se você encontrar um problema ao instalar a CLI através do Homebrew, aqui estão alguns erros comuns. Se o problema não estiver listado aqui, [registre um problema no github](https://github.com/Azure/azure-cli/issues).

### <a name="unable-to-find-python-or-installed-packages"></a>Não é possível localizar o Python ou os pacotes instalados

Se a instalação não conseguir localizar o Python nem os pacotes instalados, poderá haver uma incompatibilidade de versão secundária ou outro problema que ocorreu durante a instalação do homebrew. Como a CLI não usa um ambiente virtual Python, ela depende de conseguir localizar as versões corretas do Python. Você pode corrigir esses problemas vinculando novamente a instalação do Python.

```bash
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
