---
title: "Extensões da CLI 2.0 do Azure"
description: "Usar extensões com a CLI 2.0 do Azure"
keywords: "CLI do Azure, Extensões"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 10/30/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 930073324d68f9719ce5035388120e7b6ac41a98
ms.sourcegitcommit: 93f6bd2c199774fcb3b43c6b14d714196873ed04
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/07/2017
---
# <a name="using-extensions-with-the-azure-cli-20"></a>Usar extensões com a CLI 2.0 do Azure

Extensões são módulos individuais não enviados com a CLI do Azure, o que lhe permite adicionar funcionalidades por meio de novos comandos. Elas podem ser ofertas experimentais ou de pré-lançamento, ferramentas especializadas da Microsoft para suas necessidades ou até extensões gravadas por você mesmo. As extensões possibilitam um nível de flexibilidade com a CLI que permite modificá-la conforme as suas necessidades, sem ter de enviar uma grande quantidade de pacotes adicionais que não são considerados parte do conjunto de recursos principais.

Este artigo ajuda a entender como instalar, atualizar e remover extensões da CLI. Ele também deve responder a perguntas comuns sobre o comportamento das extensões.

## <a name="finding-extensions"></a>Encontrar extensões

Para saber quais extensões estão disponíveis, use `az extension list-available`. Esse comando lista as extensões oficiais disponíveis, que são fornecidas e com suporte pela Microsoft.

## <a name="installing-extensions"></a>Instalar extensões

Depois de encontrar uma extensão para instalar, use `az extension add` para obtê-la. Se for uma extensão oficial da Microsoft listada em `az extension list-available`, instale a extensão pelo nome.

```azurecli
az extension add --name <extension-name>
```

Se a extensão for de um recurso externo ou se você tiver um link direto a ela, é possível fornecer a URL de origem ou o caminho local. Ela _deve_ ser um arquivo wheel Python compilado.

```azurecli
az extension add --source <URL-or-path>
```

Depois de instalada, a extensão pode ser encontrada no valor da variável do shell `$AZURE_EXTENSION_DIR`. Se essa variável tiver sua definição removida, por padrão, o valor é `$HOME/.azure/cliextensions` no Linux e macOS e `%USERPROFILE%\.azure\cliextensions` no Windows.

## <a name="updating-extensions"></a>Atualizar extensões

As extensões só podem ser atualizadas por nome:

```azurecli
az extension update --name <extension-name>
```

Se o nome de uma extensão não pode ser resolvido pela CLI por qualquer motivo, reinstale a extensão para atualizá-lo. Também há a possibilidade da extensão ter sido movida do modo de versão prévia e ter se tornado um comando interno da CLI. Nesse caso, atualize a CLI e desinstale a extensão.

## <a name="uninstalling-extensions"></a>Desinstalar extensões

Caso você não precise mais de uma extensão, ela pode ser removida com `az extension remove`,

```azurecli
az extension remove --name <extension-name>
```

Também é possível remover uma extensão manualmente, excluindo-a do local onde foi instalada. Esse será o valor de variável do shell `$AZURE_EXTENSION_DIR`. Se essa variável tiver sua definição removida, por padrão, o valor é `$HOME/.azure/cliextensions` no Linux e macOS e `%USERPROFILE%\.azure\cliextensions` no Windows.

```bash
rm -rf $AZURE_EXTENSION_DIR/<extension-name>
```

Recomenda-se fazer a desinstalação usando `az extension remove`.

## <a name="faq"></a>Perguntas frequentes

Aqui estão algumas respostas para outras perguntas comuns sobre extensões da CLI.

### <a name="what-file-formats-are-allowed-for-installation"></a>Quais formatos de arquivo são permitidos para instalação?

Atualmente, apenas wheels compilados do Python podem ser instalados como extensões.

### <a name="can-extensions-replace-existing-commands"></a>As extensões podem substituir os comandos existentes?

Sim. As extensões podem substituir os comandos existentes, mas antes de executar um comando que foi substituído, a CLI emitirá um aviso.

### <a name="how-can-i-tell-if-an-extension-is-in-pre-release"></a>Como posso saber se uma extensão está em pré-lançamento?

Uma extensão deve indicar, por meio de sua própria documentação e controle de versão, se está em pré-lançamento. Também é comum a Microsoft lançar comandos de versão prévia para a CLI como extensões, com planos para movê-las para a interface principal da CLI assim que o produto estiver fora da versão prévia.

### <a name="can-extensions-depend-upon-each-other"></a>As extensões podem depender umas das outras?

Não. As extensões devem ser pacotes individuais que não dependem um do outro. Isso porque a CLI não oferece nenhuma garantia sobre quando as extensões são carregadas. Assim, não se pode garantir que as dependências sejam atendidas. Ao instalar uma extensão, apenas essa extensão é instalada e ela deve continuar a funcionar mesmo que outras extensões sejam removidas.

### <a name="are-extensions-updated-along-with-the-cli"></a>As extensões são atualizadas juntamente com a CLI?

Não. As extensões devem ser atualizadas separadamente, conforme descrito na seção [Atualizar extensões](#updating-extensions).
