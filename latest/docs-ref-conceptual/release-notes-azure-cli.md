---
title: "Notas de versão da CLI do Azure 2.0"
description: "Saiba mais sobre as últimas atualizações da CLI do Azure 2.0"
keywords: "Notas da versão, CLI do Azure 2.0"
author: sptramer
ms.author: sttramer
manager: douge
ms.date: 04/03/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: ce0428f7-0a59-4e72-9237-d907b171af51
ms.openlocfilehash: 72630c52b5e6afd69809ff19145717c0d65e0252
ms.sourcegitcommit: 3a490ae3a2a1b2e63a062806f9b720fa4c6be01e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/25/2017
---
# <a name="azure-cli-20-release-notes"></a>Notas de versão da CLI do Azure 2.0

## <a name="september-22-2017"></a>22 de setembro de 2017

Versão 2.0.1.8

### <a name="resource"></a>Recurso

* Suporte adicionado para mostrar as definições de políticas internas
* Parâmetro de modo de suporte adicionado para a criação de definições de política
* Suporte adicionado para definições de interface do usuário e modelos em `managedapp definition create`
* [ALTERAÇÃO SIGNIFICATIVA] O tipo de recurso `managedapp` foi alterado de `appliances` para `applications` e `applianceDefinitions` para `applicationDefinitions`

### <a name="network"></a>Rede

* Suporte adicionado para a zona de disponibilidade para os subcomandos `network lb` e `network public-ip`
* Suporte adicionado ao Emparelhamento IPv6 da Microsoft para `express-route`
* Adicionados `asg` comandos de grupo de segurança do aplicativo
* Adicionado o argumento `--application-security-groups` para `nic [create|ip-config create|ip-config update]`
* Adicionados os argumentos `--source-asgs` e `--destination-asgs` para `nsg rule [create|update]`
* Adicionados os argumentos `--ddos-protection` e `--vm-protection` para `vnet [create|update]`
* Adicionados os comandos `network [vnet-gateway|vpn-client|show-url]`

### <a name="storage"></a>Armazenamento

* Correção do problema onde `storage account network-rule` comandos poderão falhar após a atualização do SDK

### <a name="eventgrid"></a>Grade de eventos

* Atualizada SDK Python da Grade de Eventos do Azure para usar a versão de API mais recente "2017-09-15-preview"

### <a name="sql"></a>SQL

* Alterado o `sql server list` argumento `--resource-group` para ser opcional. Se não for especificado, todos os servidores sql na assinatura serão retornados
* Adicionado o `--no-wait` parâmetro para `db [create|copy|restore|update|replica create|create|update]` e `dw [create|update]`

### <a name="keyvault"></a>Keyvault

* Adicionado suporte para comandos Keyvault por trás de um proxy

### <a name="vm"></a>VM

* Adicionado suporte à zona de disponibilidade para `[vm|vmss|disk] create`
* Correção do problema onde usar`--app-gateway ID` com `vmss create` poderia causar uma falha
* Adicionado o argumento `--asgs` para `vm create`
* Suporte adicionado para executar comandos em VMs com `vm run-command`
* [VERSÃO PRÉVIA] Adicionado suporte para criptografia de disco VMSS com `vmss encryption`
* Suporte adicionado para realizar a manutenção em VMs com `vm perform-maintenance`

### <a name="acs"></a>ACS

* [VERSÃO PRÉVIA] Adicionado `--orchestrator-release` argumento para `acs create` para regiões de versão prévia do ACS

### <a name="appservice"></a>AppService

* Adicionada a capacidade para atualizar e mostrar as configurações de autenticação com `webapp auth [update|show]`

### <a name="backup"></a>Backup

* Versão prévia


## <a name="september-11-2017"></a>11 de setembro de 2017

Versão 2.0.17

### <a name="core"></a>Núcleo

* Módulo de comando habilitado para definir sua própria ID de correlação na telemetria
* Problema de despejo de JSON corrigido quando a telemetria é definida como modo de diagnóstico

### <a name="acs"></a>Acs

* Adicionado o comando `acs list-locations`
* Fez `ssh-key-file` vir com o valor padrão esperado

### <a name="appservice"></a>AppService

* Foi incluída a capacidade de criar um aplicativo Web em um grupo de recursos que não seja o plano de serviço ativo

### <a name="cdn"></a>CDN

* Foi corrigido o bug 'Não é possível interar CustomDomain' para `cdn custom-domain create`.

### <a name="extension"></a>Extensão

* Versão Inicial.

### <a name="keyvault"></a>Keyvault

* Foi corrigido o problema onde permissões diferenciavam maiúsculas de minúsculas para `keyvault set-policy`.

### <a name="network"></a>Rede

* `vnet list-private-access-services` renomeado para `vnet list-endpoint-services`
* Foi renomeado o argumento `--private-access-services` para `--service-endpoints` para `vnet subnet create/update`
* Foi adicionado suporte a vários intervalos de IP e intervalos de portas para `nsg rule create/update`
* Adicionado suporte ao SKU para `lb create`
* Adicionado suporte ao SKU para `public-ip create`

### <a name="resource"></a>Recurso

* Permitir a passagem de definições de parâmetro de políticas de recursos em `policy definition create` e`policy definition update`
* Permitir a passagem de valores de parâmetro para`policy assignment create`
* Permitir a passagem de JSON ou arquivo para todos os parâmetros
* Versão da API incrementada

### <a name="sql"></a>SQL

* Adicionados os comandos `sql server vnet-rule`

### <a name="vm"></a>VM

* Corrigido: Não atribuir acesso, a menos que `--scope` seja fornecido
* Corrigido: Usar a mesma nomenclatura de extensão do que o portal
* Foi removido `subscription` da saída de `[vm|vmss] create`
* Corrigido: SKU de armazenamento do `[vm|vmss] create` não é aplicada em discos de dados com uma imagem
* Corrigido: `vm format-secret --secrets` não aceita IDs de separados de nova linha

## <a name="august-31-2017"></a>31 de agosto de 2017

Versão 2.0.16

### <a name="keyvault"></a>Keyvault

* Correção do bug ao tentar resolver automaticamente a codificação secreta com `secret download`

### <a name="sf"></a>Sf

* Substituição de todos os comandos em favor da CLI do Service Fabric (sfctl)

### <a name="storage"></a>Armazenamento

* Correção de problema onde as contas de armazenamento não conseguiam ser criadas em regiões sem suporte ao recurso NetworkACLs
* Determinar o tipo de conteúdo e a codificação do conteúdo durante o upload de arquivo e de blob se nem o tipo de conteúdo nem a codificação de conteúdo forem especificados

## <a name="august-28-2017"></a>28 de agosto de 2017

Versão 2.0.15

### <a name="cli"></a>CLI

* Adicionada uma observação legal para `--version`.

### <a name="acs"></a>ACS

* Corrigidas as regiões de visualização.
* Corrigida a formatação padrão de `dns_name_prefix`.
* Otimização de saída de comando do ACS.

### <a name="appservice"></a>AppService

* [ALTERAÇÃO SIGNIFICATIVA] Corrigidas as inconsistências na saída de `az webapp config appsettings [delete|set]`
* Adicionado um novo alias de `-i` para `az webapp config container set --docker-custom-image-name`
* Exposto `az webapp log show`
* Expostos novos argumentos de `az webapp delete` para manter o plano, as métricas ou o registro de DNS do serviço de aplicativo
* Correção: detectar as configurações de slot corretamente

### <a name="iot"></a>IoT

* Correção #3934: Criação de política não limpa as políticas existentes

### <a name="network"></a>Rede

* [ALTERAÇÃO SIGNIFICATIVA] `vnet list-private-access-services` renomeado para `vnet list-endpoint-services`
* [ALTERAÇÃO SIGNIFICATIVA] Opção `--private-access-services` renomeada como `--service-endpoints` para `vnet subnet [create|update]`
* Adicionado suporte para vários IP e intervalos de porta para `nsg rule [create|update]`
* Adicionado suporte ao SKU para `lb create`
* Adicionado suporte ao SKU para `public-ip create`

### <a name="profile"></a>Perfil

* Exposto `--msi` e `--msi-port` para logon com a identidade de uma máquina virtual

### <a name="service-fabric"></a>Service Fabric

* Versão prévia
* Simplificadas as regras de registro de usuário/senha para comando
* Corrigido o prompt de senha para o usuário mesmo após a passagem do parâmetro
* Adicionado suporte para `registry_cred` vazio

### <a name="storage"></a>Armazenamento

* Habilitada a camada de blob de configuração
* Adicionados os argumentos `--bypass` e `--default-action` para `storage account [create|update]` para dar suporte ao serviço de túnel
* Comandos adicionados para adicionar as regras de rede virtual e com base em IP para `storage account network-rule`  
* Habilitada a criptografia de serviço por chave gerenciada de cliente
* [ALTERAÇÃO SIGNIFICATIVA] Opção `--encryption` renomeada como `--encryption-services` para o comando `az storage account create and az storage account update`
* Correção #4220: `az storage account update encryption` - incompatibilidade de sintaxe

### <a name="vm"></a>VM

* Corrigido o problema em que informações incorretas extras eram exibidas para `vmss get-instance-view` ao usar `--instance-id *`
* Adicionado suporte ao `--lb-sku` para `vmss create`: 
* Removidos nomes humanos da lista de bloqueio de nome de administrador para `[vm|vmss] create` 
* Corrigido o problema onde `[vm|vmss] create` geraria um erro se não for possível extrair informações do plano de uma imagem
* Corrigida uma falha ao criar um conjunto de dimensionamento de máquinas virtuais com um balanceamento de carga interno
* Corrigido o problema onde o argumento `--no-wait` não funcionava com `vm availability-set create`


## <a name="august-15-2017"></a>15 de agosto de 2017

Versão 2.0.14

### <a name="acs"></a>ACS

* Corrigido o número da porta SSH Master0 para kubernetes

### <a name="appservice"></a>AppService

* Corrigida uma exceção ao criar um novo GIT com base no aplicativo Web Linux

### <a name="event-grid"></a>Grade de Eventos

* Adicionadas dependências SDK

## <a name="august-11-2017"></a>11 de agosto de 2017

Versão 2.0.13

### <a name="acs"></a>ACS

* Adicionadas mais regiões de visualização

### <a name="batch"></a>Batch

* Atualizado para o SDK 3.1.0 do Lote e SDK 4.1.0 do Gerenciamento de Lote
* Adicionado um novo comando que mostra as contagens de tarefa de um trabalho
* Corrigido o bug no processamento de URL de SAS do arquivo de recurso
* Ponto de extremidade de conta de lote agora dá suporte ao prefixo conta do Lote “https://” opcional
* Suporte para adicionar listas de mais de 100 tarefas a um trabalho
* Adicionado log de depuração para carregar o módulo do comando de Extensões

### <a name="component"></a>Componente

* Aviso de substituição adicionado aos comandos 'az component'

### <a name="container"></a>Contêiner

* `create`: corrigido o problema onde o sinal de igual não era permitido dentro de uma variável de ambiente


### <a name="data-lake-store"></a>Data Lake Store

* Habilitado o controle de progresso

### <a name="event-grid"></a>Grade de Eventos

* Versão inicial

### <a name="network"></a>Rede

* `lb`: corrigido o problema onde os nomes de recursos filhos específicos não eram resolvidos corretamente quando omitidos
* `application-gateway {subresource} delete`: corrigido o problema onde `--no-wait` não foi liquidado
* `application-gateway http-settings update`: Corrigido o problema onde `--connection-draining-timeout` não podia ser desativado
* Corrigido o erro de argumento de palavra-chave inesperado `sa_data_size_kilobyes` com `az network vpn-connection ipsec-policy add`

### <a name="profile"></a>Perfil

* `account list`: adicionado `--refresh` para sincronizar as assinaturas mais recentes do servidor

### <a name="storage"></a>Armazenamento

* Habilitar atualização de conta de armazenamento com a identidade atribuída do sistema

### <a name="vm"></a>VM

* `availability-set`: exposta a contagem de domínios de falha durante a conversão
* Exposto o comando `list-skus`
* Suporte para atribuir identidade sem criar atribuições de função
* Aplicar o SKU de armazenamento ao anexar discos de dados
* Removido o nome do disco do sistema operacional padrão e SKU de armazenamento ao usar discos gerenciados


## <a name="july-28-2017"></a>28 de julho de 2017

Versão 2.0.12

* Adicionado os comandos de contêiner
* Adicionados módulos de cobrança e de consumo

```
azure-cli (2.0.12)  

acr (2.0.9)  
acs (2.0.11)  
appservice (0.1.11)  
batch (3.0.3)  
billing (0.1.3)  
cdn (0.0.6)  
cloud (2.0.7)  
cognitiveservices (0.1.6)  
command-modules-nspkg (2.0.1)  
component (2.0.6)  
configure (2.0.10)  
consumption (0.1.3)  
container (0.1.7)  
core (2.0.12)  
cosmosdb (0.1.11)  
dla (0.0.10)  
dls (0.0.11)  
feedback (2.0.6)  
find (0.2.6)  
interactive (0.3.7)  
iot (0.1.10)  
keyvault (2.0.8)  
lab (0.0.9)  
monitor (0.0.8)  
network (2.0.11)  
nspkg (3.0.1)  
profile (2.0.9)  
rdbms (0.0.5)  
redis (0.2.7)  
resource (2.0.11)  
role (2.0.9)  
sf (1.0.5)  
sql (2.0.8)  
storage (2.0.11)  
vm (2.0.11) 
```

### <a name="core"></a>Núcleo

* Informações de autenticação de SDK de saída para entidades de serviço com certificados
* Corrigidas as exceções de andamento da implantação
* Usar o ponto de extremidade do ARM da nuvem atual para criar cliente da assinatura
* Melhor manipulação simultânea do arquivo clouds.config (#3636)
* Atualização da ID de solicitação do cliente para cada execução de comando
* Criar clientes de assinatura com o perfil correto do SDK (#3635)
* Relatório de andamento para implantações de modelo (#3510)
* Adicionado suporte para escolher campos de saída da tabela através da consulta JMESpath (#3581)
* Aprimorado a desativação de áudio de argumentos de análise e acrescentar histórico com gestos (#3434)
* Criar clientes de assinatura com o perfil correto do SDK
* Mover todos os arquivos existentes de gravação para a pasta mais recente
* Corrigida a idempotência fixa para criação de VM/VMSS (#3586)
* Os caminhos de comando não diferenciam mais maiúsculas de minúsculas
* Determinados parâmetros do tipo booliano não diferenciam mais maiúsculas de minúsculas
* Suporte para logon do ADFS em um servidor local como o Azure Stack
* Corrigidas as gravações simultâneas para clouds.config (#3255)

### <a name="acr"></a>ACR

* Adicionado o comando `show-usage` para registros gerenciados
* Suporte para atualização do SKU para registros gerenciados
* Adicionados registros gerenciados com o SKU gerenciado
* Adicionados webhooks para registros gerenciados com o módulo de comando de webhook do ACR
* Adicionada autenticação do AAD adicionada com o comando de logon de ACR
* Adicionado comando de exclusão para marcas, manifestos e repositórios do Docker

### <a name="acs"></a>ACS

* Suporte para a API versão 2017-07-01

### <a name="appservice"></a>AppService

* Corrigido o bug onde listar o aplicativo Web Linux não retornava nada
* Suporte para recuperar credenciais de ACR
* Remover todos os comandos em `appservice web`
* Máscara de senhas de registro do Docker da saída do comando (#3656)
* Verifique se o navegador padrão é usado no macOS sem erros (#3623)
* Aprimorada a Ajuda de `webapp log tail` e `webapp log download` (#3624)
* Exposto o comando `traffic-routing` para configurar roteamento estático (#3566)
* Adicionadas correções de confiabilidade na configuração de controle do código-fonte (#3245)
* Removido o argumento `--node-version` sem suporte de `webapp config update` para aplicativos Web do Windows. Em vez disso, use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`

### <a name="batch"></a>Batch

* Atualizado para o SDK 3.0.0 do Lote com suporte para VMs de baixa prioridade em pools
* Opção `pool create` renomeada como `--target-dedicated` para `--target-dedicated-nodes`
* Adicionadas as opções `pool create` e `--target-low-priority-nodes` de `--application-licenses`

### <a name="cdn"></a>CDN

* Fornecida uma mensagem de erro mais adequada para `cdn endpoint list` quando o perfil especificado por `--profile-name` não existe.

### <a name="cloud"></a>Nuvem

* Alterada a versão de API do ponto de extremidade de metadados de nuvem para o formato AAAA-MM-DD
* Ponto de extremidade da galeria não é necessário
* Suporte para registrar a nuvem somente com o ponto de extremidade de gerenciador de recursos do ARM
* Fornecida uma opção para `cloud set` para escolher o perfil ao selecionar a nuvem atual
* Exposto `endpoint_vm_image_alias_doc`

### <a name="cosmosdb"></a>CosmosDB

* Corrigida a permissão para criação de coleção com chave de partição personalizada
* Adicionado suporte para o TTL padrão de coleção.

### <a name="data-lake-analytics"></a>Data Lake Analytics

* Adicionados comandos para gerenciamento de política de computação sob o título `dla account compute-policy`
* Adicionado `dla job pipeline show`
* Adicionado `dla job recurrence list`

### <a name="data-lake-store"></a>Data Lake Store

* Adicionado suporte para a rotação de chave de cofre de chaves gerenciado do usuário em `dls account update`
* Atualizada a versão SDK do sistema de arquivos do Data Lake Store subjacente para resolver um problema de desempenho
* Adicionado o comando `dls enable-key-vault`. Esse comando tenta permitir que um Cofre de Chaves fornecido pelo usuário use a criptografia de dados em uma conta do Data Lake Store

### <a name="interactive"></a>Interativo

* Melhor tempo de inicialização, usando comandos em cache
* Maior cobertura de teste
* Aprimorado o gesto “?” para injetar também o próximo comando
* Corrigidos os erros interativos com o perfil 2017-03-09-profile-preview (#3587)
* Permitido `--version` como um parâmetro para o modo interativo (#3645)
* Impedir que o modo interativo gere erros de conclusões de validação (#3570)
* Relatório de andamento para implantações de modelo (#3510)
* Adicionado o sinalizador `--progress`
* Removidos `--debug` e `--verbose` de conclusões
* Removido `interactive` de conclusões (#3324)

### <a name="iot"></a>IoT

* A criação de uma política não limpa as políticas existentes. (#3934)

### <a name="key-vault"></a>Cofre de chaves

* Comandos adicionados para recursos de recuperação do cofre de chaves:
  * Subcomandos `purge`, `recover`, `keyvault list-deleted` de `keyvault`
  * Subcomandos `backup`, `restore`, `purge`, `recover`, `list-deleted` de `keyvault secret`
  * Subcomandos `purge`, `recover`, `list-deleted` de `keyvault certificate`
  * Subcomandos `purge`, `recover`, `list-deleted` de `keyvault key`
* Adicionada a integração do cofre de chaves da entidade de serviço (#3133)
* Atualizado o plano de dados de cofre de chaves para 0.3.2. (#3307)

### <a name="lab"></a>Laboratório

* Adicionado o suporte para reivindicar qualquer VM no laboratório através de `az lab vm claim`
* Adicionada o formatador de tabela `az lab vm list` e `az lab vm show`

### <a name="monitor"></a>Monitoramento

* Correção para o arquivo de modelo com o comando `monitor autoscale-settings get-parameters-template` (#3349)
* `monitor alert-rule-incidents list` renomeado para `monitor alert list-incidents`
* `monitor alert-rule-incidents show` renomeado para `monitor alert show-incident`
* `monitor metric-defintions list` renomeado para `monitor metrics list-definitions`
* `monitor alert-rules` renomeado para `monitor alert`
* Alterado `monitor alert create`:
  * Os subcomandos `condition` e `action` não aceitarão mais JSON
  * Adicionar vários parâmetros para simplificar o processo de criação de regra
  * `location` não é mais necessário
  * Adicionar nome e o suporte a ID de destino
  * Remover `--alert-rule-resource-name`
  * Renomear `is-enabled` para `enabled` não é mais necessário
  * Padrões de `description` agora baseados na condição fornecida
  *  Adicionar exemplos para ajudar a esclarecer o novo formato
* Suporte para nomes ou IDs para comandos `monitor metric`
* Argumentos de conveniência adicional e exemplos para `monitor alert rule update`

### <a name="network"></a>Rede

* Adicionado o comando `list-private-access-services`
* Adicionado argumento `--private-access-services` para `vnet subnet create` e `vnet subnet update`
* Corrigido o problema onde `application-gateway redirect-config create` falhava
* Corrigido o problema onde `application-gateway redirect-config update` com `--no-wait` não funcionava
* Corrigido o bug ao usar o argumento `--servers` com `application-gateway address-pool create` e `application-gateway address-pool update`
* Adicionados os comandos `application-gateway redirect-config`
* Adicionados os comandos para `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`
* Adicionados os argumentos para `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`
* Adicionados os argumentos para `application-gateway http-settings create` e `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`
* Adicionados os argumentos para `application-gateway url-path-map create` e `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`
* Adicionado o argumento `--redirect-config` para `application-gateway url-path-map rule create`
* Adicionado o suporte ao `--no-wait` para `application-gateway url-path-map rule delete`
* Adicionados os argumentos para `application-gateway probe create` e `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`
* Adicionado o argumento `--redirect-config` para `application-gateway rule create` e `application-gateway rule update`
* Adicionado o suporte ao `--accelerated-networking` para `nic create` e `nic update`
* Removido o argumento `--internal-dns-name-suffix` de `nic create`
* Adicionado suporte ao `--dns-servers` para `nic update` e `nic create`: Adicionar suporte para servidores DNS
* Corrigido o bug onde `local-gateway create` ignorava `--local-address-prefixes`
* Adicionado o suporte ao `--dns-servers` para `vnet update`
* Corrigido o bug ao criar um emparelhamento sem filtragem de rotas com `express-route peering create`
* Corrigido o bug onde os argumentos `--provider` e `--bandwidth` não funcionavam com `express-route update`
* Corrigido o bug com a lógica padrão de `network watcher show-topology`
* Aprimorada a formatação de saída para `network list-usages`
* Usar IP de front-end padrão para `application-gateway http-listener create` se existir apenas um
* Usar o pool padrão de pool de endereços, configurações de HTTP e o ouvinte HTTP para `application-gateway rule create` se existir apenas um
* Usar IP de front-end e pool de back-end padrão para `lb rule create` se existir apenas um
* Usar IP de front-end padrão para `lb inbound-nat-rule create` se existir apenas um

### <a name="profile"></a>Perfil

* Suporte a logon em uma VM com uma identidade gerenciada
* Suporte a saída para `account show` em formato de arquivo de autenticação do SDK
* Mostrar avisos de código obsoleto ao usar o “modo de exibição expandido”
* Adicionado o comando `get-access-token` para fornecer o token bruto do AAD
* Suporte a logon com uma conta de usuário sem nenhuma assinatura associada

### <a name="rdbms"></a>RDBMS

* Suporte para listar servidores em uma assinatura (#3417)
* Corrigido o `%s` não processado devido à ausência de `% server_type` (#3393)
* Corrigido o mapa do código-fonte do documento e adicionada a tarefa CI para verificação (#3361)
* Corrigida a ajuda de MySQL e PostgreSQL (#3369)

### <a name="resource"></a>Recurso

* Aprimorados os prompts para parâmetros ausentes para `group deployment create`
* Aprimorada a análise da sintaxe `--parameters KEY=VALUE`
* Corrigidos os problemas onde os arquivos de parâmetros `group deployment create` não eram mais reconhecidos usando a sintaxe `@<file>`
* Suporte do argumento `--ids` para os comandos `resource` e `managedapp`
* Corrigidas algumas mensagens de erro e análise (#3584)
* Corrigida a análise de `--resource-type` para o comando `lock` aceitar `<resource-namespace>` e `<resource-type>`
* Adicionados parâmetros de verificação para modelos de link do modelo (#3629)
* Adicionado suporte para especificar parâmetros de implantação usando a sintaxe `KEY=VALUE`

### <a name="role"></a>Função

* Suporte à saída para no formato de arquivo de autenticação do SDK para `create-for-rbac`
* Limpar as atribuições de função e aplicativos relacionados ao AAD ao excluir uma entidade de serviço (#3610)
* Incluir o formato de hora nos argumentos `app create` e descrições `--start-date` e `--end-date`
* Mostrar avisos de código obsoleto ao usar `--expanded-view`
* Adicionada a integração do cofre da chaves para os comandos `create-for-rbac` e `reset-credentials`

### <a name="service-fabric"></a>Service Fabric
* Corrigido um problema com arquivos grandes em aplicativos que eram truncados ao serem carregados (#3666)
* Adicionados testes para os comandos do Service Fabric (#3424)
* Corrigidos vários comandos do Service Fabric (#3234)

### <a name="sql"></a>SQL

* Removido o parâmetro `sql server create` `--identity`
* Remover os valores de senha da saída dos comandos `sql server create` e `sql server update`
* Adicionados os comandos para `sql db list-editions` e `sql elastic-pool list-editions`

### <a name="storage"></a>Armazenamento

* Removida a opção `--marker` dos comandos `storage blob list`, `storage container list`, e `storage share list` (#3745)
* Habilitado a criação de uma conta de armazenamento somente para https
* Atualizadas as métricas de armazenamento, registro em log e os comandos do CORS (#3495)
* Mensagem de exceção reformulada do ADD do CORS adicionar (#3638) (#3362)  
* Convertido o gerador para uma lista no modo de simulação de comando do lote de download (#3592) 
* Corrigido o problema de simulação do lote de download de blob (#3640) (#3592)

### <a name="vm"></a>VM

* Suporte para configuração de NSG
* Corrigido o bug onde o servidor DNS não era configurado corretamente
* Suporte às identidades de serviço gerenciado
* Corrigido o problema onde `cmss create` com um balanceador de carga existente exigia `--backend-pool-name`.
* Os discos de dados criados com LUN do `vm image create` agora começam com 0


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

* [ACS] Adicionar suporte para configurar um cluster do ACS padrão ([#2554](https://github.com/Azure/azure-cli/pull/2554))
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
Você pode fazer perguntas sobre [StackOverflow usando a marcação azure-cli](http://stackoverflow.com/questions/tagged/azure-cli) ou entrar em contato com a equipe do produto pelo endereço [ azfeedback@microsoft.com ](mailto:azfeedback@microsoft.com). Você pode fornecer comentários a partir da linha de comando com o comando `az feedback`.

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

