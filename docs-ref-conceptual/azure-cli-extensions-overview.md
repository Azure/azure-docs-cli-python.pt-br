---
title: Extensões da CLI do Azure
description: Usando extensões com a CLI do Azure
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 08/06/2020
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: a399fde57b85b7e0b46e426d35cb67fd10efed1a
ms.sourcegitcommit: 5d29362589078b66d15f5cd494fe903a5195658d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/25/2020
ms.locfileid: "91225738"
---
# <a name="use-extensions-with-azure-cli"></a>Usar extensões com a CLI do Azure 

A CLI do Azure oferece a capacidade de carregar extensões. As extensões são arquivos wheel Python que não são enviadas como parte da CLI, mas executadas como comandos da CLI.
Com as extensões, você recebe acesso a comandos experimentais e de pré-lançamento, juntamente com a capacidade de escrever suas próprias interfaces de CLI. Este artigo aborda como gerenciar extensões e responde a perguntas comuns sobre seu uso.

## <a name="find-extensions"></a>Localizar extensões

Para ver as extensões fornecidas e mantidas pela Microsoft, use o comando [az extension list-available](/cli/azure/extension#az-extension-list-available).

```azurecli-interactive
az extension list-available --output table
```

Também hospedamos uma [lista de extensões](azure-cli-extensions-list.md) no site de documentação.

## <a name="install-extensions"></a>Instalar extensões

### <a name="install-extensions-manually"></a>Instalar extensões manualmente

Depois de encontrar uma extensão para instalar, use [az extension add](/cli/azure/extension#az-extension-add) para obtê-la. Se a extensão estiver listada em `az extension list-available`, é possível instalar a extensão pelo nome.

```azurecli-interactive
az extension add --name <extension-name>
```

Se a extensão for de um recurso externo ou se você tiver um link direto para ela, forneça a URL de origem ou o caminho local. A extensão _deve_ ser um arquivo wheel Python compilado.

```azurecli-interactive
az extension add --source <URL-or-path>
```

Depois de instalada, a extensão pode ser encontrada no valor da variável do shell `$AZURE_EXTENSION_DIR`. Se essa variável tiver sua definição removida, por padrão, o valor é `$HOME/.azure/cliextensions` no Linux e macOS e `%USERPROFILE%\.azure\cliextensions` no Windows.

### <a name="install-extensions-automatically"></a>Instalar extensões automaticamente

Quando você executa um comando de extensão que não está instalado, a CLI do Azure pode reconhecer o comando executado e instalar automaticamente a extensão para você da versão `2.10.0` em diante. Esse recurso, conhecido como **instalação dinâmica**, é habilitado por meio de configuração.
```azurecli-interactive
az config set extension.use_dynamic_install=yes_prompt
```

Use o comando de configuração a seguir para habilitar a instalação dinâmica sem um prompt.
```azurecli-interactive
az config set extension.use_dynamic_install=yes_without_prompt
```

Use o comando de configuração a seguir para desligar o recurso de instalação dinâmica e reverter para o comportamento padrão. O comando de extensão retornará um erro de comando não encontrado se a extensão não estiver instalada.
```azurecli-interactive
az config set extension.use_dynamic_install=no
```

Por padrão, um comando de extensão que solicita a instalação dinâmica não continuará sendo executado. Definindo a propriedade `run_after_dynamic_install` como `yes`, altere o comportamento padrão e faça o comando continuar.
```azurecli-interactive
az config set extension.run_after_dynamic_install=yes
```

## <a name="update-extensions"></a>Atualizar extensões

Se uma extensão tiver sido instalada pelo nome, atualize-a usando [az extension update](/cli/azure/extension#az-extension-update).

```azurecli-interactive
az extension update --name <extension-name>
```

Caso contrário, uma extensão poderá ser atualizada a partir da origem seguindo as instruções em [Instalar extensões](#install-extensions).

Se o nome de uma extensão não puder ser resolvido pela CLI, desinstale-a e tente reinstalá-la. A extensão também pode ter se tornado parte da CLI base.
Tente atualizar a CLI conforme descrito em [Instalar a CLI do Azure](install-azure-cli.md) e verifique se os comandos da extensão foram adicionados.

## <a name="uninstall-extensions"></a>Desinstalar as extensões

Se você já não precisar de uma extensão, remova-a com [az extension remove](/cli/azure/extension#az-extension-remove).

```azurecli-interactive
az extension remove --name <extension-name>
```

Também é possível remover uma extensão manualmente, excluindo-a do local onde foi instalada. A variável do shell `$AZURE_EXTENSION_DIR` define onde os módulos são instalados.
Se essa variável tiver sua definição removida, por padrão, o valor é `$HOME/.azure/cliextensions` no Linux e macOS e `%USERPROFILE%\.azure\cliextensions` no Windows.

```bash
rm -rf $AZURE_EXTENSION_DIR/<extension-name>
```

## <a name="faq"></a>Perguntas frequentes

Aqui estão algumas respostas para outras perguntas comuns sobre extensões da CLI.

### <a name="what-file-formats-are-allowed-for-installation"></a>Quais formatos de arquivo são permitidos para instalação?

Atualmente, apenas wheels compilados do Python podem ser instalados como extensões.

### <a name="can-extensions-replace-existing-commands"></a>As extensões podem substituir os comandos existentes?

Sim. As extensões podem substituir os comandos existentes, mas antes de executar um comando que foi substituído, a CLI emitirá um aviso.

### <a name="how-can-i-tell-if-an-extension-is-in-pre-release"></a>Como posso saber se uma extensão está em pré-lançamento?

O controle de versão e a documentação de uma extensão mostrará se ela está em pré-lançamento. Geralmente, a Microsoft lança comandos de visualização como extensões da CLI, com a opção de movê-los para o produto principal da CLI posteriormente. Quando os comandos são removidos das extensões, a extensão antiga deve ser desinstalada. 

### <a name="can-extensions-depend-upon-each-other"></a>As extensões podem depender umas das outras?

Não. Como a CLI não garante uma ordem de carga, as dependências não poderão ser atendidas. Remover uma extensão não afetará outras extensões.

### <a name="are-extensions-updated-along-with-the-cli"></a>As extensões são atualizadas juntamente com a CLI?

Não. As extensões devem ser atualizadas separadamente, conforme descrito em [Atualizar extensões](#update-extensions).

### <a name="how-to-develop-our-own-extension"></a>Como desenvolver sua própria extensão?
Confira o repositório oficial para receber mais ajuda. [Azure/azure-cli-extensions](https://github.com/Azure/azure-cli/tree/master/doc/extensions)