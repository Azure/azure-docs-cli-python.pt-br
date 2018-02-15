---
title: Instalar a CLI do Azure 2.0 para Linux manualmente
description: Como instalar a CLI do Azure 2.0 no Linux manualmente
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 4ab1f70308810e045b9a1d923fd809ad9848f6c6
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/15/2018
---
# <a name="install-azure-cli-20-on-linux-manually"></a>Instalar CLI do Azure 2.0 no Linux manualmente

Se não tiver um pacote para a CLI do Azure disponível em sua distribuição, você sempre poderá instalar a CLI manualmente executando um script de instalação.

> [!NOTE]
> É altamente recomendável que você use um gerenciador de pacotes para a CLI. Um gerenciador de pacotes garante que você sempre obtenha as atualizações mais recentes, além da estabilidade dos componentes da CLI. Verifique e veja se há um pacote de distribuição antes de instalar manualmente.

## <a name="prerequisites"></a>pré-requisitos

Para instalar a CLI, você precisa dos seguintes softwares disponíveis em seu sistema:

* [Python 2.7 ou Python 3. x](https://www.python.org/downloads/)
* [libffi](https://sourceware.org/libffi/)
* [OpenSSL 1.0.2](https://www.openssl.org/source/)

## <a name="install-or-update"></a>Instalar ou atualizar

Se você estiver instalando ou atualizando a CLI, precisa executar uma instalação completa. Assim que tiver os pré-requisitos, poderá instalar a CLI executando `curl`.

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

Você também pode baixar o script e executá-lo localmente. Talvez você precise reiniciar o shell para que as alterações entrem em vigor. Após a instalação, execute a CLI com o comando `az`.

## <a name="troubleshooting"></a>solução de problemas

Aqui estão alguns problemas comuns observados durante uma instalação manual. Se o problema não estiver listado aqui, [registre um problema no github](https://github.com/Azure/azure-cli/issues).
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

  ```
  <install location>/lib/azure-cli/az.completion
  ```

3. Se usar `bash` ou `zsh`, recarregue o cache de comando do shell.

  ```bash
  hash -r
  ```
