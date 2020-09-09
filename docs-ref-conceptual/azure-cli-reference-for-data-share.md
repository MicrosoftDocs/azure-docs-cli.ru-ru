---
title: Справочники по Azure CLI для Azure Data Share
description: Целевая страница справочников по Azure CLI для Azure Data Share
services: data-share
author: dbradish-microsoft
manager: barbkess
ms.service: data-share
ms.devlang: azurecli
ms.topic: reference
ms.date: 05/27/2020
ms.author: dbradish
ms.custom: devx-track-azurecli
ms.openlocfilehash: e8d834864b2d967beb18e9cd304b922db859ef09
ms.sourcegitcommit: 2da241715d25407ed22c1065c0c793acfd865996
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/09/2020
ms.locfileid: "89562776"
---
# <a name="azure-cli-for-azure-data-share"></a>Azure CLI для Azure Data Share

Интерфейс командной строки Azure ([Azure CLI](/cli/azure/what-is-azure-cli)) — это набор команд для создания ресурсов Azure и управления ими.  Он доступен во многих службах Azure, включая Azure Data Share.  Для Data Share существует более 65 разных команд.  Эти команды дают возможность эффективно работать со службой с помощью командной строки.

## <a name="references-for-data-share"></a>Справочники для Data Share

Все команды Azure CLI для Azure Data Share сейчас являются расширениями Azure CLI.  Расширение предоставляет доступ к экспериментальным и предварительным версиям командам.  Узнайте больше о расширениях из статьи [Использование расширений с Azure CLI](/cli/azure/azure-cli-extensions-overview).

|Справочник по Azure CLI |Описание
|-|-|-|
| [az datashare](/cli/azure/ext/datashare/datashare) | Все команды для управления Azure Data Share.
| [az datashare account](/cli/azure/ext/datashare/datashare/account) | Команды для управления учетными записями Azure Data Share.
| [az datashare consumer](/cli/azure/ext/datashare/datashare/consumer) | Команды для потребителей для управления Azure Data Share.
| [az datashare dataset](/cli/azure/ext/datashare/datashare/dataset) | Команды для поставщиков для управления наборами данных Azure Data Share.
| [az datashare invitation](/cli/azure/ext/datashare/datashare/invitation) | Команды для потребителей для управления приглашениями Azure Data Share.
| [az datashare provider-share-subscription](/cli/azure/ext/datashare/datashare/provider-share-subscription) | Команды для поставщиков для управления подписками Azure Data Share.
| [az datashare synchronization](/cli/azure/ext/datashare/datashare/synchronization)  | Команды для управления синхронизацией Azure Data Share.
| [az datashare synchronization-setting](/cli/azure/ext/datashare/datashare/synchronization-setting)  | Команды для поставщиков для управления параметрами синхронизации Azure Data Share.

## <a name="reference-examples"></a>Примеры справочников

Примеры приведены для каждого справочника по Azure CLI. Хотя эти задачи также можно выполнить с помощью портала Azure, при использовании Azure CLI требуется одна командная строка.  Ниже представлено несколько блоков кода, которые помогут вам понять, насколько просто использовать Azure CLI.

Для работы с Azure Data Share вам потребуется группа ресурсов.  Группы ресурсов Azure можно без усилий создавать и администрировать с помощью Azure CLI.  

```azurecli
#create a resource group
az group create -location westus -name MyResourceGroup
```

```azurecli
#get a list of resource groups for a subscription
az group list --subscription MySubscription --output table
```

Создать учетную запись Data Share очень просто.

```azurecli
#create a data share account
az datashare account create --location "West US 2" --tags tag1=Red tag2=White --name MyAccount --resource-group MyResourceGroup
```

## <a name="see-also"></a>См. также раздел

* [Начните работу с Azure CLI](/cli/azure/get-started-with-azure-cli), чтобы узнать об установке и входе.

* Найдите дополнительные справочники по [основным командам](/cli/azure/reference-index) и [командам расширения](/cli/azure/azure-cli-extensions-list) в документации по Azure CLI.
