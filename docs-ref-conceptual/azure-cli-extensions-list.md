---
title: Доступные расширения для Azure CLI 2.0
description: Полный список официально поддерживаемых расширений для Azure CLI 2.0.
author: derekbekoe
ms.author: debekoe
manager: routlaw
ms.date: 05/16/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 82f2aec902ff7a9061f056139551990334ff6fb9
ms.sourcegitcommit: 42f1ba77b2f562d89dadd302655d1f02ee4b6130
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/17/2018
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
| [azure-batch-cli-extensions](https://github.com/Azure/azure-batch-cli-extensions) | 2.2.2 | Дополнительные команды для работы с пакетной службой Azure. |  |
| [azure-cli-iot-ext](https://github.com/azure/azure-iot-cli-extension) | 0.4.4 | Предоставление уровня команд плоскости данных для Центра Интернета вещей Azure, IoT Edge и службы подготовки устройств к добавлению в Центр Интернета вещей. |  |
| [botservice](https://github.com/Azure/azure-cli-extensions) | 0.0.1 | Поддержка функций предварительной версии 2017-12-01 службы Azure Bot | Yes |
| [dev-spaces-preview](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Рабочие среды Azure для разработчиков предоставляют быстрый итеративный интерфейс разработки Kubernetes для команд. | Yes |
| [dns](https://github.com/Azure/azure-cli-extensions) | 0.0.2 | Расширение Azure CLI для зон DNS. |  |
| [eventgrid](https://github.com/Azure/azure-cli-extensions) | 0.2.0 | Поддержка функций службы 	"Сетка событий Azure" версии 2018-05-01-preview | Yes |
| [image-copy-extension](https://github.com/Azure/azure-cli-extensions) | 0.0.6 | Поддержка копирования управляемых образов виртуальных машин в другие регионы |  |
| [keyvault-preview](https://github.com/Azure/azure-keyvault-cli-extension) | 0.1.3 | Команды предварительной версии Azure Key Vault. | Yes |
| [managementgroups](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Расширение Azure CLI для групп управления. |  |
| [managementpartner](https://github.com/Azure/azure-cli-extensions) | 0.1.2 | Поддержка партнера управления (предварительная версия). |  |
| [signalr](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Поддержка управления с помощью SignalR (предварительная версия). | Yes |
| [storage-preview](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Предварительная версия ожидаемых функций хранилища. | Yes |
| [subscription](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Поддержка управления подписками (предварительная версия). |  |
| [webapp](https://github.com/Azure/azure-cli-extensions) | 0.2.6 | Расширение Azure CLI для управления ресурсами службы приложений. | Yes |
