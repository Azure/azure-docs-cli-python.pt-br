---
title: Referências da CLI do Azure para a Rede do Azure
description: Página de aterrissagem da referência da CLI do Azure para a Rede do Azure
author: dbradish-microsoft
manager: barbkess
ms.devlang: azurecli
ms.topic: reference
ms.date: 06/30/2020
ms.author: dbradish
ms.service: azure-cli
ms.reviewer: mohnader
ms.custom: devx-track-azurecli
ms.openlocfilehash: 2155be0bca6b6aa297e4be07a685a379892523c6
ms.sourcegitcommit: 5d29362589078b66d15f5cd494fe903a5195658d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/25/2020
ms.locfileid: "91225908"
---
# <a name="azure-cli-for-azure-network"></a>CLI do Azure para a Rede do Azure

A [CLI do Azure](./what-is-azure-cli.md) (Interface de Linha de Comando do Azure) é um conjunto de comandos usados para criar e gerenciar recursos do Azure.  A CLI está disponível em vários serviços do Azure, incluindo a Rede do Azure, oferecendo a você a capacidade de gerenciar serviços de rede por meio de uma linha de comando.

## <a name="references-for-azure-network"></a>Referências para a Rede do Azure

A experiência da CLI da Rede do Azure é composta por duas partes: **principal** e **extensão**.  Os comandos principais da CLI do Azure são fornecidos como parte da CLI e têm suporte total.  Uma extensão fornece acesso a comandos experimentais e de pré-lançamento e deve ser instalada antes do uso.  Scripts de instalação de exemplo são fornecidos em [Instalação de referências de extensão](#installing-extension-references).

Veja [az network](/cli/azure/network) para obter uma lista completa de referências principais da CLI do Azure para a Rede do Azure.  Siga os links abaixo para obter referências de extensão.

### <a name="virtual-network"></a>Rede virtual

| Subgrupo | Referência | Use | É extensão
|-|-|-|-|
| Dispositivo | [az network virtual-appliance](/cli/azure/network/virtual-appliance) | Gerenciar a solução de virtualização da Rede do Azure.
| DNS | [az network private-dns](/cli/azure/network/private-dns) | Gerenciar domínios de DNS privado no Azure. |
| Ponto de extremidade | [az network service-endpoint](/cli/azure/network/service-endpoint) | Gerenciar políticas relacionadas a pontos de extremidade de serviço. |
| NAT | [az network nat](/cli/azure/network/nat) | Gerenciar recursos de conversão de endereços de rede. |
| NIC | [az network nic](/cli/azure/network/nic) | Gerenciar adaptadores de rede. |
| Emparelhamento | [az peering](/cli/azure/ext/peering/peering) | Gerenciar o emparelhamento. | sim
| Perfil | [az network profile](/cli/azure/network/profile) | Gerenciar perfis de rede. |
| Rota | [az network route-filter](/cli/azure/network/route-filter) | Gerenciar filtros de rota. |
| Rota | [az network route-table](/cli/azure/network/route-table) | Gerenciar tabelas de rotas. |
| VMware | [az network vmware](/cli/azure/ext/vmware/vmware) | Comandos para gerenciar Soluções VMware no Azure. | sim
| vNet | [az network vnet](/cli/azure/network/vnet) | Gerenciar Redes Virtuais do Azure. |
| vNet | [az network vnet-tap](/cli/azure/ext/virtual-network-tap/network/vnet/tap) | Gerenciar TAPs de rede virtual. | sim
| vNet | [az network vnet-gateway](/cli/azure/network/vnet-gateway) | Usar um gateway de Rede Virtual do Azure para estabelecer conectividade segura entre locais. |

### <a name="wan-and-on-premise-connectivity"></a>Conectividade WAN e local

| Subgrupo | Referência | Use | É extensão
|-|-|-|-|
| Conexão cruzada | [az network cross-connection](/cli/azure/ext/express-route-cross-connection/network/cross-connection) | Gerenciar recursos da Rede do Azure. | sim
| ExpressRoute | [az network express-route](/cli/azure/network/express-route) | Gerencie os hubs IoT do Azure. |
| vHub | [az network vhub](/cli/azure/ext/virtual-wan/network/vhub) | Gerenciar hubs virtuais. | sim
| VPN | [az network vpn-connection](/cli/azure/network/vpn-connection) | Gerenciar conexões VPN. |
| VPN | [az network vpn-gateway](/cli/azure/ext/virtual-wan/network/vpn-gateway) | Gerenciar gateways de VPN. | sim
| VPN | [az network vpn-site](/cli/azure/ext/virtual-wan/network/vpn-site) | Gerenciar configurações de site VPN. | sim
| vRouter | [az network vrouter](/cli/azure/network/vrouter) | Gerenciar o roteador virtual. |
| vWAN | [az network vwan](/cli/azure/ext/virtual-wan/network/vwan) | Gerenciar WANs virtuais. | sim

### <a name="load-balancing-and-ip"></a>Balanceamento de carga e IP

| Subgrupo | Referência | Use | É extensão
|-|-|-|-|
| Gateway de Aplicativo | [az network application-gateway](/cli/azure/network/application-gateway) | Gerenciar o roteamento no nível do aplicativo e os serviços de balanceamento de carga. |
| Balancear carga | [az network lb](/cli/azure/network/lb) | Gerenciar e configurar balanceadores de carga. |
| IP | [az network ip-group](/cli/azure/ext/ip-group/network/ip-group) | Gerenciar IpGroups. | sim
| IP | [az network public-ip](/cli/azure/network/public-ip) | Gerenciar endereços IP públicos. |
| Front Door | [az network front-door](/cli/azure/ext/front-door/network/front-door) | Gerenciar recursos do Front Door da rede. | sim
| Gateway local | [az network local-gateway](/cli/azure/network/local-gateway) | Gerenciar gateways locais. |
| Gerenciador de tráfego | [az network traffic-manager](/cli/azure/network/traffic-manager) | Gerencie o roteamento do tráfego de entrada. |

### <a name="security"></a>Segurança

| Subgrupo | Referência | Use | É extensão
|-|-|-|-|
| ASG | [az asg](/cli/azure/network/asg) | Gerenciar grupos de segurança do aplicativo. |
| Bastion | [az network bastion](/cli/azure/network/bastion) | Gerenciar o bastion host do Azure. |
| DDoS | [az network ddos-protection](/cli/azure/network/ddos-protection) | Gerenciar Planos de Proteção contra DDoS. |
| Firewall | [az network firewall](/cli/azure/ext/azure-firewall/network/firewall) | Gerenciar e configurar Firewalls do Azure. | sim
| Firewall | [az network security-partner-provider](/cli/azure/network/security-partner-provider) | Gerenciar o provedor de parceiros de segurança do Azure. |
| NSG | [az network nsg](/cli/azure/network/nsg)| Gerenciar grupos de segurança de rede do Azure. |
| Ponto de extremidade privado | [az network private-endpoint](/cli/azure/network/private-endpoint) | Gerenciar pontos de extremidade privados. |
| Ponto de extremidade privado | [az network private-endpoint-connection](/cli/azure/network/private-endpoint-connection) | Gerenciar conexões de ponto de extremidade privado. |
| Link privado | [az network private-link-resource](/cli/azure/network/private-link-resource) | Gerenciar recursos do link privado. |
| Link privado | [az network private-link-service](/cli/azure/network/private-link-service) | Gerenciar serviços do link privado. |

### <a name="monitoring"></a>Monitoramento

| Subgrupo | Referência | Use | É extensão
|-|-|-|-|
| Observador | [az network watcher](/cli/azure/network/watcher) | Gerenciar o Observador de Rede do Azure. |

### <a name="list"></a>Lista

| Subgrupo | Referência | Use | É extensão
|-|-|-|-|
| Serviço | [az network list-service-aliases](/cli/azure/network#az-network-list-service-aliases) | Listar os aliases de serviço disponíveis na região que podem ser usados para as políticas de ponto de extremidade de serviço. |
| Serviço | [az network list-service-tags](/cli/azure/network#az-network-list-service-tags) | Lista todas as marcas de serviço que pertencem a recursos diferentes. |
| Uso | [az network list-usages](/cli/azure/network#az-network-list-usages) | Lista o número de recursos de rede em uma região que são usados em uma cota de assinatura. |

## <a name="installing-extension-references"></a>Instalar referências de extensão

As referências de extensão da CLI do Azure devem ser instaladas antes do uso.  O comando [az extension add](./azure-cli-extensions-overview.md) instala uma referência de extensão por nome.  Saiba mais sobre as referências de extensão em [Usar extensões com a CLI do Azure](./azure-cli-extensions-overview.md).

```azurecli
## get a list of available Azure CLI extensions
az extension list-available --output table

# install the extension for az network express-route-cross-connection
az extension add --name express-route-cross-connection

# install the extension for az network front-door
az extension add --name front-door

# install the extension for az network virtual-wan
az extension add --name virtual-wan

# install the extension for az network vm-repair
az extension add --name virtual-network-tap

# install the extension for az network vmware
az extension add --name vmware

# install the extension for az peering
az extension add --name peering
```

## <a name="popular-network-articles-using-the-azure-cli"></a>Artigos populares de rede que usam a CLI do Azure

- [Criar máquinas virtuais](/cli/azure/azure-cli-vm-tutorial)
- [Criar uma rede virtual](/azure/virtual-network/quick-create-cli)
- [Exemplos de CLI do Azure para máquinas virtuais do Windows](/azure/virtual-machines/windows/cli-samples?toc=%2Fcli%2Fazure%2Ftoc.json&bc=%2Fcli%2Fazure%2Fbreadcrumb%2Ftoc.json)
- [Criar um conjunto de dimensionamento de máquinas virtuais](/azure/virtual-machine-scale-sets/quick-create-cli)
- [Executar Azure IoT Edge em Máquinas Virtuais do Ubuntu](/azure/iot-edge/how-to-install-iot-edge-ubuntuvm#deploy-from-azure-cli)
- [Balancear carga de máquinas virtuais do Linux no Azure](/azure/virtual-machines/linux/tutorial-load-balancer)
- [Criar e gerenciar redes virtuais do Azure para VMs do Linux](/azure/virtual-machines/linux/tutorial-virtual-network)
- [Configurar um ponto de extremidade de serviço para o Cosmos DB](/azure/cosmos-db/how-to-configure-vnet-service-endpoint#configure-using-cli)

## <a name="see-also"></a>Confira também

- [Introdução à CLI do Azure](./get-started-with-azure-cli.md) para saber mais sobre a instalação e a conexão.

- Descubra referências adicionais de [núcleo](/cli/azure/reference-index) e de [extensão](./azure-cli-extensions-list.md) na documentação da CLI do Azure.

- Gerencie máquinas virtuais do Linux ou do Windows com [az vm](/cli/azure/vm).