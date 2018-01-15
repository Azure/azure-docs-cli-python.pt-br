---
title: Instalar a CLI do Azure para macOS
description: Como instalar a CLI do Azure 2.0 no macOS
keywords: CLI do Azure, Instalar CLI do Azure, macos do azure, macos instalar azure
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 10/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ROBOTS: NOINDEX,NOFOLLOW
ms.openlocfilehash: e615d2b3ab3b1307e982cb1d4d456633440afdf6
ms.sourcegitcommit: 3eef136ae752eb90c67af604d4ddd298d70b1c9d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/06/2018
---
# <a name="install-azure-cli-20-on-macos"></a>Instalar CLI do Azure 2.0 no macOS

Para a plataforma macOS, você pode instalar a CLI do Azure usando o [gerenciador de pacotes homebrew](http://brew.sh) ou manualmente. O método preferencial de instalação é com o homebrew para que seja mais fácil instalar, atualizar e desinstalar se você precisar.

## <a name="use-homebrew-to-install"></a>Usar o homebrew para instalar

O homebrew é a maneira mais fácil de gerenciar a instalação da CLI. Ele fornece maneiras convenientes de instalar, atualizar e desinstalar. É parecido com outros gerenciadores de pacotes, como o `apt` ou `yum`.
Se você não tiver o homebrew disponível em seu sistema, [instale-o](https://docs.brew.sh/Installation.html) antes de continuar.

### <a name="install-with-homebrew"></a>Instalar com o homebrew

Você pode instalar a CLI atualizando suas informações de repositório brew e executando o comando `install`:

```bash
brew update && brew install azure-cli
```

É possível executar a CLI do Azure com o comando `az`.

### <a name="update-with-homebrew"></a>Atualizar com o homebrew

A CLI é atualizada regularmente com correções de bugs, aprimoramentos, novos recursos e funcionalidade de visualização. Uma nova versão fica disponível aproximadamente a cada duas semanas. Você precisará atualizar as informações do repositório local, assim como o pacote da CLI.

```bash
brew update && brew upgrade azure-cli
```

### <a name="troubleshooting"></a>solução de problemas

Você encontrou um problema ao instalar ou atualizar a CLI com o homebrew? Veja alguns erros comuns que podem ocorrer e maneiras de diagnosticá-los e resolvê-los.

#### <a name="unable-to-find-python-or-installed-packages"></a>Não é possível localizar o Python ou os pacotes instalados

Se a instalação não conseguir localizar o Python nem os pacotes instalados, poderá haver uma incompatibilidade de versão secundária ou outro problema que ocorreu durante a instalação do homebrew. Como a CLI não usa um virtualenv, ela depende de conseguir localizar as versões corretas do Python instaladas pelo homebrew. Você pode corrigir esses problemas vinculando novamente a instalação do Python:

```bash
brew link --overwrite python3
```

#### <a name="the-cli-version-is-out-of-date"></a>A versão da CLI está desatualizada

Se você achar que a versão instalada da CLI pode estar desatualizada, precisará executar um comando `brew update`, seguido de `brew upgrade azure-cli`. Se isso não atualizar a CLI, lembre que os pacotes homebrew podem ser implementados mais lentamente que as versões gerais. Se precisar de instalações mais atuais da CLI, deverá [instalar manualmente](#manage-the-cli-manually).

### <a name="uninstall-with-homebrew"></a>Desinstalar com o homebrew

Se você decidiu desinstalar a CLI do Azure, lamentamos sua saída. Antes de desinstalar, use o comando `az feedback` para nos fornecer algumas razões por ter escolhido desinstalar e como poderíamos melhorar a experiência da CLI. Queremos assegurar que a CLI do Azure não tenha bugs e seja amigável o máximo possível. Você também pode [registrar um problema do github](https://github.com/Azure/azure-cli/issues).

Se você instalou com o homebrew, também deve usá-lo para desinstalar.

```bash
brew uninstall azure-cli
```

## <a name="install-the-cli-manually"></a>Instalar a CLI manualmente

Se você não pode ou não deseja depender do homebrew para gerenciar a instalação da CLI, pode instalar manualmente.

Siga as [instruções de instalação manual do Linux](install-azure-cli-linux.md) para instalar manualmente no macOS. as versões 10.9 e posterior do macOS devem incluir todas as dependências necessárias.
