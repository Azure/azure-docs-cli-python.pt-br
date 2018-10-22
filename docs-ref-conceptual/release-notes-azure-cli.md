---
title: Notas de versão da CLI do Azure
description: Saiba mais sobre as últimas atualizações da CLI do Azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 10/09/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 0aec9dce0eda007c71df3693b39c7ec8cc9856cd
ms.sourcegitcommit: 0fc354c24454f5c9c5ff4b7296ad7b18ffdf31b1
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/10/2018
ms.locfileid: "48904779"
---
# <a name="azure-cli-release-notes"></a>Notas de versão da CLI do Azure

## <a name="october-9-2018"></a>9 de outubro de 2018

Versão 2.0.47

### <a name="core"></a>Núcleo
* Melhoria do tratamento de erro para os erros de "Solicitação Incorreta"

### <a name="acr"></a>ACR
* Suporte adicionado para o formato de tabela semelhante como cliente do helm

### <a name="acs"></a>ACS
* `aks [create|scale] --nodepool-name` adicionado para configurar o nome nodepool, truncado com 12 caracteres, padrão – nodepool1 
* Corrigido para voltar para “scp” quando Parimiko falha
* `aks create` alterado para não precisar mais de `--aad-tenant-id`
* Melhoria da mesclagem das credenciais do Kubernetes quando houver entradas duplicadas

### <a name="container"></a>Contêiner
* `functionapp create` alterado para dar suporte à criação de um tipo de plano de consumo do Linux com um tempo de execução específico
* [VERSÃO PRÉVIA] Suporte adicionado para hospedar aplicativos Web nos contêineres do Windows

### <a name="event-hub"></a>Hub de evento
* Corrigido o comando `eventhub update`
* [ALTERAÇÃO SIGNIFICATIVA] `list` comandos alterados para lidar com os erros de recurso(s) NotFound(404) do modo típico, em vez de mostrar uma lista vazia

### <a name="extensions"></a>Extensões
* Corrigido o problema ao tentar adicionar uma extensão já instalada

### <a name="hdinsight"></a>HDInsight
* Versão inicial

### <a name="iot"></a>IoT
* Comando de instalação da extensão adicionado à faixa inicial

### <a name="keyvault"></a>KeyVault
* Alterado para restringir os comandos de armazenamento do keyvault ao perfil da API mais recente

### <a name="network"></a>Rede
* `network dns zone create` corrigido: o comando terá êxito mesmo se o usuário tiver configurado um local padrão. Veja o n° 6052
* Preterido `--remote-vnet-id` para `network vnet peering create`
* `--remote-vnet` a `network vnet peering create` adicionados, que aceita um nome ou uma ID
* Suporte adicionado para vários prefixos de sub-rede a `network vnet create` com `--subnet-prefixes`
* Suporte adicionado para vários prefixos de sub-rede a `network vnet subnet [create|update]` com `--address-prefixes`
* Corrigido o problema com `network application-gateway create` que impedia a criação de gateways com a SKU `WAF_v2` ou `Standard_v2`
* Argumento de conveniência `--service-endpoint-policy` adicionado a `network vnet subnet update`

### <a name="role"></a>Função
* Suporte adicionado para listar os proprietários de aplicativo do Azure AD para `ad app owner`
* Suporte adicionado para listar os proprietários da entidade de serviço do Azure AD para `ad sp owner`
* Alterado para garantir que os comandos para criar e atualizar a definição da função aceitem várias configurações de permissão
* `ad sp create-for-rbac` alterado para garantir que a URI da home page sempre seja "https"

### <a name="service-bus"></a>Barramento de Serviço
* [ALTERAÇÃO SIGNIFICATIVA] `list` comandos alterados para lidar com os erros de recurso(s) NotFound(404) do modo típico, em vez de mostrar uma lista vazia

### <a name="vm"></a>VM
* Corrigido o campo `accessSas` vazio em `disk grant-access`
* `vmss create` alterado para reservar um intervalo de portas de front-end grande o suficiente para lidar com excesso de provisionamento
* Corrigidos os comandos de atualização para `sig`
* Suporte `--no-wait` adicionado para gerenciar as versões da imagem em `sig`
* `vm list-ip-addresses` alterado para mostrar a zona de disponibilidade dos endereços IP públicos
* `[vm|vmss] disk attach` alterado para definir o LUN padrão do disco para o primeiro ponto disponível

## <a name="september-21-2018"></a>21 de setembro de 2018

Versão 2.0.46

### <a name="acr"></a>ACR
* Adicionados comandos de tarefa de ACR
* Adicionado o comando de execução rápido
* Grupo de comandos `build-task` preteridos
* Adicionado o grupo de comando `helm` para dar suporte ao gerenciamento de gráficos Helm com o ACR
* Suporte adicionado para criação idempotente para registro gerenciado
* Adicionado um sinalizador de formato no para exibir logs de build

### <a name="acs"></a>ACS
* Alterado o comando `install-connector` para definir o FQDN mestre do AKS
* Corrigida a criação de atribuição de função para vnet-subnet-id ao não especificar a entidade de serviço e skip-role-assignment

### <a name="appservice"></a>AppService

* Adicionado suporte para o gerenciamento de operações de WebJobs (contínuos e disparados)
* Suporte de az webapp config set para a propriedade --fts-state property. Adicionado suporte também para az functionapp config set & show
* Adicionado suporte para trazer seu próprio armazenamento para aplicativos Web
* Adicionado suporte para a listar e restaurar aplicativos Web excluídos

### <a name="batch"></a>Lote
* Alterada a inclusão de tarefas por meio de `--json-file` para dar suporte à sintaxe AddTaskCollectionParameter
* Atualizada a documentação de formatos `--json-file` aceitos
* `--max-tasks-per-node-option` foi adicionado a `batch pool create`
* Alterado o comportamento de `batch account` para mostrar as contas atualmente conectadas se nenhuma opção foi especificada

### <a name="batch-ai"></a>Lote AI 
* Corrigida a falha na criação de conta de armazenamento automática no comando `batchai cluster create`

### <a name="cognitive-services"></a>Serviços Cognitivos
* Adicionado o complemento para os argumentos `--sku`, `--kind`, `--location`
* Adicionado o comando `cognitiveservices account list-usage`
* Adicionado o comando `cognitiveservices account list-kinds`
* Adicionado o comando `cognitiveservices account list`
* Preterido `cognitiveservices list`
* Alterado `--name` para que seja opcional para `cognitiveservices account list-skus`

### <a name="container"></a>Contêiner
* Adicionada a capacidade de reiniciar e parar um grupo de contêineres em execução
* Adicionado `--network-profile` para passar em um perfil de rede
* Adicionado `--subnet`, `--vnet_name`, para permitir a criação de grupos de contêineres em uma rede virtual
* Alterada a saída da tabela para mostrar o status do grupo de contêineres

### <a name="datalake"></a>DataLake
* Comandos adicionados para regras de rede virtual

### <a name="interactive-shell"></a>Shell interativo
* Corrigido o erro no Windows em que comandos não são executados corretamente
* Corrigido o problema para carregar o comando no modo interativo que era causado por objetos preteridos

### <a name="iot"></a>IoT
* Adicionado suporte para roteamento de Hubs de IoT

### <a name="key-vault"></a>Key Vault
* Corrigida a importação de chave do Key Vault para chaves RSA

### <a name="network"></a>Rede
* Adicionados os comandos `network public-ip prefix` para dar suporte a recursos de prefixos de IP público
* Adicionados os comandos `network service-endpoint` para dar suporte a recursos de política de ponto de extremidade de serviço
* Adicionados os comandos `network lb outbound-rule` para dar suporte à criação de regras de saída do Standard Load Balancer
* Adicionado `--public-ip-prefix` a `network lb frontend-ip create/update` para dar suporte a configurações de IP de front-end usando prefixos de IP público
* Adicionado `--enable-tcp-reset` a `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`
* Adicionado `--disable-outbound-snat` a `network lb rule create/update`
* Permitido o uso de `network watcher flow-log show/configure` com NSGs clássicos
* Adição do comando `network watcher run-configuration-diagnostic`
* Corrigido o comando `network watcher test-connectivity` e adicionadas as propriedades `--method`, `--valid-status-codes` e `--headers`
* `network express-route create/update`: Adicionado o sinalizador `--allow-global-reach`
* `network vnet subnet create/update`: Adicionado suporte para `--delegation`
* Adicionado o comando `network vnet subnet list-available-delegations`
* `network traffic-manager profile create/update`: Adicionado suporte para `--interval`, `--timeout` e `--max-failures` para as opções preteridas de configuração do monitor `--monitor-path`, `--monitor-port` e `--monitor-protocol`, que foram substituídas por `--path`, `--port` e `--protocol`
* `network lb frontend-ip create/update`: Corrigida a lógica para configurar o método de alocação de IP privado. Se um endereço IP privado for fornecido, a alocação será estática. Se nenhum endereço IP privado for fornecido ou uma cadeia de caracteres vazia for fornecida para o endereço IP privado, a alocação será dinâmica.
* `dns record-set * create/update`: Adicionado suporte para `--target-resource`
* Adicionados comandos `network interface-endpoint` para consultar objetos do ponto de extremidade da interface
* Adicionado `network profile show/list/delete` para gerenciamento parcial dos perfis de rede
* Adicionados comandos `network express-route peering connection` para gerenciar conexões de emparelhamento entre as ExpressRoutes

### <a name="rdbms"></a>RDBMS
* Adicionado suporte para o serviço MariaDB

### <a name="reservation"></a>Reserva
* Adicionado CosmosDB no tipo enumerado de recurso reservado
* Adicionada a propriedade nome no modelo do Patch

### <a name="manage-app"></a>Gerenciar aplicativo
* Corrigido o bug em `managedapp create --kind MarketPlace` que resultava em falha durante a criação da instância de um aplicativo gerenciado do Marketplace
* Alterados os comandos `feature` para serem restritos somente aos perfis com suporte

### <a name="role"></a>Função
* Adicionado suporte para listar membros de grupo de usuários

### <a name="signalr"></a>SignalR
* Primeira versão

### <a name="storage"></a>Armazenamento
* Adicionado o parâmetro `--auth-mode login` para usar as credenciais de login do usuário para autorização de filas e blobs
* Adicionado `storage container immutability-policy/legal-hold` para gerenciar o armazenamento imutável

### <a name="vm"></a>VM
* Corrigido o problema em que `vm create --generate-ssh-keys` sobrescreve o arquivo de chave privada se o arquivo de chave pública estiver ausente (#4725, #6780)
* Adicionado suporte para galeria de imagem compartilhada através de `az sig`

## <a name="august-28-2018"></a>28 de Agosto de 2018

Versão 2.0.45

### <a name="core"></a>Núcleo

* Corrigido o problema de carregamento de arquivo de configuração vazio
* Adicionado suporte para o perfil `2018-03-01-hybrid` para o Azure Stack

### <a name="acr"></a>ACR

* Adicionada uma solução alternativa para operações de tempo de execução sem solicitações ARM
* Alterado para excluir arquivos de controle de versão (por exemplo, .git, .gitignore) de tar carregados por padrão no comando `build`

### <a name="acs"></a>ACS

* Alterado `aks create` para os padrões para VMs `Standard_DS2_v2`
* Alterado `aks get-credentials` para agora chamar novas APIs para obter credenciais de cluster

### <a name="appservice"></a>AppService

* Adicionado suporte para CORS no functionapp e webapp
* Adicionado suporte a marcas ARM ao criar comandos
* Alterado `[webapp|functionapp] identity show` para sair com o código 3 mediante um recurso ausente

### <a name="backup"></a>Backup

* Alterado `backup vault backup-properties show` para sair com o código 3 mediante um recurso ausente

### <a name="bot-service"></a>Serviço de Bot

* Versão da CLI do serviço de Bot inicial

### <a name="cognitive-services"></a>Serviços Cognitivos

* Adicionado novo parâmetro `--api-properties,` que é necessário para a criação de alguns dos serviços

### <a name="iot"></a>IoT

* Corrigido o problema com a associação de hubs vinculados

### <a name="monitor"></a>Monitoramento

* Adicionados comandos `monitor metrics alert` para alertas de métrica quase em tempo real
* Comandos `monitor alert` preteridos

### <a name="network"></a>Rede

* Alterado `network application-gateway ssl-policy predefined show` para sair com o código 3 mediante um recurso ausente

### <a name="resource"></a>Recurso

* Alterado `provider operation show` para sair com o código 3 mediante um recurso ausente

### <a name="storage"></a>Armazenamento

* Alterado `storage share policy show` para sair com o código 3 mediante um recurso ausente

### <a name="vm"></a>VM

* Alterado `vm/vmss identity show` para sair com o código 3 mediante um recurso ausente 
* Preterido `--storage-caching` para `vm create`

## <a name="auguest-14-2018"></a>14 de agosto de 2018

Versão 2.0.44

### <a name="core"></a>Núcleo

* Corrigida a exibição numérica na saída `table`
* Adicionado o formato de saída YAML

### <a name="telemetry"></a>Telemetria

* Melhorias nos relatórios de telemetria

### <a name="acr"></a>ACR

* Adicionados os comandos `content-trust policy`
* Corrigido o problema onde `.dockerignore` não foi tratado adequadamente

### <a name="acs"></a>ACS

* Alterado `az acs/aks install-cli` para instalar em `%USERPROFILE%\.azure-kubectl` no Windows
* Alterado `az aks install-connector` para detectar se o cluster tem RBAC e configurar o conector ACI adequadamente
* Alterado para atribuição de função à sub-rede quando ela é fornecida
* Adicionada uma nova opção para “ignorar a atribuição de função” à sub-rede quando ela é fornecida                                 
* Alterado para ignorar a atribuição de função à sub-rede quando a atribuição já existe                

### <a name="appservice"></a>AppService

* Corrigido um bug que impede a criação de um aplicativo de funções usando contas de armazenamento em grupos de recursos externos
* Corrigida uma falha na implantação de zip

### <a name="batchai"></a>BatchAI

* Alterada a saída do agente para criação de conta de armazenamento automática para especificar “*grupo* de recurso”.        

### <a name="container"></a>Contêiner

* Adicionado `--secure-environment-variables` para passar as variáveis de ambiente seguras para um contêiner      

### <a name="iot"></a>IoT

* [ALTERAÇÃO SIGNIFICATIVA] Removidos os comandos preteridos que foram movidos para a extensão iot
* Atualizados os elementos para não presumirem o domínio `azure-devices.net`

### <a name="iot-central"></a>Central de IoT

* Versão inicial do módulo do IoT Central

### <a name="keyvault"></a>KeyVault


* Comandos adicionados para gerenciar contas de armazenamento e as definições de sas
* Comandos adicionados para regras de rede                                                           
* Adicionado o parâmetro `--id` para operações de certificado, chave e segredo
* Adicionado suporte para a versão de várias APIs de gerenciamento KV
* Adicionado suporte para a versão de várias APIs do plano de dados KV

### <a name="relay"></a>Retransmissão

* Versão inicial

### <a name="sql"></a>Sql

* Adicionados os comandos `sql failover-group`

### <a name="storage"></a>Armazenamento

* [ALTERAÇÃO SIGNIFICATIVA] Alterado `storage account show-usage` para exigir o parâmetro `--location` e listará por região
* Alterado o parâmetro `--resource-group` para ser opcional para comandos `storage account`
* Removidos os avisos de “Falha na pré-condição” para as falhas individuais em comandos em lote para uma única mensagem agregada
* Alterados os comandos `[blob|file] delete-batch` para não exibir mais matriz de nulos
* Alterados os comandos `blob [download|upload|delete-batch]` para ler o token de sas da url do contêiner

### <a name="vm"></a>VM

* Adicionado filtros comuns à `vm list-skus` para facilidade de uso

## <a name="july-31-2018"></a>31 de julho de 2018

Versão 2.0.43

### <a name="acr"></a>ACR

* Sinalizador `--with-secure-properties` adicionado ao comando `acr build-task show`
* Adicionado o comando `acr build-task update-build`

### <a name="acs"></a>ACS

* Alterado para retornar 0 (êxito) ao terminar `az aks browse` pressionando [Ctrl+C]

### <a name="batch"></a>Lote

* Bug corrigido ao mostrar o token AAD no cloudshell

### <a name="container"></a>Contêiner

* Requisito removido de `--log-analytics-workspace-key` para o nome ou a ID ao definir assinatura

### <a name="network"></a>Rede

* Suporte a DNS adicionado a 2017-03-09-profile para o Azure Stack 

### <a name="resource"></a>Recurso

* `--rollback-on-error` a `group deployment create` adicionado para executar uma implantação válida no erro
* Problema corrigido onde `--parameters {}` com `group deployment create` resultou em um erro

### <a name="role"></a>Função

* Suporte adicionado para o perfil da pilha 2017-03-09-profile
* Problema corrigido onde os parâmetros de atualização genéricos para `app update` não funcionariam corretamente

### <a name="search"></a>Search

* Comandos adicionados para o serviço Azure Search

### <a name="service-bus"></a>Barramento de Serviço

* Grupo de comandos de migração adicionados para migrar um namespace do Barramento de Serviço Standard para Premium
* Novas propriedades opcionais adicionadas à fila do Barramento de Serviço e à Assinatura
  *  `--enable-batched-operations` e `--enable-dead-lettering-on-message-expiration` em `queue`
  *  `--dead-letter-on-filter-exceptions` em `subscriptions`

### <a name="storage"></a>Armazenamento

* Suporte adicionado para o download de arquivos grandes usando uma única conexão
* Comandos `show` convertidos que foram perdidos na falha com código de saída 3 mediante um recurso ausente

### <a name="vm"></a>VM

* Suporte adicionado para listar conjuntos de disponibilidade por assinatura
* Adicionado o suporte para `StandardSSD_LRS`
* Suporte adicionado para o grupo de segurança do aplicativo ao criar um conjunto de dimensionamento da VM
* [ALTERAÇÃO SIGNIFICATIVA] `[vm|vmss] create`, `[vm|vmss] identity assign` e `[vm|vmss] identity remove` alterados para produzir identidades de usuário atribuídas no formato de dicionário

## <a name="july-18-2018"></a>18 de julho de 2018

Versão 2.0.42

### <a name="core"></a>Núcleo

* Adicionado suporte para logon baseado em navegador, na janela de bash WSL
* O sinalizador `--force-string` foi adicionado a todos os comandos de atualização genérica
* [ALTERAÇÃO SIGNIFICATIVA] Os comandos 'show' foram alterados para registrar mensagens de erro e falha com código de saída 3 quando um recurso está ausente

### <a name="acr"></a>ACR

* [ALTERAÇÃO SIGNIFICATIVA] '--no-push' foi atualizado para um sinalizador puro no comando 'acr build'
* Foram adicionados os comandos `show` e `update` no grupo `acr repository`
* Foi adicionado o sinalizador `--detail` a `show-manifests` e `show-tags` para mostrar informações mais detalhadas
* Foi adicionado o parâmetro `--image` para dar suporte aos detalhes do build get ou aos logs por meio de uma imagem

### <a name="acs"></a>ACS

* `az aks create` foi alterado para excluir o erro se `--max-pods` for menor que 5

### <a name="appservice"></a>AppService

* Suporte adicionado para skus PremiumV2

### <a name="batch"></a>Lote

* Corrigido o bug sobre como usar a credencial de token no modo do Cloud Shell
* Alterada a entrada JSON para diferenciar maiúsculas de minúsculas

### <a name="batch-ai"></a>Lote AI

* Corrigido o comando `az batchai job exec`

### <a name="container"></a>Contêiner

* Removido o requisito de nome de usuário e senha para os registros não dockerhub
* Correção de erro durante a criação de grupos de contêineres de arquivo yaml

### <a name="network"></a>Rede

* Adicionado o suporte `--no-wait` para `network nic [create|update|delete]` 
* Adicionado `network nic wait`
* Preterido o argumento `--ids` para `network vnet [subnet|peering] list`
* Adicionado o sinalizador `--include-default` para incluir regras de segurança padrão na saída do `network nsg rule list`  

### <a name="resource"></a>Recurso

* Adicionado o suporte `--no-wait` para `group deployment delete`
* Adicionado o suporte `--no-wait` para `deployment delete`
* Adicionado o comando `deployment wait`
* Correção do problema em que os comandos de nível de assinatura `az deployment` erroneamente apareceram no perfil 2017-03-09-profile

### <a name="sql"></a>SQL

* O erro “O nome de grupo de recursos fornecido ... não correspondeu ao nome na Url” foi fixado ao especificar o nome do pool elástico para os comandos `sql db copy` e `sql db replica create`
* Permitir a configuração do padrão do SQL Server, executando `az configure --defaults sql-server=<name>`
* Os formatadores de tabela foram implementados aos comandos `sql server`, `sql server firewall-rule`, `sql list-usages` e `sql show-usage`

### <a name="storage"></a>Armazenamento

* Adicionada a propriedade `pageRanges` à saída `storage blob show` que será preenchida para blobs de página

### <a name="vm"></a>VM

* [ALTERAÇÃO SIGNIFICATIVA] Alterado `vmss create` para usar o `Standard_DS1_v2` como o tamanho de instância padrão
* Adicionado o suporte `--no-wait` para `vm extension [set|delete]` e `vmss extension [set|delete]`
* Adicionado `vm extension wait`

## <a name="july-3-2018"></a>3 de julho de 2018

Versão 2.0.41

### <a name="aks"></a>AKS

* Monitoramento alterado para usar a ID de assinatura

## <a name="july-3-2018"></a>3 de julho de 2018

Versão 2.0.40

### <a name="core"></a>Núcleo

* Adicionado um novo fluxo de código de autorização para o logon interativo

### <a name="acr"></a>ACR

* Status da compilação de sondagem adicionado
* Suporte adicionado para valores de enumeração que não diferenciam maiúsculas de minúsculas
* Parâmetros `--top` e `--orderby` adicionados para `show-manifests`

### <a name="acs"></a>ACS

* [ALTERAÇÃO SIGNIFICATIVA] Habilitar controle de acesso baseado em funções do Kubernetes por padrão
* Argumento `--disable-rbac` e preterido `--enable-rbac` adicionados, pois é o padrão agora
* Opções atualizadas do comando `aks browse`. Suporte `--listen-port` adicionado
* Atualizado o pacote de gráficos do helm padrão para o comando `aks install-connector`. Usar virtual-kubelet-para-aks-latest.tgz
* Comandos `aks enable-addons` e `aks disable-addons` adicionados para atualizar um cluster existente

### <a name="appservice"></a>AppService

* Suporte adicionado para desabilitar a identidade via `webapp identity remove`
* Marca `preview` removida para o recurso de Identidade

### <a name="backup"></a>Backup

* Definição do módulo atualizada

### <a name="batchai"></a>BatchAI

* Saída da tabela corrigida para comandos `batchai cluster node list` e `batchai job node list`

### <a name="cloud"></a>Nuvem

* Sufixo do servidor `acr login` adicionado à configuração de nuvem

### <a name="container"></a>Contêiner

* `container create` alterado para padrão para a operação de longa execução
* Parâmetros `--log-analytics-workspace` e `--log-analytics-workspace-key` adicionados do Log Analytics
* Parâmetro `--protocol` adicionado para especificar qual protocolo de rede usar

### <a name="extension"></a>Extensão

* `extension list-available` alterado para mostrar apenas as extensões compatíveis com a versão da CLI

### <a name="network"></a>Rede

* Corrigido o problema onde os tipos de registro diferenciam maiúsculas de minúsculas ([#6602](https://github.com/Azure/azure-cli/issues/6602))

### <a name="rdbms"></a>Rdbms

* Adicionados os comandos `[postgres|myql] server vnet-rule`

### <a name="resource"></a>Recurso

* Novo grupo de operação `deployment` adicionado

### <a name="vm"></a>VM

* Suporte adicionado para remover a identidade atribuída do sistema

## <a name="june-25-2018"></a>25 de junho de 2018

Versão 2.0.39

### <a name="cli"></a>CLI

* Corte de arquivo atualizado no instalador MSI para corrigir o problema de instalação da extensão

## <a name="june-19-2018"></a>19 de junho de 2018

Versão 2.0.38

### <a name="core"></a>Núcleo

* Suporte global adicionado para `--subscription` a maioria dos comandos

### <a name="acr"></a>ACR

* `azure-storage-blob` foi adicionado como dependência
* A configuração de CPU padrão foi alterada com `acr build-task create` para usar 2 núcleos

### <a name="acs"></a>ACS

* As opções do comando `aks use-dev-spaces` foram atualizadas. Suporte `--update` adicionado
* `aks get-credentials --admin` foi alterado para substituir o contexto do usuário em `$HOME/.kube/config`
* A propriedade `nodeResourceGroup` somente leitura foi exposta em clusters gerenciados
* O erro de comando `acs browse` foi corrigido
* Foram feitas `--connector-name` opcional para `aks install-connector`, `aks upgrade-connector` e `aks remove-connector`
* Novas regiões de Instância de Contêiner do Azure foram adicionadas para `aks install-connector`
* O local normalizado foi adicionado no nome de versão do comando e no nome do nó para `aks install-connector`

### <a name="appservice"></a>AppService

* Foi adicionado suporte para versões mais recentes do urllib
* Foi adicionado suporte para `functionapp create` para usar o plano de serviço de aplicativo de grupos de recursos externos

### <a name="batch"></a>Lote

* A dependência `azure-batch-extensions` foi removida

### <a name="batch-ai"></a>Lote AI

* Foi adicionado suporte aos workspaces. Os workspaces permitem agrupar clusters, servidores de arquivos e experimentos, removendo a limitação no número de recursos que podem ser criados
* Foi adicionado suporte para os experimentos. Os experimentos permitem agrupar trabalhos em coleções removendo a limitação no número de trabalhos criados
* Foi adicionado suporte para configurar `/dev/shm` para trabalhos em execução em um contêiner de docker
* Foram adicionados os comandos `batchai cluster node exec` e `batchai job node exec`. Esses comandos permitem executar qualquer comando diretamente nos nós e fornece a funcionalidade de encaminhamento de porta.
* Foi adicionado suporte a `--ids` para os comandos `batchai`
* [ALTERAÇÃO SIGNIFICATIVA] Todos os clusters e servidores de arquivos devem ser criados nos espaços de trabalho
* [ALTERAÇÃO SIGNIFICATIVA] Os trabalhos devem ser criados nas experiências
* [ALTERAÇÃO SIGNIFICATIVA] `--nfs-resource-group` foi removido dos comandos `cluster create` e `job create`. Para montar um NFS pertencente a outro workspace/grupo de recursos, forneça a ID de ARM do servidor de arquivos através da opção `--nfs`
* [ALTERAÇÃO SIGNIFICATIVA] `--cluster-resource-group` foi removido do comando `job create`. Para enviar um trabalho em um cluster pertencente a outro workspace/grupo de recursos, forneça a ID de ARM do cluster através da opção `--cluster`
* [ALTERAÇÃO SIGNIFICATIVA] O atributo `location` foi removido de trabalhos, cluster e servidores de arquivos. Agora, o local é um atributo de um workspace.
* [ALTERAÇÃO SIGNIFICATIVA] `--location` foi removido dos comandos `job create` e `cluster create` e `file-server create`
* [ALTERAÇÃO SIGNIFICATIVA] Os nomes das opções curtas foi alterado para tornar a interface mais consistente:
 - [`--config`, `-c`] foi renomeado para [`--config-file`, `-f`]
 - [`--cluster`, `-r`] foi renomeado para [`--cluster`, `-c`]
 - [`--cluster`, `-n`] foi renomeado para [`--cluster`, `-c`]
 - [`--job`, `-n`] foi renomeado para [`--job`, `-j`]

### <a name="maps"></a>Mapas

* [ALTERAÇÃO SIGNIFICATIVA] `maps account create` foi alterado para exigir a aceitação dos Termos de Serviço pelo prompt interativo ou sinalizador `--accept-tos`

### <a name="network"></a>Rede

* Foi adicionado suporte a `https` para `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)
* Foi corrigido o problema em que `--endpoint-status` diferenciava maiúsculas de minúsculas. [#6502](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a>Reservas

* [ALTERAÇÃO SIGNIFICATIVA] Foi adicionado o parâmetro `ReservedResourceType` necessário a `reservations catalog show`
* Parâmetro `Location` adicionado a `reservations catalog show`
* [ALTERAÇÃO SIGNIFICATIVA] `kind` foi removido de `ReservationProperties`
* [ALTERAÇÃO SIGNIFICATIVA] `capabilities` foi renomeado para `sku_properties` em `Catalog`
* [ALTERAÇÃO SIGNIFICATIVA] As propriedades `size` e `tier` foram removidas de `Catalog`
* Parâmetro `InstanceFlexibility` adicionado a `reservations reservation update`

### <a name="role"></a>Função

* Tratamento de erro melhorado

### <a name="sql"></a>SQL

* Foi corrigido um erro confuso ao executar `az sql db list-editions` para um local que não está disponível para sua assinatura

### <a name="storage"></a>Armazenamento

* A saída da tabela foi alterada para `storage blob download` para ser mais legível

### <a name="vm"></a>VM

* A verificação da refinação do tamanho da VM foi aprimorada para o suporte de rede acelerada em `vm create`
* Foi adicionado um aviso para `vmss create` informando que o tamanho padrão da VM será alternado de `Standard_D1_v2` para `Standard_DS1_v2`
* Foi adicionado `--force-update` a `[vm|vmss] extension set` para atualizar a extensão mesmo quando a configuração não foi alterada

## <a name="june-13-2018"></a>13 de junho de 2018

Versão 2.0.37

### <a name="core"></a>Núcleo

* A telemetria interativa foi melhorada

## <a name="june-13-2018"></a>13 de junho de 2018

Versão 2.0.36

### <a name="aks"></a>AKS

* Foram adicionadas opções avançadas de rede para `aks create`
* Foram adicionados argumentos para `aks create` para habilitar o monitoramento e roteamento de HTTP
* Adicionado o argumento `--no-ssh-key` para `aks create`
* Adicionado o argumento `--enable-rbac` para `aks create`
* [VERSÃO PRÉVIA] Suporte adicionado para a autenticação do Azure Active Directory no `aks create`

### <a name="appservice"></a>AppService

* Foi corrigido um problema com as versões urllib incompatíveis

## <a name="june-5-2018"></a>5 de junho de 2018

Versão 2.0.35

### <a name="interactive"></a>Interativo

* Foram adicionados limites para as dependências do modo interativo

## <a name="june-5-2018"></a>5 de junho de 2018

Versão 2.0.34

### <a name="core"></a>Núcleo

* Suporte adicionado para referência de recursos de locatário cruzado
* Melhor confiabilidade de carregamento de telemetria

### <a name="acr"></a>ACR

* Suporte adicionado para VSTS como um local de origem remota
* Adicionado o comando `acr import`

### <a name="aks"></a>AKS

* `aks get-credentials` foi alterado para criar o arquivo de configuração kube com permissões de sistema de arquivos mais seguras

### <a name="batch"></a>Lote

* Correção do bug na formatação de tabela da lista de Pool [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]

### <a name="iot"></a>IOT

* Suporte adicionado para a criação de Hubs IoT de Camada Básica

### <a name="network"></a>Rede

* `network vnet peering` melhorado

### <a name="policy-insights"></a>Informações sobre a Política

* Versão Inicial

### <a name="arm"></a>ARM

* Comandos `account management-group` adicionados.

### <a name="sql"></a>SQL

* Novos comandos de instância gerenciada adicionados:
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* Novos comandos de banco de dados gerenciado adicionados:
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a>Armazenamento

* Mimetypes extra adicionados para json e javascript para ser deduzido de extensões de arquivo

### <a name="vm"></a>VM

* `vm list-skus` foi alterado para usar colunas fixas e adicionar o aviso de que `Tier` e `Size` serão removidos
* Opção `--accelerated-networking` adicionada a `vm create`
* `--tags` foi adicionado a `identity create`

## <a name="may-22-2018"></a>22 de maio de 2018

Versão 2.0.33

### <a name="core"></a>Núcleo

* Suporte adicionado para expandir `@` em nomes de arquivos

### <a name="acs"></a>ACS

* Novos comandos de espaços de desenvolvimento `aks use-dev-spaces` e `aks remove-dev-spaces` foram adicionados
* Erro de digitação corrigido na mensagem de ajuda

### <a name="appservice"></a>AppService

* Comandos melhorados de atualização genérica
* Suporte assíncrono adicionado para `webapp deployment source config-zip`

### <a name="container"></a>Contêiner

* Suporte adicionado para a exportação de um grupo de contêiner no formato yaml
* Suporte adicionado para usar um arquivo yaml para criar/atualizar um grupo de contêiner

### <a name="extension"></a>Extensão

* Remoção de extensões melhorada

### <a name="interactive"></a>Interativo

* Log de alterações alterado para silenciar o analisador para conclusões
* Manipulação aprimorada de caches de ajuda inválida

### <a name="keyvault"></a>KeyVault

* Comandos de keyvault corrigidos para trabalhar no cloud shell ou VMs com identidade

### <a name="network"></a>Rede

* Corrija o problema em que `network watcher show-topology` não funcionará com o nome de rede virtual e/ou sub-rede [#6326](https://github.com/Azure/azure-cli/issues/6326)
* Corrija o problema onde alguns comandos `network watcher` iriam declarar que o Observador de Rede não está habilitado para regiões quando na verdade é [#6264](https://github.com/Azure/azure-cli/issues/6264)

### <a name="sql"></a>SQL

* [ALTERAÇÃO SIGNIFICATIVA] Objetos de resposta alterados retornados dos comandos `db` e `dw`:
    * A propriedade `serviceLevelObjective` foi renomeada para `currentServiceObjectiveName`
    * As propriedades `currentServiceObjectiveId` e `requestedServiceObjectiveId` foram removidas
    * A propriedade `maxSizeBytes` foi alterada para ser um valor inteiro em vez de uma cadeia de caracteres
* [ALTERAÇÃO SIGNIFICATIVA] As propriedades `db` e `dw` a seguir foram alteradas para somente leitura:
    * `requestedServiceObjectiveName`.  Para atualizar, use o parâmetro `--service-objective` ou defina a propriedade `sku.name`
    * `edition`. Para atualizar, use o parâmetro `--edition` ou defina a propriedade `sku.tier`
    * `elasticPoolName`. Para atualizar, use o parâmetro `--elastic-pool` ou defina a propriedade `elasticPoolId`
* [ALTERAÇÃO SIGNIFICATIVA] As propriedades `elastic-pool` a seguir foram alteradas para somente leitura:
    * `edition`. Para atualizar, use o parâmetro `--edition`
    * `dtu`. Para atualizar, use o parâmetro `--capacity`
    *  `databaseDtuMin`. Para atualizar, use o parâmetro `--db-min-capacity`
    *  `databaseDtuMax`. Para atualizar, use o parâmetro `--db-max-capacity`
* Os parâmetros `--family` e `--capacity` foram adicionados aos comandos `db`, `dw` e `elastic-pool`.
* Os formatadores de tabela foram adicionados aos comandos `db`, `dw` e `elastic-pool`.

### <a name="storage"></a>Armazenamento

* Complemento adicionado ao argumento `--account-name`
* O problema com `storage entity query` foi corrigido

### <a name="vm"></a>VM

* [ALTERAÇÃO SIGNIFICATIVA] Removeu `--write-accelerator` de `vm create`. O mesmo suporte pode ser acessado por meio de `vm update` ou `vm disk attach`
* Imagem de extensão fixa correspondente em `[vm|vmss] extension`
* `--boot-diagnostics-storage` foi adicionado a `vm create` para capturar o log de inicialização
* `--license-type` foi adicionado a `[vm|vmss] update`

## <a name="may-7-2018"></a>7 de maio de 2018

Versão 2.0.32

### <a name="core"></a>Núcleo

* Foi corrigida uma exceção sem tratamento ao recuperar segredos de uma conta de entidade de serviço com certificado
* Adicionado suporte limitado para argumentos posicionais
* Corrigir problema no qual `--query` não pôde ser usado com `--ids`. [#5591](https://github.com/Azure/azure-cli/issues/5591)
* Foram melhorados os cenários de redirecionamento de comandos ao usar `--ids`. Oferece suporte a `-o tsv` com uma consulta especificada ou `-o json` sem especificar uma consulta
* Foram adicionadas sugestões de comando sobre o erro se os usuários cometeram algum erro de digitação em seus comandos
* Erro corrigido quando os usuários digitam `az ''`
* Foram adicionados tipos de recursos personalizados com suporte para módulos de comando e extensões

### <a name="acr"></a>ACR

* Foram adicionados comandos de compilação de ACR
* O recurso aprimorado não encontrou mensagens de erro
* Desempenho de criação de recurso aprimorado e tratamento de erros
* Logon de acr aprimorado em consoles não padrão e WSL
* Mensagens de erro de comandos de repositório aprimoradas
* Colunas de tabela e ordenação atualizadas

### <a name="acs"></a>ACS

* Foi adicionado um aviso informando que `az aks` é um serviço de versão prévia
* Foi corrigido um problema de permissão em `aks install-connector` quando `--aci-resource-group` não for especificado

### <a name="ams"></a>AMS

* Versão inicial — Gerenciar recursos dos Serviços de Mídia do Azure

### <a name="appservice"></a>AppService

* Correção de bug no `webapp delete` quando `--slot` é fornecido
* `--runtime-version` foi removido de `webapp auth update`
* Foi adicionado suporte para min\_tls\_versão e https2.0
* Suporte adicionado para vários contêineres

### <a name="batch-ai"></a>Lote AI

* O `batchai create cluster` foi alterado para respeitar a prioridade de VM configurada no arquivo de configuração do cluster

### <a name="cognitive-services"></a>Serviços Cognitivos

* Foi corrigido um erro de digitação no exemplo para `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)

### <a name="consumption"></a>Consumo

* Foram adicionados novos comandos para a API de orçamento

### <a name="container"></a>Contêiner

* Requisito removido para `--registry-server` e `container create` quando um servidor de registro estiver incluído no nome da imagem

### <a name="cosmos-db"></a>Cosmos DB

* Introdução ao suporte de rede virtual para a CLI do Azure — Cosmos DB

### <a name="dms"></a>DMS

* Versão inicial — Adiciona suporte ao SQL para o cenário de migração do SQL do Azure

### <a name="extension"></a>Extensão

* Correção do bug em que os metadados de extensão pararam de ser exibidos

### <a name="interactive"></a>Interativo

* Permitir que complementos interativos funcionem com argumentos posicionais
* Resultado mais simplificado quando os usuários digitam '\'
* Conclusões corrigidas para parâmetros sem ajuda
* Descrições corrigidas para grupos de comando

### <a name="lab"></a>Laboratório

* Regressões corrigidas de conversão de aptidão

### <a name="network"></a>Rede

* [ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--ids` removido de:
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a>Perfil

* Detecção de origem do `disk create` corrigida
* [ALTERAÇÃO SIGNIFICATIVA] `--msi-port` e `--identity-port` removidos porque não são mais usados
* Erro de digitação corrigido no resumo do `account get-access-token`

### <a name="redis"></a>Redis

* `redis patch-schedule patch-schedule show` preterido em favor de `redis patch-schedule show`
* `redis list-all` preterido. Esta funcionalidade foi dobrada em `redis list`
* `redis import-method` preterido em favor de `redis import`
* Foi adicionado suporte a `--ids` para vários comandos

### <a name="role"></a>Função

* [ALTERAÇÃO SIGNIFICATIVA] Remoção de `ad sp reset-credentials` preterido

### <a name="storage"></a>Armazenamento

* Permitir que o token SAS de destino aplique na origem a cópia do blob se a SAS de origem e a chave de conta não forem especificadas
* Exposto -- tempo limite do soquete para carregamentos e downloads de blobs
* Tratar os nomes de blobs que começam com separadores de caminho como caminhos relativos
* Permitir `storage blob copy --source-sas` com a inicialização char de consulta, '?'
* `storage entity query --marker` foi corrigido para aceitar a lista de chaves = valores

### <a name="vm"></a>VM

* Uma lógica de detecção inválida foi corrigida no URI do blob não gerenciado
* Adicionada criptografia de disco de suporte sem entidades de serviço fornecidas pelo usuário
* [ALTERAÇÃO SIGNIFICATIVA] Não usar a VM 'ManagedIdentityExtension' para suporte de MSI
* Suporte adicionado para a política de remoção em `vmss`
* [ALTERAÇÃO SIGNIFICATIVA] Removeu `--ids` de:
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* Foi adicionado suporte do acelerador de gravação
* Adicionado `vmss perform-maintenance`
* `vm diagnostics set` foi corrigido para detectar o tipo de sistema operacional da VM de forma confiável
* `vm resize` foi alterado para verificar se o tamanho solicitado é diferente daquele definido no momento e atualizar somente na alteração


## <a name="april-10-2018"></a>10 de abril de 2018

Versão 2.0.31

### <a name="acr"></a>ACR

* Melhoria do tratamento de erros do fallback do wincred

### <a name="acs"></a>ACS

* Alteração da validade de SPNs criados pelo AKS para 5 anos

### <a name="appservice"></a>AppService

* [ALTERAÇÃO SIGNIFICATIVA]: Removed `assign-identity`
* Correção da exceção não identificada de planos de webapp inexistentes

### <a name="batchai"></a>BatchAI

* Adição de suporte para a API 2018-03-01

 - Montagem de nível de trabalho
 - Variáveis de ambiente com valores secretos
 - Configurações de contadores de desempenho
 - Relatório de segmento de linha específico de trabalho
 - Suporte para subpastas na API de arquivos de lista
 - Relatório de uso e limites
 - Permitir a especificação do tipo de cache para servidores NFS
 - Suporte para imagens personalizadas
 - Adição de suporte para o kit de ferramentas pyTorch

* Adição do comando `job wait`, que permite aguardar a conclusão do trabalho e relata o código de saída de trabalho
* Adição do comando `usage show` para listar o uso e os limites do IA do Lote atual para diferentes regiões
* Há suporte para nuvens nacionais
* Adição de argumentos de linha de comando do trabalho para montar sistemas de arquivos no nível de trabalho, além de arquivos de configuração
* Adição de mais opções para personalizar clusters — prioridade de VM, sub-rede, contagem inicial de nós para clusters de dimensionamento automático, especificando a imagem personalizada
* Adição de opção de linha de comando para especificar o tipo de cache de NFS gerenciado por IA do Lote
* Simplificação da especificação do sistema de arquivos de montagem nos arquivos de configuração. Agora é possível omitir as credenciais do Compartilhamento de arquivos do Azure e Contêineres de Blob do Azure — a CLI preencherá credenciais ausentes usando a chave da conta de armazenamento fornecida por meio dos parâmetros de linha de comando ou especificada por meio da variável de ambiente ou consultará a chave a partir do Armazenamento do Azure (se a conta de armazenamento pertencer à assinatura atual)
* O comando do fluxo de arquivo de trabalho agora é preenchido automaticamente quando o trabalho é concluído (com êxito, com falha, encerrado ou excluído)
* Melhoria da saída de `table` para operações de `show`
* Adição da opção `--use-auto-storage` para a criação de cluster. Essa opção simplifica o gerenciamento de contas de armazenamento e a montagem do Compartilhamento de arquivos do Azure e dos Contêineres de Blob do Azure para clusters
* Adição da opção `--generate-ssh-keys` para `cluster create` e `file-server create`
* Adição da capacidade de fornecer a tarefa de configuração de nó por meio da linha de comando
* [ALTERAÇÃO SIGNIFICATIVA] Comandos `job stream-file` e `job list-files` movidos para o grupo `job file`
* [ALTERAÇÃO SIGNIFICATIVA] `--admin-user-name` renomeado para `--user-name` no comando `file-server create` para ser consistente com o comando `cluster create`

### <a name="billing"></a>Cobrança

* Adição de comandos da conta de registro

### <a name="consumption"></a>Consumo

* Adicionados os comandos `marketplace`
* [ALTERAÇÃO SIGNIFICATIVA] `reservations summaries` renomeado para `reservation summary`
* [ALTERAÇÃO SIGNIFICATIVA] `reservations details` renomeado para `reservation detail`
* [ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--reservation-order-id` e `--reservation-id` para os comandos `reservation`
* [ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--grain` para os comandos `reservation summary`
* [ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--include-meter-details` para os comandos `pricesheet`

### <a name="container"></a>Contêiner

* Adição dos parâmetros de montagem de volume de repositório git `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` e `--gitrepo-mount-path`
* Correção de [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` com falha com --container-name especificado

### <a name="extension"></a>Extensão

* Alteração da mensagem de verificação de distribuição para ser de nível de depuração

### <a name="interactive"></a>Interativo

* Alteração para interromper as conclusões após comandos não reconhecidos
* Adição de ganchos de eventos antes e depois da criação da subárvore do comando
* Adição de conclusão para parâmetros `--ids`

### <a name="network"></a>Rede

* Correção de [#5936](https://github.com/Azure/azure-cli/issues/5936): as marcas `application-gateway create` não podiam ser definidas
* Adição do argumento `--auth-certs` para anexar certificados de autenticação para `application-gateway http-settings [create|update]`. [#4910](https://github.com/Azure/azure-cli/issues/4910)
* Adição dos comandos `ddos-protection` para criar planos de proteção contra DDoS
* Adição de suporte de `--ddos-protection-plan` a `vnet [create|update]` para associar uma VNET a um plano de proteção contra DDoS
* Correção do problema com o sinalizador `--disable-bgp-route-propagation` em `network route-table [create|update]`
* Remoção de argumentos fictícios `--public-ip-address-type` e `--subnet-type` para `network lb [create|update]`
* Adição de suporte para registros TXT com sequências de escape RFC 1035 para `network dns zone [import|export]` e `network dns record-set txt add-record`

### <a name="profile"></a>Perfil

* Adição de suporte para contas clássicas do Azure em `account list`
* [ALTERAÇÃO SIGNIFICATIVA] Remoção dos argumentos `--msi` & `--msi-port`

### <a name="rdbms"></a>RDBMS

* Adicionado o comando `georestore`
* Remoção da restrição de tamanho de armazenamento do comando `create`

### <a name="resource"></a>Recurso

* Adicionado o suporte ao `--metadata` para `policy definition create`
* Adição de suporte para `--metadata`, `--set`, `--add`, `--remove` para `policy definition update`

### <a name="sql"></a>SQL

* Adição de `sql elastic-pool op list` e `sql elastic-pool op cancel`

### <a name="storage"></a>Armazenamento

* Melhoria de mensagens de erro para cadeias de conexão malformadas

### <a name="vm"></a>VM

* Adição de suporte para configurar a contagem de domínios de falha da plataforma para `vmss create`
* Alteração de `vmss create` para balanceador de carga padrão para um conjunto de dimensionamento desabilitado zonal, grande ou de único grupo de posicionamento
* [ALTERAÇÃO SIGNIFICATIVA]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret`
* Adição de suporte para a SKU de IP público para `vm create`
* Adição dos argumentos `--keyvault` e `--resource-group` para `vm secret format` para oferecer suporte a cenários em que o comando não é capaz de resolver a ID do cofre. [#5718](https://github.com/Azure/azure-cli/issues/5718)
* Melhoria de erros de `[vm|vmss create]` quando um local do grupo de recursos não tem suporte de zona


## <a name="march-27-2018"></a>27 de março de 2018

Versão 2.0.30

### <a name="core"></a>Núcleo

* Mostrar mensagem para extensões marcadas como versão prévia na Ajuda

### <a name="acs"></a>ACS

* Corrija o erro de verificação de certificado SSL para `aks install-cli` no Cloud Shell

### <a name="appservice"></a>AppService

* Adição do suporte somente para HTTPS para `webapp update`
* Adição do suporte para os slots `az webapp identity [assign|show]` e `az functionapp identity [assign|show]`

### <a name="backup"></a>Backup

* Adição do novo comando `az backup protection isenabled-for-vm`. Esse comando pode ser usado para verificar se o backup de uma VM é realizado por qualquer cofre na assinatura
* Habilitação das IDs de objeto do Azure para os parâmetros `--resource-group` e `--vault-name` para os seguintes comandos:
  * `backup container show`
  * `backup item set-policy`
  * `backup item show`
  * `backup job show`
  * `backup job stop`
  * `backup job wait`
  * `backup policy delete`
  * `backup policy get-default-for-vm`
  * `backup policy list-associated-items`
  * `backup policy set`
  * `backup policy show`
  * `backup protection backup-now`
  * `backup protection disable`
  * `backup protection enable-for-vm`
  * `backup recoverypoint show`
  * `backup restore files mount-rp`
  * `backup restore files unmount-rp`
  * `backup restore restore-disks`
  * `backup vault delete`
  * `backup vault show`
* `--name` parâmetros alterados a fim de aceitar o formato de saída dos comandos `backup ... show`

### <a name="container"></a>Contêiner

* Adição do comando `container exec`. Executa comandos em um contêiner para um grupo de contêiner em execução
* Permitir a saída da tabela para criar e atualizar um grupo de contêiner

### <a name="extension"></a>Extensão

* Mensagem adicionada para `extension add`, se a extensão estiver no modo de versão prévia
* `extension list-available` alterado para mostrar dados de extensão total com `--show-details`
* [ALTERAÇÃO SIGNIFICATIVA] `extension list-available` alterado para mostrar dados de extensão simplificados por padrão

### <a name="interactive"></a>Interativo

* Alteração nas conclusões para ativar após a conclusão do carregamento da tabela de comandos
* Correção de bug usando o parâmetro `--style`
* Analisador léxico interativo instanciado após a falta do despejo da tabela de comandos
* Suporte aprimorado ao completador

### <a name="lab"></a>Laboratório

* Correção de bugs com o comando `create environment`

### <a name="monitor"></a>Monitoramento

* Adição de suporte para `--top`, `--orderby` e `--namespace` para `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)
* [#4529](https://github.com/Azure/azure-cli/issues/5785) corrigido: `metrics list` aceita uma lista separada por espaços de métricas para recuperação
* Adição de suporte para `--namespace` para `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)

### <a name="network"></a>Rede

* Adição de suporte para zonas DNS privado

### <a name="profile"></a>Perfil

* Adição de avisos para `--identity-port` e `--msi-port` para `login`

### <a name="rdbms"></a>RDBMS

* Adição de modelo de negócios GA API versão 2017-12-01

### <a name="resource"></a>Recurso

* [ALTERAÇÃO SIGNIFICATIVA]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a>Função

* Adição de suporte para configurações de acesso necessário e clientes nativos para `az ad app create`
* `rbac` comandos alterados para retornar menos de 1000 IDs na resolução do objeto
* Adição de comandos de gerenciamento de credencial `ad sp credential [reset|list|delete]`
* [ALTERAÇÃO SIGNIFICATIVA] "Propriedades" removidas da saída `az role assignment [list|show]`
* Adição de suporte para as permissões `dataActions` e `notDataActions` para `role definition`

### <a name="storage"></a>Armazenamento

* Correção de problema ao carregar um arquivo com tamanho entre 195 e 200 GB
* [4049#](https://github.com/Azure/azure-cli/issues/4049) corrigido: problemas com o acréscimo de uploads de blob ignorando os parâmetros da condição

### <a name="vm"></a>VM

* Adição de aviso para `vmss create` para alterações de falha futuras para conjuntos com mais de 100 instâncias
* Adição de suporte com flexibilidade de região para `vm [snapshot|image]`
* Alteração no modo de exibição de instância de disco para reportar status de criptografia mais adequados
* [ALTERAÇÃO SIGNIFICATIVA] `vm extension delete` alterado para não retornar mais a saída

## <a name="march-13-2018"></a>13 de março de 2018

Versão 2.0.29

### <a name="acr"></a>ACR

* Suporte adicionado do parâmetro `--image` a `repository delete`
* Parâmetros `--manifest` e `--tag` preteridos do comando `repository delete`
* Comando `repository untag` adicionado para remover uma marcação sem excluir dados

### <a name="acs"></a>ACS

* Comando `aks upgrade-connector` adicionado para atualizar um conector existente
* Arquivos de configuração `kubectl` alterados para usar um YAML mais legível em bloco

### <a name="advisor"></a>Supervisor

* [ALTERAÇÃO SIGNIFICATIVA] `advisor configuration get` renomeado para `advisor configuration list`
* [ALTERAÇÃO SIGNIFICATIVA] `advisor configuration set` renomeado para `advisor configuration update`
* [ALTERAÇÃO SIGNIFICATIVA] `advisor recommendation generate` removido
* Parâmetro `--refresh` adicionado a `advisor recommendation list`
* Adicionado o comando `advisor recommendation show`

### <a name="appservice"></a>AppService

* Preterido `[webapp|functionapp] assign-identity`
* Comandos de identidade gerenciada `webapp identity [assign|show]` e `functionapp identity [assign|show]` adicionados

### <a name="eventhubs"></a>Hubs de eventos

* Versão inicial

### <a name="extension"></a>Extensão

* Verificação adicionada para avisar ao usuário se a distribuição usada é diferente da armazenado no arquivo de origem do pacote, pois isso pode levar a erros

### <a name="interactive"></a>Interativo

* [5625](https://github.com/Azure/azure-cli/issues/5625) corrigido: manter histórico em sessões diferentes
* [3016](https://github.com/Azure/azure-cli/issues/3016) corrigido: histórico não registrado no escopo
* [5688](https://github.com/Azure/azure-cli/issues/5688) corrigido: as conclusões não aparecerão se o carregamento da tabela de comando encontrou uma exceção
* Medidor de progresso corrigido para operações de longa execução

### <a name="monitor"></a>Monitoramento

* Comandos `monitor autoscale-settings` preteridos
* Adicionados os comandos `monitor autoscale`
* Adicionados os comandos `monitor autoscale profile`
* Adicionados os comandos `monitor autoscale rule`

### <a name="network"></a>Rede

* [ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--tags` removido de `route-filter rule create`
* Valores padrão incorretos removidos dos seguintes comandos:
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* Comandos `network watcher connection-monitor` adicionados
* Parâmetros `--vnet` e `--subnet` adicionados a `network watcher show-topology`

### <a name="profile"></a>Perfil

* Parâmetro `--msi` preterido de `az login`
* Parâmetro `--identity` adicionado de `az login` para substituir `--msi`

### <a name="rdbms"></a>RDBMS

* [VISUALIZAÇÃO] Alterado para usar a API 2017-12-01-preview

### <a name="service-bus"></a>Barramento de Serviço

* Versão inicial

### <a name="storage"></a>Armazenamento

* [#4971](https://github.com/Azure/azure-cli/issues/4971) corrigido: `storage blob copy` agora dá suporte a outras nuvens do Azure
* [5286](https://github.com/Azure/azure-cli/issues/5286) corrigido: os comandos em lotes `storage blob [delete-batch|download-batch|upload-batch]` não geram mais um erro após falhas da pré-condição

### <a name="vm"></a>VM

* Suporte adicionado a `[vm|vmss] create` anexar discos de dados não gerenciados e configurar o cache
* `[vm|vmss] assign-identity` e `[vm|vmss] remove-identity` preteridos
* Comandos `vm identity [assign|remove|show]` e `vmss identity [assign|remove|show]` adicionados para substituir comandos preteridos
* Prioridade padrão alterada em `vmss create` para None

## <a name="february-27-2018"></a>27 de fevereiro de 2018

Versão 2.0.28

### <a name="core"></a>Núcleo

* Correção [#5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalação do Homebrew
* Adição de suporte para telemetria de extensão com chaves personalizadas
* Adição de log HTTP em `--debug`

### <a name="acs"></a>ACS

* Alteração para usa o gráfico `virtual-kubelet-for-aks` do Helm para `aks install-connector` por padrão
* Correção do problema de permissão insuficiente para entidades de serviço criarem um grupo de contêiner ACI
* Adição dos parâmetros `--aci-container-group`, `--location` e `--image-tag` ao `aks install-connector`
* Remoção do aviso de reprovação de `aks get-versions`

### <a name="appservice"></a>AppService

* Atualizações para a nova versão do SDK (azure-mgmt-web 0.35.0)
* Correção [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` relatado como SKU inválido

### <a name="cognitive-services"></a>Serviços Cognitivos

* Atualização do “aviso” ao criar uma nova conta dos Serviços Cognitivos

### <a name="consumption"></a>Consumo

* Adição de novos comandos para a API pricesheet
* Atualização dos formatos existentes de Detalhes de uso e Detalhes de reserva

### <a name="container"></a>Contêiner

* Adição dos argumentos `--secrets` e `--secrets-mount-path` ao `container create` para usar segredos na ACI

### <a name="network"></a>Rede

* Correção [#5559](https://github.com/Azure/azure-cli/issues/5559): cliente ausente em `network vnet-gateway vpn-client generate`

### <a name="resource"></a>Recurso

* Alteração do `group deployment export` para exibir um modelo parcial e erros ao falhar

### <a name="role"></a>Função

* Adição de `role assignment list-changelogs` para permitir a auditoria das funções da entidade de serviço

### <a name="sql"></a>SQL

* Adição de suporte para a redundância de zona para os bancos de dados e pools elásticos em criação ou atualização

### <a name="storage"></a>Armazenamento

* Habilitação de especificação de caminho de destino/prefixo do `storage blob [upload-batch|download-batch]`

### <a name="vm"></a>VM

* Adição de suporte para anexar/desanexar discos em uma instância única de VMSS


## <a name="february-13-2018"></a>13 de fevereiro de 2018

Versão 2.0.27

### <a name="core"></a>Núcleo

* Alterada a autenticação para chave tanto na ID de assinatura quanto no nome de logon do MSI

### <a name="acs"></a>ACS

* [ALTERAÇÃO SIGNIFICATIVA] `aks get-versions` renomeado para `aks get-upgrades` para fins de precisão
* `aks get-versions` alterado para mostrar versões do Kubernetes disponíveis para `aks create`
* Alterados os padrões de `aks create` para permitir que o servidor escolha a versão do Kubernetes
* Atualizadas as mensagens de ajuda sobre a entidade de serviço gerada pelo AKS
* Alterados os tamanhos de nó padrão para `aks create` de “Standard\_D1\_v2” para “Standard\_DS1\_v2”
* Aumentada a confiabilidade ao localizar o pod de painel para `az aks browse`
* `aks get-credentials` corrigido para tratar de erros de Unicode ao carregar arquivos de configuração do Kubernetes
* Adicionada uma mensagem para `az aks install-cli` para ajudar a obter `kubectl` em `$PATH`

### <a name="appservice"></a>AppService

* Corrigido o problema em que `webapp [backup|restore]` falhou devido a uma referência nula
* Adicionado suporte para planos de serviço de aplicativo padrão por meio de `az configure --defaults appserviceplan=my-asp`

### <a name="cdn"></a>CDN

* Adicionados os comandos `cdn custom-domain [enable-https|disable-https]`

### <a name="container"></a>Contêiner

* Adicionada a opção `--follow` para `az container logs` para logs de streaming
* Adicionado o comando `container attach` que anexa fluxos locais de saída e erro padrão para um contêiner em um grupo de contêiner

### <a name="cosmosdb"></a>CosmosDB

* Adicionado suporte para a configuração de recursos

### <a name="extension"></a>Extensão

* Adicionado suporte para parâmetro `--pip-proxy` para comandos `az extension [add|update]`
* Adicionado suporte para argumento `--pip-extra-index-urls` para comandos `az extension [add|update]`

### <a name="feedback"></a>Comentários

* Adicionadas informações de extensão aos dados de telemetria

### <a name="interactive"></a>Interativo

* Corrigido o problema em que o usuário é solicitado a fazer logon ao usar o modo interativo no Cloud Shell
* Corrigida a regressão com conclusões de parâmetro ausentes

### <a name="iot"></a>IoT

* Correção do problema em que `iot dps access policy [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso
* Correção do problema em que `iot dps linked-hub [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso
* Adicionado o suporte `--no-wait` para `iot dps access policy [create|update]` e `iot dps linked-hub [create|update]`
* `iot hub create` alterado para permitir a especificação do número de partições

### <a name="monitor"></a>Monitoramento

* Corrigido o comando `az monitor log-profiles create`

### <a name="network"></a>Rede

* Corrigida a opção `--tags` para os seguintes comandos:
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a>Perfil

* `az login` habilitado no modo interativo

### <a name="resource"></a>Recurso

* `feature show` adicionado novamente

### <a name="role"></a>Função

* Adicionado o argumento `--available-to-other-tenants` para `ad app update`

### <a name="sql"></a>SQL

* Adicionados os comandos `sql server dns-alias`
* Adicionado `sql db rename`
* Adicionado suporte para o argumento `--ids` para todos os comandos sql

### <a name="storage"></a>Armazenamento

* Adicionados os comandos `storage blob service-properties delete-policy` e `storage blob undelete` para habilitar a exclusão reversível

### <a name="vm"></a>VM

* Corrigida uma falha quando a criptografia de VM não pode ser totalmente inicializada
* Adicionada saída de ID de entidade de segurança ao habilitar o MSI
* `vm boot-diagnostics get-boot-log` fixo


## <a name="january-31-2018"></a>31 de janeiro de 2018

Versão 2.0.26

### <a name="core"></a>Núcleo

* Adicionado suporte para recuperação de token bruto no contexto MSI
* Removida a cadeia de caracteres do indicador de sondagem depois de terminar o LRO no Windows cmd.exe
* Adicionado um aviso que aparece ao usar um padrão configurado que foi alterado para uma entrada de nível de informações. Usar `--verbose` para ver
* Adicionar um indicador de progresso para comandos de espera

### <a name="acs"></a>ACS

* Argumento `--disable-browser` esclarecido
* Preenchimento de guia melhorado para argumentos `--vm-size`

### <a name="appservice"></a>AppService

* `webapp log [tail|download]` fixo
* Removida a verificação de `kind` em aplicativos Web e funções

### <a name="cdn"></a>CDN

* Corrigido o problema de cliente ausente com `cdn custom-domain create`

### <a name="cosmosdb"></a>CosmosDB

* Corrigida a descrição do parâmetro para políticas de failover

### <a name="interactive"></a>Interativo

* Corrigido o problema em que as conclusões de opção de comando não aparecem mais

### <a name="network"></a>Rede

* Adicionada a proteção para `--cert-password` para `application-gateway create`
* Corrigido o problema com `application-gateway update` em que `--sku` aplicou um valor padrão de forma errada
* Adicionada proteção para `--shared-key` e `--authorization-key` para `vpn-connection create`
* Corrigido o problema de cliente ausente com `asg create`
* Adicionado o parâmetro `--file-name / -f` para nomes exportados para `dns zone export`
* Os seguintes problemas foram corrigidos com `dns zone export`:
  * Corrigido o problema em que registros TXT longos foram exportados incorretamente
  * Corrigido o problema em que registros TXT entre aspas foram exportados incorretamente sem as aspas com caracteres de escape
* Corrigido o problema em que determinados registros foram importados duas vezes com `dns zone import`
* Restaurados os comandos `vnet-gateway root-cert` e `vnet-gateway revoked-cert`

### <a name="profile"></a>Perfil

* `get-access-token` corrigido para trabalhar em uma VM com identidade

### <a name="resource"></a>Recurso

* Corrigido o bug com `deployment [create|validate]` em que um aviso era exibido incorretamente quando um campo ‘tipo’ do modelo continha valores maiúsculos

### <a name="storage"></a>Armazenamento

* Corrigido o problema com a migração de contas de Armazenamento V1 para Armazenamento V2
* Adicionado o relatório de andamento de todos os comandos de upload/download
* Corrigido o bug que impedia a opção “-n” arg com `storage account check-name`
* Adicionada a coluna ‘instantâneo’ à saída de tabela para `blob [list|show]`
* Corrigidos bugs com vários parâmetros que precisam ser analisados como ints

### <a name="vm"></a>VM

* Adicionado o comando `vm image accept-terms` para permitir a criação de VMs a partir de imagens com encargos adicionais
* `[vm|vmss create]` corrigido para garantir que comandos possam ser executados sob o proxy com certificados não assinados
* [VERSÃO PRÉVIA] Adicionado suporte para “baixa” prioridade para VMSS
* Adicionada a proteção para `--admin-password` para `[vm|vmss] create`


## <a name="january-17-2018"></a>17 de janeiro de 2018

Versão 2.0.25

### <a name="acr"></a>ACR

* Adicionado fallback de logon de acr em erros de credencial do Windows
* Habilitados os logs de registro

### <a name="acs"></a>ACS

* Corrigido o comando `get-credentials`
* Removido o requisito de função do SPN

### <a name="appservice"></a>AppService

* Corrigido o bug com `config ssl upload` onde `hosting_environment_profile` era nulo
* Adicionado suporte para URLs personalizadas para `browse`
* Corrigido o suporte de slot para `log tail`

### <a name="backup"></a>Backup

* Alterada a opção `--container-name` de `backup item list` para ser opcional
* Adicionadas opções da conta de armazenamento para `backup restore restore-disks`
* Corrigido o check-in de local de `backup protection enable-for-vm` para não diferenciar maiúsculas e minúsculas
* Corrigido o problema em que os comandos falhavam com um nome de contêiner inválido
* Alterado `backup item list` para incluir o 'Status de Integridade' como padrão

### <a name="batch"></a>Lote

* Alterado `batch login` para retornar detalhes de autenticação

### <a name="cloud"></a>Nuvem

* Alterado para não exigir pontos de extremidade ao definir `--profile` em uma nuvem

### <a name="consumption"></a>Consumo

* Adicionados novos comandos para reservas: `consumption reservations summaries` e `consumption reservations details`

### <a name="event-grid"></a>Grade de Eventos

* [ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid topic event-subscription` transferidos para `eventgrid event-subscription`
* [ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid resource event-subscription` transferidos para `eventgrid event-subscription`
* [ALTERAÇÃO SIGNIFICATIVA] Comando `eventgrid event-subscription show-endpoint-url` removido. Usar `eventgrid event-subscription show --include-full-endpoint-url`
* Adicionado o comando `eventgrid topic update`
* Adicionado o comando `eventgrid event-subscription update`
* Adicionado o parâmetro `--ids` para comandos `eventgrid topic`
* Adicionado o suporte de conclusão de guia para nomes de tópico

### <a name="interactive"></a>Interativo

* Corrigido o problema em que o modo interativo não funcionava com o Python 2.x
* Corrigidos os erros na inicialização
* Corrigido o problema com alguns comandos que não estavam em execução no modo interativo

### <a name="iot"></a>IoT

* Adicionado suporte para o serviço de provisionamento de dispositivos
* Adicionadas mensagens de reprovação em comandos e ajuda de comando
* Adicionada verificação de IoT para informar os usuários da Extensão de IoT

### <a name="monitor"></a>Monitoramento

* Adicionado o suporte de configuração de vários diagnósticos. Agora o parâmetro `--name` é necessário para `az monitor diagnostic-settings create`
* Adicionado o comando `monitor diagnostic-settings categories` para obter a categoria de configurações de diagnóstico

### <a name="network"></a>Rede

* Corrigido o problema ao tentar alterar de/para o modo ativo-em espera com `vnet-gateway update`
* Adicionado o suporte para HTTP2 para `application-gateway [create|update]`

### <a name="profile"></a>Perfil

* Adicionado o suporte para logon com identidades atribuídas ao usuário

### <a name="role"></a>Função

* Adicionado o argumento `--assignee-object-id` para `role assignment create` para ignorar a consulta do gráfico

### <a name="service-fabric"></a>Service Fabric

* Adicionados erros detalhados à resposta de validação ao criar cluster
* Corrigido o problema de cliente ausente com vários comandos

### <a name="vm"></a>VM

* [VERSÃO PRÉVIA] Suporte entre zonas para `vmss`
* [ALTERAÇÃO SIGNIFICATIVA] Alterada única zona `vmss` padrão para o balanceador de carga "Padrão"
* [ALTERAÇÃO SIGNIFICATIVA] `externalIdentities` alterado para `userAssignedIdentities` para EMSI
* [VERSÃO PRÉVIA] Adicionado o suporte para a troca de disco do sistema operacional
* Adicionado o suporte para o uso de imagens da VM de outras assinaturas
* Adicionados os argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` e `--plan-publisher` para `[vm|vmss] create`
* Corrigidos os problemas de erro com `[vm|vmss] create`
* Corrigido o uso excessivo de recursos causados por `vm image list --all`

## <a name="december-19-2017"></a>19 de dezembro de 2017

Versão 2.0.23

* Adicionado o suporte para logon com identidades atribuídas ao usuário

### <a name="container"></a>Contêiner

* Corrigida a ordem incorreta de parâmetros para logs de contêiner

### <a name="network"></a>Rede

* Adicionado o argumento `--disable-bgp-route-propagation` para `route-table [create|update]`
* Adicionado o argumento `--ip-tags` para `public-ip [create|update]`

### <a name="storage"></a>Armazenamento

* Adicionado suporte para armazenamento V2

### <a name="vm"></a>VM

* [VERSÃO PRÉVIA] Adicionado suporte para identidades atribuídas a usuários para VMs e VMSSes


## <a name="december-5-2017"></a>5 de dezembro de 2017

Versão 2.0.22

* Comandos `az component` removidos. Usar `az extension`

### <a name="core"></a>Núcleo
* Modificou o ponto de extremidade de autoridade AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com para login.microsoftonline.us
* Corrigido o problema onde a telemetria reenviaria continuamente

### <a name="acs"></a>ACS

* Comandos `aks install-connector` e `aks remove-connector` adicionados
* Relatório de erros aprimorado para `acs create`
* Corrigido o uso de `aks get-credentials -f` sem um caminho totalmente qualificado

### <a name="advisor"></a>Supervisor

* Versão inicial

### <a name="appservice"></a>AppService

* Corrigida a geração de nome do certificado com `webapp config ssl upload`
* Corrigidos `webapp [list|show]` e `functionapp [list|show]` para exibir os aplicativos corretos
* Valor padrão adicionado para `WEBSITE_NODE_DEFAULT_VERSION`

### <a name="consumption"></a>Consumo

* Suporte adicionado para a API versão de 30/11/2017

### <a name="container"></a>Contêiner

* Corrigida a regressão de portas padrão

### <a name="monitor"></a>Monitoramento

* Suporte de várias dimensões adicionado ao comando de métricas

### <a name="resource"></a>Recurso

* Adicionado o argumento `--include-response-body` para `resource show`

### <a name="role"></a>Função

* Exibição de atribuições padrão adicionada dos administradores "clássicos" para `role assignment list`
* Suporte adicionado a `ad sp reset-credentials` para adicionar as credenciais em vez de substituir
* Relatório de erros aprimorado para `ad sp create-for-rbac`

### <a name="sql"></a>SQL

* Comandos `sql db list-usages` e `sql db show-usage` adicionados
* Comandos `sql server conn-policy show` e `sql server conn-policy update` adicionados

### <a name="vm"></a>VM

* Informações da zona adicionadas a `az vm list-skus`


## <a name="november-14-2017"></a>14 de novembro de 2017

Versão 2.0.21

### <a name="acr"></a>ACR

* Suporte adicionado para criar webhooks em regiões de replicação


### <a name="acs"></a>ACS

* Alteradas todas as palavras "agente" para "nó" no AKS
* Opção `--orchestrator-release` preterida para `acs create`
* Tamanho alterado da VM padrão do AKS para `Standard_D1_v2`
* `az aks browse` corrigido no Windows
* `az aks get-credentials` corrigido no Windows

### <a name="appservice"></a>AppService

* Origem da implantação adicional `config-zip` para webapps e aplicativos de funções
* Opção `--docker-container-logging` adicionada a `az webapp log config`
* Removida a opção `storage` do parâmetro `--web-server-logging` de `az webapp log config`
* Mensagens de erro aprimoradas para `deployment user set`
* Suporte adicionado para criar aplicativos de funções do Linux
* `list-locations` fixo

### <a name="batch"></a>Lote

* Bug corrigido no comando pool create quando uma ID do recurso foi usada com o sinalizador `--image`

### <a name="batchai"></a>Batchai

* Opção curta adicionada `-s` para `--vm-size` ao fornecer o tamanho da VM no comando `file-server create`
* Nome da conta de armazenamento e argumentos-chave adicionados aos parâmetros `cluster create`
* Documentação corrigida para `job list-files` e `job stream-file`
* Opção curta adicionada `-r` para `--cluster-name` ao fornecer o nome do cluster no comando `job create`

### <a name="cloud"></a>Nuvem

* `cloud [register|update]` alterado para evitar registrar nuvens sem os pontos de extremidade necessários

### <a name="container"></a>Contêiner

* Suporte adicionado para abrir várias portas
* Política de reinicialização do grupo de contêiner adicionada
* Suporte adicionado para montar o compartilhamento de Arquivos do Azure como um volume
* Documentos de ajuda atualizados

### <a name="data-lake-analytics"></a>Data Lake Analytics

* `[job|account] list` alterada para retornar informações mais concisas

### <a name="data-lake-store"></a>Data Lake Store

* `account list` alterada para retornar informações mais concisas

### <a name="extension"></a>Extensão

* `extension list-available` adicionado para permitir a listagem de extensões oficiais da Microsoft
* `--name` adicionado a `extension [add|update]` para permitir a instalação de extensões por nome

### <a name="iot"></a>IoT

* Suporte adicionado para as autoridades de certificação (CA) e cadeias de certificado

### <a name="monitor"></a>Monitoramento

* Adicionados os comandos `activity-log alert`

### <a name="network"></a>Rede

* Suporte adicionado para registros DNS da CAA
* Problema corrigido onde os pontos de extremidade não podem ser atualizados com `traffic-manager profile update`
* Problema corrigido onde `vnet update --dns-servers` não funcionou dependendo de como a VNET foi criada
* Problema corrigido onde os nomes DNS relativos foram importados incorretamente por`dns zone import`

### <a name="reservations"></a>Reservas

* Versão prévia inicial

### <a name="resource"></a>Recurso

* Suporte adicionado das IDs de recurso ao parâmetro `--resource` e bloqueios no nível do recurso

### <a name="sql"></a>SQL

* Parâmetro `--ignore-missing-vnet-service-endpoint` adicionado a `sql server vnet-rule [create|update]`

### <a name="storage"></a>Armazenamento

* `storage account create` criado ao usar o SKU `Standard_RAGRS` como padrão
* Bugs corrigidos ao lidar com nomes de arquivo/blob que incluem caracteres não ascii
* Bug corrigido que impedia usar `--source-uri` com `storage [blob|file] copy start-batch`
* Comandos adicionados para usar o glob e excluir vários objetos com `storage [blob|file] delete-batch`
* Problema corrigido ao habilitar métricas com `storage metrics update`
* Problema corrigido com arquivos acima de 200 GB ao usar `storage blob upload-batch`
* Problema corrigido onde `--bypass` e `--default-action` foram ignorados por `storage account [create|update]`

### <a name="vm"></a>VM

* Bug corrigido com `vmss create`, que impediu o uso da camada de tamanho `Basic`
* Argumentos `--plan` adicionados a `[vm|vmss] create` para ter imagens personalizadas com informações de cobrança
* Comandos `vm secret `[add|remove|list]` adicionados
* `vm format-secret` renomeado para `vm secret format`
* Adicionado o argumento `--encrypt format` para `vm encryption enable`

## <a name="october-24-2017"></a>24 de outubro de 2017

Versão 2.0.20

### <a name="core"></a>Núcleo

* Atualizado `2017-03-09-profile` para usar a `MGMT_STORAGE` versão da API`2016-01-01`

### <a name="acr"></a>ACR

* Gerenciamento de recursos atualizado para apontar para a versão da API `2017-10-01`
* SKU 'traga seu próprio armazenamento' alterada para Clássico
* SKUs de registro renomeados como Básico, Standard e Premium

### <a name="acs"></a>ACS

* [VERSÃO PRÉVIA] Comandos `az aks` adicionados
* Kubernetes `get-credentials` corrigido

### <a name="appservice"></a>AppService

* Problema corrigido onde os logs `webapp` baixados podem ser inválidos

### <a name="component"></a>Componente

* Mensagem de reprovação mais clara adicionada para todos os instaladores e prompt de confirmação

### <a name="monitor"></a>Monitoramento

* Adicionados os comandos `action-group`

### <a name="resource"></a>Recurso

* Incompatibilidade corrigida com a versão mais recente de dependência msrest em `group export`
* `policy assignment create` corrigido para trabalhar com as definições de política internas e as definições do conjunto de políticas

### <a name="vm"></a>VM

* Adicionado o argumento `--accelerated-networking` para `vmss create`


## <a name="october-9-2017"></a>9 de outubro de 2017

Versão 2.0.19

### <a name="core"></a>Núcleo

* Tratamento de URLs de autoridade do AD FS adicionado com uma barra à direita para o Azure Stack

### <a name="appservice"></a>AppService

* Atualização genérica adicionada com o novo comando `webapp update`

### <a name="batch"></a>Lote

* Atualizado para o SDK do Lote 4.0.0
* A opção `--image` de VirtualMachineConfiguration foi atualizada para dar suporte a referências de imagem ARM além de publish:offer:sku:version
* Suporte adicionado para o novo modelo de extensão da CLI para comandos de Extensões de Lote
* Removeu o suporte de Lote do modelo de componente

### <a name="batchai"></a>Batchai

* Versão inicial do módulo de IA de Lote

### <a name="keyvault"></a>Keyvault

* Correção do problema de autenticação do Cofre de Chaves ao usar o AD FS no Azure Stack. [(#4448)](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a>Rede

* Alterado `--server` argumento de `application-gateway address-pool create` para ser opcional, permitindo pools de endereços vazios
* `traffic-manager` foi atualizado para oferecer suporte aos recursos mais recentes

### <a name="resource"></a>Recurso

* Suporte adicionado para `--resource-group/-g` opções do nome do grupo de recursos para `group`
* Comandos adicionados a `account lock` para funcionar com bloqueios no nível da assinatura
* Comandos adicionados a `group lock` para funcionar com bloqueios no nível do grupo
* Comandos adicionados a `resource lock` para funcionar com bloqueios no nível do recurso

### <a name="sql"></a>Sql

* Suporte adicionado para SQL TDE (Transparent Data Encryption) e TDE com Traga sua própria chave
* Comando `db list-deleted` e parâmetro `db restore --deleted-time` adicionados, permitindo localizar e restaurar bancos de dados excluídos
* `db op list` e `db op cancel` adicionados, permitindo listar e cancelar operações em andamento no banco de dados

### <a name="storage"></a>Armazenamento

* Suporte adicionado para instantâneo de compartilhamento de arquivos

### <a name="vm"></a>VM

* Correção de um bug em `vm show` onde o uso de `-d` causou uma falha nos endereços IP privados ausentes
* [VERSÃO PRÉVIA] Suporte adicionado para atualização sem interrupção para `vmss create`
* Suporte adicionado para atualizar as configurações de criptografia com `vm encryption enable`
* Parâmetro `--os-disk-size-gb` adicionado a `vm create`
* Parâmetro `--license-type` adicionado ao Windows para `vmss create`


## <a name="september-22-2017"></a>22 de setembro de 2017

Versão 2.0.1.8

### <a name="resource"></a>Recurso

* Suporte adicionado para mostrar as definições de políticas internas
* Parâmetro de modo de suporte adicionado para a criação de definições de política
* Suporte adicionado para definições de interface do usuário e modelos em `managedapp definition create`
* [ALTERAÇÃO SIGNIFICATIVA] Tipo de recurso `managedapp` alterado de `appliances` para `applications` e de `applianceDefinitions` para `applicationDefinitions`

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

* Foi corrigido o bug 'Não é possível interar CustomDomain' para `cdn custom-domain create`

### <a name="extension"></a>Extensão

* Versão Inicial

### <a name="keyvault"></a>Keyvault

* Foi corrigido o problema onde permissões diferenciavam maiúsculas de minúsculas para `keyvault set-policy`

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

* Nota legal adicionada ao `--version`

### <a name="acs"></a>ACS

* Corrigidas as regiões de visualização
* Corrigida a formatação padrão de `dns_name_prefix`
* Saída de comando ACS otimizada

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
* Adicionado suporte para vários  intervalos de IP e portas para `nsg rule [create|update]`
* Adicionado suporte ao SKU para `lb create`
* Adicionado suporte ao SKU para `public-ip create`

### <a name="profile"></a>Perfil

* `--msi` e `--msi-port` expostos a logon usando a identidade de uma máquina virtual

### <a name="service-fabric"></a>Service Fabric

* Versão prévia
* Simplificadas as regras de registro de usuário/senha para comando
* Corrigido o prompt de senha para o usuário mesmo após a passagem do parâmetro
* Adicionado suporte para `registry_cred` vazio

### <a name="storage"></a>Armazenamento

* Habilitada a camada de blob de configuração
* Adicionados os argumentos `--bypass` e `--default-action` ao `storage account [create|update]` para dar suporte ao serviço de túnel
* Comandos adicionados ao `storage account network-rule` para adicionar as regras de rede virtual e regras baseadas em IP
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

### <a name="batch"></a>Lote

* Atualizado para o Lote SDK 3.1.0 e Gerenciamento de Lote SDK 4.1.0
* Adicionado um novo comando que mostra as contagens de tarefas de um trabalho
* Corrigido o bug no processamento de URL de SAS do arquivo de recurso
* Ponto de extremidade da conta de lote agora dá suporte ao prefixo opcional “https://” 
* Suporte para adicionar listas de mais de 100 tarefas a um trabalho
* Adicionado log de depuração para carregar o módulo do comando de Extensões

### <a name="component"></a>Componente

* Aviso de substituição adicionado aos comandos 'az component'

### <a name="container"></a>Contêiner

* `create`: corrigido o problema onde o sinal de igual não era permitido dentro de uma variável de ambiente


### <a name="data-lake-store"></a>Data Lake Store

* Habilitado o controle do andamento

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

```text
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
* Aprimoramento da desativação de áudio de argumentos de análise e da adição do histórico com gestos (#3434)
* Criar clientes de assinatura com o perfil correto do SDK
* Mover todos os arquivos existentes de gravação para a pasta mais recente
* Corrigida a idempotência para a criação de VM/VMSS (#3586)
* Os caminhos de comando não diferenciam mais maiúsculas de minúsculas
* Determinados parâmetros do tipo booliano não diferenciam mais maiúsculas de minúsculas
* Suporte para logon do ADFS em um servidor local como o Azure Stack
* Corrigidas as gravações simultâneas para clouds.config (#3255)

### <a name="acr"></a>ACR

* Adicionado o comando `show-usage` para registros gerenciados
* Suporte para atualização do SKU para registros gerenciados
* Adicionados registros gerenciados com o SKU gerenciado
* Adicionados webhooks para registros gerenciados com o módulo de comando de webhook do ACR
* Adicionada autenticação do AAD com o comando de logon de ACR
* Adicionado comando de exclusão para marcas, manifestos e repositórios do Docker

### <a name="acs"></a>ACS

* Suporte para a API versão 2017-07-01

### <a name="appservice"></a>AppService

* Corrigido o bug onde listar o aplicativo Web Linux não retornava nada
* Suporte para recuperar credenciais de ACR
* Remover todos os comandos em `appservice web`
* Ocultar as senhas de registro do Docker da saída do comando (#3656)
* Verifique se o navegador padrão é usado no macOS sem erros (#3623)
* Aprimorada a Ajuda de `webapp log tail` e `webapp log download` (#3624)
* Exposto o comando `traffic-routing` para configurar roteamento estático (#3566)
* Adicionadas correções de confiabilidade na configuração de controle do código-fonte (#3245)
* Removido o argumento `--node-version` sem suporte de `webapp config update` para aplicativos Web do Windows. Em vez disso, use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`

### <a name="batch"></a>Lote

* Atualizado para o Lote SDK 3.0.0 com suporte para VMs de baixa prioridade em pools
* Opção `pool create` renomeada como `--target-dedicated` para `--target-dedicated-nodes`
* Adicionadas as opções `pool create` e `--target-low-priority-nodes` de `--application-licenses`

### <a name="cdn"></a>CDN

* Uma mensagem de erro mais adequada foi fornecida para `cdn endpoint list` quando o perfil especificado por `--profile-name` não existir

### <a name="cloud"></a>Nuvem

* Alterada a versão de API do ponto de extremidade de metadados de nuvem para o formato AAAA-MM-DD
* Ponto de extremidade da galeria não é necessário
* Suporte para registrar a nuvem somente com o ponto de extremidade de gerenciador de recursos do ARM
* Fornecida uma opção para `cloud set` para escolher o perfil ao selecionar a nuvem atual
* Exposto `endpoint_vm_image_alias_doc`

### <a name="cosmosdb"></a>CosmosDB

* Corrigida a permissão para criação de coleção com chave de partição personalizada
* Adicionado suporte para o TTL padrão de coleção

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
* Adicionado o formatador de saída da tabela para `az lab vm list` e `az lab vm show`

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
* Exemplos e argumentos de conveniência adicionados ao `monitor alert rule update`

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
* Usar o pool padrão de endereços, configurações de HTTP e o ouvinte HTTP para `application-gateway rule create`, se existir apenas um
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

* Suporte à saída no formato de arquivo de autenticação do SDK para `create-for-rbac`
* Limpar as atribuições de função e aplicativos relacionados ao AAD ao excluir uma entidade de serviço (#3610)
* Incluir o formato de hora nos argumentos `app create` e descrições `--start-date` e `--end-date`
* Mostrar avisos de código obsoleto ao usar `--expanded-view`
* Adicionada a integração do cofre de chaves para os comandos `create-for-rbac` e `reset-credentials`

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
* Corrigido o problema onde `cmss create` com um balanceador de carga existente exigia `--backend-pool-name`
* Os discos de dados criados com LUN do `vm image create` agora começam com 0


## <a name="may-10-2017"></a>10 de maio de 2017

Versão 2.0.6

* Renomeação do DocumentDB para CosmosDB
* Adição do RDBMS (MySQL, Postgres)
* Inclusão dos módulos Data Lake Analytics e Data Lake Store
* Inclusão do módulo Serviços Cognitivos
* Inclusão do módulo Service Fabric
* Inclusão do módulo Interativo (renomeação de az-shell)
* Adição de suporte para comandos CDN
* Remoção do módulo Contêiner
* Adição de “az -v” como atalho para “az --version” ([nº 2926](https://github.com/Azure/azure-cli/issues/2926))
* Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))

```text
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

* Renomeação do módulo DocumentDB para CosmosDB
* Adição de suporte para APIs do plano de dados do DocumentDB: gerenciamento de banco de dados e de coleção
* Adição de suporte para habilitar o failover automático em contas de banco de dados
* Adição de suporte para nova política de consistência ConsistentPrefix

### <a name="data-lake-analytics"></a>Data Lake Analytics

* Correção de um bug em que a filtragem no resultado e no estado das listas de trabalho gera um erro
* Adição de suporte para o novo tipo de item de catálogo: pacote. acessado por meio de: `az dla catalog package`
* Possibilidade de listar os seguintes itens de catálogo no banco de dados (sem a necessidade de especificação de esquema):

  * Tabela
  * Função com valor de tabela
  * Visualizar
  * Estatísticas de Tabela. Isso também pode ser listado com um esquema, mas sem a especificação de um nome de tabela

### <a name="data-lake-store"></a>Data Lake Store

* Atualização da versão do SDK do sistema de arquivos subjacente, que fornece melhor suporte para lidar com cenários de limitação do servidor
* Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))
* Ausência de ajuda para mostrar o acesso. Adição em andamento. ([nº 2743](https://github.com/Azure/azure-cli/issues/2743))

### <a name="find"></a>Localizar

* melhoria dos resultados da pesquisa e permissão de controle de versão do índice de pesquisa

### <a name="keyvault"></a>KeyVault

* BC:`az keyvault certificate download` alteração de -e da cadeia de caracteres ou do binário para PEM ou DER a fim de representar melhor as opções
* BC: remoção de --expires e --not-before de `keyvault certificate create`, pois esses parâmetros não têm suporte no serviço
* Adição do parâmetro --validity a `keyvault certificate create` para substituir seletivamente o valor em --policy
* Correção do problema em `keyvault certificate get-default-policy`, em que “expires” e “not_before” eram expostos, ao contrário de “validity_in_months”
* Correção do cofre de chaves para importação de PEM e PFX ([nº 2754](https://github.com/Azure/azure-cli/issues/2754))

### <a name="lab"></a>Laboratório

* Adição dos comandos create, show, delete e list ao ambiente do laboratório
* Adição dos comandos show e list para exibir modelos ARM no laboratório
* Adição do sinalizador --environment a `az lab vm list` para filtrar as VMs por ambiente no laboratório
* Adição do comando de conveniência `az lab formula export-artifacts` para exportar o scaffold de artefato em uma fórmula do Laboratório
* Adição de comandos para gerenciar segredos em um Laboratório

### <a name="monitor"></a>Monitoramento

* Correção de bug: modelagem de `--actions` de `az alert-rules create` para consumir a cadeia de caracteres JSON ([nº 3009](https://github.com/Azure/azure-cli/issues/3009))
* Correção de bug – as configurações de diagnóstico criam, mas não aceitam logs e métrica de comandos show ([nº 2913](https://github.com/Azure/azure-cli/issues/2913))

### <a name="network"></a>Rede

* Adição do comando `network watcher test-connectivity`
* Adição de suporte para o parâmetro `--filters` de `network watcher packet-capture create`
* Adição de suporte para drenagem de conexão do Gateway de Aplicativo
* Adição de suporte para a configuração do conjunto de regras WAF do Gateway de Aplicativo
* Adição de suporte para filtros de rota e regras do ExpressRoute
* Adição de suporte para o roteamento geográfico do Gerenciador de Tráfego
* Adição de suporte para seletores de tráfego baseados em política da conexão VPN
* Adição de suporte para políticas IPsec da conexão VPN
* Correção de um bug com `vpn-connection create` ao usar os parâmetros `--no-wait` ou `--validate`
* Adição de suporte para gateways de VNet ativos/ativos
* Remoção de valores nulos na saída de comandos `network vpn-connection list/show`
* BC: correção de um bug na saída de `vpn-connection create`
* Correção de um bug em que o argumento “--key-length” de “vpn-connection create” não é analisado corretamente
* Correção de um bug em `dns zone import`, em que os registros não são importados corretamente
* Correção de um bug em que `traffic-manager endpoint update` não funciona
* Adição de comandos de visualização “network watcher”

### <a name="profile"></a>Perfil

* Suporte ao logon quando não há nenhuma assinatura encontrada ([nº 2560](https://github.com/Azure/azure-cli/issues/2560))
* Suporte ao nome curto do parâmetro em az account set --subscription ([nº 2980](https://github.com/Azure/azure-cli/issues/2980))

### <a name="redis"></a>Redis

* Adição do comando update que também adiciona a capacidade de dimensionar o Cache Redis
* Preterição do comando “update-settings”

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

* Adição dos comandos az sql server list-usages e az sql db list-usages
* SQL – capacidade de se conectar diretamente ao provedor de recursos ([nº 2832](https://github.com/Azure/azure-cli/issues/2832))

### <a name="storage"></a>Armazenamento

* Localização padrão da localização do grupo de recursos de `storage account create`
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

Lançamos os componentes ACR, Batch, KeyVault, e SQL nessa versão

```text
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

* Adicionar módulos acr, laboratório, monitor e localizar à lista padrão
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

* Versão inicial do módulo do Data Lake Analytics
* Versão inicial do módulo do Data Lake Store

### <a name="docuemntdb"></a>DocuemntDB

* DocumentDB: Adicionar suporte para a listagem de cadeias de conexão ([#2580](https://github.com/Azure/azure-cli/pull/2580))

### <a name="vm"></a>VM

* [Compute] Adicionar suporte a AppGateway para criar o conjunto de dimensionamento de máquinas virtuais ([#2570](https://github.com/Azure/azure-cli/pull/2570))
* [VM/VMSS] Suporte aprimorado ao cache de disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))
* VM/VMSS: incorporar a lógica de validação de credenciais usada pelo portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))
* Adicionar comandos de espera e suporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))
* Conjunto de dimensionamento de máquinas virtuais: suporte à * para listar a exibição de instâncias em vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))
* Adicionar: segredos da VM e do conjunto de dimensionamento de máquinas virtuais ([2212}(https://github.com/Azure/azure-cli/pull/2212))
* Permitir a criação de VMs com VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))

## <a name="february-27-2017"></a>27 de fevereiro de 2017

Versão 2.0.0

Esta versão da CLI do Azure 2.0 é a primeira versão "Amplamente Disponível". A disponibilidade geral se aplica a estes módulos de comando:
- Serviço de Contêiner (acs)
- Computação (incluindo Gerenciador de Recursos, VM, conjunto de dimensionamento de máquinas virtuais, Managed Disks)
- Rede
- Armazenamento

Esses módulos de comando podem ser usados na produção e têm suporte do SLA padrão da Microsoft. Você pode abrir problemas diretamente com o suporte da Microsoft ou em nossa [lista de problemas do github](https://github.com/azure/azure-cli/issues/). Faça perguntas no [StackOverflow usando a marca azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contate a equipe de produto em [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) Forneça comentários na linha de comando com o comando `az feedback`

Os comandos nesses módulos são estáveis e a sintaxe não deve ser alterada em versões futuras dessa versão da CLI do Azure

Para verificar a versão da CLI, use `az --version` A saída lista a versão da CLI (2.0.0 nessa versão), os módulos de comando individuais, as versões do Python e GCC que você está usando

```text
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
> Alguns dos módulos de comando têm um sufixo "b*n*" ou "rc*n*". Esses módulos de comando ainda estão em versão prévia e estarão disponíveis no futuro

Também temos compilações de versão prévia noturnas da CLI. Para obter informações, consulte essas instruções sobre [como obter as compilações diárias](https://github.com/Azure/azure-cli#nightly-builds) e essas instruções sobre [configuração do desenvolvedor e código de contribuição](https://github.com/Azure/azure-cli#developer-setup)

Você pode relatar problemas com as compilações de visualização diárias das seguintes maneiras:
- Relatar problemas na [lista de problemas do github](https://github.com/azure/azure-cli/issues/)
- Entre em contato com a equipe do produto no endereço [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)
- Forneça comentários a partir da linha de comando com o comando `az feedback`

