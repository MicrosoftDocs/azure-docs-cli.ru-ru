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
# <a name="azure-cli-for-azure-data-share"></a><span data-ttu-id="3b55d-103">Azure CLI для Azure Data Share</span><span class="sxs-lookup"><span data-stu-id="3b55d-103">Azure CLI for Azure Data Share</span></span>

<span data-ttu-id="3b55d-104">Интерфейс командной строки Azure ([Azure CLI](/cli/azure/what-is-azure-cli)) — это набор команд для создания ресурсов Azure и управления ими.</span><span class="sxs-lookup"><span data-stu-id="3b55d-104">The Azure Command Line Interface ([Azure CLI](/cli/azure/what-is-azure-cli)) is a set of commands used to create and manage Azure resources.</span></span>  <span data-ttu-id="3b55d-105">Он доступен во многих службах Azure, включая Azure Data Share.</span><span class="sxs-lookup"><span data-stu-id="3b55d-105">It is available across many Azure services including Azure Data Share.</span></span>  <span data-ttu-id="3b55d-106">Для Data Share существует более 65 разных команд.</span><span class="sxs-lookup"><span data-stu-id="3b55d-106">There are over 65 different commands for data share!</span></span>  <span data-ttu-id="3b55d-107">Эти команды дают возможность эффективно работать со службой с помощью командной строки.</span><span class="sxs-lookup"><span data-stu-id="3b55d-107">These commands give you the ability to work effectively with the service from a command line.</span></span>

## <a name="references-for-data-share"></a><span data-ttu-id="3b55d-108">Справочники для Data Share</span><span class="sxs-lookup"><span data-stu-id="3b55d-108">References for Data Share</span></span>

<span data-ttu-id="3b55d-109">Все команды Azure CLI для Azure Data Share сейчас являются расширениями Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="3b55d-109">All Azure CLI commands for Azure Data Share are currently extensions to the Azure CLI.</span></span>  <span data-ttu-id="3b55d-110">Расширение предоставляет доступ к экспериментальным и предварительным версиям командам.</span><span class="sxs-lookup"><span data-stu-id="3b55d-110">An extension gives you access to experimental and pre-release commands.</span></span>  <span data-ttu-id="3b55d-111">Узнайте больше о расширениях из статьи [Использование расширений с Azure CLI](/cli/azure/azure-cli-extensions-overview).</span><span class="sxs-lookup"><span data-stu-id="3b55d-111">Find out more about extension references in [Use extensions with Azure CLI](/cli/azure/azure-cli-extensions-overview).</span></span>

|<span data-ttu-id="3b55d-112">Справочник по Azure CLI</span><span class="sxs-lookup"><span data-stu-id="3b55d-112">Azure CLI Reference</span></span> |<span data-ttu-id="3b55d-113">Описание</span><span class="sxs-lookup"><span data-stu-id="3b55d-113">Description</span></span>
|-|-|-|
| [<span data-ttu-id="3b55d-114">az datashare</span><span class="sxs-lookup"><span data-stu-id="3b55d-114">az datashare</span></span>](/cli/azure/ext/datashare/datashare) | <span data-ttu-id="3b55d-115">Все команды для управления Azure Data Share.</span><span class="sxs-lookup"><span data-stu-id="3b55d-115">All commands to manage Azure Data Share.</span></span>
| [<span data-ttu-id="3b55d-116">az datashare account</span><span class="sxs-lookup"><span data-stu-id="3b55d-116">az datashare account</span></span>](/cli/azure/ext/datashare/datashare/account) | <span data-ttu-id="3b55d-117">Команды для управления учетными записями Azure Data Share.</span><span class="sxs-lookup"><span data-stu-id="3b55d-117">Commands to manage Azure Data Share accounts.</span></span>
| [<span data-ttu-id="3b55d-118">az datashare consumer</span><span class="sxs-lookup"><span data-stu-id="3b55d-118">az datashare consumer</span></span>](/cli/azure/ext/datashare/datashare/consumer) | <span data-ttu-id="3b55d-119">Команды для потребителей для управления Azure Data Share.</span><span class="sxs-lookup"><span data-stu-id="3b55d-119">Commands for consumers to manage Azure Data Share.</span></span>
| [<span data-ttu-id="3b55d-120">az datashare dataset</span><span class="sxs-lookup"><span data-stu-id="3b55d-120">az datashare dataset</span></span>](/cli/azure/ext/datashare/datashare/dataset) | <span data-ttu-id="3b55d-121">Команды для поставщиков для управления наборами данных Azure Data Share.</span><span class="sxs-lookup"><span data-stu-id="3b55d-121">Commands for providers to manage Azure Data Share datasets.</span></span>
| [<span data-ttu-id="3b55d-122">az datashare invitation</span><span class="sxs-lookup"><span data-stu-id="3b55d-122">az datashare invitation</span></span>](/cli/azure/ext/datashare/datashare/invitation) | <span data-ttu-id="3b55d-123">Команды для потребителей для управления приглашениями Azure Data Share.</span><span class="sxs-lookup"><span data-stu-id="3b55d-123">Commands for consumers to manage Azure Data Share invitations.</span></span>
| [<span data-ttu-id="3b55d-124">az datashare provider-share-subscription</span><span class="sxs-lookup"><span data-stu-id="3b55d-124">az datashare provider-share-subscription</span></span>](/cli/azure/ext/datashare/datashare/provider-share-subscription) | <span data-ttu-id="3b55d-125">Команды для поставщиков для управления подписками Azure Data Share.</span><span class="sxs-lookup"><span data-stu-id="3b55d-125">Commands for providers to manage Azure Data Share subscriptions.</span></span>
| [<span data-ttu-id="3b55d-126">az datashare synchronization</span><span class="sxs-lookup"><span data-stu-id="3b55d-126">az datashare synchronization</span></span>](/cli/azure/ext/datashare/datashare/synchronization)  | <span data-ttu-id="3b55d-127">Команды для управления синхронизацией Azure Data Share.</span><span class="sxs-lookup"><span data-stu-id="3b55d-127">Commands to manage Azure Data Share synchronization.</span></span>
| [<span data-ttu-id="3b55d-128">az datashare synchronization-setting</span><span class="sxs-lookup"><span data-stu-id="3b55d-128">az datashare synchronization-setting</span></span>](/cli/azure/ext/datashare/datashare/synchronization-setting)  | <span data-ttu-id="3b55d-129">Команды для поставщиков для управления параметрами синхронизации Azure Data Share.</span><span class="sxs-lookup"><span data-stu-id="3b55d-129">Commands for providers to manage Azure Data Share synchronization settings.</span></span>

## <a name="reference-examples"></a><span data-ttu-id="3b55d-130">Примеры справочников</span><span class="sxs-lookup"><span data-stu-id="3b55d-130">Reference examples</span></span>

<span data-ttu-id="3b55d-131">Примеры приведены для каждого справочника по Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="3b55d-131">Examples are provided with every Azure CLI reference.</span></span> <span data-ttu-id="3b55d-132">Хотя эти задачи также можно выполнить с помощью портала Azure, при использовании Azure CLI требуется одна командная строка.</span><span class="sxs-lookup"><span data-stu-id="3b55d-132">Although you can also complete these tasks through the Azure portal, using the Azure CLI requires a single command line.</span></span>  <span data-ttu-id="3b55d-133">Ниже представлено несколько блоков кода, которые помогут вам понять, насколько просто использовать Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="3b55d-133">Here are a few code blocks to give you an idea of how easy it is to use the Azure CLI.</span></span>

<span data-ttu-id="3b55d-134">Для работы с Azure Data Share вам потребуется группа ресурсов.</span><span class="sxs-lookup"><span data-stu-id="3b55d-134">To work with Azure Data Share, you'll first need a resource group.</span></span>  <span data-ttu-id="3b55d-135">Группы ресурсов Azure можно без усилий создавать и администрировать с помощью Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="3b55d-135">Azure resource groups are simple to create and manage with the Azure CLI.</span></span>  

```azurecli
#create a resource group
az group create -location westus -name MyResourceGroup
```

```azurecli
#get a list of resource groups for a subscription
az group list --subscription MySubscription --output table
```

<span data-ttu-id="3b55d-136">Создать учетную запись Data Share очень просто.</span><span class="sxs-lookup"><span data-stu-id="3b55d-136">It is as straightforward to create a data share account.</span></span>

```azurecli
#create a data share account
az datashare account create --location "West US 2" --tags tag1=Red tag2=White --name MyAccount --resource-group MyResourceGroup
```

## <a name="see-also"></a><span data-ttu-id="3b55d-137">См. также раздел</span><span class="sxs-lookup"><span data-stu-id="3b55d-137">See also</span></span>

* <span data-ttu-id="3b55d-138">[Начните работу с Azure CLI](/cli/azure/get-started-with-azure-cli), чтобы узнать об установке и входе.</span><span class="sxs-lookup"><span data-stu-id="3b55d-138">[Get started with Azure CLI](/cli/azure/get-started-with-azure-cli) to learn about installation and sign in.</span></span>

* <span data-ttu-id="3b55d-139">Найдите дополнительные справочники по [основным командам](/cli/azure/reference-index) и [командам расширения](/cli/azure/azure-cli-extensions-list) в документации по Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="3b55d-139">Discover additional [core](/cli/azure/reference-index) and [extension](/cli/azure/azure-cli-extensions-list) references in the Azure CLI documentation.</span></span>
