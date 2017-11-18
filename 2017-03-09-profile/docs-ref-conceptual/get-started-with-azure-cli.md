---
title: "Introdução à CLI do Azure 2.0"
description: "Introdução à CLI do Azure 2.0 no Linux, Mac ou Windows."
keywords: CLI do Azure 2.0, Linux, Mac, Windows, OS X, Ubuntu, Debian, CentOS, RHEL, SUSE, CoreOS, Docker, Windows, Python, PIP
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 85c418a8-6177-4833-bb8d-ff4ce2233c1a
ms.openlocfilehash: 11153c13fb9868897b0bb21dac9d64072c3af16e
ms.sourcegitcommit: 70c4d7a14591e5b761e261105cd2d376753f2a54
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/19/2017
---
# <a name="get-started-with-azure-cli-20"></a>Introdução à CLI do Azure 2.0

A CLI 2.0 do Azure é a nova experiência de linha de comando do Azure para gerenciar recursos do Azure.
Você pode usá-lo no seu navegador com o [Azure Cloud Shell](/azure/cloud-shell/overview) ou pode [instalá-lo](install-azure-cli.md) no macOS, Linux e Windows e executá-lo da linha de comando.

A CLI do Azure 2.0 foi projetada para gerenciar e administrar os recursos do Azure da linha de comando e para a compilação de scripts de automação que funcionam no Azure Resource Manager.
Esse artigo ajuda você a começar a usá-lo, além de ensinar os conceitos básicos por trás dele.

Para saber mais sobre a versão mais recente, veja as [notas de versão](release-notes-azure-cli.md).

## <a name="connect"></a>Connect

A maneira mais simples de começar é [iniciar o Cloud Shell](/azure/cloud-shell/quickstart).

1. Inicie o Cloud Shell no painel de navegação superior do portal do Azure.

   ![Ícone do Shell](media/get-started-with-azure-cli/shell-icon.png)

2. Escolha a assinatura que você deseja usar e crie uma conta de armazenamento.

   ![Criar uma conta de armazenamento](media/get-started-with-azure-cli/storage-prompt.png)

Você também pode [instalar](install-azure-cli.md) a CLI e executá-la localmente a partir da linha de comando. Assim que tiver instalado a CLI, execute `az login` para entrar com sua assinatura padrão.

## <a name="create-a-resource-group"></a>Criar um grupo de recursos

Agora que tudo foi configurado, vamos usar a CLI do Azure para criar recursos no Azure.

Primeiro, crie um Grupo de Recursos.  Os Grupos de Recursos no Azure fornecem uma maneira de gerenciar vários recursos que você deseja agrupar logicamente.  Por exemplo, você pode criar um Grupo de recursos para um aplicativo ou projeto e adicionar uma máquina virtual, um banco de dados e um serviço CDN dentro dele.

Vamos criar um grupo de recursos chamado "MyResourceGroup" na região *westus2* do Azure.  Para fazer isso, digite o seguinte comando:

```azurecli-interactive
az group create -n MyResourceGroup -l westus2 
```

Quando o grupo de recursos for criado, o comando `az group create` gerará várias propriedades do recurso recém-criado:

```Output
{
  "id": "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MyResourceGroup",
  "location": "westus2",
  "managedBy": null,
  "name": "MyResourceGroup",
  "properties": {
    "provisioningState": "Succeeded"
  },
  "tags": null
}
```

## <a name="create-a-linux-virtual-machine"></a>Criar uma Máquina Virtual do Linux

Agora que temos nosso grupo de recursos, vamos criar uma VM do Linux dentro dele.

Você pode criar uma VM Linux usando a imagem popular do UbuntuLTS, com dois discos de armazenamento anexados de 10 GB e 20 GB, usando o seguinte comando:

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS --data-disk-sizes-gb 10 20
```

Ao executar o comando anterior, a CLI do Azure 2.0 procura um par de chaves SSH armazenado em seu diretório ~/.ssh.  Se você ainda não tiver um par de chaves SSH armazenado ali, solicite à CLI do Azure para criar um para você automaticamente passando o parâmetro --generate-ssh-keys:

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS --data-disk-sizes-gb 10 20 --generate-ssh-keys
```

O comando `az vm create` gera uma saída após a VM ter sido totalmente criada e estar pronta para ser acessada e usada. A saída inclui várias propriedades da VM recém-criada, incluindo seu endereço IP público:

```Output
{
  "fqdns": "",
  "id": "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MyResourceGroup/providers/Microsoft.Compute/virtualMachines/MyLinuxVM",
  "location": "westus2",
  "macAddress": "xx-xx-xx-xx-xx-xx",
  "powerState": "VM running",
  "privateIpAddress": "xx.x.x.x",
  "publicIpAddress": "xx.xxx.xxx.xx",
  "resourceGroup": "MyResourceGroup"
}
```

Agora que a VM foi criada, faça logon em sua nova VM do Linux usando **SSH** com o endereço IP público da VM criada:

```azurecli-interactive
ssh xx.xxx.xxx.xxx
```

```Output
Welcome to Ubuntu 14.04.4 LTS (GNU/Linux 3.19.0-65-generic x86_64)

 * Documentation:  https://help.ubuntu.com/

  System information as of Sun Feb 19 00:32:28 UTC 2017

  System load: 0.31              Memory usage: 3%   Processes:       89
  Usage of /:  39.6% of 1.94GB   Swap usage:   0%   Users logged in: 0

  Graph this data and manage this system at:
    https://landscape.canonical.com/

  Get cloud support with Ubuntu Advantage Cloud Guest:
    http://www.ubuntu.com/business/services/cloud

0 packages can be updated.
0 updates are security updates.



The programs included with the Ubuntu system are free software;
the exact distribution terms for each program are described in the
individual files in /usr/share/doc/*/copyright.

Ubuntu comes with ABSOLUTELY NO WARRANTY, to the extent permitted by
applicable law.

my-login@MyLinuxVM:~$
```

## <a name="create-a-windows-server-virtual-machine"></a>Criar uma Máquina Virtual do Windows Server

Agora, vamos criar uma VM baseada no Windows Server 2016 Datacenter usando o comando `az vm create` e adicioná-la ao mesmo grupo de recursos “MyResourceGroup” que usamos em nossa VM Linux.  Como no exemplo da VM Linux, também anexaremos dois discos de armazenamento usando o parâmetro `--data-disk-sizes-gb`.

O Azure exige que você evite usar nomes de usuário/senha fáceis de adivinhar. Há regras específicas para quais caracteres podem ser usados, além do comprimento mínimo do nome de usuário e senha.  

> [!NOTE]
> Você deverá inserir o nome de usuário e a senha ao executar esse comando.

```azurecli-interactive
az vm create -n MyWinVM -g MyResourceGroup --image Win2016Datacenter
```

O comando `az vm create` gera uma saída após a VM ter sido totalmente criada e estar pronta para ser acessada e usada.

```Output
{
  "fqdns": "",
  "id": "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MyResourceGroup/providers/Microsoft.Compute/virtualMachines/MyWinVM",
  "location": "westus2",
  "macAddress": "xx-xx-xx-xx-xx-xx",
  "powerState": "VM running",
  "privateIpAddress": "xx.x.x.x",
  "publicIpAddress": "xx.xxx.xx.xxx",
  "resourceGroup": "MyResourceGroup"
}
```

Agora faça logon em sua VM do Windows Server criada recentemente usando a Área de Trabalho Remota e o endereço IP público da VM (que é retornada na saída de `az vm create`).  
Se você estiver em um sistema baseado em Windows, faça isso na linha de comando usando o comando `mstsc`:

```azurecli-interactive
mstsc /v:xx.xxx.xx.xxx
```

Forneça a mesma combinação de nome de usuário/senha usada ao criar a VM para efetuar o logon.

## <a name="creating-other-resources-in-azure"></a>Criar outros recursos no Azure

Agora percorremos a criação de um Grupo de recursos, uma VM do Linux e uma VM do Windows Server. Você também pode criar vários outros tipos de recursos do Azure.  

Todos os novos recursos são criados usando um processo consistente padrão de nomenclatura `az <resource type name> create`.  Por exemplo, para criar um Balanceador de Carga de Rede do Azure que poderíamos associar às nossas VMs recém-criadas, podemos usar o seguinte comando create:

```azurecli-interactive
az network lb create -n MyLoadBalancer -g MyResourceGroup
```

Também poderíamos criar uma nova Rede Virtual privada (conhecida como "VNet" no Azure) para nossa infraestrutura usando o seguinte comando create:

```azurecli-interactive
az network vnet create -n MyVirtualNetwork -g MyResourceGroup --address-prefix 10.0.0.0/16
```

O que torna o Azure e a CLI do Azure tão poderosos é que podemos usar isso não apenas para obter a infraestrutura baseada em nuvem, mas também para criar serviços de plataforma gerenciados.  Os serviços de plataforma gerenciados também podem ser combinados com a infraestrutura para compilar soluções ainda mais eficientes.

Por exemplo, é possível usar a CLI do Azure para criar um Serviço de Aplicativo do Azure.  O Serviço de Aplicativo do Azure é um serviço de plataforma gerenciado que fornece uma ótima maneira para hospedar aplicativos Web sem precisar se preocupar com a infraestrutura.  Depois de criar o Serviço de Aplicativo do Azure, você pode criar dois novos Aplicativos Web do Azure dentro do Serviço de Aplicativo usando os seguintes comandos create:

```azurecli-interactive
# Create an Azure AppService that we can host any number of web apps within
az appservice plan create -n MyAppServicePlan -g MyResourceGroup

# Create Two Web Apps within the AppService (note: name param must be a unique DNS entry)
az webapp create -n MyWebApp43432 -g MyResourceGroup --plan MyAppServicePlan 
az webapp create -n MyWebApp43433 -g MyResourceGroup --plan MyAppServicePlan 
```

Depois de compreender os conceitos básicos do padrão `az <resource type name> create`, é fácil criar qualquer coisa. A seguir veja alguns tipos de recursos populares do Azure e comandos create da CLI do Azure correspondentes para criá-los:

```
Resource Type               Azure CLI create command
-------------               ------------------------
Resource Group              az group create
Virtual Machine             az vm create
Virtual Network             az network vnet create
Load Balancer               az network lb create
Managed Disk                az disk create
Storage account             az storage account create
Virtual Machine Scale Set   az vmss create
Azure Container Service     az acs create
Web App                     az webapp create
SQL Database Server         az sql server create
Document DB                 az documentdb create
```

Visite a [Documentação de referência](/cli/azure) para saber mais sobre os outros parâmetros específicos de recursos que você pode passar para cada um dos comandos anteriores e os tipos de recursos que você pode criar. 

## <a name="useful-tip-optimizing-create-operations-using---no-wait"></a>Dica útil: otimização das operações de criação usando --no-wait

Por padrão, ao criar recursos usando a CLI do Azure 2.0, o comando `az <resource type name> create` aguardará até que o recurso seja criado e esteja pronto para uso.  Por exemplo, se você criar uma VM, o comando `az vm create`, por padrão, não retornará até que a VM seja criada e esteja pronta para você usar SSH ou RDP nela.

Usamos essa abordagem, pois ela facilita a gravação de scripts de automação que contêm várias etapas com dependências (e precisam de uma tarefa anterior para serem concluídas com êxito antes de continuar).

Se não for necessário esperar a criação de um recurso antes de continuar, você pode usar a opção `no-wait` para iniciar uma ação de criação em segundo plano. Você pode continuar usando a CLI para outros comandos.

Por exemplo, o seguinte uso de `az vm create` inicia uma implantação de VM e, em seguida, gera resultados com maior rapidez (e antes da VM ser totalmente inicializada):

```azurecli-interactive
az vm create -n MyLinuxVM2 -g MyResourceGroup --image UbuntuLTS --no-wait
```

A abordagem `--no-wait` pode ajudá-lo a otimizar consideravelmente o desempenho de seus scripts de automação.

## <a name="listing-resources-and-formatting-output"></a>Listagem de recursos e a formatação de saída

Você pode usar o comando `list` na CLI do Azure para localizar e listar os recursos em execução no Azure. 

Como acontece com o comando create, você pode listar recursos usando a CLI do Azure 2.0 usando um padrão de nomenclatura `az <resource type name> list` comum que seja consistente em todos os tipos de recursos.  Há vários formatos de saída e opções de consulta para filtrar e classificar a lista de recursos da maneira que você prefere vê-los.

Por exemplo, `az vm list` mostra a lista de todas as VMs que você possui.   

```azurecli-interactive
az vm list 
```
Os valores retornados estão em JSON por padrão (mostrando apenas o resultado parcial para fins de brevidade).

```json
[
  {
    "availabilitySet": null,
    "diagnosticsProfile": null,
    "hardwareProfile": {
      "vmSize": "Standard_DS1_v2"
    },
    "id": "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010",
    "instanceView": null,
    "licenseType": null,
    "location": "westus2",
    "name": "MyLinuxVM",
    "networkProfile": {
      "networkInterfaces": [
        {
          "id": "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/demorg1/providers/Microsoft.Network/networkInterfaces/DemoVM010VMNic",
          "primary": null,
          "resourceGroup": "MyResourceGroup"
        }
      ]
    },
          ...
          ...
          ...   
]
```

Opcionalmente, você pode modificar o formato de saída usando a opção `--output`.  Execute o comando `az vm list` para ver VMs do Linux e do Windows Server criadas anteriormente, juntamente com as propriedades mais comuns de uma VM, usando a opção de formato *tabela* que é muito fácil de ler:

```azurecli-interactive
az vm list --output table
```

```Output
Name       ResourceGroup    Location
---------  ---------------  ----------
MyLinuxVM  MyResourceGroup  westus2
MyWinVM    MyResourceGroup  westus2
```

A opção de saída *tsv* pode ser usada para obter um formato baseado em texto, separado por tabulações, sem nenhum cabeçalho.  Esse formato é útil quando você deseja redirecionar a saída para outra ferramenta baseada em texto como grep. 

```azurecli-interactive
az vm list --output tsv
```

```
None    None            /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MyResourceGroup/providers/Microsoft.Compute/virtualMachines/MyLinuxVM        None    None    westus2 MyLinuxVM                   None        Succeeded       MyResourceGroup None                    Microsoft.Compute/virtualMachines       XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
None    None            /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MyResourceGroup/providers/Microsoft.Compute/virtualMachines/MyWinVM  None    None    westus2 MyWinVM                 None    Succeeded       MyResourceGroup None                    Microsoft.Compute/virtualMachines       XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
```
Visite o artigo [formatos de saída](format-output-azure-cli.md) para saber mais sobre outras maneiras de listar recursos e formatar a saída.

## <a name="querying-resources-and-shaping-outputs"></a>Consulta de recursos e modelagem de saídas

Geralmente, convém consultar apenas os recursos que atendem a uma condição específica.  

O comando `list` conta com suporte interno que facilita a filtragem de recursos pelo nome do Grupo de Recursos.  Por exemplo, você pode passar a um parâmetro `--ResourceGroup` ou `-g` para um comando `list` para recuperar apenas os recursos dentro de um grupo de recursos específico:


```azurecli-interactive
az vm list -g MyResourceGroup --output table
```

```Output
Name       ResourceGroup    Location
---------  ---------------  ----------
MyLinuxVM  MyResourceGroup  westus2
MyWinVM    MyResourceGroup  westus2
```

Para obter ainda um suporte à consulta ainda mais avançado, use o parâmetro `--query` para executar uma consulta JMESPath nos resultados de *qualquer* comando `az`.  As consultas JMESPath podem ser usadas para filtrar e também modelar a saída de qualquer resultado retornado.

Por exemplo, execute o seguinte comando para consultar qualquer recurso de máquina virtual dentro de qualquer grupo de recursos que contenha as letras "Meu":

```azurecli-interactive
az vm list --output table --query "[?contains(resourceGroup,'MY')]" 
```

```Output
ResourceGroup    ProvisioningState    Name       Location    VmId
---------------  -------------------  ---------  ----------  ------------------------------------
MYRESOURCEGROUP  Succeeded            MyLinuxVM  westus2     XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
MYRESOURCEGROUP  Succeeded            MyWinVM    westus2     XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
```

Em seguida, poderíamos escolher refinar ainda mais a saída usando o recurso de modelagem de consultas JMESPath para também gerar valores diferentes.  Por exemplo, o comando a seguir recupera o tipo de disco do sistema operacional que a máquina virtual está usando para determinar se o sistema operacional é baseado em Linux ou Windows:

```azurecli-interactive
az vm list --output table --query "[?contains(resourceGroup,'MY')].{ VMName:name,OSType:storageProfile.osDisk.osType }" 
```

```Output
VMName     OSType
---------  --------
MyLinuxVM  Linux
MyWinVM    Windows
```

O suporte a JMESPath na CLI do Azure é poderoso.  Saiba mais sobre como usá-lo no artigo [consulta](query-azure-cli.md).

## <a name="deleting-resources"></a>Excluir os recursos

Você pode usar o comando `delete` na CLI do Azure para excluir os recursos desnecessários. Você pode usar o comando `delete` com qualquer recurso, da mesma forma com o comando `create`.

```azurecli-interactive
az vm delete -n MyLinuxVM -g MyResourceGroup
```

Por padrão, a CLI solicita a confirmação da exclusão.  Você pode suprimir esse aviso para scripts automatizados.

```Output
Are you sure you want to perform this operation? (y/n): y
EndTime                           Name                                  StartTime                         Status
--------------------------------  ------------------------------------  --------------------------------  ---------
2017-02-19T02:35:56.678905+00:00  5b74ab80-9b29-4329-b483-52b406583e2f  2017-02-19T02:33:35.372769+00:00  Succeeded
```

Também é possível usar o comando `delete` para excluir vários recursos ao mesmo tempo. Por exemplo, o comando a seguir exclui todos os recursos no grupo de recursos "MyResourceGroup" que usamos para todos os exemplos nesse tutorial de Introdução.

```azurecli-interactive
az group delete -n MyResourceGroup
```

```Output
Are you sure you want to perform this operation? (y/n): y
```

## <a name="get-samples"></a>Obter exemplos

Para saber mais sobre como usar a CLI do Azure, consulte nossos scripts mais comuns para [VMs do Linux](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json), [VMs do Windows](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json), [Aplicativos Web](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json) e [Banco de Dados SQL](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json).

## <a name="read-the-api-reference-docs"></a>Leia os documentos de referência de API

[Referência de API](/cli/azure)

## <a name="get-help"></a>Obter ajuda

A CLI do Azure tem documentação de ajuda interna que corresponde à nossa documentação da Web que pode ser executada na linha de comando:

```azurecli-interactive
az [command-group [command]] -h
```

Por exemplo, para ver quais comandos e subgrupos estão disponíveis para VMs, use:

```azurecli-interactive
az vm -h
```

Para obter ajuda com o comando para criar uma VM, use:

```azurecli-interactive
az vm create -h
```

## <a name="switch-from-azure-cli-10"></a>Alternar a partir da CLI do Azure 1.0

Se já souber como usar a CLI do Azure 1.0 (azure.js), você verá lugares onde os comandos não são exatamente os mesmos.
Às vezes, os comandos para executar uma tarefa são significativamente diferentes.
Para ajudá-lo a fazer a transição da CLI do Azure 1.0 para a CLI do Azure 2.0, iniciamos esse [mapeamento do comando](https://github.com/Azure/azure-cli/blob/master/doc/azure2az_commands.rst).

## <a name="send-us-your-feedback"></a>Envie-nos seus comentários

```azurecli-interactive
az feedback
```
