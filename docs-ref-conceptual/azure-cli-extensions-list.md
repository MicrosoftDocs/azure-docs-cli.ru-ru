---
title: Доступные расширения для Azure CLI 2.0
description: Полный список официально поддерживаемых расширений для Azure CLI 2.0.
author: derekbekoe
ms.author: debekoe
manager: routlaw
ms.date: 03/15/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: ceca7ed92435ab03b196e60dee37195330f6f3c7
ms.sourcegitcommit: b5a6296c006e3a44f66892729e47d7a967267d3e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/28/2018
---
# <a name="available-extensions-for-the-azure-cli-20"></a>Доступные расширения для Azure CLI 2.0

В этой статье приведен полный список доступных расширений для Azure 2.0 CLI, которые предлагаются и поддерживаются корпорацией Майкрософт.

Список расширений также можно получить непосредственно из CLI. Для этого выполните команду [az extension list-available](/cli/azure/extension?view=azure-cli-latest#az-extension-list-available):

```azurecli
az extension list-available --output table
```

| ИМЯ | Version (версия) | Сводка | Предварительный просмотр |
|------|---------|---------|---------|
| [aem](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Управление расширенным мониторингом Azure для SAP. |  |
| [alias](https://github.com/Azure/azure-cli-extensions) | 0.2.0 | Поддержка псевдонимов команд. |  |
| [azure-batch-cli-extensions](https://github.com/Azure/azure-batch-cli-extensions) | 2.1.0 | Дополнительные команды пакетной службы Azure (предварительная версия). |  |
| [azure-cli-iot-ext](https://github.com/azure/azure-iot-cli-extension) | 0.4.1 | Предоставление уровня команд плоскости данных для Центра Интернета вещей, Azure IoT Edge и службы подготовки устройств IoT. |  |
| [dns](https://github.com/Azure/azure-cli-extensions) | 0.0.1 | Поддержка Частной зоны DNS (общедоступная предварительная версия). |  |
| [image-copy-extension](https://github.com/Azure/azure-cli-extensions) | 0.0.5 | Копирование изображений между регионами. |  |
| [managementgroups](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Поддержка групп управления (предварительная версия). | Yes |
| [managementpartner](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Поддержка партнера управления (предварительная версия). | Yes |
| [rdbms](https://github.com/Azure/azure-cli-extensions) | 0.0.4 | Поддержка Azure MySQL и Azure PostgreSQL. |  |
| [subscription](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Поддержка определений подписки (предварительная версия). | Yes |
| [webapp](https://github.com/Azure/azure-cli-extensions) | 0.2.0 | Создание и развертывание ресурсов служб приложений. | Yes |
