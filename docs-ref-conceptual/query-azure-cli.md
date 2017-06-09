---
title: Resultados do comando de consulta com a CLI do Azure 2.0
description: "Use --query para realizar consultas JMESPath na saída dos comandos da CLI do Azure 2.0."
keywords: CLI do Azure 2.0, JMESPath, consulta, Linux, Mac, Windows, OS X
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 5979acc5-21a5-41e2-a4b6-3183bfe6aa22
ms.openlocfilehash: 23c743210ccc506935f6e78489ca0df2b99d46a1
ms.sourcegitcommit: 4fd631a58cf19c494162510d073fbbbdf0524d16
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/05/2017
---
# <a name="using-jmespath-queries-with-azure-cli-20"></a>Como usar consultas JMESPath com a CLI do Azure 2.0

A CLI do Azure 2.0 usa o parâmetro `--query` para executar uma [consulta JMESPath](http://jmespath.org) nos resultados do comando `az`. JMESPath é uma linguagem de consulta eficiente para saídas JSON.  Se estiver familiarizado com consultas JMESPath, consulte um tutorial em [JMESPath.org/tutorial](http:/JMESPath.org/tutorial.html).

O parâmetro `Query` é suportado por cada tipo de recurso (Serviços de Contêiner, Aplicativos Web, VM, etc.) na CLI do Azure 2.0 e pode ser usado para várias finalidades diferentes.  Listamos vários exemplos abaixo.

## <a name="selecting-simple-properties"></a>Seleção de propriedades simples

O comando `list` simples com o formato de saída `table` retorna um conjunto estruturado com as propriedades mais comuns e simples para cada tipo de recurso em um formato tabular de fácil leitura.

```azurecli-interactive
az vm list --out table
```

```
Name         ResourceGroup    Location
-----------  ---------------  ----------
DemoVM010    DEMORG1          westus
demovm212    DEMORG1          westus
demovm213    DEMORG1          westus
KBDemo001VM  RGDEMO001        westus
KBDemo020    RGDEMO001        westus
```

Você pode usar o parâmetro `--query` para mostrar apenas o nome do Grupo de Recursos e o nome da VM para todas as máquinas virtuais em sua assinatura.

```azurecli-interactive
az vm list \
  --query [*].[name,resourceGroup] --out table
```

```
Column1     Column2
---------   -----------
DemoVM010   DEMORG1
demovm111   DEMORG1
demovm211   DEMORG1
demovm212   DEMORG1
demovm213   DEMORG1
demovm214   DEMORG1
demovm222   DEMORG1
KBDemo001VM RGDEMO001
KBDemo020   RGDEMO001
```

No exemplo anterior, observe que os cabeçalhos das colunas são "Coluna1" e "Coluna2".  Também é possível adicionar nomes ou rótulos amigáveis às propriedades selecionadas.  No exemplo a seguir, adicionamos os rótulos "VMName" e "RGName" às propriedades selecionadas "name" e "resourceGroup".


```azurecli-interactive
az vm list \
  --query "[].{RGName:resourceGroup, VMName:name}" --out table
```

```
RGName     VMName
---------  -----------
DEMORG1    DemoVM010
DEMORG1    demovm111
DEMORG1    demovm211
DEMORG1    demovm212
DEMORG1    demovm213
DEMORG1    demovm214
DEMORG1    demovm222
RGDEMO001  KBDemo001VM
RGDEMO001  KBDemo020
```

## <a name="selecting-complex-nested-properties"></a>Seleção de propriedades aninhadas complexas

Se a propriedade que você deseja selecionar estiver aninhada profundamente na saída JSON, será necessário fornecer o caminho completo para a propriedade aninhada. O exemplo a seguir mostra como selecionar o nome da VM e o tipo do SO a partir do comando de lista da vm.

```azurecli-interactive
az vm list \
  --query "[].{VMName:name,OSType:storageProfile.osDisk.osType}" --out table
```

```
VMName       OSType
-----------  --------
DemoVM010    Linux
demovm111    Linux
demovm211    Linux
demovm212    Linux
demovm213    Linux
demovm214    Linux
demovm222    Linux
KBDemo001VM  Linux
KBDemo020    Linux
```

## <a name="filter-with-the-contains-function"></a>Filtrar com a função contains

Você pode usar a função `contains` do JMESPath para refinar os resultados retornados na consulta.
No exemplo a seguir, o comando seleciona apenas as VMs com o texto "RGD" em seu nome.  

```azurecli-interactive
az vm list \
  --query "[?contains(resourceGroup,'RGD')].{ resource: resourceGroup, name: name }" --out table
```

```
Resource    VMName
----------  -----------
RGDEMO001   KBDemo001VM
RGDEMO001   KBDemo020
```

Com o exemplo a seguir, os resultados retornarão as VMs com o vmSize 'Standard_DS1'.

```azurecli-interactive
az vm list \
  --query "[?contains(hardwareProfile.vmSize, 'Standard_DS1')]" --out table
```

```
ResourceGroup    VMName     VmId                                  Location    ProvisioningState
---------------  ---------  ------------------------------------  ----------  -------------------
DEMORG1          DemoVM010  cbd56d9b-9340-44bc-a722-25f15b578444  westus      Succeeded
DEMORG1          demovm111  c1c024eb-3837-4075-9117-bfbc212fa7da  westus      Succeeded
DEMORG1          demovm211  95eda642-417f-4036-9475-67246ac0f0d0  westus      Succeeded
DEMORG1          demovm212  4bdac85d-c2f7-410f-9907-ca7921d930b4  westus      Succeeded
DEMORG1          demovm213  2131c664-221a-4b7f-9653-f6d542fbfa34  westus      Succeeded
DEMORG1          demovm214  48f419af-d27a-4df0-87f3-9481007c2e5a  westus      Succeeded
DEMORG1          demovm222  e0f59516-1d69-4d54-b8a2-f6c4a5d031de  westus      Succeeded
```

## <a name="filter-with-grep"></a>Filtrar com grep

O formato de saída `tsv` é um texto separado por tabulações sem cabeçalhos. Ele pode ser transferido para comandos como `grep` e `cut` para analisar ainda mais os valores específicos da saída `list`. No exemplo a seguir, o comando `grep` seleciona apenas as VMs com o texto "RGD" em seu nome.  O comando `cut` seleciona apenas o valor do oitavo campo (separado por tabulações) para mostrar na saída.

```azurecli-interactive
az vm list --out tsv | grep RGD | cut -f8
```

```
KBDemo001VM
KBDemo020
```

## <a name="explore-with-jpterm"></a>Explorar com jpterm

Você também pode transferir a saída do comando para [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) e testar sua consulta JMESPath lá.

```bash
pip install jmespath-terminal
az vm list | jpterm
```

