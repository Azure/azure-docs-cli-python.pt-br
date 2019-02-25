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
### <a name="cli-fails-to-install-or-run-on-windows-subsystem-for-linux"></a><span data-ttu-id="3ee50-101">A CLI não consegue instalar nem ser executada no Subsistema Windows para Linux</span><span class="sxs-lookup"><span data-stu-id="3ee50-101">CLI fails to install or run on Windows Subsystem for Linux</span></span>

<span data-ttu-id="3ee50-102">Como o [Subsistema Windows para Linux (WSL)](/windows/wsl/about) é uma camada de tradução de chamadas do sistema com base na plataforma Windows, você pode encontrar um erro ao tentar instalar ou executar a CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="3ee50-102">Since [Windows Subsystem for Linux (WSL)](/windows/wsl/about) is a system call translation layer on top of the Windows platform, you might experience an error when trying to install or run the Azure CLI.</span></span> <span data-ttu-id="3ee50-103">A CLI depende de alguns recursos que podem apresentar um bug no WSL.</span><span class="sxs-lookup"><span data-stu-id="3ee50-103">The CLI relies on some features that may have a bug in WSL.</span></span> <span data-ttu-id="3ee50-104">Caso encontre um erro independentemente da forma de instalação da CLI, há uma boa chance de ser um problema com o WSL, e não com o processo de instalação da CLI.</span><span class="sxs-lookup"><span data-stu-id="3ee50-104">If you experience an error no matter how you install the CLI, there's a good chance it's an issue with WSL and not with the CLI install process.</span></span>

<span data-ttu-id="3ee50-105">Para solucionar os problemas de instalação do WSL e possivelmente resolvê-los:</span><span class="sxs-lookup"><span data-stu-id="3ee50-105">To troubleshoot your WSL installation and possibly resolve issues:</span></span>

* <span data-ttu-id="3ee50-106">Se possível, execute um processo de instalação idêntico em um computador Linux ou em uma VM para ver se tem êxito.</span><span class="sxs-lookup"><span data-stu-id="3ee50-106">If you can, run an identical install process on a Linux machine or VM to see if it succeeds.</span></span> <span data-ttu-id="3ee50-107">Se isso acontecer, é praticamente certo que o problema está relacionado ao WSL.</span><span class="sxs-lookup"><span data-stu-id="3ee50-107">If it does, your issue is almost certainly related to WSL.</span></span> <span data-ttu-id="3ee50-108">Para iniciar uma VM Linux no Azure, consulte a documentação para [criar uma VM Linux no Portal do Azure](/azure/virtual-machines/linux/quick-create-portal).</span><span class="sxs-lookup"><span data-stu-id="3ee50-108">To start a Linux VM in Azure, see the [create a Linux VM in the Azure Portal](/azure/virtual-machines/linux/quick-create-portal) documentation.</span></span>
* <span data-ttu-id="3ee50-109">Verifique se você está executando a versão mais recente do WSL.</span><span class="sxs-lookup"><span data-stu-id="3ee50-109">Make sure that you're running the latest version of WSL.</span></span> <span data-ttu-id="3ee50-110">Para obter a versão mais recente, [atualize sua instalação do Windows 10](https://support.microsoft.com/help/4027667/windows-10-update).</span><span class="sxs-lookup"><span data-stu-id="3ee50-110">To get the latest version, [update your Windows 10 installation](https://support.microsoft.com/help/4027667/windows-10-update).</span></span>
* <span data-ttu-id="3ee50-111">Verifique se há [problemas em aberto](https://github.com/Microsoft/WSL/issues) com o WSL que possam endereçar o problema.</span><span class="sxs-lookup"><span data-stu-id="3ee50-111">Check for any [open issues](https://github.com/Microsoft/WSL/issues) with WSL which might address your problem.</span></span>
  <span data-ttu-id="3ee50-112">Muitas vezes, haverá sugestões sobre como resolvê-lo ou informações sobre uma versão em que ele será corrigido.</span><span class="sxs-lookup"><span data-stu-id="3ee50-112">Often there will be suggestions on how to work around the problem, or information about a release where the issue will be fixed.</span></span>
* <span data-ttu-id="3ee50-113">Se não houver nenhum problema existente seu caso, [registre um novo problema no WSL](https://github.com/Microsoft/WSL/issues/new) e inclua o máximo de informações possível.</span><span class="sxs-lookup"><span data-stu-id="3ee50-113">If there are no existing issues for your problem, [file a new issue with WSL](https://github.com/Microsoft/WSL/issues/new) and make sure that you include as much information as possible.</span></span>

<span data-ttu-id="3ee50-114">Se continuar ocorrendo problemas de instalação ou execução no WSL, cogite [instalar a CLI para Windows](../install-azure-cli-windows.md).</span><span class="sxs-lookup"><span data-stu-id="3ee50-114">If you continue to have issues installing or running on WSL, consider [installing the CLI for Windows](../install-azure-cli-windows.md).</span></span>
