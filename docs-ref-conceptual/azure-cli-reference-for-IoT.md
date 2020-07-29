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
ms.openlocfilehash: aa4653ceaba41709cd54a098f649a9c922e93fa8
ms.sourcegitcommit: 05ef6cb6cf049d8c8eb54dd408f56cb145fb5905
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/29/2020
ms.locfileid: "87374394"
---
# <a name="azure-cli-for-azure-iot"></a><span data-ttu-id="81a00-103">Azure CLI для Azure IoT</span><span class="sxs-lookup"><span data-stu-id="81a00-103">Azure CLI for Azure IoT</span></span>

<span data-ttu-id="81a00-104">Интерфейс командной строки Azure ([Azure CLI](/cli/azure/what-is-azure-cli)) — это набор команд для создания ресурсов Azure и управления ими.</span><span class="sxs-lookup"><span data-stu-id="81a00-104">The Azure Command Line Interface ([Azure CLI](/cli/azure/what-is-azure-cli)) is a set of commands used to create and manage Azure resources.</span></span>  <span data-ttu-id="81a00-105">Он доступен во многих службах Azure, включая Azure IoT.</span><span class="sxs-lookup"><span data-stu-id="81a00-105">It is available across many Azure services including Azure IoT.</span></span>  <span data-ttu-id="81a00-106">Существует более 100 справочников для Azure IoT, которые помогают эффективно работать со службами Интернета вещей из командной строки.</span><span class="sxs-lookup"><span data-stu-id="81a00-106">There are over 100 references for Azure IoT giving you the ability to work effectively with IoT services from a command line.</span></span>

## <a name="references-for-iot"></a><span data-ttu-id="81a00-107">Справочники для Интернета вещей</span><span class="sxs-lookup"><span data-stu-id="81a00-107">References for IoT</span></span>

<span data-ttu-id="81a00-108">Интерфейс командной строки для Azure IoT состоит из двух частей: Azure CLI (обычно называется **основной** CLI) и **расширение** CLI для Azure IoT.</span><span class="sxs-lookup"><span data-stu-id="81a00-108">The Azure IoT CLI experience is composed of two parts: Azure CLI (commonly referred to as CLI **core**) and the Azure IoT CLI **extension**.</span></span>

<span data-ttu-id="81a00-109">Возможности Интернета вещей в **основном** Azure CLI предназначены для администрирования и настройки инфраструктуры.</span><span class="sxs-lookup"><span data-stu-id="81a00-109">IoT functionality in Azure CLI **core** is focused on infrastructure management and configuration.</span></span> <span data-ttu-id="81a00-110">Операции CRUD в Центре Интернета вещей или настройка маршрутов сообщений Центра Интернета вещей — типичные варианты использования основных команд.</span><span class="sxs-lookup"><span data-stu-id="81a00-110">IoT Hub CRUD operations, or configuring IoT Hub message routes are typical use cases for core commands.</span></span>

<span data-ttu-id="81a00-111">**Расширение** Интернета вещей предоставляет широкие возможности и функции для управления данными, сущностями и объектами в самой инфраструктуре, а также для работы с ними.</span><span class="sxs-lookup"><span data-stu-id="81a00-111">The IoT **extension** introduces rich features and functionality to manage, manipulate and interact with the data, entities and objects on the infrastructure itself.</span></span> <span data-ttu-id="81a00-112">Например, управление парками устройств, отслеживание событий, передаваемых с устройства в облако и вызов методов облака для устройств, включены через расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="81a00-112">For example managing fleets of devices, monitoring device-to-cloud events and invoking cloud to device methods are all enabled via the IoT extension.</span></span> <span data-ttu-id="81a00-113">Расширение Интернета вещей Azure для Azure CLI позволяет использовать экспериментальные или предварительные технологии, обеспечивающие его универсальность в разных сценариях и вариантах использования.</span><span class="sxs-lookup"><span data-stu-id="81a00-113">The Azure IoT extension for Azure CLI unlocks the use of experimental or pre-release technology contributing to its versatility in a variety of scenarios and use cases.</span></span>

### <a name="core-reference-commands"></a><span data-ttu-id="81a00-114">Справочник по основным командам</span><span class="sxs-lookup"><span data-stu-id="81a00-114">Core reference commands</span></span>

| <span data-ttu-id="81a00-115">Справочник</span><span class="sxs-lookup"><span data-stu-id="81a00-115">Reference</span></span> | <span data-ttu-id="81a00-116">Используется в расширении</span><span class="sxs-lookup"><span data-stu-id="81a00-116">Has extension</span></span> | <span data-ttu-id="81a00-117">Описание</span><span class="sxs-lookup"><span data-stu-id="81a00-117">Description</span></span>
|-|-|-|
| [<span data-ttu-id="81a00-118">az iot</span><span class="sxs-lookup"><span data-stu-id="81a00-118">az iot</span></span>](/cli/azure/iot) | <span data-ttu-id="81a00-119">да</span><span class="sxs-lookup"><span data-stu-id="81a00-119">yes</span></span>  | <span data-ttu-id="81a00-120">Все доступные основные команды Azure CLI для Azure IoT.</span><span class="sxs-lookup"><span data-stu-id="81a00-120">All available Azure CLI core commands for Azure IoT.</span></span>
| [<span data-ttu-id="81a00-121">az iot central</span><span class="sxs-lookup"><span data-stu-id="81a00-121">az iot central</span></span>](/cli/azure/iot/central) | <span data-ttu-id="81a00-122">да</span><span class="sxs-lookup"><span data-stu-id="81a00-122">yes</span></span> | <span data-ttu-id="81a00-123">Управление ресурсами IoT Central.</span><span class="sxs-lookup"><span data-stu-id="81a00-123">Manage IoT Central assets.</span></span>
| [<span data-ttu-id="81a00-124">az iot dps</span><span class="sxs-lookup"><span data-stu-id="81a00-124">az iot dps</span></span>](/en-us/cli/azure/iot/dps) | <span data-ttu-id="81a00-125">да</span><span class="sxs-lookup"><span data-stu-id="81a00-125">yes</span></span> | <span data-ttu-id="81a00-126">Управление службой подготовки устройств к добавлению в Центр Интернета вещей Azure.</span><span class="sxs-lookup"><span data-stu-id="81a00-126">Manage Azure IoT Hub Device Provisioning Service.</span></span>
| [<span data-ttu-id="81a00-127">az iot hub</span><span class="sxs-lookup"><span data-stu-id="81a00-127">az iot hub</span></span>](/cli/azure/iot/hub) | <span data-ttu-id="81a00-128">да</span><span class="sxs-lookup"><span data-stu-id="81a00-128">yes</span></span> | <span data-ttu-id="81a00-129">Управление инфраструктурой Центра Интернета вещей Azure.</span><span class="sxs-lookup"><span data-stu-id="81a00-129">Manage Azure IoT Hub infrastructure.</span></span>

### <a name="extension-reference-commands"></a><span data-ttu-id="81a00-130">Справочник по командам расширения</span><span class="sxs-lookup"><span data-stu-id="81a00-130">Extension reference commands</span></span>

| <span data-ttu-id="81a00-131">Справочник</span><span class="sxs-lookup"><span data-stu-id="81a00-131">Reference</span></span> | <span data-ttu-id="81a00-132">Используется в основной версии</span><span class="sxs-lookup"><span data-stu-id="81a00-132">Has core</span></span> | <span data-ttu-id="81a00-133">Описание</span><span class="sxs-lookup"><span data-stu-id="81a00-133">Description</span></span>
|-|-|-|
| [<span data-ttu-id="81a00-134">az iot</span><span class="sxs-lookup"><span data-stu-id="81a00-134">az iot</span></span>](/cli/azure/ext/azure-iot/iot) | <span data-ttu-id="81a00-135">да</span><span class="sxs-lookup"><span data-stu-id="81a00-135">yes</span></span> | <span data-ttu-id="81a00-136">Все доступные команды расширения Azure CLI для Azure IoT.</span><span class="sxs-lookup"><span data-stu-id="81a00-136">All available Azure CLI extension commands for Azure IoT.</span></span>
| [<span data-ttu-id="81a00-137">az iot central</span><span class="sxs-lookup"><span data-stu-id="81a00-137">az iot central</span></span>](/cli/azure/ext/azure-iot/iot/central) | <span data-ttu-id="81a00-138">да</span><span class="sxs-lookup"><span data-stu-id="81a00-138">yes</span></span> | <span data-ttu-id="81a00-139">Управление решениями и инфраструктурой Azure Central (IoT Central).</span><span class="sxs-lookup"><span data-stu-id="81a00-139">Manage Azure Central (IoT Central) solutions & infrastructure.</span></span>
| [<span data-ttu-id="81a00-140">az iot device</span><span class="sxs-lookup"><span data-stu-id="81a00-140">az iot device</span></span>](/cli/azure/ext/azure-iot/iot/device) | | <span data-ttu-id="81a00-141">Использование возможностей двунаправленного обмена сообщениями между устройствами и облаком.</span><span class="sxs-lookup"><span data-stu-id="81a00-141">Leverage device-to-cloud and cloud-to-device messaging capabilities.</span></span>
| [<span data-ttu-id="81a00-142">az dt</span><span class="sxs-lookup"><span data-stu-id="81a00-142">az dt</span></span>](/cli/azure/ext/azure-iot/dt) | | <span data-ttu-id="81a00-143">Управление решениями и инфраструктурой Azure Digital Twins.</span><span class="sxs-lookup"><span data-stu-id="81a00-143">Manage Azure Digital Twins solutions & infrastructure.</span></span>
| [<span data-ttu-id="81a00-144">az iot dps</span><span class="sxs-lookup"><span data-stu-id="81a00-144">az iot dps</span></span>](/cli/azure/ext/azure-iot/iot/dps) | <span data-ttu-id="81a00-145">да</span><span class="sxs-lookup"><span data-stu-id="81a00-145">yes</span></span> | <span data-ttu-id="81a00-146">Управление сущностями в службе подготовки устройств к добавлению в Центр Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="81a00-146">Manage entities in an Azure IoT Hub Device Provisioning Service.</span></span>
| [<span data-ttu-id="81a00-147">az iot edge</span><span class="sxs-lookup"><span data-stu-id="81a00-147">az iot edge</span></span>](/cli/azure/ext/azure-iot/iot/edge) | | <span data-ttu-id="81a00-148">Управление решениями Интернета вещей в пограничной среде.</span><span class="sxs-lookup"><span data-stu-id="81a00-148">Manage IoT solutions on the Edge.</span></span>
| [<span data-ttu-id="81a00-149">az iot hub</span><span class="sxs-lookup"><span data-stu-id="81a00-149">az iot hub</span></span>](/cli/azure/ext/azure-iot/iot/hub) | <span data-ttu-id="81a00-150">да</span><span class="sxs-lookup"><span data-stu-id="81a00-150">yes</span></span> | <span data-ttu-id="81a00-151">Управление сущностями в Центре Интернета вещей Azure.</span><span class="sxs-lookup"><span data-stu-id="81a00-151">Manage entities in an Azure IoT Hub.</span></span>
| [<span data-ttu-id="81a00-152">az iot pnp</span><span class="sxs-lookup"><span data-stu-id="81a00-152">az iot pnp</span></span>](/cli/azure/ext/azure-iot/iot/pnp) | <span data-ttu-id="81a00-153">да</span><span class="sxs-lookup"><span data-stu-id="81a00-153">yes</span></span> | <span data-ttu-id="81a00-154">Управление сущностями в репозитории моделей IoT Plug and Play.</span><span class="sxs-lookup"><span data-stu-id="81a00-154">Manage entities of an IoT Plug and Play model repository.</span></span>

### <a name="additional-cli-commands-for-azure-services-used-by-iot"></a><span data-ttu-id="81a00-155">Дополнительные команды CLI для служб Azure, используемых в Интернете вещей</span><span class="sxs-lookup"><span data-stu-id="81a00-155">Additional CLI commands for Azure services used by IoT</span></span>

| <span data-ttu-id="81a00-156">Справочник</span><span class="sxs-lookup"><span data-stu-id="81a00-156">Reference</span></span> | <span data-ttu-id="81a00-157">Тип</span><span class="sxs-lookup"><span data-stu-id="81a00-157">Type</span></span> | <span data-ttu-id="81a00-158">Описание</span><span class="sxs-lookup"><span data-stu-id="81a00-158">Description</span></span>
|-|-|-|
| [<span data-ttu-id="81a00-159">az maps</span><span class="sxs-lookup"><span data-stu-id="81a00-159">az maps</span></span>](/cli/azure/maps) | <span data-ttu-id="81a00-160">core</span><span class="sxs-lookup"><span data-stu-id="81a00-160">core</span></span> | <span data-ttu-id="81a00-161">Управление Azure Maps.</span><span class="sxs-lookup"><span data-stu-id="81a00-161">Manage Azure Maps.</span></span>
| [<span data-ttu-id="81a00-162">az timeseriesinsights</span><span class="sxs-lookup"><span data-stu-id="81a00-162">az timeseriesinsights</span></span>](/cli/azure/ext/timeseriesinsights/timeseriesinsights) | <span data-ttu-id="81a00-163">Расширение</span><span class="sxs-lookup"><span data-stu-id="81a00-163">extension</span></span> | <span data-ttu-id="81a00-164">Управление Аналитикой временных рядов Azure.</span><span class="sxs-lookup"><span data-stu-id="81a00-164">Manage Azure Time Series Insights.</span></span>

### <a name="extension-reference-installation"></a><span data-ttu-id="81a00-165">Установка расширений из справочника</span><span class="sxs-lookup"><span data-stu-id="81a00-165">Extension reference installation</span></span>

<span data-ttu-id="81a00-166">Перед использованием необходимо установить расширения Azure CLI из справочника.</span><span class="sxs-lookup"><span data-stu-id="81a00-166">Azure CLI extension references must be installed prior to use.</span></span>  <span data-ttu-id="81a00-167">Чтобы установить расширение из справочника по имени, используйте команду [az extension add](/cli/azure/azure-cli-extensions-overview).</span><span class="sxs-lookup"><span data-stu-id="81a00-167">Use the [az extension add](/cli/azure/azure-cli-extensions-overview) command to install an extension reference by name.</span></span>  <span data-ttu-id="81a00-168">Узнайте больше о расширениях из статьи [Использование расширений с Azure CLI](/cli/azure/azure-cli-extensions-overview).</span><span class="sxs-lookup"><span data-stu-id="81a00-168">Find out more about extension references in [Use extensions with Azure CLI](/cli/azure/azure-cli-extensions-overview).</span></span>

```azurecli
# install the Azure CLI extension reference for Azure IoT
az extension add --name azure-iot
```

## <a name="popular-iot-articles-using-the-azure-cli"></a><span data-ttu-id="81a00-169">Популярные статьи, посвященные Интернету вещей, в которых описывается Azure CLI</span><span class="sxs-lookup"><span data-stu-id="81a00-169">Popular IoT articles using the Azure CLI</span></span>

- [<span data-ttu-id="81a00-170">Создание Центра Интернета вещей</span><span class="sxs-lookup"><span data-stu-id="81a00-170">Create an IoT hub</span></span>](/azure/iot-hub/iot-hub-create-using-cli)
- [<span data-ttu-id="81a00-171">Управление IoT Central</span><span class="sxs-lookup"><span data-stu-id="81a00-171">Manage IoT Central</span></span>](/azure/iot-central/core/howto-manage-iot-central-from-cli)
- [<span data-ttu-id="81a00-172">Руководства по устройствам, управляемым CLI с помощью ОСРВ Azure</span><span class="sxs-lookup"><span data-stu-id="81a00-172">CLI driven device tutorials using Azure RTOS</span></span>](/azure/rtos/getting-started?branch=master)
- [<span data-ttu-id="81a00-173">Использование расширения Интернета вещей для управления устройствами в Центре Интернета вещей Azure</span><span class="sxs-lookup"><span data-stu-id="81a00-173">Use the IoT extension for Azure IoT Hub device management</span></span>](/azure/iot-hub/iot-hub-device-management-iot-extension-azure-cli-2-0)
- [<span data-ttu-id="81a00-174">Развертывание и мониторинг модулей IoT Edge в большом масштабе с помощью расширения Azure CLI для Интернета вещей</span><span class="sxs-lookup"><span data-stu-id="81a00-174">Deploy and monitor IoT Edge modules at scale with the Azure CLI extension for IoT</span></span>](/azure/iot-edge/how-to-deploy-cli-at-scale)
- [<span data-ttu-id="81a00-175">Отправка данных телеметрии на устройство и их отслеживание с помощью расширения Azure CLI для Интернета вещей</span><span class="sxs-lookup"><span data-stu-id="81a00-175">Send Telemetry to a device and monitor it with the Azure CLI extension for IoT</span></span>](/azure/iot-hub/quickstart-send-telemetry-cli)
- [<span data-ttu-id="81a00-176">Маршрутизация сообщений Центра Интернета вещей с помощью Azure CLI</span><span class="sxs-lookup"><span data-stu-id="81a00-176">Use the Azure CLI to configure IoT Hub message routing</span></span>](/azure/iot-hub/tutorial-routing-config-message-routing-cli)
- [<span data-ttu-id="81a00-177">Управление интерфейсами в репозитории моделей Plug and Play</span><span class="sxs-lookup"><span data-stu-id="81a00-177">Manage interfaces in a Plug and Play model repository</span></span>](/azure/iot-pnp/howto-install-pnp-cli#manage-interfaces-in-a-model-repository)

## <a name="azure-cli-reference-examples"></a><span data-ttu-id="81a00-178">Справочник по примерам использования Azure CLI</span><span class="sxs-lookup"><span data-stu-id="81a00-178">Azure CLI reference examples</span></span>

<span data-ttu-id="81a00-179">Примеры приведены для каждого справочника по Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="81a00-179">Examples are provided with every Azure CLI reference.</span></span> <span data-ttu-id="81a00-180">Хотя эти задачи также можно выполнить с помощью портала Azure, при использовании Azure CLI требуется одна командная строка.</span><span class="sxs-lookup"><span data-stu-id="81a00-180">Although you can also complete these tasks through the Azure portal, using the Azure CLI requires a single command line.</span></span>  <span data-ttu-id="81a00-181">Ниже представлено несколько блоков кода, которые помогут вам понять, насколько просто использовать Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="81a00-181">Here are a few code blocks to give you an idea of how easy it is to use the Azure CLI.</span></span>

<span data-ttu-id="81a00-182">Для работы с Azure IoT вам потребуется группа ресурсов.</span><span class="sxs-lookup"><span data-stu-id="81a00-182">To work with Azure IoT, you'll first need a resource group.</span></span>  <span data-ttu-id="81a00-183">Группы ресурсов Azure можно без усилий создавать и администрировать с помощью Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="81a00-183">Azure resource groups are simple to create and manage with the Azure CLI.</span></span>  

```azurecli
#create a resource group
az group create -location westus -name MyResourceGroup
```

```azurecli
#get a list of resource groups for a subscription
az group list --subscription MySubscription --output table
```

<span data-ttu-id="81a00-184">Вы можете без усилий создать Центр Интернета вещей Azure в регионе westus в ценовой категории "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="81a00-184">It is as straightforward to create an Azure IoT Hub in the '''westus''' region in the standard pricing tier.</span></span>

```azurecli
#create an Azure IoT hub
az iot hub create --resource-group MyResourceGroup --name MyIotHub --location westus
```

## <a name="see-also"></a><span data-ttu-id="81a00-185">См. также раздел</span><span class="sxs-lookup"><span data-stu-id="81a00-185">See also</span></span>

- <span data-ttu-id="81a00-186">[Начните работу с Azure CLI](/cli/azure/get-started-with-azure-cli), чтобы узнать об установке и входе.</span><span class="sxs-lookup"><span data-stu-id="81a00-186">[Get started with Azure CLI](/cli/azure/get-started-with-azure-cli) to learn about installation and sign in.</span></span>

- <span data-ttu-id="81a00-187">Найдите дополнительные справочники по [выпущенным командам](/cli/azure/reference-index) и [командам расширения](/cli/azure/azure-cli-extensions-list) в документации по Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="81a00-187">Discover additional [released](/cli/azure/reference-index) and [extension](/cli/azure/azure-cli-extensions-list) references in the Azure CLI documentation.</span></span>
