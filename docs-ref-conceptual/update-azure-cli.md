---
title: Atualizar a CLI do Azure
description: Referência para a atualização da CLI do Azure
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 10/19/2020
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 91ed79b9f59af4ad070983eb7d0744bc85d09216
ms.sourcegitcommit: 9beaf9abb794f1006a56acee4e1cfb8ea7fe2405
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2020
ms.locfileid: "96850865"
---
# <a name="update-the-azure-cli"></a>Atualizar a CLI do Azure

Você pode contar com os gerenciadores de pacotes para atualizar uma instalação local da CLI do Azure em ambientes Windows, macOS e Linux (confira a seção `Update` em cada instrução de instalação específica da plataforma). A CLI também fornece comandos dentro ferramenta para atualização manual ou automática.

## <a name="manual-update"></a>Atualização manual
[!INCLUDE [az-upgrade](includes/az-upgrade.md)]

O `az upgrade` é compatível com o Windows, o macOS e algumas distribuições do Linux, desde que haja suporte para a instalação. Ele dá suporte apenas à atualização para a versão mais recente. Se você está executando a CLI do Azure por meio do Azure Cloud Shell, provavelmente já está usando a instalação da CLI do Azure mais recente. Exceto em casos como a versão ad hoc de uma versão de correção de bug secundária, você precisará esperar pelo próximo build do Azure Cloud Shell, já que não há suporte para `az upgrade` no Azure Cloud Shell.

Quando `azure-cli` já for a versão mais recente, a execução de `az upgrade` verificará e atualizará todas as [extensões](azure-cli-extensions-overview.md) instaladas.

## <a name="automatic-update"></a>Atualização automática

Por padrão, a atualização automática da CLI do Azure está desabilitada. Se você quiser acompanhar a versão mais recente, poderá habilitar a atualização automática por meio da [configuração](/cli/azure/config).

```azurecli
az config set auto-upgrade.enable=yes
```

A CLI do Azure verificará novas versões regularmente e solicitará que você atualize após terminar a execução de qualquer comando quando a atualização estiver disponível.

A mensagem do prompt e as mensagens de saída durante a atualização poderão interromper o resultado do comando se ele for atribuído a alguma variável ou estiver em um fluxo automatizado. Para evitar a interrupção, você pode usar a configuração a seguir para permitir que a atualização ocorra automaticamente sem confirmação e mostrar apenas avisos e erros durante a atualização.

```azurecli
az config auto-upgrade.prompt=no
```

Por padrão, todas as extensões instaladas também serão atualizadas. Você pode desabilitar a atualização de extensão por meio da configuração.

```azurecli
az config auto-upgrade.all=no
```

> [!NOTE]
> Aguarde até que `az upgrade` seja concluído antes de prosseguir para o próximo conjunto de comandos, caso contrário, as novas versões da CLI (+ extensões) poderão ter alterações da falha.

Se você decidir não usar mais o recurso de atualização automática para casos como manter scripts de comando em execução de modo estável, você poderá desativá-lo por meio da configuração.
```azurecli
az config set auto-upgrade.enable=no
```
