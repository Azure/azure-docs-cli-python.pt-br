---
title: Tipos de referência da CLI do Azure
description: Uma explicação sobre status e tipos de referência
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 08/14/2020
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 2b6b3c5faef66e714cddf7b07126ba14af8c149b
ms.sourcegitcommit: fd8c3e32f0f50feb6fea33ead636a80a050bcf2a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2020
ms.locfileid: "88714334"
---
# <a name="overview-azure-cli-reference-types-and-status"></a>Visão geral: Status e tipos de referência da CLI do Azure

A CLI do Azure tem tipos de referência diferentes que, às vezes, são descritos de maneira intercambiável com os status de referência.  Este artigo explica a diferença entre um tipo e um status da CLI do Azure e fornece informações para trabalhar com ambos.

## <a name="azure-cli-syntax-components"></a>Componentes da sintaxe da CLI do Azure

A sintaxe da CLI do Azure é uma combinação de referências, comandos e parâmetros.  Geralmente, o comando de referência completa é simplesmente chamado de **comando**.

| Serviço do Azure | Referência | Subserviço de referência | Comando | Comando de referência completa | Exemplos de parâmetro
|-|-|-|-|-|-|
| CLI do Azure | [az configure](/cli/azure/reference-index#az-configure) | | | az configure | --defaults, --list-default, --scope
| Rede do Azure | [az network](/cli/azure/network) | application-gateway | create | [az network application-gateway create](/cli/azure/network/application-gateway#az-network-application-gateway-create) | --name, --resource-group, --capacity
| Azure DevOps | [az pipelines](/cli/azure/pipelines) | agente | list | [az pipelines agent list](/cli/azure/pipelines/agent) | --pool-id, --agent-name, --demands

## <a name="reference-types"></a>Tipos de referência

Um tipo de referência informa se o comando de referência faz parte do serviço primário da CLI do Azure ou se é um complemento opcional.  Há dois tipos de comandos de referência da CLI do Azure: **principal** e **extensão**.

|         | Núcleo  | Extensão
|-|-|-|
| **Referências** | Fazem parte do serviço primário da CLI do Azure | São comandos de referência opcionais que devem ser instalados
| **Instalar** | Em conjunto com o [MSI Installer]() | Individualmente com [az extension add]()|
| **Lançado** | Com base em um agendamento | Conforme novos recursos ou atualizações ficam disponíveis
| **Status** | Pode ser GA, versão prévia ou experimental | Também pode ser GA, versão prévia ou experimental

Todas as referências da CLI do Azure podem ser executadas no Windows, no macOS, no Linux, no Docker e no Azure Cloud Shell.

### <a name="core"></a>Núcleo

As referências da CLI do Azure que foram publicadas como parte permanente da CLI são chamadas **referências principais**.  Todas as referências principais são instaladas com a CLI do Azure e não é possível escolher um subconjunto de referências.  Se você executar a CLI por meio do Azure Cloud Shell, as referências principais estarão sempre atualizadas.  Confira a [Lista de referências principais da CLI do Azure](/cli/azure/reference-index) para obter uma lista completa de comandos de referência principais.

### <a name="extension"></a>Extensão

As extensões não são enviadas como parte da CLI, mas executadas como comandos da CLI.  Algumas extensões são parte permanente da CLI do Azure, mas, muitas vezes, uma extensão dará a você acesso a comandos experimentais e de versão prévia privada.  Uma única referência, como **az iot hub**, pode ter comandos principais e de extensão.  Veja quatro exemplos:

| Comando de referência completa | É principal | É extensão
|-|-|-|
| az iot hub list | sim |
| az iot hub query | | sim
| az iot hub certificate create | sim |
| az iot hub device identify create | | sim

> [!IMPORTANT]
> Você deve instalar uma extensão antes de usá-la executando o comando [az extension add](/cli/azure/extension#az-extension-add).

Saiba mais sobre referências de extensão, incluindo instalação e atualização em [Usar extensões com a CLI do Azure](azure-cli-extensions-overview.md).  Examine as [dicas wiki](https://github.com/Azure/azure-network-cli-extension/wiki/Tips) sobre extensão para maximizar o uso.  Confira [Extensões disponíveis para a CLI do Azure](azure-cli-extensions-list.md) para obter uma lista completa de comandos de referência de extensão.

## <a name="reference-status"></a>Status de referência

Independentemente do tipo, as referências da CLI do Azure se enquadram em três categorias de status: **GA** (Disponibilidade Geral), **versão prévia pública** ou **experimental**.  É o status do comando de referência, não o tipo, que determina a estabilidade e o nível de suporte.

| | GA  | Versão prévia pública | Habilitação
|-|-|-|-|
| **Estabilidade** | Permanente | Sujeito aos termos de [Versões prévias do Microsoft Azure](/support/legal/preview-supplemental-terms/) | Mudará para a versão prévia pública ou poderá ser removida
| **Nível de suporte** | Completo | Parcial | Nenhum

Embora a maioria dos comandos e parâmetros de uma única referência tenha um único status, esse nem sempre é o caso.  Uma referência em GA que está sendo criada para oferecer mais comandos pode ter comandos de referência em GA, versão prévia e experimental.  Normalmente, em resposta a comentários públicos e conforme novos parâmetros são adicionados para aumentar a funcionalidade, um único comando também pode ter parâmetros que se enquadram em categorias de status diferentes.  Veja exemplos de referências que têm status diferentes:

| Comando de referência completa | Parâmetros | Tipo | GA | Versão prévia pública | Habilitação
|-|-|-|-|-|-|
| az network dns zone list | Tudo | Núcleo | sim |
| az network dns zone create | --name, --resource-group, --if-none-match, --parent-name | Núcleo | sim |
|  | --newFutureParameter1 | Núcleo | | sim
|  | --newFutureParameter2 | Núcleo | | | sim
| az network vhub list | Tudo |Extensão | sim
| az network vhub create | --address-prefix, --name, --resource-group, -vwan, --location, --sku |Extensão | sim
|  | --newFutureParameter1 |Extensão | | sim
|  | --newFutureParameter2|Extensão | | | sim
| az network firewall create | Tudo | Extensão | | | sim

> [!NOTE]
> Avisos que indicam **versão prévia pública** ou **experimental** fazem parte da saída do comando da CLI do Azure e devem ser esperados.

## <a name="see-also"></a>Confira também

- [Lista de referências principais da CLI do Azure](/cli/azure/reference-index)
- [Extensões disponíveis para a CLI do Azure](azure-cli-extensions-list.md)
