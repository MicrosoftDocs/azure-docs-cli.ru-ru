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
# <a name="managing-multiple-clouds-with-azure-cli-20"></a><span data-ttu-id="39af2-104">Управление несколькими облаками с помощью Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="39af2-104">Managing multiple clouds with Azure CLI 2.0</span></span>

<span data-ttu-id="39af2-105">При наличии нескольких подписок, связанных с Azure, у вас может быть несколько доступных облаков.</span><span class="sxs-lookup"><span data-stu-id="39af2-105">If you have multiple subscriptions associated with Azure, you may have more than one cloud available.</span></span> <span data-ttu-id="39af2-106">У каждого облака свои связанные конечные точки и возможности. Также облака часто привязаны к определенному региону, в котором приняты свои стандарты и требования к защите данных.</span><span class="sxs-lookup"><span data-stu-id="39af2-106">Each cloud has its own associated endpoints and capabilities, and is often associated with a particular region that has different data protection standards or requirements.</span></span>

<span data-ttu-id="39af2-107">Чтобы эффективно работать с несколькими облаками, требуется возможность переключаться между активными облаками и, возможно, создавать новые.</span><span class="sxs-lookup"><span data-stu-id="39af2-107">To effectively work with multiple clouds, you will need to be able to switch between which is currently active, and possibly create new clouds.</span></span>

## <a name="listing-clouds"></a><span data-ttu-id="39af2-108">Вывод списка облаков</span><span class="sxs-lookup"><span data-stu-id="39af2-108">Listing clouds</span></span>

<span data-ttu-id="39af2-109">Вы можете отобразить список доступных облаков с помощью команды [cloud list](/cli/azure/cloud#list).</span><span class="sxs-lookup"><span data-stu-id="39af2-109">You may list your available clouds with the [cloud list](/cli/azure/cloud#list) command.</span></span> <span data-ttu-id="39af2-110">Так вы узнаете, какое облако активно и какой у него текущий профиль, а также получите сведения о суффиксах регионов и именах узлов.</span><span class="sxs-lookup"><span data-stu-id="39af2-110">This will tell you which cloud is currently active, what its current profile is, and can provide information on regional suffixes and host names.</span></span>

<span data-ttu-id="39af2-111">Вот как получить список доступных облаков и узнать, какое облако сейчас активно:</span><span class="sxs-lookup"><span data-stu-id="39af2-111">To get a list of the available clouds and the currently active one:</span></span>

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

## <a name="switching-the-active-cloud"></a><span data-ttu-id="39af2-112">Переключение активного облака</span><span class="sxs-lookup"><span data-stu-id="39af2-112">Switching the active cloud</span></span>

<span data-ttu-id="39af2-113">Чтобы переключиться с текущего активного облака, выполните команду [cloud set](/cli/azure/cloud#set).</span><span class="sxs-lookup"><span data-stu-id="39af2-113">In order to switch the currently active cloud, you run the [cloud set](/cli/azure/cloud#set) command.</span></span> <span data-ttu-id="39af2-114">Эта команда принимает один обязательный аргумент — имя облака.</span><span class="sxs-lookup"><span data-stu-id="39af2-114">This command takes one required argument, the name of the cloud.</span></span>

```azurecli
az cloud set --name AzureChinaCloud
```

> [!IMPORTANT]
> <span data-ttu-id="39af2-115">Если вы никогда не выполняли аутентификацию для активного облака, вам потребуется выполнить ее, прежде чем переходить к другим операциям в интерфейсе командной строки.</span><span class="sxs-lookup"><span data-stu-id="39af2-115">If you have never authenticated for the active cloud, you will need to do so before performing any other CLI operations.</span></span> <span data-ttu-id="39af2-116">Инструкции по аутентификации см. в статье [Вход с помощью Azure CLI 2.0](/cli/azure/authenticate-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="39af2-116">For instructions on authenticating, see [Log in with Azure CLI 2.0](/cli/azure/authenticate-azure-cli).</span></span>

## <a name="register-or-unregister-a-cloud"></a><span data-ttu-id="39af2-117">Регистрация и отмена регистрации облака</span><span class="sxs-lookup"><span data-stu-id="39af2-117">Register or unregister a cloud</span></span>

<span data-ttu-id="39af2-118">Зарегистрируйте новое облако, чтобы использовать свои конечные точки или другой профиль.</span><span class="sxs-lookup"><span data-stu-id="39af2-118">Register a new cloud if you have your own endpoints or require a different profile.</span></span> <span data-ttu-id="39af2-119">Облако создается с помощью команды [cloud register](/cli/azure/cloud#register).</span><span class="sxs-lookup"><span data-stu-id="39af2-119">Creating a cloud is done with the [cloud register](/cli/azure/cloud#register) command.</span></span> <span data-ttu-id="39af2-120">Для этой команды требуется имя облака. Также можно указать функции и обозначения конечных точек.</span><span class="sxs-lookup"><span data-stu-id="39af2-120">This command requires a name, and optionally a set of capabilities and endpoint designations.</span></span>

<span data-ttu-id="39af2-121">Вот как создать облако с определенной конечной точкой для диспетчера ресурсов и с определенным профилем:</span><span class="sxs-lookup"><span data-stu-id="39af2-121">To create a cloud with a specialized endpoint for the resource manager, with a specific profile:</span></span>

```azurecli
az cloud register --name MyCloud --endpoint-resource-manager "https://my.endpoint.manager" --profile 2017-03-09-profile
```

<span data-ttu-id="39af2-122">Этот код позволяет создать облако, но _не_ выбрать его автоматически.</span><span class="sxs-lookup"><span data-stu-id="39af2-122">This creates the cloud, but does _not_ automatically select it.</span></span>

<span data-ttu-id="39af2-123">Если созданное облако вам больше не нужно, вы можете отменить его регистрацию с помощью команды [cloud unregister](/cli/azure/cloud#unregister).</span><span class="sxs-lookup"><span data-stu-id="39af2-123">If you no longer require the created cloud, it can be unregistered with the [cloud unregister](/cli/azure/cloud#unregister) command:</span></span>

```azurecli
az cloud unregister --name MyCloud
```

