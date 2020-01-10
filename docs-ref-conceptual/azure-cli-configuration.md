---
title: Opções de configuração da CLI do Azure
description: Como configurar a CLI do Azure
keywords: CLI do Azure, definição, configurações, Azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 06/11/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 792a4bde1876bda620d31bccb7abcfc8e880332f
ms.sourcegitcommit: 503cf343422ab8d2a587d2ccb795953b8ad66376
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "75559987"
---
# <a name="azure-cli-configuration"></a>Configuração da CLI do Azure

A CLI do Azure permite a definição, pelo usuário, de configurações como registro em log, coleta de dados e valores de argumento padrão.
A CLI oferece um comando de conveniência para gerenciar alguns padrões, `az configure`. Outros valores podem ser definidos em um arquivo de configuração ou com variáveis de ambiente.

Os valores da configuração usados pela CLI são avaliados na seguinte precedência, com os itens na parte superior da lista sendo prioridade.

1. Parâmetros de linha de comando
2. Variáveis de ambiente
3. Valores no arquivo de configuração ou definidos com `az configure`

## <a name="cli-configuration-with-az-configure"></a>Configurar a CLI com o az configure

Você define padrões para a CLI com o comando [az configure](/cli/azure/reference-index#az-configure).
Esse comando usa um argumento, `--defaults`, que é uma lista separada por espaços de pares `key=value`. Os valores fornecidos são usados pela CLI no lugar dos argumentos necessários.

A tabela a seguir contém uma lista de chaves de configuração disponíveis.

| Nome | DESCRIÇÃO |
|------|-------------|
| group | O grupo de recursos padrão para usar para todos os comandos. |
| local | O local padrão para usar para todos os comandos. |
| web | O nome de aplicativo padrão para usar para os comandos `az webapp`. |
| vm | O nome de VM padrão para usar para os comandos `az vm`. |
| vmss | O nome do conjunto de dimensionamento de máquinas virtuais (VMSS) padrão que será usado em comandos `az vmss`. |
| acr | O nome de registro de contêiner padrão para usar para os comandos `az acr`. |

Como exemplo, a seguir você vê como poderia definir o grupo de recursos e local padrão para todos os comandos.

```azurecli-interactive
az configure --defaults location=westus2 group=MyResourceGroup
```

## <a name="cli-configuration-file"></a>Arquivo de configuração da CLI

O arquivo de configuração da CLI contém outras configurações que são usadas para gerenciar o comportamento da CLI. O arquivo de configuração em si está localizado em `$AZURE_CONFIG_DIR/config`. O valor padrão de `AZURE_CONFIG_DIR` é `$HOME/.azure` no Linux e macOS, e `%USERPROFILE%\.azure` no Windows.

Os arquivos de configuração são gravados no formato de arquivo INI. Esse formato de arquivo é definido por cabeçalhos de seção, seguidos por uma lista de entradas de chave-valor.

* Os cabeçalhos de seção são gravados como `[section-name]`. Os nomes de seção diferenciam maiúsculas de minúsculas.
* As entradas são gravadas como `key=value`. Os nomes de chave não diferenciam maiúsculas de minúsculas.
* Os comentários são qualquer linha que comece com um `#` ou `;`. Não são permitidos comentários em linha.

Os valores boolianos diferenciam maiúsculas de minúsculas e são representados pelos valores a seguir.

* __True__: 1, yes, true, on
* __False__: 0, no, false, off

Veja um exemplo de um arquivo de configuração da CLI que desabilita prompts de confirmação e define o log para o diretório `/var/log/azure`.

```ini
[core]
disable_confirm_prompt=Yes

[logging]
enable_log_file=yes
log_dir=/var/log/azure
```

Consulte a próxima seção para obter detalhes sobre todos os valores de configuração disponíveis e o que significam. Para obter detalhes completos sobre o formato de arquivo INI, consulte a [Documentação do Python sobe INI](https://docs.python.org/3/library/configparser.html#supported-ini-file-structure).

## <a name="cli-configuration-values-and-environment-variables"></a>Valores de configuração da CLI e variáveis de ambiente

A tabela a seguir contém todas as seções e as opções de nomes que podem ser colocadas em um arquivo de configuração. Suas variáveis de ambiente correspondentes estão definidas como `AZURE_{section}_{name}`, tudo em maiúsculas. Por exemplo, o padrão `storage_account` para `batchai` é definido na variável `AZURE_BATCHAI_STORAGE_ACCOUNT`.

Quando você fornece um valor padrão, esse argumento já não é exigido pelos comandos. Em vez disso, o valor padrão é usado.

| Seção | Nome      | Type | DESCRIÇÃO|
|---------|-----------|------|------------|
| __core__ | output | string | O formato de saída padrão. Pode ser `json`, `jsonc`, `tsv` ou `table`. |
| | disable\_confirm\_prompt | booleano | Ativa e desativa prompts de confirmação. |
| | collect\_telemetry | booleano | Permitir que a Microsoft colete dados anônimos sobre o uso da CLI. Para obter informações de privacidade, confira os [Termos de uso da CLI do Azure](http://aka.ms/AzureCliLegal). |
| __logging__ | enable\_log\_file | booleano | Ativar e desativar o registro em log. |
| | log\_dir | string | O diretório no qual gravar os logs. Por padrão, esse valor é `${AZURE_CONFIG_DIR}/logs`. |
| __storage__ | connection\_string | string | A cadeia de conexão padrão a ser usada para comandos `az storage`. |
| | account | string | O nome de conta padrão a ser usado para comandos `az storage`. |
| | chave | string | A chave de conta padrão a ser usada para comandos `az storage`. |
| | sas\_token | string | O token SAS padrão a ser usado para comandos `az storage`. |
| __batchai__ | storage\_account | string | A conta de armazenamento padrão a ser usada para comandos `az batchai`. |
| | storage\_key | string | A chave de armazenamento padrão a ser usada para comandos `az batchai`. |
| __batch__ | account | string | O nome de conta do Lote do Azure a ser usado para comandos `az batch`. |
| | access\_key | string | A chave de acesso padrão a ser usada para comandos `az batch`. Usado somente com autorização `aad`. |
| | endpoint | string | O ponto de extremidade padrão ao qual se conectar para comandos `az batch`. |
| | auth\_mode | string | O modo de autorização a ser usado para comandos `az batch`. Pode ser `shared_key` ou `aad`. |
| __nuvem__ | name | string | A nuvem padrão para todos os comandos `az`.  Os valores possíveis são `AzureCloud` (padrão), `AzureChinaCloud`, `AzureUSGovernment` e `AzureGermanCloud`. Para alterar as nuvens é possível usar o comando `az cloud set –name`.  Para obter um exemplo, consulte [Gerenciar Nuvens com a CLI do Azure](manage-clouds-azure-cli.md). |

> [!NOTE]
> Você pode ver outros valores em seu arquivo de configuração, mas eles são gerenciados diretamente por meio de comandos da CLI, incluindo `az configure`. Os valores listados na tabela acima são os únicos que você mesmo deve alterar.
