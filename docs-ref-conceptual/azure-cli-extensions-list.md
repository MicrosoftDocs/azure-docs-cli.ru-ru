---
title: Доступные расширения для Azure CLI
description: Полный список официально поддерживаемых расширений для Azure CLI.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/26/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: e429fb30bdfeb7eb1bb9d93b21e9b02a7f25aca9
ms.sourcegitcommit: 6fb38e801096708c4922b10778d6582776a8ac91
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "71317928"
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
| [aks-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/aks-preview) | 0.4.16 | Предварительное знакомство с будущими возможностями AKS. | Yes |
| [alias](https://github.com/Azure/azure-cli-extensions) | 0.5.2 | Поддержка псевдонимов команд. | Yes |
| [appconfig](https://github.com/Azure/azure-cli-extensions) | 0.5.0 | Предварительное знакомство с новыми возможностями службы конфигурации приложений. | Yes |
| [application-insights](https://github.com/Azure/azure-cli-extensions/tree/master/src/application-insights) | 0.1.1 | Поддержка компонентов управления Application Insights, а также запрашивание метрик, событий и журналов из таких компонентов. | Yes |
| [azure-batch-cli-extensions](https://github.com/Azure/azure-batch-cli-extensions) | 5.0.0 | Дополнительные команды для работы с пакетной службой Azure. |  |
| [azure-cli-iot-ext](https://github.com/azure/azure-iot-cli-extension) | 0.8.2 | Предоставление уровня команд плоскости данных для Центра Интернета вещей Azure, IoT Edge и службы подготовки устройств к добавлению в Центр Интернета вещей. |  |
| [azure-cli-ml](https://docs.microsoft.com/azure/machine-learning/service/) | 1.0.62 | Командный модуль средств командной строки Azure ML в Microsoft Azure |  |
| [azure-devops](https://github.com/Microsoft/azure-devops-cli-extension) | 0.12.0 | Инструменты для управления Azure DevOps. |  |
| [azure-firewall](https://github.com/Azure/azure-cli-extensions/tree/master/src/azure-firewall) | 0.1.3 | Управление ресурсами Брандмауэра Azure. | Yes |
| [db-up](https://github.com/Azure/azure-cli-extensions/tree/master/src/db-up) | 0.1.13 | Дополнительные команды для упрощения рабочих процессов Базы данных Azure. | Yes |
| [dev-spaces](https://github.com/Azure/azure-cli-extensions) | 1.0.3 | Рабочие среды Azure для разработчиков предоставляют быстрый итеративный интерфейс разработки Kubernetes для команд. |  |
| [dev-spaces-preview](https://github.com/Azure/azure-cli-extensions) | 0.1.6 | Рабочие среды Azure для разработчиков предоставляют быстрый итеративный интерфейс разработки Kubernetes для команд. | Yes |
| [dms-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/dms-preview) | 0.9.0 | Поддержка новых сценариев Database Migration Service. | Yes |
| [dns](https://github.com/Azure/azure-cli-extensions) | 0.0.2 | Расширение Azure CLI для зон DNS. |  |
| [eventgrid](https://github.com/Azure/azure-cli-extensions) | 0.4.3 | Командный модуль средств командной строки Сетки событий в Microsoft Azure. | Yes |
| [express-route](https://github.com/Azure/azure-cli-extensions/tree/master/src/express-route) | 0.1.3 | Управление ExpressRoute с помощью предварительных версий функций. | Yes |
| [express-route-cross-connection](https://github.com/Azure/azure-cli-extensions/tree/master/src/express-route-cross-connection) | 0.1.1 | Управление пользовательскими каналами ExpressRoute с использованием перекрестного подключения ExpressRoute. |  |
| [find](https://github.com/Azure/azure-cli-extensions/tree/master/src/find) | 0.3.0 | Интеллектуальный запрос для получения сведений CLI. | Yes |
| [front-door](https://github.com/Azure/azure-cli-extensions/tree/master/src/front-door) | 1.0.0 | Управление сетевыми службами Front Door. |  |
| [healthcareapis](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Расширение программы командной строки Microsoft Azure HealthCareApis | Yes |
| [image-copy-extension](https://github.com/Azure/azure-cli-extensions) | 0.2.1 | Поддержка копирования управляемых образов виртуальных машин в другие регионы |  |
| [интерактивный](https://github.com/Azure/azure-cli) | 0.4.3 | Интерактивная оболочка командной строки Microsoft Azure | Yes |
| [keyvault-preview](https://github.com/Azure/azure-keyvault-cli-extension) | 0.1.3 | Команды предварительной версии Azure Key Vault. | Yes |
| [log-analytics](https://github.com/Azure/azure-cli-extensions/tree/master/src/log-analytics) | 0.1.3 | Поддержка возможностей запросов Azure Log Analytics. | Yes |
| [managementgroups](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Расширение Azure CLI для групп управления. |  |
| [managementpartner](https://github.com/Azure/azure-cli-extensions) | 0.1.2 | Поддержка партнера управления (предварительная версия). |  |
| [mesh](https://github.com/Azure/azure-cli-extensions) | 0.10.6 | Поддержка Сетки Microsoft Azure Service Fabric (общедоступная предварительная версия) | Yes |
| [mixed-reality](https://github.com/Azure/azure-cli-extensions) | 0.0.1 | Расширение Azure CLI смешанной реальности. |  |
| [netappfiles-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/netappfiles-preview) | 0.3.2 | Предварительное знакомство с новыми возможностями Azure NetApp Files (ANF). | Yes |
| [privatedns](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Команды для управления Частными зонами DNS. | Yes |
| [resource-graph](https://github.com/Azure/azure-cli-extensions/tree/master/src/resource-graph) | 1.0.0 | Поддержка запросов к ресурсам Azure с помощью Resource Graph. |  |
| [sap-hana](https://github.com/Azure/azure-hanaonazure-cli-extension) | 0.5.5 | Дополнительные команды для работы с экземплярами SAP HanaOnAzure. |  |
| [storage-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/storage-preview) | 0.2.8 | Предварительная версия ожидаемых функций хранилища. | Yes |
| [subscription](https://github.com/Azure/azure-cli-extensions) | 0.1.3 | Поддержка управления подписками (предварительная версия). |  |
| [virtual-network-tap](https://github.com/Azure/azure-cli-extensions/tree/master/src/virtual-network-tap) | 0.1.0 | Управление точками доступа к виртуальным сетям (VTAP). | Yes |
| [virtual-wan](https://github.com/Azure/azure-cli-extensions/tree/master/src/virtual-wan) | 0.1.0 | Управление виртуальными глобальными сетями, концентраторами, шлюзами и сайтами VPN. | Yes |
| [vm-repair](https://github.com/Azure/azure-cli-extensions/tree/master/src/vm-repair) | 0.2.1 | Команды автоматического восстановления для исправления виртуальных машин. |  |
| [webapp](https://github.com/Azure/azure-cli-extensions/tree/master/src/webapp) | 0.2.24 | Дополнительные команды для Службы приложений Azure. | Yes |