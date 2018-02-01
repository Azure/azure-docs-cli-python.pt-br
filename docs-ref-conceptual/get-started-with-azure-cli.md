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
ms.openlocfilehash: 689b8f4d77af5a6f398c0dd85e922baa398f767a
ms.sourcegitcommit: dd5b2c7b0b56608ef9ea8730c7dc76e6c532d5ea
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2018
---
# <a name="get-started-with-azure-cli-20"></a><span data-ttu-id="bafc0-104">Introdução à CLI do Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="bafc0-104">Get started with Azure CLI 2.0</span></span>

<span data-ttu-id="bafc0-105">A CLI 2.0 do Azure é a nova experiência de linha de comando do Azure para gerenciar recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="bafc0-105">The Azure CLI 2.0 is Azure's new command line experience for managing Azure resources.</span></span>
<span data-ttu-id="bafc0-106">Você pode usá-lo no seu navegador com o [Azure Cloud Shell](/azure/cloud-shell/overview) ou pode [instalá-lo](install-azure-cli.md) no macOS, Linux e Windows e executá-lo da linha de comando.</span><span class="sxs-lookup"><span data-stu-id="bafc0-106">You can use it in your browser with [Azure Cloud Shell](/azure/cloud-shell/overview), or you can [install](install-azure-cli.md) it on macOS, Linux, and Windows and run it from the command line.</span></span>

<span data-ttu-id="bafc0-107">A CLI do Azure 2.0 foi projetada para gerenciar e administrar os recursos do Azure da linha de comando e para a compilação de scripts de automação que funcionam no Azure Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="bafc0-107">Azure CLI 2.0 is optimized for managing and administering Azure resources from the command line, and for building automation scripts that work against the Azure Resource Manager.</span></span>
<span data-ttu-id="bafc0-108">Esse artigo ajuda você a começar a usá-lo, além de ensinar os conceitos básicos por trás dele.</span><span class="sxs-lookup"><span data-stu-id="bafc0-108">This article helps get you started using it, and teaches you the core concepts behind it.</span></span>

<span data-ttu-id="bafc0-109">Para saber mais sobre a versão mais recente, veja as [notas de versão](release-notes-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="bafc0-109">For information about the latest release, see the [release notes](release-notes-azure-cli.md).</span></span>

## <a name="connect"></a><span data-ttu-id="bafc0-110">Connect</span><span class="sxs-lookup"><span data-stu-id="bafc0-110">Connect</span></span>

<span data-ttu-id="bafc0-111">A maneira mais simples de começar é [iniciar o Cloud Shell](/azure/cloud-shell/quickstart).</span><span class="sxs-lookup"><span data-stu-id="bafc0-111">The simplest way to get started is to [launch Cloud Shell](/azure/cloud-shell/quickstart).</span></span>

1. <span data-ttu-id="bafc0-112">Inicie o Cloud Shell no painel de navegação superior do portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="bafc0-112">Launch Cloud Shell from the top navigation of the Azure portal.</span></span>

   ![Ícone do Shell](media/get-started-with-azure-cli/shell-icon.png)

2. <span data-ttu-id="bafc0-114">Escolha a assinatura que você deseja usar e crie uma conta de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="bafc0-114">Choose the subscription you want to use and create a storage account.</span></span>

   ![Criar uma conta de armazenamento](media/get-started-with-azure-cli/storage-prompt.png)

<span data-ttu-id="bafc0-116">Você também pode [instalar](install-azure-cli.md) a CLI e executá-la localmente a partir da linha de comando.</span><span class="sxs-lookup"><span data-stu-id="bafc0-116">You can also [install](install-azure-cli.md) the CLI and run it locally from the command line.</span></span> <span data-ttu-id="bafc0-117">Assim que tiver instalado a CLI, execute `az login` para entrar com sua assinatura padrão.</span><span class="sxs-lookup"><span data-stu-id="bafc0-117">Once you have installed the CLI, run `az login` to log in with your default subscription.</span></span>

## <a name="create-a-resource-group"></a><span data-ttu-id="bafc0-118">Criar um grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="bafc0-118">Create a Resource Group</span></span>

<span data-ttu-id="bafc0-119">Agora que tudo foi configurado, vamos usar a CLI do Azure para criar recursos no Azure.</span><span class="sxs-lookup"><span data-stu-id="bafc0-119">Now that we've got everything set up, let's use the Azure CLI to create resources within Azure.</span></span>

<span data-ttu-id="bafc0-120">Primeiro, crie um Grupo de Recursos.</span><span class="sxs-lookup"><span data-stu-id="bafc0-120">First, create a Resource Group.</span></span>  <span data-ttu-id="bafc0-121">Os Grupos de Recursos no Azure fornecem uma maneira de gerenciar vários recursos que você deseja agrupar logicamente.</span><span class="sxs-lookup"><span data-stu-id="bafc0-121">Resource Groups in Azure provide a way to manage multiple resources that you want to logically group.</span></span>  <span data-ttu-id="bafc0-122">Por exemplo, você pode criar um Grupo de recursos para um aplicativo ou projeto e adicionar uma máquina virtual, um banco de dados e um serviço CDN dentro dele.</span><span class="sxs-lookup"><span data-stu-id="bafc0-122">For example, you might create a Resource Group for an application or project and add a virtual machine, a database and a CDN service within it.</span></span>

<span data-ttu-id="bafc0-123">Vamos criar um grupo de recursos chamado "MyResourceGroup" na região *westus2* do Azure.</span><span class="sxs-lookup"><span data-stu-id="bafc0-123">Let's create a resource group named "MyResourceGroup" in the *westus2* region of Azure.</span></span>  <span data-ttu-id="bafc0-124">Para fazer isso, digite o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="bafc0-124">To do so type the following command:</span></span>

```azurecli-interactive
az group create -n MyResourceGroup -l westus2
```

<span data-ttu-id="bafc0-125">Quando o grupo de recursos for criado, o comando `az group create` gerará várias propriedades do recurso recém-criado:</span><span class="sxs-lookup"><span data-stu-id="bafc0-125">Once the resource group has been created, the `az group create` command outputs several properties of the newly created resource:</span></span>

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

## <a name="create-a-linux-virtual-machine"></a><span data-ttu-id="bafc0-126">Criar uma Máquina Virtual do Linux</span><span class="sxs-lookup"><span data-stu-id="bafc0-126">Create a Linux Virtual Machine</span></span>

<span data-ttu-id="bafc0-127">Agora que temos nosso grupo de recursos, vamos criar uma VM do Linux dentro dele.</span><span class="sxs-lookup"><span data-stu-id="bafc0-127">Now that we have our resource group, let's create a Linux VM within it.</span></span>

<span data-ttu-id="bafc0-128">Você pode criar uma VM Linux usando a imagem popular do UbuntuLTS, com dois discos de armazenamento anexados de 10 GB e 20 GB, usando o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="bafc0-128">You can create a Linux VM using the popular UbuntuLTS image, with two attached storage disks of 10 GB and 20 GB, with the following command:</span></span>

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS --data-disk-sizes-gb 10 20
```

<span data-ttu-id="bafc0-129">Ao executar o comando anterior, a CLI do Azure 2.0 procura um par de chaves SSH armazenado em seu diretório ~/.ssh.</span><span class="sxs-lookup"><span data-stu-id="bafc0-129">When you run the preceding command, the Azure CLI 2.0 looks for an SSH key pair stored under your ~/.ssh directory.</span></span>  <span data-ttu-id="bafc0-130">Se você ainda não tiver um par de chaves SSH armazenado ali, solicite à CLI do Azure para criar um para você automaticamente passando o parâmetro --generate-ssh-keys:</span><span class="sxs-lookup"><span data-stu-id="bafc0-130">If you don't already have an SSH key pair stored there, you can ask the Azure CLI to automatically create one for you by passing the --generate-ssh-keys parameter:</span></span>

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS --data-disk-sizes-gb 10 20 --generate-ssh-keys
```

<span data-ttu-id="bafc0-131">O comando `az vm create` gera uma saída após a VM ter sido totalmente criada e estar pronta para ser acessada e usada.</span><span class="sxs-lookup"><span data-stu-id="bafc0-131">The `az vm create` command returns output once the VM has been fully created and is ready to be accessed and used.</span></span> <span data-ttu-id="bafc0-132">A saída inclui várias propriedades da VM recém-criada, incluindo seu endereço IP público:</span><span class="sxs-lookup"><span data-stu-id="bafc0-132">The output includes several properties of the newly created VM including its public IP address:</span></span>

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

<span data-ttu-id="bafc0-133">Agora que a VM foi criada, faça logon em sua nova VM do Linux usando **SSH** com o endereço IP público da VM criada:</span><span class="sxs-lookup"><span data-stu-id="bafc0-133">Now that the VM has been created, you can log on to your new Linux VM using **SSH** with the public IP address of the VM you created:</span></span>

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

## <a name="create-a-windows-server-virtual-machine"></a><span data-ttu-id="bafc0-134">Criar uma Máquina Virtual do Windows Server</span><span class="sxs-lookup"><span data-stu-id="bafc0-134">Create a Windows Server Virtual Machine</span></span>

<span data-ttu-id="bafc0-135">Agora, vamos criar uma VM baseada no Windows Server 2016 Datacenter usando o comando `az vm create` e adicioná-la ao mesmo grupo de recursos “MyResourceGroup” que usamos em nossa VM Linux.</span><span class="sxs-lookup"><span data-stu-id="bafc0-135">Let's now create a Windows Server 2016 Datacenter-based VM using the `az vm create` command and add it to the same "MyResourceGroup" resource group that we used for our Linux VM.</span></span>  <span data-ttu-id="bafc0-136">Como no exemplo da VM Linux, também anexaremos dois discos de armazenamento usando o parâmetro `--data-disk-sizes-gb`.</span><span class="sxs-lookup"><span data-stu-id="bafc0-136">Like the Linux VM example, we'll also attach two storage disks using the `--data-disk-sizes-gb` parameter.</span></span>

<span data-ttu-id="bafc0-137">O Azure exige que você evite usar nomes de usuário/senha fáceis de adivinhar.</span><span class="sxs-lookup"><span data-stu-id="bafc0-137">Azure requires that you avoid using easily guessed usernames/passwords.</span></span> <span data-ttu-id="bafc0-138">Há regras específicas para quais caracteres podem ser usados, além do comprimento mínimo do nome de usuário e senha.</span><span class="sxs-lookup"><span data-stu-id="bafc0-138">There are specific rules for what characters can be used as well as the minimum length of both username and password.</span></span>

> [!NOTE]
> <span data-ttu-id="bafc0-139">Você deverá inserir o nome de usuário e a senha ao executar esse comando.</span><span class="sxs-lookup"><span data-stu-id="bafc0-139">You will be prompted to enter your username and password when running this command.</span></span>

```azurecli-interactive
az vm create -n MyWinVM -g MyResourceGroup --image Win2016Datacenter
```

<span data-ttu-id="bafc0-140">O comando `az vm create` gera uma saída após a VM ter sido totalmente criada e estar pronta para ser acessada e usada.</span><span class="sxs-lookup"><span data-stu-id="bafc0-140">The `az vm create` command output results once the VM has been fully created and is ready to be accessed and used.</span></span>

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

<span data-ttu-id="bafc0-141">Agora faça logon em sua VM do Windows Server criada recentemente usando a Área de Trabalho Remota e o endereço IP público da VM (que é retornada na saída de `az vm create`).</span><span class="sxs-lookup"><span data-stu-id="bafc0-141">Now log on to your newly created Windows Server VM using Remote Desktop and the public IP address of the VM (which is returned in the output from `az vm create`).</span></span>
<span data-ttu-id="bafc0-142">Se você estiver em um sistema baseado em Windows, faça isso na linha de comando usando o comando `mstsc`:</span><span class="sxs-lookup"><span data-stu-id="bafc0-142">If you are on a Windows-based system, you can do this from the command line using the `mstsc` command:</span></span>

```azurecli-interactive
mstsc /v:xx.xxx.xx.xxx
```

<span data-ttu-id="bafc0-143">Forneça a mesma combinação de nome de usuário/senha usada ao criar a VM para efetuar o logon.</span><span class="sxs-lookup"><span data-stu-id="bafc0-143">Supply the same username/password combination you used when creating the VM to log in.</span></span>

## <a name="creating-other-resources-in-azure"></a><span data-ttu-id="bafc0-144">Criar outros recursos no Azure</span><span class="sxs-lookup"><span data-stu-id="bafc0-144">Creating other resources in Azure</span></span>

<span data-ttu-id="bafc0-145">Agora percorremos a criação de um Grupo de recursos, uma VM do Linux e uma VM do Windows Server.</span><span class="sxs-lookup"><span data-stu-id="bafc0-145">We've now walked through how to create a Resource Group, a Linux VM, and a Windows Server VM.</span></span> <span data-ttu-id="bafc0-146">Você também pode criar vários outros tipos de recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="bafc0-146">You can create many other types of Azure resources as well.</span></span>

<span data-ttu-id="bafc0-147">Todos os novos recursos são criados usando um processo consistente padrão de nomenclatura `az <resource type name> create`.</span><span class="sxs-lookup"><span data-stu-id="bafc0-147">All new resources are created using a consistent `az <resource type name> create` naming pattern.</span></span>  <span data-ttu-id="bafc0-148">Por exemplo, para criar um Balanceador de Carga de Rede do Azure que poderíamos associar às nossas VMs recém-criadas, podemos usar o seguinte comando create:</span><span class="sxs-lookup"><span data-stu-id="bafc0-148">For example, to create an Azure Network Load Balancer that we could then associate with our newly created VMs, we can use the following create command:</span></span>

```azurecli-interactive
az network lb create -n MyLoadBalancer -g MyResourceGroup
```

<span data-ttu-id="bafc0-149">Também poderíamos criar uma nova Rede Virtual privada (conhecida como "VNet" no Azure) para nossa infraestrutura usando o seguinte comando create:</span><span class="sxs-lookup"><span data-stu-id="bafc0-149">We could also create a new private Virtual Network (commonly referred to as a "VNet" within Azure) for our infrastructure using the following create command:</span></span>

```azurecli-interactive
az network vnet create -n MyVirtualNetwork -g MyResourceGroup --address-prefix 10.0.0.0/16
```

<span data-ttu-id="bafc0-150">O que torna o Azure e a CLI do Azure tão poderosos é que podemos usar isso não apenas para obter a infraestrutura baseada em nuvem, mas também para criar serviços de plataforma gerenciados.</span><span class="sxs-lookup"><span data-stu-id="bafc0-150">What makes Azure and the Azure CLI powerful is that we can use it not just to get cloud-based infrastructure but also to create managed platform services.</span></span>  <span data-ttu-id="bafc0-151">Os serviços de plataforma gerenciados também podem ser combinados com a infraestrutura para compilar soluções ainda mais eficientes.</span><span class="sxs-lookup"><span data-stu-id="bafc0-151">The managed platform services can also be combined with infrastructure to build even more powerful solutions.</span></span>

<span data-ttu-id="bafc0-152">Por exemplo, é possível usar a CLI do Azure para criar um Serviço de Aplicativo do Azure.</span><span class="sxs-lookup"><span data-stu-id="bafc0-152">For example, you can use the Azure CLI to create an Azure AppService.</span></span>  <span data-ttu-id="bafc0-153">O Serviço de Aplicativo do Azure é um serviço de plataforma gerenciado que fornece uma ótima maneira para hospedar aplicativos Web sem precisar se preocupar com a infraestrutura.</span><span class="sxs-lookup"><span data-stu-id="bafc0-153">Azure AppService is a managed platform service that provides a great way to host web apps without having to worry about infrastructure.</span></span>  <span data-ttu-id="bafc0-154">Depois de criar o Serviço de Aplicativo do Azure, você pode criar dois novos Aplicativos Web do Azure dentro do Serviço de Aplicativo usando os seguintes comandos create:</span><span class="sxs-lookup"><span data-stu-id="bafc0-154">After creating the Azure AppService, you can create two new Azure Web Apps within the AppService using the following create commands:</span></span>

```azurecli-interactive
# Create an Azure AppService that we can host any number of web apps within
az appservice plan create -n MyAppServicePlan -g MyResourceGroup

# Create Two Web Apps within the AppService (note: name param must be a unique DNS entry)
az webapp create -n MyWebApp43432 -g MyResourceGroup --plan MyAppServicePlan
az webapp create -n MyWebApp43433 -g MyResourceGroup --plan MyAppServicePlan
```

<span data-ttu-id="bafc0-155">Depois de compreender os conceitos básicos do padrão `az <resource type name> create`, é fácil criar qualquer coisa.</span><span class="sxs-lookup"><span data-stu-id="bafc0-155">Once you understand the basics of the `az <resource type name> create` pattern, it becomes easy to create anything.</span></span> <span data-ttu-id="bafc0-156">A seguir veja alguns tipos de recursos populares do Azure e comandos create da CLI do Azure correspondentes para criá-los:</span><span class="sxs-lookup"><span data-stu-id="bafc0-156">Following are some popular Azure resource types and the corresponding Azure CLI create commands to create them:</span></span>

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

<span data-ttu-id="bafc0-157">Visite a [Documentação de referência](/cli/azure) para saber mais sobre os outros parâmetros específicos de recursos que você pode passar para cada um dos comandos anteriores e os tipos de recursos que você pode criar.</span><span class="sxs-lookup"><span data-stu-id="bafc0-157">Visit the [Reference documentation](/cli/azure) to learn more about the additional resource-specific parameters that you can pass to each of the preceding commands and the resource types you can create.</span></span>

## <a name="useful-tip-optimizing-create-operations-using---no-wait"></a><span data-ttu-id="bafc0-158">Dica útil: otimização das operações de criação usando --no-wait</span><span class="sxs-lookup"><span data-stu-id="bafc0-158">Useful tip: Optimizing create operations using --no-wait</span></span>

<span data-ttu-id="bafc0-159">Por padrão, ao criar recursos usando a CLI do Azure 2.0, o comando `az <resource type name> create` aguardará até que o recurso seja criado e esteja pronto para uso.</span><span class="sxs-lookup"><span data-stu-id="bafc0-159">By default when you create resources using the Azure CLI 2.0, the `az <resource type name> create` command waits until the resource has been created and is ready for you to use.</span></span>  <span data-ttu-id="bafc0-160">Por exemplo, se você criar uma VM, o comando `az vm create`, por padrão, não retornará até que a VM seja criada e esteja pronta para você usar SSH ou RDP nela.</span><span class="sxs-lookup"><span data-stu-id="bafc0-160">For example, if you create a VM, the `az vm create` command will, by default, not return until the VM is created and is ready for you to SSH or RDP into it.</span></span>

<span data-ttu-id="bafc0-161">Usamos essa abordagem, pois ela facilita a gravação de scripts de automação que contêm várias etapas com dependências (e precisam de uma tarefa anterior para serem concluídas com êxito antes de continuar).</span><span class="sxs-lookup"><span data-stu-id="bafc0-161">We use this approach because it makes it easier to write automation scripts that contain multiple steps with dependencies (and need a prior task to have completed successfully before continuing).</span></span>

<span data-ttu-id="bafc0-162">Se não for necessário esperar a criação de um recurso antes de continuar, você pode usar a opção `no-wait` para iniciar uma ação de criação em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="bafc0-162">If you do not need to wait on creation of a resource before continuing, you can use the `no-wait` option to start a create action in the background.</span></span> <span data-ttu-id="bafc0-163">Você pode continuar usando a CLI para outros comandos.</span><span class="sxs-lookup"><span data-stu-id="bafc0-163">You can continue using the CLI for other commands.</span></span>

<span data-ttu-id="bafc0-164">Por exemplo, o seguinte uso de `az vm create` inicia uma implantação de VM e, em seguida, gera resultados com maior rapidez (e antes da VM ser totalmente inicializada):</span><span class="sxs-lookup"><span data-stu-id="bafc0-164">For example, the following usage of the `az vm create` starts a VM deployment and then return much more quickly (and before the VM has fully booted):</span></span>

```azurecli-interactive
az vm create -n MyLinuxVM2 -g MyResourceGroup --image UbuntuLTS --no-wait
```

<span data-ttu-id="bafc0-165">A abordagem `--no-wait` pode ajudá-lo a otimizar consideravelmente o desempenho de seus scripts de automação.</span><span class="sxs-lookup"><span data-stu-id="bafc0-165">Using the `--no-wait` approach can help you optimize the performance of your automation scripts considerably.</span></span>

## <a name="listing-resources-and-formatting-output"></a><span data-ttu-id="bafc0-166">Listagem de recursos e a formatação de saída</span><span class="sxs-lookup"><span data-stu-id="bafc0-166">Listing resources and formatting output</span></span>

<span data-ttu-id="bafc0-167">Você pode usar o comando `list` na CLI do Azure para localizar e listar os recursos em execução no Azure.</span><span class="sxs-lookup"><span data-stu-id="bafc0-167">You can use the `list` command within the Azure CLI to find and list the resources running in Azure.</span></span>

<span data-ttu-id="bafc0-168">Como acontece com o comando create, você pode listar recursos usando a CLI do Azure 2.0 usando um padrão de nomenclatura `az <resource type name> list` comum que seja consistente em todos os tipos de recursos.</span><span class="sxs-lookup"><span data-stu-id="bafc0-168">Like with the create command, you can list resources using the Azure CLI 2.0 using a common `az <resource type name> list` naming pattern that is consistent across all resource types.</span></span>  <span data-ttu-id="bafc0-169">Há vários formatos de saída e opções de consulta para filtrar e classificar a lista de recursos da maneira que você prefere vê-los.</span><span class="sxs-lookup"><span data-stu-id="bafc0-169">There are various output formats and query options available to filter and sort the list of resources in the way you prefer to see them.</span></span>

<span data-ttu-id="bafc0-170">Por exemplo, `az vm list` mostra a lista de todas as VMs que você possui.</span><span class="sxs-lookup"><span data-stu-id="bafc0-170">For example, `az vm list` shows the list of all VMs you have.</span></span>

```azurecli-interactive
az vm list
```
<span data-ttu-id="bafc0-171">Os valores retornados estão em JSON por padrão (mostrando apenas o resultado parcial para fins de brevidade).</span><span class="sxs-lookup"><span data-stu-id="bafc0-171">The values returned are by default in JSON (only showing partial output for sake of brevity).</span></span>

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

<span data-ttu-id="bafc0-172">Opcionalmente, você pode modificar o formato de saída usando a opção `--output`.</span><span class="sxs-lookup"><span data-stu-id="bafc0-172">You can optionally modify the output format using the `--output` option.</span></span>  <span data-ttu-id="bafc0-173">Execute o comando `az vm list` para ver VMs do Linux e do Windows Server criadas anteriormente, juntamente com as propriedades mais comuns de uma VM, usando a opção de formato *tabela* que é muito fácil de ler:</span><span class="sxs-lookup"><span data-stu-id="bafc0-173">Run the `az vm list` command to see both the Linux and Windows Server VMs created earlier, along with the most common properties of a VM, using the easy to read *table* format option:</span></span>

```azurecli-interactive
az vm list --output table
```

```Output
Name       ResourceGroup    Location
---------  ---------------  ----------
MyLinuxVM  MyResourceGroup  westus2
MyWinVM    MyResourceGroup  westus2
```

<span data-ttu-id="bafc0-174">A opção de saída *tsv* pode ser usada para obter um formato baseado em texto, separado por tabulações, sem nenhum cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="bafc0-174">The *tsv* output option can be used to get a text-based, tab-separated format without any headers.</span></span>  <span data-ttu-id="bafc0-175">Esse formato é útil quando você deseja redirecionar a saída para outra ferramenta baseada em texto como grep.</span><span class="sxs-lookup"><span data-stu-id="bafc0-175">This format is useful when you want to pipe the output into another text-based tool like grep.</span></span>

```azurecli-interactive
az vm list --output tsv
```

```
None    None            /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MyResourceGroup/providers/Microsoft.Compute/virtualMachines/MyLinuxVM        None    None    westus2 MyLinuxVM                   None        Succeeded       MyResourceGroup None                    Microsoft.Compute/virtualMachines       XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
None    None            /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MyResourceGroup/providers/Microsoft.Compute/virtualMachines/MyWinVM  None    None    westus2 MyWinVM                 None    Succeeded       MyResourceGroup None                    Microsoft.Compute/virtualMachines       XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
```
<span data-ttu-id="bafc0-176">Visite o artigo [formatos de saída](format-output-azure-cli.md) para saber mais sobre outras maneiras de listar recursos e formatar a saída.</span><span class="sxs-lookup"><span data-stu-id="bafc0-176">Visit the [output formats](format-output-azure-cli.md) article to learn more about the additional ways to list resources and format the output.</span></span>

## <a name="querying-resources-and-shaping-outputs"></a><span data-ttu-id="bafc0-177">Consulta de recursos e modelagem de saídas</span><span class="sxs-lookup"><span data-stu-id="bafc0-177">Querying resources and shaping outputs</span></span>

<span data-ttu-id="bafc0-178">Geralmente, convém consultar apenas os recursos que atendem a uma condição específica.</span><span class="sxs-lookup"><span data-stu-id="bafc0-178">Often you want to be able to query for only those resources that meet a specific condition.</span></span>

<span data-ttu-id="bafc0-179">O comando `list` conta com suporte interno que facilita a filtragem de recursos pelo nome do Grupo de Recursos.</span><span class="sxs-lookup"><span data-stu-id="bafc0-179">The `list` command has built-in support that makes it easy to filter resources by Resource Group name.</span></span>  <span data-ttu-id="bafc0-180">Por exemplo, você pode passar a um parâmetro `--ResourceGroup` ou `-g` para um comando `list` para recuperar apenas os recursos dentro de um grupo de recursos específico:</span><span class="sxs-lookup"><span data-stu-id="bafc0-180">For example, you can pass either a `--ResourceGroup` or `-g` parameter to a `list` command to only retrieve those resources within a specific resource group:</span></span>


```azurecli-interactive
az vm list -g MyResourceGroup --output table
```

```Output
Name       ResourceGroup    Location
---------  ---------------  ----------
MyLinuxVM  MyResourceGroup  westus2
MyWinVM    MyResourceGroup  westus2
```

<span data-ttu-id="bafc0-181">Para obter ainda um suporte à consulta ainda mais avançado, use o parâmetro `--query` para executar uma consulta JMESPath nos resultados de *qualquer* comando `az`.</span><span class="sxs-lookup"><span data-stu-id="bafc0-181">For even more powerful querying support, you can use the `--query` parameter to execute a JMESPath query on the results of *any* `az` command.</span></span>  <span data-ttu-id="bafc0-182">As consultas JMESPath podem ser usadas para filtrar e também modelar a saída de qualquer resultado retornado.</span><span class="sxs-lookup"><span data-stu-id="bafc0-182">JMESPath queries can be used both to filter as well as shape the output of any returned result.</span></span>

<span data-ttu-id="bafc0-183">Por exemplo, execute o seguinte comando para consultar qualquer recurso de máquina virtual dentro de qualquer grupo de recursos que contenha as letras "Meu":</span><span class="sxs-lookup"><span data-stu-id="bafc0-183">For example, execute the following command to query for any VM resource within any resource group that contains the letters "My":</span></span>

```azurecli-interactive
az vm list --output table --query "[?contains(resourceGroup, 'MY')]"
```

```Output
ResourceGroup    ProvisioningState    Name       Location    VmId
---------------  -------------------  ---------  ----------  ------------------------------------
MYRESOURCEGROUP  Succeeded            MyLinuxVM  westus2     XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
MYRESOURCEGROUP  Succeeded            MyWinVM    westus2     XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
```

<span data-ttu-id="bafc0-184">Em seguida, poderíamos escolher refinar ainda mais a saída usando o recurso de modelagem de consultas JMESPath para também gerar valores diferentes.</span><span class="sxs-lookup"><span data-stu-id="bafc0-184">We could then choose to further refine the output by using the shaping capability of JMESPath queries to output different values as well.</span></span>  <span data-ttu-id="bafc0-185">Por exemplo, o comando a seguir recupera o tipo de disco do sistema operacional que a máquina virtual está usando para determinar se o sistema operacional é baseado em Linux ou Windows:</span><span class="sxs-lookup"><span data-stu-id="bafc0-185">For example, the following command retrieves the type of OS disk the VM is using to determine whether the OS is Linux or Windows based:</span></span>

```azurecli-interactive
az vm list --output table --query "[?contains(resourceGroup, 'MY')].{ VMName:name, OSType:storageProfile.osDisk.osType }"
```

```Output
VMName     OSType
---------  --------
MyLinuxVM  Linux
MyWinVM    Windows
```

<span data-ttu-id="bafc0-186">O suporte a JMESPath na CLI do Azure é poderoso.</span><span class="sxs-lookup"><span data-stu-id="bafc0-186">The JMESPath support in Azure CLI is powerful.</span></span>  <span data-ttu-id="bafc0-187">Saiba mais sobre como usá-lo no artigo [consulta](query-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="bafc0-187">Learn more about how to use it in our [query](query-azure-cli.md) article.</span></span>

## <a name="deleting-resources"></a><span data-ttu-id="bafc0-188">Excluir os recursos</span><span class="sxs-lookup"><span data-stu-id="bafc0-188">Deleting resources</span></span>

<span data-ttu-id="bafc0-189">Você pode usar o comando `delete` na CLI do Azure para excluir os recursos desnecessários.</span><span class="sxs-lookup"><span data-stu-id="bafc0-189">You can use the `delete` command within Azure CLI to delete the resources you no longer need.</span></span> <span data-ttu-id="bafc0-190">Você pode usar o comando `delete` com qualquer recurso, da mesma forma com o comando `create`.</span><span class="sxs-lookup"><span data-stu-id="bafc0-190">You can use the `delete` command with any resource just like you can with the `create` command.</span></span>

```azurecli-interactive
az vm delete -n MyLinuxVM -g MyResourceGroup
```

<span data-ttu-id="bafc0-191">Por padrão, a CLI solicita a confirmação da exclusão.</span><span class="sxs-lookup"><span data-stu-id="bafc0-191">By default the CLI prompts to confirm deletion.</span></span>  <span data-ttu-id="bafc0-192">Você pode suprimir esse aviso para scripts automatizados.</span><span class="sxs-lookup"><span data-stu-id="bafc0-192">You can suppress this prompt for automated scripts.</span></span>

```Output
Are you sure you want to perform this operation? (y/n): y
EndTime                           Name                                  StartTime                         Status
--------------------------------  ------------------------------------  --------------------------------  ---------
2017-02-19T02:35:56.678905+00:00  5b74ab80-9b29-4329-b483-52b406583e2f  2017-02-19T02:33:35.372769+00:00  Succeeded
```

<span data-ttu-id="bafc0-193">Também é possível usar o comando `delete` para excluir vários recursos ao mesmo tempo.</span><span class="sxs-lookup"><span data-stu-id="bafc0-193">You can also use the `delete` command to delete many resources at a time.</span></span> <span data-ttu-id="bafc0-194">Por exemplo, o comando a seguir exclui todos os recursos no grupo de recursos "MyResourceGroup" que usamos para todos os exemplos nesse tutorial de Introdução.</span><span class="sxs-lookup"><span data-stu-id="bafc0-194">For example, the following command deletes all the resources in the "MyResourceGroup" resource group that we've used for all the samples in this Get Started tutorial.</span></span>

```azurecli-interactive
az group delete -n MyResourceGroup
```

```Output
Are you sure you want to perform this operation? (y/n): y
```

## <a name="get-samples"></a><span data-ttu-id="bafc0-195">Obter exemplos</span><span class="sxs-lookup"><span data-stu-id="bafc0-195">Get samples</span></span>

<span data-ttu-id="bafc0-196">Para saber mais sobre como usar a CLI do Azure, consulte nossos scripts mais comuns para [VMs do Linux](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json), [VMs do Windows](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json), [Aplicativos Web](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json) e [Banco de Dados SQL](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json).</span><span class="sxs-lookup"><span data-stu-id="bafc0-196">To learn more about ways to use the Azure CLI, check out our most common scripts for [Linux VMs](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json), [Windows VMs](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json), [Web apps](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json), and [SQL Database](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json).</span></span>

## <a name="read-the-api-reference-docs"></a><span data-ttu-id="bafc0-197">Leia os documentos de referência de API</span><span class="sxs-lookup"><span data-stu-id="bafc0-197">Read the API reference docs</span></span>

[<span data-ttu-id="bafc0-198">Referência de API</span><span class="sxs-lookup"><span data-stu-id="bafc0-198">API reference</span></span>](/cli/azure)

## <a name="get-help"></a><span data-ttu-id="bafc0-199">Obter ajuda</span><span class="sxs-lookup"><span data-stu-id="bafc0-199">Get help</span></span>

<span data-ttu-id="bafc0-200">A CLI do Azure tem documentação de ajuda interna que corresponde à nossa documentação da Web que pode ser executada na linha de comando:</span><span class="sxs-lookup"><span data-stu-id="bafc0-200">The Azure CLI has built-in help documentation, which matches our web documentation that you can run from the command line:</span></span>

```azurecli-interactive
az [command-group [command]] -h
```

<span data-ttu-id="bafc0-201">Por exemplo, para ver quais comandos e subgrupos estão disponíveis para VMs, use:</span><span class="sxs-lookup"><span data-stu-id="bafc0-201">For example, to see what commands and subgroups are available for VMs, use:</span></span>

```azurecli-interactive
az vm -h
```

<span data-ttu-id="bafc0-202">Para obter ajuda com o comando para criar uma VM, use:</span><span class="sxs-lookup"><span data-stu-id="bafc0-202">To get help with the command to create a VM, use:</span></span>

```azurecli-interactive
az vm create -h
```

## <a name="switch-from-azure-cli-10"></a><span data-ttu-id="bafc0-203">Alternar a partir da CLI do Azure 1.0</span><span class="sxs-lookup"><span data-stu-id="bafc0-203">Switch from Azure CLI 1.0</span></span>

<span data-ttu-id="bafc0-204">Se já souber como usar a CLI do Azure 1.0 (azure.js), você verá lugares onde os comandos não são exatamente os mesmos.</span><span class="sxs-lookup"><span data-stu-id="bafc0-204">If you already know how to use Azure CLI 1.0 (azure.js), you'll notice places where the commands aren't quite the same.</span></span>
<span data-ttu-id="bafc0-205">Às vezes, os comandos para executar uma tarefa são significativamente diferentes.</span><span class="sxs-lookup"><span data-stu-id="bafc0-205">Sometimes the commands to perform a task are significantly different.</span></span>
<span data-ttu-id="bafc0-206">Para ajudá-lo a fazer a transição da CLI do Azure 1.0 para a CLI do Azure 2.0, iniciamos esse [mapeamento do comando](https://github.com/Azure/azure-cli/blob/master/doc/azure2az_commands.rst).</span><span class="sxs-lookup"><span data-stu-id="bafc0-206">To help you make the switch from Azure CLI 1.0 to Azure CLI 2.0, we've started this [command mapping](https://github.com/Azure/azure-cli/blob/master/doc/azure2az_commands.rst).</span></span>

## <a name="send-us-your-feedback"></a><span data-ttu-id="bafc0-207">Envie-nos seus comentários</span><span class="sxs-lookup"><span data-stu-id="bafc0-207">Send us your feedback</span></span>

```azurecli-interactive
az feedback
```
