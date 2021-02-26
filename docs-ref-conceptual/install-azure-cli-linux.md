---
title: Instalar a CLI do Azure para Linux manualmente
description: Como instalar a CLI do Azure no Linux manualmente
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 12/15/2020
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
zone_pivot_group_filename: azure/zone-pivot-groups.json
zone_pivot_groups: cli-linux-installation-method
ms.openlocfilehash: 03c7e7e4915f48dce70d2bc2cab16b4688f8b5fd
ms.sourcegitcommit: 594e9c620a6f74f5eaedf91a7f6a791e03a64c74
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2021
ms.locfileid: "100630993"
---
# <a name="install-the-azure-cli-on-linux"></a>Instalar a CLI do Azure no Linux

É recomendável instalar a CLI do Azure usando o gerenciador de pacotes da distribuição do Linux. Selecione o gerenciador de pacotes apropriado para a sua distribuição nas opções acima.  Se você não tiver nenhum dos gerenciadores de pacotes listados, poderá instalar manualmente a CLI do Azure selecionando a opção *Instalar script*.

[!INCLUDE [current-version](includes/current-version.md)]

::: zone pivot="apt"

[!INCLUDE [cli-install-linux-apt](includes/cli-install-linux-apt.md)]

::: zone-end

::: zone pivot="dnf"

[!INCLUDE [cli-install-linux-apt](includes/cli-install-linux-dnf.md)]

::: zone-end

::: zone pivot="zypper"

[!INCLUDE [cli-install-linux-apt](includes/cli-install-linux-zypper.md)]

::: zone-end

::: zone pivot="script"

[!INCLUDE [cli-install-linux-apt](includes/cli-install-linux-script.md)]

::: zone-end

## <a name="next-steps"></a>Próximas etapas

Agora que você instalou a CLI do Azure, faça um tour breve de seus recursos e comandos comuns.

> [!div class="nextstepaction"]
> [Introdução à CLI do Azure](get-started-with-azure-cli.md)
