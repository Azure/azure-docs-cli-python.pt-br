---
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/26/2018
ms.topic: include
ms.openlocfilehash: ee0b2b0c8c557aa54255f28429bb3a174c0e21a9
ms.sourcegitcommit: 7f79860c799e78fd8a591d7a5550464080e07aa9
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/12/2019
ms.locfileid: "56158000"
---
### <a name="cli-fails-to-install-or-run-on-windows-subsystem-for-linux"></a>A CLI não consegue instalar nem ser executada no Subsistema Windows para Linux

Como o [Subsistema Windows para Linux (WSL)](/windows/wsl/about) é uma camada de tradução de chamadas do sistema com base na plataforma Windows, você pode encontrar um erro ao tentar instalar ou executar a CLI do Azure. A CLI depende de alguns recursos que podem apresentar um bug no WSL. Caso encontre um erro independentemente da forma de instalação da CLI, há uma boa chance de ser um problema com o WSL, e não com o processo de instalação da CLI.

Para solucionar os problemas de instalação do WSL e possivelmente resolvê-los:

* Se possível, execute um processo de instalação idêntico em um computador Linux ou em uma VM para ver se tem êxito. Se isso acontecer, é praticamente certo que o problema está relacionado ao WSL. Para iniciar uma VM Linux no Azure, consulte a documentação para [criar uma VM Linux no Portal do Azure](/azure/virtual-machines/linux/quick-create-portal).
* Verifique se você está executando a versão mais recente do WSL. Para obter a versão mais recente, [atualize sua instalação do Windows 10](https://support.microsoft.com/help/4027667/windows-10-update).
* Verifique se há [problemas em aberto](https://github.com/Microsoft/WSL/issues) com o WSL que possam endereçar o problema.
  Muitas vezes, haverá sugestões sobre como resolvê-lo ou informações sobre uma versão em que ele será corrigido.
* Se não houver nenhum problema existente seu caso, [registre um novo problema no WSL](https://github.com/Microsoft/WSL/issues/new) e inclua o máximo de informações possível.

Se continuar ocorrendo problemas de instalação ou execução no WSL, cogite [instalar a CLI para Windows](../install-azure-cli-windows.md).
