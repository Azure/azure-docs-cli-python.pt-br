---
title: Instalar a CLI do Azure 2.0 para Linux manualmente
description: Como instalar a CLI do Azure 2.0 no Linux manualmente
keywords: CLI do Azure, Instalar CLI do Azure, linux do azure, linux instalar azure
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 11/01/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ROBOTS: NOINDEX,NOFOLLOW
ms.openlocfilehash: cf1405cae70762146f63bc6629edc0dd1d949fff
ms.sourcegitcommit: 3eef136ae752eb90c67af604d4ddd298d70b1c9d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/06/2018
---
# <a name="install-azure-cli-20-on-linux-manually"></a>Instalar CLI do Azure 2.0 no Linux manualmente

Se você não tiver um pacote para a CLI do Azure disponível em sua distribuição, sempre poderá instalar a CLI manualmente executando um script de instalação. Se tiver um pacote disponível, este sempre será o método de instalação recomendado.

## <a name="prerequisites"></a>Pré-requisitos

Para instalar a CLI, você precisará do seguinte software disponível em seu sistema:

* [Python 2.7 ou Python 3. x](https://www.python.org/downloads/)
* [libffi](https://sourceware.org/libffi/)
* [OpenSSL 1.0.2](https://www.openssl.org/source/)

## <a name="install-or-update-manually"></a>Instalar ou atualizar manualmente

Se você estiver instalando ou atualizando a CLI, precisará executar uma instalação completa. Assim que tiver os pré-requisitos, poderá instalar a CLI executando `curl`.

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

Se preferir ou não tiver o `curl` em seu sistema, poderá baixar o script e executá-lo localmente. Talvez você precise reiniciar o shell para que as alterações entrem em vigor. Após a instalação, execute a CLI com o comando `az`.

## <a name="troubleshooting"></a>solução de problemas

### <a name="curl-object-moved-error"></a>Erro "Objeto movido" de cURL

Se você receber um erro de `curl` relacionado ao parâmetro `-L` ou uma mensagem de erro incluindo o texto "Objeto movido", tente usar a URL completa em vez da `aka.ms` de redirecionamento:

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a>`az` comando não encontrado

Após a instalação, se não puder executar o comando, talvez seja necessário limpar o cache do hash de comando do shell. Executar

```bash
hash -r
```

e ver se o problema foi resolvido.

Isso também poderá ocorrer se você não reiniciou o shell após a instalação. Verifique se o local do comando `az` está no `$PATH`.

Se você executou o script de instalação, isso irá:

```bash
<install path>/bin
```

## <a name="unstinall-manually"></a>Desinstalar manualmente

Se você decidiu desinstalar a CLI do Azure, lamentamos sua saída. Antes de desinstalar, use o comando `az feedback` para nos fornecer algumas razões por ter escolhido desinstalar e como poderíamos melhorar a experiência da CLI. Queremos assegurar que a CLI do Azure não tenha bugs e seja amigável o máximo possível. Você também pode [registrar um problema do github](https://github.com/Azure/azure-cli/issues).

Você pode desinstalar a CLI excluindo diretamente os arquivos do local de instalação. O local de instalação deve ter sido selecionado no momento da instalação, se você instalou via script `https://aka.ms/InstallAzureCLI`. O local de instalação padrão é `$HOME`.

Primeiro, remova os arquivos CLI instalados:

```bash
rm -r <install location>/lib/azure-cli
rm <install location>/bin/az
```

Então, modifique o arquivo `$HOME/.bash_profile` para remover a linha:

```
<install location>/lib/azure-cli/az.completion
```

E, por fim, recarregue o cache de comando do shell se ele usar um. Os usuários `bash` e `zsh` precisarão executar esta etapa:

```bash
hash -r
```
