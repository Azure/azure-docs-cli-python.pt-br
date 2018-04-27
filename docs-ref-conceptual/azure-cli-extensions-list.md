---
title: Extensões disponíveis para a CLI do Azure 2.0
description: Uma lista completa das extensões com suporte oficial para a CLI do Azure 2.0.
author: derekbekoe
ms.author: debekoe
manager: routlaw
ms.date: 04/25/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: f22565e4b9bb4fe0656aae90724bf124611ef3c8
ms.sourcegitcommit: 2836d0739f55ba06cbc7c556fdf3e698a3fd1e4e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2018
---
# <a name="available-extensions-for-the-azure-cli-20"></a>Extensões disponíveis para a CLI do Azure 2.0

Este artigo é uma lista completa das extensões disponíveis para a CLI do Azure 2.0 que são oferecidas e têm suporte da Microsoft.

A lista de extensões também está disponível diretamente na CLI. Para obtê-la, execute [az extension list-available](/cli/azure/extension?view=azure-cli-latest#az-extension-list-available):

```azurecli
az extension list-available --output table
```

| NOME | Versão | Resumo | Visualização |
|------|---------|---------|---------|
| [aem](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Gerenciar Extensões de Monitoramento Aprimorado do Azure para SAP |  |
| [alias](https://github.com/Azure/azure-cli-extensions) | 0.5.1 | Suporte para aliases de comando | sim |
| [azure-batch-cli-extensions](https://github.com/Azure/azure-batch-cli-extensions) | 2.2.1 | Comandos adicionais para trabalhar com o serviço de Lote do Azure |  |
| [azure-cli-iot-ext](https://github.com/azure/azure-iot-cli-extension) | 0.4.3 | Fornece a camada de comandos do plano de dados para o Azure Hub IoT, IoT Edge e o Serviço de Provisionamento de Dispositivos |  |
| [dns](https://github.com/Azure/azure-cli-extensions) | 0.0.2 | Uma extensão da CLI do Azure para zonas DNS |  |
| [image-copy-extension](https://github.com/Azure/azure-cli-extensions) | 0.0.5 | Uma extensão da CLI do Azure que copia imagens de região para região. |  |
| [managementgroups](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Uma extensão da CLI do Azure para grupos de gerenciamento |  |
| [managementpartner](https://github.com/Azure/azure-cli-extensions) | 0.1.2 | Suporte à versão prévia de Parceiro de Gerenciamento |  |
| [rdbms](https://github.com/Azure/azure-cli-extensions) | 0.0.5 | Uma extensão da CLI do Azure que oferece suporte para o MySQL do Azure e o PostgreSQL do Azure. |  |
| [signalr](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Suporte à versão prévia de gerenciamento de signalr. | sim |
| [subscription](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Suporte à versão prévia de gerenciamento de assinatura. |  |
| [webapp](https://github.com/Azure/azure-cli-extensions) | 0.2.1 | Uma extensão da CLI do Azure para gerenciar recursos de appservice | sim |