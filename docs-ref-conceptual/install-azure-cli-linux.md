---
title: Instalar a CLI do Azure 2.0 para Linux manualmente
description: Como instalar a CLI do Azure 2.0 no Linux manualmente
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: c5c7ea61a35e915760081897e88d8c43b80919e0
ms.sourcegitcommit: 0e688704889fc88b91588bb6678a933c2d54f020
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/11/2018
ms.locfileid: "44388347"
---
# <a name="install-azure-cli-20-on-linux-manually"></a>Instalar CLI do Azure 2.0 no Linux manualmente

Se não houver nenhum pacote da CLI do Azure para a sua distribuição, instale a CLI manualmente executando um script.

> [!NOTE]
> É altamente recomendável instalar a CLI com um gerenciador de pacotes. Um gerenciador de pacotes garante que você sempre obtenha as atualizações mais recentes, além da estabilidade dos componentes da CLI. Verifique e veja se há um pacote de distribuição antes de instalar manualmente.

## <a name="prerequisites"></a>Pré-requisitos

A CLI requer o seguinte software:

* [Python 2.7 ou Python 3. x](https://www.python.org/downloads/)
* [libffi](https://sourceware.org/libffi/)
* [OpenSSL 1.0.2](https://www.openssl.org/source/)

## <a name="install-or-update"></a>Instalar ou atualizar

Instalar e atualizar a CLI exige executar novamente o script de instalação. Instale a CLI executando `curl`.

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

O script também pode ser baixado e executado localmente. Talvez você precise reiniciar o shell para que as alterações entrem em vigor.

É possível executar a CLI do Azure com o comando `az`. Para entrar, use o comando [az login](/cli/azure/reference-index#az-login).

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Para saber mais sobre os diferentes métodos de autenticação, consulte [Conectar com a CLI do Azure 2.0](authenticate-azure-cli.md).

## <a name="troubleshooting"></a>solução de problemas

Aqui estão alguns problemas comuns observados durante uma instalação manual. Se você tiver um problema não abordado aqui, [arquive um problema no github](https://github.com/Azure/azure-cli/issues).

### <a name="curl-object-moved-error"></a>Erro "Objeto movido" de cURL

Se você receber um erro de `curl` relacionado ao parâmetro `-L` ou uma mensagem de erro incluindo o texto "Objeto movido", tente usar a URL completa em vez da `aka.ms` de redirecionamento:

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a>`az` comando não encontrado

Se não conseguir executar o comando após a instalação e usar `bash` ou `zsh`, limpe o cache do hash de comando do shell. Executar

```bash
hash -r
```

e verificar se o problema foi resolvido.

O problema também pode ocorrer se você não reiniciou o shell após a instalação. Verifique se o local do comando `az` está no `$PATH`. A localização do comando `az` é

```bash
<install path>/bin
```

## <a name="uninstall"></a>Desinstalar

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

Desinstale a CLI excluindo diretamente os arquivos do local escolhido no momento da instalação. O local de instalação padrão é `$HOME`.

1. Remova os arquivos da CLI instalados.

  ```bash
  rm -r <install location>/lib/azure-cli
  rm <install location>/bin/az
  ```

2. Modifique o arquivo `$HOME/.bash_profile` para remover a seguinte linha:

  ```text
  <install location>/lib/azure-cli/az.completion
  ```

3. Se usar `bash` ou `zsh`, recarregue o cache de comando do shell.

  ```bash
  hash -r
  ```
