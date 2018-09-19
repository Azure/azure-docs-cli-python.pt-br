---
title: Extensões da CLI 2.0 do Azure
description: Usar extensões com a CLI 2.0 do Azure
keywords: CLI do Azure, Extensões
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 8df4c82253e958fdad37ef1551c051f3d17fb191
ms.sourcegitcommit: 0e688704889fc88b91588bb6678a933c2d54f020
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/11/2018
ms.locfileid: "44388534"
---
# <a name="use-extensions-with-azure-cli-20"></a>Usar extensões com a CLI do Azure 2.0

A CLI do Azure 2.0 oferece a capacidade de carregar extensões. As extensões são arquivos wheel Python que não são enviadas como parte da CLI, mas executadas como comandos da CLI.
Com as extensões, você recebe acesso a comandos experimentais e de pré-lançamento, juntamente com a capacidade de escrever suas próprias interfaces de CLI. Este artigo aborda como gerenciar extensões e responde a perguntas comuns sobre seu uso.

## <a name="find-extensions"></a>Localizar extensões

Para ver as extensões fornecidas e mantidas pela Microsoft, use o comando [az extension list-available](/cli/azure/extension#az-extension-list-available).

```azurecli-interactive
az extension list-available --output table
```

Também hospedamos uma [lista de extensões](azure-cli-extensions-list.md) no site de documentação.

## <a name="install-extensions"></a>Instalar extensões

Depois de encontrar uma extensão para instalar, use [az extension add](https://docs.microsoft.com/cli/azure/extension#az-extension-add) para obtê-la. Se a extensão estiver listada em `az extension list-available`, é possível instalar a extensão pelo nome.

```azurecli-interactive
az extension add --name <extension-name>
```

Se a extensão for de um recurso externo ou se você tiver um link direto para ela, forneça a URL de origem ou o caminho local. A extensão _deve_ ser um arquivo wheel Python compilado.

```azurecli-interactive
az extension add --source <URL-or-path>
```

Depois de instalada, a extensão pode ser encontrada no valor da variável do shell `$AZURE_EXTENSION_DIR`. Se essa variável tiver sua definição removida, por padrão, o valor é `$HOME/.azure/cliextensions` no Linux e macOS e `%USERPROFILE%\.azure\cliextensions` no Windows.

## <a name="update-extensions"></a>Atualizar extensões

Se uma extensão tiver sido instalada pelo nome, atualize-a usando [az extension update](https://docs.microsoft.com/cli/azure/extension#az-extension-update).

```azurecli-interactive
az extension update --name <extension-name>
```

Caso contrário, uma extensão poderá ser atualizada a partir da origem seguindo as instruções em [Instalar extensões](#install-extensions).

Se o nome de uma extensão não puder ser resolvido pela CLI, desinstale-a e tente reinstalá-la. A extensão também pode ter se tornado parte da CLI base.
Tente atualizar a CLI, conforme descrito em [Instalar a CLI do Azure 2.0](install-azure-cli.md) e verifique se os comandos da extensão foram adicionados.

## <a name="uninstall-extensions"></a>Desinstalar as extensões

Se você já não precisar de uma extensão, remova-a com [az extension remove](https://docs.microsoft.com/cli/azure/extension#az-extension-remove).

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
