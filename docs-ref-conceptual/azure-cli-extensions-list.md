---
title: Доступные расширения для Azure CLI
description: Полный список официально поддерживаемых расширений для Azure CLI.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 01/06/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 276bd619408760416910c099dee2aa8377011d0d
ms.sourcegitcommit: 2c18e8fc2da012bf8ceb2aa77e0671f2413c43c9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/08/2019
ms.locfileid: "54071885"
---
# <a name="available-extensions-for-the-azure-cli"></a>Доступные расширения для Azure CLI

В этой статье приведен полный список доступных расширений для Azure CLI, которые поддерживает корпорация Майкрософт.

Список расширений также доступен из CLI. Для этого выполните команду [az extension list-available](/cli/azure/extension?view=azure-cli-latest#az-extension-list-available):

```azurecli-interactive
az extension list-available --output table
```

| ИМЯ | Version (версия) | Сводка | Предварительный просмотр |
|------|---------|---------|---------|
| [aem](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Управление расширениями для улучшенного мониторинга Azure для SAP. |  |
| [aks-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/aks-preview) | 0.1.0 | Предварительное знакомство с будущими возможностями AKS. | Yes |
| [alias](https://github.com/Azure/azure-cli-extensions) | 0.5.2 | Поддержка псевдонимов команд. | Yes |
| [azure-batch-cli-extensions](https://github.com/Azure/azure-batch-cli-extensions) | 2.5.1 | Дополнительные команды для работы с пакетной службой Azure. |  |
| [azure-cli-iot-ext](https://github.com/azure/azure-iot-cli-extension) | 0.6.1 | Предоставление уровня команд плоскости данных для Центра Интернета вещей Azure, IoT Edge и службы подготовки устройств к добавлению в Центр Интернета вещей. |  |
| [azure-devops](https://github.com/Microsoft/vsts-cli/tree/azuredevopscli-dev) | 0.1.0 | Инструменты для управления Azure DevOps. | Yes |
| [azure-firewall](https://github.com/Azure/azure-cli-extensions/tree/master/src/azure-firewall) | 0.1.1 | Управление ресурсами Брандмауэра Azure. | Yes |
| [botservice](https://github.com/Azure/azure-cli-extensions) | 0.4.3 | Исправления ошибок в собственном командном модуле botservice cli. | Yes |
| [dev-spaces-preview](https://github.com/Azure/azure-cli-extensions) | 0.1.6 | Рабочие среды Azure для разработчиков предоставляют быстрый итеративный интерфейс разработки Kubernetes для команд. | Yes |
| [dms-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/dms-preview) | 0.6.0 | Поддержка новых сценариев Database Migration Service. | Yes |
| [dns](https://github.com/Azure/azure-cli-extensions) | 0.0.2 | Расширение Azure CLI для зон DNS. |  |
| [eventgrid](https://github.com/Azure/azure-cli-extensions) | 0.4.0 | Поддержка функций службы "Сетка событий Azure" версии 2018-09-15-preview | Yes |
| [express-route](https://github.com/Azure/azure-cli-extensions/tree/master/src/express-route) | 0.1.3 | Управление ExpressRoute с помощью предварительных версий функций. | Yes |
| [express-route-cross-connection](https://github.com/Azure/azure-cli-extensions/tree/master/src/express-route-cross-connection) | 0.1.0 | Управление пользовательскими каналами ExpressRoute с использованием перекрестного подключения ExpressRoute. |  |
| [find](https://github.com/Azure/azure-cli-extensions/tree/master/src/find) | 0.3.0 | Интеллектуальный запрос для получения сведений CLI. | Yes |
| [front-door](https://github.com/Azure/azure-cli-extensions/tree/master/src/front-door) | 0.1.1 | Управление сетевыми службами Front Door. | Yes |
| [image-copy-extension](https://github.com/Azure/azure-cli-extensions) | 0.0.9 | Поддержка копирования управляемых образов виртуальных машин в другие регионы |  |
| [интерактивный](https://github.com/Azure/azure-cli) | 0.4.1 | Интерактивная оболочка командной строки Microsoft Azure | Yes |
| [keyvault-preview](https://github.com/Azure/azure-keyvault-cli-extension) | 0.1.3 | Команды предварительной версии Azure Key Vault. | Yes |
| [log-analytics](https://github.com/Azure/azure-cli-extensions/tree/master/src/log-analytics) | 0.1.3 | Поддержка возможностей запросов Azure Log Analytics. | Yes |
| [managementgroups](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Расширение Azure CLI для групп управления. |  |
| [managementpartner](https://github.com/Azure/azure-cli-extensions) | 0.1.2 | Поддержка партнера управления (предварительная версия). |  |
| [mesh](https://github.com/Azure/azure-cli-extensions) | 0.10.2 | Поддержка Сетки Microsoft Azure Service Fabric (общедоступная предварительная версия) | Yes |
| [rdbms-vnet](https://github.com/Azure/azure-cli-extensions) | 10.0.0 | Поддержка правил виртуальной сети в ресурсах Azure MySQL и Azure PostgreSQL. |  |
| [resource-graph](https://github.com/Azure/azure-cli-extensions/tree/master/src/resource-graph) | 0.1.8 | Поддержка запросов к ресурсам Azure с помощью Resource Graph. | Yes |
| [sap-hana](https://github.com/Azure/azure-hanaonazure-cli-extension) | 0.1.6 | Дополнительные команды для работы с экземплярами SAP HanaOnAzure. |  |
| [signalr](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Поддержка управления с помощью SignalR (предварительная версия). | Yes |
| [sqlvm-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/sqlvm-preview) | 0.1.0 | Инструменты для управления виртуальными машинами SQL, группами и прослушивателями групп доступности. | Yes |
| [storage-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/storage-preview) | 0.2.1 | Предварительная версия ожидаемых функций хранилища. | Yes |
| [subscription](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Поддержка управления подписками (предварительная версия). |  |
| [virtual-network-tap](https://github.com/Azure/azure-cli-extensions/tree/master/src/virtual-network-tap) | 0.1.0 | Управление точками доступа к виртуальным сетям (VTAP). | Yes |
| [virtual-wan](https://github.com/Azure/azure-cli-extensions/tree/master/src/virtual-wan) | 0.1.0 | Управление виртуальными глобальными сетями, концентраторами, шлюзами и сайтами VPN. | Yes |
| [webapp](https://github.com/Azure/azure-cli-extensions) | 0.2.16 | Дополнительные команды для Службы приложений Azure. | Yes |