---
title: Links entre serviços para trabalhar com a CLI do Azure
description: Links para tutoriais populares, inícios rápidos, exemplos, conceitos e guias de instruções, CLI do Azure, máquinas virtuais, AKS (Serviço de Kubernetes do Azure), Lote, CLI do Azure (Core), Azure Resource Manager, Key Vault, Azure Stack Hub, Functions, Banco de Dados, Hubs de Eventos, Configuração de Aplicativos, Configuração de Aplicativos, Alemanha, Segurança, Governança, Insights, IoT, Internet das Coisas, DevOps, Rede Virtual, Computação, Rede, Ferramentas para Desenvolvedores, Bancos de Dados, Análise, Gerenciamento e Governança, Híbrido, Armazenamento, Segurança, IA, IA + Machine Learning, Linux, Windows, Ubuntu, automação, aplicativo, aplicativo Web, script
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 03/01/2020
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 42e9de630530568a15bc6f9f05d2442d790d8b68
ms.sourcegitcommit: 2da241715d25407ed22c1065c0c793acfd865996
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/09/2020
ms.locfileid: "89563137"
---
# <a name="popular-articles-using-the-azure-cli"></a>Artigos populares que usam a CLI do Azure

A CLI do Azure é usada em diversos serviços do Azure. Por isso, há artigos em todos os repositórios de documentos.  Nesta página, há links para artigos populares selecionados.  

## <a name="compute"></a>Computação

| | | | |
|-|-|-|-|
|Máquinas Virtuais | Tutorial: Linux | [Criar uma máquina virtual Linux com a CLI do Azure](azure-cli-vm-tutorial.yml) | Crie uma máquina virtual.  Saiba mais sobre as consultas de saída e como configurar as variáveis de ambiente.
|Máquinas Virtuais | Início Rápido: Linux | [Criar uma máquina virtual do Linux usando a CLI do Azure](/azure/virtual-machines/linux/quick-create-cli) | Crie e implante uma máquina virtual do Linux.  Abra uma porta para o tráfego da Web e instale um servidor Web.
|Máquinas Virtuais | Guia de instruções: Linux |[Criar uma imagem do Linux de máquina virtual ou um VHD](/azure/virtual-machines/linux/capture-image) | Desprovisione uma máquina virtual existente, crie uma imagem e crie uma máquina virtual com a imagem capturada.
|Máquinas Virtuais | Guia de instruções: Linux | [Carregar um VHD no Azure usando a CLI do Azure](/azure/virtual-machines/linux/disks-upload-vhd-to-managed-disk-cli) | Crie um disco gerenciado vazio, carregue o arquivo VHD local e copie um disco gerenciado.
|Máquinas Virtuais | Guia de instruções: Linux | [Criar uma galeria de imagens compartilhadas com a CLI do Azure](/azure/virtual-machines/linux/shared-images) | Crie uma Galeria de Imagens Compartilhadas com imagens de VM personalizadas com outras pessoas em sua organização, dentro ou entre regiões, ou em um locatário do Azure Active Directory.
|Máquinas Virtuais | Guia de instruções: Linux | [Implantar VMs do Spot com a CLI do Azure (versão prévia)](/azure/virtual-machines/linux/spot-cli) | Implante uma máquina virtual spot do Linux que não será removida com base no preço.
|Máquinas Virtuais | Início Rápido: Windows | [Criar uma máquina virtual do Windows com a CLI do Azure](/azure/virtual-machines/windows/quick-create-cli) | Implante uma máquina virtual no Azure que executa o Windows Server 2016.
|Máquinas Virtuais | Módulo de aprendizagem | [Gerenciar máquinas virtuais com a CLI do Azure](https://docs.microsoft.com/learn/modules/manage-virtual-machines-with-azure-cli/) | Crie, inicie, pare e realize outras tarefas de gerenciamento relacionadas às máquinas virtuais.
|AKS (Serviço de Kubernetes do Azure)| Guia de Início Rápido | [Implantar um cluster do AKS (Serviço de Kubernetes do Azure) usando a CLI do Azure](/azure/aks/kubernetes-walkthrough) | Implante e gerencie clusters do AKS.  Veja como monitorar a integridade do cluster e dos pods que executam o aplicativo.
|Lote do Azure|Amostra | [Executar um trabalho e tarefas com o Lote do Azure usando a CLI do Azure](/azure/batch/scripts/batch-cli-sample-run-job) | Crie um trabalho em lotes e adicione uma série de tarefas a ele. Monitore um trabalho e suas tarefas.
|Lote do Azure|Amostra | [Criar e gerenciar um pool do Windows no Lote do Azure usando a CLI do Azure](/azure/batch/scripts/batch-cli-sample-manage-windows-pool) | Crie e gerencie um pool de nós de computação do Windows com uma configuração dos Serviços de Nuvem.
|Azure Container Instance|Guia de Início Rápido | [Implantar uma instância de contêiner com a CLI do Azure](/azure/container-instances/container-instances-quickstart) | Implante um contêiner do Docker isolado e disponibilize o aplicativo com um FQDN (nome de domínio totalmente qualificado). Execute um comando único de implantação e navegue até o aplicativo em execução no contêiner.
|Azure Function|Guia de Início Rápido |  [Criar uma função no Azure que responde às solicitações HTTP com a CLI do Azure](/azure/azure-functions/functions-create-first-azure-function-azure-cli) | Use as ferramentas da linha de comando para criar uma função que responde às solicitações HTTP. Após testar o código localmente, implante a função no ambiente sem servidor do Azure Functions.

## <a name="networking"></a>Rede

| | | | |
|-|-|-|-|
|Rede Virtual|Guia de Início Rápido | [Criar uma rede virtual usando a CLI do Azure](/azure/virtual-network/quick-create-cli) | Crie uma rede virtual, implante duas máquinas virtuais nessa rede virtual e conecte-se às máquinas virtuais na Internet.
|Rede Virtual|Guia de instruções | [Habilitar a Rede Acelerada em uma máquina virtual do Linux com a CLI do Azure](/azure/virtual-network/create-vm-accelerated-networking-cli) | Crie uma máquina virtual do Linux, realize a associação dinâmica e a revogação da função virtual e habilite a Rede Acelerada.

## <a name="internet-of-things"></a>Internet das coisas

| | | | |
|-|-|-|-|
|Hub IoT|Tutorial | [Configurar o roteamento de mensagens do Hub IoT com a CLI do Azure](/azure/iot-hub/tutorial-routing) | Configurar e usar consultas de roteamento personalizadas com o Hub IoT.

## <a name="developer-tools"></a>Ferramentas para Desenvolvedores

| | | | |
|-|-|-|-|
|Configuração de Aplicativo do Azure|Exemplos |[Exemplos da CLI do Azure para a Configuração de Aplicativos do Azure](/azure/azure-app-configuration/cli-samples) | Receba links para scripts de bash que usam a CLI do Azure para a Configuração de Aplicativos do Azure.
|Azure DevOps| Introdução: pipeline de DevOps |[Criar seu primeiro pipeline do Azure com a CLI do Azure](/azure/devops/pipelines/create-first-pipeline-cli) | Crie um pipeline em um diretório clonado do GitHub, gerencie e execute seus pipelines.
|Azure DevOps| Guia de instruções: pipeline de DevOps |[Tarefas de implantação de pipeline do Azure com a CLI do Azure](/azure/devops/pipelines/tasks/deploy/azure-cli?view=azure-devops) | Em um pipeline de lançamento ou build, execute um script de shell ou em lotes que contém a CLI do Azure.  Os comandos são executados em agentes multiplataforma em execução em sistemas operacionais Linux, macOS ou Windows.
|Azure DevOps| Tutorial: pipeline do Jenkins |[Implantar no Serviço de Aplicativo do Azure com o Jenkins usando a CLI do Azure](/azure/jenkins/execute-cli-jenkins-pipeline) | Crie e configure uma máquina virtual do Jenkins, crie um aplicativo Web no Azure e prepare um repositório do GitHub.  Crie e execute o pipeline do Jenkins.

## <a name="databases"></a>Bancos de dados

| | | | |
|-|-|-|-|
|Banco de Dados SQL| Amostra |[Configurar o Banco de Dados SQL do Azure com a CLI do Azure](/azure/sql-database/sql-database-cli-samples?tabs=single-database) | Exemplos da CLI do Azure para o Banco de Dados SQL do Azure.
|MySQL|Guia de Início Rápido |[Criar um servidor de Banco de Dados do Azure para MySQL usando a CLI do Azure](/azure/mysql/quickstart-create-mysql-server-database-using-azure-cli) | Criar um servidor de Banco de Dados do Azure para MySQL.  Defina uma regra de firewall e as configurações do SSL.  Obtenha e use as informações de conexão.
|Cosmos DB |Guia de instruções |[Gerenciar recursos do Azure Cosmos com a CLI do Azure](/azure/cosmos-db/manage-with-cli) | Use comandos comuns para automatizar o gerenciamento das contas, dos bancos de dados e dos contêineres do Azure Cosmos DB.
|Cosmos DB |Amostra |[Exemplos da CLI do Azure para a API do SQL (Core) do Azure Cosmos DB](/azure/cosmos-db/cli-samples) | Siga os links para ver exemplos de script da CLI do Azure para a API do SQL (Core) do Azure Cosmos DB.

## <a name="analytics"></a>Análise

| | | | |
|-|-|-|-|
Hub de Eventos do Azure |Guia de Início Rápido |[Criar um hub de eventos com a CLI do Azure](/azure/event-hubs/event-hubs-quickstart-cli) | Crie um namespace dos Hubs de Eventos e um hub de eventos.
HDInsight |Guia de instruções |[Criar os clusters do HDInsight usando a CLI do Azure](/azure/hdinsight/hdinsight-hadoop-create-linux-clusters-azure-cli) | Crie um cluster do HDInsight 3.6.
HDInsight |Tutorial |[Gerenciar os clusters do Azure HDInsight com a CLI do Azure](/azure/hdinsight/hdinsight-administer-use-command-line) | Liste, mostre, exclua e escale os clusters do HDInsight.

## <a name="management-and-governance"></a>Gerenciamento e governança

| | | | |
|-|-|-|-|
Modelos do Resource Manager |Guia de instruções |[Implantar recursos com os modelos do Resource Manager e a CLI do Azure](/azure/azure-resource-manager/templates/deploy-cli) | Implante recursos no Azure com modelos.
Grupos do Resource Manager |Guia de instruções |[Gerenciar grupos de recursos do Azure Resource Manager com a CLI do Azure](/azure/azure-resource-manager/management/manage-resource-groups-cli) | Use o Azure Resource Manager para gerenciar os grupos de recursos do Azure.
Resource Graph |Guia de Início Rápido |[Execute sua primeira consulta do Resource Graph com a CLI do Azure](/azure/governance/resource-graph/first-query-azurecli) | Adicione o Azure Resource Graph à instalação da CLI do Azure e execute sua primeira consulta do Resource Graph.
Atribuição de política |Guia de Início Rápido |[Criar uma atribuição de política para identificar recurso sem conformidade com a CLI do Azure](/azure/governance/policy/assign-policy-azurecli) | Crie uma atribuição de política para identificar máquinas virtuais que não usam discos gerenciados.

## <a name="hybrid"></a>Híbrido

| | | | |
|-|-|-|-|
Azure Stack Hub| Início Rápido: VM Linux |[Criar uma máquina virtual de servidor do Linux no Azure Stack Hub com a CLI do Azure](/azure-stack/user/azure-stack-quick-create-vm-linux-cli) | Crie uma máquina virtual do Ubuntu Server 16.04 LTS, conecte-se à máquina virtual com um cliente remoto e instale um servidor Web do NGINX.
Azure Stack Hub| Início Rápido: VM Windows |[Criar uma máquina virtual do Windows Server no Azure Stack Hub com a CLI do Azure](/azure-stack/user/azure-stack-quick-create-vm-windows-cli) |Crie uma máquina virtual do Windows Server 2016, conecte-se à máquina virtual com um cliente remoto e instale um servidor Web do IIS.
Azure Stack Hub| Guia de instruções: recursos do ASDK |[Gerenciar e implantar recursos no Azure Stack Hub com a CLI do Azure](/azure-stack/user/azure-stack-version-profiles-azurecli2) | Configure a CLI do Azure para gerenciar os recursos do ASDK (Kit de Desenvolvimento do Azure Stack) nas plataformas de cliente do Linux, do Mac e do Windows.

## <a name="storage"></a>Armazenamento

| | | | |
|-|-|-|-|
Armazenamento de Blobs |Guia de Início Rápido |  [Criar, baixar e listar blobs com a CLI do Azure](/azure/storage/blobs/storage-quickstart-blobs-cli) | Carregar e baixar dados do Armazenamento de Blobs do Azure.
Armazenamento de Blobs |Guia de instruções |[Autorizar acesso a dados de blob ou fila com a CLI do Azure](/azure/storage/common/authorize-data-operations-cli) | Especifique como as operações de dados são autorizadas e configure variáveis de ambiente para os parâmetros.
Armazenamento de Blobs |Guia de instruções |[Usar a CLI do Azure para gerenciar diretórios, arquivos e ACLs no Azure Data Lake Storage Gen2 (versão prévia)](/azure/storage/blobs/data-lake-storage-directory-file-acl-cli) | Crie e gerencie diretórios, arquivos e permissões nas contas de armazenamento que têm um namespace hierárquico.
Armazenamento de arquivos |Guia de Início Rápido |[Criar e gerenciar os compartilhamentos de arquivo do Azure com a CLI do Azure](/azure/storage/files/storage-how-to-use-files-cli) | Crie e use os compartilhamentos de arquivo do Azure.  Crie e gerencie instantâneos de compartilhamento.

## <a name="security"></a>Segurança

| | | | |
|-|-|-|-|
Entidade de serviço |Guia de instruções |[Criar uma entidade de serviço do Azure com a CLI do Azure](/cli/azure/create-an-azure-service-principal-azure-cli) | Crie, obtenha informações e redefina uma entidade de serviço com a CLI do Azure.
RBAC |Guia de instruções |[Adicione ou remova atribuições de função com o RBAC do Azure e a CLI do Azure](/azure/role-based-access-control/role-assignments-cli) | Atribua funções ao controle de acesso baseado em função do Azure.
Key Vault |Guia de instruções |[Gerenciar o Key Vault usando a CLI do Azure](/azure/key-vault/key-vault-manage-with-cli2) | Crie e gerencie o Azure Key Vault.  Registre e autorize um aplicativo, defina políticas de acesso avançadas e aprenda comandos de interface de linha de comando multiplataforma.
Key Vault |Tutorial |[Gerenciar chaves de conta de armazenamento com o Key Vault e a CLI do Azure](/azure/key-vault/key-vault-ovw-storage-keys) | Gerencie chaves de conta de armazenamento e gere tokens de assinatura de acesso compartilhado.

## <a name="ai--machine-learning"></a>IA + Machine Learning

| | | | |
|-|-|-|-|
Machine Learning |Referência |[Usar a extensão da CLI do Azure para o Azure Machine Learning](/azure/machine-learning/reference-azure-machine-learning-cli) | Execute experimentos para criar modelos de machine learning e registre esses modelos para o uso do cliente.  Empacote, implante e rastreie o ciclo de vida de seus modelos de machine learning.
Serviços Cognitivos |Guia de instruções |[Criar um recurso dos Serviços Cognitivos com a CLI do Azure](/azure/cognitive-services/cognitive-services-apis-create-account-cli) | Inscreva-se nos Serviços Cognitivos do Azure e crie uma conta de serviço único ou uma assinatura de vários serviços.  Use as chaves e o ponto de extremidade gerados para você para autenticar seus aplicativos.
Azure Monitor |Guia de instruções |[Criar um workspace do Log Analytics com a CLI do Azure](/azure/azure-monitor/learn/quick-create-workspace-cli) | Crie e implante um workspace do Log Analytics.

## <a name="geographies"></a>Geografias

| | | | |
|-|-|-|-|
Azure Alemanha |Introdução |[Conectar-se ao Azure Alemanha com a CLI do Azure](/azure/germany/germany-get-started-connect-with-cli) | Com o Azure Alemanha, é possível gerenciar uma assinatura de grande porte por meio de scripts e acessar recursos que não estão disponíveis no portal do Azure global no momento.
Azure Government|Introdução |[Conectar-se ao Azure Governamental com a CLI do Azure](/azure/azure-government/documentation-government-get-started-connect-with-cli)|Acesse e comece a gerenciar recursos no Azure Government.

## <a name="see-also"></a>Confira também

* [Introdução à CLI do Azure](get-started-with-azure-cli.md)
* [Lista de referência completa de comandos da CLI do Azure](/cli/azure/reference-index)
* [Serviços que a CLI do Azure pode gerenciar](azure-services-the-azure-cli-can-manage.md)
