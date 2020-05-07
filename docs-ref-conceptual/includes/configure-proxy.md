---
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/28/2019
ms.topic: include
ms.prod: azure
ms.technology: azure-cli
ms.openlocfilehash: 676f33377a4e7122941bc789c51465b7f34aa1d3
ms.sourcegitcommit: ee64dc738cfe689a2a479e32a87bf420f96c31c8
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2020
ms.locfileid: "66516255"
---
<span data-ttu-id="46ceb-101">Se você não conseguir se conectar a um recurso externo por causa de um proxy, verifique se as variáveis `HTTP_PROXY` e `HTTPS_PROXY` foram definidas corretamente no shell.</span><span class="sxs-lookup"><span data-stu-id="46ceb-101">If you're unable to connect to an external resource due to a proxy, make sure that you've correctly set the `HTTP_PROXY` and `HTTPS_PROXY` variables in your shell.</span></span> <span data-ttu-id="46ceb-102">Será preciso entrar em contato com o administrador do sistema para saber quais hosts e portas devem ser usados para esses proxies.</span><span class="sxs-lookup"><span data-stu-id="46ceb-102">You will need to contact your system administrator to know what host(s) and port(s) to use for these proxies.</span></span>

<span data-ttu-id="46ceb-103">Esses valores são seguidos por vários programas do Linux, incluindo os que são usados no processo de instalação.</span><span class="sxs-lookup"><span data-stu-id="46ceb-103">These values are respected by many Linux programs, including those which are used in the install process.</span></span> <span data-ttu-id="46ceb-104">Para definir esses valores:</span><span class="sxs-lookup"><span data-stu-id="46ceb-104">To set these values:</span></span>

```bash
# No auth
export HTTP_PROXY=http://[proxy]:[port]
export HTTPS_PROXY=https://[proxy]:[port]

# Basic auth
export HTTP_PROXY=http://[username]:[password]@[proxy]:[port]
export HTTPS_PROXY=https://[username]:[password]@[proxy]:[port]
```

> [!IMPORTANT]
> <span data-ttu-id="46ceb-105">Se você estiver atrás de um proxy, as variáveis do shell precisarão ser definidas para se conectarem aos serviços do Azure com a CLI.</span><span class="sxs-lookup"><span data-stu-id="46ceb-105">If you are behind a proxy, these shell variables must be set to connect to Azure services with the CLI.</span></span>
> <span data-ttu-id="46ceb-106">Se você não estiver usando a autenticação básica, é recomendável exportar as variáveis no arquivo `.bashrc`.</span><span class="sxs-lookup"><span data-stu-id="46ceb-106">If you are not using basic auth, it's recommended to export these variables in your `.bashrc` file.</span></span>
> <span data-ttu-id="46ceb-107">Sempre siga as políticas de segurança da sua empresa e os requisitos do administrador do sistema.</span><span class="sxs-lookup"><span data-stu-id="46ceb-107">Always follow your business' security policies and the requirements of your system administrator.</span></span>
