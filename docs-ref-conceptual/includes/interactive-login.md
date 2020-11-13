---
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: include
ms.openlocfilehash: 7aae9e9050306ee834858e528504ae87ff605fa0
ms.sourcegitcommit: 488d53525f1c647ea853d9227d95fdce35b9fb85
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2020
ms.locfileid: "93330977"
---
1. Execute o comando `login`.

    ```azurecli-interactive
    az login
    ```

    Se a CLI puder abrir o navegador padrão, ela o fará e carregará uma página de entrada do Azure.

    Caso contrário, abra uma página de navegador em [https://aka.ms/devicelogin](https://aka.ms/devicelogin) e insira o código de autorização exibido no terminal.

    Se nenhum navegador da Web estiver disponível ou se não for possível abrir o navegador da Web, use o fluxo de código do dispositivo com **az login --use-device-code**.

2. Entre com suas credenciais de conta no navegador.
