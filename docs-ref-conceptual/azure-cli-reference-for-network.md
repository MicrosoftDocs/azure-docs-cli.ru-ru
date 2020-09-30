---
title: Справочники по Azure CLI для Сети Azure
description: Целевая страница справочника по Azure CLI для Сети Azure
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
ms.contentlocale: ru-RU
ms.lasthandoff: 09/25/2020
ms.locfileid: "91225921"
---
# <a name="azure-cli-for-azure-network"></a>Azure CLI для Сети Azure

Интерфейс командной строки Azure ([Azure CLI](./what-is-azure-cli.md)) — это набор команд для создания ресурсов Azure и управления ими.  CLI используется во многих службах Azure, включая Сеть Azure, позволяя управлять сетевыми службами из командной строки.

## <a name="references-for-azure-network"></a>Справочники для Сети Azure

Интерфейс командной строки для Сети Azure состоит из двух частей: **базовой** и **расширения**.  Команды базового Azure CLI входят в состав CLI и полностью поддерживаются.  Расширение предоставляет доступ к экспериментальным командам и предварительным версиям команд, но перед использованием его нужно установить.  Примеры скриптов установки см. в разделе [Установка справочников по расширению](#installing-extension-references).

Полный список справочников по базовому Azure CLI для Сети Azure см. в описании [az network](/cli/azure/network).  Справочники по расширению см. по ссылкам ниже.

### <a name="virtual-network"></a>Виртуальная сеть

| Подгруппа | Справочник | Использование | Является расширением
|-|-|-|-|
| Устройство | [az network virtual-appliance](/cli/azure/network/virtual-appliance) | Управление сетевым виртуальным модулем Azure.
| DNS | [az network private-dns](/cli/azure/network/private-dns) | Управление доменами Частной зоны DNS в Azure. |
| Конечная точка | [az network service-endpoint](/cli/azure/network/service-endpoint) | Управление политиками, относящимися к конечным точкам служб. |
| NAT | [az network nat](/cli/azure/network/nat) | Управление ресурсами преобразования сетевых адресов. |
| Сетевая карта | [az network nic](/cli/azure/network/nic) | Управление сетевыми интерфейсами. |
| Пиринг | [az peering](/cli/azure/ext/peering/peering) | Управление пирингом. | да
| Профиль | [az network profile](/cli/azure/network/profile) | Управление сетевыми профилями. |
| Маршрут | [az network route-filter](/cli/azure/network/route-filter) | Управление фильтрами маршрутов. |
| Маршрут | [az network route-table](/cli/azure/network/route-table) | Управление таблицами маршрутизации. |
| VMware | [az network vmware](/cli/azure/ext/vmware/vmware) | Команды для управления Решениями Azure VMware. | да
| Виртуальная сеть | [az network vnet](/cli/azure/network/vnet) | Управление виртуальными сетями Azure. |
| Виртуальная сеть | [az network vnet-tap](/cli/azure/ext/virtual-network-tap/network/vnet/tap) | Управление точками TAP виртуальных сетей. | да
| Виртуальная сеть | [az network vnet-gateway](/cli/azure/network/vnet-gateway) | Используйте шлюз виртуальной сети Azure, чтобы установить безопасное подключение между сетями. |

### <a name="wan-and-on-premise-connectivity"></a>WAN и локальные подключения

| Подгруппа | Справочник | Использование | Является расширением
|-|-|-|-|
| Перекрестное подключение | [az network cross-connection](/cli/azure/ext/express-route-cross-connection/network/cross-connection) | Управление ресурсами Сети Azure. | да
| ExpressRoute | [az network express-route](/cli/azure/network/express-route) | Управление центрами Интернета вещей Azure. |
| vHub | [az network vhub](/cli/azure/ext/virtual-wan/network/vhub) | Управление виртуальными концентраторами. | да
| Виртуальная частная сеть | [az network vpn-connection](/cli/azure/network/vpn-connection) | Управление VPN-подключениями. |
| Виртуальная частная сеть | [az network vpn-gateway](/cli/azure/ext/virtual-wan/network/vpn-gateway) | Управление VPN-шлюзами. | да
| Виртуальная частная сеть | [az network vpn-site](/cli/azure/ext/virtual-wan/network/vpn-site) | Управление конфигурациями сайтов VPN. | да
| vRouter | [az network vrouter](/cli/azure/network/vrouter) | Управление виртуальным маршрутизатором. |
| vWAN | [az network vwan](/cli/azure/ext/virtual-wan/network/vwan) | Управление виртуальными глобальными сетями. | да

### <a name="load-balancing-and-ip"></a>Балансировка нагрузки и IP-адресация

| Подгруппа | Справочник | Использование | Является расширением
|-|-|-|-|
| Шлюз приложений | [az network application-gateway](/cli/azure/network/application-gateway) | Управление маршрутизацией на уровне приложений и службами балансировки нагрузки. |
| Балансировка нагрузки | [az network lb](/cli/azure/network/lb) | Управление подсистемами балансировки нагрузки и их настройка. |
| IP-адрес | [az network ip-group](/cli/azure/ext/ip-group/network/ip-group) | Управление группами IP-адресов. | да
| IP-адрес | [az network public-ip](/cli/azure/network/public-ip) | Управление общедоступными IP-адресами. |
| Front Door | [az network front-door](/cli/azure/ext/front-door/network/front-door) | Управление сетевыми ресурсами Front Door. | да
| Локальный шлюз | [az network local-gateway](/cli/azure/network/local-gateway) | Управление локальными шлюзами. |
| Диспетчер трафика | [az network traffic-manager](/cli/azure/network/traffic-manager) | Управление маршрутизацией входящего трафика. |

### <a name="security"></a>Безопасность

| Подгруппа | Справочник | Использование | Является расширением
|-|-|-|-|
| ASG | [az asg](/cli/azure/network/asg) | Управление группами безопасности приложений. |
| Бастион | [az network bastion](/cli/azure/network/bastion) | Управление узлом-бастионом Azure. |
| DDoS | [az network ddos-protection](/cli/azure/network/ddos-protection) | Управление планами Защиты от атак DDoS. |
| Брандмауэр | [az network firewall](/cli/azure/ext/azure-firewall/network/firewall) | Управление Брандмауэрами Azure и их настройка. | да
| Брандмауэр | [az network security-partner-provider](/cli/azure/network/security-partner-provider) | Управление поставщиком партнера по безопасности Azure. |
| Группа безопасности сети (NSG) | [az network nsg](/cli/azure/network/nsg)| Управление группами безопасности сети Azure. |
| Частная конечная точка | [az network private-endpoint](/cli/azure/network/private-endpoint) | Управление частными конечными точками. |
| Частная конечная точка | [az network private-endpoint-connection](/cli/azure/network/private-endpoint-connection) | Управление подключениями к частным конечным точкам. |
| Приватный канал | [az network private-link-resource](/cli/azure/network/private-link-resource) | Управление ресурсами Приватного канала. |
| Приватный канал | [az network private-link-service](/cli/azure/network/private-link-service) | Управление службами Приватного канала. |

### <a name="monitoring"></a>Наблюдение

| Подгруппа | Справочник | Использование | Является расширением
|-|-|-|-|
| Наблюдатель за сетями | [az network watcher](/cli/azure/network/watcher) | Управление Наблюдателем за сетями Azure. |

### <a name="list"></a>Список

| Подгруппа | Справочник | Использование | Является расширением
|-|-|-|-|
| Служба | [az network list-service-aliases](/cli/azure/network#az-network-list-service-aliases) | Вывод списка доступных псевдонимов служб в регионе, который можно использовать для политик конечной точки службы. |
| Служба | [az network list-service-tags](/cli/azure/network#az-network-list-service-tags) | Вывод списка всех тегов служб, принадлежащих разным ресурсам. |
| Использование | [az network list-usages](/cli/azure/network#az-network-list-usages) | Вывод количества сетевых ресурсов в регионе, используемых с учетом квоты подписки. |

## <a name="installing-extension-references"></a>Установка ссылок на расширения

Перед использованием необходимо установить расширения Azure CLI из справочника.  Команда [az extension add](./azure-cli-extensions-overview.md) устанавливает ссылку на расширение по имени.  Узнайте больше о расширениях из статьи [Использование расширений с Azure CLI](./azure-cli-extensions-overview.md).

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

## <a name="popular-network-articles-using-the-azure-cli"></a>Популярные статьи по работе с Azure CLI для сети

- [Создание виртуальных машин](/cli/azure/azure-cli-vm-tutorial)
- [Создание виртуальной сети](/azure/virtual-network/quick-create-cli)
- [Azure CLI Samples for Windows virtual machines](/azure/virtual-machines/windows/cli-samples?toc=%2Fcli%2Fazure%2Ftoc.json&bc=%2Fcli%2Fazure%2Fbreadcrumb%2Ftoc.json) (Примеры Azure CLI для виртуальных машин Windows)
- [Создание масштабируемого набора виртуальных машин](/azure/virtual-machine-scale-sets/quick-create-cli)
- [Запуск Azure IoT Edge на виртуальных машинах Ubuntu](/azure/iot-edge/how-to-install-iot-edge-ubuntuvm#deploy-from-azure-cli)
- [Балансировка нагрузки виртуальных машин Linux в Azure](/azure/virtual-machines/linux/tutorial-load-balancer)
- [Создание и администрирование виртуальных сетей Azure для виртуальных машин Linux](/azure/virtual-machines/linux/tutorial-virtual-network)
- [Настройка конечной точки службы для Cosmos DB](/azure/cosmos-db/how-to-configure-vnet-service-endpoint#configure-using-cli)

## <a name="see-also"></a>См. также раздел

- [Начните работу с Azure CLI](./get-started-with-azure-cli.md), чтобы узнать об установке и входе.

- Найдите дополнительные справочники по [основным командам](/cli/azure/reference-index) и [командам расширения](./azure-cli-extensions-list.md) в документации по Azure CLI.

- Управление виртуальными машинами Linux или Windows с помощью [az vm](/cli/azure/vm).