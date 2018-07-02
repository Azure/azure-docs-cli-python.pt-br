---
title: Extensões disponíveis para a CLI do Azure 2.0
description: Uma lista completa das extensões com suporte oficial para a CLI do Azure 2.0.
author: derekbekoe
ms.author: debekoe
manager: routlaw
ms.date: 06/25/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: bd93775373c8e779dff8a3af3c721e31d0e038c0
ms.sourcegitcommit: f4a4b1a1cd8be99abeaa655ef4797b97518a52a0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2018
ms.locfileid: "36943219"
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
| [azure-batch-cli-extensions](https://github.com/Azure/azure-batch-cli-extensions) | 2.2.2 | Comandos adicionais para trabalhar com o serviço de Lote do Azure |  |
| [azure-cli-iot-ext](https://github.com/azure/azure-iot-cli-extension) | 0.4.5 | Fornece a camada de comandos do plano de dados para o Azure Hub IoT, IoT Edge e o Serviço de Provisionamento de Dispositivos |  |
| [botservice](https://github.com/Azure/azure-cli-extensions) | 0.0.3 | Suporte para recursos de visualização do Serviço de Bot do Azure 2017-12-01 | sim |
| [dev-spaces-preview](https://github.com/Azure/azure-cli-extensions) | 0.1.5 | Os Espaços de Desenvolvimento fornecem uma experiência de desenvolvimento Kubernetes rápida e iterativa para equipes. | sim |
| [dns](https://github.com/Azure/azure-cli-extensions) | 0.0.2 | Uma extensão da CLI do Azure para zonas DNS |  |
| [eventgrid](https://github.com/Azure/azure-cli-extensions) | 0.2.1 | Suporte para recursos do Azure EventGrid 2018-05-01-preview | sim |
| [image-copy-extension](https://github.com/Azure/azure-cli-extensions) | 0.0.7 | Suporte para copiar imagens de vm gerenciadas entre regiões |  |
| [keyvault-preview](https://github.com/Azure/azure-keyvault-cli-extension) | 0.1.3 | Visualizar comandos do Azure Key Vault. | sim |
| [managementgroups](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Uma extensão da CLI do Azure para grupos de gerenciamento |  |
| [managementpartner](https://github.com/Azure/azure-cli-extensions) | 0.1.2 | Suporte à versão prévia de Parceiro de Gerenciamento |  |
| [rdbms-vnet](https://github.com/Azure/azure-cli-extensions) | 10.0.0 | Suporte para regras de Rede Virtual no Azure MySQL e recursos do Azure PostgreSQL |  |
| [signalr](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Suporte à versão prévia de gerenciamento de signalr. | sim |
| [storage-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/storage-preview) | 0.1.2 | Fornece uma visualização para recursos de armazenamento futuras. | sim |
| [subscription](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Suporte à versão prévia de gerenciamento de assinatura. |  |
| [webapp](https://github.com/Azure/azure-cli-extensions) | 0.2.6 | Uma extensão da CLI do Azure para gerenciar recursos de appservice | sim |
