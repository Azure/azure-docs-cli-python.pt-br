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
1. <span data-ttu-id="2d56a-101">Execute o comando `login`.</span><span class="sxs-lookup"><span data-stu-id="2d56a-101">Run the `login` command.</span></span>

    ```azurecli-interactive
    az login
    ```

    <span data-ttu-id="2d56a-102">Se a CLI puder abrir o navegador padrão, ela o fará e carregará uma página de entrada do Azure.</span><span class="sxs-lookup"><span data-stu-id="2d56a-102">If the CLI can open your default browser, it will do so and load an Azure sign-in page.</span></span>

    <span data-ttu-id="2d56a-103">Caso contrário, abra uma página de navegador em [https://aka.ms/devicelogin](https://aka.ms/devicelogin) e insira o código de autorização exibido no terminal.</span><span class="sxs-lookup"><span data-stu-id="2d56a-103">Otherwise, open a browser page at [https://aka.ms/devicelogin](https://aka.ms/devicelogin) and enter the  authorization code displayed in your terminal.</span></span>

    <span data-ttu-id="2d56a-104">Se nenhum navegador da Web estiver disponível ou se não for possível abrir o navegador da Web, use o fluxo de código do dispositivo com **az login --use-device-code**.</span><span class="sxs-lookup"><span data-stu-id="2d56a-104">If no web browser is available or the web browser fails to open, use device code flow with **az login --use-device-code**.</span></span>

2. <span data-ttu-id="2d56a-105">Entre com suas credenciais de conta no navegador.</span><span class="sxs-lookup"><span data-stu-id="2d56a-105">Sign in with your account credentials in the browser.</span></span>
