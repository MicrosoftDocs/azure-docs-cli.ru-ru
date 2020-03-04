---
title: Выбор облаков с помощью Azure CLI
description: Создание и администрирование нескольких облаков и вход в них с помощью Azure CLI.
author: dbradish-microsoft
manager: barbkess
ms.author: dbradish
ms.date: 09/09/2018
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 8e24a4740d97ddf67f81e60fef9217a4e72daab0
ms.sourcegitcommit: 7caa6673f65e61deb8d6def6386e4eb9acdac923
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/28/2020
ms.locfileid: "77779471"
---
# <a name="select-clouds-with-the-azure-cli"></a><span data-ttu-id="e9de0-103">Выбор облаков с помощью Azure CLI</span><span class="sxs-lookup"><span data-stu-id="e9de0-103">Select clouds with the Azure CLI</span></span>

<span data-ttu-id="e9de0-104">При работе в разных регионах или использовании [Azure Stack](https://docs.microsoft.com/azure/azure-stack/user/) вам может понадобиться несколько облаков.</span><span class="sxs-lookup"><span data-stu-id="e9de0-104">If you work across different regions or use [Azure Stack](https://docs.microsoft.com/azure/azure-stack/user/), you may need to use more than one cloud.</span></span> <span data-ttu-id="e9de0-105">Корпорация Майкрософт предоставляет доступные для использования облака в соответствии с местным законодательством в пределах каждого региона.</span><span class="sxs-lookup"><span data-stu-id="e9de0-105">Microsoft provides clouds for compliance with regional laws, which are available for your use.</span></span> <span data-ttu-id="e9de0-106">В этой статье показано, как получить сведения об облаках, изменить текущее облако, а также зарегистрировать новые облака или отменить их регистрацию.</span><span class="sxs-lookup"><span data-stu-id="e9de0-106">This article shows you how to get information on clouds, change the current cloud, and register or unregister new clouds.</span></span>

## <a name="list-available-clouds"></a><span data-ttu-id="e9de0-107">Получение списка доступных облаков</span><span class="sxs-lookup"><span data-stu-id="e9de0-107">List available clouds</span></span>

<span data-ttu-id="e9de0-108">Вы можете отобразить список доступных облаков с помощью команды [az cloud list](/cli/azure/cloud#az-cloud-list).</span><span class="sxs-lookup"><span data-stu-id="e9de0-108">You can list available clouds with the [az cloud list](/cli/azure/cloud#az-cloud-list) command.</span></span> <span data-ttu-id="e9de0-109">Эта команда показывает, какое облако сейчас используется и какой у него текущий профиль, а также отображает сведения о суффиксах регионов и именах узлов.</span><span class="sxs-lookup"><span data-stu-id="e9de0-109">This command shows which cloud is currently active, what its current profile is, and information on regional suffixes and host names.</span></span>

<span data-ttu-id="e9de0-110">Получить сведения об активном облаке и полном списке доступных облаков можно так:</span><span class="sxs-lookup"><span data-stu-id="e9de0-110">To get the active cloud and a list of all the available clouds:</span></span>

```azurecli-interactive
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

<span data-ttu-id="e9de0-111">Активное сейчас облако обозначено значением `True` в столбце `IsActive`.</span><span class="sxs-lookup"><span data-stu-id="e9de0-111">The currently active cloud has `True` in the `IsActive` column.</span></span> <span data-ttu-id="e9de0-112">В одно и то же время использоваться может только одно облако.</span><span class="sxs-lookup"><span data-stu-id="e9de0-112">Only one cloud can be active at any time.</span></span> <span data-ttu-id="e9de0-113">Получить дополнительные сведения об облаке, включая описание конечных точек, используемых им для служб Azure, можно с помощью команды `cloud show`:</span><span class="sxs-lookup"><span data-stu-id="e9de0-113">To get more detailed information on a cloud, including the endpoints that it uses for Azure services, use the `cloud show` command:</span></span>

```azurecli-interactive
az cloud show --name AzureChinaCloud --output json
```

```json
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

## <a name="switch-the-active-cloud"></a><span data-ttu-id="e9de0-114">Изменение активного облака</span><span class="sxs-lookup"><span data-stu-id="e9de0-114">Switch the active cloud</span></span>

<span data-ttu-id="e9de0-115">Чтобы задать облако по умолчанию с помощью файла конфигурации, ознакомьтесь с разделом [Переменные среды и значения конфигурации CLI](/cli/azure/azure-cli-configuration?view=azure-cli-latest#cli-configuration-values-and-environment-variables).</span><span class="sxs-lookup"><span data-stu-id="e9de0-115">To set the default cloud using a configuration file, see [CLI configuration values and environment variables](/cli/azure/azure-cli-configuration?view=azure-cli-latest#cli-configuration-values-and-environment-variables).</span></span>  <span data-ttu-id="e9de0-116">Чтобы переключиться с активного сейчас облака, выполните команду [az cloud set](/cli/azure/cloud#az-cloud-set).</span><span class="sxs-lookup"><span data-stu-id="e9de0-116">To switch the active cloud, run the [az cloud set](/cli/azure/cloud#az-cloud-set) command.</span></span> <span data-ttu-id="e9de0-117">Эта команда принимает один обязательный аргумент — имя облака.</span><span class="sxs-lookup"><span data-stu-id="e9de0-117">This command takes one required argument, the name of the cloud.</span></span>

```azurecli-interactive
az cloud set --name AzureChinaCloud
```

> [!IMPORTANT]
> <span data-ttu-id="e9de0-118">Если срок действия аутентификации для активации облака истек, необходимо повторно выполнить аутентификацию, прежде чем выполнять другие задачи CLI.</span><span class="sxs-lookup"><span data-stu-id="e9de0-118">If your authentication for the activated cloud has expired, you need to re-authenticate before performing any other CLI tasks.</span></span> <span data-ttu-id="e9de0-119">Если вы переключаетесь на новое облако впервые, вам также понадобится настроить активную подписку.</span><span class="sxs-lookup"><span data-stu-id="e9de0-119">If this is your first time switching to the new cloud, you also need to set the active subscription.</span></span>
> <span data-ttu-id="e9de0-120">Инструкции по проверке подлинности см. в статье [Вход с помощью Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="e9de0-120">For instructions on authenticating, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span> <span data-ttu-id="e9de0-121">Сведения об управлении подписками см. в руководстве по [управлению подписками Azure с помощью Azure CLI](manage-azure-subscriptions-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="e9de0-121">For information on subscription management, see [Manage Azure subscriptions with Azure CLI](manage-azure-subscriptions-azure-cli.md)</span></span>

## <a name="register-a-new-cloud"></a><span data-ttu-id="e9de0-122">Регистрация нового облака</span><span class="sxs-lookup"><span data-stu-id="e9de0-122">Register a new cloud</span></span>

<span data-ttu-id="e9de0-123">Зарегистрируйте новое облако, если у вас есть свои конечные точки для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="e9de0-123">Register a new cloud if you have your own endpoints for Azure Stack.</span></span> <span data-ttu-id="e9de0-124">Облако создается с помощью команды [az cloud register](/cli/azure/cloud#az-cloud-register).</span><span class="sxs-lookup"><span data-stu-id="e9de0-124">Creating a cloud is done with the [az cloud register](/cli/azure/cloud#az-cloud-register) command.</span></span> <span data-ttu-id="e9de0-125">Для этой команды требуется имя и набор конечных точек службы.</span><span class="sxs-lookup"><span data-stu-id="e9de0-125">This command requires a name and a set of service endpoints.</span></span> <span data-ttu-id="e9de0-126">Сведения о регистрации облака для использования Azure Stack см. в статье [Использование профилей версий API и Azure CLI в Azure Stack](/azure/azure-stack/user/azure-stack-version-profiles-azurecli2#connect-to-azure-stack).</span><span class="sxs-lookup"><span data-stu-id="e9de0-126">To learn how to register a cloud for use with Azure Stack, see [Use API version profiles with Azure CLI in Azure Stack](/azure/azure-stack/user/azure-stack-version-profiles-azurecli2#connect-to-azure-stack).</span></span>

<span data-ttu-id="e9de0-127">Вам не нужно регистрировать сведения в регионах "Китай", "US Government" или "Германия".</span><span class="sxs-lookup"><span data-stu-id="e9de0-127">You don't need to register information for the China, US Government, or German regions.</span></span> <span data-ttu-id="e9de0-128">Эти облака управляются корпорацией Майкрософт и доступны по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e9de0-128">These clouds are managed by Microsoft and available by default.</span></span>  <span data-ttu-id="e9de0-129">Дополнительные сведения обо всех доступных конечных точках см. в [документации по `az cloud register`](/cli/azure/cloud#az-cloud-register).</span><span class="sxs-lookup"><span data-stu-id="e9de0-129">For more information on all of the available endpoint settings, see the [documentation for `az cloud register`](/cli/azure/cloud#az-cloud-register).</span></span>

<span data-ttu-id="e9de0-130">Регистрация в облаке не подразумевает автоматическое переключение на него.</span><span class="sxs-lookup"><span data-stu-id="e9de0-130">Registering a cloud doesn't automatically switch to it.</span></span> <span data-ttu-id="e9de0-131">Для выбора нового облака используйте команду `az cloud set`.</span><span class="sxs-lookup"><span data-stu-id="e9de0-131">Use the `az cloud set` command to select the newly created cloud.</span></span>

## <a name="update-an-existing-cloud"></a><span data-ttu-id="e9de0-132">Обновление существующего облака</span><span class="sxs-lookup"><span data-stu-id="e9de0-132">Update an existing cloud</span></span>

<span data-ttu-id="e9de0-133">При наличии соответствующих разрешений вы также можете обновить существующее облако.</span><span class="sxs-lookup"><span data-stu-id="e9de0-133">If you have permissions, you can also update an existing cloud.</span></span> <span data-ttu-id="e9de0-134">Обновление облака приводит к переключению на другой профиль служб Azure или изменению конечных точек подключения.</span><span class="sxs-lookup"><span data-stu-id="e9de0-134">Updating a cloud switches to a different Azure services profile or modifies the connection endpoints.</span></span>
<span data-ttu-id="e9de0-135">Это можно сделать с помощью команды [az cloud update](/cli/azure/cloud#az-cloud-update), которая принимает те же аргументы, что и команда `az cloud register`.</span><span class="sxs-lookup"><span data-stu-id="e9de0-135">Update a cloud with the [az cloud update](/cli/azure/cloud#az-cloud-update) command, which takes the same arguments as `az cloud register`.</span></span>

## <a name="unregister-a-cloud"></a><span data-ttu-id="e9de0-136">Отмена регистрации облака</span><span class="sxs-lookup"><span data-stu-id="e9de0-136">Unregister a cloud</span></span>

<span data-ttu-id="e9de0-137">Если созданное облако вам больше не нужно, его регистрацию можно отменить с помощью команды [az cloud unregister](/cli/azure/cloud#az-cloud-unregister):</span><span class="sxs-lookup"><span data-stu-id="e9de0-137">If you no longer need a created cloud, it can be unregistered with the [az cloud unregister](/cli/azure/cloud#az-cloud-unregister) command:</span></span>

```azurecli-interactive
az cloud unregister --name MyCloud
```
