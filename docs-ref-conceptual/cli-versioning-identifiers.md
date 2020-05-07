---
title: Diferenças entre os produtos da CLI do Azure
description: Entenda como os produtos da CLI do Azure são nomeados e têm a versão controlada, e como atualizá-los.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 07/12/2018
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 3cd61d2166d03f7b9d58db1ee1cee77d17b5b336
ms.sourcegitcommit: ee64dc738cfe689a2a479e32a87bf420f96c31c8
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2020
ms.locfileid: "77779968"
---
# <a name="differences-between-azure-cli-products"></a><span data-ttu-id="9ee00-103">Diferenças entre os produtos da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="9ee00-103">Differences between Azure CLI products</span></span>

<span data-ttu-id="9ee00-104">A partir do final de junho de 2018, os números de versão explícitos foram removidos dos nomes de produto da CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="9ee00-104">As of the end of June 2018, explicit version numbers have been removed from Azure CLI product names.</span></span> <span data-ttu-id="9ee00-105">Essa alteração ajuda a eliminar a confusão que às vezes aparecia na documentação, em que os usuários eram instruídos a usar "a CLI do Azure", mas não ficava claro qual versão do produto estava sendo referenciada.</span><span class="sxs-lookup"><span data-stu-id="9ee00-105">This change helps eliminate confusion that sometimes showed up in documentation where users were told to use "the Azure CLI" but it was unclear what version of the product was being referenced.</span></span> <span data-ttu-id="9ee00-106">Se você estiver familiarizado com os nomes dos produto antigos, veja como eles foram alterados:</span><span class="sxs-lookup"><span data-stu-id="9ee00-106">If you're familiar with the old product names, here is how they have changed:</span></span>

* <span data-ttu-id="9ee00-107">As versões da CLI do Azure 2.0 e posteriores agora são chamadas apenas de "CLI do Azure".</span><span class="sxs-lookup"><span data-stu-id="9ee00-107">Azure CLI versions 2.0 and later are now referred to only as "Azure CLI."</span></span>
* <span data-ttu-id="9ee00-108">As versões mais antigas da CLI do Azure (1.x e anteriores) agora são chamadas de "CLI clássica do Azure".</span><span class="sxs-lookup"><span data-stu-id="9ee00-108">Earlier Azure CLI versions (1.x and lower) are now referred to as "Azure classic CLI."</span></span>

<span data-ttu-id="9ee00-109">A alteração do nome para CLI clássica do Azure deixa claro que essa ferramenta destina-se a ser usada apenas com o modelo de implantação clássico.</span><span class="sxs-lookup"><span data-stu-id="9ee00-109">The name change to Azure classic CLI makes it clear that this tool is meant to be used only with the classic deployment model.</span></span> <span data-ttu-id="9ee00-110">A CLI clássica é também não é mais atualizada ou recebe manutenção.</span><span class="sxs-lookup"><span data-stu-id="9ee00-110">The classic CLI is also no longer updated or maintained.</span></span> <span data-ttu-id="9ee00-111">Por essa e outras razões, é recomendável que você mude todas as implantações clássicas para usar o modelo do Azure Resource Manager e migre para a versão mais recente da CLI do Azure disponível.</span><span class="sxs-lookup"><span data-stu-id="9ee00-111">For this reason, and many more, it's recommended that you move any classic deployments to use the Azure Resource Manager model and migrate to the latest available version of the Azure CLI.</span></span>

<span data-ttu-id="9ee00-112">Se você ainda está usando a CLI clássica, pode aprender sobre o processo de migração nos seguintes artigos:</span><span class="sxs-lookup"><span data-stu-id="9ee00-112">If you are still using the classic CLI, you can learn about the process of migrating in the following articles:</span></span>

* [<span data-ttu-id="9ee00-113">Migrando do Clássico para o Azure Resource Manager</span><span class="sxs-lookup"><span data-stu-id="9ee00-113">Migrate from Classic to Azure Resource Manager</span></span>](/azure/virtual-machines/linux/migration-classic-resource-manager-overview)
* [<span data-ttu-id="9ee00-114">Instalar a CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="9ee00-114">Install the Azure CLI</span></span>](install-azure-cli.md)
* [<span data-ttu-id="9ee00-115">Migrando da CLI clássica do Azure para a CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="9ee00-115">Migrating from Azure classic CLI to Azure CLI</span></span>](https://github.com/Azure/azure-cli/blob/dev/doc/classic_cli_migration.md)
