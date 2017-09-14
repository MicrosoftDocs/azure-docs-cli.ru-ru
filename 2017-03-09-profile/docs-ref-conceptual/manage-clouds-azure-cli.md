---
title: "Управление несколькими облаками с помощью Azure CLI 2.0"
description: "Создавайте, администрируйте и входите в разные облака с помощью Azure CLI 2.0."
keywords: Azure CLI 2.0, Azure, clouds, datacenters, government, region, china, germany
author: sptramer
manager: douge
ms.author: sttramer
ms.date: 06/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.openlocfilehash: 0222b7339e46346ef6c7e9ad98616d9b71129942
ms.sourcegitcommit: f107cf927ea1ef51de181d87fc4bc078e9288e47
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2017
---
# <a name="managing-multiple-clouds-with-azure-cli-20"></a>Управление несколькими облаками с помощью Azure CLI 2.0

При наличии нескольких подписок, связанных с Azure, у вас может быть несколько доступных облаков. У каждого облака свои связанные конечные точки и возможности. Также облака часто привязаны к определенному региону, в котором приняты свои стандарты и требования к защите данных.

Чтобы эффективно работать с несколькими облаками, требуется возможность переключаться между активными облаками и, возможно, создавать новые.

## <a name="listing-clouds"></a>Вывод списка облаков

Вы можете отобразить список доступных облаков с помощью команды [cloud list](/cli/azure/cloud#list). Так вы узнаете, какое облако активно и какой у него текущий профиль, а также получите сведения о суффиксах регионов и именах узлов.

Вот как получить список доступных облаков и узнать, какое облако сейчас активно:

```azurecli
az cloud list --output table
```

```output
IsActive    Name               Profile
----------  -----------------  ---------
True        AzureCloud         latest
            AzureChinaCloud    latest
            AzureUSGovernment  latest
            AzureGermanCloud   latest
```

## <a name="switching-the-active-cloud"></a>Переключение активного облака

Чтобы переключиться с текущего активного облака, выполните команду [cloud set](/cli/azure/cloud#set). Эта команда принимает один обязательный аргумент — имя облака.

```azurecli
az cloud set --name AzureChinaCloud
```

> [!IMPORTANT]
> Если вы никогда не выполняли аутентификацию для активного облака, вам потребуется выполнить ее, прежде чем переходить к другим операциям в интерфейсе командной строки. Инструкции по аутентификации см. в статье [Вход с помощью Azure CLI 2.0](/cli/azure/authenticate-azure-cli).

## <a name="register-or-unregister-a-cloud"></a>Регистрация и отмена регистрации облака

Зарегистрируйте новое облако, чтобы использовать свои конечные точки или другой профиль. Облако создается с помощью команды [cloud register](/cli/azure/cloud#register). Для этой команды требуется имя облака. Также можно указать функции и обозначения конечных точек.

Вот как создать облако с определенной конечной точкой для диспетчера ресурсов и с определенным профилем:

```azurecli
az cloud register --name MyCloud --endpoint-resource-manager "https://my.endpoint.manager" --profile 2017-03-09-profile
```

Этот код позволяет создать облако, но _не_ выбрать его автоматически.

Если созданное облако вам больше не нужно, вы можете отменить его регистрацию с помощью команды [cloud unregister](/cli/azure/cloud#unregister).

```azurecli
az cloud unregister --name MyCloud
```

