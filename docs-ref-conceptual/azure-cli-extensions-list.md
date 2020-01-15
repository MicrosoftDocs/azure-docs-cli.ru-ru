---
title: Доступные расширения для Azure CLI
description: Полный список официально поддерживаемых расширений для Azure CLI.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 11/26/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 60240bd73d80a2a10f82d71c36dca90a40bff83d
ms.sourcegitcommit: 18973ac471bbd12af2c8f8fa32a233b0abe5b020
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/13/2020
ms.locfileid: "75913649"
---
# <a name="available-extensions-for-the-azure-cli"></a>Доступные расширения для Azure CLI

В этой статье приведен полный список доступных расширений для Azure CLI, которые поддерживает корпорация Майкрософт.

Список расширений также доступен из CLI. Для этого выполните команду [az extension list-available](/cli/azure/extension?view=azure-cli-latest#az-extension-list-available):

```azurecli-interactive
az extension list-available --output table
```

| Имя | Версия | Сводка | Preview (Предварительный просмотр) |
|------|---------|---------|---------|
| [aem](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Управление расширениями для улучшенного мониторинга Azure для SAP. |  |
| [aks-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/aks-preview) | 0.4.23 | Предварительное знакомство с будущими возможностями AKS. | Да |
| [alias](https://github.com/Azure/azure-cli-extensions) | 0.5.2 | Поддержка псевдонимов команд. | Да |
| [appconfig](https://github.com/Azure/azure-cli-extensions) | 0.5.0 | Предварительное знакомство с новыми возможностями службы конфигурации приложений. | Да |
| [application-insights](https://github.com/Azure/azure-cli-extensions/tree/master/src/application-insights) | 0.1.1 | Поддержка компонентов управления Application Insights, а также запрашивание метрик, событий и журналов из таких компонентов. | Да |
| [azure-batch-cli-extensions](https://github.com/Azure/azure-batch-cli-extensions) | 5.0.0 | Дополнительные команды для работы с пакетной службой Azure. |  |
| [azure-cli-iot-ext](https://github.com/azure/azure-iot-cli-extension) | 0.8.6 | Предоставление уровня команд плоскости данных для Центра Интернета вещей Azure, IoT Edge и службы подготовки устройств к добавлению в Центр Интернета вещей. |  |
| [azure-cli-ml](https://docs.microsoft.com/azure/machine-learning/service/) | 1.0.76 | Командный модуль средств командной строки Azure ML в Microsoft Azure |  |
| [azure-devops](https://github.com/Microsoft/azure-devops-cli-extension) | 0.15.0 | Инструменты для управления Azure DevOps. |  |
| [azure-firewall](https://github.com/Azure/azure-cli-extensions/tree/master/src/azure-firewall) | 0.1.5 | Управление ресурсами Брандмауэра Azure. | Да |
| [connectedmachine](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Расширение Connectedmachine программ командной строки Microsoft Azure | Да |
| [db-up](https://github.com/Azure/azure-cli-extensions/tree/master/src/db-up) | 0.1.13 | Дополнительные команды для упрощения рабочих процессов Базы данных Azure. | Да |
| [dev-spaces](https://github.com/Azure/azure-cli-extensions) | 1.0.3 | Рабочие среды Azure для разработчиков предоставляют быстрый итеративный интерфейс разработки Kubernetes для команд. |  |
| [dev-spaces-preview](https://github.com/Azure/azure-cli-extensions) | 0.1.6 | Рабочие среды Azure для разработчиков предоставляют быстрый итеративный интерфейс разработки Kubernetes для команд. | Да |
| [dms-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/dms-preview) | 0.9.0 | Поддержка новых сценариев Database Migration Service. | Да |
| [dns](https://github.com/Azure/azure-cli-extensions) | 0.0.2 | Расширение Azure CLI для зон DNS. |  |
| [eventgrid](https://github.com/Azure/azure-cli-extensions) | 0.4.4 | Командный модуль средств командной строки Сетки событий в Microsoft Azure. | Да |
| [express-route](https://github.com/Azure/azure-cli-extensions/tree/master/src/express-route) | 0.1.3 | Управление ExpressRoute с помощью предварительных версий функций. | Да |
| [express-route-cross-connection](https://github.com/Azure/azure-cli-extensions/tree/master/src/express-route-cross-connection) | 0.1.1 | Управление пользовательскими каналами ExpressRoute с использованием перекрестного подключения ExpressRoute. |  |
| [find](https://github.com/Azure/azure-cli-extensions/tree/master/src/find) | 0.3.0 | Интеллектуальный запрос для получения сведений CLI. | Да |
| [front-door](https://github.com/Azure/azure-cli-extensions/tree/master/src/front-door) | 1.0.2 | Управление сетевыми службами Front Door. |  |
| [hack](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Расширение программ командной строки Microsoft Azure для взлома | Да |
| [healthcareapis](https://github.com/Azure/azure-cli-extensions) | 0.1.2 | Расширение программы командной строки Microsoft Azure HealthCareApis |  |
| [image-copy-extension](https://github.com/Azure/azure-cli-extensions) | 0.2.1 | Поддержка копирования управляемых образов виртуальных машин в другие регионы |  |
| [интерактивный](https://github.com/Azure/azure-cli) | 0.4.3 | Интерактивная оболочка командной строки Microsoft Azure | Да |
| [internet-analyzer](https://github.com/Azure/azure-cli-extensions) | 0.1.0rc4 | Расширение Internet Analyzer программ командной строки Microsoft Azure | Да |
| [ip-group](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Расширение IpGroup программ командной строки Microsoft Azure |  |
| [keyvault-preview](https://github.com/Azure/azure-keyvault-cli-extension) | 0.1.3 | Команды предварительной версии Azure Key Vault. | Да |
| [log-analytics](https://github.com/Azure/azure-cli-extensions/tree/master/src/log-analytics) | 0.1.4 | Поддержка возможностей запросов Azure Log Analytics. | Да |
| [maintenance](https://github.com/Azure/azure-cli-extensions) | 1.0.0 | Поддержка управления обслуживанием Azure (предварительная версия). | Да |
| [managementgroups](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Расширение Azure CLI для групп управления. |  |
| [managementpartner](https://github.com/Azure/azure-cli-extensions) | 0.1.2 | Поддержка партнера управления (предварительная версия). |  |
| [mesh](https://github.com/Azure/azure-cli-extensions) | 0.10.6 | Поддержка Сетки Microsoft Azure Service Fabric (общедоступная предварительная версия) | Да |
| [mixed-reality](https://github.com/Azure/azure-cli-extensions) | 0.0.1 | Расширение Azure CLI смешанной реальности. |  |
| [netappfiles-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/netappfiles-preview) | 0.3.2 | Предварительное знакомство с новыми возможностями Azure NetApp Files (ANF). | Да |
| [peering](https://github.com/Azure/azure-cli-extensions) | 0.1.0rc1 | Расширение Peering программ командной строки Microsoft Azure | Да |
| [privatedns](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Команды для управления Частными зонами DNS. | Да |
| [resource-graph](https://github.com/Azure/azure-cli-extensions/tree/master/src/resource-graph) | 1.0.0 | Поддержка запросов к ресурсам Azure с помощью Resource Graph. |  |
| [sap-hana](https://github.com/Azure/azure-hanaonazure-cli-extension) | 0.5.5 | Дополнительные команды для работы с экземплярами SAP HanaOnAzure. |  |
| [spring-cloud](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Расширение spring-cloud программ командной строки Microsoft Azure | Да |
| [storage-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/storage-preview) | 0.2.10 | Предварительная версия ожидаемых функций хранилища. | Да |
| [subscription](https://github.com/Azure/azure-cli-extensions) | 0.1.3 | Поддержка управления подписками (предварительная версия). |  |
| [virtual-network-tap](https://github.com/Azure/azure-cli-extensions/tree/master/src/virtual-network-tap) | 0.1.0 | Управление точками доступа к виртуальным сетям (VTAP). | Да |
| [virtual-wan](https://github.com/Azure/azure-cli-extensions/tree/master/src/virtual-wan) | 0.1.2 | Управление виртуальными глобальными сетями, концентраторами, шлюзами и сайтами VPN. | Да |
| [vm-repair](https://github.com/Azure/azure-cli-extensions/tree/master/src/vm-repair) | 0.2.3 | Команды автоматического восстановления для исправления виртуальных машин. |  |
| [vmware-cs](https://github.com/Azure/az-vmware-cli) | 0.2.0 | Управление решением Azure VMware. | Да |
| [webapp](https://github.com/Azure/azure-cli-extensions/tree/master/src/webapp) | 0.2.24 | Дополнительные команды для Службы приложений Azure. | Да |