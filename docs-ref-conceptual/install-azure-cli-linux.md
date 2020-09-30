---
title: Instalar a CLI do Azure para Linux manualmente
description: Como instalar a CLI do Azure no Linux manualmente
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/09/2018
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 9f70e0eb4f518c8fbb7bf8803b93b8b8246d8791
ms.sourcegitcommit: 5d29362589078b66d15f5cd494fe903a5195658d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/25/2020
ms.locfileid: "91225653"
---
# <a name="install-azure-cli-on-linux-manually"></a>Instalar CLI do Azure no Linux manualmente

Se não houver nenhum pacote da CLI do Azure para a sua distribuição, instale a CLI manualmente executando um script.

[!INCLUDE [current-version](includes/current-version.md)]

> [!NOTE]
> É altamente recomendável instalar a CLI com um gerenciador de pacotes. Um gerenciador de pacotes garante que você sempre obtenha as atualizações mais recentes, além da estabilidade dos componentes da CLI. Verifique e veja se há um pacote de distribuição antes de instalar manualmente.

## <a name="prerequisites"></a>Prerequisites

A CLI requer o seguinte software:

* [Python 3.6.x, 3.7.x ou 3.8.x](https://www.python.org/downloads/). 
* [libffi](https://sourceware.org/libffi/)
* [OpenSSL 1.0.2](https://www.openssl.org/source/)

> [!IMPORTANT]
>
> A CLI não é mais compatível com o Python 2.7 desde a versão `2.1.0`. Não há garantia de que as novas versões serão executadas com o Python 2.7 corretamente.

## <a name="install-or-update"></a>Instalar ou atualizar

Instalar e atualizar a CLI exige executar novamente o script de instalação. Instale a CLI executando `curl`.

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

O script também pode ser baixado e executado localmente. Talvez você precise reiniciar o shell para que as alterações entrem em vigor.

É possível executar a CLI do Azure com o comando `az`. Para entrar, use o comando [az login](/cli/azure/reference-index#az-login).

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Para saber mais sobre os diferentes métodos de autenticação, confira [Entrar com a CLI do Azure](authenticate-azure-cli.md).

## <a name="troubleshooting"></a>solução de problemas

Aqui estão alguns problemas comuns observados durante uma instalação manual. Se você tiver um problema não abordado aqui, [arquive um problema no GitHub](https://github.com/Azure/azure-cli/issues).

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

### <a name="proxy-blocks-connection"></a>Conexão de blocos de proxy

[!INCLUDE[configure-proxy](includes/configure-proxy.md)]

Para obter os scripts de instalação, o proxy precisa permitir conexões HTTPS com os seguintes endereços:

* `https://aka.ms/`
* `https://azurecliprod.blob.core.windows.net/`
* `https://pypi.python.org`
* Pontos de extremidade usados pelo gerenciador de pacotes da distribuição (se houver) para pacotes essenciais

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

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

## <a name="next-steps"></a>Próximas etapas

Agora que você instalou a CLI do Azure, faça um tour breve de seus recursos e comandos comuns.

> [!div class="nextstepaction"]
> [Introdução à CLI do Azure](get-started-with-azure-cli.md)