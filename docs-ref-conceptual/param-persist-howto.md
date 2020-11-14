---
title: Опции хранимых параметров Azure CLI
description: Использование хранимых параметров Azure CLI для сохранения значений многократно используемых параметров
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.prod: azure
ms.date: 10/30/2020
ms.topic: conceptual
ms.devlang: azurecli
ms.technology: azure-cli
ms.custom: devex-track-azurecli
ms.openlocfilehash: 47fb93c7f78af94c58d509a969bab70b814e6128
ms.sourcegitcommit: 8d514f4147d6edfc02d8d95d5a4243d100a7fcc9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2020
ms.locfileid: "93423225"
---
# <a name="azure-cli-persisted-parameter"></a>Хранимые параметры Azure CLI

Ссылочная команда Azure CLI [az config param-persist](/cli/azure/param-persist) предоставляет возможность сохранять локальные значения хранимых параметров для команд Azure CLI.  Таким образом устраняется необходимость в постоянном повторном вводе общих параметров. Например, location и resource-group являются обязательными параметрами во многих командах CLI, но они не влияют на _намерение_ команды.  При сохранении значения параметров с помощью функции хранимых параметров, вы уменьшаете избыточность и можете значительно сократить синтаксис команд CLI.

Значения конфигурации, используемые CLI, вычисляются в указанном ниже порядке. Элементы, расположенные выше в списке, имеют больший приоритет.

1. Параметры командной строки
1. Значения в локальной рабочей папке, заданные с помощью команды **az config param-persist**
1. Переменные среды
1. Значения в файле конфигурации или заданные с помощью команды **az config**

[Установите Azure CLI](install-azure-cli.md) или откройте [Azure Cloud Shell](https://shell.azure.com), чтобы запустить скрипты, указанные в этой статье.  При использовании локальной установки Azure CLI для выполнения команд **az config param-persist** требуется версия 2.12.0 или более поздняя.  Выполните команду [az version](/cli/azure/reference-index?#az_version), чтобы узнать установленную версию и зависимые библиотеки. Чтобы обновиться до последней версии, выполните команду [az upgrade](/cli/azure/reference-index?#az_upgrade).  В Azure Cloud Shell всегда установлена последняя версия Azure CLI.

## <a name="persisted-parameter-data-file"></a>Файл данных хранимого параметра

Значения хранимых параметров хранятся в файле с именем **.param_persist** , который находится в вашей рабочей папке.  При использовании [Azure Cloud Shell](https://shell.azure.com) для выполнения команд Azure CLI рабочая папка будет находиться в учетной записи хранения, используемой Azure CLI.  При использовании [локальной установки](/install-azure-cli) Azure CLI рабочая папка будет находиться на локальном компьютере.  В любом из этих расположений файл **.param_persist** будет скрыт. Его не нужно обновлять вручную.

## <a name="persisted-parameter-storage-and-support"></a>Сохранение и поддержка хранимых параметров

Функция хранимых параметров поддерживается для указанных ниже параметров Azure CLI.  Параметры **resource_group_name** и **location** сохраняются иначе. Вы можете добавить их в хранимый параметр _без_ выполнения команды создания.

| Хранимый параметр | Действие сохранения | Поддерживаются
|-|-|-|
| location | Выполнение любой команды | Все справочники по Azure CLI
| resource_group_name | Выполнение любой команды | Все справочники по Azure CLI
| vnet_name | Выполнение команды создания | Только веб-приложения Azure
| storage_account_name | Выполнение команды создания |  Только веб-приложения Azure
| webapp_name | Выполнение команды создания | Только веб-приложения Azure
| function_app_name | Выполнение команды создания | Только Функции Azure

## <a name="sample-script-using-persisted-parameters"></a>Пример скрипта с использованием хранимых параметров

Без хранимых параметров для последовательного выполнения команд CLI необходимо указывать одни и те же значения параметров.  Если хранимые параметры включены, сохраненные значения параметров можно опустить в последовательном выполнении команд.  В этом примере значения параметров **location** , **resource group name** или **storage account name** повторяются в последующих командах.

```azurecli
# Reminder: function app and storage account names must be unique.

# turn persisted parameters on
az config param-persist on

# Create a resource group which will store "resource group" and "location" in persisted parameter.
az group create --name RGlocalContext --location westeurope

# Create an Azure storage account omitting location and resource group.
az storage account create \
  --name sa1localcontext \
  --sku Standard_LRS

# Create a serverless function app in the resource group omitting storage account and resource group.
az functionapp create \
  --name FAlocalContext \
  --consumption-plan-location westeurope \
  --functions-version 2

# See the stored parameter values
az config param-persist show
```

## <a name="persisted-parameter-and-global-variable-comparison"></a>Сравнение хранимых параметров и глобальных переменных

Для значений параметров по умолчанию можно использовать две команды Azure CLI: **az configure** и **az config param-persist**.  С помощью команды **az configure** можно указать _глобальные переменные_ , например group, location или web.  С помощью команды **az param-persist** можно указать _локальные значения по умолчанию_ , уникальные для вашей рабочей нагрузки.  Сохраненные значения используются CLI вместо обязательных аргументов.

> [!Important]
> Хранимые параметры переопределяют глобальные значения контекста.
>

| Справочные сведения | Область | Присвойте параметру | Использовать
|-|-|-|-|
[az configure](/cli/azure/reference-index#az_configure) | Глобальный охват через CLI | Устанавливается явным образом с помощью команды **az configure --defaults** | Используется для таких параметров, как ведение журнала, сбор данных и значения аргументов по умолчанию
[az config param-persist](/cli/azure/config/param-persist) | Локальный охват в конкретной рабочей папке | Устанавливается автоматически после включения хранимых параметров | Используется для последовательного выполнения команд отдельных рабочих нагрузок.

### <a name="command-examples"></a>Примеры команд

С помощью **az config param-persist** можно задать глобальную переменную, используемую при создании учетной записи хранения Azure.

```azurecli
# set the global variable for resource group
az configure --defaults group=myGlobalVariableRG

# Create an Azure storage account omitting the resource group relying on the global variable value
# Substitute the storage account name parameter with a unique value
az storage account create \
  --name mystorageaccount1 \
  --location westeurope \
  --sku Standard_LRS
```

В выходных данных команды CLI указано, что новая учетная запись хранения была создана в группе ресурсов, обнаруженной в глобальной переменной myGlobalVariableRG.

```output
...
},
  "primaryLocation": "westeurope",
  "privateEndpointConnections": [],
  "provisioningState": "Succeeded",
  "resourceGroup": "myGlobalVariableRG",
  "routingPreference": null,
  "secondaryEndpoints": null,
  "secondaryLocation": null,
  "sku": {
    "name": "Standard_LRS",
    "tier": "Standard"
},
...
```

С помощью команды **az config param-persist** можно задать хранимые параметры, используемые при создании учетной записи хранения Azure.  Если для того же объекта задана глобальная переменная, хранимый параметр переопределит ее.

```azurecli
# turn persisted parameter on
az config param-persist on

# Create a resource group in order to write to persisted parameter
az group create --name myParamPersistRG --location westeurope

# Create an Azure storage account omitting the resource group relying on the persisted parameter value
# Substitute the storage account name parameter with a unique value
az storage account create \
  --name mystorageaccount2 \
  --location westeurope \
  --sku Standard_LRS
```

Даже с глобальной переменной, заданной для группы ресурсов со значением `myGlobalVariableRG`, и с включенными хранимыми параметрами новая учетная запись хранения была создана с помощью `myParamPersistRG`.

```output
...
},
  "primaryLocation": "westeurope",
  "privateEndpointConnections": [],
  "provisioningState": "Succeeded",
  "resourceGroup": "myParamPersistRG",
  "routingPreference": null,
  "secondaryEndpoints": null,
  "secondaryLocation": null,
  "sku": {
    "name": "Standard_LRS",
    "tier": "Standard"
},
...
```

## <a name="see-also"></a>См. также раздел

* [Учебник. Использование хранимых параметров для последовательного выполнения команд Azure CLI](param-persist-tutorial.md)
* [Настройка Azure CLI с помощью команды az configure](azure-cli-configuration.md)

