---
title: "Управление несколькими облаками с помощью Azure CLI 2.0"
description: "Создавайте, администрируйте и входите в разные облака с помощью Azure CLI 2.0."
keywords: Azure CLI 2.0, Azure, clouds, datacenters, government, region, china, germany
author: sptramer
manager: routlaw
ms.author: sttramer
ms.date: 10/20/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.openlocfilehash: cb470d179daf7cb4ecf535903adb12071602034e
ms.sourcegitcommit: 905939cc44764b4d1cc79a9b36c0793f7055a686
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/20/2017
---
# <a name="managing-multiple-clouds-with-azure-cli-20"></a><span data-ttu-id="fea66-104">Управление несколькими облаками с помощью Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="fea66-104">Managing multiple clouds with Azure CLI 2.0</span></span>

<span data-ttu-id="fea66-105">При работе в разных регионах или использовании [Azure Stack](https://docs.microsoft.com/en-us/azure/azure-stack/user/) вам может понадобиться несколько облаков.</span><span class="sxs-lookup"><span data-stu-id="fea66-105">If you work across different regions or use [Azure Stack](https://docs.microsoft.com/en-us/azure/azure-stack/user/), you may need to use more than one cloud.</span></span> <span data-ttu-id="fea66-106">Корпорация Майкрософт предоставляет доступные для использования облака в соответствии с местным законодательством в пределах каждого региона.</span><span class="sxs-lookup"><span data-stu-id="fea66-106">Microsoft provides clouds for compliance with regional laws, which are available for your use.</span></span> <span data-ttu-id="fea66-107">В этой статье показано, как получить информацию о доступных для вашей учетной записи облаках, об изменении текущего облака, а также о регистрации и отмене регистрации новых облаков для использования с Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="fea66-107">This article shows you how to get information on clouds available to your account, change the current cloud, and register or unregister new clouds for use with Azure Stack.</span></span>

## <a name="listing-clouds"></a><span data-ttu-id="fea66-108">Вывод списка облаков</span><span class="sxs-lookup"><span data-stu-id="fea66-108">Listing clouds</span></span>

<span data-ttu-id="fea66-109">Вы можете отобразить список доступных облаков с помощью команды [cloud list](/cli/azure/cloud#list).</span><span class="sxs-lookup"><span data-stu-id="fea66-109">You can list available clouds with the [cloud list](/cli/azure/cloud#list) command.</span></span> <span data-ttu-id="fea66-110">Так вы узнаете, какое облако сейчас используется и какой у него текущий профиль, а также получите сведения о суффиксах регионов и именах узлов.</span><span class="sxs-lookup"><span data-stu-id="fea66-110">This tells you which cloud is currently active, what its current profile is, and information on regional suffixes and host names.</span></span>

<span data-ttu-id="fea66-111">Получить сведения об активном облаке и полном списке доступных облаков можно так:</span><span class="sxs-lookup"><span data-stu-id="fea66-111">To get the active cloud and a list of all the available clouds:</span></span>

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

<span data-ttu-id="fea66-112">Активное сейчас облако обозначено значением `True` в столбце `IsActive`.</span><span class="sxs-lookup"><span data-stu-id="fea66-112">The currently active cloud has `True` in the `IsActive` column.</span></span> <span data-ttu-id="fea66-113">В одно и то же время использоваться может только одно облако.</span><span class="sxs-lookup"><span data-stu-id="fea66-113">Only one cloud can be active at any time.</span></span> <span data-ttu-id="fea66-114">Получить дополнительные сведения об облаке, включая описание конечных точек, используемых им для служб Azure, можно с помощью команды `cloud show`:</span><span class="sxs-lookup"><span data-stu-id="fea66-114">To get more detailed information on a cloud, including the endpoints that it uses for Azure services, use the `cloud show` command:</span></span>

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

## <a name="switching-the-active-cloud"></a><span data-ttu-id="fea66-115">Переключение активного облака</span><span class="sxs-lookup"><span data-stu-id="fea66-115">Switching the active cloud</span></span>

<span data-ttu-id="fea66-116">Чтобы переключиться с активного сейчас облака, выполните команду [cloud set](/cli/azure/cloud#set).</span><span class="sxs-lookup"><span data-stu-id="fea66-116">To switch the currently active cloud, run the [cloud set](/cli/azure/cloud#set) command.</span></span> <span data-ttu-id="fea66-117">Эта команда принимает один обязательный аргумент — имя облака.</span><span class="sxs-lookup"><span data-stu-id="fea66-117">This command takes one required argument, the name of the cloud.</span></span>

```azurecli
az cloud set --name AzureChinaCloud
```

> [!IMPORTANT]
> <span data-ttu-id="fea66-118">Если срок действия аутентификации для активации облака истек, необходимо повторно выполнить аутентификацию, прежде чем выполнять другие задачи CLI.</span><span class="sxs-lookup"><span data-stu-id="fea66-118">If your authentication for the activated cloud has expired, you need to re-authenticate before performing any other CLI tasks.</span></span> <span data-ttu-id="fea66-119">Если вы переключаетесь на новое облако впервые, вам также понадобится настроить активную подписку.</span><span class="sxs-lookup"><span data-stu-id="fea66-119">If this is your first time switching to the new cloud, you also need to set the active subscription.</span></span>
> <span data-ttu-id="fea66-120">Инструкции по аутентификации см. в статье [Вход с помощью Azure CLI 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="fea66-120">For instructions on authenticating, see [Log in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span> <span data-ttu-id="fea66-121">Сведения об управлении подписками см. в руководстве по [управлению подписками Azure с помощью Azure CLI 2.0](manage-azure-subscriptions-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="fea66-121">For information on subscription management, see [Manage Azure subscriptions with Azure CLI 2.0](manage-azure-subscriptions-azure-cli.md)</span></span>

## <a name="register-a-cloud"></a><span data-ttu-id="fea66-122">Регистрация облака</span><span class="sxs-lookup"><span data-stu-id="fea66-122">Register a cloud</span></span>

<span data-ttu-id="fea66-123">Зарегистрируйте новое облако, если у вас есть свои конечные точки для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="fea66-123">Register a new cloud if you have your own endpoints for Azure Stack.</span></span> <span data-ttu-id="fea66-124">Облако создается с помощью команды [cloud register](/cli/azure/cloud#register).</span><span class="sxs-lookup"><span data-stu-id="fea66-124">Creating a cloud is done with the [cloud register](/cli/azure/cloud#register) command.</span></span> <span data-ttu-id="fea66-125">Для этой команды требуется имя облака и набор функций для связанных конечных точек.</span><span class="sxs-lookup"><span data-stu-id="fea66-125">This command requires a name and a set of capabilities with associated endpoints.</span></span> <span data-ttu-id="fea66-126">Дополнительные сведения о регистрации в облаке для использования Azure Stack см. в руководстве по [установке и настройке CLI для использования с Azure Stack](/azure/azure-stack/user/azure-stack-connect-cli#connect-to-azure-stack).</span><span class="sxs-lookup"><span data-stu-id="fea66-126">To learn how to register a cloud for use with Azure Stack, see [Install and configure CLI for use with Azure Stack](/azure/azure-stack/user/azure-stack-connect-cli#connect-to-azure-stack).</span></span>  

<span data-ttu-id="fea66-127">Вам не нужно регистрировать свое облако в таких регионах, как Китай или Германия, а также для использования в государственных организациях США.</span><span class="sxs-lookup"><span data-stu-id="fea66-127">You do not need to register your own cloud for China, US Government, or German regions.</span></span> <span data-ttu-id="fea66-128">Эти облака управляются корпорацией Майкрософт и доступны по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="fea66-128">These are managed by Microsoft and available by default.</span></span>  <span data-ttu-id="fea66-129">Дополнительные сведения обо всех доступных конечных точках см. в [документации по `az cloud register`](/cli/azure/cloud?view=azure-cli-latest#az_cloud_register).</span><span class="sxs-lookup"><span data-stu-id="fea66-129">For more information on all of the available endpoint settings, see the [documentation for `az cloud register`](/cli/azure/cloud?view=azure-cli-latest#az_cloud_register).</span></span>

<span data-ttu-id="fea66-130">Регистрация в облаке не предусматривает автоматическое переключение на него.</span><span class="sxs-lookup"><span data-stu-id="fea66-130">Registering a cloud does not automatically switch to it.</span></span> <span data-ttu-id="fea66-131">Используйте команду `az cloud set`, чтобы выбрать только что созданное облако, как описано выше.</span><span class="sxs-lookup"><span data-stu-id="fea66-131">Use the `az cloud set` command to select the newly created cloud as described above.</span></span>

## <a name="update-an-existing-cloud"></a><span data-ttu-id="fea66-132">Обновление существующего облака</span><span class="sxs-lookup"><span data-stu-id="fea66-132">Update an existing cloud</span></span>

<span data-ttu-id="fea66-133">При наличии соответствующих разрешений вы также можете обновить существующее облако.</span><span class="sxs-lookup"><span data-stu-id="fea66-133">If you have permissions, you can also update an existing cloud.</span></span> <span data-ttu-id="fea66-134">Это необходимо сделать, если вам нужно переключиться на другой профиль Azure, а также добавить или изменить конечную точку.</span><span class="sxs-lookup"><span data-stu-id="fea66-134">Do this when you need to switch to a different Azure profile, add an endpoint, or change an endpoint.</span></span>
<span data-ttu-id="fea66-135">Это можно сделать с помощью команды `az cloud update`, которая принимает те же аргументы, что и команда `az cloud register`.</span><span class="sxs-lookup"><span data-stu-id="fea66-135">You do this with the `az cloud update` command, which takes the same arguments as `az cloud register`.</span></span> <span data-ttu-id="fea66-136">Дополнительные сведения см. в [документации по `az cloud update`](/cli/azure/cloud?view=azure-cli-latest#az_cloud_update).</span><span class="sxs-lookup"><span data-stu-id="fea66-136">For more information, see the [documentation for `az cloud update`](/cli/azure/cloud?view=azure-cli-latest#az_cloud_update).</span></span>

## <a name="unregister-a-cloud"></a><span data-ttu-id="fea66-137">Отмена регистрации облака</span><span class="sxs-lookup"><span data-stu-id="fea66-137">Unregister a cloud</span></span>

<span data-ttu-id="fea66-138">Если зарегистрированное облако вам больше не нужно, вы можете отменить его регистрацию с помощью команды [cloud unregister](/cli/azure/cloud#unregister).</span><span class="sxs-lookup"><span data-stu-id="fea66-138">If you no longer require a registered cloud, it can be unregistered with the [cloud unregister](/cli/azure/cloud#unregister) command:</span></span>

```azurecli
az cloud unregister --name MyCloud
```
