---
title: Доступные расширения для Azure CLI 2.0
description: Полный список официально поддерживаемых расширений для Azure CLI 2.0.
author: derekbekoe
ms.author: debekoe
manager: routlaw
ms.date: 07/30/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 92d2ac36d0176469f8f5a77e7a27d0b11ab6d947
ms.sourcegitcommit: 70bb8b115f7b9079ca1fdb65c7f5582b060a466f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2018
ms.locfileid: "39356613"
---
# <a name="available-extensions-for-the-azure-cli-20"></a>Доступные расширения для Azure CLI 2.0

В этой статье приведен полный список доступных расширений для Azure 2.0 CLI, которые предлагаются и поддерживаются корпорацией Майкрософт.

Список расширений также можно получить непосредственно из CLI. Для этого выполните команду [az extension list-available](/cli/azure/extension?view=azure-cli-latest#az-extension-list-available):

```azurecli
az extension list-available --output table
```

| ИМЯ | Version (версия) | Сводка | Предварительный просмотр |
|------|---------|---------|---------|
| [aem](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Управление расширениями для улучшенного мониторинга Azure для SAP. |  |
| [alias](https://github.com/Azure/azure-cli-extensions) | 0.5.1 | Поддержка псевдонимов команд. | Yes |
| [azure-batch-cli-extensions](https://github.com/Azure/azure-batch-cli-extensions) | 2.4.1 | Дополнительные команды для работы с пакетной службой Azure. |  |
| [azure-cli-iot-ext](https://github.com/azure/azure-iot-cli-extension) | 0.5.1 | Предоставление уровня команд плоскости данных для Центра Интернета вещей Azure, IoT Edge и службы подготовки устройств к добавлению в Центр Интернета вещей. |  |
| [botservice](https://github.com/Azure/azure-cli-extensions) | 0.0.3 | Поддержка функций предварительной версии 2017-12-01 службы Azure Bot | Yes |
| [dev-spaces-preview](https://github.com/Azure/azure-cli-extensions) | 0.1.6 | Рабочие среды Azure для разработчиков предоставляют быстрый итеративный интерфейс разработки Kubernetes для команд. | Yes |
| [dns](https://github.com/Azure/azure-cli-extensions) | 0.0.2 | Расширение Azure CLI для зон DNS. |  |
| [eventgrid](https://github.com/Azure/azure-cli-extensions) | 0.2.1 | Поддержка функций службы 	"Сетка событий Azure" версии 2018-05-01-preview | Yes |
| [image-copy-extension](https://github.com/Azure/azure-cli-extensions) | 0.0.7 | Поддержка копирования управляемых образов виртуальных машин в другие регионы |  |
| [keyvault-preview](https://github.com/Azure/azure-keyvault-cli-extension) | 0.1.3 | Команды предварительной версии Azure Key Vault. | Yes |
| [log-analytics](https://github.com/Azure/azure-cli-extensions/tree/master/src/log-analytics) | 0.1.2 | Поддержка возможностей запросов Azure Log Analytics. | Yes |
| [managementgroups](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Расширение Azure CLI для групп управления. |  |
| [managementpartner](https://github.com/Azure/azure-cli-extensions) | 0.1.2 | Поддержка партнера управления (предварительная версия). |  |
| [mesh](https://github.com/Azure/azure-cli-extensions) | 0.9.1 | Поддержка Сетки Microsoft Azure Service Fabric (общедоступная предварительная версия) | Yes |
| [rdbms-vnet](https://github.com/Azure/azure-cli-extensions) | 10.0.0 | Поддержка правил виртуальной сети в ресурсах Azure MySQL и Azure PostgreSQL. |  |
| [signalr](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Поддержка управления с помощью SignalR (предварительная версия). | Yes |
| [storage-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/storage-preview) | 0.1.3 | Предварительная версия ожидаемых функций хранилища. | Yes |
| [subscription](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Поддержка управления подписками (предварительная версия). |  |
| [webapp](https://github.com/Azure/azure-cli-extensions) | 0.2.6 | Расширение Azure CLI для управления ресурсами службы приложений. | Yes |
