---
title: Доступные расширения для Azure CLI
description: Полный список официально поддерживаемых расширений для Azure CLI.
author: haroldrandom
ms.author: jianzen
manager: yonzhan,yungezz
ms.date: 08/28/2020
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 1c12add4370df3cdf9450164d4b4061863a0046f
ms.sourcegitcommit: 28e3282487dab68f9a4635f8bec161fbc412c3b9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/28/2020
ms.locfileid: "89054586"
---
# <a name="available-extensions-for-the-azure-cli"></a>Доступные расширения для Azure CLI

В этой статье приведен полный список доступных расширений для Azure CLI, которые поддерживает корпорация Майкрософт.

Список расширений также доступен из CLI. Для этого выполните команду [az extension list-available](/cli/azure/extension?view=azure-cli-latest#az-extension-list-available):

```azurecli-interactive
az extension list-available --output table
```

| Имя | Версия | Сводка | Preview (Предварительный просмотр) |
|------|---------|---------|---------|
| [учетная запись](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Расширение SubscriptionClient для программ командной строки Microsoft Azure |  |
| [aem](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Управление расширениями для улучшенного мониторинга Azure для SAP. |  |
| [ai-did-you-mean-this](https://github.com/Azure/azure-cli-extensions/tree/master/src/ai-did-you-mean-this) | 0.2.1 | Рекомендуемые параметры восстановления при сбое. |  |
| [ai-examples](https://github.com/Azure/azure-cli-extensions/tree/master/src/ai-examples) | 0.2.3 | Добавление примеров на основе искусственного интеллекта в содержимое справки. | Да |
| [aks-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/aks-preview) | 0.4.61 | Предварительное знакомство с будущими возможностями AKS. | Да |
| [alertsmanagement](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Расширение оповещений для программ командной строки Microsoft Azure |  |
| [alias](https://github.com/Azure/azure-cli-extensions) | 0.5.2 | Поддержка псевдонимов команд. | Да |
| [application-insights](https://github.com/Azure/azure-cli-extensions/tree/master/src/application-insights) | 0.1.9 | Поддержка компонентов управления Application Insights, а также запрашивание метрик, событий и журналов из таких компонентов. | Да |
| [attestation](https://github.com/Azure/azure-cli-extensions/tree/master/src/attestation) | 0.1.0 | Расширение AttestationManagementClient для средств командной строки Microsoft Azure |  |
| [azure-batch-cli-extensions](https://github.com/Azure/azure-batch-cli-extensions) | 6.0.0 | Дополнительные команды для работы с пакетной службой Azure. |  |
| [azure-cli-iot-ext](https://github.com/azure/azure-iot-cli-extension) | 0.8.10 | Не рекомендуется: удалите azure-cli-iot-ext и установите расширение azure-iot. Удаление устаревшего расширения azure-cli-iot-ext планируется после 15.09.2020. |  |
| [azure-cli-ml](https://docs.microsoft.com/python/api/overview/azure/ml/?view=azure-ml-py) | 1.12.0 | Командный модуль средств командной строки Azure ML в Microsoft Azure |  |
| [azure-devops](https://github.com/Microsoft/azure-devops-cli-extension) | 0.18.0 | Инструменты для управления Azure DevOps. |  |
| [azure-firewall](https://github.com/Azure/azure-cli-extensions/tree/master/src/azure-firewall) | 0.5.1 | Управление ресурсами Брандмауэра Azure. | Да |
| [azure-iot](https://github.com/azure/azure-iot-cli-extension) | 0.9.8 | Расширение Azure IoT для Azure CLI. |  |
| [blockchain](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Расширение BlockchainManagementClient для средств командной строки Microsoft Azure |  |
| [blueprint](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Расширение Blueprint для программ командной строки Microsoft Azure |  |
| [codespaces](https://github.com/Azure/azure-cli-extensions) | 0.3.0 | Расширение Codespaces для Azure CLI | Да |
| [connectedk8s](https://github.com/Azure/azure-cli-extensions) | 0.2.4 | Расширение Connectedk8s для программ командной строки Microsoft Azure | Да |
| [connectedmachine](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Расширение Connectedmachine программ командной строки Microsoft Azure | Да |
| [connection-monitor-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/connection-monitor-preview) | 0.1.0 | Расширение Connection Monitor для командной строки Microsoft Azure (версия 2) | Да |
| [costmanagement](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Расширение CostManagementClient для средств командной строки Microsoft Azure |  |
| [csvmware](https://github.com/Azure/az-vmware-cli) | 0.3.0 | Управление решением VMware в Azure от CloudSimple. | Да |
| [custom-providers](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Расширение Custom Providers для программ командной строки Microsoft Azure |  |
| [databox](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Расширение Data Box для программ командной строки Microsoft Azure |  |
| [databricks](https://github.com/Azure/azure-cli-extensions) | 0.5.0 | Расширение DatabricksClient для программ командной строки Microsoft Azure | Да |
| [datafactory](https://github.com/Azure/azure-cli-extensions/tree/master/src/datafactory) | 0.1.0 | Расширение DataFactoryManagementClient для программ командной строки Microsoft Azure |  |
| [datashare](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Расширение DataShareManagementClient для программ командной строки Microsoft Azure |  |
| [db-up](https://github.com/Azure/azure-cli-extensions/tree/master/src/db-up) | 0.1.15 | Дополнительные команды для упрощения рабочих процессов Базы данных Azure. | Да |
| [deploy-to-azure](https://github.com/Azure/deploy-to-azure-cli-extension) | 0.2.0 | Развертывание в Azure с помощью действий GitHub. | Да |
| [desktopvirtualization](https://github.com/Azure/azure-cli-extensions/tree/master/src/desktopvirtualization) | 0.1.0 | Расширение DesktopVirtualizationAPIClient для программ командной строки Microsoft Azure |  |
| [dev-spaces](https://github.com/Azure/azure-cli-extensions) | 1.0.5 | Рабочие среды Azure для разработчиков предоставляют быстрый итеративный интерфейс разработки Kubernetes для команд. |  |
| [dev-spaces-preview](https://github.com/Azure/azure-cli-extensions) | 0.1.6 | Рабочие среды Azure для разработчиков предоставляют быстрый итеративный интерфейс разработки Kubernetes для команд. | Да |
| [dms-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/dms-preview) | 0.11.0 | Поддержка новых сценариев Database Migration Service. | Да |
| [eventgrid](https://github.com/Azure/azure-cli-extensions) | 0.4.9 | Командный модуль средств командной строки Сетки событий в Microsoft Azure. | Да |
| [express-route](https://github.com/Azure/azure-cli-extensions/tree/master/src/express-route) | 0.1.3 | Управление ExpressRoute с помощью предварительных версий функций. | Да |
| [express-route-cross-connection](https://github.com/Azure/azure-cli-extensions/tree/master/src/express-route-cross-connection) | 0.1.1 | Управление пользовательскими каналами ExpressRoute с использованием перекрестного подключения ExpressRoute. |  |
| [footprint](https://github.com/Azure/azure-cli-extensions/tree/master/src/footprint) | 1.0.0 | Расширение FootprintMonitoringManagementClient для средств командной строки Microsoft Azure |  |
| [front-door](https://github.com/Azure/azure-cli-extensions/tree/master/src/front-door) | 1.0.9 | Управление сетевыми службами Front Door. |  |
| [guestconfig](https://github.com/Azure/azure-cli-extensions/tree/master/src/guestconfig) | 0.1.0 | Расширение GuestConfigurationClient для программ командной строки Microsoft Azure |  |
| [hack](https://github.com/Azure/azure-cli-extensions) | 0.4.2 | Расширение программ командной строки Microsoft Azure для взлома | Да |
| [hardware-security-modules](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Расширение AzureDedicatedHSMResourceProvider для средств командной строки Microsoft Azure |  |
| [healthcareapis](https://github.com/Azure/azure-cli-extensions) | 0.2.0 | Расширение HealthcareApisManagementClient для программ командной строки Microsoft Azure |  |
| [hpc-cache](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Расширение кэша хранилища для программ командной строки Microsoft Azure | Да |
| [image-copy-extension](https://github.com/Azure/azure-cli-extensions) | 0.2.6 | Поддержка копирования управляемых образов виртуальных машин в другие регионы |  |
| [import-export](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Расширение StorageImportExport для программ командной строки Microsoft Azure |  |
| [интерактивный](https://github.com/Azure/azure-cli) | 0.4.4 | Интерактивная оболочка командной строки Microsoft Azure | Да |
| [internet-analyzer](https://github.com/Azure/azure-cli-extensions) | 0.1.0rc5 | Расширение Internet Analyzer программ командной строки Microsoft Azure | Да |
| [ip-group](https://github.com/Azure/azure-cli-extensions) | 0.1.2 | Расширение IpGroup программ командной строки Microsoft Azure | Да |
| [k8sconfiguration](https://github.com/Azure/azure-cli-extensions) | 0.1.8 | Расширение K8sconfiguration для программ командной строки Microsoft Azure | Да |
| [keyvault-preview](https://github.com/Azure/azure-keyvault-cli-extension) | 0.1.3 | Команды предварительной версии Azure Key Vault. | Да |
| [kusto](https://github.com/Azure/azure-cli-extensions/tree/master/src/kusto) | 0.1.1 | Расширение KustoManagementClient для программ командной строки Microsoft Azure |  |
| [log-analytics](https://github.com/Azure/azure-cli-extensions/tree/master/src/log-analytics) | 0.2.1 | Поддержка возможностей запросов Azure Log Analytics. | Да |
| [log-analytics-solution](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Поддержка решения Azure Log Analytics |  |
| [logic](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Расширение LogicManagementClient для программ командной строки Microsoft Azure |  |
| [maintenance](https://github.com/Azure/azure-cli-extensions) | 1.0.1 | Поддержка управления обслуживанием Azure. |  |
| [managementpartner](https://github.com/Azure/azure-cli-extensions) | 0.1.3 | Поддержка партнера управления (предварительная версия). |  |
| [mesh](https://github.com/Azure/azure-cli-extensions) | 0.10.6 | Поддержка Сетки Microsoft Azure Service Fabric (общедоступная предварительная версия) | Да |
| [mixed-reality](https://github.com/Azure/azure-cli-extensions) | 0.0.2 | Расширение Azure CLI смешанной реальности. | Да |
| [netappfiles-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/netappfiles-preview) | 0.3.2 | Предварительное знакомство с новыми возможностями Azure NetApp Files (ANF). | Да |
| [notification-hub](https://github.com/Azure/azure-cli-extensions) | 0.2.0 | Расширение Notification Hub для программ командной строки Microsoft Azure |  |
| [peering](https://github.com/Azure/azure-cli-extensions) | 0.2.0 | Расширение PeeringManagementClient для программ командной строки Microsoft Azure |  |
| [portal](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Расширение Portal программ командной строки Microsoft Azure |  |
| [powerbidedicated](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Расширение PowerBIDedicated для программ командной строки Microsoft Azure | Да |
| [privatedns](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Команды для управления Частными зонами DNS. | Да |
| [resource-graph](https://github.com/Azure/azure-cli-extensions/tree/master/src/resource-graph) | 1.1.0 | Поддержка запросов к ресурсам Azure с помощью Resource Graph. | Да |
| [sap-hana](https://github.com/Azure/azure-hanaonazure-cli-extension) | 0.6.4 | Дополнительные команды для работы с экземплярами SAP HanaOnAzure. |  |
| [spring-cloud](https://github.com/Azure/azure-cli-extensions) | 1.0.0 | Расширение spring-cloud программ командной строки Microsoft Azure |  |
| [storage-or-preview](https://github.com/Azure/azure-cli-extensions) | 0.4.0 | Расширение Storage-or-preview для программ командной строки Microsoft Azure | Да |
| [storage-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/storage-preview) | 0.2.12 | Предварительная версия ожидаемых функций хранилища. | Да |
| [storagesync](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Расширение синхронизации службы хранилища Майкрософт для программ командной строки Microsoft Azure |  |
| [stream-analytics](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Расширение Stream Analytics для программ командной строки Microsoft Azure |  |
| [subscription](https://github.com/Azure/azure-cli-extensions) | 0.1.4 | Поддержка управления подписками (предварительная версия). | Да |
| [support](https://github.com/azure/azure-cli-extensions/tree/master/src/support) | 1.0.2 | Расширение Support для программ командной строки Microsoft Azure |  |
| [synapse](https://github.com/Azure/azure-cli-extensions) | 0.3.0 | Расширение Synapse для программ командной строки Microsoft Azure | Да |
| [timeseriesinsights](https://github.com/Azure/azure-cli-extensions/src/timeseriesinsights) | 0.1.2 | Расширение TimeSeriesInsightsClient для программ командной строки Microsoft Azure |  |
| [virtual-network-tap](https://github.com/Azure/azure-cli-extensions/tree/master/src/virtual-network-tap) | 0.1.0 | Управление точками доступа к виртуальным сетям (VTAP). | Да |
| [virtual-wan](https://github.com/Azure/azure-cli-extensions/tree/master/src/virtual-wan) | 0.2.0 | Управление виртуальными глобальными сетями, концентраторами, шлюзами и сайтами VPN. | Да |
| [vm-repair](https://github.com/Azure/azure-cli-extensions/tree/master/src/vm-repair) | 0.3.2 | Команды автоматического восстановления для исправления виртуальных машин. |  |
| [vmware](https://github.com/virtustream/azure-vmware-virtustream-cli-extension) | 0.6.0 | Команды предварительной версии решения Azure VMware. | Да |
| [webapp](https://github.com/Azure/azure-cli-extensions/tree/master/src/webapp) | 0.2.24 | Дополнительные команды для Службы приложений Azure. | Да |