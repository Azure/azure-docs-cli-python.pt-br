---
title: "Notas de versão da CLI do Azure 2.0"
description: "Saiba mais sobre as últimas atualizações da CLI do Azure 2.0"
keywords: "Notas da versão, CLI do Azure 2.0"
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 04/03/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: ce0428f7-0a59-4e72-9237-d907b171af51
ms.openlocfilehash: 3bd4b9c059da3b841fc0757a11bc7ce78ec64b08
ms.sourcegitcommit: 66d997a5afcf32143a4d4817ec1608cbdf58a59f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2017
---
# <a name="azure-cli-20-release-notes"></a>Notas de versão da CLI do Azure 2.0

## <a name="may-10-2017"></a>10 de maio de 2017

Versão 2.0.6

* Renomeação do DocumentDB para CosmosDB
* Adição do RDBMS (MySQL, Postgres)
* Inclusão dos módulos Data Lake Analytics e Data Lake Store.
* Inclusão do módulo Serviços Cognitivos.
* Inclusão do módulo Service Fabric.
* Inclusão do módulo Interativo (renomeação de az-shell).
* Adição de suporte para comandos CDN.
* Remoção do módulo Contêiner.
* Adição de “az -v” como atalho para “az --version” ([nº 2926](https://github.com/Azure/azure-cli/issues/2926))
* Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))

```
azure-cli (2.0.6)

acr (2.0.4)
acs (2.0.6)
appservice (0.1.6)
batch (2.0.4)
cdn (0.0.2)
cloud (2.0.2)
cognitiveservices (0.1.2)
command-modules-nspkg (2.0.0)
component (2.0.4)
configure (2.0.6)
core (2.0.6)
cosmosdb (0.1.6)
dla (0.0.6)
dls (0.0.6)
feedback (2.0.2)
find (0.2.2)
interactive (0.3.1)
iot (0.1.5)
keyvault (2.0.4)
lab (0.0.4)
monitor (0.0.4)
network (2.0.6)
nspkg (3.0.0)
profile (2.0.4)
rdbms (0.0.1)
redis (0.2.3)
resource (2.0.6)
role (2.0.4)
sf (1.0.1)
sql (2.0.3)
storage (2.0.6)
vm (2.0.6)
```

### <a name="core"></a>Núcleo

* núcleo: captura de exceções causadas por um provedor não registrado e seu registro automático   
* desempenho: persistência do cache de tokens do ADAL na memória até o encerramento do processo ([nº 2603](https://github.com/Azure/azure-cli/issues/2603))
* Correção de bytes retornados da impressão digital hexadecimal -o tsv ([nº 3053](https://github.com/Azure/azure-cli/issues/3053))
* Melhoria do download do Certificado do Key Vault e da integração de SP do AAD ([nº 3003](https://github.com/Azure/azure-cli/issues/3003))
* Adição da localização do Python a “az —version” ([nº 2986](https://github.com/Azure/azure-cli/issues/2986))
* logon: suporte ao logon quando não há nenhuma assinatura ([nº 2929](https://github.com/Azure/azure-cli/issues/2929))
* núcleo: correção de uma falha ao fazer logon usando uma entidade de serviço duas vezes ([nº 2800](https://github.com/Azure/azure-cli/issues/2800))
* núcleo: permissão ao caminho do arquivo accessTokens.json para ser configurável por meio de um env var ([nº 2605](https://github.com/Azure/azure-cli/issues/2605))
* núcleo: permissão aos padrões configurados para serem aplicados em argumentos opcionais ([nº 2703](https://github.com/Azure/azure-cli/issues/2703))
* núcleo: melhoria do desempenho
* núcleo: Certificados de AC personalizados – suporte à configuração da variável de ambiente REQUESTS_CA_BUNDLE
* núcleo: configuração na nuvem – uso do ponto de extremidade do “Resource Manager” caso o ponto de extremidade de “Gerenciamento” não esteja definido

### <a name="acs"></a>ACS

* correção da contagem mestre e de agente para ser inteiro em vez de cadeia de caracteres
* exposição de “az acs create --no-wait” e “az acs wait” para a criação assíncrona
* exposição de “az acs create --validate” para validações de simulação
* remoção do perfil do Windows antes da chamada PUT ao comando scale ([nº 2755](https://github.com/Azure/azure-cli/issues/2755))

### <a name="appservice"></a>AppService

* functionapp: adição de suportes completos a functionapp, incluindo create, show, list, delete, hostname, ssl, etc.
* Adição do VSTS (Team Services) como uma opção de entrega contínua a “appservice web source-control config”
* Criação de “az webapp” para substituição de “az appservice web” (para compatibilidade com versões anteriores, “az appservice web” permanecerá por duas versões)
* Exposição de argumentos para configurar a implantação e as “pilhas em tempo de execução” em webapp create
* Exposição de “webapp list-runtimes”
* suporte à configuração de cadeias de conexão ([nº 2647](https://github.com/Azure/azure-cli/issues/2647))
* suporte à permuta de slots com visualização
* Correção de erros em comandos appservice ([nº 2948](https://github.com/Azure/azure-cli/issues/2948))
* Uso do grupo de recursos do plano do serviço de aplicativo para operações de certificado ([nº 2750](https://github.com/Azure/azure-cli/issues/2750))

### <a name="cosmosdb"></a>CosmosDB

* Renomeação do módulo DocumentDB para CosmosDB.
* Adição de suporte para APIs do plano de dados do DocumentDB: gerenciamento de banco de dados e de coleção
* Adição de suporte para habilitar o failover automático em contas de banco de dados
* Adição de suporte para nova política de consistência ConsistentPrefix

### <a name="data-lake-analytics"></a>Análises Data Lake

* Correção de um bug em que a filtragem no resultado e no estado das listas de trabalho gera um erro.
* Adição de suporte para o novo tipo de item de catálogo: pacote. acessado por meio de: `az dla catalog package`
* Possibilidade de listar os seguintes itens de catálogo no banco de dados (sem a necessidade de especificação de esquema):

  * Tabela
  * Função com valor de tabela
  * Visualizar
  * Estatísticas de Tabela. Isso também pode ser listado com um esquema, mas sem a especificação de um nome de tabela.

### <a name="data-lake-store"></a>Repositório Data Lake

* Atualização da versão do SDK do sistema de arquivos subjacente, que fornece melhor suporte para lidar com cenários de limitação do servidor.
* Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))
* Ausência de ajuda para mostrar o acesso. Adição em andamento. ([nº 2743](https://github.com/Azure/azure-cli/issues/2743))

### <a name="find"></a>Localizar

* melhoria dos resultados da pesquisa e permissão de controle de versão do índice de pesquisa

### <a name="keyvault"></a>KeyVault

* BC:`az keyvault certificate download` alteração de -e da cadeia de caracteres ou do binário para PEM ou DER a fim de representar melhor as opções
* BC: remoção de --expires e --not-before de `keyvault certificate create`, pois esses parâmetros não têm suporte no serviço.
* Adição do parâmetro --validity a `keyvault certificate create` para substituir seletivamente o valor em --policy
* Correção do problema em `keyvault certificate get-default-policy`, em que “expires” e “not_before” eram expostos, ao contrário de “validity_in_months”.
* Correção do cofre de chaves para importação de PEM e PFX ([nº 2754](https://github.com/Azure/azure-cli/issues/2754))

### <a name="lab"></a>Laboratório

* Adição dos comandos create, show, delete e list ao ambiente do laboratório.
* Adição dos comandos show e list para exibir modelos ARM no laboratório.
* Adição do sinalizador --environment a `az lab vm list` para filtrar as VMs por ambiente no laboratório.
* Adição do comando de conveniência `az lab formula export-artifacts` para exportar o scaffold de artefato em uma fórmula do Laboratório.
* Adição de comandos para gerenciar segredos em um Laboratório.

### <a name="monitor"></a>Monitoramento

* Correção de bug: modelagem de `--actions` de `az alert-rules create` para consumir a cadeia de caracteres JSON ([nº 3009](https://github.com/Azure/azure-cli/issues/3009))
* Correção de bug – as configurações de diagnóstico criam, mas não aceitam logs e métrica de comandos show ([nº 2913](https://github.com/Azure/azure-cli/issues/2913))

### <a name="network"></a>Rede

* Adição do comando `network watcher test-connectivity`.
* Adição de suporte para o parâmetro `--filters` de `network watcher packet-capture create`.
* Adição de suporte para drenagem de conexão do Gateway de Aplicativo.
* Adição de suporte para a configuração do conjunto de regras WAF do Gateway de Aplicativo.
* Adição de suporte para filtros de rota e regras do ExpressRoute.
* Adição de suporte para o roteamento geográfico do Gerenciador de Tráfego.
* Adição de suporte para seletores de tráfego baseados em política da conexão VPN.
* Adição de suporte para políticas IPsec da conexão VPN.
* Correção de um bug com `vpn-connection create` ao usar os parâmetros `--no-wait` ou `--validate`.
* Adição de suporte para gateways de VNet ativos/ativos
* Remoção de valores nulos na saída de comandos `network vpn-connection list/show`.
* BC: correção de um bug na saída de `vpn-connection create` 
* Correção de um bug em que o argumento “--key-length” de “vpn-connection create” não é analisado corretamente.
* Correção de um bug em `dns zone import`, em que os registros não são importados corretamente.
* Correção de um bug em que `traffic-manager endpoint update` não funciona.
* Adição de comandos de visualização “network watcher”.

### <a name="profile"></a>Perfil

* Suporte ao logon quando não há nenhuma assinatura encontrada ([nº 2560](https://github.com/Azure/azure-cli/issues/2560))
* Suporte ao nome curto do parâmetro em az account set --subscription ([nº 2980](https://github.com/Azure/azure-cli/issues/2980))

### <a name="redis"></a>Redis

* Adição do comando update que também adiciona a capacidade de dimensionar o Cache Redis
* Preterição do comando “update-settings”.

### <a name="resource"></a>Recurso

* Adição dos comandos de definição managedapp e managedapp ([nº 2985](https://github.com/Azure/azure-cli/issues/2985))
* Suporte aos comandos “provider operation” ([nº 2908](https://github.com/Azure/azure-cli/issues/2908))
* Suporte à criação de recurso genérico ([nº 2606](https://github.com/Azure/azure-cli/issues/2606))
* Correção da análise de recurso e da pesquisa de versão de API. ([nº 2781](https://github.com/Azure/azure-cli/issues/2781))
* Adição de documentos a az lock update. ([nº 2702](https://github.com/Azure/azure-cli/issues/2702))
* Erro ao tentar listar recursos de um grupo que não existe. ([nº 2769](https://github.com/Azure/azure-cli/issues/2769))
* [Computação] Correção de problemas com a atualização do conjunto de disponibilidade da VMSS e da VM. ([nº 2773](https://github.com/Azure/azure-cli/issues/2773))
* Correção de lock create e delete se parent-resource-path é None ([nº 2742](https://github.com/Azure/azure-cli/issues/2742))

### <a name="role"></a>Função

* create-for-rbac: garantia de que a data de término do SP não excederá a data de validade do certificado ([nº 2989](https://github.com/Azure/azure-cli/issues/2989))
* RBAC: adição de suporte completo a “ad group” ([nº 2016](https://github.com/Azure/azure-cli/issues/2016))
* função: correção de problemas na atualização de definição de função ([nº 2745](https://github.com/Azure/azure-cli/issues/2745))
* create-for-rbac: garantia de que a senha fornecida pelo usuário é coletada

### <a name="sql"></a>SQL

* Adição dos comandos az sql server list-usages e az sql db list-usages.
* SQL – capacidade de se conectar diretamente ao provedor de recursos ([nº 2832](https://github.com/Azure/azure-cli/issues/2832))

### <a name="storage"></a>Armazenamento

* Localização padrão da localização do grupo de recursos de `storage account create`.
* Adição de suporte para cópia incremental de blob
* Adição de suporte para upload de blobs de blocos grandes
* Alteração do tamanho do bloco para 100MB quando o arquivo a ser carregado é maior que 200GB

### <a name="vm"></a>VM

* avail-set: as contagens de domínio de UD e FD agora são opcionais

  observação: comandos da VM em nuvens soberanas Evite recursos relacionados ao disco gerenciado, incluindo os seguintes:
  1. az disk/snapshot/image
  2. az vm/vmss disk
  3. Em “az vm/vmss create”, use “—use-unmanaged-disk” para evitar o disco gerenciado Outros comandos deverão funcionar
* VM/VMSS: melhoria do texto de aviso ao gerar pares de chaves SSH
* VM/VMSS: suporte à criação com base em uma imagem do Marketplace que exige informações de plano ([nº 1209](https://github.com/Azure/azure-cli/issues/1209))


## <a name="april-3-2017"></a>3 de abril de 2017

Versão 2.0.2

Lançamos os componentes ACR, Batch, KeyVault, e SQL nessa versão.

```
azure-cli (2.0.2)
 
acr (2.0.0)
acs (2.0.2)
appservice (0.1.2)
batch (2.0.0)
cloud (2.0.0)
component (2.0.0)
configure (2.0.2)
container (0.1.2)
core (2.0.2)
documentdb (0.1.2)
feedback (2.0.0)
find (0.0.1b1)
iot (0.1.2)
keyvault (2.0.0)
lab (0.0.1)
monitor (0.0.1)
network (2.0.2)
nspkg (2.0.0)
profile (2.0.2)
redis (0.1.1b3)
resource (2.0.2)
role (2.0.1)
sql (2.0.0)
storage (2.0.2)
vm (2.0.2)
```

### <a name="core"></a>Núcleo

* Adicionar módulos acr, laboratório, monitor e localizar à lista padrão.
* Logon: ignorar locatário errado ([#2634](https://github.com/Azure/azure-cli/pull/2634))
* logon: definir assinatura padrão como um com o estado de "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))
* Adicionar comandos de espera e suporte --no-wait para mais comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))
* núcleo: suporte a logon usando a entidade de serviço com um certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))
* Adicione solicitação para parâmetros de modelo ausentes. ([#2364](https://github.com/Azure/azure-cli/pull/2364))
* Suporte à definição de valores padrão para os argumentos comuns como grupo de recursos padrão, Web padrão, vm padrão
* Suporte a logon para um locatário específico
 
### <a name="acs"></a>ACS

* [ACS] Adicionar suporte para configurar um cluster do ACS padrão ([&#2554;](https://github.com/Azure/azure-cli/pull/2554))
* Adicione suporte para solicitação de senha de chave ssh. ([#2044](https://github.com/Azure/azure-cli/pull/2044))
* Adicione suporte para clusters do windows. ([#2211](https://github.com/Azure/azure-cli/pull/2211))
* Alterne da função Proprietário para Colaborador. ([#2321](https://github.com/Azure/azure-cli/pull/2321))
 
### <a name="appservice"></a>AppService

* AppService: suporte para obter o endereço ip externo usado para registros de DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))
* AppService: suporte à associação de certificados curinga ([#2625](https://github.com/Azure/azure-cli/pull/2625))
* AppService: lista de suporte à publicação de perfis ([#2504](https://github.com/Azure/azure-cli/pull/2504))
* AppService - Aciona a sincronização de controle de origem após a configuração ([#2326](https://github.com/Azure/azure-cli/pull/2326))
 
### <a name="datalake"></a>DataLake

* Versão inicial do módulo do Data Lake Analytics.
* Versão inicial do módulo do Data Lake Store.
 
### <a name="docuemntdb"></a>DocuemntDB

* DocumentDB: Adicionar suporte para a listagem de cadeias de conexão ([#2580](https://github.com/Azure/azure-cli/pull/2580))

### <a name="vm"></a>VM

* [Compute] Adicionar suporte a AppGateway para criar o conjunto de dimensionamento de máquinas virtuais ([#2570](https://github.com/Azure/azure-cli/pull/2570))
* [VM/VMSS] Suporte aprimorado ao cache de disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))
* VM/VMSS: incorporar a lógica de validação de credenciais usada pelo portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))
* Adicionar comandos de espera e suporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))
* Conjunto de dimensionamento de máquinas virtuais: suporte à * para listar a exibição de instâncias em vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))
* Adicionar --secrets para o conjunto de dimensionamento de máquinas virtuais e VM ([#2212}(https://github.com/Azure/azure-cli/pull/2212))
* Permitir a criação de VMs com VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))

## <a name="february-27-2017"></a>27 de fevereiro de 2017

Versão 2.0.0

Essa versão da CLI do Azure 2.0 é a primeira versão “Disponível”.
A disponibilidade se aplica a esses módulos de comando:
- Serviço de Contêiner (acs)
- Computação (incluindo Gerenciador de Recursos, VM, conjunto de dimensionamento de máquinas virtuais, Managed Disks)
- Rede
- Armazenamento

Esses módulos de comando podem ser usados na produção e são compatíveis com o SLA do Microsoft padrão.
Você pode abrir problemas diretamente com o suporte da Microsoft ou em nossa [lista de problemas do github](https://github.com/azure/azure-cli/issues/).
Você pode fazer perguntas sobre [StackOverflow usando a marcação azure-cli](http://stackoverflow.com/questions/tagged/azure-cli) ou entrar em contato com a equipe do produto pelo endereço [ azfeedback@microsoft.com ](mailto:azfeedback@microsoft.com).
Você pode fornecer comentários a partir da linha de comando com o comando `az feedback`.

Os comandos nesses módulos são estáveis e a sintaxe não deve ser alterada em versões futuras dessa versão da CLI do Azure.

Para verificar a versão da CLI, utilize `az --version`.
A saída lista a versão da CLI (2.0.0 nessa versão), os módulos de comando individuais, as versões do Python e GCC que você está usando.

```
azure-cli (2.0.0)

acs (2.0.0)
appservice (0.1.1b5)
batch (0.1.1b4)
cloud (2.0.0)
component (2.0.0)
configure (2.0.0)
container (0.1.1b4)
core (2.0.0)
documentdb (0.1.1b2)
feedback (2.0.0)
iot (0.1.1b3)
keyvault (0.1.1b5)
network (2.0.0)
nspkg (2.0.0)
profile (2.0.0)
redis (0.1.1b3)
resource (2.0.0)
role (2.0.0)
sql (0.1.1b5)
storage (2.0.0)
vm (2.0.0)
 
Python (Darwin) 2.7.10 (default, Jul 30 2016, 19:40:32) 
[GCC 4.2.1 Compatible Apple LLVM 8.0.0 (clang-800.0.34)]
```

> [!Note]
> Alguns dos módulos de comando têm um “b*n*” ou “rc*n*” pós-fixado.
> Esses módulos de comando ainda estão em visualização e estarão disponíveis no futuro.

Também temos compilações de visualização diárias da CLI.
Para obter informações, consulte essas instruções sobre [como obter as compilações diárias](https://github.com/Azure/azure-cli#nightly-builds) e essas instruções sobre [configuração do desenvolvedor e código de contribuição](https://github.com/Azure/azure-cli#developer-setup).

Você pode relatar problemas com as compilações de visualização diárias das seguintes maneiras:
- Relatar problemas na [lista de problemas do github](https://github.com/azure/azure-cli/issues/)
- Entre em contato com a equipe do produto no endereço [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).
- Forneça comentários a partir da linha de comando com o comando `az feedback`.

