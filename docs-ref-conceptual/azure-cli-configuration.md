---
title: Opções de configuração da CLI do Azure
description: Como configurar a CLI do Azure 2.0
keywords: CLI do Azure, definição, configurações, Azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 12/13/2017
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: dac383fa0dbd785f9448514e3d0a3242e4853038
ms.sourcegitcommit: 42f1ba77b2f562d89dadd302655d1f02ee4b6130
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/17/2018
---
# <a name="azure-cli-20-configuration"></a>Configuração da CLI do Azure 2.0

A CLI do Azure 2.0 permite que a configuração de usuário substitua configurações internas, como o registro em log e coleta de dados, e fornece opções padrão para alguns parâmetros necessários. A CLI fornece um comando de conveniência para gerenciar alguns desses valores, `az configure`, e outros valores podem ser definidos em um arquivo de configuração ou com variáveis de ambiente.

Os valores de configuração usados pela CLI são avaliados na seguinte precedência, com os itens da parte superior da lista sendo prioridade.

1. Parâmetros de linha de comando
2. Variáveis de ambiente
3. Valores no arquivo de configuração ou definidos com `az configure`

## <a name="cli-configuration-with-az-configure"></a>Configurar a CLI com o az configure

Você define padrões para a CLI com o comando [az configure](/cli/azure/reference-index#az-configure).
Esse comando usa um argumento, `--defaults`, que é uma lista separada por espaços de pares `key=value`. Os valores fornecidos são usados pela CLI no lugar dos argumentos necessários.

A seguir há uma lista de chaves disponíveis que você pode usar.

| NOME | DESCRIÇÃO |
|------|-------------|
| group | O grupo de recursos padrão para usar para todos os comandos. |
| location | O local padrão para usar para todos os comandos. |
| web | O nome de aplicativo padrão para usar para os comandos `az webapp`. |
| vm | O nome de VM padrão para usar para os comandos `az vm`. |
| vmss | O nome de VMSS padrão para usar para os comandos `az vmss`. |
| acr | O nome de registro de contêiner padrão para usar para os comandos `az acr`. |
| acs | O nome de serviço de contêiner padrão para usar para os comandos `az acs`. |

Como exemplo, a seguir você vê como poderia definir o grupo de recursos e local padrão para todos os comandos.

```azurecli
az configure --defaults location=westus2 group=MyResourceGroup
```

## <a name="cli-configuration-file"></a>Arquivo de configuração da CLI

O arquivo de configuração da CLI contém outras configurações que são usadas para gerenciar o comportamento da CLI. O arquivo de configuração em si está localizado em `$AZURE_CONFIG_DIR/config`. O valor padrão de `AZURE_CONFIG_DIR` é `$HOME/.azure` no Linux e macOS, e `%USERPROFILE%\.azure` no Windows.

Os arquivos de configuração são gravados no formato de arquivo INI. Esses arquivos são compostos de seções que começam com um cabeçalho `[section-name]`, seguido por uma lista de entradas `key=value`. Os nomes de seção diferenciam maiúsculas de minúsculas, mas nomes de chave não.
Os comentários são qualquer linha que comece com um `#` ou `;`. Não são permitidos comentários em linha. Os valores boolianos diferenciam maiúsculas de minúsculas e são representados pelos valores a seguir.

* __Verdadeiro__: 1, yes, true, on
* __Falso__: 0, no, false, off

Aqui está um exemplo de um arquivo de configuração da CLI que desabilita quaisquer prompts de confirmação e define o log para o diretório `/var/log/azure`.

```
[core]
disable_confirm_prompt=Yes

[logging]
enable_log_file=yes
log_dir=/var/log/azure
```

Consulte a próxima seção para obter detalhes sobre todos os valores de configuração disponíveis e o que significam. Para obter detalhes completos sobre o formato de arquivo INI, consulte a [Documentação do Python sobe INI](https://docs.python.org/3/library/configparser.html#supported-ini-file-structure).

## <a name="cli-configuration-values-and-environment-variables"></a>Valores de configuração da CLI e variáveis de ambiente

A tabela a seguir contém todas as seções e as opções de nomes que podem ser colocadas em um arquivo de configuração. Suas variáveis de ambiente correspondentes podem ser definidas como `AZURE_{section}_{name}`, tudo em maiúsculas. Por exemplo, você pode definir a `storage_account` da seção `batchai` como padrão na variável `AZURE_BATCHAI_STORAGE_ACCOUNT`.

Valores com um padrão disponível não precisam estar presente nos argumentos de linha de comando, mesmo se for necessário.

| Seção | NOME      | type | DESCRIÇÃO|
|---------|-----------|------|------------|
| __core__ | output | string | O formato de saída padrão. Pode ser `json`, `jsonc`, `tsv` ou `table`. |
| | disable\_confirm\_prompt | booleano | Ativa e desativa prompts de confirmação. |
| | collect\_telemetry | booleano | Permitir que a Microsoft colete dados anônimos sobre o uso da CLI. Para obter informações de privacidade, consulte os [Termos de uso da CLI do Azure 2.0](http://aka.ms/AzureCliLegal). |
| __logging__ | enable\_log\_file | booleano | Ativar e desativar o registro em log. |
| | log\_dir | string | O diretório no qual gravar os logs. Por padrão, é `${AZURE_CONFIG_DIR}/logs`. |
| __storage__ | connection\_string | string | A cadeia de conexão padrão a ser usada para comandos `az storage`. |
| | conta | string | O nome de conta padrão a ser usado para comandos `az storage`. |
| | chave | string | A chave de conta padrão a ser usada para comandos `az storage`. |
| | sas\_token | string | O token SAS padrão a ser usado para comandos `az storage`. |
| __batchai__ | storage\_account | string | A conta de armazenamento padrão a ser usada para comandos `az batchai`. |
| | storage\_key | string | A chave de armazenamento padrão a ser usada para comandos `az batchai`. |
| __batch__ | conta | string | O nome de conta do Lote do Azure a ser usado para comandos `az batch`. |
| | access\_key | string | A chave de acesso padrão a ser usada para comandos `az batch`. Usado somente com autorização `aad`. |
| | endpoint | string | O ponto de extremidade padrão ao qual se conectar para comandos `az batch`. |
| | auth\_mode | string | O modo de autorização a ser usado para comandos `az batch`. Pode ser `shared_key` ou `aad`. |

> [!NOTE]
> Você pode ver outros valores em seu arquivo de configuração, mas eles são gerenciados diretamente por meio de comandos da CLI, incluindo `az configure`. Os valores listados na tabela acima são os únicos que você mesmo deve alterar.
