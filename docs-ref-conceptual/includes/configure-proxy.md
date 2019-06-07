---
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/28/2019
ms.topic: include
ms.prod: azure
ms.technology: azure-cli
ms.openlocfilehash: 676f33377a4e7122941bc789c51465b7f34aa1d3
ms.sourcegitcommit: 08043c47d3ccf23522b91e6bba3932e312c04c7f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2019
ms.locfileid: "66516255"
---
Se você não conseguir se conectar a um recurso externo por causa de um proxy, verifique se as variáveis `HTTP_PROXY` e `HTTPS_PROXY` foram definidas corretamente no shell. Será preciso entrar em contato com o administrador do sistema para saber quais hosts e portas devem ser usados para esses proxies.

Esses valores são seguidos por vários programas do Linux, incluindo os que são usados no processo de instalação. Para definir esses valores:

```bash
# No auth
export HTTP_PROXY=http://[proxy]:[port]
export HTTPS_PROXY=https://[proxy]:[port]

# Basic auth
export HTTP_PROXY=http://[username]:[password]@[proxy]:[port]
export HTTPS_PROXY=https://[username]:[password]@[proxy]:[port]
```

> [!IMPORTANT]
> Se você estiver atrás de um proxy, as variáveis do shell precisarão ser definidas para se conectarem aos serviços do Azure com a CLI.
> Se você não estiver usando a autenticação básica, é recomendável exportar as variáveis no arquivo `.bashrc`.
> Sempre siga as políticas de segurança da sua empresa e os requisitos do administrador do sistema.
