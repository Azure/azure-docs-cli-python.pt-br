---
title: Instalar a CLI clássica do Azure
description: Instalar a CLI clássica do Azure para Mac, Linux e Windows para começar a usar os serviços do Azure
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 06/11/2018
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 6e2032cf6db312474431796149b8dde990820671
ms.sourcegitcommit: bf84dfb62e910ea246586481863bb43d09d07795
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/04/2020
ms.locfileid: "87551431"
---
# <a name="install-the-azure-classic-cli"></a>Instalar a CLI clássica do Azure

> [!IMPORTANT]
> Este tópico descreve como instalar a CLI clássica do Azure. A CLI clássica foi preterida e só deve ser usada com o modelo de implantação clássico.
> Para todas as outras implantações, use [a CLI do Azure](/cli/azure).

Instale rapidamente a CLI clássica do Azure para usar comandos de software livre baseados em shell a fim de criar e gerenciar recursos no Microsoft Azure. Você tem várias opções para instalar essas ferramentas de plataforma cruzada em seu computador:

* **Pacote npm**: execute o npm (o gerenciador de pacotes para JavaScript) para instalar o pacote da CLI clássica do Azure em sua distribuição Linux ou sistema operacional. Requer Node.js e npm.
* **Instalador**: baixe um instalador para facilitar a instalação no macOS ou no Windows.
* **Contêiner do Docker**: comece a usar a CLI clássica em um contêiner do Docker pronto para ser executado. Requer um host do Docker.

Para obter mais opções e um histórico, consulte o repositório do projeto no [GitHub](https://github.com/azure/azure-xplat-cli).

Quando a CLI clássica do Azure estiver instalada conecte-a com `azure login` e execute os comandos`azure` na interface de linha de comando (Bash, Terminal, Prompt de comando e assim por diante) para trabalhar com os recursos do Azure.

## <a name="option-1-install-an-npm-package"></a>Opção 1: Instalar um pacote npm

Para instalar a CLI clássica de um pacote npm, você precisa baixar e instalar os [Node.js e npm mais recentes](https://nodejs.org/en/download/package-manager/). Em seguida, execute `npm install` para instalar o pacote azure-cli:

```bash
npm install -g azure-cli
```

Em distribuições Linux, talvez seja necessário usar `sudo` para executar o comando `npm` com êxito, da seguinte forma:

```bash
sudo npm install -g azure-cli
```

> [!NOTE]
> Se você precisa instalar ou atualizar o Node.js e o npm em seu sistema operacional, recomendamos que você instale o Node.js LTS versão 4.x ou posterior. Se você usar uma versão mais antiga, poderá obter erros de instalação.

Se preferir, você também poderá baixar um arquivo tar das [Versões do GitHub](https://github.com/Azure/azure-xplat-cli/releases). Em seguida, instale o pacote npm baixado da seguinte maneira (em distribuições Linux, talvez seja necessário usar `sudo`):

```bash
npm install -g <path to downloaded tar file>
```

## <a name="option-2-use-an-installer"></a>Opção 2: Usar um instalador

Se você usa um computador Windows ou Mac, há instaladores DMG e MSI disponíveis nas [Versões do GitHub](https://github.com/Azure/azure-xplat-cli/releases).

> [!TIP]
> No Windows, você também pode baixar o [Web Platform Installer](https://go.microsoft.com/?linkid=9828653) para instalar a CLI clássica. Esse instalador dá a opção de instalar o SDK do Azure e outras ferramentas de linha de comando.

## <a name="option-3-use-a-docker-container"></a>Opção 3: Usar um contêiner do Docker

Se você tiver configurado seu computador como um host do [Docker](https://docs.docker.com/engine/understanding-docker/), execute a CLI clássica do Azure em um contêiner do Docker. Execute o seguinte comando (em distribuições Linux, talvez seja necessário usar `sudo`):

```bash
docker run -it microsoft/azure-cli:0.10.17
```

## <a name="run-azure-classic-cli-commands"></a>Executar comandos da CLI clássica do Azure

Quando a CLI clássica do Azure estiver instalada, execute o comando `azure` na interface do usuário de linha de comando (Bash, Terminal, Prompt de comando e assim por diante). Por exemplo, para executar o comando de ajuda, digite o seguinte:

```azurecli-interactive
azure help
```

> [!NOTE]
> Em algumas distribuições Linux, você poderá receber um erro semelhante a `/usr/bin/env: ‘node’: No such file or directory`. Esse erro ocorre quando instalações recentes do Node.js são instaladas em /usr/bin/nodejs. Para corrigi-lo, crie um link simbólico para /usr/bin/node executando este comando:

```bash
sudo ln -s /usr/bin/nodejs /usr/bin/node
```

Para ver a versão da CLI clássica do Azure que você instalou, digite o seguinte:

```azurecli-interactive
azure --version
```

> [!NOTE]
> Ao usar a CLI clássica do Azure pela primeira vez, você verá uma mensagem perguntando se deseja permitir que a Microsoft colete informações de uso. A participação é voluntária. Se optar por participar, você poderá parar a qualquer momento executando `azure telemetry --disable`. Para habilitar a participação a qualquer momento, execute `azure telemetry --enable`.

## <a name="update-the-classic-cli"></a>Atualizar a CLI clássica

A Microsoft pode lançar versões atualizadas da CLI clássica do Azure. Reinstale a CLI clássica usando o instalador do seu sistema operacional ou executando o contêiner do Docker mais recente. Ou, caso tenha o Node.js e o npm mais recentes instalados, atualize-os digitando o que é mostrado abaixo (em distribuições Linux, talvez seja necessário usar `sudo`).

```bash
npm update -g azure-cli
```

## <a name="enable-tab-completion"></a>Ativar o recurso auto-completar com TAB

Há suporte à conclusão de tabulação de comandos da CLI clássica para Mac e Linux.

Para habilitá-lo no zsh, execute:

```bash
echo '. <(azure --completion)' >> .zshrc
```

Para habilitá-lo no bash, execute:

```bash
azure --completion >> ~/azure.completion.sh
echo 'source ~/azure.completion.sh' >> ~/.bash_profile
```

## <a name="next-steps"></a>Próximas etapas

* Para saber mais sobre a CLI clássica do Azure, baixar o código-fonte, relatar problemas ou colaborar com o projeto, visite o [Repositório GitHub para a CLI clássica do Azure](https://github.com/azure/azure-xplat-cli).
