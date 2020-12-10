---
title: Notas de versão da CLI do Azure
description: Saiba mais sobre as últimas atualizações da CLI do Azure
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 12/08/2020
ms.topic: article
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: bcbf52e6321e283864fb585cd314be22c2241c9d
ms.sourcegitcommit: 9beaf9abb794f1006a56acee4e1cfb8ea7fe2405
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2020
ms.locfileid: "96850296"
---
# <a name="azure-cli-release-notes"></a>Notas de versão da CLI do Azure

# <a name="current-release-notes"></a>[Notas sobre a versão atuais](#tab/azure-cli)

## <a name="december-08-2020"></a>08 de dezembro de 2020

Versão 2.16.0

### <a name="acr"></a>ACR

* Descrição da atualização do parâmetro KEK

### <a name="aks"></a>AKS

* `az aks nodepool add/update/upgrade`: executa o parâmetro de sobretensão máxima
* Adiciona suporte para o complemento AGIC
* Altera o cluster MSI para padrão

### <a name="apim"></a>APIM

* `az apim restore`: novo comando para restaurar um backup de um serviço de Gerenciamento de API

### <a name="app-service"></a>Serviço de Aplicativo

* Correção nº 14857: permite que os usuários atualizem a configuração do aplicativo Web mesmo com a restrição de acesso
* `az functionapp create`: aceita `--runtime python` e `--runtime-version 3.9` como um parâmetro do Azure Functions v3
* Correção nº 16041: az webapp config ssl create resulta em um erro desconhecido

### <a name="arm"></a>ARM

* `az deployment-scripts`: remove o sinalizador de visualização

### <a name="backup"></a>Backup

* Correção nº 14976: aprimoramentos de erro da CLI para os casos ValueError e AttributeError
* `az backup protection undelete`: adiciona suporte para restaurar a proteção do AzureWorkload usando a CLI
* Corrige um erro de solicitação incorreta para a entrada do tipo de carga de trabalho correta

### <a name="cdn"></a>CDN

* Adiciona o suporte de várias origens na versão prévia.
* Adiciona a rotação automática de BYOC.

### <a name="key-vault"></a>Key Vault

* `az keyvault key/secret list`: adiciona um parâmetro `--include-managed` para listar recursos gerenciados

### <a name="monitor"></a>Monitoramento

* `az monitor metrics alert create`: dá suporte a limites dinâmicos para o parâmetro de condição
* `az monitor metrics alert update`: dá suporte a limites dinâmicos para o parâmetro de condição
* `az monitor metrics alert dimension create`: cria uma dimensão de regra de alerta de métrica
* `az monitor metrics alert condition create`: cria uma condição de regra de alerta de métrica

### <a name="mysql"></a>MySQL

* Adiciona a CLI de atualização de versão do MySQL

### <a name="netappfiles"></a>NetAppFiles

* `az netappfiles account ad add`: dois parâmetros opcionais adicionados, aes_encryption e ldap_signing
* `az netappfiles account backup-policy update`: três parâmetros opcionais adicionados, chamados tags, type e id
* `az netappfiles snapshot policy create`: um parâmetro opcional adicionado, chamado provisioning_state

### <a name="network"></a>Rede

* `az network network watcher configure`: corrige o erro NetworkWatcherCountLimitReached causado pela diferenciação de maiúsculas e minúsculas do valor de localização
* `az network application-gateway http-listener`: corrige um bug em que não é possível criar e atualizar com o nome da política de WAF
* `az network route-table`: pretere a tabela de rotas V1
* `az network cross-region-lb`: suporte do balanceador de carga entre regiões
* `az network express-route port generate-loa`: novo comando para gerar e baixar a carta de autorização do PDF de um ExpressRoutePort

### <a name="packaging"></a>Empacotamento

* Adiciona o pacote Ubuntu Groovy

### <a name="rdbms"></a>RDBMS

* Adiciona um servidor show-connection-string, testa os comandos de contexto local e realiza a criação de servidor

### <a name="role"></a>Função

* Adiciona um aviso/resumo longo para comandos que geram credenciais

### <a name="search"></a>Pesquisar

* Adiciona uma opção de SKU

### <a name="service-fabric"></a>Service Fabric

* Atualiza documentos do aplicativo SF. Suporte apenas para recursos implantados do ARM

### <a name="synapse"></a>Synapse

* Dá suporte para cmdlets synapse sql dw e atualiza o cmdlet az synapse workspace create

## <a name="november-20-2020"></a>20 de novembro de 2020

Versão 2.15.1

### <a name="profile"></a>Perfil

* Hotfix: Correção nº 15961: az login: UnboundLocalError: variável local 'token_entry' referenciada antes da atribuição

## <a name="november-17-2020"></a>17 de novembro de 2020

Versão 2.15.0

### <a name="acs"></a>ACS

* Adição de avisos de substituição da v3

### <a name="aks"></a>AKS

* Adição de funcionalidade de sistema operacional efêmero
* Aprimoramento de engenharia: substituição das cadeias de caracteres de complemento por constantes
* `az aks install-cli`: suporte à personalização da URL de download
* `az aks browse`: apontamento para a exibição de recursos de Kubernetes do portal do Azure se k8s for maior ou igual a 1,19 ou kube-dashboard não estiver habilitado
* Suporte à identidade do painel de controle BYO
* `az aks use-dev-spaces`: indicação de que comandos dev-spaces foram preteridos

### <a name="ams"></a>AMS

* Alteração de "region" para "location" na cadeia de caracteres de saída: az ams account sp create

### <a name="app-config"></a>Configuração do Aplicativo

* Correção da inicialização do cliente do cofre de chaves

### <a name="app-service"></a>Serviço de Aplicativo

* Correção nº 13646: não é possível criar um Plano do Serviço de Aplicativo em um grupo de recursos diferente para o Ambiente do Serviço de Aplicativo
* Correções nº 11698 nº 15198 nº 14862 nº 15409: az webapp/functionapp config access-restriction add
* `az functionapp create`: adição de suporte à versão prévia do Node 14.
* `az functionapp create`: remoção do sinalizador da versão prévia de manipuladores personalizados.
* [ALTERAÇÃO DA FALHA] az functionapp update: a migração de um functionapp do plano Premium para o de Consumo agora requer o sinalizador '--force'.
* `az functionapp update`: adição de mensagem de erro se a migração do functionapp envolver planos no Linux.
* `az functionapp update`: adição de uma mensagem de erro mais descritiva se a migração de functionapp falhar.

### <a name="arm"></a>ARM

* Correção de um problema em que What-If mostrava dois escopos de grupo de recursos com usos diferentes de maiúsculas e minúsculas
* `az deployment`: impressão de detalhes do erro para implantação

### <a name="backup"></a>Backup

* Correção nº 14976: correção de KeyError e aprimoramento do texto de ajuda

### <a name="batch"></a>Lote

* Correção nº 15464: atualização da verificação de arquivo pfx sem senha no lote create_certificate

### <a name="billing"></a>Cobrança

* [ALTERAÇÃO DA FALHA] az billing invoice: remoção das propriedades BillingPeriodsNames e DownloadUrlExpiry da resposta.
* `az billing invoice`: suporte a muitos outros escopos, como BillingAccount, BillingProfile e assinatura existente.
* `az billing account`: novos comandos para dar suporte à exibição e à atualização de contas de cobrança existentes.
* `az billing balance`: novos comandos para dar suporte à exibição do saldo de um perfil de cobrança.
* `az billing customer`: novos comandos para dar suporte à exibição do cliente da conta de cobrança.
* `az billing policy`: novos comandos para dar suporte à exibição e atualização da política de um cliente ou de um perfil de cobrança.
* `az billing product`: novos comandos para gerenciar produtos de uma conta de cobrança.
* `az billing profile`: novos comandos para gerenciar um perfil de cobrança.
* `az billing property`: novos comandos para exibir e atualizar as propriedades de uma conta de cobrança.
* `az billing subscription`: novos comandos para gerenciar as assinaturas de uma conta de cobrança.
* `az billing transaction`: novos comandos para listar a transação de uma fatura.
* `az billing agreement`: novos comandos para gerenciar o contrato de cobrança.
* `az billing permission`: novos comandos para gerenciar a permissão de cobrança.
* `az billing role-assignment`: novos comandos para gerenciar a atribuição de função.
* `az billing role-definition`: novos comandos para exibir a definição de função.
* `az billing instruction`: novos comandos para gerenciar as instruções de cobrança.

### <a name="compute"></a>Computação

* Correção do problema de verificação de permissão de atualização
* Melhoria de vm list-skus table format
* vm host group create: --platform-fault-domain-count obrigatório e atualização da ajuda
* Suporte à atualização da versão de VM/imagem quando ela usa imagens entre locatários

### <a name="dps"></a>DPS

* Permissão para marcas no comando create do DPS em IoT

### <a name="hdinsight"></a>HDInsight

* az hdinsight create: adição de dois parâmetros `--resource-provider-connection` e `--enable-private-link` para dar suporte ao recurso de link privado e saída de retransmissão.

### <a name="key-vault"></a>Key Vault

* Refinamento de mensagens de erro para `list-deleted` e `purge` HSM
* Suporte à restauração de chave seletiva para HSMs gerenciados

### <a name="netappfiles"></a>NetAppFiles

* [ALTERAÇÃO DA FALHA] az netappfiles pool update: remoção do nível de serviço dos parâmetros.
* `az netappfiles pool update`: adição do parâmetro opcional qos-type.
* `az netappfiles pool create`: adição do parâmetro opcional qos-type.
* `az netappfiles volume replication suspend`: adição de force-break-replication como parâmetro opcional.
* Adição de az netappfiles volume replication re-initialize: o novo comando é adicionado para reinicializar a replicação.
* Adição de az netappfiles volume pool-change: novo comando para alterar o pool de um volume.
* Adição de az netappfiles snapshot policy: novo grupo de comandos com os comandos list, delete, update, show, create e volumes.
* Adição de az netappfiles account backup: novo grupo de comandos com os comandos show, list e delete
* Adição de az netappfiles volume backups: novo grupo de comandos com os comandos show, list, delete, update e create.
* Adição de az netappfiles account backup-policy: novo grupo de comandos com os comandos show, list, delete e update.
* Adição de az netappfiles vault list: um novo comando foi adicionado.
* `az netappfiles account ad add`: adição dos parâmetros opcionais kdc-ip, ad-name, server-root-ca-certificate e backup-operators
* `az netappfiles volumes create`: adição dos parâmetros opcionais snapshot-policy-id, backup-policy-id, backup-enabled, backup-id, policy-enforced, vault-id, kerberos-enabled, throughput-mibps, snapshot-directory-visible, security-style, kerberos5-read-only, kerberos5-read-write, kerberos5i-read-only, kerberos5i-read-write, kerberos5p-read-only, kerberos5p-read-write e has-root-access.
* `az netappfiles volume update`: adição dos parâmetros opcionais vault-id, backup-enabled, backup-policy-id, policy-enforced e throughput-mibps

### <a name="network"></a>Rede

* Correção do bug que não permitia a criação de um gateway de aplicativo Standard_v2 sem um endereço IP estático privado
* `az network dns zone import`: adição de FileOperationError em vez de FileNotFoundError se o arquivo de zona não existir
* Correção da falha de erro NoneType durante a exclusão de recursos não existentes de ApplicationGateway, LoadBalancer, Nic

### <a name="private-dns"></a>DNS privado

* `az network private-dns zone import`: adição de FileOperationError em vez de FileNotFoundError se o arquivo de zona não existir

### <a name="profile"></a>Perfil

* `az login`: nova adição do aviso de que um navegador está aberto

### <a name="role"></a>Função

* `az role assignment create`: `--description`, `--condition`, `--condition-version` em versão prévia

### <a name="security"></a>Segurança

* `az security pricing`: atualização da ajuda para refletir a versão atual da API que está sendo chamada

### <a name="storage"></a>Armazenamento

* Correção nº 15600: az storage fs existe: caso fs não exista, será retornado ResourceNotFoundError
* Correção nº 15706: os exemplos de storage container create estão incorretos
* `az storage blob delete-batch`: correção de um erro de digitação na documentação.

## <a name="november-09-2020"></a>9 de novembro de 2020

Versão 2.14.2

### <a name="app-service"></a>Serviço de Aplicativo

* Correção nº 15604, nº 15605: adicionar suporte ao Dotnet5

## <a name="november-06-2020"></a>6 de novembro de 2020

Versão 2.14.1

### <a name="arm"></a>ARM

* Hotfix: adicionar suporte de cadeia de caracteres com várias linhas do TS para entradas de modelo

## <a name="october-27-2020"></a>27 de outubro de 2020

Versão 2.14.0

### <a name="aks"></a>AKS

* Adição de suporte a PPG
* Atualização do tempo limite máximo Standard Load Balancer para 100 minutos

### <a name="apim"></a>APIM

* Correção de um problema com a criação da instância da camada de consumo

### <a name="app-config"></a>Configuração do Aplicativo

* Correção da consulta de pares chave-valor por rótulos separados por vírgula

### <a name="app-service"></a>Serviço de Aplicativo

* Correção de bug: falha no comando az webapp up quando o usuário não tem permissões de gravação no diretório pai do projeto
* Correção nº 13777: Correção para remover caracteres de escape do XML
* Correção nº 15441: falha no comando az webapp create-remote-connection com AttributeError: o objeto 'Thread' não tem nenhum atributo 'isAlive'
* [ALTERAÇÃO DA FALHA] az webapp up: adição de parâmetros opcionais (sistema operacional e runtime) e atualização de runtimes

### <a name="arm"></a>ARM

* Migração para GA de comandos What-If de implantação de modelo
* [ALTERAÇÃO DA FALHA] Adição da confirmação do usuário ao comando az ts create
* Correção dos dados retornados na marcação de vários recursos

### <a name="backup"></a>Backup

* `az backup policy create`: adição de suporte para criação da política de backup de IaaSVM por meio da CLI
* Aumento do limite de proteção da VM de 100 para 1.000

### <a name="compute"></a>Computação

* sig image-definition create: add --features
* Nova versão de API de gallery_images 2020-09-30
* `az vm update / az sig image-version update`: suporte à atualização da versão de VM/imagem mesmo quando ela usa uma imagem entre locatários
* Remoção da validação de SKUs de host de VM

### <a name="cosmos-db"></a>Cosmos DB

* `az cosmosdb create/update`: aprimoramento da mensagem de erro da entrada incorreta de --locations
* `az cosmosdb sql container create/update`: adição do parâmetro --analytical-storage-ttl

### <a name="hdinsight"></a>HDInsight

* [ALTERAÇÃO DA FALHA] az hdinsight create: remoção de dois parâmetros: --public-network-access-type e --outbound-public-network-access-type

### <a name="iot-central"></a>Central da IoT

* Remoção do aviso de versão prévia, pois ela já está em GA

### <a name="key-vault"></a>Key Vault

* Invalidação de `--enable-soft-delete false` na criação ou na atualização de cofres
* Alteração para que `--bypass` e `--default-action` trabalhem em conjunto com parâmetros da ACL de rede na criação de cofres

### <a name="misc"></a>Diversos.

* Adição de bash-completion a Dockerfile

### <a name="rdbms"></a>RDBMS

* Adição do comando list-SKUS, de transformadores de tabela e do contexto local para o Postgres, o MySQL e o MariaDB – Servidor Único
* [ALTERAÇÃO DA FALHA] Atualizações de nomes de parâmetros. Aprimoramentos no plano de gerenciamento para o MySQL e o PostgreSQL
* `az postgres|mariadb|mysql server create`: atualização da experiência de criação para o Postgres, o MySQL e o MariaDB: novos campos na saída e introdução de novos valores para o parâmetro `--public` no comando create (tudo, <IP>, <IPRange>, 0.0.0.0)

### <a name="signalr"></a>SignalR

* `az signalr create`: adição da nova opção `--enable-messaging-logs` para controlar o serviço na geração de logs de mensagens ou não
* `az signalr update`: adição da nova opção `--enable-messaging-logs` para controlar o serviço na geração de logs de mensagens ou não

### <a name="sql"></a>SQL

* [ALTERAÇÃO DA FALHA] Correção da resposta do nome de parâmetro de redundância do armazenamento de backup e do valor para a MI
* `az sql db audit-policy show`: extensão para mostrar a política de auditoria do banco de dados, incluindo os dados de LA e EH
* `az sql db audit-policy update`: extensão para permitir a atualização de LA e EH juntamente com a política de auditoria do banco de dados
* `az sql db audit-policy wait`: colocação da CLI em um estado de espera até que uma condição da política de auditoria do banco de dados seja atendida.
* `az sql server audit-policy show`: extensão para mostrar a política de auditoria do servidor, incluindo os dados de LA e EH
* `az sql server audit-policy update`: extensão para permitir a atualização de LA e EH juntamente com a política de auditoria do servidor
* `az sql server audit-policy wait`: colocação da CLI em um estado de espera até que uma condição da política de auditoria do servidor seja atendida.
* Adição de suporte somente ao AAD para Servidores e Instâncias Gerenciadas de SQL
* `az sql db replica create`: adição do argumento --partner-database

### <a name="storage"></a>Armazenamento

* Correção nº 15111: falha no comando `az storage logging update` sem argumento opcional
* Correção de bug no uso do comando set-tier com o logon da entidade de serviço
* Atualização da versão do data lake do arquivo para 2020-02-10
* `az storage queue list`: suporte a Track2
* `az storage fs access`: suporte ao gerenciamento de ACLs de maneira recursiva

### <a name="synapse"></a>Synapse

* adição de cmdlets relacionados a pipeline, serviço vinculado, gatilho, notebook, fluxo de dados e conjunto de dados

## <a name="october-13-2020"></a>13 de outubro de 2020

Versão 2.13.0

### <a name="acr"></a>ACR

* `az acr helm`: atualizar a URL de substituição
* Adicionar alterações de logtemplate e systemtask para Tarefas do ACR

### <a name="aks"></a>AKS

* Dar suporte ao nó virtual com o comando aks create: `az aks create --enable-addons virtual-node`
* Adicionar a única opção de imagem de nó para a CLI
* Esperar que o complemento kube-dashboard seja desabilitado por padrão
* `az aks create/update`: adicionar suporte ao LicenseType para o Windows
* Dar suporte para adicionar pools de nós spot
* Respeitar os nomes de complementos definidos na CLI do Azure

### <a name="ams"></a>AMS

* Correção nº 14687: o grupo de recursos e o nome da conta misturados no comando "az ams streaming-endpoint show"

### <a name="app-config"></a>Configuração do Aplicativo

* Corrigir o bug de teste
* Dar suporte à autenticação do AAD para operações de dados

### <a name="app-service"></a>Serviço de Aplicativo

* `az functionapp deployment source config-zip`: correção de um problema em que o config-zip poderia gerar uma exceção em caso de sucesso no consumo em Linux
* Bugfix: mensagens de erro aprimoradas para comandos webapp
* `az appservice domain create, show-terms`: adicionar a capacidade de criar um domínio do serviço de aplicativo
* `az functionapp create`: o sinalizador de visualização do Java 11 foi removido durante a criação de um aplicativo de funções
* [ALTERAÇÃO DA FALHA] az webapp create e az webapp up – Atualizar runtimes de webapp disponíveis

### <a name="arm"></a>ARM

* `az ts`: adicionar novos comandos para especificações de modelo
* `az deployment`: adicionar suporte para --template-spec -s

### <a name="compute"></a>Computação

* Corrigir a limitação de contagem FD de criação de grupos de hosts
* Adicionar um novo comando para dar suporte à atualização de extensões para VMSS
* Não há problemas na correção da referência da imagem

### <a name="hdinsight"></a>HDInsight

* `az hdinsight create`: adicionar informações preteridas para os argumentos --public-networrk-access-type e --outbound-public-network-access-type
* `az hdinsight create`: adicionar informações preteridas para os argumentos `--public-networrk-access-type` e `--outbound-public-network-access-type`
* `az hdinsight create`: adicionar o parâmetro `--idbroker` para dar suporte ao cliente a fim de criar um cluster ESP com o Agente de IDs do HDInsight

### <a name="iot-central"></a>Central da IoT

* Remover o módulo de comando 'az iotcentral' preterido

### <a name="key-vault"></a>Key Vault

* Dar suporte à `--hsm-name` para `az keyvault key encrypt/decrypt`

### <a name="lab"></a>Laboratório

* Correção nº 14127: `__init__()` precisa de um argumento posicional, porém dois foram fornecidos

### <a name="network"></a>Rede

* `az network application-gateway ssl-cert show`: adicionar um exemplo para demonstrar o formato do certificado e buscar informações
* `az network application-gateway rule`: dar suporte a --priority option
* `az network application-gateway create`: corrigir um bug que não pode ser criado sem um IP especificado
* `az network application-gateway waf-policy managed-rule rule-set add`: expor o erro do servidor ao usuário para fornecer uma mensagem de dica mais intuitiva.
* `az network application-gateway waf-policy managed-rule rule-set update`: dar suporte para alterar a versão do tipo de conjunto de regras.

### <a name="rdbms"></a>RDBMS

* Bugfix: az postgres flexible-server create. Remover a versão de API codificada do cliente de rede.

### <a name="role"></a>Função

* Correção nº 15278: `az role assignment list/delete`: proibir argumentos de cadeias de caracteres vazias

### <a name="sql"></a>SQL

* `az sql midb log-replay`: dar suporte para serviços de reprodução de log em um banco de dados gerenciado
* Ignorar a formatação de maiúsculas/minúsculas dos caracteres para o valor de parâmetro de redundância de armazenamento de backup para uma instância gerenciada
* [ALTERAÇÃO DA FALHA] az sql db create: adicionar o parâmetro --backup-storage-redundancy. Adicionar um aviso para o bsr/bsr == Geo não especificado.

### <a name="sql-vm"></a>SQL VM

* `az sql vm show`: adicionar opções de configuração ao sinalizador --expand

### <a name="storage"></a>Armazenamento

* [ALTERAÇÃO DA FALHA] `az storage blob copy start`: corrigir o problema de formato para `--destination-if-modified-since` e `--destination-if-unmodified-since`
* [ALTERAÇÃO DA FALHA] `az storage blob incremental-copy start`: corrigir o problema de formato para `--destination-if-modified-since` e `--destination-if-unmodified-since`
* `az storage fs`: corrigir um problema de cadeia de conexão
* `az storage share-rm`: camada de acesso da versão de GA
* `az storage container-rm`: adicionar um novo grupo de comandos com o objetivo de usar o provedor de recursos Microsoft.Storage para operações de gerenciamento de contêineres.

## <a name="september-29-2020"></a>29 de setembro de 2020

Versão 2.12.1

### <a name="rdbms"></a>RDBMS

* Hotfix: `az postgres flexible-server create`: Atualizar o VnetName para excluir o nome do servidor e atualizar a região padrão para MySQL

## <a name="september-22-2020"></a>22 de setembro de 2020

Versão 2.12.0

### <a name="acr"></a>ACR

* Correção nº 14811: adicionar suporte para substituição dockerignore

### <a name="aks"></a>AKS

* A CLI deve tolerar kubeconfig vazio
* CORREÇÃO nº 12871: az aks enable-addons: o exemplo de ajuda gerada automaticamente está errado para a opção virtual-node
* Remover ações do conector do aci herdado
* Dar suporte ao complemento do Azure Policy em azure-cli
* Corrigir o problema de diferenciação de maiúsculas e minúsculas do complemento do painel do AKS
* Atualizar mgmt-containerservice para a versão 9.4.0 e habilitar a API 09-01

### <a name="apim"></a>APIM

* Dar suporte aos comandos de entidade product/productapi/namedValue e a versão do SDK bump &&

### <a name="app-config"></a>Configuração do Aplicativo

* Dar suporte para habilitar/desabilitar PublicNetworkAccess para armazenamentos existentes

### <a name="app-service"></a>Serviço de Aplicativo

* Adicionar suporte para o tipo de preço Premium V3
* Correção nº12653: az webapp log config --application-logging false não o desativa
* Correção nº 14684: a remoção de access-restriction por endereço IP não funcionava; nº 13837-az webapp create – Exemplo para diferentes RSgroups para Plan e WebApp
* functionapp: Adicionar suporte para manipuladores personalizados. PowerShell 6.2 preterido.
* functionapp: Correção do problema em que a configuração do aplicativo estava sendo definida incorretamente para imagens personalizadas do Linux

### <a name="arm"></a>ARM

* `az deployment group/sub/mg/tenant what-if`: Mostrar alterações de recurso "Ignorar" por último

### <a name="compute"></a>Computação

* Adicionar novo license_type na criação/atualização de VM: RHEL_BYOS, SLES_BYOS
* Atualizar a API do disco para a versão 2020-06-30
* criação do disco: add --logical-sector-size, --tier
* atualização do disco: Suporte a --disk-iops-read-only, --disk-mbps-read-only, --max-shares
* Novo comando disk-encryption-set list-associated-resources
* Habilitação de vm boot-diagnostics: --storage se torna opcional
* Novo comando: vm boot-diagnostics get-boot-log-uris
* vm boot-diagnostics get-boot-log: suporte ao armazenamento gerenciado

### <a name="config"></a>Config

* Renomear local-context para configurar param-persist

### <a name="cosmos-db"></a>Cosmos DB

* Dar suporte a APIs de Migração para o recurso de taxa de transferência para o recurso de dimensionamento automático no CosmosDB

### <a name="eventhub"></a>Eventhub

Adição de comandos de cluster e do parâmetro trusted_service_access_enabled para Networkruleset

### <a name="extension"></a>Extensão

* `az extension add`: adicionar a opção `--upgrade` para atualizar a extensão, se ela já estiver instalada
* Ativar a instalação dinâmica por padrão

### <a name="iot"></a>IoT

* Versão mínima do TLS habilitada na criação do Hub IoT

### <a name="iot-central"></a>IoT Central

* A operação de exclusão de aplicativo agora é uma operação de execução prolongada

### <a name="iot-hub"></a>Hub IoT

* Comando 'show-connection-string' preterido

### <a name="key-vault"></a>Key Vault

* Versão prévia pública do HSM gerenciado
* Corrigir o problema em que `--maxresults` não entrou em vigor durante a listagem de recursos ou versões de recursos

### <a name="kusto"></a>Kusto

* Adicionar mensagem de substituição

### <a name="monitor"></a>Monitoramento

* `az monitor log-analytics workspace linked-storage`: expor a mensagem de erro detalhada aos clientes

### <a name="network"></a>Rede

* `az network vnet subnet`: dar suporte a --disable-private-endpoint-network-policies e --disable-private-link-service-network-policies
* Corrigir o bug durante a atualização do log de fluxos quando a subpropriedade network_watcher_flow_analytics_configuration for None
* Elevação da API para a versão 2020-06-01
* Dar suporte --tcp-port-behavior durante a definição da configuração do TCP de um Monitor da Conexão V2
* Dar suporte a mais tipos e ao nível de cobertura durante a criação do ponto de extremidade do Monitor da Conexão v2
* Dar suporte a --host-subnet para criar o VirtualHub abaixo como VirtualRouter

### <a name="rdbms"></a>RDBMS

* Atualizações do Plano de Gerenciamento para PostgreSQL e MySQL

### <a name="role"></a>Função

* `az role assignment create/update`: dar suporte a `--description`, `--condition` e `--condition-version`
* `az ad app permission delete`: dar suporte a `--api-permissions` para excluir o `ResourceAccess` específico

### <a name="service-fabric"></a>Service Fabric

* Adicionar comandos de tipo de nó e cluster gerenciado

### <a name="sql"></a>SQL

* Atualizar azure-mgmt-sql para 0.20.0
* Adicionar parâmetro opcional de redundância de armazenamento de backup ao cmdlet MI create

### <a name="storage"></a>Armazenamento

* `az storage share-rm stats`: obter os bytes de uso dos dados armazenados no compartilhamento.
* PITR de blob de armazenamento de versão GA
* `az storage blob query`: dar suporte à Aceleração de Consulta do Armazenamento do Azure
* Dar suporte à exclusão reversível para o compartilhamento de arquivo
* `az storage copy`: adicionar suporte a credenciais de conta e substituir `--source-local-path`, `--destination-local-path`, `--destination-account-name`
* `az storage account blob-service-properties update`: adicionar suporte à política de retenção de exclusão de contêiner

### <a name="synapse"></a>Synapse

* Correção de erro de digitação no exemplo de criação e exclusão de atribuição de função do az synapse

## <a name="august-28-2020"></a>28 de agosto de 2020

Versão 2.11.1

### <a name="acr"></a>ACR

* Adição de camada isolada ao pool de agentes
* Adição de contexto de origem do artefato de OCI

### <a name="aks"></a>AKS

* Correção de um problema de criação do cluster do AKS

### <a name="cognitive-services"></a>Serviços Cognitivos

* [ALTERAÇÃO DA FALHA] Mostrar um termo legal adicional para determinadas APIs

### <a name="network"></a>Rede

* [ALTERAÇÃO DA FALHA] Permitir a criação de IP público e IP privado ao criar um Gateway de Aplicativo
* `az network list-service-tags`: adição de detalhes sobre o uso de parâmetro de localização para a mensagem de ajuda

### <a name="storage"></a>Armazenamento

* `az storage blob list`: suporte OU propriedades com a nova versão de API

## <a name="august-25-2020"></a>25 de agosto de 2020

Versão 2.11.0

### <a name="aks"></a>AKS

* Remoção da marca de visualização do complemento de Nó Virtual
* Adição do argumento CMK do AKS na criação do cluster
* Definição do perfil de rede durante o uso do balanceador de carga básico.
* Remoção da validação máxima de pods da CLI e permissão para que a simulação lide com ela
* Correção de complementos disponíveis na mensagem de ajuda em `az aks create`
* Introdução de suporte para o perfil de dimensionamento automático do cluster na CLI principal

### <a name="appservice"></a>AppService

* `az webapp`: adição do comando list-instances
* `az webapp ssh`: adição do parâmetro --instance para se conectar a uma instância específica
* `az webapp create-remote-connection`: adição do parâmetro --instance para se conectar a uma instância específica
* Correção nº 14758: erros de az webapp create durante a criação de um aplicativo do Windows com --runtime dotnetcore
* Correção nº 14701: implementação de functionapp create --assign-identity
* Correção nº 11244: `az webapp auth update`: adição do parâmetro opcional para atualizar client-secret-certificate-thumbprint
* `az functionapp keys`: comandos adicionados que permitem aos usuários gerenciar as chaves do aplicativo de funções
* `az functionapp function`: comandos adicionados que permitem aos usuários gerenciar as funções individuais
* `az functionapp function keys`: comandos adicionados que permitem aos usuários gerenciar as chaves de função
* Correção nº14788: az webapp create não obtém o webapp correto quando os nomes são substrings
* `az functionapp create`: capacidade removida para criar funções 2.x em regiões que não têm compatibilidade

### <a name="arm"></a>ARM

* `az resource list`: extensão dos dados retornados de `createdTime`, `changedTime` e `provisioningState`
* `az resource`: adição do parâmetro `--latest-include-preview` para dar suporte ao uso da api-version mais recente se ela for versão prévia

### <a name="aro"></a>ARO

* Aprimoramentos da CLI, incluindo permissões de verificação da tabela de rotas

### <a name="cloud"></a>Nuvem

* `az cloud register`: correção do registro de nuvens com um arquivo de configuração

### <a name="compute"></a>Computação

* Atualização de SKUs de VM compatíveis com rede acelerada
* `az vm create`: aplicação automática de patches no convidado
* `az image builder create`: adição de --vm-size, --os-disk-size, --vnet, --subnet
* Novo comando az vm assess-patches

### <a name="container"></a>Contêiner

* Correção nº 6235: atualização do texto de ajuda para o parâmetro de portas na criação do contêiner

### <a name="datalake-store"></a>Datalake Store

* Correção do problema nº 14545 para a operação de ingresso no data lake

### <a name="eventhub"></a>EventHub

* `az eventhubs eventhub create/update`: alterar a documentação de destination_name

### <a name="extension"></a>Extensão

* Adição do comando `az extension list-versions` para listar todas as versões disponíveis de uma extensão

### <a name="hdinsight"></a>HDInsight

* Suporte à criação de cluster com configuração de dimensionamento automático e suporte ao gerenciamento de configuração de dimensionamento automático
* Suporte à criação de cluster com criptografia no host

### <a name="iotcentral"></a>IoT Central

* Aprimoramentos na documentação da CLI

### <a name="monitor"></a>Monitor

* `az monitor metrics alert create`: suporte a RG e Sub como os valores de escopo

### <a name="netappfiles"></a>NetAppFiles

* [ALTERAÇÃO DA FALHA] az netappfiles snapshot create: file-system-id removido dos parâmetros
* [ALTERAÇÃO DA FALHA] az netappfiles snapshot show: o instantâneo não tem mais o parâmetro file-system-id
* `az netappfiles account`: Model ActiveDirectory tem um novo parâmetro backup_operators
* `az netappfiles volume show`: Model dataProtection tem um novo parâmetro snapshot
* `az netappfiles volume show`: Model Volume tem um novo parâmetro snapshot_directory_visible

### <a name="network"></a>Rede

* `az network dns export`: exportação do FQDN para o tipo MX, PTR, NS e SRV em vez do caminho relativo
* Suporte ao link privado para discos gerenciados
* `az network application-gateway auth-cert show`: adição de exemplo para demonstrar o formato do certificado
* `az network private-endpoint-connection`: suporte à configuração de aplicativos

### <a name="rbac"></a>RBAC

* `az ad group create`: suporte à especificação da descrição durante a criação de um grupo
* `az role definition create`: impressão de mensagem legível em vez de exceção quando assignableScope for uma matriz vazia
* [ALTERAÇÃO DA FALHA] `az ad sp create-for-rbac`: alteração da permissão padrão do certificado criado

### <a name="sql"></a>SQL

* `az sql server audit-policy`: adição de suporte à auditoria do SQL Server

### <a name="storage"></a>Armazenamento

* `az storage blob copy start-batch`: correção nº 6018 para --source-sas
* `az storage account or-policy`: suporte à política de replicação de objeto de conta de armazenamento
* Correção do problema nº 14083 para atualizar a versão do pacote do azure-multiapi-storage para o problema do pacote e suporte da versão à nova API
* `az storage blob generate-sas`: adição de exemplos para --ip e refinamento da mensagem de erro
* `az storage blob list`: correção do problema de next_marker

### <a name="synapse"></a>Synapse

* Adição de cmdlets relacionados a workspace, sparkpool e sqlpool
* Adição de comandos relacionados a spark job com base no track2 sdk
* Adição de comandos relacionados ao recurso accesscontrol com base no track2 sdk

### <a name="upgrade"></a>Atualizar

* Adição do comando `az upgrade` para atualizar a CLI do Azure e as extensões

## <a name="august-11-2020"></a>11 de agosto de 2020

Versão 2.10.1

### <a name="app-service"></a>Serviço de Aplicativo

* Correção nº 9887 webapp e functionapp, dar suporte à atribuição/remoção de identidade gerenciada pelo usuário
* Correção nº 1382, 14055: atualizar mensagens de erro para az webapp create e az webapp config container set
* `az webapp up`: corrigir a lógica de seleção padrão do ASP quando o parâmetro --plan não é fornecido

### <a name="appconfig"></a>AppConfig

* Dar suporte para habilitar/desabilitar PublicNetworkAccess durante a criação da loja

### <a name="compute"></a>Computação

* Dar suporte à associação de disco e instantâneo com um recurso de acesso a disco

### <a name="lab"></a>Laboratório

* Correção do problema nº 7904: bug de validação de data na criação de VM do laboratório

### <a name="storage"></a>Armazenamento

* `az storage blob upload-batch`: correção do problema nº 14660 com argumentos não posicionais

## <a name="august-04-2020"></a>04 de agosto de 2020

Versão 2.10.0

### <a name="aks"></a>AKS

* `az aks update`: Alteração do argumento --enable-aad para migrar um cluster não AAD habilitado para RBAC para um cluster AAD gerenciado por AKS
* `az aks install-cli`: Adição de argumentos --kubelogin-version e --kubelogin-install-location para instalar o kubelogin
* Adição do comando az aks nodepool get-upgrades

### <a name="ams"></a>AMS

* Correção nº 14021: az ams account sp não é idempotente

### <a name="apim"></a>APIM

* importação da API de APIM: suporte à importação de API e aprimoramento de outros comandos da CLI de nível da API

### <a name="app-service"></a>Serviço de Aplicativo

* Correção nº 13035: Adição de validação para az webapp config access-restriction para evitar a adição de duplicatas

### <a name="appconfig"></a>AppConfig

* Adoção de SKU padrão se não for especificado
* [ALTERAÇÃO SIGNIFICATIVA] Configurações de suporte com tipo de conteúdo JSON

### <a name="arm"></a>ARM

* `az resource tag`: Correção do bug de marcação managedApp e alguns problemas de teste relacionados
* `az deployment mg/tenant what-if`: Adição de suporte ao grupo de gerenciamento e à implantação de nível de locatário What-If
* `az deployment mg/tenant create`: Adição do parâmetro --confirm-with-what-if/-c.
* `az deployment mg/tenant create`: Adição do parâmetro --what-if-result-format/-r.
* `az deployment mg/tenant create`: adicionar parâmetro --what-if-exclude-change-types/-x.
* `az tag`: az tag support para parâmetro ID de recurso

### <a name="backup"></a>Backup

* Disparar a descoberta de contêiner/item AFS somente quando necessário

### <a name="cdn"></a>CDN

* Adicionar campos de link privado à origem

### <a name="compute"></a>Computação

* `az vm/vmss create`: Selecione um nome de usuário válido para usuário se o nome de usuário padrão for inválido
* `az vm update`: suporte à imagem entre locatários
* `az disk-access`: Adicionar novo grupo de comandos para operar o recurso de acesso ao disco
* Suporte ao posicionamento automático do grupo de hosts dedicado
* Suporte a PPG e SPG no modo de orquestração de VMSS

### <a name="config"></a>Config

* `az config`: Adição do novo módulo de comando `config`

### <a name="extension"></a>Extensão

* Suporte à instalação automática de uma extensão se a extensão de um comando não estiver instalada

### <a name="hdinsight"></a>HDInsight

* Adição de três parâmetros ao comando `az hdinsight create` para compatibilidade com o link privado e o recurso de criptografia em trânsito:

### <a name="iot-hub"></a>Hub IoT

* Correção nº 7792: A criação do Hub IoT não é idempotente

### <a name="iot-central"></a>Central da IoT

* Adição de lista de opções de parâmetros para IoT Central

### <a name="keyvault"></a>KeyVault

* `az keyvault key encrypt/decrypt`: adição de parâmetro `--data-type` para especificar explicitamente o tipo de dado original

### <a name="monitor"></a>Monitoramento

* `az monitor log-analytics workspace data-export`: suporte ao namespace do hub de eventos como o destino.
* `az monitor autoscale`: suporte a namespace e dimensões para --condition

### <a name="netappfiles"></a>NetAppFiles

* `az volume revert`:  Adição de Reversão de Volume para reverter um volume para um de seus instantâneos.
* [ALTERAÇÃO SIGNIFICATIVA] Remoção de `az netappfiles mount-target`.
* `az volume show`: Adição de site para Propriedades do Active Directory

### <a name="network"></a>Rede

* `az application-gateway private-link add`: suporte para especificar uma sub-rede existente por ID
* `az network application-gateway waf-policy create`: versão e tipo de suporte

### <a name="storage"></a>Armazenamento

* Correção nº 10302: Suporte à estimativa de tipo de conteúdo ao sincronizar arquivos
* `az storage blob lease`: Aplicação de nova versão de API para operações de concessão de blob
* `az storage fs access`: Suporte a credencial do AAD no gerenciamento de controle de acesso para conta do ADLS Gen2
* `az storage share-rm create/update`: adição de --access-tier para dar suporte à camada de acesso

## <a name="july-16-2020"></a>16 de julho de 2020

Versão 2.9.1

### <a name="aks"></a>AKS

* Remove a configuração explícita de VMSS no comando de exemplo do Windows, pois ele agora é padrão

### <a name="iot"></a>IoT

* [ALTERAÇÃO DA FALHA] `az iot pnp`: Remove comandos de versão prévia do IoT PNP da CLI principal

### <a name="rest"></a>REST

* Correção nº14152: `az rest`: aceita URLs do ARM sem a ID de assinatura

### <a name="storage"></a>Armazenamento

* Correção nº 14138: torna algumas permissões opcionais

## <a name="july-14-2020"></a>14 de julho de 2020

Versão 2.9.0

### <a name="acr"></a>ACR

* Manipular o link do artefato de log do Registro para os logs de fluxo
* Substituir comandos helm2

### <a name="aks"></a>AKS

* `az aks create`: adiciona o argumento --enable-aad
* `az aks update`: adiciona o argumento --enable-aad

### <a name="apim"></a>APIM

* Comandos az apim api gerais adicionados

### <a name="appconfig"></a>AppConfig

* Adicionar exemplo para usar --fields na revisão do appconfig

### <a name="appservice"></a>AppService

* `az functionapp create`: Suporte para Java 11 e PowerShell 7 adicionado. Suporte à API de pilhas adicionado.
* Correção nº 14208 falha na criação de um aplicativo com vários contêineres
* Corrige az webapp create – usa pilhas de runtime embutidas em código

### <a name="arm"></a>ARM

* `az resource tag`: corrige o problema de marcar recursos com o tipo de recurso `Microsoft.ContainerInstance/containerGroups`

### <a name="compute"></a>Computação

* Avançar os discos de versão 2020-05-01, computação 2020-06-01
* Criptografia dupla do conjunto de criptografia de disco
* `az vmss update`: dá suporte à especificação de imagem entre locatários.
* `az sig image-version create`: dá suporte à especificação de imagem entre locatários.
* vm/vmss create: Criptografia de cache e dados em trânsito para discos do sistema operacional/de dados e discos temporários para VM e VMSS
* Adicionar operação de remoção simulada para VM e VMSS

### <a name="cosmosdb"></a>CosmosDB

* Recursos recentes: Autoscale, IpRules, EnableFreeTier e EnableAnalyticalStorage

### <a name="eventgrid"></a>EventGrid

* Adicionar suporte de CLI para 2020-04-01-preview e marcar a versão prévia dos recursos com is_Preview=True

### <a name="find"></a>Localizar

* Correção nº 14094 az find Corrige consultas que falhavam quando não estavam conectadas e quando a telemetria estava desabilitada

### <a name="hdinsight"></a>HDInsight

* Adicionar dois comandos para dar suporte ao recurso de reinicialização do nó do hdinsight

### <a name="monitor"></a>Monitoramento

* Remover sinalizador de visualização para comandos no workspace do Log Analytics
* `az monitor diagnostic-settings subscription`: Dar suporte às configurações de diagnóstico para a assinatura
* `az monitor metrics`: dá suporte para ', ' e '|' no nome da métrica
* `az monitor log-analytics workspace data-export`: suporte à exportação de dados do Log Analytics

### <a name="network"></a>Rede

* `az network application-gateway frontend-ip update`: Substituir o parâmetro --public-ip-address
* Avançar azure-mgmt-network para 11.0.0
* `az network express-route gateway connection`: dá suporte à configuração de roteamento
* `az network virtual-appliance`: dá suporte à solução de virtualização de rede do Azure.
* Recurso de link privado de suporte do Gateway de Aplicativo

### <a name="policyinsights"></a>PolicyInsights

* `az policy state`: adiciona o comando trigger-scan para disparar avaliações de conformidade de política
* `az policy state list`: expõe versões de entidades de política em cada registro de conformidade

### <a name="profile"></a>Perfil

* `az account get-access-token`: Mostra expiresOn para Identidade Gerenciada

### <a name="rdbms"></a>RDBMS

* Dar suporte à versão mínima do TLS
* Adicionar criptografia de infraestrutura para o Azure Postgres e MySQL

### <a name="security"></a>Segurança

* Adicionar comandos allowed_connections
* Adicionar comandos hardeningss da rede adaptável
* Adicionar comandos adaptive_application_controls
* Adição de az security iot-solution/ iot-alerts/iot-recommendations/iot-analytics REST à CLI do Azure
* Adicionar CLI de conformidade regulatória

### <a name="signalr"></a>SignalR

* Adicionar recursos, incluindo o gerenciamento de conexões de ponto de extremidade privado, regras de rede e upstream

### <a name="sql"></a>SQL

* `az sql mi create`, `az sql mi update`: adiciona o parâmetro `--tags` para dar suporte à marcação de recursos
* `az sql mi failover`: dá suporte ao failover de um ponto primário ou secundário

### <a name="storage"></a>Armazenamento

* `az storage account create/update`: adiciona --allow-blob-public-access para permitir ou não permitir acesso público para blob e contêineres
* `az storage account create/update`: adiciona `--min-tls-version` para dar suporte à definição da versão mínima do TLS a ser permitida em solicitações de armazenamento.
* Remover credencial de token de check-in
* Corrigir o nome da conta de armazenamento em exemplos

### <a name="webapp"></a>Webapp

* Bugfix: az webapp log deployment show – retorna logs de implantação em vez de metadados de log
* Bugfix: az webapp vnet-integration add – corrige o tratamento de erro se o nome da VNet é inadequado, dá suporte à ID do recurso da vnet

## <a name="june-23-2020"></a>23 de junho de 2020

Versão 2.8.0

### <a name="acr"></a>ACR

* Adicionar suporte para desabilitar roteamento/ponto de extremidade da região
* [ALTERAÇÃO DA FALHA] `az acr login --expose-token` não aceita nome de usuário e senha

### <a name="acs"></a>ACS

* Remover o cluster privado e a API 2019-10-27-preview

### <a name="aks"></a>AKS

* Suporte a --yes para az aks upgrade
* Reverter "alteração da sku de vm padrão para Standard_D2s_v3 (#13541)"
* Adicionar "az aks update --uptime-sla"
* Corrigir erro de digitação no comando az aks update
* Alteração para dar suporte ao pool de agentes do nó 0 e bloquear a escala manual do pool habilitado para CAS
* Corrigir erro de digitação em VirtualMachineScaleSets e atualizar referências a versões do Kubernetes

### <a name="ams"></a>AMS

* ALTERAR o texto da ajuda do parâmetro "--expiry".

### <a name="appservice"></a>AppService

* `az webapp log deployment show`: mostrar o log de implantação mais recente ou os logs de uma implantação específica se a ID da implantação for especificada
* `az webapp log deployment list`: lista de logs de implantação disponíveis
* Correção: erro de superfície quando um nome de webapp inválido é fornecido
* Correção #13261: az webapp list-runtimes usa a lista estática até que a nova API de Pilhas Disponíveis esteja disponível
* `az appservice ase create`: correção na criação do problema #13361
* `az appservice ase list-addresses`: correção na alteração do SDK #13140.
* Correção da criação de webapp/slot para Contêineres do Windows
* `az webapp auth update`: adicionar parâmetro opcional para atualizar a versão do runtime
* Suporte para listar, excluir, aprovar e rejeitar conexão de ponto de extremidade privado para webapp na CLI
* Correção #13888: adicionar suporte para WebApps Estáticos: comandos get, list, create
* Mensagens de erro aprimoradas para Conexão de Túnel SSH

### <a name="arm"></a>ARM

* `az tag`: adicionar exemplos para -h
* `az deployment group/sub what-if`: adicionar parâmetro --exclude-change-types/-x.
* `az deployment group/sub/mg/tenant create`: adicionar parâmetro --what-if-exclude-change-types/-x.
* `az deployment group/sub/mg/tenant validate`: mostrar mensagens de erro em um formato melhor.
* `az group export`: adicionar novos parâmetros `--skip-resource-name-params` e `--skip-all-params` para dar suporte para ignorar parametrização
* Adicionar az feature unregister api

### <a name="aro"></a>ARO

* Adicionar Public e Private aos parâmetros para obter ajuda com a visibilidade de entrada/apiserver

### <a name="batch"></a>Lote

* `az batch account create`: adicionar novo parâmetro `--public-network-access`
* `az batch account create`: adicionar novo parâmetro `--identity-type`
* `az batch account set`: adicionar novo parâmetro `--identity-type`
* [ALTERAÇÃO SIGNIFICATIVA] az batch pool create: ao criar um pool usando uma imagem personalizada, a propriedade --image agora pode se referir apenas a uma imagem da Galeria de Imagens Compartilhadas.
* [ALTERAÇÃO SIGNIFICATIVA] az batch pool create: ao criar um pool com a opção --json-file e especificar uma networkConfiguration, a propriedade publicIPs foi movida para uma nova propriedade publicIPAddressConfiguration. Essa nova propriedade também dá suporte a uma nova propriedade ipAddressProvisioningType, que especifica como o pool deve alocar os IPs, e a uma propriedade publicIPs, que permite a configuração de uma lista de recursos de PublicIP a serem usados caso ipAddressProvisioningType seja definido como UserManaged
* `az network private-link-resource`: adicionar suporte para o recurso Microsoft.Batch batchAccount
* `az network private-endpoint-connection`: adicionar suporte para o recurso Microsoft.Batch batchAccount

### <a name="cdn"></a>CDN

* `az cdn custom-domain enable-https`: adicionar suporte para BYOC.
* `az cdn custom-domain enable-https`: corrigir a habilitação de HTTPS personalizado com certificados gerenciados da CDN para os SKUs Standard_Verizon e Standard_Microsoft.

### <a name="cognitive-services"></a>Serviços Cognitivos

* [ALTERAÇÃO DA FALHA] `az cognitiveservices account` agora, há uma estrutura unificada para todos os comandos.
* `az cognitiveservices account identity`: adicionar gerenciamento de identidades para os Serviços Cognitivos.

### <a name="compute"></a>Computação

* `az image builder`: atualização da versão da API para 2020-02-14
* `az image builder create`: adicionar `--identity` para dar suporte à configuração de identidade
* `az image builder customizer add`: suporte para o personalizador de atualização do Windows
* Novo comando `az image builder cancel`
* Mostrar um aviso quando um usuário implanta um VMSS fixado a uma versão de uma imagem específica em vez da mais recente

### <a name="cosmos-db"></a>Cosmos DB

* `az cosmosdb`: adicionar o comando exists ao banco de dados e aos grupos de contêineres
* Permitir a criação de coleções fixas

### <a name="eventhub"></a>EventHub

* `az eventhubs namespace create`: adicionar parâmetros de identidade gerenciada

### <a name="extension"></a>Extensão

* Adicionar --version para dar suporte à instalação de uma versão específica
* Habilitar as extensões da CLI a incluírem pacotes no namespace 'azure'

### <a name="iot-hub"></a>Hub IoT

* [ALTERAÇÃO SIGNIFICATIVA] az iot hub job: remover comandos de trabalho preteridos

### <a name="keyvault"></a>KeyVault

* `az keyvault key import`: dá suporte à importação de cadeias de caracteres por meio de dois novos parâmetros.
* Suporte à criptografia e descriptografia de cadeias de caracteres/bytes com chaves armazenadas

### <a name="monitor"></a>Monitoramento

* Suporte para não aguardar a criação do cluster
* `az monitor log-analytics workspace saved-search`: suporte para novos comandos para a pesquisa salva

### <a name="network"></a>Rede

* `az network application-gateway address-pool update`: refinar a mensagem de ajuda e adicionar exemplos.
* `az network vnet create`: suporte para o argumento --nsg
* `az network lb address-pool`: suporte para criar o pool de back-end de lb com endereço de back-end.
* `az network application-gateway address-pool`: correção para o argumento --add

### <a name="rbac"></a>RBAC

* `az ad sp create-for-rabc`: suporte para nome com espaço, barra e barra invertida
* `az ad sp create-for-rbac`: refinar mensagem de erro quando o usuário especifica um escopo inválido

### <a name="security"></a>Segurança

* Adicionar comandos de avaliação de segurança

### <a name="sql"></a>SQL

* `az sql db ltr-policy/ltr-backup`: atualizar/mostrar política de retenção de longo prazo, mostrar/excluir backups de retenção de longo prazo, restaurar backup de retenção de longo prazo

### <a name="storage"></a>Armazenamento

* Corrigir problema de autenticação para dar suporte a get token para --subscription
* `az storage remove`: correção do problema #13459 para gerar exceção para a falha da operação
* Correção dos problemas #13012, #13632 e #13657 para remover argumentos não utilizados para comandos relacionados à geração de SAS
* `az storage logging update`: adicionar verificação da versão de log
* `az storage blob show`: adicionar mais propriedades para o blob com o SDK da faixa 2
* Correção #13708: refinar a mensagem de aviso para a credencial
* `az storage share-rm create/update`: adicionar suporte para protocolo NFS e squash raiz
* `az storage account create`: adicionar suporte para criptografia dupla
* [ALTERAÇÃO DA FALHA] `az storage blob/container/file/share/table/queue generate-sas`: tornar --expiry e --permissions obrigatórios
* `az storage blob set-tier`: migrar para a Faixa 2 para dar suporte à definição da prioridade de reidratação

## <a name="june-02-2020"></a>02 de Junho de 2020

Versão 2.7.0

### <a name="acr"></a>ACR

* Correção de um erro de digitação em uma mensagem de erro de criação de token

### <a name="aks"></a>AKS

* Alteração da sku de vm padrão para Standard_D2s_v3
* Correção da criação de atribuição de função para sub-rede personalizada MSI cluster Plus

### <a name="appservice"></a>AppService

* A correção #12739 az appservice list-locations retorna alguns locais inválidos

### <a name="arm"></a>ARM

* `az deployment`: Correção do problema #13159 de mensagem incorreta do JSON após a remoção de comentários e a compactação
* `az resource tag`: Correção do problema #13255 de marcação de recursos com o tipo de recurso `Microsoft.ContainerRegistry/registries/webhooks`
* Melhoria dos exemplos do módulo de recursos

### <a name="aro"></a>ARO

* Alteração do CLIError para corrigir o sinalizador para --worker-vm-disk-size-gb

### <a name="eventhub"></a>EventHub

* Correção do problema #12406 Argumento --capture-interval não atualiza o "intervalInSeconds"

### <a name="hdinsight"></a>HDInsight

* Alteração de get_json_object para shell_safe_json_parse

### <a name="monitor"></a>Monitoramento

* `az monitor metrics alert`: ajuste de várias mensagens de ajuda
* `az monitor diagnostic-settings create`: suporte ao argumento --export-to-resource-specific
* Suporte para recuperar o workspace de LA

### <a name="network"></a>Rede

* `az network dns zone`: suporte – caractere
* `az network vpn-connection ipsec-policy`: alteração do --sa-lifetime e do --sa-max-size para valores maiores no exemplo
* Aumento da rede para 2020-04-01
* `az network private-endpoint-connection`: suporte à grade de eventos
* `az network express-route list-route-tables`: correção do bug que faz não ser possível listar rotas como tabela

### <a name="packaging"></a>Empacotamento

* Adição do Pacote Focal do Ubuntu

### <a name="rbac"></a>RBAC

* `az ad sp credential reset`: modificar a geração de credenciais para evitar caracteres especiais problemáticos

### <a name="redis"></a>Redis

* Correção #13529: alteração da documentação do parâmetro enable_non_ssl_port

### <a name="storage"></a>Armazenamento

* `az storage copy`: adição do parâmetro `--follow-symlinks` para dar suporte ao symlinks
* Habilitar contexto local para a conta de armazenamento
* `az storage logging`: Correção do problema #11969 para ajustar a mensagem de erro

## <a name="may-19-2020"></a>19 de maio de 2020

Versão 2.6.0

### <a name="acr"></a>ACR

* Adiciona tempo limite padrão de 5 minutos para solicitações ao ACR
* Suporte para desabilitar o acesso à redes públicas
* `az acr token create`: expõe o argumento --days
* `az acr import`: aceita valores do argumento --source que contêm logon no nome do servidor por meio da correção final do cliente

### <a name="acs"></a>ACS

* Correção de bug: remover limpeza de campos para campos que não existem mais

### <a name="aks"></a>AKS

* Atualiza o tempo de atividade do contexto de ajuda de comando do SLA
* Remove a verificação do intervalo para a atualização da contagem de minutos do dimensionador automático
* Corrige o problema que fazia com que a CLI falhasse quando o usuário especificava apenas a senha do Windows

### <a name="ams"></a>AMS

* `az ams transform create`: Adiciona a capacidade de criar uma transformação com um FaceDetector predefinido
* `az ams content-key-policy create`: Adiciona a capacidade de criar uma política de chave de conteúdo do FairPlay com uma configuração de aluguel offline

### <a name="appconfig"></a>AppConfig

* Correção de bug para valores de chave da lista com campos

### <a name="appservice"></a>AppService

* `az functionapp create`: AzureWebJobsDashboard será definido somente se AppInsights estiver desabilitado
* Correção #10664 – Integração VNet – Problema de Verificação de Localização e Correção #13257-AZ Web App falha quando o RG precisar ser criado
* `az webapp|functionapp config ssl import`: Pesquisa o cofre de chaves em grupos de recursos na assinatura e aprimora a ajuda e os exemplos.
* Integra o contexto local para o serviço de aplicativo

### <a name="arm"></a>ARM

* `az deployment`: Corrige o problema que faz com que o templateLink não seja retornado ao implantar ou validar o template-uri
* `az deployment`: Corrige o problema que faz com que implantação/validação não dê suporte ao caractere codificado especialmente
* `az deployment sub/group what-if`: Corrige o alinhamento de matriz e o tratamento de erro
* `az deployment operation`: Modifica as informações preteridas

### <a name="aro"></a>ARO

* Adiciona exemplos para az aro create, list, list-credentials, show, delete
* Adiciona a função generate_random_id

### <a name="backup"></a>Backup

* Permite FriendlyName ao habilitar proteção para o comando AzureFileShare
* Correção do comando restore-disks da IaasVM
* Adiciona o BackupManagementType "MAB" ao comando item list
* Adiciona suporte para a repetição de tentativas de atualização da política para itens com falha.
* Adiciona a funcionalidade de Retomada de Proteção para as Máquinas Virtuais do Azure
* Adiciona suporte para especificar o ResourceGroup para armazenar instantRP durante a Criação ou Modificação de Política

### <a name="ci"></a>CI

* Suporte para flake8 3.8.0

### <a name="compute"></a>Computação

* Novo comando az vm auto-shutdown
* `az vm list-skus`: Atualização do comportamento --zone, retorna SKUs de todos os tipos agora

### <a name="core"></a>Núcleo

* Atualiza o status de ativado/desativado do contexto local para o nível de usuário global

### <a name="extension"></a>Extensão

* `az extension add`: Adiciona --system para habilitar a instalação de extensões em um caminho do sistema
* Suporte para .egg-info para armazenar metadados de extensão de tipo de roda

### <a name="iot"></a>IoT

* `az iot`: Atualiza a mensagem de reconhecimento de extensão da primeira execução do módulo de comando IoT para a ID precisa e moderna não preterida `azure-iot`.

### <a name="iot-hub"></a>Hub IoT

* Suporte para comandos de isolamento de rede e API 2020-03-01

### <a name="netappfiles"></a>NetAppFiles

* `az volume create`: Adiciona snapshot-id como um parâmetro para criar volume – isso permitirá que os usuários criem um volume por meio de um instantâneo existente.

### <a name="network"></a>Rede

* Corrige o valor TTL alterado não destinado ao DNS add-record
* `az network public-ip create`: Informa os clientes sobre futuras alterações da falha
* Suporte para comandos genéricos para cenários de link privado
* `az network private-endpoint-connection`: suporte a tipos mysql, postgres e mariadb
* `az network private-endpoint-connection`: Suporte para tipos cosmosdb
* `az network private-endpoint`: pretere --group-ids e redireciona para --group-id

### <a name="output"></a>Saída

* Mostra instruções de atualização em localizar, comentários e --help

### <a name="packaging"></a>Empacotamento

* Cria pacotes MSI/Homebrew com dependências resolvidas de requirements.txt

### <a name="rbac"></a>RBAC

* `az ad sp credential reset`: corrige a geração de credenciais fracas

### <a name="storage"></a>Armazenamento

* `az storage account file-service-properties update/show`: Adiciona suporte a propriedades de arquivo para a conta de armazenamento
* `az storage container create`: Correção #13373 ao adicionar o validador para acesso público
* Adiciona suporte a ADLS Gen2 track2
* `az storage blob sync`: Dar suporte à `--connection-string`
* `az storage blob sync`: Corrige a mensagem de erro incorreta quando azcopy não consegue encontrar o local de instalação

## <a name="april-30-2020"></a>30 de abril de 2020

Versão 2.5.1

### <a name="acr"></a>ACR

* `az acr check-health`: correção de "DOCKER_PULL_ERROR" no Windows

### <a name="compute"></a>Computação

* `az vm list-ip-addresses`: Tratamento de erros
* Correção de um bug de criação de VM caso endpoint_vm_image_alias_doc não estivesse definido no perfil de nuvem
* `az vmss create`: adição de --os-disk-size-gb

### <a name="cosmos-db"></a>Cosmos DB

* `az cosmosdb create/update`: adição de suporte a --enable-public-network

### <a name="extension"></a>Extensão

* Correção do carregamento de metadados errados para a extensão de tipo roda

### <a name="packaging"></a>Empacotamento

* Adição de script az para Git Bash/Cygwin no Windows

### <a name="sql"></a>SQL

* `az sql instance-pool`: adição de grupo de comando de pools de instância

### <a name="storage"></a>Armazenamento

* Atualização do pacote azure-multiapi-storage para 0.3.0
* Dá suporte ao GZRS para a criação e atualização da conta de armazenamento
* `az storage account failover`: adição de suporte para failover da conta de armazenamento de GRS/GZRS
* `az storage blob upload`: adição do parâmetro --encryption-scope para dar suporte à especificação da informação do escopo da criptografia

## <a name="april-28-2020"></a>28 de abril de 2020

Versão 2.5.0

### <a name="acs"></a>ACS

* [ALTERAÇÃO SIGNIFICATIVA] az openshift create: remove o parâmetro --vnet-peer.
* `az openshift create`: adição de sinalizadores para dar suporte a clusters privados.
* `az openshift`: atualização para a versão `2019-10-27-preview` da API.
* `az openshift`: adição do comando `update`.

### <a name="aks"></a>AKS

* `az aks create`: adição do suporte para Windows

### <a name="appservice"></a>AppService

* `az webapp deployment source config-zip`: remoção da suspensão após request.get()

### <a name="arm"></a>ARM

* Adição de comandos What-If de implantação de modelo

### <a name="aro"></a>ARO

* `az aro`: correção da saída da tabela

### <a name="ci"></a>CI

* Integração do pytest e preterição do nose para o teste de automação

### <a name="compute"></a>Computação

* `az vmss disk detach`: correção do problema de NoneType do disco de dados
* `az vm availability-set list`: suporte à exibição da lista de VM
* `az vm list-skus`: correção do problema de exibição do formato de tabela

### <a name="keyvault"></a>KeyVault

* Adição de novo parâmetro `--enable-rbac-authorization` durante a criação ou atualização

### <a name="monitor"></a>Monitoramento

* Suporte aos recursos de CMK do cluster de LA
* `az monitor log-analytics workspace linked-storage`: dá suporte aos recursos BYOS

### <a name="network"></a>Rede

* `az network security-partner`: suporte para provedor de segurança de parceiros

### <a name="privatedns"></a>Privatedns

* Adição do recurso na zona DNS privada para importar o arquivo da zona de exportação

## <a name="april-21-2020"></a>21 de abril de 2020

Versão 2.4.0

### <a name="acr"></a>ACR

* `az acr run --cmd`: desabilitar a substituição do diretório de trabalho
* Suporte ao ponto de extremidade dos dados dedicados

### <a name="aks"></a>AKS

* `az aks list -o table` deve mostrar privateFqdn como fqdn para clusters privados
* Adicionar --uptime-sla
* Atualizar pacote containerservice
* Adicionar suporte ao IP público do nó
* Corrigir erros de digitação no comando de ajuda

### <a name="appconfig"></a>AppConfig

* Resolver referência do cofre de chaves para os comandos kv list e export
* Correção de bug para valores de chave da lista

### <a name="appservice"></a>AppService

* `az functionapp create`: mudou a maneira como o linuxFxVersion estava sendo definido para os aplicativos de funções dotnet linux. Isso deve corrigir um bug que estava impedindo a criação de aplicativos de consumo em dotnet linux
* [ALTERAÇÃO DA FALHA] `az webapp create`: correção para manter o AppSettings existente com o az webapp create
* [ALTERAÇÃO DA FALHA] `az webapp up`: correção para criar o RG para o comando az webapp up ao usar o sinalizador -g
* [ALTERAÇÃO DA FALHA] `az webapp config`: correção para mostrar valores de saída não JSON com o az webapp config connection-string list

### <a name="arm"></a>ARM

* `az deployment create/validate`: adicionar o parâmetro `--no-prompt` para dar suporte à ação de ignorar o prompt de parâmetros ausentes para o modelo do Resource Manager
* `az deployment group/mg/sub/tenant validate`: dar suporte aos comentários no arquivo de parâmetro de implantação
* `az deployment`: remover `is_preview` para o parâmetro `--handle-extended-json-format`
* `az deployment group/mg/sub/tenant cancel`: dar suporte para cancelar a implantação do modelo do Resource Manager
* `az deployment group/mg/sub/tenant validate`: melhorar a mensagem de erro quando a verificação de implantação falhar
* `az deployment-scripts`: adicionar novos comandos para DeploymentScripts
* `az resource tag`: adicionar o parâmetro `--is-incremental` para dar suporte à adição de marcas ao recurso de maneira incremental

### <a name="aro"></a>ARO

* `az aro`:  adicionar módulo de comando aro do Azure RedHat OpenShift V4

### <a name="batch"></a>Lote

* Atualizar a API do Lote

### <a name="compute"></a>Computação

* `az sig image-version create`: adicionar o tipo da conta de armazenamento Premium_LRS
* `az vmss update`: corrigir problema de atualização de notificação de término
* `az vm/vmss create`: adicionar suporte para a versão de imagem especializada
* Versão da API SIG 2019-12-01
* `az sig image-version create`: Adicionar --target-region-encryption
* Os testes de correção falham quando executados em série, pois o nome do keyvault está duplicado no cache global na memória

### <a name="cosmosdb"></a>CosmosDB

* Dar suporte à `az cosmosdb private-link-resource/private-endpoint-connection`

### <a name="iot-central"></a>Central da IoT

* Preterir `az iotcentral`
* Adicionar o módulo de comando `az iot central`

### <a name="monitor"></a>Monitoramento

* Dar suporte ao cenário de link privado para monitoramento
* Corrigir a maneira incorreta de simulação em test_monitor_general_operations.py

### <a name="network"></a>Rede

* Preterir o sku para o comando de atualização de ip público
* `az network private-endpoint`: dar suporte ao grupo de zona dns privada
* Habilitar o recurso de contexto local para o parâmetro vnet/sub-rede
* Corrigir o exemplo de uso incorreto em test_nw_flow_log_delete

### <a name="packaging"></a>Empacotamento

* Descartar o suporte para o pacote Ubuntu/Disco

### <a name="rbac"></a>RBAC

* `az ad app create/update`: dar suporte a --optional-claims como um parâmetro

### <a name="rdbms"></a>RDBMS

* Adicionar comandos do administrador do Azure Active Directory para PostgreSQL e MySQL

### <a name="service-fabric"></a>Service Fabric

* Correção nº 12891: `az sf application update --application-parameters` remove parâmetros antigos que não estão na solicitação
* Correção nº 12470 az sf create cluster, corrigir bugs na atualização de durabilidade e confiabilidade e encontrar vmss corretamente por meio do código, dado um nome de tipo de nó

### <a name="sql"></a>SQL

* Adicionar `az sql mi op list`, `az sql mi op get`, `az sql mi op cancel`
* `az sql midb`: atualizar/mostrar política de retenção de longo prazo, mostrar/excluir backups de retenção de longo prazo, restaurar backup de retenção de longo prazo

### <a name="storage"></a>Armazenamento

* Atualizar azure-mgmt-storage para 9.0.0
* `az storage logging off`: dar suporte à desativação do registro em log de uma conta de armazenamento
* `az storage account update`: habilitar rotação automática de chave para CMK
* `az storage account encryption-scope create/update/list/show`: adicionar suporte para personalizar o escopo de criptografia
* `az storage container create`: adicionar --default-encryption-scope e --deny-encryption-scope-override a fim de definir o escopo de criptografia para o nível de contêiner

### <a name="survey"></a>Pesquisa

* Adicionar opção para desligar o link de pesquisa

## <a name="april-01-2020"></a>1º de abril de 2020

Versão 2.3.1

### <a name="acr"></a>ACR

* Corrigir a versão errada do azure-mgmt-containerregistry para Linux

### <a name="profile"></a>Perfil

* az login: Corrigir falha de logon com perfis de nuvem diferentes de `latest`

## <a name="march-31-2020"></a>31 de março de 2020

Versão 2.3.0

### <a name="acr"></a>ACR

* 'az acr task update': exceção de ponteiro nulo
* `az acr import`: Modificar a mensagem de ajuda e de erro para esclarecer o uso de --source e --registry
* Adicionar um validador para o argumento 'registry_name'
* `az acr login`: remover o sinalizador de visualização em '--expose-token'
* O parâmetro de branch 'az acr task create/update' de [ALTERAÇÃO SIGNIFICATIVA] foi removido
* O cliente 'az acr task update' agora pode atualizar o contexto, o token do git e/ou os gatilhos individualmente
* 'az acr agentpool': novo recurso

### <a name="aks"></a>AKS

* Corrigir apiServerAccessProfile ao atualizar --api-server-authorized-ip-ranges
* aks update: Substituir IPs de saída por valores de entrada ao atualizar
* Não criar SPN para clusters MSI e dar suporte à anexação de ACR a clusters MSI

### <a name="ams"></a>AMS

* Correção nº. 12469: a adição da política de chave de conteúdo Fairplay falha devido a problemas com o parâmetro 'ask'

### <a name="appconfig"></a>AppConfig

* Adicionar --skip-keyvault a kv export

### <a name="appservice"></a>AppService

* Correção nº 12509: remover a marca para az webapp up por padrão
* az functionapp create: o menu de ajuda de --runtime-version foi atualizado e um aviso foi adicionado quando o usuário especifica --runtime-version para dotnet
* az functionapp create: atualizado o modo como o javaVersion estava sendo definido para aplicativos de funções do Windows

### <a name="arm"></a>ARM

* az deployment create/validate: usar --handle-extended-json-format por padrão
* az lock create: adicionar exemplos de criação de subrecurso na documentação da ajuda
* az deployment {group/mg/sub/tenant} list: dar suporte à filtragem de provisioningState
* az deployment: corrigir o bug de análise para o comentário no último argumento

### <a name="backup"></a>Backup

* Adicionadas várias funcionalidades de restauração de arquivo
* Adicionado suporte para backup somente de discos do SO
* Adicionado o parâmetro restore-as-unmanaged-disk para especificar a restauração não gerenciada

### <a name="compute"></a>Computação

* az vm create: adicionar opção NONE de --nsg-rule
* az vmss create/update: remover a marca de visualização de reparos automáticos do vmss
* az vm update: dar suporte a --workspace
* Corrigir um bug no código de inicialização de VirtualMachineScaleSetExtension
* Atualizar a versão do VMAccessAgent para 2.4
* az vmss set-orchestration-service-state: dar suporte para o estado de definição do serviço de orquestração do vmss
* Atualizar a API do disco para a versão 2019-11-01
* az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun

### <a name="cosmos-db"></a>Cosmos DB

* Corrigir a ausência da opção --type para redirecionamentos de preterimento

### <a name="docker"></a>Docker

* Atualizar para Alpine 3.11 e Python 3.6.10

### <a name="extension"></a>Extensão

* Permitir carregar extensões no caminho do sistema por meio de pacotes

### <a name="hdinsight"></a>HDInsight

* (az hdinsight create:) dar suporte à especificação da versão de TLS mínima pelos clientes usando o parâmetro `--minimal-tls-version`. O valor permitido é 1.0,1.1,1.2

### <a name="iot"></a>IoT

* Adicionar codeowner
* az iot hub create : alterar o SKU padrão de F1 para S1
* iot hub: dar suporte a IotHub no perfil de 2019-03-01-hybrid

### <a name="iotcentral"></a>IoT Central

* Atualizar detalhes do erro, atualizar modelo de aplicativo padrão e a mensagem de aviso

### <a name="keyvault"></a>KeyVault

* Suporte para backup/restauração de certificado
* keyvault create/update: Suporte a --retention-days
* Não exibir mais chaves/segredos gerenciados durante a listagem
* az keyvault create: suporte a `--network-acls`, `--network-acls-ips` e `--network-acls-vnets` para especificar regras de rede ao criar o cofre

### <a name="lock"></a>Bloqueio

* az lock delete fix bug: az lock delete não funciona no Microsoft.DocumentDB

### <a name="monitor"></a>Monitoramento

* az monitor clone: suporte a regras de métrica de clone de um recurso para outro
* Corrigir IcM179210086: não é possível criar um alerta de métrica personalizado para a métrica de Application Insights

### <a name="netappfiles"></a>NetAppFiles

* az volume create: permitir volumes de proteção de dados adicionando operações de replicação: approve, suspend, resume, status, remove

### <a name="network"></a>Rede

* az network application-gateway waf-policy managed-rule rule-set add: dar suporte a Microsoft_BotManagerRuleSet
* network watcher flow-log show: corrigir informações erradas em preterimento
* dar suporte a nomes de host no ouvinte do gateway de aplicativo
* az network nat gateway: dar suporte para criar um recurso vazio sem IP público nem prefixo de IP público
* Dar suporte à geração de gateway de VPN
* Dar suporte a `--if-none-match` em `az network dns record-set {} add-record`

### <a name="packaging"></a>Empacotamento

* Remover o suporte ao Python 3.5

### <a name="profile"></a>Perfil

* az login: Mostrar aviso para erro de MFA

### <a name="rdbms"></a>RDBMS

* Adicionar comandos de gerenciamento de chaves de criptografia de dados do servidor para PostgreSQL e MySQL

## <a name="march-10-2020"></a>10 de março de 2020

Versão 2.2.0

### <a name="acr"></a>ACR

* Correção: `az acr login` gerava erro incorretamente
* Adicionou o novo comando `az acr helm install-cli`
* Adicionou link privado e suporte do CMK
* Adicionou o comando 'private-link-resource list'

### <a name="aks"></a>AKS

* correção da busca do AKS no Cloud Shell
* az aks: correção dos erros de complemento de monitoramento e de agentpool NoneType
* Adicionou --nodepool-tags ao pool de nós ao criar o cluster do Kubernetes do Azure
* Adicionou --tags ao adicionar ou atualizar um pool de nós para o cluster
* AKS create: adicionou `--enable-private-cluster`
* Adicionou --nodepool-labels ao criar o cluster do Kubernetes do Azure
* Adicionou --labels ao adicionar um novo pool de nós ao cluster do Kubernetes do Azure
* Adicionou / ausente na URL do painel
* Suporte para criar clusters do AKS habilitando identidade gerenciada
* az aks: validou o plug-in de rede como "Azure" ou "Kubenet"
* az aks: adicionou suporte da chave da sessão do AAD
* [ALTERAÇÃO SIGNIFICATIVA] AZ AKS: suporte para alterações de MSI para GF e BF para omsagent (Monitoramento de contêiner) (#1)
* az aks use-dev-spaces: adicionou a opção de tipo de ponto de extremidade ao comando use-dev-spaces para personalizar o ponto de extremidade criado em um controlador Azure Dev Spaces

### <a name="appconfig"></a>AppConfig

* Desbloqueou usando "KV set" para adicionar o recurso e a referência do keyvault...

### <a name="appservice"></a>AppService

* az webapp create: correção do problema ao executar o comando com --runtime
* az functionapp deployment source config-zip: adicionou uma mensagem de erro se o grupo de recursos ou o nome da função forem inválidos/não existirem
* functionapp create: correção da mensagem de aviso que aparece com `functionapp create` hoje, que cita um sinalizador de `--functions_version`, mas usa erroneamente `_` em vez de `-` no nome do sinalizador
* az functionapp create: atualizou o modo como linuxFxVersion e o nome da imagem de contêiner eram definidos para aplicativos de funções do Linux
* az functionapp deployment source config-zip: correção de um problema causado pelas configurações do aplicativo que alterava a condição de corrida durante a implantação do zip, provocando erros 5xx durante a implantação
* Correção #5720946: AZ WebApp backup falha ao definir o nome

### <a name="arm"></a>ARM

* az resource: aprimorou os exemplos do módulo de recurso
* az policy assignment list: suporte à listagem de atribuições de política no escopo do Grupo de Gerenciamento
* Adicionou `az deployment group` e `az deployment operation group` para a implantação de modelos nos grupos de recursos. Esta é uma duplicata de `az group deployment` e `az group deployment operation`
* Adicionou `az deployment sub` e `az deployment operation sub` para a implantação de modelos no escopo da assinatura. Esta é uma duplicata de `az deployment` e `az deployment operation`
* Adicionou `az deployment mg` e `az deployment operation mg` para implantação de modelos nos grupos de gerenciamento.
* Adicionou `az deployment tenant` e `az deployment operation tenant` para implantação de modelos no escopo do locatário.
* az policy assignment create: adicionou descrição ao parâmetro `--location`
* az group deployment create: adicionou o parâmetro `--aux-tenants` para dar suporte a locatários cruzados

### <a name="cdn"></a>CDN

* Adicionou comandos do WAF da CDN

### <a name="compute"></a>Computação

* az sig image-version: adicionar --data-snapshot-luns
* AZ PPG show: adicionou --outlocation-status para habilitar a busca do status de colocalização de todos os recursos no grupo de posicionamento por proximidade
* az vmss create/update: suporte a reparos automáticos
* [ALTERAÇÃO SIGNIFICATIVA] modelo de imagem AZ: renomear modelo para builder
* AZ Image Builder Create: adicionou --Image-template

### <a name="cosmos-db"></a>Cosmos DB

* Adicionou procedimento armazenado do SQL, UDF e disparar cmdlets
* az cosmosdb create: adicionou --key-uri para dar suporte à adição de informações de criptografia do cofre de chaves

### <a name="keyvault"></a>KeyVault

* keyvault create: habilitou a exclusão reversível por padrão

### <a name="monitor"></a>Monitoramento

* az monitor metrics alert create: suporte a `~` em `--condition`

### <a name="network"></a>Rede

* az network application-gateway rewrite-rule create: suporte à configuração de URL
* az network dns zone import: --zone-name não diferenciará maiúsculas de minúsculas no futuro
* az network private-endpoint/private-link-service: removeu rótulo de visualização
* az network bastion: suporte a bastions
* az network vnet list-available-ips: dar suporte à lista de IPs disponíveis em uma vnet
* az network watcher flow-log create/list/delete/update: adicionou novos comandos para gerenciar o log de fluxo do Inspetor e expor o --local para identificá-lo explicitamente
* az network watcher flow-log configure: preterido
* az network watcher flow-log show: dá suporte a --location e --name para obter o resultado formatado por ARM, saída formatada antiga preterida

### <a name="policy"></a>Política

* az policy assignment create: correção do bug que gerou automaticamente o nome da atribuição de política, que excede o limite

### <a name="rbac"></a>RBAC

* az ad group show: correção do valor --group, que é tratado como um problema de regex

### <a name="rdbms"></a>RDBMS

* Trocou a versão do zure-mgmt-rdbms SDK para 2.0.0
* az postgres private-endpoint-connection: gerenciou conexões de ponto de extremidade privado do Postgres
* az postgres private-link-resource: gerenciou recursos de link privado do Postgres
* az mysql private-endpoint-connection: gerenciar conexões de ponto de extremidade privado do MySQL
* az mysql private-link-resource: gerenciou recursos de link privado do MySQL
* az mariadb private-endpoint-connection: gerenciou conexões de ponto de extremidade privado do MariaDB
* az mariadb private-link-resource: gerenciou recursos de link privado do MariaDB
* Atualizando testes de ponto de extremidade privado do RDBMS

### <a name="sql"></a>SQL

* Sql midb Add: list-deleted, show-deleted, update-retention, show-retention
* (sql server create:) adicionou o sinalizador ' habilitar '/' desabilitar ' opcional public-network-access ao SQL Server create
* (sql server update:) fez algumas alterações voltadas para o cliente
* adicionou a propriedade minimal_tls_version para o banco de BD de MI e SQL

### <a name="storage"></a>Armazenamento

* az storage blob delete-batch: sinalizador `--dryrun` de comportamento inadequado
* az storage account network-rule add (correção de bug): a operação de adição deve ser idempotente
* az storage account create/update: Adicionou suporte de preferência de roteamento
* Atualizou a versão do azure-mgmt-storage para 8.0.0
* az storage container immutability create: adicionou o parâmetro --allow-protected-append-write
* az storage account private-link-resource list: Adicionou suporte para lista de recursos de link privado para a conta de armazenamento
* az storage account private-endpoint-connection approve/reject/show/delete: Suporte para gerenciar conexões de ponto de extremidade privado
* az storage account blob-service-properties update: adicionou --enable-restore-policy e --restore-days
* az storage blob restore: adicionou suporte para restaurar intervalos de blob

## <a name="february-18-2020"></a>18 de fevereiro de 2020

Versão 2.1.0

### <a name="acr"></a>ACR

* Adicionar um novo argumento `--expose-token` a `az acr login`
* Corrigir a saída incorreta de `az acr task identity show -n Name -r Registry -o table`
* az acr login: Gerar CLIError se erros forem retornados pelo comando docker

### <a name="acs"></a>ACS

* aks create/update: adicionar a validação `--vnet-subnet-id`

### <a name="aladdin"></a>Aladdin

* Analisar os exemplos gerados no _help.py do comando

### <a name="ams"></a>AMS

* az ams já está em GA

### <a name="appconfig"></a>AppConfig

* Revisar a mensagem de ajuda para excluir o filtro de chave/rótulo não compatível
* Remover a marca de versão prévia da maioria dos comandos que excluem a identidade gerenciada e têm sinalizadores
* Adicionar a chave gerenciada do cliente ao atualizar os repositórios

### <a name="appservice"></a>AppService

* az webapp list-runtimes: Corrigir o bug de list-runtimes
* Adicionar az webapp|functionapp config ssl create
* Adicionar compatibilidade com aplicativos de funções v3 e nó 12

### <a name="arm"></a>ARM

* az policy assignment create: Corrigir a mensagem de erro quando o parâmetro `--policy` for inválido
* az group deployment create: Corrigir o erro "stat: o caminho é muito longo para o Windows" ao usar o arquivo grande parameters.json

### <a name="backup"></a>Backup

* Corrigir o fluxo de recuperação de nível de item no OLR
* Adicionar compatibilidade com restauração como arquivo aos bancos de dados SQL e SAP

### <a name="compute"></a>Computação

* vm/vmss/availability-set update: adicionar --ppg para permitir a atualização de ProximityPlacementGroup
* vmss create: adicionar --data-disk-iops e --data-disk-mbps
* az vm host: remover a marca de versão prévia de `vm host` e `vm host group`
* [ALTERAÇÃO SIGNIFICATIVA] Correção nº 10.728: `az vm create`: criar uma sub-rede automaticamente quando a vnet for especificada e não houver uma sub-rede
* Aumentar a robustez da lista de imagens de VM

### <a name="eventhub"></a>Eventhub

* Compatibilidade com o Azure Stack para o perfil 2019-03-01-hybrid

### <a name="keyvault"></a>KeyVault

* az keyvault key create: adicionar um novo valor `import` ao parâmetro `--ops`
* az keyvault key list-versions: compatibilidade com o parâmetro `--id` para especificar chaves
* Compatibilidade com conexões de ponto de extremidade privado

### <a name="network"></a>Rede

* Avançar para azure-mgmt-network 9.0.0
* az network private-link-service update/create: dá suporte a --enable-proxy-protocol
* Adicionar o recurso de Monitor de conexão V2

### <a name="packaging"></a>Empacotamento

* [ALTERAÇÃO SIGNIFICATIVA] Fim da compatibilidade com o Python 2.7

### <a name="profile"></a>Perfil

* Visualização: Adicionar novos atributos `homeTenantId` e `managedByTenants` às contas de assinatura. Executar `az login` novamente para as alterações entrarem em vigor
* az login: Mostrar um aviso quando uma assinatura estiver listada de mais de um locatário e definir a primeira como padrão. Para selecionar um locatário específico ao acessar essa assinatura, inclua `--tenant` em `az login`

### <a name="role"></a>Função

* az role assignment create: Corrigir o erro em que atribuir uma função a uma entidade de serviço pelo nome de exibição gera um HTTP 400

### <a name="sql"></a>SQL

* Atualizar o cmdlet da Instância Gerenciada do SQL `az sql mi update` com dois novos parâmetros: nível e família

### <a name="storage"></a>Armazenamento

* [ALTERAÇÃO DA FALHA] `az storage account create`: Alterar o tipo de conta de armazenamento padrão para StorageV2

## <a name="february-04-2020"></a>4 de fevereiro de 2020

Versão 2.0.81

### <a name="acs"></a>ACS

* Adicionar suporte para definir portas alocadas de saída e tempos limite ociosos no balanceador de carga standard
* Atualizar para a versão da API 2019-11-01

### <a name="acr"></a>ACR

* A [ALTERAÇÃO DA FALHA] `az acr delete` será exibida
* A [ALTERAÇÃO SIGNIFICATIVA] 'az acr task delete’ será exibida
* Adicionar um novo grupo de comandos ‘az acr taskrun show/list/delete’ para o gerenciamento de taskrun

### <a name="aks"></a>AKS

* Cada cluster obtém uma entidade de serviço separada para aprimorar o isolamento

### <a name="appconfig"></a>AppConfig

* Dar suporte à importação/exportação de referências keyvault de/a appservice
* Dar suporte à importação/exportação de todos os rótulos de appconfig para appconfig
* Validar nomes de chave e recursos antes de configurar e importar
* Exponha a modificação do sku para o repositório de configurações.
* Adicione o grupo de comandos à identidade gerenciada.

### <a name="appservice"></a>AppService

* Azure Stack: comandos de superfície no perfil de 2019-03-01-hybrid
* functionapp: adicionar a capacidade de criar aplicativos de funções Java no Linux

### <a name="arm"></a>ARM

* Correção de problema nº 10246: `az resource tag` falha quando o parâmetro `--ids` passado é a ID do grupo de recursos
* Correção de problema nº 11658: o comando `az group export` não é compatível com os parâmetros `--query` e `--output`
* Correção de problema nº 10279: O código de saída `az group deployment validate` é 0 quando a verificação falha
* Correção de problema nº 9916: aprimorar a mensagem de erro do conflito entre a marca e outras condições de filtro para o comando `az resource list`
* Adicionar novo parâmetro `--managed-by` para dar suporte à adição de informações managedBy para o comando `az group create`

### <a name="azure-red-hat-openshift"></a>Red Hat OpenShift no Azure

* Adicionar o subgrupo `monitor` para gerenciar o monitoramento do Log Analytics no cluster do Red Hat OpensShift no Azure

### <a name="botservice"></a>BotService

* Correção de problema nº 11697: `az bot create` não é idempotente
* Alterar testes de correção de nomes para serem executados somente em modo Ao vivo

### <a name="cdn"></a>CDN

* Adicionar suporte ao recurso rulesEngine
* Adicionar o novo grupo de comandos ‘cdn endpoint rule’ para gerenciar regras
* Atualizar a versão azure-mgmt-cdn para a 4.0.0 para usar a versão da API 2019-04-15

### <a name="deployment-manager"></a>Gerenciador de Implantação

* Adicione a operação de lista para todos os recursos.
* Aprimore o recurso de etapa do novo tipo de etapa.
* Atualize o pacote azure-mgmt-deploymentmanager para usar a versão 0.2.0.

### <a name="iot"></a>IoT

* Substitua os comandos ‘IoT hub Job’.

### <a name="iot-central"></a>Central da IoT

* Dê suporte à atualização/criação de aplicativos com o novo nome do SKU ST0, ST1, ST2.

### <a name="key-vault"></a>Key Vault

* Adicione um novo comando `az keyvault key download` para baixar chaves.

### <a name="misc"></a>Diversos

* Correção nº 6371: dar suporte à conclusão da variável de nome de arquivo e de ambiente em Bash

### <a name="network"></a>Rede

* Correção nº 2092: az network dns record-set add/remove: adicione um aviso quando record-set não é encontrado. No futuro, haverá suporte para um argumento extra para confirmar essa criação automática.

### <a name="policy"></a>Política

* Adicionar o novo comando `az policy metadata` para recuperar recursos avançados de metadados de política
* `az policy remediation create`: Especifique se a conformidade deve ser reavaliada antes da correção com o parâmetro `--resource-discovery-mode`

### <a name="profile"></a>Perfil

* `az account get-access-token`: Adicionar parâmetro `--tenant` para adquirir o token do locatário diretamente, sem a necessidade de especificar uma assinatura

### <a name="rbac"></a>RBAC

* [ALTERAÇÃO SIGNIFICATIVA] Correção nº 11883: `az role assignment create`: o escopo vazio exibirá erro

### <a name="security"></a>Segurança

* Adicione novos comandos `az atp show` e `az atp update` para exibir e gerenciar configurações avançadas de proteção contra ameaças para contas de armazenamento.

### <a name="sql"></a>SQL

* `sql dw create`: substitua os parâmetros `--zone-redundant` e `--read-replica-count`. Esses parâmetros não se aplicam ao DataWarehouse.
* [ALTERAÇÃO DA FALHA] `az sql db create`: Remova "WideWorldImportersStd" e "WideWorldImportersFull" como valores permitidos documentados para "az sql db create --sample-name". Esses bancos de dados de exemplo sempre farão a criação falhar.
* Adicione os novos comandos `sql db classification show/list/update/delete` e `sql db classification recommendation list/enable/disable` para gerenciar classificações de confidencialidade para bancos de dados SQL.
* `az sql db audit-policy`: Correção para ações e grupos de auditoria vazios

### <a name="storage"></a>Armazenamento

* Adicione um novo grupo de comandos `az storage share-rm` para usar o provedor de recursos Microsoft.Storage para operações de gerenciamento de compartilhamento de arquivo do Azure.
* Correção de problema nº 11415: erro de permissão para `az storage blob update`
* Integre Azcopy 10.3.3 e dê suporte a Win32.
* `az storage copy`: Adicione os parâmetros `--include-path`, `--include-pattern`, `--exclude-path` e `--exclude-pattern`
* `az storage remove`: Altere os parâmetros `--inlcude` e `--exclude` para os parâmetros `--include-path`, `--include-pattern`, `--exclude-path` e `--exclude-pattern`
* `az storage sync`: Adicione os parâmetros `--include-pattern`, `--exclude-path` e `--exclude-pattern`

### <a name="servicefabric"></a>ServiceFabric

* Adicione novos comandos para gerenciar o aplicativo e os serviços.

## <a name="january-13-2020"></a>13 de janeiro de 2020

Versão 2.0.80

### <a name="compute"></a>Computação

* atualização do disco: Adicionar --disk-encryption-set e --encryption-type
* criação/atualização do instantâneo: Adicionar --disk-encryption-set e --encryption-type

### <a name="storage"></a>Armazenamento

* Atualizar a versão do azure-mgmt-storage para 7.1.0
* `az storage account create`: Adicionar `--encryption-key-type-for-table` e `--encryption-key-type-for-queue` para dar suporte ao Serviço de Criptografia de Tabela e de Fila

## <a name="january-07-2020"></a>07 de janeiro de 2020

Versão 2.0.79

### <a name="acr"></a>ACR

* [ALTERAÇÃO SIGNIFICATIVA] Remover o parâmetro '--os' para 'acr build', 'acr task create/update', 'acr run' e 'acr pack'. Em vez disso, use '--platform'.

### <a name="appconfig"></a>AppConfig

* Adicionar suporte para importar/exportar sinalizadores de recurso
* Adicione o novo comando 'az appconfig kv set-keyvault' para criar a referência do keyvault
* Suporte a várias convenções de nomenclatura ao exportar os sinalizadores de recurso para o arquivo

### <a name="appservice"></a>AppService

* Corrigir o problema #7154: Atualizar a documentação para o comando <> para usar acentos grave em vez de aspas simples
* Corrigir o problema #11287: webapp up: Por padrão, faça o aplicativo criado usando 'should be 'SSL enabled'
* Corrigir o problema #11592: Adicionar o sinalizador az webapp up para sites HTML estáticos

### <a name="arm"></a>ARM

* Corrigir `az resource tag`: As marcas do Cofre dos Serviços de Recuperação não podem ser atualizadas

### <a name="backup"></a>Backup

* Novo comando 'backup protection undelete' adicionado para habilitar o recurso de exclusão reversível para carga de trabalho IaasVM
* Novo parâmetro '--soft-delete-feature-state' adicionado para definir o comando propriedades do backup
* Suporte de exclusão de disco adicionado para carga de trabalho IaasVM

### <a name="compute"></a>Computação

* Corrigir a falha `vm create` no perfil do Azure Stack.
* parte final/listar definições de métricas de monitor de vm: suporte a métricas de consulta e definições de lista para uma vm.
* Adicionar nova ação de comando de reaplicação para az vm

### <a name="hdinsight"></a>HDInsight

* Suporte para criar um cluster Kafka com o Proxy REST do Kafka
* Atualizar azure-mgmt-hdinsight para 1.3.0

### <a name="misc"></a>Diversos.

* Adicionar comando de visualização `az version show` para mostrar as versões dos módulos e das extensões da CLI do Azure no formato JSON por padrão ou no formato configurado por --output

### <a name="event-hubs"></a>Hubs de Eventos

* [ALTERAÇÃO SIGNIFICATIVA] Remover a opção de status 'ReceiveDisabled' do comando 'az eventhubs eventhub update' e 'az eventhubs eventhub create'. Essa opção não é válida para entidades do Hub de Eventos.

### <a name="service-bus"></a>Barramento de Serviço

* [ALTERAÇÃO SIGNIFICATIVA] Remover a opção de status 'ReceiveDisabled' do comando 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create' e 'az servicebus queue update'. Essa opção não é válida para tópicos e filas do Barramento de Serviço.

### <a name="rbac"></a>RBAC

* Correção #11712: `az ad app/sp show` não devolve o código de saída 3 quando o aplicativo ou a entidade de serviço não existir

### <a name="storage"></a>Armazenamento

* `az storage account create`: Remover o sinalizador de visualização do parâmetro --enable-hierarchical-namespace
* Atualizar a versão azure-mgmt-storage para 7.0.0 para usar a versão de API 2019-06-01
* Adicionar novos parâmetros `--enable-delete-retention` e `--delete-retention-days` para dar suporte ao gerenciamento da política de retenção de exclusão para a conta de armazenamento blob-service-properties.

## <a name="december-17-2019"></a>17 de dezembro de 2019

2.0.78

### <a name="acr"></a>ACR

* Contexto local de suporte adicionado na execução da tarefa acr

### <a name="acs"></a>ACS

* [ALTERAÇÃO SIGNIFICATIVA]criar az openshift: renomear `--workspace-resource-id` para `--workspace-id`.

### <a name="ams"></a>AMS

* Comandos de exibição atualizados para devolver 3 quando o recurso não for encontrado

### <a name="appconfig"></a>AppConfig

* Bug corrigido ao acrescentar a versão de API à URL de solicitação. A solução existente não funciona com a paginação.
* Suporte adicionado para a exibição de idiomas além do inglês, pois nosso serviço de back-end é compatível com unicode para globalização.

### <a name="appservice"></a>AppService

* Problema corrigido nº 11217: webapp: o upload ssl de configuração do az webapp deve ser compatível com o parâmetro do slot
* Problema corrigido nº 10965: Erro: O nome não pode estar vazio. Permitir remoção por ip_address e sub-rede
* Suporte adicionado para importar certificados do Key Vault `az webapp config ssl import`

### <a name="arm"></a>ARM

* Pacote azure-mgmt-resource atualizado para usar 6.0.0
* Suporte entre locatários para o comando `az group deployment create` adicionando o novo parâmetro `--aux-subs`
* Novo parâmetro `--metadata` adicionado para dar suporte à adição de informações de metadados para definições de conjunto de políticas.

### <a name="backup"></a>Backup

* Suporte de backup adicionado para carga de trabalho SQL e SAP Hana.

### <a name="botservice"></a>BotService

* [ALTERAÇÃO SIGNIFICATIVA] Remover o sinalizador '--version ' do comando de visualização 'az bot create'. Somente os bots do SDK v4 são compatíveis.
* Verificação de disponibilidade de nome adicionada para 'az bot create'.
* Suporte adicionado para atualizar a URL do ícone para um bot por meio de 'az bot update'.
* Suporte adicionado para atualizar um canal Direct Line por meio de 'az bot directline update'.
* Suporte ao sinalizador '--enable-enhanced-auth' adicionado para 'az bot directline create'.
* Os seguintes grupos de comandos estão em GA e não estão em versão prévia: 'az bot authsetting'.
* Os seguintes comandos em 'az bot' estão em GA e não na versão prévia: 'criar', 'preparar-implantar', 'mostrar', 'excluir', 'atualizar'.
* Correção do valor 'az bot prepare-deploy' alterando '--proj-file-path ' para letras minúsculas (por exemplo, "Test. csproj" para "Test. csproj").

### <a name="compute"></a>Computação

* Criar/atualizar vmss: --scale-in-policy adicionado, que decide quais máquinas virtuais são escolhidas para remoção quando um VMSS é dimensionado.
* atualização de vm/vmss: --priority adicionado.
* atualização de vm/vmss: --max-price adicionado.
* Grupo de comandos do conjunto de criptografia de disco adicionado (criar, mostrar, atualizar, excluir e listar).
* criação de disco: --encryption-type e --disk-encryption-set adicionados.
* vm/vmss create: --os-disk-encryption-set e --data-disk-encryption-sets adicionados.

### <a name="core"></a>Núcleo

* Suporte para Python 3.4 removido
* Pesquisa de funções de plug-in em vários comandos

### <a name="dls"></a>DLS

* Versão atualizada do SDK do ADLS (0.0.48).

### <a name="install"></a>Instalar

* Instalar suporte de script Python 3.8

### <a name="iot"></a>IOT

* [ALTERAÇÃO SIGNIFICATIVA] Parâmetro--failover-region removido de failover manual. Agora ele fará failover para a região secundária emparelhada atribuída geograficamente.

### <a name="key-vault"></a>Key Vault

* Nº 8095 corrigido: `az keyvault storage remove`: melhorar a mensagem de ajuda
* Nº 8921 corrigido: `az keyvault key/secret/certificate list/list-deleted/list-versions`: corrigir o bug de validação no parâmetro `--maxresults`
* Nº 10512 corrigido: `az keyvault set-policy`: melhorar a mensagem de erro quando nenhuma das `--object-id`, `--spn` ou `--upn` for especificada
* Nº 10846 corrigido: `az keyvault secret show-deleted`: quando `--id` for especificado, `--name/-n` não será necessário
* Nº 11084 corrigido: `az keyvault secret download`: melhorar a mensagem de ajuda do parâmetro `--encoding`

### <a name="network"></a>Rede

* Investigação de gateway de aplicativo de rede az: Suporte --port option adicionado para especificar uma porta para sondar servidores de back-end ao criar e atualizar
* az network application-gateway url-path-map create/update: correção de bug para `--waf-policy`
* az network application-gateway: Suporte `--rewrite-rule-set` adicionado
* az network list-service-aliases: Foram adicionados aliases de serviço da lista de suporte que podem ser usados para políticas de ponto de extremidade de serviço
* importar zona dns da rede az: Suporte adicionado. @ no nome do registro

### <a name="packaging"></a>Empacotamento

* Compilações de back edge adicionadas para instalação de pip
* Pacote eoan do Ubuntu adicionado

### <a name="policy"></a>Política

* Inclusão de compatibilidade com a API de Política, versão de 01/09/2019.
* az policy set-definition: Agrupamento de suporte adicionado nas definições do conjunto de políticas com `--definition-groups` parâmetro

### <a name="redis"></a>Redis

* Adicionado o parâmetro de visualização `--replicas-per-master` ao comando `az redis create`
* Azure-MGMT-Redis adicionado do 6.0.0 para o 7.0.0rc1

### <a name="servicefabric"></a>ServiceFabric

* Corrigido em nó-tipo adicionar lógica, incluindo #10963: A adição do novo tipo de nó com nível de durabilidade Gold sempre gerará erro da CLI
* Versão do ServiceFabricNodeVmExt atualizada para 1.1 no modelo de criação

### <a name="sql"></a>SQL

* Adicionados os parâmetros "--read-scale" e "--read-replicas" aos comandos criar e atualizar do BD SQL para dar suporte ao gerenciamento de escala de leitura.

### <a name="storage"></a>Armazenamento

* Propriedade de compartilhamentos de arquivos grandes da versão GA para o comando criar e atualizar da conta de armazenamento
* Suporte ao token SAS de delegação de usuário da versão GA
* Novos comandos adicionados `az storage account blob-service-properties show` e `az storage account blob-service-properties update --enable-change-feed` para gerenciar Propriedades do serviço blob para a conta de armazenamento.
* [PRÓXIMA ALTERAÇÃO DA FALHA] `az storage copy`: `*` não há mais suporte para o caractere de como um curinga na URL, mas novos parâmetros--include-pattern e --exclude-pattern serão adicionados com suporte a curinga `*`.
* Problema corrigido nº 11043: Suporte adicionado para remover contêiner/compartilhamento inteiro no comando `az storage remove`

## <a name="november-26-2019"></a>26 de novembro de 2019

Versão 2.0.77

### <a name="acr"></a>ACR

* Parâmetro `--branch` preterido da criação/atualização da tarefa ACR

### <a name="azure-red-hat-openshift"></a>Red Hat OpenShift no Azure

* Sinalizador `--workspace-resource-id` adicionado para permitir a criação do cluster do Red Hat OpenShift no Azure com monitoramento
* `monitor_profile` adicionado para criar o cluster do Red Hat OpenShift no Azure com monitoramento

### <a name="aks"></a>AKS

* Operação de rotação de certificado de cluster de suporte adicionada usando "az aks rotate-certs".

### <a name="appconfig"></a>AppConfig

* Suporte adicionado para usar ":" para o separador `as az appconfig kv import`
* Problema corrigido para listar valores de chave com vários rótulos incluindo o rótulo nulo. 
* SDK do plano de gerenciamento atualizado, azure-mgmt-appconfiguration, para a versão 0.3.0. 

### <a name="appservice"></a>AppService

* Problema corrigido nº 11100: AttributeError para az webapp up ao criar o plano de serviço
* az webapp up: Forçar a criação ou a implantação em um site para linguagens com suporte, nenhum padrão usado.
* Suporte adicionado para o Ambiente do Serviço de Aplicativo: az appservice ase show | list | list-addresses | list-plans | create | update | delete

### <a name="backup"></a>Backup

* Problema corrigido em list-associated-items da política de backup az. Parâmetro BackupManagementType opcional adicionado.

### <a name="compute"></a>Computação

* Versão de API de computação, discos e instantâneos atualizados para 2019-07-01
* vmss create: melhoria para --orchestration-mode
* sig image-definition create: --os-state adicionado para permitir a especificação se as máquinas virtuais criadas nessa imagem são 'Generalizadas' ou 'Especializadas'
* sig image-definition create: --hyper-v-generation adicionado para permitir a especificação da geração do hipervisor
* sig image-version create: --os-snapshot e --data-snapshots de suporte adicionados
* image create: --data-disk-caching adicionado para permitir a especificação da configuração de cache de discos de dados
* SDK de computação do Python atualizado para 10.0.0
* vm/vmss create: 'Spot' adicionado à propriedade de enumeração 'Priority'
* [ALTERAÇÃO SIGNIFICATIVA] Parâmetro '--max-billing' renomeado para '--max-price', para a VM e o VMSS, a fim de que seja consistente com os cmdlets do Swagger e do PowerShell
* vm monitor log show: suporte adicionado para consultar o log pelo workspace do Log Analytics vinculado.

### <a name="iot"></a>IOT

* Correção nº 2531: argumentos de conveniência adicionados para a atualização do hub.
* Correção nº 8323: parâmetros ausentes adicionados para criar o ponto de extremidade personalizado de armazenamento.
* Corrigir bug de regressão: as alterações que substituem o ponto de extremidade de armazenamento padrão foram revertidas.

### <a name="key-vault"></a>Key Vault

* Correção nº 11121: ao usar `az keyvault certificate list`, passar `--include-pending` agora não exige um valor de `true` ou `false`

### <a name="netappfiles"></a>NetAppFiles

* azure-mgmt-netapp atualizado para 0.7.0 que inclui algumas propriedades de volume adicionais associadas a operações de replicação futuras

### <a name="network"></a>Rede

* application-gateway waf-config: preterido
* application-gateway waf-policy: subgrupo managed-rules adicionado para gerenciar os conjuntos de regras e regras de exclusão gerenciados
* application-gateway waf-policy: subgrupo policy-setting adicionado para gerenciar a configuração global de um waf-policy
* [ALTERAÇÃO SIGNIFICATIVA] application-gateway waf-policy: subgrupo rule renomeado para custom-rule
* application-gateway http-listener: --firewall-policy adicionado durante a criação
* application-gateway url-path-map rule: --firewall-policy adicionado durante a criação

### <a name="packaging"></a>Empacotamento

* Wrapper az reescrito no Python
* Suporte adicionado para Python 3.8
* Alterado para Python 3 para o pacote RPM

### <a name="profile"></a>Perfil

* Erro aperfeiçoado ao executar `az login -u {} -p {}` com a conta Microsoft
* `SSLError` aperfeiçoado ao executar `az login` atrás de um proxy com o certificado raiz autoassinado
* Correção nº 10578: `az login` trava quando mais de uma instância é iniciada ao mesmo tempo no Windows ou WSL
* Correção nº 11059: `az login --allow-no-subscriptions` falhará se houver assinaturas no locatário
* Correção nº 11238: após renomear uma assinatura, fazer logon com a MSI fará a mesma assinatura aparecer duas vezes

### <a name="rbac"></a>RBAC

* Correção nº 10996: erro aperfeiçoado para `--force-change-password-next-login` em `az ad user update` quando `--password` não for especificado

### <a name="redis"></a>Redis

* Correção nº 2902: evite definir configurações de memória ao atualizar o cache do SKU básico

### <a name="reservations"></a>Reservas

* Versão do SDK atualizada para 0.6.0
* Informações de detalhes do plano de cobrança atualizadas após chamar Get-Gatalogs
* Novo comando `az reservations reservation-order calculate` adicionado para calcular o preço de uma reserva
* Novo comando `az reservations reservation-order purchase` adicionado para comprar uma nova reserva

### <a name="rest"></a>Rest
* `az rest` alterado para GA

### <a name="sql"></a>SQL

* azure-mgmt-sql atualizado para 0.15.0.

### <a name="storage"></a>Armazenamento

* storage account create: --enable-hierarchical-namespace adicionado para dar suporte à semântica do sistema de arquivos no serviço Blob.
* Exceção não relacionada removida da mensagem de erro
* Problemas corrigidos com a mensagem de erro incorreta "Você não tem as permissões necessárias para executar essa operação." quando bloqueado pelas regras de rede ou AuthenticationFailed.

## <a name="november-4-2019"></a>4 de novembro de 2019

Versão 2.0.76

### <a name="acr"></a>ACR

* O parâmetro de versão prévia `--pack-image-tag` foi adicionado ao comando `az acr pack build`.
* Suporte adicionado para habilitar a auditoria na criação de um registro
* Suporte adicionado para o RBAC com escopo de repositório

### <a name="aks"></a>AKS

* `--enable-cluster-autoscaler`, `--min-count` e `--max-count` foram adicionados ao comando `az aks create`, que habilita o dimensionamento automático do cluster para o pool de nós.
* Foram adicionados os sinalizadores acima, bem como `--update-cluster-autoscaler` e `--disable-cluster-autoscaler` ao comando `az aks update`, permitindo atualizações do cluster de dimensionamento automático.

### <a name="appconfig"></a>AppConfig

* O grupo de comandos do recurso AppConfig foi adicionado para gerenciar os sinalizadores de recurso armazenados em uma Configuração de Aplicativos.
* Foi corrigido um bug secundário do comando de exportação para arquivo appconfig kv. Foi interrompida a leitura de conteúdo do arquivo de destino durante a exportação.

### <a name="appservice"></a>AppService

* `az appservice plan create`: Foi adicionado o suporte para definir 'persitecalling' no comando appservice plan create.
* Foi corrigido um problema em que a operação webapp config ssl bind estava removendo as marcas existentes do recurso
* Foi adicionado o sinalizador `--build-remote` para `az functionapp deployment source config-zip` para dar suporte à ação de build remoto durante a implantação do aplicativo de funções.
* Foi alterada a versão do nó padrão em aplicativos de funções para ~10 para Windows
* A propriedade `--runtime-version` foi adicionada a `az functionapp create`

### <a name="arm"></a>ARM

* `az deployment/group deployment validate`: Foi adicionado o parâmetro `--handle-extended-json-format` para dar suporte a várias linhas e comentários no modelo JSON durante a implantação.
* O azure-mgmt-resource passou a usar a 2019-07-01

### <a name="backup"></a>Backup

* Foi adicionado o suporte de backup aos Arquivos do Azure

### <a name="compute"></a>Computação

* `az vm create`: foi adicionado um aviso ao especificar a rede acelerada e um adaptador de rede existente juntos.
* `az vm create`: foi adicionado `--vmss` para especificar um conjunto de dimensionamento de máquinas virtuais existente ao qual a máquina virtual deve ser atribuída.
* `az vm/vmss create`: foi adicionada uma cópia local do arquivo de alias de imagem para que ele possa ser acessado em um ambiente de rede restrita.
* `az vmss create`: foi adicionado `--orchestration-mode` para especificar como as máquinas virtuais são gerenciadas pelo conjunto de dimensionamento.
* `az vm/vmss update`: foi adicionado `--ultra-ssd-enabled` para permitir a atualização da configuração de SSD Ultra.
* [ALTERAÇÃO DA FALHA] `az vm extension set`: foi corrigido o bug em que os usuários não podiam definir uma extensão em uma VM com `--ids`.
* Foram adicionados os novos comandos `az vm image terms accept/cancel/show` para gerenciar os termos de imagem do Azure Marketplace.
* O VMAccessForLinux foi atualizado para a versão 1.5

### <a name="cosmosdb"></a>CosmosDB

* [ALTERAÇÃO DA FALHA] `az sql container create`: `--partition-key-path` foi alterado para parâmetro obrigatório
* [ALTERAÇÃO DA FALHA] `az gremlin graph create`: `--partition-key-path` foi alterado para parâmetro obrigatório
* `az sql container create`: Adição de `--unique-key-policy` e `--conflict-resolution-policy`
* `az sql container create/update`: o esquema padrão `--idx` foi atualizado
* `gremlin graph create`: Adicionado `--conflict-resolution-policy`
* `gremlin graph create/update`: o esquema padrão `--idx` foi atualizado
* Erro de digitação corrigido na mensagem de ajuda
* banco de dados: Foram adicionadas informações sobre preteridos
* coleção: Foram adicionadas informações sobre preteridos

### <a name="iot"></a>IoT

* Um novo tipo de fonte de roteamento foi adicionado: DigitalTwinChangeEvents
* Foi corrigido o erro de recursos ausentes no `az iot hub create`

### <a name="key-vault"></a>Key Vault

* Foi corrigido um erro inesperado quando o arquivo de certificado não existe
* Foi corrigido o problema em que o `az keyvault recover/purge` não funcionava

### <a name="netappfiles"></a>NetAppFiles

* O azure-mgmt-netapp foi atualizado para 0.6.0 para usar a versão da API 2019-07-01. Essa nova versão da API inclui:

    - A criação de volume `--protocol-types` agora aceita "NFSv4.1" não "NFSv4"
    - A propriedade da política de exportação de volume agora é chamada 'nfsv41' não 'nfsv4'
    - O volume `--creation-token` foi renomeado para `--file-path`
    - A data de criação do instantâneo agora é chamada apenas de 'criação'

### <a name="network"></a>Rede

* `az network private-dns link vnet create/update`: suporte à vinculação de rede virtual entre locatários.
* [ALTERAÇÃO DA FALHA] `az network vnet subnet list`: `--resource-group` e `--vnet-name` foram alterados para serem obrigatórios agora.
* `az network public-ip prefix create`: Suporte adicionado para especificar a versão do endereço IP (IPv4, IPv6) durante a criação
* O azure-mgmt-network foi atualizado para 7.0.0 e a api-version para 2019-09-01
* `az network vrouter`: Suporte adicionado para o novo roteador virtual de serviço e o emparelhamento do roteador virtual
* `az network express-route gateway connection`: Adicionado o suporte para `--internet-security`

### <a name="profile"></a>Perfil

* Foi corrigido o problema em que o `az account get-access-token --resource-type ms-graph` não funcionava
* O aviso foi removido de `az login`

### <a name="rbac"></a>RBAC

* Foi corrigido o problema em que o `az ad app update --id {} --display-name {}` não funcionava

### <a name="servicefabric"></a>ServiceFabric

* `az sf cluster create`: foi corrigido um problema que ocorria ao modificar o VMSS de computação do template.json do Linux e do Windows, do Service Fabric, de discos Standard para discos gerenciados

### <a name="sql"></a>SQL

* Os parâmetros `--compute-model`, `--auto-pause-delay` e `--min-capacity` foram adicionados para dar suporte a operações CRUD para a nova oferta de Banco de Dados SQL: Modelo de computação sem servidor.

### <a name="storage"></a>Armazenamento

* `az storage account create/update`: Foram adicionados o parâmetro --enable-files-adds e o grupo Argumentos de Propriedades do Azure Active Directory para dar suporte à Autenticação do Serviço de Domínio do Active Directory do Arquivos do Azure
* O `az storage account keys list/renew` foi expandido para dar suporte à listagem ou à regeneração de chaves Kerberos da conta de armazenamento.

## <a name="october-15-2019"></a>15 de outubro de 2019

Versão 2.0.75

### <a name="aks"></a>AKS

* Alteração do valor padrão `--load-balancer-sku` para `standard` se for compatível com a versão do Kubernetes
* Alteração do valor padrão `--vm-set-type` para `virtualmachinescalesets` se for compatível com a versão do Kubernetes

### <a name="ams"></a>AMS

* [ALTERAÇÃO SIGNIFICATIVA] Alteração do nome de `job start` para `job create`
* [ALTERAÇÃO SIGNIFICATIVA] Alteração do parâmetro `--ask` de `content-key-policy create` para usar uma cadeia de 32 caracteres hexadecimais em vez do UTF8

### <a name="appservice"></a>AppService

* Adição dos comandos `webapp config access-restriction show|set|add|remove`
* Adição de um melhor tratamento de erro a `webapp up`
* Adição de suporte do SKU `Isolated` para `appservice plan update`

### <a name="arm"></a>ARM

* Adição do parâmetro `--handle-extended-json-format``deployment create` para dar suporte a várias linhas e a comentários no modelo json

### <a name="compute"></a>Computação

* Parâmetro `--enable-agent` adicionado a `vm create`
* Alteração de `vm create` para usar um SKU de IP público padrão automaticamente ao usar zonas
* Alteração de `vm create` para criar automaticamente um nome de computador válido para uma VM, caso nenhum tenha sido fornecido
* Adição do parâmetro `--computer-name-prefix` a `vmss create` para dar suporte ao prefixo de nome de computador personalizado de máquinas virtuais no VMSS
* Adicione o parâmetro `--workspace` a `vm create` para habilitar o workspace de análise de logs automaticamente
* Versão de API de galerias atualizadas para 2019-07-01

### <a name="core"></a>Núcleo

* Adição da verificação de sintaxe para o parâmetro `--set` no comando de atualização genérica

### <a name="iot"></a>IoT

* Correção de um problema em que o `iot hub show` retornaria incorretamente um erro com "recurso não encontrado"

### <a name="monitor"></a>Monitoramento

* Adição de suporte para CRUD a `monitor log-analytics workspace`

### <a name="network"></a>Rede

* Adição de suporte para vinculação virtual entre locatários para `network private-dns link vnet [create|update]`
* [ALTERAÇÃO SIGNIFICATIVA] Alteração de `network vnet subnet list` para exigir os parâmetros `--resource-group` e `--vnet-name`

### <a name="sql"></a>SQL

* Adição de comandos a `sql mi ad-admin` que dão suporte à configuração de um administrador do AAD em instâncias gerenciadas

### <a name="storage"></a>Armazenamento

* Adição do parâmetro `--preserve-s2s-access-tier``storage copy` para preservar a camada de acesso durante a cópia do serviço para serviço
* Adição do parâmetro `--enable-large-file-share` a `storage account [create|update]` para dar suporte a compartilhamentos de arquivos grandes para a conta de armazenamento

## <a name="september-24-2019"></a>24 de setembro de 2019

Versão 2.0.74

### <a name="acr"></a>ACR

* Inclusão de um parâmetro `--type` obrigatório em `acr config retention update`
* [ALTERAÇÃO SIGNIFICATIVA] O parâmetro renomeado `--name -n` foi alterado para `--registry -r ` para o grupo de comando `acr config`

### <a name="aks"></a>AKS

* Inclusão do parâmetro `--load-balancer-sku` no comando `aks create`, o que permite criar um cluster do AKS com SLB
* Inclusão dos parâmetros `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` e `--load-balancer-outbound-ip-prefixes` nos comandos `aks [create|update]`, o que permite atualizar o perfil do balanceador de carga de um cluster do AKS com SLB
* Inclusão do parâmetro `--vm-set-type` no comando `aks create`, o que permite especificar os tipos de VM de um cluster do AKS (vmas ou vmss)

### <a name="arm"></a>ARM

* Inclusão do parâmetro `--handle-extended-json-format` no comando `group deployment create` para compatibilidade com várias linhas e comentários no modelo JSON

### <a name="compute"></a>Computação

* Inclusão do parâmetro `--terminate-notification-time` nos comandos `vmss [create|update]` para compatibilidade com a capacidade de configurar o encerramento de eventos agendados
* Inclusão do parâmetro `--enable-terminate-notification` no comando `vmss update` para compatibilidade com a capacidade de configurar o encerramento de eventos agendados
* Inclusão dos parâmetros `--priority,`, `--eviction-policy,` e `--max-billing` nos comandos `[vm|vmss] create`
* Alteração de `disk create` para permitir a especificação do tamanho exato do carregamento de disco
* Inclusão de compatibilidade com instantâneos incrementais para discos gerenciados para `snapshot create`

### <a name="cosmos-db"></a>Cosmos DB

* Inclusão do parâmetro `--type <key-type>` no comando `cosmosdb keys list` para mostrar a chave, as chaves somente leitura ou cadeias de conexão
* Adicionado o comando `cosmosdb keys regenerate`
* [PRETERIDO] Comandos `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` e `cosmosdb list-read-only-keys` preteridos

### <a name="eventgrid"></a>EventGrid

* Correção do texto de ajuda do ponto de extremidade para fazer referência ao parâmetro correto

### <a name="key-vault"></a>Key Vault

* Correção do problema em que fazer logon com um locatário (`login -t`) poderia causar uma falha no `keyvault create`

### <a name="monitor"></a>Monitoramento

* Correção do problema em que o caractere `:` não era permitido no argumento `--condition` para `monitor metrics alert create`

### <a name="policy"></a>Política

* Inclusão de compatibilidade com a API de Política, versão de 01/06/2019
* Inclusão do parâmetro `--enforcement-mode` no comando `policy assignment create`

### <a name="storage"></a>Armazenamento

* Inclusão do parâmetro `--blob-type` no comando `az storage copy`

## <a name="september-10-2019"></a>10 de setembro de 2019

### <a name="acr"></a>ACR

* Adição do grupo de comandos `acr config retention` para configurar a política de retenção

### <a name="aks"></a>AKS

* Adição de suporte para integração do ACR com os seguintes comandos:
  * Adição do parâmetro `--attach-acr` a `aks [create|update]` para anexar um ACR a um cluster do AKS
  * Adição do parâmetro `--detach-acr` a `aks update` para desanexar o ACR de um cluster do AKS

### <a name="arm"></a>ARM

* Atualização para uso da versão de API 2019-05-10

### <a name="batch"></a>Lote

* Adição de novas definições de configuração JSON de `--json-file` para `batch pool create`:
  * Adição de `MountConfigurations` para montagens do sistema de arquivos (confira https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body para obter detalhes)
  * Adição da propriedade opcional `publicIPs` a `NetworkConfiguration` para IPs públicos em pools (confira https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body para obter detalhes)
* Adição de suporte para galerias de imagens compartilhadas a `--image`
* [ALTERAÇÃO SIGNIFICATIVA] Alteração do valor padrão de `--start-task-wait-for-success` em `batch pool create` para `true`
* [ALTERAÇÃO SIGNIFICATIVA] Alteração do valor padrão de `Scope` em `AutoUserSpecification` para sempre ser Pool (anteriormente, `Task` em nós do Windows e `Pool` em nós do Linux)
  * Esse argumento só pode ser definido em uma configuração JSON com `--json-file`

### <a name="hdinsight"></a>HDInsight

* Versão de GA
* [ALTERAÇÃO SIGNIFICATIVA] Alteração do parâmetro `--workernode-count/-c` de `az hdinsight resize` para ser obrigatório.

### <a name="key-vault"></a>Key Vault

* Correção do problema em que as sub-redes não podiam ser excluídas das regras da rede
* Correção do problema em que sub-redes e endereços IP duplicados podiam ser adicionados às regras da rede

### <a name="network"></a>Rede

* Adição do parâmetro `--interval` a `network watcher flow-log` para definir o valor do intervalo de análise de tráfego
* Adição de `network application-gateway identity` para gerenciar a identidade do gateway
* Adição de suporte para definir a ID do Key Vault como `network application-gateway ssl-cert`
* Adicionado `network express-route peering peer-connection [show|list]`

### <a name="policy"></a>Política

* Atualização para uso da versão de API 2019-01-01

## <a name="august-27-2019"></a>27 de agosto de 2019

Versão 2.0.72

### <a name="acr"></a>ACR

* [ALTERAÇÃO SIGNIFICATIVA] Remoção da compatibilidade com o SKU `classic`

### <a name="api-management"></a>Gerenciamento de API

* [VERSÃO PRÉVIA] Adição do grupo de comandos `apim`

### <a name="appservice"></a>AppService

* Correção do problema com o comando `webapp webjob continuous start` ao especificar um slot
* Alteração de `webapp up` para detectar a pasta `env` e removê-la do arquivo usado para implantação

### <a name="keyvault"></a>Keyvault

* Correção de um bug no `keyvault secret set` que ignorava o argumento `--expires`

### <a name="network"></a>Rede

* Adição de suporte para endereços IPv6 a argumentos `--private-ip-address-version`
* Adição de novos comandos `network private-endpoint [create|update|list-types]` para o gerenciamento de ponto de extremidade privado
* Adição do grupo de comandos `network private-link-service`
* Adicionados os argumentos `--private-endpoint-network-policies` e `--private-link-service-network-policies` para `network vnet subnet update`

### <a name="rbac"></a>RBAC

* Correção de um problema com `ad app update --homepage` em que a página inicial não era atualizada

### <a name="servicefabric"></a>ServiceFabric

* Adição de suporte para nomes de Key Vault grafados com maiúsculas e minúsculas
* Correção de um problema ao usar certificados no Key Vault
* Correção de um problema com o uso de arquivos de certificado PFX
* Correção de um problema com `sf cluster certificate add` quando o grupo de recursos do Key Vault não era especificado
* Correção de um problema em que `sf cluster set` não funcionava

### <a name="signalr"></a>SignalR

* Novos comandos adicionados:
  * `signalr cors`: gerenciar CORS do SignalR
  * `signalr restart`: reiniciar um serviço do SignalR
  * `signalr update`: atualizar um serviço do SignalR
* Adicionado o argumento `--service-mode` para `signalr create`

### <a name="storage"></a>Armazenamento

* Adicionado o comando `storage account revoke-delegation-keys`

## <a name="august-13-2019"></a>13 de agosto de 2019

Versão 2.0.71

### <a name="appservice"></a>AppService

* Um problema de falha de slots com os comandos `webapp webjob continuous` foi corrigido

### <a name="botservice"></a>BotService

* [ALTERAÇÃO SIGNIFICATIVA] O suporte para a criação de bots SDK v3 foi removido

### <a name="cognitiveservices"></a>CognitiveServices

* Adicionados os comandos `cognitiveservices account network-rule`

### <a name="cosmos-db"></a>Cosmos DB

* Removido o aviso ao atualizar vários locais de gravação
* Foram adicionados os comandos CRUD para o CosmosDB SQL, MongoDB, Cassandra, Gremlin e Recursos de tabela e taxa de transferência do recurso

### <a name="hdinsight"></a>HDInsight

Esta versão contém um grande número de alterações da falha.

* [ALTERAÇÃO SIGNIFICATIVA] Parâmetros renomeados para `hdinsight create`:
  * `--storage-default-container` renomeado para `--storage-container`
  * `--storage-default-filesystem` renomeado para `--storage-filesystem`
* [ALTERAÇÃO SIGNIFICATIVA] O argumento `--name` de `application create` foi alterado para representar o nome do aplicativo em vez do nome do cluster
* O argumento `--cluster-name` foi adicionado a `application create` para substituir a funcionalidade `--name` antiga
* [ALTERAÇÃO SIGNIFICATIVA] Parâmetros renomeados para `application create`:
  * `--application-type` renomeado para `--type`
  * `--marketplace-identifier` renomeado para `--marketplace-id`
  * `--https-endpoint-access-mode` renomeado para `--access-mode`
  * Renomeado de `--https-endpoint-destination-port` para `--destination-port`
* [ALTERAÇÃO SIGNIFICATIVA] Parâmetros removidos para `application create`:
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* [ALTERAÇÃO DA FALHA] Renomeado de `--target-instance-count` para `--workernode-count` para `hdinsight resize`
* [ALTERAÇÃO SIGNIFICATIVA] Todos os comandos no grupo `hdinsight script-action` foram alterados para usar o parâmetro `--name` como o nome da ação de script.
* O argumento `--cluster-name` foi adicionado a todos os comandos `hdinsight script-action` para substituir a funcionalidade `--name` antiga
* [ALTERAÇÃO SIGNIFICATIVA] Renomeado de `--script-execution-id` para `--execution-id` para todos os comandos `hdinsight script-action`
* [ALTERAÇÃO SIGNIFICATIVA]`hdinsight script-action show` renomeado para `hdinsight script-action show-execution-details`
* [ALTERAÇÃO DA FALHA] Os parâmetros foram alterados para `hdinsight script-action execute --roles` para serem separados por espaços em vez de separados por vírgula
* [ALTERAÇÃO SIGNIFICATIVA] O parâmetro `--persisted` de `hdinsight script-action list` foi removido
* O parâmetro `hdinsight create --cluster-configurations` foi alterado para aceitar um caminho para um arquivo JSON local ou uma cadeia de caracteres JSON
* Adicionado o comando `hdinsight script-action list-execution-history`
* Alterado `hdinsight monitor enable --workspace` para aceitar uma ID do workspace ou nome do workspace do Log Analytics
* O argumento `hdinsight monitor enable --primary-key`, que será necessário caso uma ID do workspace seja fornecida como o parâmetro, foi adicionado
* Foram adicionados mais exemplos e atualização das descrições das mensagens de erro

### <a name="interactive"></a>Interativo

* Um erro no carregamento foi corrigido

### <a name="kubernetes"></a>Kubernetes

* Alterado para usar `https` se a porta do contêiner do painel estiver usando `https`

### <a name="network"></a>Rede

* O argumento `--yes` foi adicionado a `network dns record-set cname delete`

### <a name="profile"></a>Perfil

* O argumento `--resource-type` foi adicionado a `account get-access-token` para obter tokens de acesso de recurso

### <a name="servicefabric"></a>ServiceFabric

* Todas as versões de sistema operacional com suporte para criação do cluster sf foram adicionadas
* Foi corrigido o bug de validação do certificado primário

### <a name="storage"></a>Armazenamento

* Adicionado o comando `storage copy`

## <a name="july-30-2019"></a>30 de julho de 2019

Versão 2.0.70

### <a name="acr"></a>ACR

* Corrigido o problema #9952 (uma regressão no comando `acr pack build`)
* Removido o nome da imagem do construtor padrão em `acr pack build`

### <a name="appservice"></a>AppService

* Alterado `webapp config ssl` para mostrar uma mensagem se um recurso não for encontrado
* Corrigido o problema em que `functionapp create` não aceita o tipo de conta de armazenamento `Standard_RAGRS`
* Corrigido um problema em que `webapp up` falharia se fosse executado usando versões mais antigas do Python

### <a name="network"></a>Rede

* Removido parâmetro inválido `--ids` de `network nic ip-config add` (corrige o #9861)
* Corrige o #9604. Adicionado o parâmetro `--root-certs` ao `network application-gateway http-settings [create|update]` para dar suporte a certificados raiz confiáveis associados ao usuário.
* Fixado argumento `--subscription` para `network dns record-set ns create` (#9965)

### <a name="rbac"></a>RBAC

* Adicionado o comando `user update`
* [PRETERIDO] Preterido `--upn-or-object-id` de comandos relacionados ao usuário
    * Usar argumento de substituição `--id`
* Adicionado argumento `--id` para comandos relacionados ao usuário

### <a name="sql"></a>SQL

* Adicionados comandos de gerenciamento para chaves de instância gerenciada e protetor de TDE

### <a name="storage"></a>Armazenamento

* Adicionado o comando `storage remove`
* Corrigido um problema com `storage blob update`

### <a name="vm"></a>VM

* Alterado `list-skus` para usar versão de API mais recente a fim de externar detalhes de zona
* Alterado o padrão de `--single-placement-group` para `false` para `vmss create`
* Adicionada a capacidade de selecionar SKUs de armazenamento ZRS para `[snapshot|disk] create`
* Adicionado novo grupo de comandos `vm host` para dar suporte a hosts dedicados
* Adicionados parâmetros `--host` e `--host-group` em `vm create` para definir o host dedicado da VM

## <a name="july-16-2019"></a>16 de julho de 2019

Versão 2.0.69

### <a name="appservice"></a>AppService

* Os comandos `webapp identity` foram alterados para retornar uma mensagem de erro apropriada se o nome do aplicativo ou ResourceGroupName for inválido
* `webapp list` corrigido para retornar o valor correto para numberOfSites se nenhum ResourceGroup foi fornecido
* Corrigidos os efeitos colaterais de `appservice plan create` e `webapp create`

### <a name="core"></a>Núcleo

* Corrigido um problema em que `--subscription` aparecia apesar de não ser aplicável

### <a name="batch"></a>Lote

* [ALTERAÇÃO SIGNIFICATIVA]`batch pool node-agent-skus list` foi substituído por `batch pool supported-images list`
* Adicionado suporte para regras de segurança bloqueando o acesso de rede a um pool com base na porta de origem do tráfego ao usar a opção `--json-file` de `batch pool create network`
* Suporte adicionado para executar a tarefa no diretório de trabalho de contêiner ou no diretório de trabalho de tarefa em lotes ao usar a opção `--json-file` de `batch task create`
* Corrigido o erro na opção `--application-package-references` de `batch pool create` em que ela funcionaria apenas com padrões

### <a name="eventhubs"></a>Hubs de eventos

* Adicionada validação para o parâmetro `--rights` dos comandos `authorizationrule`

### <a name="rdbms"></a>RDBMS

* Adicionado um parâmetro opcional para especificar a réplica de SKU para criar o comando de réplica
* Corrigido o problema com a falha no teste de CI com a criação de réplica de MySQL

### <a name="relay"></a>Retransmissão

* Corrigido o problema com a conexão híbrida quando a autorização do cliente desabilitava [#8775](https://github.com/azure/azure-cli/issues/8775)
* Parâmetro `--requires-transport-security` adicionado a `relay wcfrelay create`

### <a name="servicebus"></a>Barramento de serviço

* Adicionada validação para o parâmetro `--rights` dos comandos `authorizationrule`

### <a name="storage"></a>Armazenamento

* Habilitar AADDS de arquivos para atualização da conta de armazenamento
* Problema corrigido `storage blob service-properties update --set`

## <a name="july-2-2019"></a>2 de julho de 2019

Versão 2.0.68

### <a name="core"></a>Núcleo

* Agora, os módulos de comando são consolidados em um único Python distribuível. Isso substitui o uso direto de muitos pacotes `azure-cli-` no PyPI.
  Assim, o tamanho da instalação será reduzido e apenas os usuários que tiverem instalado diretamente por meio do `pip` serão afetados.

### <a name="acr"></a>ACR

* Foi adicionado o suporte para gatilhos de temporizador para tarefa

### <a name="appservice"></a>AppService

* O `functionapp create` foi alterado para habilitar o Application Insights por padrão
* [ALTERAÇÃO SIGNIFICATIVA] Foi removido o comando `functionapp devops-build` preterido.
  *  Agora, use o novo comando `az functionapp devops-pipeline`
* Foi adicionado o suporte ao plano de aplicativo de funções Consumo em Linux ao `functionapp deployment config-zip`

### <a name="cosmos-db"></a>Cosmos DB

* Foi adicionado o suporte para desabilitar a TTL

### <a name="dls"></a>DLS

* Versão atualizada do ADLS (0.0.45)

### <a name="feedback"></a>Comentários

* Ao relatar um comando de extensão com falha, agora, o `az feedback` tenta abrir o navegador na URL do projeto/repositório da extensão por meio do índice

### <a name="hdinsight"></a>HDInsight

* [ALTERAÇÃO SIGNIFICATIVA] O nome do grupo de comandos `oms` foi alterado para `monitor`
* [ALTERAÇÃO SIGNIFICATIVA]`--http-password/-p` tornou-se um parâmetro obrigatório 
* Foram adicionados preenchedores para o preenchedor dos parâmetros `--cluster-admin-account` e `cluster-users-group-dns` 
* O parâmetro `cluster-users-group-dns` foi alterado para ser obrigatório quando `—esp` estiver presente
* Foi adicionado um tempo limite para todos os preenchedores automáticos de argumento existentes
* Foi adicionado um tempo limite para transformar o nome do recurso na ID de recurso
* Os preenchedores automáticos foram alterados para selecionar recursos de qualquer grupo de recursos. Pode ser um grupo de recursos diferente daquele especificado com `-g`
* Foi adicionado o suporte para os parâmetros `--sub-domain-suffix` e `--disable_gateway_auth` no comando `hdinsight application create`

### <a name="managed-services"></a>Serviços gerenciados

* Introdução ao módulo de comando de serviço gerenciado em versão prévia

### <a name="profile"></a>Perfil
* Suprimir o argumento `--subscription` para o comando de logoff

### <a name="rbac"></a>RBAC

* [ALTERAÇÃO SIGNIFICATIVA] O argumento `--password` foi removido de `create-for-rbac`
* Foi adicionado o parâmetro `--assignee-principal-type` ao comando `create` para evitar falhas intermitentes causadas pela latência de replicação do servidor do AAD Graph
* Foi corrigida uma falha em `ad signed-in-user` ao listar objetos de propriedade
* Foi corrigido um problema em que o `ad sp` não localizava o aplicativo certo de uma entidade de serviço

### <a name="rdbms"></a>RDBMS

* Foi adicionado o suporte à replicação para o MariaDB

### <a name="sql"></a>SQL

* Valores permitidos documentados para `sql db create --sample-name`

### <a name="storage"></a>Armazenamento

* Foi adicionado o suporte ao token SAS de delegação de usuário com `--as-user` para `storage blob generate-sas` 
* Foi adicionado o suporte ao token SAS de delegação de usuário com `--as-user` para `storage container generate-sas` 

### <a name="vm"></a>VM

* Foi corrigido o bug em que o `vmss create` retornava uma mensagem de erro quando era executado com `--no-wait`
* Foi removida a validação do lado do cliente de `vmss create --single-placement-group`. Não falha quando `--single-placement-group` é definido como `true` e `--instance-count` é maior que 100 ou quando são especificadas zonas de disponibilidade, mas deixa essa validação para o serviço de computação
* Foi corrigido o bug em que o `[vm|vmss] extension image list` falhava quando era usado com `--latest`


## <a name="june-18-2019"></a>18 de junho de 2019

Versão 2.0.67

### <a name="core"></a>Núcleo

Esta versão apresenta uma nova marca [Versão prévia] para comunicar com mais clareza aos clientes quando um comando, um grupo de comandos ou um argumento está no status de versão prévia. Anteriormente, essa informação era transmitida no texto de ajuda ou, implicitamente, pelo número da versão do módulo de comando.
A CLI removerá os números de versão dos pacotes individuais no futuro. Se um comando estiver em versão prévia, todos os seus argumentos também estarão. Se um grupo de comandos for rotulado com o status de versão prévia, então todos os seus comandos e argumentos também serão considerados em versão prévia.

Como resultado dessa alteração, diversos grupos de comandos podem parecer surgir "de repente" com o status de versão prévia com esta liberação. O que realmente aconteceu é que a maioria dos pacotes já estava com status de versão prévia, mas estão sendo consideradas GA com esta liberação

### <a name="acr"></a>ACR
* Adicionado o comando 'acr check-health'
* Melhorado o tratamento de erro para tokens do AAD e para recuperar comandos externos

### <a name="acs"></a>ACS
* Comandos preteridos do ACS agora ficam ocultos da exibição da ajuda

### <a name="ams"></a>AMS
* [ALTERAÇÃO SIGNIFICATIVA] Alterada para retornar cadeias de caracteres de tempo da ISO 8601 para archive-window-length e key-frame-interval-duration

### <a name="appservice"></a>AppService
* Adicionado roteamento com base no local para `webapp deleted list` e `webapp deleted restore`
* Corrigido problema em que a URL de destino registrada do webapp ("Não é possível iniciar o aplicativo em...") não era clicável no Azure Cloud Shell
* Corrigido um problema em que a criação de aplicativos com algumas SKUs falhava com um erro de AlwaysOn
* Adicionada a pré-validação para o `[appservice|webapp] create`
* Corrigido o `[webapp|functionapp] traffic-routing` para usar o actionHostName correto
* Adicionado o suporte de slot para comandos `functionapp`

### <a name="batch"></a>Lote
* Corrigida a regressão de autenticação do AAD causada pela geração de relatórios de erros superagressiva para autenticação de chave compartilhada

### <a name="batchai"></a>BatchAI
* Agora os comandos do BatchAI estão preteridos e ocultos

### <a name="botservice"></a>BotService
* Adição das mensagens de aviso "suporte descontinuado"/"modo de manutenção" para os comandos compatíveis com a v3 do SDK

### <a name="cosmosdb"></a>CosmosDB
* [PRETERIDO] Preterido o comando `cosmosdb list-keys`
* Adicionado o comando `cosmosdb keys list` – substitui o `cosmosdb list-keys`
* `cosmsodb create/update`: Adicionado novo formato para --location a fim de permitir a configuração da propriedade "isZoneRedundant". Formato antigo preterido

### <a name="eventgrid"></a>EventGrid
* Adicionados comandos do `eventgrid domain` para operações de CRUD no domínio
* Adicionados comandos do `eventgrid domain topic` para operações de CRUD nos tópicos do domínio
* Adicionado argumento do `--odata-query` ao `eventgrid [topic|event-subscription] list` para filtrar os resultados usando a sintaxe do OData
* `event-subscription create/update`: Adicionado o servicebusqueue como novos valores para o parâmetro `--endpoint-type`
* [ALTERAÇÃO SIGNIFICATIVA] Removido o suporte para `--included-event-types All` com `eventgrid event-subscription [create|update]`

### <a name="hdinsight"></a>HDInsight
* Adicionado suporte para o parâmetro `--ssh-public-key` no comando `hdinsight create`

### <a name="iot"></a>IoT
* Adicionado suporte para regenerar as chaves da política de autorização
* Adicionados SDK e suporte para o serviço de provisionamento de repositórios do DigitalTwin

### <a name="network"></a>Rede
* Adicionado suporte de zona para o Gateway da NAT
* Adicionado o comando `network list-service-tags`
* Corrigido o problema com o `dns zone import` em que os usuários não conseguiam importar registros do curinga A
* Corrigido o problema com o `watcher flow-log configure` em que o registro de fluxo não podia ser habilitado em determinadas regiões

### <a name="resource"></a>Recurso
* Adicionado o comando do `az rest` para fazer chamadas REST
* Corrigido o erro ao usar o `policy assignment list` com um grupo de recursos ou o nível de assinatura `--scope`

### <a name="servicebus"></a>ServiceBus
* Corrigido o problema com o `servicebus topic create --max-size`[nº9319](https://github.com/azure/azure-cli/issues/9319)

### <a name="sql"></a>SQL
* Alterado o `--location` para ser opcional para `sql [server|mi] create` – usa o local do grupo de recursos se não especificado
* Corrigido o erro "objeto 'NoneType' não é iterável" para `sql db list-editions --available`

### <a name="sqlvm"></a>SQLVm
* [ALTERAÇÃO DA FALHA] Alterado `sql vm create` para exigir o parâmetro `--license-type`
* Alterado para permitir a configuração da SKU da imagem do SQL ao criar ou atualizar uma VM do SQL

### <a name="storage"></a>Armazenamento
* Corrigido o problema com a chave de conta ignorada para `storage container generate-sas`
* Corrigido o problema com o `storage blob sync` no Linux

### <a name="vm"></a>VM
* [VERSÃO PRÉVIA] Adicionados os comandos `vm image template` para criar imagens de VM

## <a name="june-4-2019"></a>4 de junho de 2019

Versão 2.0.66

### <a name="core"></a>Núcleo
* Foi corrigido o bug em que os comandos falhavam quando `--output yaml` era usado com `--query`

### <a name="acr"></a>ACR
* Foi adicionado o grupo de comando 'pack acr' para a criação de Tarefas de build rápida usando Buildpacks.

### <a name="acs"></a>ACS
* Permitir a opção de habilitar/desabilitar o complemento kube-dashboard do AKS
* Imprimir uma mensagem amigável quando a assinatura não estiver na lista de permissões para usar o Red Hat OpenShift no Azure

### <a name="batch"></a>Lote
* Melhoria no tratamento de erro quando você não está conectado a uma conta \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]

### <a name="iot"></a>IoT
* Foi adicionado o suporte para failover manual

### <a name="network"></a>Rede
* Foram adicionados os comandos `network application-gateway waf-policy` para oferecer suporte às regras de WAF personalizadas.
* Adicionados os argumentos `--waf-policy` e `--max-capacity` para `network application-gateway [create|update]` 

### <a name="resource"></a>Recurso
* Melhoria da mensagem de erro do `deployment create` quando não há nenhum TTY disponível

### <a name="role"></a>Função
* O texto da Ajuda foi atualizado.

### <a name="compute"></a>Computação
* Foi adicionado o suporte para `vm create` para as VMs de uma imagem gerenciada com LUNs de disco de dados que não começam em 0 ou que ignoram números

## <a name="may-21-2019"></a>21 de maio de 2019

Versão 2.0.65

### <a name="core"></a>Núcleo
* Foram adicionados comentários melhores para erros de autenticação
* Corrigido um problema em que a CLI carregava extensões que não eram compatíveis com a versão do núcleo
* Corrigido um problema com a inicialização quando `clouds.config` está corrompido

### <a name="acr"></a>ACR
* Foi adicionado suporte das Identidades Gerenciadas para Tarefas

### <a name="acs"></a>ACS
* Corrigido o comando `openshift create` quando usado com o cliente AAD do consumidor

### <a name="appservice"></a>AppService
* [PRETERIDO] Preterido o comando `functionapp devops-build` – Será removido na próxima versão
* `functionapp devops-pipeline` foi alterado para buscar o log de build do Azure DevOps no modo detalhado
* [ALTERAÇÃO SIGNIFICATIVA] O sinalizador `--use_local_settings` foi removido do comando `functionapp devops-pipeline` – não estava operacional
* `webapp up` foi alterado para retornar uma saída JSON se `--logs` não for usado
* Foi adicionado suporte para escrever recursos padrão para a configuração local de `webapp up`
* Foi adicionado suporte para `webapp up` reimplantar um aplicativo sem usar o argumento `--location`
* Corrigido um problema em que o valor do SKU gratuito não funcionava na criação do ASP do SKU gratuito do Linux

### <a name="botservice"></a>BotService
* Alterado para permitir todas as capitalizações para parâmetros `--lang` em todos os comandos
* Descrição atualizada do módulo de comando

### <a name="consumption"></a>Consumo
* O parâmetro obrigatório ausente foi adicionado para executar `consumption usage list --billing-period-name`

### <a name="iot"></a>IoT
* Suporte adicionado para listar todas as chaves

### <a name="network"></a>Rede
* [ALTERAÇÃO SIGNIFICATIVA]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* O argumento `--nat-gateway` foi adicionado a `network vnet subnet [create|update]` para anexar a um gateway NAT
* Corrigido o problema de `dns zone import`, em que os nomes de registro não correspondiam ao tipo de registro

### <a name="rdbms"></a>RDBMS
* Suporte a postgres e mysql adicionado para replicação geográfica

### <a name="rbac"></a>RBAC
* Adição de suporte do escopo de grupo de gerenciamento a `role assignment`

### <a name="storage"></a>Armazenamento
* `storage blob sync`: adicionar um comando de sincronização ao armazenamento de blobs

### <a name="compute"></a>Computação
* `--computer-name` foi adicionado a `vm create` para configurar o nome do computador da VM
* `--ssh-key-value` foi renomeado para `--ssh-key-values` para `[vm|vmss] create` – Agora, pode aceitar vários valores de chave pública ou caminhos ssh
  * __Observação__: Isso **não** é uma alteração da falha – `--ssh-key-value` será analisado corretamente, pois corresponde somente a `--ssh-key-values`
* O argumento `--type` de `ppg create` foi alterado para ser opcional

## <a name="may-6-2019"></a>6 de maio de 2019

Versão 2.0.64

### <a name="acs"></a>ACS
* [ALTERAÇÃO SIGNIFICATIVA] O sinalizador `--fqdn` foi removido dos comandos `openshift`
* Alterado para usar a versão da API do Red Hat OpenShift no Azure em disponibilidade geral
* O sinalizador `customer-admin-group-id` foi adicionado a `openshift create`
* [GA] `(PREVIEW)` foi removido da opção `aks create``--network-policy`

### <a name="appservice"></a>AppService
* [PRETERIDO] O comando `functionapp devops-build` foi preterido
  * Renomeado para `functionapp devops-pipeline`
* Corrigido ao obter o nome de usuário correto para cloudshell que estava causando a falha em `webapp up`
* Documentação `appservice plan --sku` atualizada para refletir o appserviceplans com suporte
* Adicionado argumentos opcionais para o grupo de recursos e plano a `webapp up`
* Adicionado suporte a `webapp ssh` para respeitar a variável de ambiente `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`
* Adicionado suporte `appserviceplan create` para a SKU gratuita do Linux
* Alterado `webapp up` para ter uma suspensão de 30 segundos depois de definir appsetting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` para lidar com a inicialização a frio kudu
* Adicionado suporte para runtime `powershell` a `functionapp create` no Windows
* Adicionado o comando `create-remote-connection`

### <a name="batch"></a>Lote
* Corrigido o bug no validador para as opções `--application-package-references`

### <a name="botservice"></a>Serviço de bot
* [ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v4 -k webapp` foi alterado para criar um Bot de Aplicativo Web vazio por padrão (ou seja, nenhum bot será implantado no Serviço de Aplicativo)
* O sinalizador `--echo` foi adicionado ao `bot create` para usar o comportamento antigo com `-v v4`
* [ALTERAÇÃO SIGNIFICATIVA] O valor padrão de `--version` foi alterado para `v4`
  * __OBSERVAÇÃO:__ `bot prepare-publish` ainda usa o padrão antigo
* [ALTERAÇÃO SIGNIFICATIVA]`--lang` foi alterado para não definir mais `Csharp` como padrão. Se o comando exigir `--lang` e ele não for fornecido, o comando será um erro
* [ALTERAÇÃO SIGNIFICATIVA] Os argumentos `--appid` e `--password` foram alterados para `bot create` ser obrigatório e agora podem ser criados por meio de `ad app create`
* Foi adicionada validação a `--appid` e `--password`
* [ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v4` foi alterado para não criar ou usar uma Conta de Armazenamento ou o Application Insights
* [ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v3` foi alterado para exigir uma região em que o Application Insights está disponível
* [ALTERAÇÃO SIGNIFICATIVA] O `bot update` foi alterado para afetar somente as propriedades específicas de um bot
* [ALTERAÇÃO SIGNIFICATIVA] Os sinalizadores `--lang` foram alterados para aceitar `Javascript` em vez de `Node`
* [ALTERAÇÃO SIGNIFICATIVA] O `Node` foi removido como um valor `--lang` permitido
* [ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v4 -k webapp` foi alterado para não definir mais `SCM_DO_BUILD_DURING_DEPLOYMENT` como verdadeiro. Todas as implantações por meio do Kudu atuarão de acordo com o comportamento padrão
* O `bot download` foi alterado para os bots sem arquivos `.bot` para criar o arquivo de configuração específico a um idioma com os valores das Configurações de Aplicativo do bot
* Adicionado o suporte `Typescript` para `bot prepare-deploy`
* Uma mensagem de aviso foi adicionada a `bot prepare-deploy` para os bots `Javascript` e `Typescript` para quando `--code-dir` não contiver `package.json`
* O `bot prepare-deploy` foi alterado para retornar `true`, se bem-sucedido
* O log detalhado foi adicionado a `bot prepare-deploy`
* Mais regiões disponíveis do Application Insights foram adicionadas ao `az bot create -v v3`

### <a name="configure"></a>Configurar
* Adicionado suporte para configurações de valor padrão do argumento baseado em pasta

### <a name="eventhubs"></a>Hubs de eventos
* Adicionados os comandos `namespace network-rule`
* O argumento `--default-action` foi adicionado às regras de rede de `namespace [create|update]`

### <a name="network"></a>Rede
* [ALTERAÇÃO SIGNIFICATIVA] O argumento `--cache` foi substituído por `--defer` para `vnet [create|update]` 

### <a name="policy-insights"></a>Informações sobre a Política
* Suporte adicionado a `--expand PolicyEvaluationDetails` para detalhes de avaliação de política de consulta no recurso

### <a name="role"></a>Função
* [PRETERIDO] Alterado argumento ocultar '--password' `create-for-rbac` - suporte será removido em maio de 2019

### <a name="service-bus"></a>Barramento de Serviço
* Adicionados os comandos `namespace network-rule`
* O argumento `--default-action` foi adicionado às regras de rede de `namespace [create|update]`
* `topic [create|update]` foi fixado para permitir suporte a `--max-size` para valores de 10, 20, 40 e 80 GB com a SKU Premium

### <a name="sql"></a>SQL
* Adicionados os comandos `sql virtual-cluster [list|show|delete]`

### <a name="vm"></a>VM
* O `--protect-from-scale-in` e o `--protect-from-scale-set-actions` foram adicionados a `vmss update` para habilitar atualizações à política de proteção das instâncias de VM VMSS
* Adicionado a `--instance-id` e `vmss update` para habilitar atualização genérica das instâncias de VM VMSS
* `--instance-id` foi adicionado a `vmss wait`
* Adição do novo grupo de comandos `ppg` para gerenciar Grupos de Posicionamento de Proximidade
* Adicionado a `--ppg`, `[vm|vmss] create` e `vm availability-set create` para gerenciar PPGs
* Parâmetro `--hyper-v-generation` adicionado a `image create`

## <a name="april-23-2019"></a>23 de abril de 2019

Versão 2.0.63

### <a name="acs"></a>ACS
* Alterado `aks get-credentials` para solicitar substituição dos valores duplicados
* Removido `(PREVIEW)` dos comandos de espaços de desenvolvimento "aks use-dev-espaces" e "aks remove-dev-espaces"

### <a name="ams"></a>AMS
* Corrigido o bug com a atualização de filtros de conta e de ativo

### <a name="appservice"></a>AppService
* Adicionado suporte para o ASE e o tempo limite para `webapp ssh`
* Adicionado suporte para o estabelecimento de CI CD em um pipeline do Azure DevOps de um repositório do Github para aplicativos de funções
* Adicionado argumento `--github-pat` a `functionapp devops-build create` para aceitar o token de acesso pessoal do Github
* Adicionado argumento `--github-repository` a `functionapp devops-build create` para aceitar o repositório Github que contém um código-fonte functionapp
* Problema corrigido em que `az webapp up --logs` estava falhando com um erro e atualização da versão .NETCORE padrão para 2.1
* Configurações de functionapp desnecessárias removidas durante a criação de um aplicativo de funções com plano de consumo
* Alterado `webapp up` para que a cadeia de caracteres padrão asp agora acrescente o número no final para criar um novo ASP com base nas opções de SKU
* Adicionado `-b` como uma opção a `webapp up` para iniciar o aplicativo no navegador
* Alterado `webapp deployment source config zip` para lidar com a variável de ambiente `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`

### <a name="deployment-manager"></a>Gerenciador de Implantação
* [VERSÃO PRÉVIA] Criar e gerenciar artefatos que dão suporte a distribuições

### <a name="lab"></a>Laboratório
* Corrigido o bug que causa uma saída inicial

### <a name="network"></a>Rede
* Adicionada delegação de servidor de nome automática a `dns zone create` no pai durante a criação da zona filho

### <a name="resource"></a>Recurso
* [PRETERIDO] Argumentos `--link-id`, `--target-id` e `--filter-string` preteridos de `resource link`
  * Use os argumentos `--link`, `--target` e `--filter`
* Corrigido o problema em que os comandos `resource link [create|update]` não funcionavam
* Corrigido um problema em que a exclusão usando uma ID de recurso poderia causar falha no erro

### <a name="sql"></a>SQL
* Adicionado suporte para fuso horário personalizado nas instâncias gerenciadas
* Alterado para permitir que o nome do pool Elástico seja usado com `sql db update`
* Adicionado o suporte `--no-wait` para `sql server [create|update]`
* Adicionado o comando `sql server wait`

### <a name="storage"></a>Armazenamento
* Corrigido o problema com tokens SAS com codificação dupla em `storage blob generate-sas`

### <a name="vm"></a>VM
* Adicionado sinalizador `--skip-shutdown` a `vm|vmss stop` para desligar as VMs sem o desligamento
* Adicionado argumento `--storage-account-type` a `sig image-version create` para definir o tipo de conta do perfil de publicação
* Adicionado argumento `--target-regions` a `sig image-version create` para permitir definir os tipos de conta de armazenamento específico da região

## <a name="april-9-2019"></a>9 de abril de 2019

### <a name="core"></a>Núcleo
* Correção do problema em que algumas extensões mostraram uma versão do `Unknown` e não podiam ser atualizadas

### <a name="acr"></a>ACR
* Adição de suporte para execução de uma imagem sem contexto

### <a name="ams"></a>AMS
* [PRETERIDO]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [ALTERAÇÃO SIGNIFICATIVA]: Renamed the `--bitrate` parameter to `--first-quality`
* Adição de suporte para novos parâmetros de criptografia em `ams streaming-policy create`
* Adição de novo parâmetro `--filters` a `ams streaming-locator create`

### <a name="appservice"></a>AppService
* Adicionado o suporte `--logs` para `webapp up`
* Correção de problemas do comando `functionapp devops-build create` de geração de `azure-pipelines.yml`
* Melhoria do tratamento de erros e indicadores `unctionapp devops-build create`
* [ALTERAÇÃO SIGNIFICATIVA] Remoção do sinalizador `--local-git` para o comando `devops-build`; a detecção de git local e a manipulação são obrigatórias para a criação de pipelines do Azure DevOps
* Adição de suporte para a criação de planos de funções do Linux
* Adição da capacidade de trocar um plano sob um aplicativo de funções usando `functionapp update --plan`
* Adição de suporte para configurações de expansão de plano Premium do Azure Functions

### <a name="cdn"></a>CDN
* Adição de suporte para `Microsoft_Standard` e `Standard_ChinaCdn`

### <a name="feedback"></a>Comentários
* Alteração de `feedback` para mostrar metadados em comandos executados recentemente
* Alteração de `feedback` para solicitar o auxílio do usuário no processo de criação de problema abrindo um navegador e usando um modelo de problema
* Alteração do `feedback` para imprimir o corpo do problema ao executar com '--verbose'

### <a name="monitor"></a>Monitoramento
* Correção de um problema em que “count” não era um valor permitido com `metrics alert [create|update]` 

### <a name="network"></a>Rede
* Correção do formato de tabela que não estava sendo exibido com `vnet-gateway list-bgp-peer-status`
* Adição dos comandos `list-request-headers` e `list-response-headers` para `application-gateway rewrite-rule`
* Adição do comando `list-server-variables` para `application-gateway rewrite-rule condition`
* Correção de um problema em que a atualização do estado do link em uma porta express-route geraria uma exceção de atributo desconhecido `express-route port update`

### <a name="privatedns"></a>PrivateDNS
* Adição de `network private-dns` para zonas de DNS privado

### <a name="resource"></a>Recurso
* Correção do problema com `deployment create` e `group deployment create`, em que um arquivo de parâmetros com um conjunto vazio de parâmetros não funcionaria

### <a name="role"></a>Função
* Correção de `create-for-rbac` para lidar corretamente com `--years`
* [ALTERAÇÃO SIGNIFICATIVA] Alteração de `role assignment delete` para solicitar ao excluir todas as atribuições na assinatura incondicionalmente

### <a name="sql"></a>SQL
* Atualização de `sql mi [create|update]` com as propriedades proxyOverride e publicDataEndpointEnabled

### <a name="storage"></a>Armazenamento
* [ALTERAÇÃO SIGNIFICATIVA] Remoção do resultado de `storage blob delete`
* Adição de `--full-uri` a `storage blob generate-sas` para criar o URI completo para o blob com SAS
* Adição de `--file-snapshot` a `storage file copy start` para copiar arquivo do instantâneo
* Alteração de `storage blob copy cancel` para mostrar apenas o erro em vez da exceção para NoPendingCopyOperation

## <a name="march-26-2019"></a>26 de março de 2019


### <a name="core"></a>Núcleo
* Correção de problemas com incompatibilidade da extensão de desenvolvimento
* Agora o tratamento de erros encaminha os clientes para a página de problemas

### <a name="cloud"></a>Nuvem
* Erro de “assinatura não encontrada” corrigido em `cloud set`

### <a name="acr"></a>ACR
* Corrigidas fontes redundantes na importação de imagem.
* `--auth-mode` adicionado aos comandos `acr build`, `acr run`, `acr task create` e `acr task update`
* Grupo de comandos “acr task credential” adicionado para gerenciar as credenciais de uma Tarefa
* “--no-wait” adicionado ao comando `acr build`

### <a name="appservice"></a>AppService
* Bug corrigido onde `webapp up` não estava lidando corretamente com a execução do diretório vazio ou do cenário de código desconhecido
* Bug corrigido onde os slots não funcionavam para `[webapp|functionapp] config ssl bind`

### <a name="bot-service"></a>Serviço de BOT
* `bot prepare-deploy` adicionado para se preparar para a implantação de bots via `webapp`
* `bot create --kind registration` alterado para mostrar a senha se ela não for fornecida
* [ALTERAÇÃO SIGNIFICATIVA]`--endpoint` alterado em `bot create --kind registration` como padrão para uma cadeia de caracteres vazia, em vez de ser requerido
* Adicionado `SCM_DO_BUILD_DURING_DEPLOYMENT` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.

### <a name="cdn"></a>CDN
* Adicionado o suporte ao `--no-wait` para `cdn endpoint [create|update|start|stop|delete|load|purge]`  
* [ALTERAÇÃO SIGNIFICATIVA]: `cdn endpoint create` alterado para o comportamento de cache da cadeia de consulta padrão. Não há mais padrão para "IgnoreQueryString". Agora, ele é definido pelo serviço

### <a name="cosmosdb"></a>Cosmosdb
* Suporte adicionado para `--enable-multiple-write-locations` na atualização da conta
* O subgrupo `network-rule` foi adicionado com os comandos `add`, `remove` e `list` para gerenciar as regras de VNET de uma conta do Cosmos DB

### <a name="interactive"></a>Interativo
* Incompatibilidade corrigida com a extensão Interativa instalada por meio do azdev

### <a name="monitor"></a>Monitoramento
* Alterado para permitir o valor de dimensão `*` para `monitor metrics alert [create|update]`

### <a name="network"></a>Rede
* Grupo de comandos `rewrite-rule` adicionado em `application-gateway`

### <a name="profile"></a>Perfil
* Suporte de conta no nível do locatário para a identidade de serviço gerenciado adicionado em `login`

### <a name="postgres"></a>Postgres 
* Adicionados os comandos postgresql `replica` e `restart server`
* Alterado para obter o local padrão do grupo de recursos quando não fornecido para criar servidores e adicionar validação para os dias de retenção

### <a name="resource"></a>Recurso
* Saída da tabela aperfeiçoada para `deployment [create|list|show]`
* Corrigido o problema com `deployment [create|validate]` onde o tipo secureObject não era reconhecido

### <a name="graph"></a>Grafo
* Adicionado o suporte ao `--end-date` para `ad [app|sp] credential reset`
* Suporte adicionado para acrescentar permissões com `ad app permission add`
* Bug corrigido com `ad app permission list` quando não havia nenhuma permissão
* `ad sp delete` alterado para ignorar a exclusão da atribuição de função se a conta atual não tem nenhuma assinatura
* `ad app create` alterado para `--identifier-uris` passar para lista vazia como padrão se não fornecido

### <a name="storage"></a>armazenamento
* `--snapshot` adicionado a `storage file download-batch` para baixar de um instantâneo de compartilhamento
* Barra de progresso `storage blob [download-batch|upload-batch]` alterada para ser menos detalhada e indicar o blob atual
* Problema corrigido com `storage account update` ao atualizar os parâmetros de criptografia
* Problema corrigido onde `storage blob show` falharia ao usar o oauth (`--auth-mode=login`)

### <a name="vm"></a>VM
* Adicionado o comando `image update`

## <a name="march-12-2019"></a>12 de março de 2019

Versão 2.0.60

### <a name="core"></a>Núcleo

* Foi corrigido um erro incorreto no `cloud set` sobre assinatura não encontrada.

### <a name="acr"></a>ACR

* Corrigidas fontes redundantes na importação de imagem.

### <a name="acs"></a>ACS

* Alteração para ignorar o parâmetro `--listen-address` para `aks browse` se ele não for compatível com kubectl 

### <a name="appservice"></a>AppService

* Adicionado `[webapp|functionapp] deployment list-publishing-credentials` para obter a URL de publicação do Kudu e suas credenciais.
* Removida a instrução de impressão errônea de `webapp auth update`.
* Corrigido `functionapp` para definir a imagem correta do runtime nos planos do Serviço de Aplicativo no Linux.
* Removida a marca de versão prévia do `webapp up` e adicionadas melhorias ao comando.

### <a name="botservice"></a>Serviço de bot

* Adicionado `SCM_DO_BUILD_DURING_DEPLOYMENT` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.
* Adicionados `Microsoft-BotFramework-AppId` e `Microsoft-BotFramework-AppPassword` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.
* Removidas as aspas simples da saída de comando `bot publish`, no final de `bot create`.
* Alterado `bot publish` para que seja assíncrono.

### <a name="container"></a>Contêiner

* Adicionado o argumento `--no-wait` para `container [start|restart]`

### <a name="eventhub"></a>EventHub

* Adicionado o sinalizador `--skip-empty-archives` a `eventhub create|update` para dar suporte a arquivos vazios na captura.

### <a name="find"></a>Localizar

* Atualização de funcionalidade principal

### <a name="hdinsight"></a>HDInsight

* Adicionado o parâmetro `--storage-account-managed-identity` a `hdinsight create` para oferecer suporte ao MSI do ADLS Gen2.

### <a name="network"></a>Rede

* Corrigido o problema com `vpn-connection update`, onde a atualização de uma conexão VPN entre gateways em assinaturas diferentes falharia.

### <a name="rdbms"></a>Rdbms

* Correções secundárias para obter a localização padrão do grupo de recursos, quando não fornecida, para criar servidores e adicionar validação nos dias de retenção.

### <a name="role"></a>Função

* Corrigido `role definition update` para usar ID a fim de resolver a definição corretamente.
* Alterado `ad app credential reset` para remover a suposição de que a entidade de serviço do aplicativo já existe.

### <a name="service-fabric"></a>Service Fabric

* Corrigido o problema com o fato de `sf cluster list` não ser iterável.

## <a name="february-26-2019"></a>26 de fevereiro de 2019

Versão 2.0.59

### <a name="core"></a>Núcleo

* Corrigido o problema onde algumas instâncias usando `--subscription NAME` produziriam uma exceção

### <a name="acr"></a>ACR

* Parâmetro `--target` adicionado para os comandos `acr build`, `acr task create` e `acr task update`
* Melhor tratamento de erros para os comandos de execução quando não conectado ao Azure

### <a name="acs"></a>ACS

* Opção `--listen-address` adicionada a `aks port-forward`

### <a name="appservice"></a>AppService

* Adicionado o comando `functionapp devops-build`

### <a name="batch"></a>Lote
* [ALTERAÇÃO SIGNIFICATIVA] Comando `batch pool upgrade os` removido
* [ALTERAÇÃO SIGNIFICATIVA] Propriedade `Pacakges` removida das respostas `Application`
* Comando `batch application package list` adicionado para listar os pacotes de um aplicativo
* [ALTERAÇÃO SIGNIFICATIVA]`--application-id` alterado para `--application-name` em todos os comandos `batch application`, 
* O argumento `--json-file` foi adicionado aos comandos para a solicitação de resposta da API bruta
* Validação atualizada para incluir automaticamente `https://` em todos os pontos de extremidade, se ausente

### <a name="cosmosdb"></a>CosmosDB

* O subgrupo `network-rule` foi adicionado com os comandos `add`, `remove` e `list` para gerenciar as regras de VNET de uma conta do Cosmos DB

### <a name="kusto"></a>Kusto

* [ALTERAÇÃO SIGNIFICATIVA] Os tipos `hot_cache_period` e `soft_delete_period` foram alterados do banco de dados para o formato de duração ISO8601

### <a name="network"></a>Rede

* Adicionado o argumento `--express-route-gateway-bypass` para `vpn-connection [create|update]`
* Foram adicionados os grupos de comando a partir das extensões `express-route`
* Os grupos de comando `express-route gateway` e `express-route port` foram adicionados
* Adicionado o argumento `--legacy-mode` para `express-route peering [create|update]` 
* Os argumentos `--allow-classic-operations` e `--express-route-port` foram adicionados a `express-route [create|update]`
* Adicionado o argumento `--gateway-default-site` para `vnet-gateway [create|update]`
* Os comandos `ipsec-policy` foram adicionados a `vnet-gateway`

### <a name="resource"></a>Recurso

* Foi corrigido o problema com `deployment create` em que o campo do tipo diferencia letras maiúsculas e minúsculas
* Foi adicionado o suporte para arquivo de parâmetros de URI a `policy assignment create`
* Foi adicionado o suporte para parâmetros de URI e definições a `policy set-definition update`
* Foi corrigido o tratamento de parâmetros e regras para `policy definition update`
* Foi corrigido o problema com `resource show/update/delete/tag/invoke-action` em que as IDs de assinatura cruzada não respeitaram corretamente a ID da assinatura

### <a name="role"></a>Função

* Foi adicionado o suporte para as funções do aplicativo a `ad app [create|update]`

### <a name="vm"></a>VM

* Foi corrigido o problema com `vm create where ` – a rede acelerada não foi habilitada por padrão no Ubuntu 18.0

## <a name="february-12-2019"></a>12 de fevereiro de 2019

Versão 2.0.58

### <a name="core"></a>Núcleo

* `az --version` agora exibe uma notificação se você tiver pacotes para atualização
* A regressão em que `--ids` não pode ser usado com a saída JSON foi corrigida

### <a name="acr"></a>ACR
* [ALTERAÇÃO SIGNIFICATIVA] O grupo de comandos `acr build-task` foi removido
* [ALTERAÇÃO SIGNIFICATIVA] As opções `--tag` e `--manifest` de `acr repository delete` foram removidas

### <a name="acs"></a>ACS
* Suporte adicionado a `aks [enable-addons|disable-addons]` para nomes que não diferenciam maiúsculas de minúsculas
* Suporte adicionado para a operação de atualização do Azure Active Directory usando `aks update-credentials --reset-aad`
* Um esclarecimento informando que `--output` é ignorado para `aks get-credentials` foi adicionado

### <a name="ams"></a>AMS
* Adicionados os comandos `ams streaming-endpoint [start | stop | create | update] wait`
* Adicionados os comandos `ams live-event [create | start | stop | reset] wait`

### <a name="appservice"></a>AppService
* Foi adicionada a capacidade de criar e configurar funções usando contêineres de ACR
* Suporte adicionado para a atualização das configurações de aplicativos Web por meio de JSON
* A ajuda foi aprimorada para `appservice-plan-update`
* Suporte adicionado para o App Insights para auxiliar na criação de aplicativos de funções
* Os problemas com o SSH do aplicativo Web foram corrigidos

### <a name="botservice"></a>Serviço de bot
* A experiência do usuário para `bot publish` foi aprimorada
* Foram adicionados avisos de tempos limite ao executar `npm install` durante `az bot publish`
* O caractere inválido `.` de `--name` em `az bot create` foi removido
* Alteração para interromper a geração aleatória de nomes de recursos durante a criação do Armazenamento do Azure, Plano do Serviço de Aplicativo, Aplicativo Web/de funções e Application Insights
* [PRETERIDO] O argumento `--proj-name` foi preterido em favor de `--proj-file-path`
* `az bot publish` foi alterado para remover arquivos de implantação do Node.js do IIS buscados, caso eles já não existissem
* Foi adicionado o argumento `--keep-node-modules` para `az bot publish` para não excluir a pasta `node_modules` no Serviço de Aplicativo
* O par chave-valor `"publishCommand"` foi adicionado à saída de `az bot create` durante a criação de uma função do Azure ou bot de aplicativo Web
  * O valor de `"publishCommand"` é um comando `az bot publish` que é automaticamente preenchido com os parâmetros necessários para publicar o bot recém-criado
* O `"WEBSITE_NODE_DEFAULT_VERSION"` foi atualizado no modelo do ARM para que os bots de SDK v4 usem 10.14.1 em vez de 8.9.4

### <a name="key-vault"></a>Key Vault
* Foi corrigido o problema com `keyvault secret backup`, em que alguns usuários recebiam um erro `unexpected_keyword` ao usar `--id`

### <a name="monitor"></a>Monitoramento
* `monitor metrics alert [create|update]` foi alterado para permitir o valor dimensional `*`

### <a name="network"></a>Rede
* `dns zone export` foi alterado para garantir que CNAMEs exportados fossem FQDNs
* O parâmetro `--gateway-name` foi adicionado a `nic ip-config address-pool [add|remove]` para dar suporte a pools de endereços de back-end de gateway de aplicativo
* Os argumentos `--traffic-analytics` e `--workspace` foram adicionados a `network watcher flow-log configure` para dar suporte à análise de tráfego por meio de um espaço de trabalho do Log Analytics
* `--idle-timeout` e `--floating-ip` foram adicionados a `lb inbound-nat-pool [create|update]`

### <a name="policy-insights"></a>Informações sobre a Política
* Os comandos `policy remediation` foram adicionados para dar suporte a recursos de correção de política de recursos

### <a name="rdbms"></a>RDBMS
* A mensagem e os parâmetros de comando de ajuda foram aprimorados

### <a name="redis"></a>Redis
* Foram adicionados comandos para gerenciar regras de firewall (criar, atualizar, excluir, mostrar, listar)
* Foram adicionados comandos para gerenciar links do servidor (criar, excluir, mostrar, listar)
* Foram adicionados comandos para gerenciar o agendamento de patches (criar, atualizar, excluir, mostrar)
* Suporte adicionado para Zonas de Disponibilidade e versão mínima de TLS para criar Redis
* [ALTERAÇÃO SIGNIFICATIVA] Os comandos `redis update-settings` e `redis list-all` foram removidos
* [ALTERAÇÃO SIGNIFICATIVA] Parâmetro para `redis create`: “configurações de locatário” não é aceito no formato chave[=valor]
* [PRETERIDO] Uma mensagem de aviso foi adicionada para preterir o comando `redis import-method`

### <a name="role"></a>Função
* [ALTERAÇÃO SIGNIFICATIVA] O comando `az identity` foi movido dos comandos `vm` para esta localização

### <a name="sql-vm"></a>SQL VM
* [PRETERIDO] O argumento `--boostrap-acc-pwd` foi preterido devido a um erro de digitação

### <a name="vm"></a>VM
* `vm list-skus` foi alterado para permitir o uso de `--all` no lugar de `--all true`
* Adicionado `vmss run-command [invoke | list | show]`
* Foi corrigido o bug em que `vmss encryption enable` falhava se fosse executado anteriormente
* [ALTERAÇÃO SIGNIFICATIVA] O comando `az identity` foi movido para os comandos `role`

## <a name="january-31-2019"></a>31 de janeiro de 2019

Versão 2.0.57

### <a name="core"></a>Núcleo

* Hotfix para o [problema 8399](https://github.com/Azure/azure-cli/issues/8399).

## <a name="january-28-2019"></a>28 de janeiro de 2019

Versão 2.0.56

### <a name="acr"></a>ACR
* Suporte adicionado para regras de rede virtual/IP

### <a name="acs"></a>ACS
* Adicionada visualização dos nós virtuais
* Comandos do OpenShift gerenciado foram adicionados
* Suporte adicionado para operações de atualização da entidade de serviço com `aks update-credentials -reset-service-principal`

### <a name="ams"></a>AMS
* [ALTERAÇÃO SIGNIFICATIVA]`ams asset get-streaming-locators` renomeado para `ams asset list-streaming-locators`
* [ALTERAÇÃO SIGNIFICATIVA]`ams streaming-locator get-content-keys` renomeado para `ams streaming-locator list-content-keys`

### <a name="appservice"></a>AppService
* Suporte adicionado para o App Insights no `functionapp create`
* Suporte adicionado para a criação do plano de serviço de aplicativo (incluindo Elástico Premium) para Aplicativos de funções
* Foram corrigidos os problemas com de configuração de aplicativo com os planos Elástico Premium

### <a name="container"></a>Contêiner
* Adicionado o comando `container start`
* Alteração para permitir o uso de valores decimais para CPU durante a criação do contêiner

### <a name="eventgrid"></a>EventGrid
* Parâmetro `--deadletter-endpoint` adicionado a `event-subscription [create|update]`
* Storagequeue e hybridconnection foram adicionados como novos valores para 'event-subscription [create|update] --endpoint-type`
* Os parâmetros `--max-delivery-attempts` e `--event-ttl` foram adicionados a `event-subscription create` para especificar a política de repetição para eventos
* Uma mensagem de aviso foi adicionada a `event-subscription [create|update]` quando o webhook como destino for usado para uma assinatura de evento
* O parâmetro source-resource-id foi adicionado para todos os comandos relacionados a eventos e marcar todos os outros parâmetros relacionados ao recurso de origem como preteridos

### <a name="hdinsight"></a>HDInsight
* [ALTERAÇÃO SIGNIFICATIVA] Os parâmetros `--virtual-network` e `--subnet-name` de `hdinsight [application] create` foram removidos
* [ALTERAÇÃO SIGNIFICATIVA]`hdinsight create --storage-account` foi alterado para aceitar o nome ou ID da conta de armazenamento, em vez de pontos de extremidade de blob
* Parâmetros `--vnet-name` e `--subnet-name` adicionados a `hdinsight create`
* Suporte adicionado para a criptografia de disco e Enterprise Security Package ao `hdinsight create` 
* Adicionado o comando `hdinsight rotate-disk-encryption-key`
* Adicionado o comando `hdinsight update`

### <a name="iot"></a>IoT
* O formato de codificação foi adicionado ao comando routing-endpoint

### <a name="kusto"></a>Kusto
* Versão prévia

### <a name="monitor"></a>Monitoramento
* A comparação de ID foi alterada para diferenciar maiúsculas e minúsculas

### <a name="profile"></a>Perfil
* A conta de nível de locatário foi habilitada para a identidade de serviço gerenciada de `login`

### <a name="network"></a>Rede
* Foi corrigido o problema com `express-route update`: em que o argumento `--bandwidth` era ignorado
* Foi corrigido o problema com `ddos-protection update` em que definir a compreensão levava ao rastreamento de pilha

### <a name="resource"></a>Recurso
* Suporte adicionado para o arquivo de parâmetros de URI à `group deployment create`
* Suporte adicionado para a identidade gerenciada à `policy assignment [create|list|show]`

### <a name="sql-virtual-machine"></a>Máquina virtual SQL
* Versão prévia

### <a name="storage"></a>Armazenamento
* Alteração na correção para atualizar apenas as propriedades que são alteradas no mesmo objeto
* #8021 foi corrigido, dados binários são codificados em base 64 quando retornados

### <a name="vm"></a>VM
* Alteração de `vm encryption enable` para validar o cofre de chaves de criptografia de disco e se esse cofre de chaves de criptografia de chave existe
* O sinalizador `--force` foi adicionado a `vm encryption enable`

## <a name="january-15-2019"></a>15 de janeiro de 2019

Versão 2.0.55

### <a name="acr"></a>ACR
* Alteração para permitir forçar o envio por push de um gráfico Helm que não existe
* Alteração para permitir operações de runtime sem solicitações ARM
* [PRETERIDO] O parâmetro `--resource-group` foi preterido nos comandos:
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a>ACS
* Suporte adicionado para novas regiões ACI

### <a name="appservice"></a>AppService
* Foi corrigido o problema com o carregamento de certificados para aplicativos que são hospedados em um ASE, em que o RG do ASE e o RG do aplicativo são diferentes
* Alteração de `webapp up` para usar a SKU P1V1 como padrão para Linux
* `[webapp|functionapp] deployment source config-zip` foi corrigido para mostrar a mensagem de erro adequada quando uma implantação falhar 
* Adicionado o comando `webapp ssh`

### <a name="botservice"></a>Serviço de bot
* Atualizações de status de implantação foram adicionadas a `bot create`

### <a name="configure"></a>Configurar
* `none` foi adicionado como um formato de saída configurável

### <a name="cosmosdb"></a>CosmosDB
* Suporte adicionado para criar o banco de dados com taxa de transferência compartilhada

### <a name="hdinsight"></a>HDInsight
* Foram adicionados comandos para o gerenciamento de aplicativos
* Foram adicionados comandos para o gerenciamento de ações de script
* Foram adicionados comandos para o gerenciamento do Operations Management Suite (OMS)
* Suporte adicionado para listar a utilização regional ao `hdinsight list-usage`
* [ALTERAÇÃO SIGNIFICATIVA] O tipo de cluster padrão de `hdinsight create` foi removido

### <a name="network"></a>Rede
* Adicionados os argumentos `--custom-headers` e `--status-code-ranges` para `traffic-manager profile [create|update]`
* Novos tipos de roteamento foram adicionados: Subrede e múltiplos valores
* Adicionados os argumentos `--custom-headers` e `--subnets` para `traffic-manager endpoint [create|update]`  
* Foi corrigido o problema no qual fornecer `--vnets ""` a `ddos-protection update` causava um erro

### <a name="role"></a>Função
* [PRETERIDO] O argumento `--password` foi preterido para `create-for-rbac`. Como alternativa, use senhas seguras geradas pela CLI

### <a name="security"></a>Segurança
* Versão inicial

### <a name="storage"></a>Armazenamento
* [ALTERAÇÃO SIGNIFICATIVA] O número padrão de resultados de `storage [blob|file|container|share] list` foi alterado para 5.000. Use `--num-results *` para o comportamento original de retornar todos os resultados
* Parâmetro `--marker` adicionado a `storage [blob|file|container|share] list`
* Um marcador de log foi adicionado para a próxima página ao STDERR de `storage [blob|file|container|share] list` 
* O comando `storage blob service-properties update` foi adicionado com suporte para sites estáticos

### <a name="vm"></a>VM
* `vm [disk|unmanaged-disk]` e `vmss disk` foram alterados para que tenham parâmetros mais consistentes
* Suporte adicionado para referência cruzada de imagem de locatário a `[vm|vmss] create`
* O bug de configuração padrão foi corrigido em `vm diagnostics get-default-config --windows-os`
* O argumento `--provision-after-extensions` foi adicionado a `vmss extension set` para definir quais extensões deverão ser provisionadas antes da extensão ser definida
* O argumento `--replica-count` foi adicionado a `sig image-version update` para definir a contagem de replicação padrão
* Foi corrigido o bug com `image create --source` em que o disco do sistema operacional de origem era confundido com uma VM do mesmo nome, mesmo se a ID de recurso completa fosse fornecida

## <a name="december-20-2018"></a>20 de dezembro de 2018

Versão 2.0.54
### <a name="appservice"></a>AppService
* Corrigido o problema que causava falha na reimplantação do `webapp up`
* Adicionado suporte para listar e restaurar instantâneos de aplicativos Web
* Adicionado suporte para o sinalizador `--runtime` para aplicativos de funções do Windows

### <a name="iotcentral"></a>IoT Central
* Corrigida a chamada à API do comando de atualização

### <a name="role"></a>Função
* [ALTERAÇÃO SIGNIFICATIVA]`ad [app|sp] list` alterado para listar somente os 100 primeiros objetos por padrão

### <a name="sql"></a>SQL
* Adicionado suporte para ordenação personalizada nas instâncias gerenciadas

### <a name="vm"></a>VM
* Parâmetro `---os-type` adicionado a `disk create`

## <a name="december-18-2018"></a>18 de dezembro de 2018

Versão 2.0.53
### <a name="acr"></a>ACR
* Adicionado suporte para importação de imagem de Registros de Contêiner externos
* Simplificado o layout da tabela para a lista de tarefas
* Adicionado suporte para URLs do Azure DevOps

### <a name="acs"></a>ACS
* Adicionada visualização dos nós virtuais
* Removido “(VISUALIZAÇÃO)” de argumentos do AAD para `aks create`
* [PRETERIDO] Comandos `az acs` preteridos. O serviço ACS será desativado em 31 de janeiro de 2020
* Adicionado suporte da Política de Rede durante a criação de novos clusters AKS
* Removido o requisito do argumento `--nodepool-name` para `aks scale` se houver apenas um pool de nós

### <a name="appservice"></a>AppService
* Corrigido o problema em que `webapp config container` não honra o parâmetro `--slot`

### <a name="botservice"></a>Serviço de bot
* Suporte adicionado para análise do arquivo `.bot` ao chamar `bot show`
* Corrigido o bug de provisionamento do AppInsights
* Corrigido o bug de espaço em branco ao lidar com caminhos de arquivo
* Reduzidas as chamadas de rede do Kudu
* Melhorias de UX para comandos gerais

### <a name="consumption"></a>Consumo
* Corrigidos os bugs da API de orçamento ao mostrar notificações

### <a name="cosmosdb"></a>CosmosDB
* Suporte adicionado para atualizar a conta de vários mestres para mestre único

### <a name="maps"></a>Mapas
* Adicionado suporte ao SKU S1 para `maps account [create|update]`

### <a name="network"></a>Rede
* Adicionado suporte para `--format` e `--log-version` para `watcher flow-log configure`
* Corrigido o problema com `dns zone update` em que usar "" para limpar a resolução e o registro de redes virtuais não funcionava

### <a name="resource"></a>Recurso
* Corrigido o tratamento do parâmetro de escopo para grupos de gerenciamento do `policy assignment [create|list|delete|show|update]` 
* Adicionado o novo comando `resource wait`

### <a name="storage"></a>Armazenamento
*  Adicionada a capacidade de atualizar a versão do esquema de log para serviços de armazenamento no `storage logging update`

### <a name="vm"></a>VM
* Corrigida a falha em `vm identity remove` quando a VM especificada não tem nenhuma identidade de serviço gerenciado atribuída

## <a name="december-4-2018"></a>4 de dezembro de 2018

Versão 2.0.52
### <a name="core"></a>Núcleo
* Adicionado suporte para provisionamento de recursos de locatários cruzados para a entidade de serviço de multilocatários
* Corrigido o bug onde as ids enviadas por pipe de um comando com a saída tsv eram analisados incorretamente

### <a name="appservice"></a>AppService
* [VERSÃO PRÉVIA] Adicionado o comando `webapp up` que ajuda a criar e implantar conteúdo em aplicativo
* Corrigido um bug no aplicativo com base em contêiner do Windows devido à alteração de back-end

### <a name="network"></a>Rede
* Adicionado o argumento `--exclusion` a `application-gateway waf-config set` para dar suporte a exclusões de WAF

### <a name="role"></a>Função
* Adicionado suporte para identificadores personalizados para a credencial de senha 

### <a name="vm"></a>VM
* [PRETERIDO] Parâmetro `vm extension [show|wait] --expand` preterido
* Adicionado parâmetro `--force` a `vm restart` para reimplantar as VMs sem resposta
* Alterado `[vm|vmss] create --authentication-type` para aceitar "todos" para criar uma VM com senha e autenticação SSH
* Adicionado parâmetro `image create --os-disk-caching` para definir o cache de disco do sistema operacional para uma imagem

## <a name="november-20-2018"></a>20 de novembro de 2018

Versão 2.0.51
### <a name="core"></a>Núcleo
* Logon do MSI alterado para não reutilizar o nome da assinatura na identidade

### <a name="acr"></a>ACR
* Token de contexto adicionado à etapa da tarefa
* Suporte adicionado para definir segredos na execução do acr para espelhar a tarefa do acr
* Suporte aprimorado para `--top` e `--orderby` para os comandos `show-tags` e `show-manifests`

### <a name="appservice"></a>AppService
* Tempo limite padrão para a implantação do zip alterado para sondar o status aumentado para 5 minutos, também adicionando uma propriedade de tempo limite para personalizar esse valor
* Padrão `node_version` atualizado. Redefinir a ação de troca de slots durante uma troca de duas fases preserva todas as configurações do aplicativo e cadeias de conexão
* Verificação da SKU no lado do cliente removida para o Linux criar o plano do serviço de aplicativo
* Erro corrigido ao tentar obter o status de implantação do zip

### <a name="iotcentral"></a>Iot Central
* Verificação de disponibilidade do subdomínio adicionada ao criar um aplicativo do IoT Central

### <a name="keyvault"></a>KeyVault
* Bug corrigido em que os erros podem ter sido ignorados

### <a name="network"></a>Rede
* Subcomandos `root-cert` adicionados a `application-gateway` para lidar com os certificados de raiz confiável
* Opções `--min-capacity` e `--custom-error-pages` adicionadas a `application-gateway [create|update]`:
* `--zones` adicionado para suporte da zona de disponibilidade a `application-gateway create` 
* Argumentos `--file-upload-limit`, `--max-request-body-size` e `--request-body-check` a `application-gateway waf-config set` adicionados

### <a name="rdbms"></a>Rdbms
* Comandos vnet do mariadb adicionados

### <a name="rbac"></a>Rbac
* Um problema corrigido ao tentar atualizar credenciais inalteradas em `ad app update`
* Avisos de saída adicionados para comunicar alterações de falha em um futuro próximo para `ad [app|sp] list` 

### <a name="storage"></a>Armazenamento
* Melhor manipulação de casos incomuns para os comandos da cópia de armazenamento
* Corrigido o problema em que `storage blob copy start-batch` não usava credenciais de logon quando as contas de origem e destino eram iguais
* Bug corrigido com `storage [blob|file] url` em que `sas_token` não foi incorporado na URL
* Aviso de alteração da falha adicionado a `[blob|container] list`: produzirá apenas os primeiros 5.000 resultados por padrão

### <a name="vm"></a>VM
* Suporte adicionado a `[vm|vmss] create --storage-sku` para especificar a SKU da conta de armazenamento para o SO gerenciado e os discos de dados separadamente
* Parâmetros do nome da versão alterados de `sig image-version` para `--image-version -e`
* Argumento `sig image-version` preterido `--image-version-name`, substituído por `--image-version`
* Suporte adicionado para usar o disco local do SO a `[vm|vmss] create --ephemeral-os-disk`
* Adicionado o suporte ao `--no-wait` para `snapshot create/update`
* Adicionado o comando `snapshot wait`
* Suporte adicionado para usar o nome da instância com `[vm|vmss] extension set --extension-instance-name`

## <a name="november-6-2018"></a>6 de novembro de 2018

Versão 2.0.50

### <a name="core"></a>Núcleo
* Foi adicionado suporte para o serviço principal sn + autenticação do emissor

### <a name="acr"></a>ACR
* Foi adicionado suporte para eventos de git de solicitação de pull e de confirmação para o gatilho de origem da tarefa
* Alterado para usar o padrão do Dockerfile se ele não for especificado no comando de compilação

### <a name="acs"></a>ACS
* [ALTERAÇÃO SIGNIFICATIVA]`enable_cloud_console_aks_browse` foi removido para habilitar 'az aks browse' por padrão

### <a name="advisor"></a>Supervisor
* Versão de GA

### <a name="ams"></a>AMS
* Novos grupos de comandos adicionados:
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* Novos comandos adicionados:
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* Adicionados parâmetros de criptografia com suporte para `ams streaming-policy create`
* O suporte adicionado para `ams transform output remove` agora pode ser executado passando o índice de saída a ser removido
* Adicionados os argumentos `--correlation-data` e `--label` ao grupo de comandos `ams job`
* Adicionados os argumentos `--storage-account` e `--container` ao grupo de comandos `ams asset`
* Foram adicionados valores padrões para o horário de expiração (agora +23h) e permissões (Leitura) no comando `ams asset get-sas-url` 
* [ALTERAÇÃO SIGNIFICATIVA] O comando `ams streaming locator` foi substituído por `ams streaming-locator`
* [ALTERAÇÃO SIGNIFICATIVA] O argumento `--content-keys` de `ams streaming locator` foi atualizado
* [ALTERAÇÃO SIGNIFICATIVA]`--content-policy-name` foi renomeado como `--content-key-policy-name` no comando `ams streaming locator`
* [ALTERAÇÃO SIGNIFICATIVA] O comando `ams streaming policy` foi substituído por `ams streaming-policy`
* [ALTERAÇÃO SIGNIFICATIVA] O argumento `--preset-names` foi substituído por `--preset` no grupo de comandos `ams transform`. Agora, você só pode definir uma saída/predefinição de cada vez (para adicionar mais, é preciso executar `ams transform output add`). Além disso, você pode definir StandardEncoderPreset personalizado passando o caminho para seu JSON personalizado
* [ALTERAÇÃO SIGNIFICATIVA]`--output-asset-names ` foi renomeado como `--output-assets` no comando `ams job start`. Agora, ele aceita uma lista separada por espaços dos ativos no formato 'assetName=label'. Um ativo sem rótulo pode ser enviado assim: 'assetName='

### <a name="appservice"></a>AppService
* Um bug no `az webapp config backup update` que impede a configuração de um agendamento de backup foi corrigido, caso ele ainda não tenha sido definido

### <a name="configure"></a>Configurar
* O YAML foi adicionado às opções de formato de saída

### <a name="container"></a>Contêiner
* Alterado para mostrar a identidade ao exportar um grupo de contêineres para yaml

### <a name="eventhub"></a>EventHub
* O sinalizador `--enable-kafka` foi adicionado para dar suporte ao Kafka no `eventhub namespace [create|update]`

### <a name="interactive"></a>Interativo
* O interativo agora instala a extensão `interactive` que permite atualizações e suporte mais rápidos

### <a name="monitor"></a>Monitoramento
* Foi adicionado suporte para nomes de métricas, que incluem os caracteres barra (/) e ponto (.) para `--condition` em `monitor metrics alert [create|update]`

### <a name="network"></a>Rede
* Os nomes de comandos `network interface-endpoint` foram preteridos em benefício de `network private-endpoint`
* Foi corrigido um problema onde um argumento `--peer-circuit` em `express-route peering connection create` não aceitaria uma ID
* Foi corrigido um problema onde `--ip-tags` não funcionava corretamente com `public-ip create` 

### <a name="profile"></a>Perfil
* `--use-cert-sn-issuer` foi adicionado a `az login` para logon da entidade de serviço com rolagens automáticas de certificado

### <a name="rdbms"></a>RDBMS
* Adicionados comandos da réplica mysql

### <a name="resource"></a>Recurso
* Adicionado suporte para grupos de gerenciamento e assinaturas aos comandos `policy definition|set-definition`

### <a name="role"></a>Função
* Adicionado suporte para gerenciamento de permissões de API, usuário conectado e gerenciamento de senhas dos aplicativos e certificados de credenciais
* `ad sp create-for-rbac` foi alterado para esclarecer a confusão entre o displayName e o nome da entidade de serviço
* Suporte adicionado para conceder permissões a aplicativos do AAD

### <a name="storage"></a>Armazenamento
* Suporte adicionado para se conectar aos serviços de armazenamento somente com SAS e pontos de extremidade (sem um nome de conta ou uma chave), conforme descrito em `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`

### <a name="vm"></a>VM
* O argumento `storage-sku` foi adicionado a `image create` para definir o tipo de conta de armazenamento padrão da imagem
* O bug com `vm resize` onde a opção `--no-wait` faz com que o comando falhasse foi corrigido
* O formato de saída da tabela `vm encryption show` para mostrar o status foi alterado
* `vm secret format` foi alterado para exigir a saída json/jsonc. Avisa o usuário e assume como padrão a saída json se um formato de saída indesejado for escolhido
* Validação de argumento aprimorado para `vm create --image`

## <a name="october-23-2018"></a>23 de outubro de 2018

Versão 2.0.49

### <a name="core"></a>Núcleo
* Corrigido o problema com `--ids` onde `--subscription` teria precedência sobre a assinatura em `--ids`
* Adicionados avisos explícitos quando parâmetros seriam ignorados pelo uso de `--ids`

### <a name="acr"></a>ACR
* Corrigido um problema de codificação de ACR Build no Python2

### <a name="cdn"></a>CDN
* [ALTERAÇÃO SIGNIFICATIVA] Alterado o comportamento de armazenamento em cache da cadeia de caracteres de consulta padrão de `cdn endpoint create` para não assumir o padrão "IgnoreQueryString". Agora, ele é definido pelo serviço

### <a name="container"></a>Contêiner
* Adicionado `Private` como um tipo válido para passar para '--ip-address'
* Alterado para permitir o uso somente de ID de sub-rede para configurar uma rede virtual para o grupo de contêineres
* Alterado para permitir o uso de nome de rede virtual ou ID de recurso para habilitar o uso de redes virtuais de diferentes grupos de recursos
* Adicionado `--assign-identity` para adicionar uma identidade MSI a um grupo de contêineres
* Adicionado `--scope` para criar uma atribuição de função para a identidade MSI atribuída pelo sistema
* Adicionado um aviso ao criar um grupo de contêineres com uma imagem sem um processo de execução longa
* Corrigidos os problemas de saída da tabela para comandos `list` e `show`

### <a name="cosmosdb"></a>CosmosDB
* Adicionado o suporte `--enable-multiple-write-locations` para `cosmosdb create`

### <a name="interactive"></a>Interativo
* Alterado para garantir que o parâmetro de assinatura global seja exibido nos parâmetros

### <a name="iot-central"></a>Central da IoT
* Adicionadas opções de nome de exibição e modelo para criação de aplicativos de IoT Central
* [ALTERAÇÃO SIGNIFICATIVA] Removido o suporte para a SKU F1; Use a SKU S1

### <a name="monitor"></a>Monitoramento
* Alterações para `monitor activity-log list`:
  * Adicionado suporte para listar todos os eventos no nível da assinatura
  * Adicionado o parâmetro `--offset` para criar consultas de tempo mais facilmente
  * Melhorada a validação para `--start-time` e `--end-time` para usar um intervalo mais amplo de formatos ISO8601 e formatos de data/hora mais amigáveis ao usuário
  * Adicionado `--namespace` como alias para a opção preterida `--resource-provider`
  * Preterido `--filters` porque não há valores diferentes daqueles com opções fortemente tipadas compatíveis com o serviço
* Alterações para `monitor metrics list`:
  * Adicionado o parâmetro `--offset` para criar consultas de tempo mais facilmente
  * Melhorada a validação para `--start-time` e `--end-time` para usar um intervalo mais amplo de formatos ISO8601 e formatos de data/hora mais amigáveis ao usuário
* Melhorada a validação para os argumentos `--event-hub` e `--event-hub-rule` para `monitor diagnostic-settings create`

### <a name="network"></a>Rede
* Adicionados os argumentos `--app-gateway-address-pools` e `--gateway-name` para `nic create`, para dar suporte à adição de pools de endereços de back-end do gateway de aplicativo a um NIC
* Adicionados os argumentos `--app-gateway-address-pools` e `--gateway-name` para `nic ip-config create/update`, para dar suporte à adição de pools de endereços de back-end do gateway de aplicativo a um NIC

### <a name="servicebus"></a>ServiceBus
* Adicionado `migration_state` somente leitura para MigrationConfigProperties para mostrar o atual estado de migração de namespace Standard para Premium do Barramento de Serviço

### <a name="sql"></a>SQL
* Corrigidos `sql failover-group create` e `sql failover-group update` para trabalhar com a política de failover Manual

### <a name="storage"></a>Armazenamento
* Corrigida a formatação de saída `az storage cors list`, todos os itens mostram a chave correta de "Serviço"
* Adicionado o parâmetro `--bypass-immutability-policy` para a exclusão de contêiner bloqueado pela política de imutabilidade

### <a name="vm"></a>VM
* Aplicado o modo `None` de armazenamento em cache de disco para as séries Lv/Lv2 de computadores no `[vm|vmss] create`
* Atualizada a lista de tamanhos com suporte compatíveis com a aceleração de rede para `vm create`
* Adicionado argumentos fortemente tipados para configurações de iops e mbps de ultra ssd para `disk create`

## <a name="october-16-2018"></a>16 de outubro de 2018

Versão 2.0.48

### <a name="vm"></a>VM
* Corrigido o problema do SDK que causava falha durante a instalação do Homebrew

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
* `functionapp create` alterado para dar suporte à criação de um tipo de plano de consumo do Linux com um runtime específico
* [VERSÃO PRÉVIA] Suporte adicionado para hospedar aplicativos Web nos contêineres do Windows

### <a name="event-hub"></a>Hub de evento
* Corrigido o comando `eventhub update`
* [ALTERAÇÃO SIGNIFICATIVA]`list` comandos alterados para lidar com os erros de recurso(s) NotFound(404) do modo típico, em vez de mostrar uma lista vazia

### <a name="extensions"></a>Extensões
* Corrigido o problema ao tentar adicionar uma extensão já instalada

### <a name="hdinsight"></a>HDInsight
* Versão inicial

### <a name="iot"></a>IoT
* Comando de instalação da extensão adicionado à faixa inicial

### <a name="keyvault"></a>KeyVault
* Alterado para restringir os comandos de armazenamento do keyvault ao perfil da API mais recente

### <a name="network"></a>Rede
* Corrigido `network dns zone create`: O comando terá êxito mesmo se o usuário tiver configurado um local padrão. Veja o n° 6052
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
* [ALTERAÇÃO SIGNIFICATIVA]`list` comandos alterados para lidar com os erros de recurso(s) NotFound(404) do modo típico, em vez de mostrar uma lista vazia

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
* Comandos adicionados para regras da rede virtual

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

* Adicionada uma solução alternativa para operações de runtime sem solicitações ARM
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
* [ALTERAÇÃO SIGNIFICATIVA]`[vm|vmss] create`, `[vm|vmss] identity assign` e `[vm|vmss] identity remove` alterados para produzir identidades de usuário atribuídas no formato de dicionário

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
* [ALTERAÇÃO SIGNIFICATIVA] Todos os clusters e servidores de arquivos devem ser criados nos workspaces
* [ALTERAÇÃO SIGNIFICATIVA] Os trabalhos devem ser criados nas experiências
* [ALTERAÇÃO SIGNIFICATIVA]`--nfs-resource-group` foi removido dos comandos `cluster create` e `job create`. Para montar um NFS pertencente a outro workspace/grupo de recursos, forneça a ID de ARM do servidor de arquivos através da opção `--nfs`
* [ALTERAÇÃO SIGNIFICATIVA]`--cluster-resource-group` foi removido do comando `job create`. Para enviar um trabalho em um cluster pertencente a outro workspace/grupo de recursos, forneça a ID de ARM do cluster através da opção `--cluster`
* [ALTERAÇÃO SIGNIFICATIVA] O atributo `location` foi removido de trabalhos, cluster e servidores de arquivos. Agora, o local é um atributo de um workspace.
* [ALTERAÇÃO SIGNIFICATIVA]`--location` foi removido dos comandos `job create` e `cluster create` e `file-server create`
* [ALTERAÇÃO SIGNIFICATIVA] Os nomes das opções curtas foi alterado para tornar a interface mais consistente:
  - [`--config`, `-c`] foi renomeado para [`--config-file`, `-f`]
  - [`--cluster`, `-r`] foi renomeado para [`--cluster`, `-c`]
  - [`--cluster`, `-n`] foi renomeado para [`--cluster`, `-c`]
  - [`--job`, `-n`] foi renomeado para [`--job`, `-j`]

### <a name="maps"></a>Mapas

* [ALTERAÇÃO SIGNIFICATIVA]`maps account create` foi alterado para exigir a aceitação dos Termos de Serviço pelo prompt interativo ou sinalizador `--accept-tos`

### <a name="network"></a>Rede

* Suporte adicionado para `https` a `network lb probe create` [nº6571](https://github.com/Azure/azure-cli/issues/6571)
* Foi corrigido o problema em que `--endpoint-status` diferenciava maiúsculas de minúsculas. [#6502](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a>Reservas

* [ALTERAÇÃO SIGNIFICATIVA] Foi adicionado o parâmetro `ReservedResourceType` necessário a `reservations catalog show`
* Parâmetro `Location` adicionado a `reservations catalog show`
* [ALTERAÇÃO SIGNIFICATIVA]`kind` foi removido de `ReservationProperties`
* [ALTERAÇÃO SIGNIFICATIVA]`capabilities` foi renomeado para `sku_properties` em `Catalog`
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

* Versão inicial

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

* Foi corrigido um erro de digitação no exemplo para `cognitiveservices account create`[#5603](https://github.com/Azure/azure-cli/issues/5603)

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
* [ALTERAÇÃO SIGNIFICATIVA]`--msi-port` e `--identity-port` removidos porque não são mais usados
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
* [ALTERAÇÃO SIGNIFICATIVA]`--admin-user-name` renomeado para `--user-name` no comando `file-server create` para ser consistente com o comando `cluster create`

### <a name="billing"></a>Cobrança

* Adição de comandos da conta de registro

### <a name="consumption"></a>Consumo

* Adicionados os comandos `marketplace`
* [ALTERAÇÃO SIGNIFICATIVA]`reservations summaries` renomeado para `reservation summary`
* [ALTERAÇÃO SIGNIFICATIVA]`reservations details` renomeado para `reservation detail`
* [ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--reservation-order-id` e `--reservation-id` para os comandos `reservation`
* [ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--grain` para os comandos `reservation summary`
* [ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--include-meter-details` para os comandos `pricesheet`

### <a name="container"></a>Contêiner

* Adição dos parâmetros de montagem de volume do Repositório Git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` e `--gitrepo-mount-path`
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
* [ALTERAÇÃO SIGNIFICATIVA]`extension list-available` alterado para mostrar dados de extensão simplificados por padrão

### <a name="interactive"></a>Interativo

* Alteração nas conclusões para ativar após a conclusão do carregamento da tabela de comandos
* Correção de bug usando o parâmetro `--style`
* Analisador léxico interativo instanciado após a falta do despejo da tabela de comandos
* Suporte aprimorado ao completador

### <a name="lab"></a>Laboratório

* Correção de bugs com o comando `create environment`

### <a name="monitor"></a>Monitoramento

* Adicionado suporte para `--top`, `--orderby` e `--namespace` para `metrics list` [nº5785](https://github.com/Azure/azure-cli/issues/5785)
* Corrigido [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` aceita uma lista separada por espaços de métricas para recuperação
* Suporte adicionado para `--namespace` a `metrics list-definitions` [nº5785](https://github.com/Azure/azure-cli/issues/5785)

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
* Corrigido [#4049](https://github.com/Azure/azure-cli/issues/4049): problemas com o acréscimo de uploads de blob ignorando os parâmetros da condição

### <a name="vm"></a>VM

* Adição de aviso para `vmss create` para alterações de falha futuras para conjuntos com mais de 100 instâncias
* Adição de suporte com flexibilidade de região para `vm [snapshot|image]`
* Alteração no modo de exibição de instância de disco para reportar status de criptografia mais adequados
* [ALTERAÇÃO SIGNIFICATIVA]`vm extension delete` alterado para não retornar mais a saída

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

* [ALTERAÇÃO SIGNIFICATIVA]`advisor configuration get` renomeado para `advisor configuration list`
* [ALTERAÇÃO SIGNIFICATIVA]`advisor configuration set` renomeado para `advisor configuration update`
* [ALTERAÇÃO SIGNIFICATIVA]`advisor recommendation generate` removido
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

* Corrigido [#5625](https://github.com/Azure/azure-cli/issues/5625): manter histórico em sessões diferentes
* Corrigido [#3016](https://github.com/Azure/azure-cli/issues/3016): histórico não registrado no escopo
* Corrigido [#5688](https://github.com/Azure/azure-cli/issues/5688): as conclusões não aparecerão se o carregamento da tabela de comando encontrar uma exceção
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
* Corrigido [#5286](https://github.com/Azure/azure-cli/issues/5286): os comandos em lotes `storage blob [delete-batch|download-batch|upload-batch]` não geram mais um erro após falhas da pré-condição

### <a name="vm"></a>VM

* Suporte adicionado a `[vm|vmss] create` anexar discos de dados não gerenciados e configurar o cache
* `[vm|vmss] assign-identity` e `[vm|vmss] remove-identity` preteridos
* Comandos `vm identity [assign|remove|show]` e `vmss identity [assign|remove|show]` adicionados para substituir comandos preteridos
* Prioridade padrão alterada em `vmss create` para None

## <a name="february-27-2018"></a>27 de fevereiro de 2018

Versão 2.0.28

### <a name="core"></a>Núcleo

* Corrigido [#5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalação do Homebrew
* Adição de suporte para telemetria de extensão com chaves personalizadas
* Adição de log HTTP em `--debug`

### <a name="acs"></a>ACS

* Alteração para usa o gráfico `virtual-kubelet-for-aks` do Helm para `aks install-connector` por padrão
* Problema corrigido: permissão insuficiente para entidades de serviço criarem um grupo de contêiner ACI
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

* Corrigido [#5559](https://github.com/Azure/azure-cli/issues/5559): cliente ausente em `network vnet-gateway vpn-client generate`

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

* [ALTERAÇÃO SIGNIFICATIVA]`aks get-versions` renomeado para `aks get-upgrades` para fins de precisão
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
* [ALTERAÇÃO SIGNIFICATIVA]`externalIdentities` alterado para `userAssignedIdentities` para EMSI
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

* Versão inicial

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

* Corrigido: não atribuir acesso, a menos que `--scope` seja fornecido
* Corrigido: usar a mesma nomenclatura de extensão do que o portal
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
* Corrigido: detectar as configurações de slot corretamente

### <a name="iot"></a>IoT

* Corrigido #3934: a criação de uma política não limpa mais as políticas existentes

### <a name="network"></a>Rede

* [ALTERAÇÃO SIGNIFICATIVA]`vnet list-private-access-services` renomeado para `vnet list-endpoint-services`
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

* `create`: corrigido o problema em que o sinal de igual não era permitido dentro de uma variável de ambiente


### <a name="data-lake-store"></a>Data Lake Store

* Habilitado o controle do andamento

### <a name="event-grid"></a>Grade de Eventos

* Versão inicial

### <a name="network"></a>Rede

* `lb`: corrigido o problema em que os nomes de recursos filhos específicos não eram resolvidos corretamente quando omitidos
* `application-gateway {subresource} delete`: corrigido o problema em que `--no-wait` não foi liquidado
* `application-gateway http-settings update`: corrigido o problema em que `--connection-draining-timeout` não podia ser desativado
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
* Adicionado o suporte ao `--dns-servers` para `nic update` e `nic create`: Adicionar suporte para --dns-servers
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

* Removido o parâmetro `sql server create` `--identity` desfeito
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
* núcleo: permitir que o caminho do arquivo accessTokens.json seja configurável por meio de uma variável de ambiente ([#2605](https://github.com/Azure/azure-cli/issues/2605))
* núcleo: permitir que padrões configurados sejam aplicados em argumentos opcionais ([#2703](https://github.com/Azure/azure-cli/issues/2703))
* núcleo: desempenho aprimorado
* núcleo: certificados de AC personalizados – suporte à configuração da variável de ambiente REQUESTS_CA_BUNDLE
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
* Exposição de argumentos para configurar a implantação e as “pilhas em runtime” em webapp create
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
* BC: remoção de --expires e --not-before de `keyvault certificate create`, pois estes parâmetros não têm suporte no serviço
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

* Correção de bug: modelagem de `--actions` de `az alert-rules create` para consumir a cadeia de caracteres JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))
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
* BC: corrigido um bug na saída de `vpn-connection create`
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

  observação: em comandos da VM em nuvens soberanas, evite recursos relacionados ao disco gerenciado, incluindo os seguintes:
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

* DocumentDB: adicionado suporte para a listagem de cadeias de conexão ([#2580](https://github.com/Azure/azure-cli/pull/2580))

### <a name="vm"></a>VM

* [Compute] Adicionar suporte a AppGateway para criar o conjunto de dimensionamento de máquinas virtuais ([#2570](https://github.com/Azure/azure-cli/pull/2570))
* [VM/VMSS] Suporte aprimorado ao cache de disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))
* VM/VMSS: incorporar a lógica de validação de credenciais usada pelo portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))
* Adicionar comandos de espera e suporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))
* Conjunto de dimensionamento de máquinas virtuais: suporte à * para listar a exibição de instâncias em vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))
* Adicionar: segredos da VM e do conjunto de dimensionamento de máquinas virtuais ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))
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
> Alguns dos módulos de comando têm um sufixo "b *n*" ou "rc *n*". Esses módulos de comando ainda estão em versão prévia e estarão disponíveis no futuro

Também temos compilações de versão prévia noturnas da CLI. Para obter informações, consulte essas instruções sobre [como obter as compilações diárias](https://github.com/Azure/azure-cli#nightly-builds) e essas instruções sobre [configuração do desenvolvedor e código de contribuição](https://github.com/Azure/azure-cli#developer-setup)

Você pode relatar problemas com as compilações de visualização diárias das seguintes maneiras:
- Relatar problemas na [lista de problemas do github](https://github.com/azure/azure-cli/issues/)
- Entre em contato com a equipe do produto no endereço [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)
- Forneça comentários a partir da linha de comando com o comando `az feedback`

# <a name="beta-release-notes"></a>[Notas sobre a versão beta](#tab/azure-cli-beta)

A versão beta da CLI do Azure é uma migração do método de autenticação da plataforma AAD (v 1.0) para a [plataforma de Identidade da Microsoft (v 2.0)](/azure/active-directory/develop/v2-overview).

## <a name="june-23-2020"></a>23 de junho de 2020

### <a name="things-to-know-about-the-new-azure-cli-beta-release"></a>O que você precisa saber sobre a nova versão beta da CLI do Azure

-   A versão beta da CLI do Azure dá suporte a todos os comandos da CLI que você encontrará na versão lançada atual.
-   Fazer logon novamente é necessário após a instalação da versão beta.
-   A versão beta dá suporte apenas à plataforma Windows.
-   Não há suporte para o Azure Stack.
-   Não há suporte para o parâmetro `--use-cert-sn-issuer` ao usar a chave de entidade de serviço para se autenticar.
-   Não há suporte para ignorar a verificação SSL por meio do ambiente `ADAL_PYTHON_SSL_NO_VERIFY`.

Se você encontrar problemas com a versão beta, a equipe de engenharia da CLI do Azure ficará feliz por receber seus comentários no [GitHub](https://github.com/Azure/azure-cli/issues/new/choose).

---
