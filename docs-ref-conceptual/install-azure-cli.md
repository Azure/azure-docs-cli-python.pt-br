---
title: Instalar a CLI do Azure 2.0
description: "Documentos de referência para a CLI 2.0 do Azure"
keywords: "CLI 2.0 do Azure, Referência da CLI 2.0 do Azure, Instalar a CLI 2.0 do Azure, CLI Python do Azure, Desinstalar a CLI 2.0 do Azure"
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 04/06/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: ea5c0ee1-c530-4a1e-a83f-e1be71f6d416
ms.openlocfilehash: 7065ed5270ef9bfc70beea81d0bc442a7b4df38c
ms.sourcegitcommit: c077bd5cbe07f7225714c41714d3981fa0d9928f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/16/2017
---
# <a name="install-azure-cli-20"></a>Instalar a CLI 2.0 do Azure

Instale hoje mesmo a nova versão da CLI do Azure!
Nós a aprimoramos e atualizamos para fornecer uma ótima experiência de linha de comando nativa para gerenciar os recursos do Azure.
Ela pode ser usada em Windows, Linux e macOS.
Para saber mais sobre a versão mais recente, veja as [notas de versão](release-notes-azure-cli.md).

> [!NOTE]
> Se você precisa da versão anterior da CLI do Azure, veja como [instalar o Azure 1.0](/azure/cli-install-nodejs).

## <a name="macos"></a>macOS

1. Instalar a CLI 2.0 do Azure com um comando `curl`.

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

2. Talvez você precise reiniciar o shell de comando para algumas alterações entrarem em vigor.

   ```bash
   exec -l $SHELL
   ```
   
3. Execute a CLI 2.0 do Azure no prompt de comando com o comando `az`.

> [!Note]
> Quando você instala com InstallAzureCli, `az component update` não tem suporte.
> Para atualizar para a CLI mais recente, execute `curl -L https://aka.ms/InstallAzureCli | bash` novamente.
> 
> Para desinstalar, confira as [instruções para a desinstalação manual](#uninstall).

## <a name="windows"></a>Windows

É possível instalar a CLI com o MSI e usá-la na linha de comando do Windows ou instalar a CLI com apt-get no Bash, no Ubuntu no Windows.

### <a name="msi-for-the-windows-command-line"></a>MSI para a linha de comando do Windows 

Para instalar a CLI no Windows e usá-la na linha de comando do Windows, baixe e execute o [msi](https://aka.ms/InstallAzureCliWindows).

> [!NOTE]
> Ao instalar com o msi, não há suporte para `az component`.
> Para atualizar para a última CLI, execute o [msi](https://aka.ms/InstallAzureCliWindows) novamente.
> 
> Para desinstalar a CLI, execute o [msi](https://aka.ms/InstallAzureCliWindows) novamente e escolha Desinstalar.

### <a name="apt-get-for-bash-on-ubuntu-on-windows"></a>apt-get para Bash no Ubuntu no Windows

1. Se você não tiver o Bash no Windows, [instale-o](https://msdn.microsoft.com/commandline/wsl/install_guide).

2. Abra o shell do Bash.

3. Modifique sua lista de fontes.

   ```bash
   echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
   ```

4. Execute os comandos sudo a seguir:

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

> [!NOTE]
> Quando você instala com apt-get, `az component` não tem suporte.
> Para atualizar a CLI, execute `sudo apt-get update && sudo apt-get install azure-cli` novamente.
> 
> Para desinstalar, execute `sudo apt-get remove azure-cli`.

## <a name="linux"></a>Linux

1. No Linux, talvez você precise instalar [pré-requisitos](#linux-prerequisites) específicos.

2. Instalar a CLI 2.0 do Azure com um comando `curl`.

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

3. Talvez você precise reiniciar o shell de comando para algumas alterações entrarem em vigor.

   ```bash
   exec -l $SHELL
   ```

4. Execute a CLI 2.0 do Azure no prompt de comando com o comando `az`.

> [!Note]
> Quando você instala com InstallAzureCli, `az component update` não tem suporte.
> Para atualizar para a CLI mais recente, execute `curl -L https://aka.ms/InstallAzureCli | bash` novamente.
> 
> Para desinstalar, confira as [instruções para a desinstalação manual](#uninstall).

## <a name="docker"></a>Docker

Vamos manter uma imagem de Docker pré-configurada com a CLI do Azure.

Instale a CLI do Azure usando `docker run`.

```bash
docker run azuresdk/azure-cli-python:<version>
```

Confira nossas [marcas do Docker](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/) para versões disponíveis.

> [!NOTE]
> Se você quiser acompanhar as chaves SSH do seu ambiente de usuário, use `-v ${HOME}:/root` para montar $HOME como `/root`.
>
> ```bash
> docker run -v ${HOME}:/root azuresdk/azure-cli-python:<version>
> ```

> [!NOTE]
> A imagem do Docker não oferece suporte ao recurso [`component` ](/cli/azure/component).
> Para atualizar a CLI 2.0 do Azure, use `docker run` para instalar a imagem mais recente ou a imagem específica que você deseja.

## <a name="apt-get"></a>apt-get

Para sistemas baseados em Debian/Ubuntu, instale a CLI 2.0 do Azure por meio de `apt-get`.

1. Modifique sua lista de fontes.

   - sistema de 32 bits

     ```bash
     echo "deb https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

   - sistema de 64 bits

     ```bash
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. Execute os comandos sudo a seguir:

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

> [!NOTE]
> Quando você instala com apt-get, `az component` não tem suporte.
> Para atualizar a CLI, execute `sudo apt-get update && sudo apt-get install azure-cli` novamente.
> 
> Para desinstalar, execute `sudo apt-get remove azure-cli`.

## <a name="linux-prerequisites"></a>Pré-requisitos do Linux

1. Se você não tiver, instale o [Python](https://www.python.org/downloads).

2. Dependendo de sua distribuição do Linux, instale os pré-requisitos.

   ```
   Platform              | Prerequisites
   ----------------------|---------------------------------------------
   Ubuntu 15.10 or 16.04 | sudo apt-get update && sudo apt-get install -y libssl-dev libffi-dev python-dev build-essential
   Ubuntu 12.04 or 14.04 | sudo apt-get update && sudo apt-get install -y libssl-dev libffi-dev python-dev
   Debian 8              | sudo apt-get update && sudo apt-get install -y libssl-dev libffi-dev python-dev build-essential
   Debian 7              | sudo apt-get update && sudo apt-get install -y libssl-dev libffi-dev python-dev
   CentOS 7.1 or 7.2     | sudo yum check-update; sudo yum install -y gcc libffi-devel python-devel openssl-devel
   RedHat 7.2            | sudo yum check-update; sudo yum install -y gcc libffi-devel python-devel openssl-devel
   SUSE OpenSUSE 13.2    | sudo zypper refresh && sudo zypper --non-interactive install gcc libffi-devel python-devel openssl-devel
   ```

## <a name="troubleshooting"></a>Solucionar problemas

### <a name="errors-with-curl-redirection"></a>Erros com o redirecionamento de rotação

Se você receber um erro do comando `curl` sobre o parâmetro `-L` ou um erro informando "Objeto Movido", tente usar a URL completa em vez da URL aka.ms:

```
# If you see this:
curl -L https://aka.ms/InstallAzureCli | bash
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100   175  100   175    0     0    562      0 --:--:-- --:--:-- --:--:--   560
bash: line 1: syntax error near unexpected token `<'
'ash: line 1: `<html><head><title>Object moved</title></head><body>

#### Try this instead:
curl https://azurecliprod.blob.core.windows.net/install | bash
```

## <a name="uninstall"></a>Desinstalar

Se você usou o script em https://aka.ms/InstallAzureCli para instalar a CLI, é possível desinstalá-la com estas etapas.

1. Remova os arquivos instalados.

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. Exclua a linha `<install location>/lib/azure-cli/az.completion` de `<install location>/.bash_profile`.

> [!Note]
> O local de instalação padrão é `/Users/<username>`.

Se você usou apt-get, o Docker ou o msi para instalar a CLI, use a mesma ferramenta para desinstalá-la.

## <a name="reporting-issues-and-feedback"></a>Relatando comentários e problemas

Se você encontrar erros com a ferramenta, emita um problema na seção [Problemas](https://github.com/Azure/azure-cli/issues) de nosso repositório do GitHub.
Para fornecer comentários a partir da linha de comando, experimente o comando `az feedback`.
