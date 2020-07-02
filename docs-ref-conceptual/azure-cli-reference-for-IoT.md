---
title: Справочники по Azure CLI для Azure IoT
description: Целевая страница справочника по Azure CLI для Azure IoT
author: dbradish-microsoft
manager: barbkess
ms.devlang: azurecli
ms.topic: reference
ms.date: 06/05/2020
ms.author: dbradish
ms.service: azure-cli
ms.reviewer: paymaun.heidari
ms.openlocfilehash: e3bf40eab68f09dfb94e14e59d8a746d87bb0766
ms.sourcegitcommit: 415c6ddcce1da133d96b8c700e6aa570e4746b3f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2020
ms.locfileid: "85765095"
---
# <a name="azure-cli-for-azure-iot"></a>Azure CLI для Azure IoT

Интерфейс командной строки Azure ([Azure CLI](/cli/azure/what-is-azure-cli)) — это набор команд для создания ресурсов Azure и управления ими.  Он доступен во многих службах Azure, включая Azure IoT.  Существует более 100 справочников для Azure IoT, которые помогают эффективно работать со службами Интернета вещей из командной строки.

## <a name="references-for-iot"></a>Справочники для Интернета вещей

Интерфейс командной строки для Azure IoT состоит из двух частей: Azure CLI (обычно называется **основной** CLI) и **расширение** CLI для Azure IoT.

Возможности Интернета вещей в **основном** Azure CLI предназначены для администрирования и настройки инфраструктуры. Операции CRUD в Центре Интернета вещей или настройка маршрутов сообщений Центра Интернета вещей — типичные варианты использования основных команд.

**Расширение** Интернета вещей предоставляет широкие возможности и функции для управления данными, сущностями и объектами в самой инфраструктуре, а также для работы с ними. Например, управление парками устройств, отслеживание событий, передаваемых с устройства в облако и вызов методов облака для устройств, включены через расширение Интернета вещей. Расширение Интернета вещей Azure для Azure CLI позволяет использовать экспериментальные или предварительные технологии, обеспечивающие его универсальность в разных сценариях и вариантах использования.

### <a name="core-reference-commands"></a>Справочник по основным командам

| Справочник | Используется в расширении | Описание
|-|-|-|
| [az iot](/cli/azure/iot) | да  | Все доступные основные команды Azure CLI для Azure IoT.
| [az iot central](/cli/azure/iot/central) | да | Управление ресурсами IoT Central.
| [az iot dps](/en-us/cli/azure/iot/dps) | да | Управление службой подготовки устройств к добавлению в Центр Интернета вещей Azure.
| [az iot hub](/cli/azure/iot/hub) | да | Управление инфраструктурой Центра Интернета вещей Azure.
| [az iot pnp](/cli/azure/iot/pnp) | да | Управление репозиториями IoT Plug and Play и ключами доступа к репозиторию.

### <a name="extension-reference-commands"></a>Справочник по командам расширения

| Справочник | Используется в основной версии | Описание
|-|-|-|
| [az iot](/cli/azure/ext/azure-iot/iot) | да | Все доступные команды расширения Azure CLI для Azure IoT.
| [az iot central](/cli/azure/ext/azure-iot/iot/central) | да | Управление решениями и инфраструктурой Azure Central (IoT Central).
| [az iot device](/cli/azure/ext/azure-iot/iot/device) | | Использование возможностей двунаправленного обмена сообщениями между устройствами и облаком.
| [az dt](/cli/azure/ext/azure-iot/dt) | | Управление решениями и инфраструктурой Azure Digital Twins.
| [az iot dps](/cli/azure/ext/azure-iot/iot/dps) | да | Управление сущностями в службе подготовки устройств к добавлению в Центр Интернета вещей.
| [az iot edge](/cli/azure/ext/azure-iot/iot/edge) | | Управление решениями Интернета вещей в пограничной среде.
| [az iot hub](/cli/azure/ext/azure-iot/iot/hub) | да | Управление сущностями в Центре Интернета вещей Azure.
| [az iot pnp](/cli/azure/ext/azure-iot/iot/pnp) | да | Управление сущностями в репозитории моделей IoT Plug and Play.

### <a name="additional-cli-commands-for-azure-services-used-by-iot"></a>Дополнительные команды CLI для служб Azure, используемых в Интернете вещей

| Справочник | Тип | Описание
|-|-|-|
| [az maps](/cli/azure/maps) | core | Управление Azure Maps.
| [az timeseriesinsights](/cli/azure/ext/timeseriesinsights/timeseriesinsights) | Расширение | Управление Аналитикой временных рядов Azure.

## <a name="popular-iot-articles-using-the-azure-cli"></a>Популярные статьи, посвященные Интернету вещей, в которых описывается Azure CLI

- [Создание Центра Интернета вещей](/azure/iot-hub/iot-hub-create-using-cli)
- [Управление IoT Central](/azure/iot-central/core/howto-manage-iot-central-from-cli)
- [Руководства по устройствам, управляемым CLI с помощью ОСРВ Azure](/azure/rtos/getting-started?branch=master)
- [Использование расширения Интернета вещей для управления устройствами в Центре Интернета вещей Azure](/azure/iot-hub/iot-hub-device-management-iot-extension-azure-cli-2-0)
- [Развертывание и мониторинг модулей IoT Edge в большом масштабе с помощью расширения Azure CLI для Интернета вещей](/azure/iot-edge/how-to-deploy-cli-at-scale)
- [Отправка данных телеметрии на устройство и их отслеживание с помощью расширения Azure CLI для Интернета вещей](/azure/iot-hub/quickstart-send-telemetry-cli)
- [Маршрутизация сообщений Центра Интернета вещей с помощью Azure CLI](/azure/iot-hub/tutorial-routing-config-message-routing-cli)
- [Управление интерфейсами в репозитории моделей Plug and Play](/azure/iot-pnp/howto-install-pnp-cli#manage-interfaces-in-a-model-repository)

## <a name="azure-cli-reference-examples"></a>Справочник по примерам использования Azure CLI

Примеры приведены для каждого справочника по Azure CLI. Хотя эти задачи также можно выполнить с помощью портала Azure, при использовании Azure CLI требуется одна командная строка.  Ниже представлено несколько блоков кода, которые помогут вам понять, насколько просто использовать Azure CLI.

Для работы с Azure IoT вам потребуется группа ресурсов.  Группы ресурсов Azure можно без усилий создавать и администрировать с помощью Azure CLI.  

```azurecli
#create a resource group
az group create -location westus -name MyResourceGroup
```

```azurecli
#get a list of resource groups for a subscription
az group list --subscription MySubscription --output table
```

Вы можете без усилий создать Центр Интернета вещей Azure в регионе westus в ценовой категории "Стандартный".

```azurecli
#create an Azure IoT hub
az iot hub create --resource-group MyResourceGroup --name MyIotHub --location westus
```

## <a name="see-also"></a>См. также раздел

- [Начните работу с Azure CLI](/cli/azure/get-started-with-azure-cli), чтобы узнать об установке и входе.

- Найдите дополнительные справочники по [выпущенным командам](/cli/azure/reference-index) и [командам расширения](/cli/azure/azure-cli-extensions-list) в документации по Azure CLI.

- Узнайте больше о расширениях из статьи [Использование расширений с Azure CLI](/cli/azure/azure-cli-extensions-overview).
