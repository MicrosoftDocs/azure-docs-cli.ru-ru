---
title: Управление несколькими облаками с помощью Azure CLI 2.0
description: Создание, вход и администрирование нескольких облаков с помощью Azure CLI 2.0.
author: sptramer
manager: carmonm
ms.author: sttramer
ms.date: 10/20/2017
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 98915fb43f2ad3eb45164f7e47c1a41345f3f9c5
ms.sourcegitcommit: ae72b6c8916aeb372a92188090529037e63930ba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2018
---
# <a name="managing-multiple-clouds-with-azure-cli-20"></a>Управление несколькими облаками с помощью Azure CLI 2.0

При работе в разных регионах или использовании [Azure Stack](https://docs.microsoft.com/azure/azure-stack/user/) вам может понадобиться несколько облаков. Корпорация Майкрософт предоставляет доступные для использования облака в соответствии с местным законодательством в пределах каждого региона. В этой статье показано, как получить информацию о доступных для вашей учетной записи облаках, об изменении текущего облака, а также о регистрации и отмене регистрации новых облаков для использования с Azure Stack.

## <a name="listing-clouds"></a>Вывод списка облаков

Вы можете отобразить список доступных облаков с помощью команды [az cloud list](/cli/azure/cloud#az-cloud-list). Так вы узнаете, какое облако сейчас используется и какой у него текущий профиль, а также получите сведения о суффиксах регионов и именах узлов.

Получить сведения об активном облаке и полном списке доступных облаков можно так:

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

Активное сейчас облако обозначено значением `True` в столбце `IsActive`. В одно и то же время использоваться может только одно облако. Получить дополнительные сведения об облаке, включая описание конечных точек, используемых им для служб Azure, можно с помощью команды `cloud show`:

```azurecli
az cloud show --name AzureChinaCloud --output json
```

```output
{
  "endpoints": {
    "activeDirectory": "https://login.chinacloudapi.cn",
    "activeDirectoryDataLakeResourceId": null,
    "activeDirectoryGraphResourceId": "https://graph.chinacloudapi.cn/",
    "activeDirectoryResourceId": "https://management.core.chinacloudapi.cn/",
    "batchResourceId": "https://batch.chinacloudapi.cn/",
    "gallery": "https://gallery.chinacloudapi.cn/",
    "management": "https://management.core.chinacloudapi.cn/",
    "resourceManager": "https://management.chinacloudapi.cn",
    "sqlManagement": "https://management.core.chinacloudapi.cn:8443/",
    "vmImageAliasDoc": "https://raw.githubusercontent.com/Azure/azure-rest-api-specs/master/arm-compute/quickstart-templates/aliases.json"
  },
  "isActive": false,
  "name": "AzureChinaCloud",
  "profile": "latest",
  "suffixes": {
    "azureDatalakeAnalyticsCatalogAndJobEndpoint": null,
    "azureDatalakeStoreFileSystemEndpoint": null,
    "keyvaultDns": ".vault.azure.cn",
    "sqlServerHostname": ".database.chinacloudapi.cn",
    "storageEndpoint": "core.chinacloudapi.cn"
  }
}
```

## <a name="switching-the-active-cloud"></a>Переключение активного облака

Чтобы переключиться с активного сейчас облака, выполните команду [az cloud set](/cli/azure/cloud#az-cloud-set). Эта команда принимает один обязательный аргумент — имя облака.

```azurecli
az cloud set --name AzureChinaCloud
```

> [!IMPORTANT]
> Если срок действия аутентификации для активации облака истек, необходимо повторно выполнить аутентификацию, прежде чем выполнять другие задачи CLI. Если вы переключаетесь на новое облако впервые, вам также понадобится настроить активную подписку.
> Инструкции по аутентификации см. в статье [Вход с помощью Azure CLI 2.0](authenticate-azure-cli.md). Сведения об управлении подписками см. в руководстве по [управлению подписками Azure с помощью Azure CLI 2.0](manage-azure-subscriptions-azure-cli.md).

## <a name="register-a-cloud"></a>Регистрация облака

Зарегистрируйте новое облако, если у вас есть свои конечные точки для Azure Stack. Облако создается с помощью команды [az cloud register](/cli/azure/cloud#az-cloud-register). Для этой команды требуется имя облака и набор функций для связанных конечных точек. Дополнительные сведения о регистрации облака для использования Azure Stack см. в статье [Использование профилей версий API и Azure CLI 2.0 в Azure Stack](/azure/azure-stack/user/azure-stack-version-profiles-azurecli2#connect-to-azure-stack).

Вам не нужно регистрировать свое облако в таких регионах, как Китай или Германия, а также для использования в государственных организациях США. Эти облака управляются корпорацией Майкрософт и доступны по умолчанию.  Дополнительные сведения обо всех доступных конечных точках см. в [документации по `az cloud register`](/cli/azure/cloud#az-cloud-register).

Регистрация в облаке не предусматривает автоматическое переключение на него. Используйте команду `az cloud set`, чтобы выбрать только что созданное облако, как описано выше.

## <a name="update-an-existing-cloud"></a>Обновление существующего облака

При наличии соответствующих разрешений вы также можете обновить существующее облако. Это необходимо сделать, если вам нужно переключиться на другой профиль Azure, а также добавить или изменить конечную точку.
Это можно сделать с помощью команды [az cloud update](/cli/azure/cloud#az-cloud-update), которая принимает те же аргументы, что и команда `az cloud register`.

## <a name="unregister-a-cloud"></a>Отмена регистрации облака

Если зарегистрированное облако вам больше не нужно, вы можете отменить его регистрацию с помощью команды [az cloud unregister](/cli/azure/cloud#az-cloud-unregister):

```azurecli
az cloud unregister --name MyCloud
```
