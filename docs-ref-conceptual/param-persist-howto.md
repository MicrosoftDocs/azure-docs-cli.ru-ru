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
ms.openlocfilehash: 087f5f05d6a4a6b25e6aebd0d2c482ebba656b01
ms.sourcegitcommit: 9beaf9abb794f1006a56acee4e1cfb8ea7fe2405
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2020
ms.locfileid: "96850224"
---
# <a name="azure-cli-persisted-parameter"></a><span data-ttu-id="640ca-103">Хранимые параметры Azure CLI</span><span class="sxs-lookup"><span data-stu-id="640ca-103">Azure CLI persisted parameter</span></span>

<span data-ttu-id="640ca-104">Ссылочная команда Azure CLI [az config param-persist](/cli/azure/param-persist) предоставляет возможность сохранять локальные значения хранимых параметров для команд Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="640ca-104">The Azure CLI [az config param-persist](/cli/azure/param-persist) reference provides the ability to retain local persisted parameter values for Azure CLI commands.</span></span>  <span data-ttu-id="640ca-105">Таким образом устраняется необходимость в постоянном повторном вводе общих параметров.</span><span class="sxs-lookup"><span data-stu-id="640ca-105">This removes the need to continually retype common parameters.</span></span> <span data-ttu-id="640ca-106">Например, location и resource-group являются обязательными параметрами во многих командах CLI, но они не влияют на _намерение_ команды.</span><span class="sxs-lookup"><span data-stu-id="640ca-106">For example, location and resource-group are required parameters in many CLI commands, but they don't contribute to the _intent_ of the command.</span></span>  <span data-ttu-id="640ca-107">При сохранении значения параметров с помощью функции хранимых параметров, вы уменьшаете избыточность и можете значительно сократить синтаксис команд CLI.</span><span class="sxs-lookup"><span data-stu-id="640ca-107">When you store parameter values with persisted parameter, you reduce redundancy and can significantly shorten CLI command syntax.</span></span>

<span data-ttu-id="640ca-108">Значения конфигурации, используемые CLI, вычисляются в указанном ниже порядке. Элементы, расположенные выше в списке, имеют больший приоритет.</span><span class="sxs-lookup"><span data-stu-id="640ca-108">Configuration values used by the CLI are evaluated in the following precedence, with items higher on the list taking priority.</span></span>

1. <span data-ttu-id="640ca-109">Параметры командной строки</span><span class="sxs-lookup"><span data-stu-id="640ca-109">Command-line parameters</span></span>
1. <span data-ttu-id="640ca-110">Значения в локальной рабочей папке, заданные с помощью команды **az config param-persist**</span><span class="sxs-lookup"><span data-stu-id="640ca-110">Values in the local working directory set by **az config param-persist**</span></span>
1. <span data-ttu-id="640ca-111">Переменные среды</span><span class="sxs-lookup"><span data-stu-id="640ca-111">Environment variables</span></span>
1. <span data-ttu-id="640ca-112">Значения в файле конфигурации или заданные с помощью команды **az config**</span><span class="sxs-lookup"><span data-stu-id="640ca-112">Values in the configuration file or set with **az config**</span></span>

<span data-ttu-id="640ca-113">[Установите Azure CLI](install-azure-cli.md) или откройте [Azure Cloud Shell](https://shell.azure.com), чтобы запустить скрипты, указанные в этой статье.</span><span class="sxs-lookup"><span data-stu-id="640ca-113">[Install the Azure CLI](install-azure-cli.md) or open [Azure Cloud Shell](https://shell.azure.com) to run the scripts in this article.</span></span>  <span data-ttu-id="640ca-114">При использовании локальной установки Azure CLI для выполнения команд **az config param-persist** требуется версия 2.12.0 или более поздняя.</span><span class="sxs-lookup"><span data-stu-id="640ca-114">If you are using a local install of the Azure CLI, version 2.12.0 or later is needed to run **az config param-persist** commands.</span></span>  <span data-ttu-id="640ca-115">Выполните команду [az version](/cli/azure/reference-index#az_version), чтобы узнать установленную версию и зависимые библиотеки.</span><span class="sxs-lookup"><span data-stu-id="640ca-115">Run [az version](/cli/azure/reference-index#az_version) to find the version and dependent libraries that are installed.</span></span> <span data-ttu-id="640ca-116">Чтобы обновиться до последней версии, выполните команду [az upgrade](/cli/azure/reference-index#az_upgrade).</span><span class="sxs-lookup"><span data-stu-id="640ca-116">To upgrade to the latest version, run [az upgrade](/cli/azure/reference-index#az_upgrade).</span></span>  <span data-ttu-id="640ca-117">В Azure Cloud Shell всегда установлена последняя версия Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="640ca-117">Azure Cloud Shell always has the latest version of the Azure CLI.</span></span>

## <a name="persisted-parameter-data-file"></a><span data-ttu-id="640ca-118">Файл данных хранимого параметра</span><span class="sxs-lookup"><span data-stu-id="640ca-118">Persisted parameter data file</span></span>

<span data-ttu-id="640ca-119">Значения хранимых параметров хранятся в файле с именем **.param_persist**, который находится в вашей рабочей папке.</span><span class="sxs-lookup"><span data-stu-id="640ca-119">Persisted parameter values are kept in a file named **.param_persist** which is stored in your working directory.</span></span>  <span data-ttu-id="640ca-120">При использовании [Azure Cloud Shell](https://shell.azure.com) для выполнения команд Azure CLI рабочая папка будет находиться в учетной записи хранения, используемой Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="640ca-120">If you are using [Azure Cloud Shell](https://shell.azure.com) to execute Azure CLI commands, your working directory is in the storage account being used by the Azure CLI.</span></span>  <span data-ttu-id="640ca-121">При использовании [локальной установки](/install-azure-cli) Azure CLI рабочая папка будет находиться на локальном компьютере.</span><span class="sxs-lookup"><span data-stu-id="640ca-121">If you are using a [local install](/install-azure-cli) of the Azure CLI, your working directory is on your local machine.</span></span>  <span data-ttu-id="640ca-122">В любом из этих расположений файл **.param_persist** будет скрыт. Его не нужно обновлять вручную.</span><span class="sxs-lookup"><span data-stu-id="640ca-122">In either location, the **.param_persist** file is hidden and should not be manually updated.</span></span>

## <a name="persisted-parameter-storage-and-support"></a><span data-ttu-id="640ca-123">Сохранение и поддержка хранимых параметров</span><span class="sxs-lookup"><span data-stu-id="640ca-123">Persisted parameter storage and support</span></span>

<span data-ttu-id="640ca-124">Функция хранимых параметров поддерживается для указанных ниже параметров Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="640ca-124">The following Azure CLI parameters are supported by persisted parameter.</span></span>  <span data-ttu-id="640ca-125">Параметры **resource_group_name** и **location** сохраняются иначе. Вы можете добавить их в хранимый параметр _без_ выполнения команды создания.</span><span class="sxs-lookup"><span data-stu-id="640ca-125">The **resource_group_name** and **location** parameters are stored differently in that you can add them to persisted parameter _without_ executing a create command.</span></span>

| <span data-ttu-id="640ca-126">Хранимый параметр</span><span class="sxs-lookup"><span data-stu-id="640ca-126">Persisted parameter</span></span> | <span data-ttu-id="640ca-127">Действие сохранения</span><span class="sxs-lookup"><span data-stu-id="640ca-127">Storage action</span></span> | <span data-ttu-id="640ca-128">Поддерживаются</span><span class="sxs-lookup"><span data-stu-id="640ca-128">Supported by</span></span>
|-|-|-|
| <span data-ttu-id="640ca-129">location</span><span class="sxs-lookup"><span data-stu-id="640ca-129">location</span></span> | <span data-ttu-id="640ca-130">Выполнение любой команды</span><span class="sxs-lookup"><span data-stu-id="640ca-130">Execute any command</span></span> | <span data-ttu-id="640ca-131">Все справочники по Azure CLI</span><span class="sxs-lookup"><span data-stu-id="640ca-131">All Azure CLI references</span></span>
| <span data-ttu-id="640ca-132">resource_group_name</span><span class="sxs-lookup"><span data-stu-id="640ca-132">resource_group_name</span></span> | <span data-ttu-id="640ca-133">Выполнение любой команды</span><span class="sxs-lookup"><span data-stu-id="640ca-133">Execute any command</span></span> | <span data-ttu-id="640ca-134">Все справочники по Azure CLI</span><span class="sxs-lookup"><span data-stu-id="640ca-134">All Azure CLI references</span></span>
| <span data-ttu-id="640ca-135">vnet_name</span><span class="sxs-lookup"><span data-stu-id="640ca-135">vnet_name</span></span> | <span data-ttu-id="640ca-136">Выполнение команды создания</span><span class="sxs-lookup"><span data-stu-id="640ca-136">Execute a create command</span></span> | <span data-ttu-id="640ca-137">Только веб-приложения Azure</span><span class="sxs-lookup"><span data-stu-id="640ca-137">Azure Web Apps only</span></span>
| <span data-ttu-id="640ca-138">storage_account_name</span><span class="sxs-lookup"><span data-stu-id="640ca-138">storage_account_name</span></span> | <span data-ttu-id="640ca-139">Выполнение команды создания</span><span class="sxs-lookup"><span data-stu-id="640ca-139">Execute a create command</span></span> |  <span data-ttu-id="640ca-140">Только веб-приложения Azure</span><span class="sxs-lookup"><span data-stu-id="640ca-140">Azure Web Apps only</span></span>
| <span data-ttu-id="640ca-141">webapp_name</span><span class="sxs-lookup"><span data-stu-id="640ca-141">webapp_name</span></span> | <span data-ttu-id="640ca-142">Выполнение команды создания</span><span class="sxs-lookup"><span data-stu-id="640ca-142">Execute a create command</span></span> | <span data-ttu-id="640ca-143">Только веб-приложения Azure</span><span class="sxs-lookup"><span data-stu-id="640ca-143">Azure Web Apps only</span></span>
| <span data-ttu-id="640ca-144">function_app_name</span><span class="sxs-lookup"><span data-stu-id="640ca-144">function_app_name</span></span> | <span data-ttu-id="640ca-145">Выполнение команды создания</span><span class="sxs-lookup"><span data-stu-id="640ca-145">Execute a create command</span></span> | <span data-ttu-id="640ca-146">Только Функции Azure</span><span class="sxs-lookup"><span data-stu-id="640ca-146">Azure Functions only</span></span>

## <a name="sample-script-using-persisted-parameters"></a><span data-ttu-id="640ca-147">Пример скрипта с использованием хранимых параметров</span><span class="sxs-lookup"><span data-stu-id="640ca-147">Sample script using persisted parameters</span></span>

<span data-ttu-id="640ca-148">Без хранимых параметров для последовательного выполнения команд CLI необходимо указывать одни и те же значения параметров.</span><span class="sxs-lookup"><span data-stu-id="640ca-148">Without persisted parameters, sequential CLI commands must repeat the same parameter values.</span></span>  <span data-ttu-id="640ca-149">Если хранимые параметры включены, сохраненные значения параметров можно опустить в последовательном выполнении команд.</span><span class="sxs-lookup"><span data-stu-id="640ca-149">With persisted parameters enabled, your stored parameter values can be omitted from sequential commands.</span></span>  <span data-ttu-id="640ca-150">В этом примере значения параметров **location**, **resource group name** или **storage account name** повторяются в последующих командах.</span><span class="sxs-lookup"><span data-stu-id="640ca-150">In this example, the **location**, **resource group name** or **storage account name** are repeated in subsequent commands.</span></span>

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

## <a name="persisted-parameter-and-global-variable-comparison"></a><span data-ttu-id="640ca-151">Сравнение хранимых параметров и глобальных переменных</span><span class="sxs-lookup"><span data-stu-id="640ca-151">Persisted parameter and global variable comparison</span></span>

<span data-ttu-id="640ca-152">Для значений параметров по умолчанию можно использовать две команды Azure CLI: **az configure** и **az config param-persist**.</span><span class="sxs-lookup"><span data-stu-id="640ca-152">There are two Azure CLI commands that can be used to default parameter values: **az configure** and **az config param-persist**.</span></span>  <span data-ttu-id="640ca-153">С помощью команды **az configure** можно указать _глобальные переменные_, например group, location или web.</span><span class="sxs-lookup"><span data-stu-id="640ca-153">Use the **az configure** command to specify _global variables_ such as group, location, or web.</span></span>  <span data-ttu-id="640ca-154">С помощью команды **az param-persist** можно указать _локальные значения по умолчанию_, уникальные для вашей рабочей нагрузки.</span><span class="sxs-lookup"><span data-stu-id="640ca-154">Use **az param-persist** to specify _local default values_ unique to your workload.</span></span>  <span data-ttu-id="640ca-155">Сохраненные значения используются CLI вместо обязательных аргументов.</span><span class="sxs-lookup"><span data-stu-id="640ca-155">Stored values are used by the CLI in place of required arguments.</span></span>

> [!Important]
> <span data-ttu-id="640ca-156">Хранимые параметры переопределяют глобальные значения контекста.</span><span class="sxs-lookup"><span data-stu-id="640ca-156">Persisted parameters override global context values.</span></span>
>

| <span data-ttu-id="640ca-157">Справочные сведения</span><span class="sxs-lookup"><span data-stu-id="640ca-157">Reference</span></span> | <span data-ttu-id="640ca-158">Область</span><span class="sxs-lookup"><span data-stu-id="640ca-158">Scope</span></span> | <span data-ttu-id="640ca-159">Присвойте параметру</span><span class="sxs-lookup"><span data-stu-id="640ca-159">Set</span></span> | <span data-ttu-id="640ca-160">Использовать</span><span class="sxs-lookup"><span data-stu-id="640ca-160">Use</span></span>
|-|-|-|-|
[<span data-ttu-id="640ca-161">az configure</span><span class="sxs-lookup"><span data-stu-id="640ca-161">az configure</span></span>](/cli/azure/reference-index#az_configure) | <span data-ttu-id="640ca-162">Глобальный охват через CLI</span><span class="sxs-lookup"><span data-stu-id="640ca-162">Scoped globally across the CLI</span></span> | <span data-ttu-id="640ca-163">Устанавливается явным образом с помощью команды **az configure --defaults**</span><span class="sxs-lookup"><span data-stu-id="640ca-163">Set explicitly using **az configure --defaults**</span></span> | <span data-ttu-id="640ca-164">Используется для таких параметров, как ведение журнала, сбор данных и значения аргументов по умолчанию</span><span class="sxs-lookup"><span data-stu-id="640ca-164">Use for settings such as logging, data collection, and default argument values</span></span>
[<span data-ttu-id="640ca-165">az config param-persist</span><span class="sxs-lookup"><span data-stu-id="640ca-165">az config param-persist</span></span>](/cli/azure/config/param-persist) | <span data-ttu-id="640ca-166">Локальный охват в конкретной рабочей папке</span><span class="sxs-lookup"><span data-stu-id="640ca-166">Scoped locally to a specific working directory</span></span> | <span data-ttu-id="640ca-167">Устанавливается автоматически после включения хранимых параметров</span><span class="sxs-lookup"><span data-stu-id="640ca-167">Set automatically once persisted parameters are turned on</span></span> | <span data-ttu-id="640ca-168">Используется для последовательного выполнения команд отдельных рабочих нагрузок.</span><span class="sxs-lookup"><span data-stu-id="640ca-168">Use for individual workload sequential commands.</span></span>

### <a name="command-examples"></a><span data-ttu-id="640ca-169">Примеры команд</span><span class="sxs-lookup"><span data-stu-id="640ca-169">Command examples</span></span>

<span data-ttu-id="640ca-170">С помощью **az config param-persist** можно задать глобальную переменную, используемую при создании учетной записи хранения Azure.</span><span class="sxs-lookup"><span data-stu-id="640ca-170">Use **az config param-persist** to set a global variable used in the creation of an Azure storage account.</span></span>

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

<span data-ttu-id="640ca-171">В выходных данных команды CLI указано, что новая учетная запись хранения была создана в группе ресурсов, обнаруженной в глобальной переменной myGlobalVariableRG.</span><span class="sxs-lookup"><span data-stu-id="640ca-171">CLI command output shows that a new storage account was created in the resource group found in the global variable, \`myGlobalVariableRG'.</span></span>

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

<span data-ttu-id="640ca-172">С помощью команды **az config param-persist** можно задать хранимые параметры, используемые при создании учетной записи хранения Azure.</span><span class="sxs-lookup"><span data-stu-id="640ca-172">Use **az config param-persist** to set persisted parameters used in the creation of an Azure storage account.</span></span>  <span data-ttu-id="640ca-173">Если для того же объекта задана глобальная переменная, хранимый параметр переопределит ее.</span><span class="sxs-lookup"><span data-stu-id="640ca-173">If a global variable is set for the same object, the persisted parameter will override the global variable.</span></span>

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

<span data-ttu-id="640ca-174">Даже с глобальной переменной, заданной для группы ресурсов со значением `myGlobalVariableRG`, и с включенными хранимыми параметрами новая учетная запись хранения была создана с помощью `myParamPersistRG`.</span><span class="sxs-lookup"><span data-stu-id="640ca-174">Even with a global variable set for resource group with a value of `myGlobalVariableRG`, with persisted parameters turned on, the new storage account was created with `myParamPersistRG`.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="640ca-175">См. также раздел</span><span class="sxs-lookup"><span data-stu-id="640ca-175">See also</span></span>

* [<span data-ttu-id="640ca-176">Учебник. Использование хранимых параметров для последовательного выполнения команд Azure CLI</span><span class="sxs-lookup"><span data-stu-id="640ca-176">Tutorial: Use persisted parameter with sequential Azure CLI commands</span></span>](param-persist-tutorial.md)
* [<span data-ttu-id="640ca-177">Настройка Azure CLI с помощью команды az configure</span><span class="sxs-lookup"><span data-stu-id="640ca-177">Azure CLI Configuration using az configure</span></span>](azure-cli-configuration.md)

