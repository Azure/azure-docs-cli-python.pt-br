---
title: Extensões disponíveis para a CLI do Azure 2.0
description: Uma lista completa das extensões com suporte oficial para a CLI do Azure 2.0.
author: derekbekoe
ms.author: debekoe
manager: routlaw
ms.date: 04/02/18
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 794ea005816b33fe78ca6c15b86dcf94ace3eaa8
ms.sourcegitcommit: c9da729f4a42a839f13106f7589deaa0ca19cc4e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/06/2018
---
# <a name="available-extensions-for-the-azure-cli-20"></a>Extensões disponíveis para a CLI do Azure 2.0

Este artigo é uma lista completa das extensões disponíveis para a CLI do Azure 2.0 que são oferecidas e têm suporte da Microsoft.

A lista de extensões também está disponível diretamente na CLI. Para obtê-la, execute [az extension list-available](/cli/azure/extension#az-extension-list-available):

```azurecli
az extension list-available --output table
```

| NOME | Versão | Resumo | Visualização |
|------|---------|---------|---------|
| [aem](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Gerencie as Extensões de Monitoramento Aprimorado do Azure para SAP. |  |
| [alias](https://github.com/Azure/azure-cli-extensions) | 0.3.0 | Suporte para aliases de comando. | sim |
| [azure-batch-cli-extensions](https://github.com/Azure/azure-batch-cli-extensions) | 2.1.0 | Versão prévia de comandos adicionais do Lote do Azure. |  |
| [azure-cli-iot-ext](https://github.com/azure/azure-iot-cli-extension) | 0.4.1 | Fornece a camada de comandos do plano de dados para o Azure Hub IoT, IoT Edge e o Serviço de Provisionamento de Dispositivos. |  |
| [dns](https://github.com/Azure/azure-cli-extensions) | 0.0.2 | Suporte para a Visualização Pública do DNS Privado do Azure. |  |
| [image-copy-extension](https://github.com/Azure/azure-cli-extensions) | 0.0.5 | Copie imagens de região para região. |  |
| [managementgroups](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Suporte à versão prévia de Grupos de Gerenciamento. | sim |
| [managementpartner](https://github.com/Azure/azure-cli-extensions) | 0.1.2 | Suporte à versão prévia de Parceiro de Gerenciamento. | sim |
| [rdbms](https://github.com/Azure/azure-cli-extensions) | 0.0.5 | Suporte para Azure MySQL e Azure PostgreSQL. |  |
| [subscription](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Suporte à versão prévia de definições de assinatura. | sim |
| [webapp](https://github.com/Azure/azure-cli-extensions) | 0.2.0 | Criar e implantar recursos de serviço de aplicativo. | sim |
