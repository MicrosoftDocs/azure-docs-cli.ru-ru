---
title: Справочники по Azure CLI для Azure Monitor
description: Целевая страница справочника по Azure CLI для Azure Monitor
author: dbradish-microsoft
manager: barbkess
ms.devlang: azurecli
ms.topic: reference
ms.date: 06/30/2020
ms.author: dbradish
ms.service: azure-cli
ms.reviewer: robb
ms.custom: devx-track-azurecli
ms.openlocfilehash: 18b8dcb9d22cf4f0177e329f9080bf7693eade0e
ms.sourcegitcommit: 9beaf9abb794f1006a56acee4e1cfb8ea7fe2405
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2020
ms.locfileid: "96850292"
---
# <a name="azure-cli-for-azure-monitor"></a>Azure CLI для Azure Monitor

Интерфейс командной строки Azure ([Azure CLI](./what-is-azure-cli.md)) — это набор команд для создания ресурсов Azure и управления ими.  Он доступен во многих службах Azure, включая Azure Monitor.  Существует более 100 справочников для Azure Monitor, которые помогают эффективно работать со службами мониторинга из командной строки.

## <a name="references-for-azure-monitor"></a>Справочники для Azure Monitor

Интерфейс командной строки для [Azure Monitor](/azure/azure-monitor/) состоит из двух частей: Azure CLI (обычно называется **основным** CLI) и **расширение** CLI для Azure Monitor.  Перед использованием необходимо установить расширения Azure CLI из справочника. Команда [az extension add](/cli/azure/extension#az-extension-add) устанавливает ссылку на расширение по имени.

> [!IMPORTANT]
>
> Azure Monitor теперь включает Application Insights и Log Analytics. Таким образом, при работе с CLI для Azure Monitor необходимо установить расширения для каждой подобласти.

### <a name="references"></a>Ссылки

| Справочник | Установка расширения | Описание | Дополнительные сведения см. в разделе
|-|-|-|-|
| [az monitor](/cli/azure/monitor) | | Группа команд верхнего уровня для всех команд Azure CLI для Azure Monitor. | [Общие сведения о службе Azure Monitor](/azure/azure-monitor/overview)
| [az monitor action-group](/cli/azure/monitor/action-group) | | Управление группами действий, которые связаны с уведомлениями после срабатывания оповещения. | [Оповещения Azure Monitor](/azure/azure-monitor/platform/alerts-overview)
| [az monitor activity-log](/cli/azure/monitor/activity-log) | | Управление журналом действий, включая оповещения журнала действий. | [Журнал действий Azure](/azure/azure-monitor/platform/activity-log)
| [az monitor alert](/cli/azure/monitor/alert) | | НЕ ИСПОЛЬЗУЙТЕ для новых разработок.  Эта команда управляет старыми классическими правилами генерации оповещений на основе метрик, которые во всех случаях, за исключением некоторых, были перенесены в новые типы оповещений метрик. Используйте вместо этого [az monitor metrics alert](/cli/azure/monitor/metrics/alert). |
| [az monitor app-insights](/cli/azure/ext/application-insights/monitor/app-insights) | да | Управление Application Insights для мониторинга приложений. | [Что такое Azure Application Insights?](/azure/azure-monitor/app/app-insights-overview)
| [az monitor autoscale](/cli/azure/monitor/autoscale) | | Управление параметрами автомасштабирования. | [Общие сведения об автомасштабировании в Microsoft Azure](/azure/azure-monitor/platform/autoscale-overview)
| [az monitor diagnostic-settings](/cli/azure/monitor/diagnostic-settings) | | Управление параметрами диагностики службы, которые позволяют настроить сбор и маршрутизацию разных типов метрик и журналов платформы. | [Создание параметров диагностики для отправки журналов платформы и метрик в разные целевые объекты](/azure/azure-monitor/platform/diagnostic-settings)
| [az monitor log-analytics](/cli/azure/monitor/log-analytics) | | Управление кластерами журналов и рабочими пространствами. | [Проектирование развертывания журналов Azure Monitor](/azure/azure-monitor/platform/design-logs-deployment)
| [az monitor log-analytics query](/cli/azure/ext/log-analytics/monitor/log-analytics#ext-log-analytics-az-monitor-log-analytics-query) | да | Команды для запрашивания данных в рабочих областях Log Analytics.  | [Руководство. Начало работы с запросами Log Analytics](/azure/azure-monitor/log-query/get-started-portal)
| [az monitor log-profiles](/cli/azure/monitor/log-profiles) | | НЕ ИСПОЛЬЗУЙТЕ для новых разработок.  Эта команда ранее использовалась для направления журналов действий в журналы Azure Monitor и Log Analytics.  Используйте вместо этого [параметры диагностики](/azure/azure-monitor/platform/diagnostic-settings).  | [Отправка в рабочую область Log Analytics](/azure/azure-monitor/platform/activity-log#send-to-log-analytics-workspace)
| [az monitor metrics](/cli/azure/monitor/metrics) | | Управление метриками платформы и правилами генерации оповещений на основе метрик почти в реальном времени. | [Метрики в Azure Monitor](/azure/azure-monitor/platform/data-platform-metrics) и [Сведения о работе оповещений о метриках в Azure Monitor](/azure/azure-monitor/platform/alerts-metric-overview)
| [az monitor private-link-scope](/cli/azure/monitor/private-link-scope) | | Управление ресурсом области Приватного канала Azure Monitor. | [Безопасное подключение сетей к Azure Monitor с помощью Приватного канала Azure](/azure/azure-monitor/platform/private-link-security)

### <a name="installing-extension-references"></a>Установка ссылок на расширения

Перед использованием необходимо установить расширения Azure CLI из справочника.  Команда [az extension add](./azure-cli-extensions-overview.md) устанавливает ссылку на расширение по имени.

```azurecli
# install the extension for az monitor app-insights
az extension add --name application-insights

# install the extension for az monitor log-analytics
az extension add --name log-analytics
```

## <a name="popular-monitor-articles-using-the-azure-cli"></a>Популярные статьи по работе с Azure CLI для Azure Monitor

- [Примеры CLI для Azure Monitor](/azure/azure-monitor/samples/cli-samples)
- [Создание рабочей области Log Analytics с помощью Azure CLI 2.0](/azure/azure-monitor/learn/quick-create-workspace-cli)

## <a name="azure-cli-reference-examples"></a>Справочник по примерам использования Azure CLI

Примеры приведены для каждого справочника по Azure CLI. Хотя эти задачи также можно выполнить с помощью портала Azure, при использовании Azure CLI требуется одна командная строка.  Ниже представлено несколько примеров кода, которые помогут вам понять, насколько просто использовать Azure CLI.

Для работы с Azure Monitor вам потребуется группа ресурсов.  Группы ресурсов Azure можно без усилий создавать и администрировать с помощью Azure CLI.  

```azurecli
#create a resource group
az group create -location westus -name MyResourceGroup

#get a list of resource groups for a subscription
az group list --subscription MySubscription --output table
```

Создать оповещение журнала Azure Monitor очень просто.

```azurecli
#create an Azure Monitor activity log alert
az monitor activity-log alert create --name MyAlertName --resource-group MyResourceGroup
```

## <a name="see-also"></a>См. также раздел

- [Начните работу с Azure CLI](./get-started-with-azure-cli.md), чтобы узнать об установке и входе.

- Найдите дополнительные справочники по [выпущенным командам](/cli/azure/reference-index) и [командам расширения](./azure-cli-extensions-list.md) в документации по Azure CLI.

- Узнайте больше о расширениях из статьи [Использование расширений с Azure CLI](./azure-cli-extensions-overview.md).
