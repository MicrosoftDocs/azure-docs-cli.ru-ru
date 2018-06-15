---
title: Заметки о выпуске Azure CLI 2.0
description: Узнайте о последних обновлениях в Azure CLI 2.0
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 06/01/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 72e667d74ff8d55f26ecbf3b3c8845c9c03b56be
ms.sourcegitcommit: 5c80e96e96f9608c92a94fa4a9c4afb25099f3fc
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/13/2018
ms.locfileid: "35512909"
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="ca5c1-103">Заметки о выпуске Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="ca5c1-103">Azure CLI 2.0 release notes</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="ca5c1-104">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-104">June 13, 2018</span></span>

<span data-ttu-id="ca5c1-105">Версия 2.0.36</span><span class="sxs-lookup"><span data-stu-id="ca5c1-105">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="ca5c1-106">AKS</span><span class="sxs-lookup"><span data-stu-id="ca5c1-106">AKS</span></span>

* <span data-ttu-id="ca5c1-107">В `aks create` добавлены дополнительные сетевые параметры.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-107">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="ca5c1-108">В `aks create` добавлены аргументы для наблюдения и маршрутизации HTTP-трафика.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-108">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span> 
* <span data-ttu-id="ca5c1-109">Добавлен аргумент `--no-ssh-key` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="ca5c1-109">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="ca5c1-110">Добавлен аргумент `--enable-rbac` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="ca5c1-110">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="ca5c1-111">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] В `aks create` добавлена поддержка аутентификации Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-111">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="ca5c1-112">AppService</span><span class="sxs-lookup"><span data-stu-id="ca5c1-112">AppService</span></span>

* <span data-ttu-id="ca5c1-113">Устранена проблема с несовместимыми версиями urllib.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-113">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="ca5c1-114">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-114">June 5, 2018</span></span>

<span data-ttu-id="ca5c1-115">Версия 2.0.35</span><span class="sxs-lookup"><span data-stu-id="ca5c1-115">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="ca5c1-116">Interactive</span><span class="sxs-lookup"><span data-stu-id="ca5c1-116">Interactive</span></span>

* <span data-ttu-id="ca5c1-117">Добавлены ограничения в зависимости интерактивного режима.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-117">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="ca5c1-118">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-118">June 5, 2018</span></span>

<span data-ttu-id="ca5c1-119">Версия 2.0.34</span><span class="sxs-lookup"><span data-stu-id="ca5c1-119">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="ca5c1-120">Core</span><span class="sxs-lookup"><span data-stu-id="ca5c1-120">Core</span></span>

* <span data-ttu-id="ca5c1-121">Добавлена поддержка перекрестных ссылок на ресурсы клиента.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-121">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="ca5c1-122">Улучшена надежность при передаче данных телеметрии.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-122">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="ca5c1-123">ACR</span><span class="sxs-lookup"><span data-stu-id="ca5c1-123">ACR</span></span>

* <span data-ttu-id="ca5c1-124">Добавлена поддержка VSTS в качестве расположения удаленного источника.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-124">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="ca5c1-125">Добавлена команда `acr import`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-125">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="ca5c1-126">AKS</span><span class="sxs-lookup"><span data-stu-id="ca5c1-126">AKS</span></span>

* <span data-ttu-id="ca5c1-127">Изменена команда `aks get-credentials` для создания файла конфигурации kube с более надежными разрешениями файловой системы.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-127">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="ca5c1-128">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="ca5c1-128">Batch</span></span>

* <span data-ttu-id="ca5c1-129">Исправлена ошибка, связанная с форматированием таблиц при выполнении команды pool list. [[Ошибка #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="ca5c1-129">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="ca5c1-130">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="ca5c1-130">IOT</span></span>

* <span data-ttu-id="ca5c1-131">Добавлена возможность создания Центров Интернета вещей категории "Базовый".</span><span class="sxs-lookup"><span data-stu-id="ca5c1-131">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="ca5c1-132">Сеть</span><span class="sxs-lookup"><span data-stu-id="ca5c1-132">Network</span></span>

* <span data-ttu-id="ca5c1-133">Улучшена команда `network vnet peering`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-133">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="ca5c1-134">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="ca5c1-134">Policy Insights</span></span>

* <span data-ttu-id="ca5c1-135">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="ca5c1-135">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="ca5c1-136">ARM</span><span class="sxs-lookup"><span data-stu-id="ca5c1-136">ARM</span></span>

* <span data-ttu-id="ca5c1-137">Добавлены команды `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-137">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="ca5c1-138">SQL</span><span class="sxs-lookup"><span data-stu-id="ca5c1-138">SQL</span></span>

* <span data-ttu-id="ca5c1-139">Добавлены новые команды для управляемого экземпляра:</span><span class="sxs-lookup"><span data-stu-id="ca5c1-139">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="ca5c1-140">Добавлены новые команды для управляемой базы данных:</span><span class="sxs-lookup"><span data-stu-id="ca5c1-140">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="ca5c1-141">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="ca5c1-141">Storage</span></span>

* <span data-ttu-id="ca5c1-142">Добавлены типы MIME для JSON и JavaScript, выводимые из расширений файлов.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-142">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="ca5c1-143">ВМ</span><span class="sxs-lookup"><span data-stu-id="ca5c1-143">VM</span></span>

* <span data-ttu-id="ca5c1-144">Изменена команда `vm list-skus` для использования фиксированных столбцов, а также добавлено предупреждение об удалении `Tier` и `Size`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-144">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="ca5c1-145">Добавлен параметр `--accelerated-networking` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-145">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="ca5c1-146">Добавлен параметр `--tags` для команды `identity create`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-146">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="ca5c1-147">22 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-147">May 22, 2018</span></span>

<span data-ttu-id="ca5c1-148">Версия 2.0.33</span><span class="sxs-lookup"><span data-stu-id="ca5c1-148">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="ca5c1-149">Core</span><span class="sxs-lookup"><span data-stu-id="ca5c1-149">Core</span></span>

* <span data-ttu-id="ca5c1-150">Добавлена возможность включения символа `@` в имена файлов.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-150">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="ca5c1-151">ACS</span><span class="sxs-lookup"><span data-stu-id="ca5c1-151">ACS</span></span>

* <span data-ttu-id="ca5c1-152">Добавлены новые команды для Dev Spaces: `aks use-dev-spaces` и `aks remove-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-152">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="ca5c1-153">Исправлена опечатка в справочном сообщении.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-153">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="ca5c1-154">AppService</span><span class="sxs-lookup"><span data-stu-id="ca5c1-154">AppService</span></span>

* <span data-ttu-id="ca5c1-155">Улучшены команды общего обновления.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-155">Improved generic update commands</span></span>
* <span data-ttu-id="ca5c1-156">Добавлена поддержка асинхронного выполнения для `webapp deployment source config-zip`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-156">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="ca5c1-157">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ca5c1-157">Container</span></span>

* <span data-ttu-id="ca5c1-158">Добавлена возможность экспорта группы контейнеров в формате YAML.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-158">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="ca5c1-159">Добавлена возможность использования файла YAML для создания или обновления группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-159">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="ca5c1-160">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="ca5c1-160">Extension</span></span>

* <span data-ttu-id="ca5c1-161">Улучшена операция удаления расширений.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-161">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="ca5c1-162">Interactive</span><span class="sxs-lookup"><span data-stu-id="ca5c1-162">Interactive</span></span>

* <span data-ttu-id="ca5c1-163">Изменены параметры ведения журнала для отключения средства синтаксического анализа для завершенных операций.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-163">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="ca5c1-164">Улучшена обработка поврежденных кэшей справки.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-164">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="ca5c1-165">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="ca5c1-165">KeyVault</span></span>

* <span data-ttu-id="ca5c1-166">Исправлены команды хранилища ключей для работы с удостоверениями в Cloud Shell или виртуальных машинах.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-166">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="ca5c1-167">Сеть</span><span class="sxs-lookup"><span data-stu-id="ca5c1-167">Network</span></span>

* <span data-ttu-id="ca5c1-168">Исправлена проблема, при которой `network watcher show-topology` не будет выполняться, если виртуальной сети или подсети присвоить имя. [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="ca5c1-168">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="ca5c1-169">Исправлена проблема, при которой некоторые команды `network watcher` выдают ошибку, что Наблюдатель за сетями не включен в определенных регионах. [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="ca5c1-169">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="ca5c1-170">SQL</span><span class="sxs-lookup"><span data-stu-id="ca5c1-170">SQL</span></span>

* <span data-ttu-id="ca5c1-171">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены объекты ответа, возвращаемые в результатах команд `db` и `dw`:</span><span class="sxs-lookup"><span data-stu-id="ca5c1-171">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="ca5c1-172">Свойство `serviceLevelObjective` переименовано на `currentServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-172">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="ca5c1-173">Удалены свойства `currentServiceObjectiveId` и `requestedServiceObjectiveId`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-173">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span> 
    * <span data-ttu-id="ca5c1-174">Тип свойства `maxSizeBytes` изменен со строкового на целое число.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-174">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="ca5c1-175">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `db` и `dw` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="ca5c1-175">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="ca5c1-176">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-176">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="ca5c1-177">Для обновления используйте параметр `--service-objective` или задайте свойство `sku.name`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-177">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="ca5c1-178">`edition`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-178">`edition`.</span></span> <span data-ttu-id="ca5c1-179">Для обновления используйте параметр `--edition` или задайте свойство `sku.tier`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-179">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="ca5c1-180">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-180">`elasticPoolName`.</span></span> <span data-ttu-id="ca5c1-181">Для обновления используйте параметр `--elastic-pool` или задайте свойство `elasticPoolId`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-181">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="ca5c1-182">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `elastic-pool` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="ca5c1-182">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="ca5c1-183">`edition`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-183">`edition`.</span></span> <span data-ttu-id="ca5c1-184">Для обновления используйте параметр `--edition`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-184">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="ca5c1-185">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-185">`dtu`.</span></span> <span data-ttu-id="ca5c1-186">Для обновления используйте параметр `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-186">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="ca5c1-187">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-187">`databaseDtuMin`.</span></span> <span data-ttu-id="ca5c1-188">Для обновления используйте параметр `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-188">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="ca5c1-189">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-189">`databaseDtuMax`.</span></span> <span data-ttu-id="ca5c1-190">Для обновления используйте параметр `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-190">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="ca5c1-191">Добавлены параметры `--family` и `--capacity` для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-191">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="ca5c1-192">Добавлены модули форматирования таблиц для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-192">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="ca5c1-193">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="ca5c1-193">Storage</span></span>

* <span data-ttu-id="ca5c1-194">Добавлено средство заполнения для аргумента `--account-name`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-194">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="ca5c1-195">Устранена проблема, связанная с командой `storage entity query`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-195">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="ca5c1-196">ВМ</span><span class="sxs-lookup"><span data-stu-id="ca5c1-196">VM</span></span>

* <span data-ttu-id="ca5c1-197">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--write-accelerator` из команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-197">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="ca5c1-198">Такие же возможности предоставляет команда `vm update` или `vm disk attach`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-198">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="ca5c1-199">Устранена проблема с сопоставлением образов расширения в команде `[vm|vmss] extension`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-199">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="ca5c1-200">Добавлен параметр `--boot-diagnostics-storage` для команды `vm create` для записи журнала загрузки.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-200">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="ca5c1-201">Добавлен параметр `--license-type` для команды `[vm|vmss] update`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-201">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="ca5c1-202">7 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-202">May 7, 2018</span></span>

<span data-ttu-id="ca5c1-203">Версия 2.0.32</span><span class="sxs-lookup"><span data-stu-id="ca5c1-203">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="ca5c1-204">Core</span><span class="sxs-lookup"><span data-stu-id="ca5c1-204">Core</span></span>

* <span data-ttu-id="ca5c1-205">Исправлено необработанное исключение при получении секретов из основной учетной записи службы с сертификатом.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-205">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="ca5c1-206">Добавлена ограниченная поддержка для позиционных аргументов.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-206">Added limited support for positional arguments</span></span>
* <span data-ttu-id="ca5c1-207">Исправлена проблема, когда `--query` нельзя использовать с `--ids`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-207">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="ca5c1-208">#5591</span><span class="sxs-lookup"><span data-stu-id="ca5c1-208">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="ca5c1-209">Улучшены сценарии конвейерной передачи от команд при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-209">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="ca5c1-210">Добавлена поддержка `-o tsv` с указанием запроса или `-o json` без указания запроса.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-210">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="ca5c1-211">Добавлена команда предложения в случае ошибки, если пользователи вводят команды с опечаткой.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-211">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="ca5c1-212">Исправлена ошибка, когда пользователи вводят `az ''`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-212">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="ca5c1-213">Добавлена поддержка настраиваемого ресурса для командных модулей и расширений.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-213">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="ca5c1-214">ACR</span><span class="sxs-lookup"><span data-stu-id="ca5c1-214">ACR</span></span>

* <span data-ttu-id="ca5c1-215">Добавлены команды сборки ACR.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-215">Added ACR Build commands</span></span>
* <span data-ttu-id="ca5c1-216">Исправлена ошибка о не найденных сообщениях об ошибках.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-216">Improved resource not found error messages</span></span>
* <span data-ttu-id="ca5c1-217">Оптимизированы производительность создания ресурсов и обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-217">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="ca5c1-218">Улучшены возможности входа ACR в нестандартные консоли и WSL.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-218">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="ca5c1-219">Улучшены сообщения об ошибках команд репозитория.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-219">Improved repository commands error messages</span></span>
* <span data-ttu-id="ca5c1-220">Обновлены столбцы таблиц и порядок их расположения.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-220">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="ca5c1-221">ACS</span><span class="sxs-lookup"><span data-stu-id="ca5c1-221">ACS</span></span>

* <span data-ttu-id="ca5c1-222">Добавлено предупреждение о том, что `az aks` — это предварительная версия службы.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-222">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="ca5c1-223">Исправлена проблема с разрешением в `aks install-connector`, когда `--aci-resource-group` не указывается.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-223">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="ca5c1-224">AMS</span><span class="sxs-lookup"><span data-stu-id="ca5c1-224">AMS</span></span>

* <span data-ttu-id="ca5c1-225">Первоначальный выпуск. Управление ресурсами Служб мультимедиа Azure.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-225">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="ca5c1-226">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ca5c1-226">Appservice</span></span>

* <span data-ttu-id="ca5c1-227">Исправлена ошибка в `webapp delete`, когда `--slot` предоставляется.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-227">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="ca5c1-228">Удалено `--runtime-version` из `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-228">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="ca5c1-229">Добавлена поддержка min\_tls\_version и https2.0.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-229">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="ca5c1-230">Добавлена поддержка нескольких контейнеров.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-230">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="ca5c1-231">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="ca5c1-231">Batch AI</span></span>

* <span data-ttu-id="ca5c1-232">Изменено `batchai create cluster` с учетом приоритета виртуальной машины при настройке в файле конфигурации кластера.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-232">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="ca5c1-233">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="ca5c1-233">Cognitive Services</span></span>

* <span data-ttu-id="ca5c1-234">Исправлена опечатка в примере для `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-234">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="ca5c1-235">Потребление</span><span class="sxs-lookup"><span data-stu-id="ca5c1-235">Consumption</span></span>

* <span data-ttu-id="ca5c1-236">Добавлены новые команды в API для управления бюджетом.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-236">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="ca5c1-237">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ca5c1-237">Container</span></span>

* <span data-ttu-id="ca5c1-238">Удалено требование `--registry-server` для `container create`, когда сервер реестра включен в имя образа.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-238">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="ca5c1-239">База данных Cosmos</span><span class="sxs-lookup"><span data-stu-id="ca5c1-239">Cosmos DB</span></span>

* <span data-ttu-id="ca5c1-240">Добавлена поддержка VNET для Azure CLI в Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="ca5c1-240">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="ca5c1-241">DMS</span><span class="sxs-lookup"><span data-stu-id="ca5c1-241">DMS</span></span>

* <span data-ttu-id="ca5c1-242">Исходный выпуск. Добавлена поддержка сценария миграции SQL — Azure SQL.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-242">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="ca5c1-243">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="ca5c1-243">Extension</span></span>

* <span data-ttu-id="ca5c1-244">Исправлена ошибка, когда метаданные остановленного расширения отображались.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-244">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="ca5c1-245">Interactive</span><span class="sxs-lookup"><span data-stu-id="ca5c1-245">Interactive</span></span>

* <span data-ttu-id="ca5c1-246">Разрешена работа интерактивных средств завершения с позиционными аргументами.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-246">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="ca5c1-247">Добавлены более понятные выходные данные, когда пользователи вводят \'.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-247">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="ca5c1-248">Исправлены завершения для параметров без справки.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-248">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="ca5c1-249">Исправлены описания для групп команд.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-249">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="ca5c1-250">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="ca5c1-250">Lab</span></span>

* <span data-ttu-id="ca5c1-251">Исправлены регрессии из преобразования Knack.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-251">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="ca5c1-252">Сеть</span><span class="sxs-lookup"><span data-stu-id="ca5c1-252">Network</span></span>

* <span data-ttu-id="ca5c1-253">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--ids` для:</span><span class="sxs-lookup"><span data-stu-id="ca5c1-253">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span> 
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="ca5c1-254">Профиль</span><span class="sxs-lookup"><span data-stu-id="ca5c1-254">Profile</span></span>

* <span data-ttu-id="ca5c1-255">Исправлено определение источника `disk create`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-255">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="ca5c1-256">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--msi-port` и `--identity-port`, так как они больше не используются.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-256">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="ca5c1-257">Исправлена опечатка в кратком описании `account get-access-token`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-257">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="ca5c1-258">Redis</span><span class="sxs-lookup"><span data-stu-id="ca5c1-258">Redis</span></span>

* <span data-ttu-id="ca5c1-259">Вместо `redis patch-schedule patch-schedule show` теперь используется `redis patch-schedule show`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-259">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="ca5c1-260">`redis list-all` теперь не используется.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-260">Deprecated `redis list-all`.</span></span> <span data-ttu-id="ca5c1-261">Эта функция включена в `redis list`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-261">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="ca5c1-262">Вместо `redis import-method` теперь используется `redis import`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-262">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="ca5c1-263">Добавлена поддержка `--ids` для разных команд.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-263">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="ca5c1-264">Роль</span><span class="sxs-lookup"><span data-stu-id="ca5c1-264">Role</span></span>

* <span data-ttu-id="ca5c1-265">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `ad sp reset-credentials` по причине устаревания.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-265">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="ca5c1-266">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="ca5c1-266">Storage</span></span>

* <span data-ttu-id="ca5c1-267">Разрешено применение SAS-токенов назначения к источнику для копирования BLOB-объектов, если SAS источника и ключ учетной записи не указаны.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-267">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="ca5c1-268">Добавлено отображение времени ожидания сокета для отправки и скачивания большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-268">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="ca5c1-269">Добавлена обработка имен больших двоичных объектов, которые начинаются с разделителей пути, как относительных путей.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-269">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="ca5c1-270">Разрешено использовать `storage blob copy --source-sas` с начальным символом запроса "?".</span><span class="sxs-lookup"><span data-stu-id="ca5c1-270">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="ca5c1-271">Исправлено `storage entity query --marker` для принятия списка пар "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="ca5c1-271">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="ca5c1-272">ВМ</span><span class="sxs-lookup"><span data-stu-id="ca5c1-272">VM</span></span>

* <span data-ttu-id="ca5c1-273">Исправлена недопустимая логика обнаружения в URI неуправляемого BLOB-объекта.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-273">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="ca5c1-274">Добавлена поддержка шифрования диска без предоставления пользователем субъектов-служб.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-274">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="ca5c1-275">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]. Не используйте ManagedIdentityExtension виртуальной машины для включения поддержки MSI.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-275">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="ca5c1-276">Добавлена поддержка политики вытеснения для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-276">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="ca5c1-277">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--ids` из:</span><span class="sxs-lookup"><span data-stu-id="ca5c1-277">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="ca5c1-278">Добавлена поддержка ускорителя записи.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-278">Added write accelerator support</span></span> 
* <span data-ttu-id="ca5c1-279">Добавлена команда `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-279">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="ca5c1-280">Исправлено `vm diagnostics set` для надежного определения типа ОС виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-280">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="ca5c1-281">Изменено `vm resize` для проверки того, отличается ли запрошенный размер от установленного (с обновлением только при изменении).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-281">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="ca5c1-282">10 апреля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-282">April 10, 2018</span></span>

<span data-ttu-id="ca5c1-283">Версия 2.0.31</span><span class="sxs-lookup"><span data-stu-id="ca5c1-283">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="ca5c1-284">ACR</span><span class="sxs-lookup"><span data-stu-id="ca5c1-284">ACR</span></span>

* <span data-ttu-id="ca5c1-285">Улучшена обработка ошибок при откате wincred.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-285">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="ca5c1-286">ACS</span><span class="sxs-lookup"><span data-stu-id="ca5c1-286">ACS</span></span>

* <span data-ttu-id="ca5c1-287">Срок действия имен субъектов-служб, созданных службой контейнеров Azure, изменен до 5 лет.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-287">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="ca5c1-288">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ca5c1-288">Appservice</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="ca5c1-290">Исправлено неперехватываемое исключение для несуществующих планов веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-290">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="ca5c1-291">Batch AI</span><span class="sxs-lookup"><span data-stu-id="ca5c1-291">BatchAI</span></span>

* <span data-ttu-id="ca5c1-292">Добавлена поддержка API 2018-03-01.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-292">Added support for 2018-03-01 API</span></span>

 - <span data-ttu-id="ca5c1-293">Подключение на уровне задания.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-293">Job level mounting</span></span>
 - <span data-ttu-id="ca5c1-294">Переменные среды со значениями секретов.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-294">Environment variables with secret values</span></span>
 - <span data-ttu-id="ca5c1-295">Параметры счетчиков производительности</span><span class="sxs-lookup"><span data-stu-id="ca5c1-295">Performance counters settings</span></span>
 - <span data-ttu-id="ca5c1-296">Предоставление информации о сегменте пути конкретного задания.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-296">Reporting of job specific path segment</span></span>
 - <span data-ttu-id="ca5c1-297">Поддержка вложенных папок в API списка файлов.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-297">Support for subfolders in list files api</span></span>
 - <span data-ttu-id="ca5c1-298">Предоставление информации об использовании и ограничениях.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-298">Usage and limits reporting</span></span>
 - <span data-ttu-id="ca5c1-299">Возможность указать тип кэширования для NFS-серверов.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-299">Allow to specify caching type for NFS servers</span></span>
 - <span data-ttu-id="ca5c1-300">Поддержка пользовательских образов.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-300">Support for custom images</span></span>
 - <span data-ttu-id="ca5c1-301">Добавлена поддержка инструментария pyTorch.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-301">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="ca5c1-302">Добавлена команда `job wait`, позволяющая дождаться завершения задания и сообщить код выхода задания.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-302">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="ca5c1-303">Добавлена команда `usage show`, позволяющая получить актуальные сведения об использовании и ограничениях ресурсов Batch AI для различных регионов.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-303">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="ca5c1-304">Поддержка национальных облаков.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-304">National clouds are supported</span></span>
* <span data-ttu-id="ca5c1-305">Для заданий добавлены аргументы командной строки, которые позволяют подключать файловые системы на уровне заданий. Эти же действия можно выполнять в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-305">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="ca5c1-306">Добавлены дополнительные параметры для настройки кластеров: приоритет виртуальной машины, подсеть, исходное число узлов для кластеров с автоматическим масштабированием, выбор пользовательского образа.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-306">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="ca5c1-307">Добавлен параметр командной строки, который позволяет указать тип кэширования для управляемой файловой системы NFS службы Batch AI.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-307">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="ca5c1-308">Упрощена процедура выбора подключаемой файловой системы в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-308">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="ca5c1-309">Теперь учетные данные для общего файлового ресурса Azure и контейнеров BLOB-объектов Azure указывать не нужно: CLI получит отсутствующие учетные данные с помощью ключа учетной записи хранения, указанного в параметрах командной строки, или переменной среды либо запросит ключ из службы хранилища Azure (если учетная запись хранения относится к текущей подписке).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-309">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="ca5c1-310">Команда задания потоковой передачи файлов теперь автоматически завершается при завершении задания (успешное выполнение, сбой, прерывание или удаление).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-310">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="ca5c1-311">Улучшены выходные данные `table` для операций `show`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-311">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="ca5c1-312">Добавлен параметр `--use-auto-storage` для создания кластера.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-312">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="ca5c1-313">Этот параметр упрощает управление учетными записями хранения, а также подключение общего файлового ресурса Azure и контейнеров BLOB-объектов Azure к кластеру.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-313">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="ca5c1-314">Добавлен параметр `--generate-ssh-keys` для команд `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-314">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="ca5c1-315">Добавлена возможность запустить задачу настройки узла через командную строку.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-315">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="ca5c1-316">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `job stream-file` и `job list-files` перемещены в группу `job file`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-316">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="ca5c1-317">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В команде `file-server create` параметр `--admin-user-name` переименован в `--user-name` для согласованности с командой `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-317">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="ca5c1-318">Выставление счетов</span><span class="sxs-lookup"><span data-stu-id="ca5c1-318">Billing</span></span>

* <span data-ttu-id="ca5c1-319">Добавлены команды для учетной записи регистрации.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-319">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="ca5c1-320">Потребление</span><span class="sxs-lookup"><span data-stu-id="ca5c1-320">Consumption</span></span>

* <span data-ttu-id="ca5c1-321">Добавлены команды `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-321">Added `marketplace` commands</span></span>
* <span data-ttu-id="ca5c1-322">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations summaries` переименована в `reservation summary`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-322">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="ca5c1-323">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations details` переименована в `reservation detail`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-323">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="ca5c1-324">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation` удалены короткие параметры `--reservation-order-id` и `--reservation-id`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-324">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="ca5c1-325">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation summary` удалены короткие параметры `--grain`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-325">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="ca5c1-326">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `pricesheet` удалены короткие параметры `--include-meter-details`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-326">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="ca5c1-327">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ca5c1-327">Container</span></span>

* <span data-ttu-id="ca5c1-328">Добавлены параметры подключения тома репозитория git: `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` и `--gitrepo-mount-path`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-328">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="ca5c1-329">Исправлена ошибка [#5926](https://github.com/Azure/azure-cli/issues/5926): команда `az container exec` возвращает ошибку, когда указан параметр --container-name.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-329">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="ca5c1-330">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="ca5c1-330">Extension</span></span>

* <span data-ttu-id="ca5c1-331">Сообщение о проверке распространения перенесено на уровень отладки.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-331">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="ca5c1-332">Interactive</span><span class="sxs-lookup"><span data-stu-id="ca5c1-332">Interactive</span></span>

* <span data-ttu-id="ca5c1-333">Если команда не распознана, выполнение прерывается.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-333">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="ca5c1-334">Добавлены перехватчики событий, которые используются до и после создания поддерева команд.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-334">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="ca5c1-335">Добавлены сведения о выполнении для параметров `--ids`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-335">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="ca5c1-336">Сеть</span><span class="sxs-lookup"><span data-stu-id="ca5c1-336">Network</span></span>

* <span data-ttu-id="ca5c1-337">Исправлена ошибка [#5936](https://github.com/Azure/azure-cli/issues/5936): не задаются теги `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-337">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="ca5c1-338">Добавлен аргумент `--auth-certs`, который позволяет подключать сертификаты аутентификации для `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-338">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> <span data-ttu-id="ca5c1-339">[#4910](https://github.com/Azure/azure-cli/issues/4910).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-339">[#4910](https://github.com/Azure/azure-cli/issues/4910)</span></span>
* <span data-ttu-id="ca5c1-340">Добавлены команды `ddos-protection` для создания планов защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-340">Added `ddos-protection` commands to create DDoS protection plans</span></span> 
* <span data-ttu-id="ca5c1-341">В команду `vnet [create|update]` добавлена поддержка `--ddos-protection-plan` для связи виртуальной сети с планом защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-341">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="ca5c1-342">Исправлена ошибка с флагом `--disable-bgp-route-propagation` в команде `network route-table [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-342">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="ca5c1-343">Удалены фиктивные аргументы `--public-ip-address-type` и `--subnet-type` для команды `network lb [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-343">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="ca5c1-344">В `network dns zone [import|export]` и `network dns record-set txt add-record` добавлена поддержка записей типа TXT с escape-последовательностями RFC 1035.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-344">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="ca5c1-345">Профиль</span><span class="sxs-lookup"><span data-stu-id="ca5c1-345">Profile</span></span>

* <span data-ttu-id="ca5c1-346">Добавлена поддержка классических учетных записей Azure для команды `account list`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-346">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="ca5c1-347">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены аргументы `--msi`  &  `--msi-port`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-347">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="ca5c1-348">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="ca5c1-348">RDBMS</span></span>

* <span data-ttu-id="ca5c1-349">Добавлена команда `georestore`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-349">Added `georestore` command</span></span>
* <span data-ttu-id="ca5c1-350">Из команды `create` исключено ограничение на размер хранилища.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-350">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="ca5c1-351">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ca5c1-351">Resource</span></span>

* <span data-ttu-id="ca5c1-352">Добавлена поддержка параметра `--metadata` в команде `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-352">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="ca5c1-353">Добавлена поддержка `--metadata`, `--set`, `--add` и `--remove` для команды `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-353">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="ca5c1-354">SQL</span><span class="sxs-lookup"><span data-stu-id="ca5c1-354">SQL</span></span>

* <span data-ttu-id="ca5c1-355">Добавлены команды `sql elastic-pool op list` и `sql elastic-pool op cancel`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-355">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="ca5c1-356">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="ca5c1-356">Storage</span></span>

* <span data-ttu-id="ca5c1-357">Улучшены сообщения об ошибках для строк подключения, имеющих неправильный формат.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-357">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="ca5c1-358">ВМ</span><span class="sxs-lookup"><span data-stu-id="ca5c1-358">VM</span></span>

* <span data-ttu-id="ca5c1-359">В команде `vmss create` добавлена возможность настроить для платформы количество доменов сбоя.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-359">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="ca5c1-360">Команда `vmss create` теперь по умолчанию использует стандартную балансировку нагрузки для зональных и больших масштабируемых наборов, а также масштабируемых наборов, в которых отключена одна группа размещения.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-360">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="ca5c1-362">Добавлена поддержка SKU общедоступного IP-адреса для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-362">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="ca5c1-363">В команду `vm secret format` добавлены аргументы `--keyvault` и `--resource-group` для тех случаев, когда команда не может разрешить идентификатор хранилища.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-363">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> <span data-ttu-id="ca5c1-364">[#5718](https://github.com/Azure/azure-cli/issues/5718).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-364">[#5718](https://github.com/Azure/azure-cli/issues/5718)</span></span>
* <span data-ttu-id="ca5c1-365">Улучшены сообщения об ошибках для команды `[vm|vmss create]`, когда расположение группы ресурсов не поддерживает зоны.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-365">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="ca5c1-366">27 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-366">March 27, 2018</span></span>

<span data-ttu-id="ca5c1-367">Версия 2.0.30</span><span class="sxs-lookup"><span data-stu-id="ca5c1-367">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="ca5c1-368">Core</span><span class="sxs-lookup"><span data-stu-id="ca5c1-368">Core</span></span>

* <span data-ttu-id="ca5c1-369">Отображение сообщения для расширений, которые отмечены в справке как предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-369">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="ca5c1-370">ACS</span><span class="sxs-lookup"><span data-stu-id="ca5c1-370">ACS</span></span>

* <span data-ttu-id="ca5c1-371">Устранена ошибка с проверкой SSL-сертификата для `aks install-cli` в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-371">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="ca5c1-372">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ca5c1-372">Appservice</span></span>

* <span data-ttu-id="ca5c1-373">Добавлена поддержка только протокола HTTPS для `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-373">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="ca5c1-374">Добавлена поддержка слотов для `az webapp identity [assign|show]` и `az functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-374">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="ca5c1-375">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="ca5c1-375">Backup</span></span>

* <span data-ttu-id="ca5c1-376">Добавлена новая команда `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-376">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="ca5c1-377">Эта команда используется для проверки резервного копирования виртуальной машины в любое хранилище в подписке.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-377">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="ca5c1-378">Включены идентификаторы объектов Azure для параметров `--resource-group` и `--vault-name` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="ca5c1-378">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
  * `backup container show`
  * `backup item set-policy`
  * `backup item show`
  * `backup job show`
  * `backup job stop`
  * `backup job wait`
  * `backup policy delete`
  * `backup policy get-default-for-vm`
  * `backup policy list-associated-items`
  * `backup policy set`
  * `backup policy show`
  * `backup protection backup-now`
  * `backup protection disable`
  * `backup protection enable-for-vm`
  * `backup recoverypoint show`
  * `backup restore files mount-rp`
  * `backup restore files unmount-rp`
  * `backup restore restore-disks`
  * `backup vault delete`
  * `backup vault show`
* <span data-ttu-id="ca5c1-379">Изменены параметры `--name` для поддержки формата вывода команд `backup ... show`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-379">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="ca5c1-380">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ca5c1-380">Container</span></span>

* <span data-ttu-id="ca5c1-381">Добавлена команда `container exec`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-381">Added `container exec` command.</span></span> <span data-ttu-id="ca5c1-382">Выполнение команды в контейнере для выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-382">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="ca5c1-383">Разрешение выходной таблице создавать и обновлять группу контейнеров.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-383">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="ca5c1-384">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="ca5c1-384">Extension</span></span>

* <span data-ttu-id="ca5c1-385">Добавлено сообщение для `extension add`, если расширение доступно в режиме предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-385">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="ca5c1-386">Изменен параметр `extension list-available` для отображения всех данных расширения с использованием `--show-details`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-386">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="ca5c1-387">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменена команда `extension list-available` для отображения упрощенных данных расширения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-387">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="ca5c1-388">Interactive</span><span class="sxs-lookup"><span data-stu-id="ca5c1-388">Interactive</span></span>

* <span data-ttu-id="ca5c1-389">Изменены операции завершения, активируемые сразу после завершения загрузки таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-389">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="ca5c1-390">Исправлена ошибка с использованием параметра `--style`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-390">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="ca5c1-391">Отсутствующий интерактивный лексический анализатор создается после дампа таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-391">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="ca5c1-392">Улучшена поддержка средства заполнения.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-392">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="ca5c1-393">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="ca5c1-393">Lab</span></span>

* <span data-ttu-id="ca5c1-394">Исправлены ошибки с командой `create environment`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-394">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="ca5c1-395">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="ca5c1-395">Monitor</span></span>

* <span data-ttu-id="ca5c1-396">Добавлена поддержка `--top`, `--orderby` и `--namespace` для `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-396">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="ca5c1-397">Исправлена ошибка [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` принимает разделенный пробелами список метрик для извлечения.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-397">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="ca5c1-398">Добавлена поддержка `--namespace` для `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-398">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="ca5c1-399">Сеть</span><span class="sxs-lookup"><span data-stu-id="ca5c1-399">Network</span></span>

* <span data-ttu-id="ca5c1-400">Добавлена поддержка Частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-400">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="ca5c1-401">Профиль</span><span class="sxs-lookup"><span data-stu-id="ca5c1-401">Profile</span></span>

* <span data-ttu-id="ca5c1-402">Добавлено предупреждение для `--identity-port` и `--msi-port` в `login`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-402">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="ca5c1-403">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="ca5c1-403">RDBMS</span></span>

* <span data-ttu-id="ca5c1-404">Добавлена общедоступная версия 2017-12-01 бизнес-модели API.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-404">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="ca5c1-405">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ca5c1-405">Resource</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="ca5c1-407">Роль</span><span class="sxs-lookup"><span data-stu-id="ca5c1-407">Role</span></span>

* <span data-ttu-id="ca5c1-408">Добавлена поддержка конфигурации требуемого уровня доступа и собственных клиентов для `az ad app create`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-408">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="ca5c1-409">Изменены команды `rbac`, чтобы возвращать не более 1000 идентификаторов в разрешении объекта.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-409">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="ca5c1-410">Добавлены команды `ad sp credential [reset|list|delete]` для управления учетными данными.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-410">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="ca5c1-411">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр properties из выходных данных `az role assignment [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-411">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="ca5c1-412">Добавлена поддержка разрешений `dataActions` и `notDataActions` для `role definition`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-412">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="ca5c1-413">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="ca5c1-413">Storage</span></span>

* <span data-ttu-id="ca5c1-414">Исправлена проблема с отправкой файла размером от 195 до 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-414">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="ca5c1-415">Исправлена ошибка [#4049](https://github.com/Azure/azure-cli/issues/4049): проблемы, когда при отправке добавочного большого двоичного объекта игнорируются параметры условия.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-415">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="ca5c1-416">ВМ</span><span class="sxs-lookup"><span data-stu-id="ca5c1-416">VM</span></span>

* <span data-ttu-id="ca5c1-417">Добавлено предупреждение `vmss create` для предстоящих критически важных изменений для наборов из 100 и более экземпляров.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-417">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="ca5c1-418">Добавлена поддержка устойчивости зон для `vm [snapshot|image]`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-418">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="ca5c1-419">Изменено представление экземпляра диска для улучшения отчета о состоянии шифрования.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-419">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="ca5c1-420">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] `vm extension delete` Изменена команда, которая больше не возвращает выходные данные.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-420">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="ca5c1-421">13 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-421">March 13, 2018</span></span>

<span data-ttu-id="ca5c1-422">Версия 2.0.29</span><span class="sxs-lookup"><span data-stu-id="ca5c1-422">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="ca5c1-423">ACR</span><span class="sxs-lookup"><span data-stu-id="ca5c1-423">ACR</span></span>

* <span data-ttu-id="ca5c1-424">Добавлена поддержка параметра `--image` для `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-424">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="ca5c1-425">Параметры `--manifest` и `--tag` команды `repository delete` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-425">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="ca5c1-426">Добавлена команда `repository untag` для удаления тега без удаления данных.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-426">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="ca5c1-427">ACS</span><span class="sxs-lookup"><span data-stu-id="ca5c1-427">ACS</span></span>

* <span data-ttu-id="ca5c1-428">Добавлена команда `aks upgrade-connector` для обновления существующего соединителя.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-428">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="ca5c1-429">Изменены файлы конфигурации `kubectl`. Теперь используется более разборчивый стиль YAML с разбивкой на блоки.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-429">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="ca5c1-430">Помощник</span><span class="sxs-lookup"><span data-stu-id="ca5c1-430">Advisor</span></span>

* <span data-ttu-id="ca5c1-431">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration get` переименована в `advisor configuration list`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-431">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="ca5c1-432">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration set` переименована в `advisor configuration update`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-432">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="ca5c1-433">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `advisor recommendation generate`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-433">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span> 
* <span data-ttu-id="ca5c1-434">Добавлен параметр `--refresh` для команды `advisor recommendation list`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-434">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="ca5c1-435">Добавлена команда `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-435">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="ca5c1-436">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ca5c1-436">Appservice</span></span>

* <span data-ttu-id="ca5c1-437">Команда `[webapp|functionapp] assign-identity` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-437">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="ca5c1-438">Добавлены команды управляемого удостоверения `webapp identity [assign|show]` и `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-438">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="ca5c1-439">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="ca5c1-439">Eventhubs</span></span>

* <span data-ttu-id="ca5c1-440">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="ca5c1-440">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="ca5c1-441">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="ca5c1-441">Extension</span></span>

* <span data-ttu-id="ca5c1-442">Добавлена проверка, позволяющая предупредить пользователя, если используемый дистрибутив отличается от хранящегося в исходном файле пакета, так как это может привести к возникновению ошибок.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-442">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="ca5c1-443">Interactive</span><span class="sxs-lookup"><span data-stu-id="ca5c1-443">Interactive</span></span>

* <span data-ttu-id="ca5c1-444">Исправлена ошибка [#5625](https://github.com/Azure/azure-cli/issues/5625): теперь записи журнала сохраняются в разных сеансах.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-444">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="ca5c1-445">Исправлена ошибка [#3016](https://github.com/Azure/azure-cli/issues/3016): при использовании области не создавались записи журнала.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-445">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="ca5c1-446">Исправлена ошибка [#5688](https://github.com/Azure/azure-cli/issues/5688): если при загрузке таблицы команд возникало исключение, опережающий ввод не выполнялся.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-446">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="ca5c1-447">Исправлен индикатор хода выполнения для длительных операций.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-447">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="ca5c1-448">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="ca5c1-448">Monitor</span></span>

* <span data-ttu-id="ca5c1-449">Команды `monitor autoscale-settings` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-449">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="ca5c1-450">Добавлены команды `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-450">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="ca5c1-451">Добавлены команды `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-451">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="ca5c1-452">Добавлены команды `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-452">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="ca5c1-453">Сеть</span><span class="sxs-lookup"><span data-stu-id="ca5c1-453">Network</span></span>

* <span data-ttu-id="ca5c1-454">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--tags` из `route-filter rule create`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-454">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="ca5c1-455">Удалены некоторые ошибочные значения по умолчанию для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="ca5c1-455">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="ca5c1-456">Добавлены команды `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-456">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="ca5c1-457">Добавлены параметры `--vnet` и `--subnet` для `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-457">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="ca5c1-458">Профиль</span><span class="sxs-lookup"><span data-stu-id="ca5c1-458">Profile</span></span>

* <span data-ttu-id="ca5c1-459">Параметр `--msi` для `az login` отмечен как нерекомендуемый.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-459">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="ca5c1-460">Добавлен параметр `--identity` для `az login`. Он заменяет `--msi`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-460">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="ca5c1-461">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="ca5c1-461">RDBMS</span></span>

* <span data-ttu-id="ca5c1-462">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Внесены изменения для использования предварительной версии API 2017-12-01.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-462">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="ca5c1-463">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="ca5c1-463">Service Bus</span></span>

* <span data-ttu-id="ca5c1-464">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="ca5c1-464">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="ca5c1-465">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="ca5c1-465">Storage</span></span>

* <span data-ttu-id="ca5c1-466">Исправлена ошибка [#4971](https://github.com/Azure/azure-cli/issues/4971): теперь `storage blob copy` поддерживает другие облака Azure.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-466">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="ca5c1-467">Исправлена ошибка [#5286](https://github.com/Azure/azure-cli/issues/5286): при пакетном выполнении команд `storage blob [delete-batch|download-batch|upload-batch]` больше не отображается сообщение об ошибке в предусловии.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-467">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="ca5c1-468">ВМ</span><span class="sxs-lookup"><span data-stu-id="ca5c1-468">VM</span></span>

* <span data-ttu-id="ca5c1-469">В `[vm|vmss] create` добавлена поддержка присоединения неуправляемых дисков данных и настройки кэширования.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-469">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="ca5c1-470">`[vm|vmss] assign-identity` и `[vm|vmss] remove-identity` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-470">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="ca5c1-471">Вместо нерекомендуемых команд добавлены команды `vm identity [assign|remove|show]` и `vmss identity [assign|remove|show]`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-471">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="ca5c1-472">Для приоритета `vmss create` по умолчанию установлено значение None.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-472">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="ca5c1-473">27 февраля 2018 г</span><span class="sxs-lookup"><span data-stu-id="ca5c1-473">February 27, 2018</span></span>

<span data-ttu-id="ca5c1-474">Версия 2.0.28</span><span class="sxs-lookup"><span data-stu-id="ca5c1-474">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="ca5c1-475">Core</span><span class="sxs-lookup"><span data-stu-id="ca5c1-475">Core</span></span>

* <span data-ttu-id="ca5c1-476">Исправлена ошибка с установкой Homebrew [№ 5184](https://github.com/Azure/azure-cli/issues/5184).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-476">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="ca5c1-477">Добавлена поддержка телеметрии расширения с применением пользовательских ключей.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-477">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="ca5c1-478">Добавлена функция ведения журнала HTTP в `--debug`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-478">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="ca5c1-479">ACS</span><span class="sxs-lookup"><span data-stu-id="ca5c1-479">ACS</span></span>

* <span data-ttu-id="ca5c1-480">Изменено для использования диаграмм Helm `virtual-kubelet-for-aks` для `aks install-connector` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-480">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="ca5c1-481">Исправлена ошибка с недостаточными разрешениями субъектов-служб на создание групп контейнеров ACI.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-481">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="ca5c1-482">Добавлены параметры `--aci-container-group`, `--location` и `--image-tag` для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-482">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="ca5c1-483">Удалено уведомление об устаревании из `aks get-versions`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-483">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="ca5c1-484">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ca5c1-484">Appservice</span></span>

* <span data-ttu-id="ca5c1-485">Обновления для новой версии пакета SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="ca5c1-485">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="ca5c1-486">Исправлена ошибка с сообщением `Free` о недопустимом SKU [№ 5538](https://github.com/Azure/azure-cli/issues/5538)</span><span class="sxs-lookup"><span data-stu-id="ca5c1-486">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="ca5c1-487">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="ca5c1-487">Cognitive Services</span></span>

* <span data-ttu-id="ca5c1-488">Обновлено уведомление при создании новой учетной записи Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-488">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="ca5c1-489">Потребление</span><span class="sxs-lookup"><span data-stu-id="ca5c1-489">Consumption</span></span>

* <span data-ttu-id="ca5c1-490">Добавлены новые команды для резервирования API прейскуранта.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-490">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="ca5c1-491">Обновлены существующие форматы сведений об использовании и резервировании.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-491">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="ca5c1-492">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ca5c1-492">Container</span></span>

* <span data-ttu-id="ca5c1-493">Добавлены аргументы `--secrets` и `--secrets-mount-path` в командах `container create` для использования секретов в ACI.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-493">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="ca5c1-494">Сеть</span><span class="sxs-lookup"><span data-stu-id="ca5c1-494">Network</span></span>

* <span data-ttu-id="ca5c1-495">Исправлена ошибка с отсутствующим клиентом в `network vnet-gateway vpn-client generate` [№ 5559](https://github.com/Azure/azure-cli/issues/5559).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-495">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="ca5c1-496">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ca5c1-496">Resource</span></span>

* <span data-ttu-id="ca5c1-497">Изменено `group deployment export` для отображения частичного шаблона и ошибок при сбое.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-497">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="ca5c1-498">Роль</span><span class="sxs-lookup"><span data-stu-id="ca5c1-498">Role</span></span>

* <span data-ttu-id="ca5c1-499">Добавлено `role assignment list-changelogs` для включения аудита ролей субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-499">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="ca5c1-500">SQL</span><span class="sxs-lookup"><span data-stu-id="ca5c1-500">SQL</span></span>

* <span data-ttu-id="ca5c1-501">Добавлена поддержка избыточности зон для создания и обновления баз данных и эластичных пулов.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-501">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="ca5c1-502">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="ca5c1-502">Storage</span></span>

* <span data-ttu-id="ca5c1-503">Включено определение пути назначения и префикса для `storage blob [upload-batch|download-batch]`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-503">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="ca5c1-504">ВМ</span><span class="sxs-lookup"><span data-stu-id="ca5c1-504">VM</span></span>

* <span data-ttu-id="ca5c1-505">Добавлена поддержка присоединения и отсоединения дисков на одном экземпляре VMSS.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-505">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="ca5c1-506">13 февраля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-506">February 13, 2018</span></span>

<span data-ttu-id="ca5c1-507">Версия 2.0.27</span><span class="sxs-lookup"><span data-stu-id="ca5c1-507">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="ca5c1-508">Core</span><span class="sxs-lookup"><span data-stu-id="ca5c1-508">Core</span></span>

* <span data-ttu-id="ca5c1-509">Изменен способ аутентификации при входе с помощью MSI: применяется ключ при использовании идентификатора подписки и имени.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-509">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="ca5c1-510">ACS</span><span class="sxs-lookup"><span data-stu-id="ca5c1-510">ACS</span></span>

* <span data-ttu-id="ca5c1-511">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименовано `aks get-versions` на `aks get-upgrades` для точности.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-511">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="ca5c1-512">Изменено `aks get-versions` для отображения версий Kubernetes, доступных для `aks create`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-512">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="ca5c1-513">Изменены значения по умолчанию `aks create`, чтобы разрешить серверу выбирать версию Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-513">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="ca5c1-514">Обновлены справочные сообщения, связанные с субъектом-службой и создаваемые AKS.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-514">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="ca5c1-515">Изменены стандартные размеры узла для `aks create` с уровня Standard\_D1\_v2 на уровень Standard\_DS1\_v2.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-515">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="ca5c1-516">Улучшена надежность при поиске панели мониторинга для группы pod для `az aks browse`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-516">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="ca5c1-517">Исправлена команда `aks get-credentials` для обработки ошибок Юникода при загрузке файлов конфигурации Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-517">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="ca5c1-518">Добавлено сообщение в `az aks install-cli`, чтобы помочь получить `kubectl` в `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-518">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="ca5c1-519">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ca5c1-519">Appservice</span></span>

* <span data-ttu-id="ca5c1-520">Исправлена проблема со сбоем `webapp [backup|restore]` из-за пустой ссылки.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-520">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="ca5c1-521">Добавлена поддержка стандартных планов службы приложений с помощью `az configure --defaults appserviceplan=my-asp`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-521">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="ca5c1-522">CDN</span><span class="sxs-lookup"><span data-stu-id="ca5c1-522">CDN</span></span>

* <span data-ttu-id="ca5c1-523">Добавлены команды `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-523">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="ca5c1-524">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ca5c1-524">Container</span></span>

* <span data-ttu-id="ca5c1-525">Добавлен параметр `--follow` для `az container logs` для журналов потоковой передачи.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-525">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="ca5c1-526">Добавлена команда `container attach`, которая добавляет локальный стандартный поток вывода и поток вывода сообщений об ошибках к контейнеру в группе контейнеров.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-526">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="ca5c1-527">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="ca5c1-527">CosmosDB</span></span>

* <span data-ttu-id="ca5c1-528">Добавлена поддержка настройки параметров.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-528">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="ca5c1-529">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="ca5c1-529">Extension</span></span>

* <span data-ttu-id="ca5c1-530">Добавлена поддержка параметра `--pip-proxy` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-530">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="ca5c1-531">Добавлена поддержка аргумента `--pip-extra-index-urls` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-531">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="ca5c1-532">Отзыв</span><span class="sxs-lookup"><span data-stu-id="ca5c1-532">Feedback</span></span>

* <span data-ttu-id="ca5c1-533">Добавлены сведения о расширении к данным телеметрии.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-533">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="ca5c1-534">Interactive</span><span class="sxs-lookup"><span data-stu-id="ca5c1-534">Interactive</span></span>

* <span data-ttu-id="ca5c1-535">Исправлена проблема, когда пользователю предлагалось войти в интерактивном режиме в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-535">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="ca5c1-536">Исправлена регрессия с отсутствующей функцией заполнения параметров.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-536">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="ca5c1-537">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="ca5c1-537">IoT</span></span>

* <span data-ttu-id="ca5c1-538">Исправлена проблема, когда `iot dps access policy [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="ca5c1-538">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="ca5c1-539">Исправлена проблема, когда `iot dps linked-hub [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="ca5c1-539">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="ca5c1-540">Добавлена поддержка параметра `--no-wait` для `iot dps access policy [create|update]` и `iot dps linked-hub [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-540">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="ca5c1-541">Изменена команда `iot hub create` для указания числа секций.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-541">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="ca5c1-542">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="ca5c1-542">Monitor</span></span>

* <span data-ttu-id="ca5c1-543">Исправлена команда `az monitor log-profiles create`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-543">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="ca5c1-544">Сеть</span><span class="sxs-lookup"><span data-stu-id="ca5c1-544">Network</span></span>

* <span data-ttu-id="ca5c1-545">Исправлен параметр `--tags` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="ca5c1-545">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="ca5c1-546">Профиль</span><span class="sxs-lookup"><span data-stu-id="ca5c1-546">Profile</span></span>

* <span data-ttu-id="ca5c1-547">Включена команда `az login` для использования в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-547">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="ca5c1-548">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ca5c1-548">Resource</span></span>

* <span data-ttu-id="ca5c1-549">Снова добавлена команда `feature show`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-549">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="ca5c1-550">Роль</span><span class="sxs-lookup"><span data-stu-id="ca5c1-550">Role</span></span>

* <span data-ttu-id="ca5c1-551">Добавлен аргумент `--available-to-other-tenants` для команды `ad app update`</span><span class="sxs-lookup"><span data-stu-id="ca5c1-551">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="ca5c1-552">SQL</span><span class="sxs-lookup"><span data-stu-id="ca5c1-552">SQL</span></span>

* <span data-ttu-id="ca5c1-553">Добавлены команды `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-553">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="ca5c1-554">Добавлена команда `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-554">Added `sql db rename`</span></span>
* <span data-ttu-id="ca5c1-555">Добавлена поддержка аргумента `--ids` для команд SQL.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-555">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="ca5c1-556">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="ca5c1-556">Storage</span></span>

* <span data-ttu-id="ca5c1-557">Добавлены команды `storage blob service-properties delete-policy` и `storage blob undelete` для включения обратимого удаления.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-557">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="ca5c1-558">ВМ</span><span class="sxs-lookup"><span data-stu-id="ca5c1-558">VM</span></span>

* <span data-ttu-id="ca5c1-559">Исправлена ошибка, когда шифрование виртуальной машины инициализировалось не полностью.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-559">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="ca5c1-560">Добавлены выходные данные идентификатора субъекта для включения MSI.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-560">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="ca5c1-561">Фиксированное значение `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="ca5c1-561">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="ca5c1-562">31 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-562">January 31, 2018</span></span>

<span data-ttu-id="ca5c1-563">Версия 2.0.26</span><span class="sxs-lookup"><span data-stu-id="ca5c1-563">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="ca5c1-564">Core</span><span class="sxs-lookup"><span data-stu-id="ca5c1-564">Core</span></span>

* <span data-ttu-id="ca5c1-565">Добавлена поддержка получения необработанного маркера в контексте MSI.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-565">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="ca5c1-566">Удалена строка индикатора опроса после завершения LRO при выполнении cmd.exe в Windows.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-566">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="ca5c1-567">Добавлено предупреждение, которое появляется при использовании настроенных по умолчанию параметров, измененных на запись уровня INFO.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-567">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="ca5c1-568">Используйте `--verbose` для просмотра.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-568">Use `--verbose` to see</span></span>
* <span data-ttu-id="ca5c1-569">Добавьте индикатор хода выполнения для ожидания команд.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-569">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="ca5c1-570">ACS</span><span class="sxs-lookup"><span data-stu-id="ca5c1-570">ACS</span></span>

* <span data-ttu-id="ca5c1-571">Добавлено описание аргумента `--disable-browser`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-571">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="ca5c1-572">Улучшено заполнение нажатием клавиши TAB для аргументов `--vm-size`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-572">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="ca5c1-573">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ca5c1-573">Appservice</span></span>

* <span data-ttu-id="ca5c1-574">Фиксированное значение `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="ca5c1-574">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="ca5c1-575">Удалена проверка `kind` в веб-приложениях и функциях.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-575">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="ca5c1-576">CDN</span><span class="sxs-lookup"><span data-stu-id="ca5c1-576">CDN</span></span>

* <span data-ttu-id="ca5c1-577">Устранена проблема с отсутствием клиента для команды `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-577">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="ca5c1-578">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="ca5c1-578">CosmosDB</span></span>

* <span data-ttu-id="ca5c1-579">Исправлено описание параметров для политик отработки отказа.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-579">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="ca5c1-580">Interactive</span><span class="sxs-lookup"><span data-stu-id="ca5c1-580">Interactive</span></span>

* <span data-ttu-id="ca5c1-581">Исправлена проблема, когда заполнение параметров команд больше не выполнялось.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-581">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="ca5c1-582">Сеть</span><span class="sxs-lookup"><span data-stu-id="ca5c1-582">Network</span></span>

* <span data-ttu-id="ca5c1-583">Добавлена защита `--cert-password` для `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-583">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="ca5c1-584">Исправлена проблема с `application-gateway update`, когда команда `--sku` ошибочно применяла значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-584">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="ca5c1-585">Добавлена защита `--shared-key` и `--authorization-key` для `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-585">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="ca5c1-586">Устранена проблема с отсутствием клиента для команды `asg create`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-586">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="ca5c1-587">Добавлен параметр `--file-name / -f` для экспортируемых имен в `dns zone export`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-587">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="ca5c1-588">Исправлены следующие ошибки для `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="ca5c1-588">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="ca5c1-589">Исправлена проблема, когда длинные записи ТХТ неправильно экспортировались.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-589">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="ca5c1-590">Исправлена проблема, когда записи ТХТ в кавычках неправильно экспортировались без символов экранирования.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-590">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="ca5c1-591">Исправлена проблема, когда некоторые записи импортировались дважды с помощью `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-591">Fixed issue where certain records were imported twice with `dns zone import`</span></span> 
* <span data-ttu-id="ca5c1-592">Восстановлены команды `vnet-gateway root-cert` и `vnet-gateway revoked-cert`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-592">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="ca5c1-593">Профиль</span><span class="sxs-lookup"><span data-stu-id="ca5c1-593">Profile</span></span>

* <span data-ttu-id="ca5c1-594">Исправлена команда `get-access-token` для работы в виртуальной машине с идентификатором.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-594">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="ca5c1-595">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ca5c1-595">Resource</span></span>

* <span data-ttu-id="ca5c1-596">Исправлена ошибка с `deployment [create|validate]`, когда предупреждение неправильно отображалось, если поле type шаблона содержало значения в верхнем регистре.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-596">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="ca5c1-597">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="ca5c1-597">Storage</span></span>

* <span data-ttu-id="ca5c1-598">Исправлена проблема с переносом учетных записей хранения из версии 1 в версию 2.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-598">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="ca5c1-599">Добавлены отчеты о ходе выполнения всех команд отправки или скачивания.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-599">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="ca5c1-600">Исправлена ошибка, которая препятствовала использованию параметра аргумента -n с `storage account check-name`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-600">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>  
* <span data-ttu-id="ca5c1-601">Добавлен столбец snapshot в табличные выходные данные для `blob [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-601">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="ca5c1-602">Исправлены ошибки с разными параметрами, которые должны были анализироваться как целые числа.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-602">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="ca5c1-603">ВМ</span><span class="sxs-lookup"><span data-stu-id="ca5c1-603">VM</span></span>

* <span data-ttu-id="ca5c1-604">Добавлена команда `vm image accept-terms` для разрешения создания виртуальных машин из образов с дополнительными расходами.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-604">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="ca5c1-605">Исправлена команда `[vm|vmss create]` для выполнения команд с прокси-сервера с помощью неподписанных сертификатов.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-605">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="ca5c1-606">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка режима низкого приоритета для VMSS.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-606">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="ca5c1-607">Добавлена защита `--admin-password` для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-607">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="ca5c1-608">17 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-608">January 17, 2018</span></span>

<span data-ttu-id="ca5c1-609">Версия 2.0.25</span><span class="sxs-lookup"><span data-stu-id="ca5c1-609">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="ca5c1-610">ACR</span><span class="sxs-lookup"><span data-stu-id="ca5c1-610">ACR</span></span>

* <span data-ttu-id="ca5c1-611">Добавлена возможность отката входа ACR при ошибках учетных данных в Windows.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-611">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="ca5c1-612">Включены журналы реестра.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-612">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="ca5c1-613">ACS</span><span class="sxs-lookup"><span data-stu-id="ca5c1-613">ACS</span></span>

* <span data-ttu-id="ca5c1-614">Исправлена команда `get-credentials`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-614">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="ca5c1-615">Удалено требование роли для имени субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-615">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="ca5c1-616">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ca5c1-616">Appservice</span></span>

* <span data-ttu-id="ca5c1-617">Исправлена ошибка с `config ssl upload`, при которой значение `hosting_environment_profile` было NULL.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-617">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="ca5c1-618">В `browse` добавлена поддержка для пользовательских URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-618">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="ca5c1-619">Исправлена поддержка слотов для `log tail`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-619">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="ca5c1-620">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="ca5c1-620">Backup</span></span>

* <span data-ttu-id="ca5c1-621">Параметр `--container-name` для `backup item list` теперь не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-621">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="ca5c1-622">В `backup restore restore-disks` добавлены варианты учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-622">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="ca5c1-623">Для проверки расположения в `backup protection enable-for-vm` добавлена чувствительность к регистру.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-623">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="ca5c1-624">Устранена проблема, при которой команды завершались сбоем с указанием недопустимого имени контейнера.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-624">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="ca5c1-625">В `backup item list` теперь по умолчанию включен параметр Health Status.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-625">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="ca5c1-626">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="ca5c1-626">Batch</span></span>

* <span data-ttu-id="ca5c1-627">`batch login` теперь возвращает сведения об аутентификации.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-627">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="ca5c1-628">Облако</span><span class="sxs-lookup"><span data-stu-id="ca5c1-628">Cloud</span></span>

* <span data-ttu-id="ca5c1-629">При установке `--profile` в облаке теперь не требуется указывать конечные точки.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-629">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="ca5c1-630">Потребление</span><span class="sxs-lookup"><span data-stu-id="ca5c1-630">Consumption</span></span>

* <span data-ttu-id="ca5c1-631">Добавлены новые команды для резервирования: `consumption reservations summaries` и `consumption reservations details`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-631">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="ca5c1-632">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="ca5c1-632">Event Grid</span></span>

* <span data-ttu-id="ca5c1-633">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid topic event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-633">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="ca5c1-634">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid resource event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-634">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="ca5c1-635">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-635">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="ca5c1-636">Вместо нее следует использовать `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-636">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="ca5c1-637">Добавлена команда `eventgrid topic update`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-637">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="ca5c1-638">Добавлена команда `eventgrid event-subscription update`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-638">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="ca5c1-639">Добавлен параметр `--ids` для команд `eventgrid topic`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-639">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="ca5c1-640">Добавлена поддержка заполнения нажатием клавиши TAB для имен разделов.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-640">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="ca5c1-641">Interactive</span><span class="sxs-lookup"><span data-stu-id="ca5c1-641">Interactive</span></span>

* <span data-ttu-id="ca5c1-642">Устранена проблема, при которой интерактивный режим не работал с Python 2.x.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-642">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="ca5c1-643">Исправлены ошибки при запуске.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-643">Fixed errors on startup</span></span>
* <span data-ttu-id="ca5c1-644">Устранена проблема, при которой некоторые команды не работали в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-644">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="ca5c1-645">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="ca5c1-645">IoT</span></span>

* <span data-ttu-id="ca5c1-646">Добавлена поддержка службы подготовки устройств.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-646">Added support for device provisioning service</span></span>
* <span data-ttu-id="ca5c1-647">В команды и справочную информацию о них добавлены сообщения о нерекомендуемых версиях.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-647">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="ca5c1-648">Теперь при проверке Интернета вещей указывается расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-648">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="ca5c1-649">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="ca5c1-649">Monitor</span></span>

* <span data-ttu-id="ca5c1-650">Добавлена поддержка параметра нескольких диагностических операций.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-650">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="ca5c1-651">Теперь параметр `--name` является обязательным для `az monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-651">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="ca5c1-652">Добавлена команда `monitor diagnostic-settings categories` для получения категории параметров диагностики.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-652">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="ca5c1-653">Сеть</span><span class="sxs-lookup"><span data-stu-id="ca5c1-653">Network</span></span>

* <span data-ttu-id="ca5c1-654">Устранена проблема с `vnet-gateway update` при попытке входа в активный режим и режим ожидания или выхода из них.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-654">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="ca5c1-655">Для `application-gateway [create|update]` добавлена поддержка HTTP2.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-655">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="ca5c1-656">Профиль</span><span class="sxs-lookup"><span data-stu-id="ca5c1-656">Profile</span></span>

* <span data-ttu-id="ca5c1-657">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-657">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="ca5c1-658">Роль</span><span class="sxs-lookup"><span data-stu-id="ca5c1-658">Role</span></span>

* <span data-ttu-id="ca5c1-659">В `role assignment create` добавлен аргумент `--assignee-object-id`, чтобы обойти запрос графов.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-659">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="ca5c1-660">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="ca5c1-660">Service Fabric</span></span>

* <span data-ttu-id="ca5c1-661">В результат проверки при создании кластера добавлены подробные сведения об ошибках.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-661">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="ca5c1-662">Устранена проблема отсутствия клиента при выполнении некоторых команд.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-662">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="ca5c1-663">ВМ</span><span class="sxs-lookup"><span data-stu-id="ca5c1-663">VM</span></span>

* <span data-ttu-id="ca5c1-664">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Поддержка разных зон для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-664">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="ca5c1-665">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию `vmss` для одной зоны заменено данными подсистемы балансировки нагрузки уровня "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="ca5c1-665">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="ca5c1-666">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для EMSI параметр `externalIdentities` изменен на `userAssignedIdentities`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-666">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="ca5c1-667">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка переключения дисков ОС.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-667">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="ca5c1-668">Добавлена поддержка использования образов виртуальных машин из других подписок.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-668">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="ca5c1-669">В `[vm|vmss] create` добавлены аргументы `--plan-name`, `--plan-product`, `--plan-promotion-code` и `--plan-publisher`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-669">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="ca5c1-670">Устранены проблемы с `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-670">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="ca5c1-671">Устранена проблема чрезмерного использования ресурсов из-за `vm image list --all`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-671">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="ca5c1-672">19 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-672">December 19, 2017</span></span>

<span data-ttu-id="ca5c1-673">Версия 2.0.23</span><span class="sxs-lookup"><span data-stu-id="ca5c1-673">Version 2.0.23</span></span>

* <span data-ttu-id="ca5c1-674">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-674">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="ca5c1-675">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ca5c1-675">Container</span></span>

* <span data-ttu-id="ca5c1-676">Исправлен неправильный порядок параметров для журналов контейнеров.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-676">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="ca5c1-677">Сеть</span><span class="sxs-lookup"><span data-stu-id="ca5c1-677">Network</span></span>

* <span data-ttu-id="ca5c1-678">Добавлен аргумент `--disable-bgp-route-propagation` для команды `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="ca5c1-678">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="ca5c1-679">Добавлен аргумент `--ip-tags` для команды `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="ca5c1-679">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="ca5c1-680">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="ca5c1-680">Storage</span></span>

* <span data-ttu-id="ca5c1-681">Добавлена поддержка хранилища версии 2.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-681">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="ca5c1-682">ВМ</span><span class="sxs-lookup"><span data-stu-id="ca5c1-682">VM</span></span>

* <span data-ttu-id="ca5c1-683">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для назначенных пользователям удостоверений для виртуальных машин и VMSS.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-683">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="ca5c1-684">5 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-684">December 5, 2017</span></span>

<span data-ttu-id="ca5c1-685">Версия 2.0.22</span><span class="sxs-lookup"><span data-stu-id="ca5c1-685">Version 2.0.22</span></span>

* <span data-ttu-id="ca5c1-686">Удалена команда `az component`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-686">Removed `az component` commands.</span></span> <span data-ttu-id="ca5c1-687">Вместо нее следует использовать `az extension`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-687">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="ca5c1-688">Core</span><span class="sxs-lookup"><span data-stu-id="ca5c1-688">Core</span></span>
* <span data-ttu-id="ca5c1-689">Конечная точка `AZURE_US_GOV_CLOUD` центра AAD изменена с login.microsoftonline.com на login.microsoftonline.us.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-689">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="ca5c1-690">Исправлена проблема с непрерывной отправкой телеметрии.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-690">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="ca5c1-691">ACS</span><span class="sxs-lookup"><span data-stu-id="ca5c1-691">ACS</span></span>

* <span data-ttu-id="ca5c1-692">Добавлены команды `aks install-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-692">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="ca5c1-693">Улучшены сообщения об ошибках для команды `acs create`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-693">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="ca5c1-694">Добавлена возможность использования команды `aks get-credentials -f` без полного пути.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-694">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="ca5c1-695">Помощник</span><span class="sxs-lookup"><span data-stu-id="ca5c1-695">Advisor</span></span>

* <span data-ttu-id="ca5c1-696">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="ca5c1-696">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="ca5c1-697">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ca5c1-697">Appservice</span></span>

* <span data-ttu-id="ca5c1-698">Добавлена возможность создания имени сертификата с помощью команды `webapp config ssl upload`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-698">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="ca5c1-699">Исправлены команды `webapp [list|show]` и `functionapp [list|show]` для отображения правильных приложений.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-699">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="ca5c1-700">Добавлено стандартное значение для переменной `WEBSITE_NODE_DEFAULT_VERSION`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-700">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="ca5c1-701">Потребление</span><span class="sxs-lookup"><span data-stu-id="ca5c1-701">Consumption</span></span>

* <span data-ttu-id="ca5c1-702">Добавлена поддержка API версии 2017-11-30.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-702">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="ca5c1-703">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ca5c1-703">Container</span></span>

* <span data-ttu-id="ca5c1-704">Исправлены стандартные порты регрессии.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-704">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="ca5c1-705">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="ca5c1-705">Monitor</span></span>

* <span data-ttu-id="ca5c1-706">Добавлена поддержка нескольких измерений для команд метрик.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-706">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="ca5c1-707">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ca5c1-707">Resource</span></span>

* <span data-ttu-id="ca5c1-708">Добавлен аргумент `--include-response-body` для команды `resource show`</span><span class="sxs-lookup"><span data-stu-id="ca5c1-708">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="ca5c1-709">Роль</span><span class="sxs-lookup"><span data-stu-id="ca5c1-709">Role</span></span>

* <span data-ttu-id="ca5c1-710">Добавлено отображение стандартных назначений "классических" администраторов для команды `role assignment list`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-710">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="ca5c1-711">Добавлена поддержка команды `ad sp reset-credentials` для добавления учетных данных вместо перезаписи.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-711">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="ca5c1-712">Улучшены сообщения об ошибках для команды `ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-712">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="ca5c1-713">SQL</span><span class="sxs-lookup"><span data-stu-id="ca5c1-713">SQL</span></span>

* <span data-ttu-id="ca5c1-714">Добавлены команды `sql db list-usages` и `sql db show-usage`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-714">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="ca5c1-715">Добавлены команды `sql server conn-policy show` и `sql server conn-policy update`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-715">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="ca5c1-716">ВМ</span><span class="sxs-lookup"><span data-stu-id="ca5c1-716">VM</span></span>

* <span data-ttu-id="ca5c1-717">Добавлены сведения о зонах для команды `az vm list-skus`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-717">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="ca5c1-718">14 ноября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-718">November 14, 2017</span></span>

<span data-ttu-id="ca5c1-719">Версия 2.0.21</span><span class="sxs-lookup"><span data-stu-id="ca5c1-719">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="ca5c1-720">ACR</span><span class="sxs-lookup"><span data-stu-id="ca5c1-720">ACR</span></span>

* <span data-ttu-id="ca5c1-721">Добавлена поддержка создания веб-перехватчиков в регионах репликации.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-721">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="ca5c1-722">ACS</span><span class="sxs-lookup"><span data-stu-id="ca5c1-722">ACS</span></span>

* <span data-ttu-id="ca5c1-723">В AKS агент теперь называется узлом.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-723">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="ca5c1-724">Параметр `--orchestrator-release` для командлета `acs create` не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-724">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="ca5c1-725">Изменен размер виртуальной машины для AKS по умолчанию на `Standard_D1_v2`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-725">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="ca5c1-726">Исправлена команда `az aks browse` для Windows.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-726">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="ca5c1-727">Исправлена команда `az aks get-credentials` для Windows.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-727">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="ca5c1-728">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ca5c1-728">Appservice</span></span>

* <span data-ttu-id="ca5c1-729">Добавлен источник развертывания `config-zip` для веб-приложений и приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-729">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="ca5c1-730">Добавлен параметр `--docker-container-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-730">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="ca5c1-731">Удален параметр `storage` из параметра `--web-server-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-731">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="ca5c1-732">Улучшены сообщения об ошибках для команды `deployment user set`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-732">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="ca5c1-733">Добавлена поддержка создания приложений-функций Linux</span><span class="sxs-lookup"><span data-stu-id="ca5c1-733">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="ca5c1-734">Фиксированное значение `list-locations`</span><span class="sxs-lookup"><span data-stu-id="ca5c1-734">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="ca5c1-735">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="ca5c1-735">Batch</span></span>

* <span data-ttu-id="ca5c1-736">Исправлена ошибка в команде создания пула, когда идентификатор ресурса использовался с флагом `--image`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-736">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="ca5c1-737">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="ca5c1-737">Batchai</span></span>

* <span data-ttu-id="ca5c1-738">Добавлен короткий параметр `-s` для параметра `--vm-size` при указании размера виртуальной машины в команде `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-738">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="ca5c1-739">Добавлены аргументы ключа и имени учетной записи хранения в параметры команды `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-739">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="ca5c1-740">Исправлена документация по командам `job list-files` и `job stream-file`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-740">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="ca5c1-741">Добавлен короткий параметр `-r` для параметра `--cluster-name` при указании имени кластера в команде `job create`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-741">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="ca5c1-742">Облако</span><span class="sxs-lookup"><span data-stu-id="ca5c1-742">Cloud</span></span>

* <span data-ttu-id="ca5c1-743">Изменена команда `cloud [register|update]` для предотвращения регистрации облаков, для которых отсутствуют необходимые конечные точки.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-743">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="ca5c1-744">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ca5c1-744">Container</span></span>

* <span data-ttu-id="ca5c1-745">Добавлена поддержка открытия нескольких портов.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-745">Added support to open multiple ports</span></span>
* <span data-ttu-id="ca5c1-746">Добавлена политика перезапуска группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-746">Added container group restart policy</span></span>
* <span data-ttu-id="ca5c1-747">Добавлена поддержка подключения файлового ресурса Azure в качестве тома.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-747">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="ca5c1-748">Обновлена вспомогательная документация.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-748">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="ca5c1-749">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="ca5c1-749">Data Lake Analytics</span></span>

* <span data-ttu-id="ca5c1-750">Изменена команда `[job|account] list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-750">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="ca5c1-751">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="ca5c1-751">Data Lake Store</span></span>

* <span data-ttu-id="ca5c1-752">Изменена команда `account list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-752">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="ca5c1-753">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="ca5c1-753">Extension</span></span>

* <span data-ttu-id="ca5c1-754">Добавлена команда `extension list-available` для отображения официальных расширений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-754">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="ca5c1-755">Добавлен параметр `--name` для команды `extension [add|update]` для установки расширений по имени.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-755">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="ca5c1-756">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="ca5c1-756">IoT</span></span>

* <span data-ttu-id="ca5c1-757">Добавлена поддержка центров сертификации (ЦС) и цепочек сертификатов.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-757">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="ca5c1-758">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="ca5c1-758">Monitor</span></span>

* <span data-ttu-id="ca5c1-759">Добавлены команды `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-759">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="ca5c1-760">Сеть</span><span class="sxs-lookup"><span data-stu-id="ca5c1-760">Network</span></span>

* <span data-ttu-id="ca5c1-761">Добавлена поддержка DNS-записей типа CAA.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-761">Added support for CAA DNS records</span></span>
* <span data-ttu-id="ca5c1-762">Исправлена проблема, когда конечные точки могли не обновляться с помощью команды `traffic-manager profile update`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-762">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="ca5c1-763">Исправлена проблема, когда команда `vnet update --dns-servers` не работала в зависимости от способа создания виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-763">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="ca5c1-764">Исправлена проблема, когда относительные DNS-имена неправильно импортировались с помощью команды `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-764">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="ca5c1-765">Резервирование</span><span class="sxs-lookup"><span data-stu-id="ca5c1-765">Reservations</span></span>

* <span data-ttu-id="ca5c1-766">Первоначальный выпуск предварительной версии</span><span class="sxs-lookup"><span data-stu-id="ca5c1-766">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="ca5c1-767">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ca5c1-767">Resource</span></span>

* <span data-ttu-id="ca5c1-768">Добавлена поддержка идентификаторов ресурсов для блокировок на уровне ресурсов и параметра `--resource`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-768">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="ca5c1-769">SQL</span><span class="sxs-lookup"><span data-stu-id="ca5c1-769">SQL</span></span>

* <span data-ttu-id="ca5c1-770">Добавлен параметр `--ignore-missing-vnet-service-endpoint` для команды `sql server vnet-rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-770">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="ca5c1-771">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="ca5c1-771">Storage</span></span>

* <span data-ttu-id="ca5c1-772">Изменена команда `storage account create` для использования номера SKU `Standard_RAGRS` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-772">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="ca5c1-773">Исправлены ошибки при обработке имени файла или большого двоичного объекта, содержащего символы, отличные от ASCII.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-773">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="ca5c1-774">Исправлена ошибка, препятствующая использованию параметра `--source-uri` с командой `storage [blob|file] copy start-batch`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-774">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="ca5c1-775">Добавлены команды для удаления нескольких объектов с помощью команды `storage [blob|file] delete-batch`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-775">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="ca5c1-776">Исправлена проблема с включением метрик с помощью команды `storage metrics update`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-776">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="ca5c1-777">Исправлена проблема с файлами более 200 ГБ при использовании команды `storage blob upload-batch`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-777">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="ca5c1-778">Исправлена проблема, когда параметры `--bypass` и `--default-action` игнорировались командой `storage account [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-778">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="ca5c1-779">ВМ</span><span class="sxs-lookup"><span data-stu-id="ca5c1-779">VM</span></span>

* <span data-ttu-id="ca5c1-780">Исправлена ошибка с командой `vmss create`, препятствующая использованию уровня `Basic`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-780">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="ca5c1-781">Добавлены аргументы `--plan` для команды `[vm|vmss] create` для пользовательских образов с информацией о выставлении счетов.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-781">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="ca5c1-782">Добавлены команды `vm secret `[add|remove|list]\`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-782">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="ca5c1-783">Команда `vm format-secret` переименована в `vm secret format`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-783">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="ca5c1-784">Добавлен аргумент `--encrypt format` для команды `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="ca5c1-784">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="ca5c1-785">24 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-785">October 24, 2017</span></span>

<span data-ttu-id="ca5c1-786">Версия 2.0.20</span><span class="sxs-lookup"><span data-stu-id="ca5c1-786">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="ca5c1-787">Core</span><span class="sxs-lookup"><span data-stu-id="ca5c1-787">Core</span></span>

* <span data-ttu-id="ca5c1-788">Обновление `2017-03-09-profile` для использования API `MGMT_STORAGE` версии `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="ca5c1-788">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="ca5c1-789">ACR</span><span class="sxs-lookup"><span data-stu-id="ca5c1-789">ACR</span></span>

* <span data-ttu-id="ca5c1-790">Обновление службы управления ресурсами для указания API версии `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="ca5c1-790">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="ca5c1-791">Изменение номера SKU BYOS-хранилища на "Классический"</span><span class="sxs-lookup"><span data-stu-id="ca5c1-791">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="ca5c1-792">Переименование номеров SKU реестра на "Базовый", "Стандартный" и "Премиум"</span><span class="sxs-lookup"><span data-stu-id="ca5c1-792">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="ca5c1-793">ACS</span><span class="sxs-lookup"><span data-stu-id="ca5c1-793">ACS</span></span>

* <span data-ttu-id="ca5c1-794">[ПРЕДВАРИЕТЛЬНАЯ ВЕРСИЯ] Добавление команд `az aks`</span><span class="sxs-lookup"><span data-stu-id="ca5c1-794">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="ca5c1-795">Исправление Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="ca5c1-795">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="ca5c1-796">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ca5c1-796">Appservice</span></span>

* <span data-ttu-id="ca5c1-797">Исправление проблемы с недопустимыми скачанными журналами `webapp`</span><span class="sxs-lookup"><span data-stu-id="ca5c1-797">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="ca5c1-798">Компонент</span><span class="sxs-lookup"><span data-stu-id="ca5c1-798">Component</span></span>

* <span data-ttu-id="ca5c1-799">Добавление более понятного сообщения об устаревании для всех установщиков, а также запроса на подтверждение</span><span class="sxs-lookup"><span data-stu-id="ca5c1-799">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="ca5c1-800">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="ca5c1-800">Monitor</span></span>

* <span data-ttu-id="ca5c1-801">Добавлены команды `action-group`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-801">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="ca5c1-802">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ca5c1-802">Resource</span></span>

* <span data-ttu-id="ca5c1-803">Исправление несовместимости с самой последней версии зависимости msrest в `group export`</span><span class="sxs-lookup"><span data-stu-id="ca5c1-803">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="ca5c1-804">Исправление `policy assignment create` для работы с определениями встроенных политик и наборов политик</span><span class="sxs-lookup"><span data-stu-id="ca5c1-804">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="ca5c1-805">ВМ</span><span class="sxs-lookup"><span data-stu-id="ca5c1-805">VM</span></span>

* <span data-ttu-id="ca5c1-806">Добавлен аргумент `--accelerated-networking` для команды `vmss create`</span><span class="sxs-lookup"><span data-stu-id="ca5c1-806">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="ca5c1-807">9 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-807">October 9, 2017</span></span>

<span data-ttu-id="ca5c1-808">Версия 2.0.19</span><span class="sxs-lookup"><span data-stu-id="ca5c1-808">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="ca5c1-809">Core</span><span class="sxs-lookup"><span data-stu-id="ca5c1-809">Core</span></span>

* <span data-ttu-id="ca5c1-810">В Azure Stack добавлена обработка URL-адресов центра ADFS с завершающей косой чертой.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-810">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="ca5c1-811">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ca5c1-811">Appservice</span></span>

* <span data-ttu-id="ca5c1-812">Добавлена возможность общего обновления с помощью новой команды `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-812">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="ca5c1-813">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="ca5c1-813">Batch</span></span>

* <span data-ttu-id="ca5c1-814">Обновление до пакета SDK для пакетной службы версии 4.0.0</span><span class="sxs-lookup"><span data-stu-id="ca5c1-814">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="ca5c1-815">Обновлен параметр `--image` для команды VirtualMachineConfiguration, обеспечивающий поддержку ссылок на образы ARM в дополнение к publish:offer:sku:version.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-815">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="ca5c1-816">Добавлена поддержка новой модели расширений CLI для команд расширений пакетной службы.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-816">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="ca5c1-817">Удалена поддержка пакетной службы для модели компонентов.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-817">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="ca5c1-818">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="ca5c1-818">Batchai</span></span>

* <span data-ttu-id="ca5c1-819">Исходный выпуск модуля искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="ca5c1-819">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="ca5c1-820">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="ca5c1-820">Keyvault</span></span>

* <span data-ttu-id="ca5c1-821">Исправлена проблема с аутентификацией Key Vault при использовании ADFS в Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-821">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="ca5c1-822">(#4448)</span><span class="sxs-lookup"><span data-stu-id="ca5c1-822">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="ca5c1-823">Сеть</span><span class="sxs-lookup"><span data-stu-id="ca5c1-823">Network</span></span>

* <span data-ttu-id="ca5c1-824">Аргумент `--server` для `application-gateway address-pool create` изменен на необязательный (разрешено использование пустых пулов адресов).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-824">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="ca5c1-825">Обновлен элемент `traffic-manager` для поддержки последних функций.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-825">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="ca5c1-826">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ca5c1-826">Resource</span></span>

* <span data-ttu-id="ca5c1-827">Добавлена поддержка параметров `--resource-group/-g` для изменения имени группы ресурсов на `group`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-827">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="ca5c1-828">Добавлены команды для `account lock` для работы с блокировками на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-828">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="ca5c1-829">Добавлены команды для `group lock` для работы с блокировками на уровне группы.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-829">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="ca5c1-830">Добавлены команды для `resource lock` для работы с блокировками на уровне ресурса.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-830">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="ca5c1-831">SQL</span><span class="sxs-lookup"><span data-stu-id="ca5c1-831">Sql</span></span>

* <span data-ttu-id="ca5c1-832">Добавлена поддержка SQL TDE и BYOK TDE.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-832">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="ca5c1-833">Добавлена команда `db list-deleted` и параметр `db restore --deleted-time` для поиска и восстановления удаленных баз данных.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-833">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="ca5c1-834">Добавлено `db op list` и `db op cancel` для отображения и отмены выполняющихся операций в базе данных.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-834">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="ca5c1-835">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="ca5c1-835">Storage</span></span>

* <span data-ttu-id="ca5c1-836">Добавлена поддержка моментальных снимков файловых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-836">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="ca5c1-837">Виртуальные машины</span><span class="sxs-lookup"><span data-stu-id="ca5c1-837">Vm</span></span>

* <span data-ttu-id="ca5c1-838">Исправлена ошибка в команде `vm show`, когда использование `-d` вызывало сбой отсутствующих частных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-838">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="ca5c1-839">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка последовательного обновления для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-839">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="ca5c1-840">Добавлена поддержка обновления параметров шифрования с помощью команды `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-840">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="ca5c1-841">Добавлен параметр `--os-disk-size-gb` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-841">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="ca5c1-842">Добавлен параметр `--license-type` для команды `vmss create` (для Windows).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-842">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="ca5c1-843">22 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-843">September 22, 2017</span></span>

<span data-ttu-id="ca5c1-844">Версия 2.0.18</span><span class="sxs-lookup"><span data-stu-id="ca5c1-844">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="ca5c1-845">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ca5c1-845">Resource</span></span>

* <span data-ttu-id="ca5c1-846">Добавлена поддержка отображения определений встроенных политик</span><span class="sxs-lookup"><span data-stu-id="ca5c1-846">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="ca5c1-847">Добавлена поддержка параметра mode для создания определения политик</span><span class="sxs-lookup"><span data-stu-id="ca5c1-847">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="ca5c1-848">Добавлена поддержка шаблонов и определений пользовательского интерфейса для команды `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="ca5c1-848">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="ca5c1-849">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен тип ресурса `managedapp` с `appliances` на `applications` и с `applianceDefinitions` на `applicationDefinitions`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-849">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="ca5c1-850">Сеть</span><span class="sxs-lookup"><span data-stu-id="ca5c1-850">Network</span></span>

* <span data-ttu-id="ca5c1-851">Добавлена поддержка зоны доступности для подкоманд `network lb` и `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="ca5c1-851">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="ca5c1-852">Добавлена поддержка IPv6 (пиринг Майкрософт) для `express-route`</span><span class="sxs-lookup"><span data-stu-id="ca5c1-852">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="ca5c1-853">Добавлены команды группы безопасности приложения `asg`</span><span class="sxs-lookup"><span data-stu-id="ca5c1-853">Added `asg` application security group commands</span></span>
* <span data-ttu-id="ca5c1-854">Добавлен аргумент `--application-security-groups` для команды `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="ca5c1-854">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="ca5c1-855">Добавлены аргументы `--source-asgs` и `--destination-asgs` для команды `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="ca5c1-855">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="ca5c1-856">Добавлены аргументы `--ddos-protection` и `--vm-protection` для команды `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="ca5c1-856">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="ca5c1-857">Добавлены команды `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-857">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="ca5c1-858">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="ca5c1-858">Storage</span></span>

* <span data-ttu-id="ca5c1-859">Исправлена проблема, когда команды `storage account network-rule` могут не работать после обновления пакета SDK</span><span class="sxs-lookup"><span data-stu-id="ca5c1-859">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="ca5c1-860">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="ca5c1-860">Eventgrid</span></span>

* <span data-ttu-id="ca5c1-861">Обновлен пакет SDK Python для службы "Сетка событий Azure" для использования новой версии API 2017-09-15-preview</span><span class="sxs-lookup"><span data-stu-id="ca5c1-861">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="ca5c1-862">SQL</span><span class="sxs-lookup"><span data-stu-id="ca5c1-862">SQL</span></span>

* <span data-ttu-id="ca5c1-863">Аргумент `--resource-group` для команды `sql server list` сделан необязательным.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-863">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="ca5c1-864">Если он не указан, возвращаются все серверы SQL Server в подписке</span><span class="sxs-lookup"><span data-stu-id="ca5c1-864">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="ca5c1-865">Добавлен параметр `--no-wait` для команд `db [create|copy|restore|update|replica create|create|update]` и `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="ca5c1-865">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="ca5c1-866">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="ca5c1-866">Keyvault</span></span>

* <span data-ttu-id="ca5c1-867">Добавлена поддержка команд хранилища ключей за прокси-сервером</span><span class="sxs-lookup"><span data-stu-id="ca5c1-867">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="ca5c1-868">ВМ</span><span class="sxs-lookup"><span data-stu-id="ca5c1-868">VM</span></span>

* <span data-ttu-id="ca5c1-869">Добавлена поддержка зоны доступности для команды `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="ca5c1-869">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="ca5c1-870">Исправлена проблема, когда использование аргумента `--app-gateway ID` с командой `vmss create` приводило к сбою</span><span class="sxs-lookup"><span data-stu-id="ca5c1-870">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="ca5c1-871">Добавлен аргумент `--asgs` для команды `vm create`</span><span class="sxs-lookup"><span data-stu-id="ca5c1-871">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="ca5c1-872">Добавлена поддержка выполнения команд на виртуальных машинах с помощью команды `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="ca5c1-872">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="ca5c1-873">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка шифрования диска VMSS с помощью команды `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="ca5c1-873">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="ca5c1-874">Добавлена поддержка обслуживания виртуальных машин с помощью команды `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="ca5c1-874">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="ca5c1-875">ACS</span><span class="sxs-lookup"><span data-stu-id="ca5c1-875">ACS</span></span>

* <span data-ttu-id="ca5c1-876">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлен аргумент `--orchestrator-release` для команды `acs create` для регионов служб ACS (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="ca5c1-876">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="ca5c1-877">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ca5c1-877">Appservice</span></span>

* <span data-ttu-id="ca5c1-878">Добавлена возможность обновлять и отображать параметры аутентификации с помощью команды `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="ca5c1-878">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="ca5c1-879">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="ca5c1-879">Backup</span></span>

* <span data-ttu-id="ca5c1-880">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-880">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="ca5c1-881">11 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-881">September 11, 2017</span></span>

<span data-ttu-id="ca5c1-882">Версия 2.0.17</span><span class="sxs-lookup"><span data-stu-id="ca5c1-882">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="ca5c1-883">Core</span><span class="sxs-lookup"><span data-stu-id="ca5c1-883">Core</span></span>

* <span data-ttu-id="ca5c1-884">Включен командный модуль для настройки собственного идентификатора корреляции в телеметрии.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-884">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="ca5c1-885">Исправлена проблема с дампом JSON, когда для телеметрии настроен режим диагностики.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-885">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="ca5c1-886">ACS</span><span class="sxs-lookup"><span data-stu-id="ca5c1-886">Acs</span></span>

* <span data-ttu-id="ca5c1-887">Добавлена команда `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-887">Added `acs list-locations` command</span></span>
* <span data-ttu-id="ca5c1-888">Для `ssh-key-file` предоставляется ожидаемое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-888">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="ca5c1-889">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ca5c1-889">Appservice</span></span>

* <span data-ttu-id="ca5c1-890">Добавлена возможность создавать веб-приложения в группе ресурсов в рамках плана службы, отличной от активной.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-890">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="ca5c1-891">CDN</span><span class="sxs-lookup"><span data-stu-id="ca5c1-891">CDN</span></span>

* <span data-ttu-id="ca5c1-892">Исправлена ошибка "CustomDomain не пригоден к итерации" для `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-892">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="ca5c1-893">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="ca5c1-893">Extension</span></span>

* <span data-ttu-id="ca5c1-894">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="ca5c1-894">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="ca5c1-895">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="ca5c1-895">Keyvault</span></span>

* <span data-ttu-id="ca5c1-896">Исправлена проблема с зависимостью разрешений от регистра для `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-896">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="ca5c1-897">Сеть</span><span class="sxs-lookup"><span data-stu-id="ca5c1-897">Network</span></span>

* <span data-ttu-id="ca5c1-898">Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-898">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="ca5c1-899">Аргумент `--private-access-services` переименован в `--service-endpoints` для команды `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-899">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="ca5c1-900">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-900">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="ca5c1-901">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-901">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="ca5c1-902">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-902">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="ca5c1-903">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ca5c1-903">Resource</span></span>

* <span data-ttu-id="ca5c1-904">Разрешена передача в определениях параметров политики ресурсов в командах `policy definition create` и `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-904">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="ca5c1-905">Разрешена передача значений параметров для команды `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-905">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="ca5c1-906">Разрешена передача JSON или файла для всех параметров.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-906">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="ca5c1-907">Версия API изменена на более позднюю.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-907">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="ca5c1-908">SQL</span><span class="sxs-lookup"><span data-stu-id="ca5c1-908">SQL</span></span>

* <span data-ttu-id="ca5c1-909">Добавлены команды `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-909">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="ca5c1-910">ВМ</span><span class="sxs-lookup"><span data-stu-id="ca5c1-910">VM</span></span>

* <span data-ttu-id="ca5c1-911">Исправлено: не назначать доступ, если `--scope` не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-911">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="ca5c1-912">Исправлено: использование тех же расширений имен, что и для портала.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-912">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="ca5c1-913">Удалено `subscription` из выходных данных `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-913">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="ca5c1-914">Исправлено: номер SKU хранилища `[vm|vmss] create` неприменим для дисков данных с образом.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-914">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="ca5c1-915">Исправлено: `vm format-secret --secrets` не принимает идентификаторы, разделенные строками.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-915">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="ca5c1-916">31 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-916">August 31, 2017</span></span>

<span data-ttu-id="ca5c1-917">Версия 2.0.16</span><span class="sxs-lookup"><span data-stu-id="ca5c1-917">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="ca5c1-918">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="ca5c1-918">Keyvault</span></span>

* <span data-ttu-id="ca5c1-919">Исправлена ошибка при попытке автоматически разрешить шифрование секрета с помощью `secret download`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-919">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="ca5c1-920">Sf</span><span class="sxs-lookup"><span data-stu-id="ca5c1-920">Sf</span></span>

* <span data-ttu-id="ca5c1-921">Объявлены неподдерживаемыми все команды; вместо них используется Service Fabric CLI (sfctl).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-921">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="ca5c1-922">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="ca5c1-922">Storage</span></span>

* <span data-ttu-id="ca5c1-923">Исправлена проблема, когда учетные записи хранения нельзя было создавать в регионах, которые не поддерживают функцию NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-923">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="ca5c1-924">Определение типа и кодировки содержимого во время передачи больших двоичных объектов и файла, если оба свойства не указаны.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-924">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="ca5c1-925">28 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-925">August 28, 2017</span></span>

<span data-ttu-id="ca5c1-926">Версия 2.0.15</span><span class="sxs-lookup"><span data-stu-id="ca5c1-926">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="ca5c1-927">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="ca5c1-927">CLI</span></span>

* <span data-ttu-id="ca5c1-928">Для `--version` добавлено юридическое примечание.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-928">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="ca5c1-929">ACS</span><span class="sxs-lookup"><span data-stu-id="ca5c1-929">ACS</span></span>

* <span data-ttu-id="ca5c1-930">Исправлены регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-930">Corrected preview regions</span></span>
* <span data-ttu-id="ca5c1-931">Правильно отформатирован параметр по умолчанию `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-931">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="ca5c1-932">Оптимизированы выходные данные команды ACS.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-932">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="ca5c1-933">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ca5c1-933">Appservice</span></span>

* <span data-ttu-id="ca5c1-934">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправлены несоответствия в выходных данных `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-934">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="ca5c1-935">Добавлен новый псевдоним `-i` в команду `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-935">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="ca5c1-936">Предоставлена команда `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-936">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="ca5c1-937">Предоставлены новые аргументы команды `az webapp delete`, которые позволяют сохранить план службы приложений, метрики и данные регистрации DNS.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-937">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="ca5c1-938">Исправление. Параметры слота определяются правильно.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-938">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="ca5c1-939">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="ca5c1-939">IoT</span></span>

* <span data-ttu-id="ca5c1-940">Исправление 3934. При создании политики существующие политики больше не удаляются.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-940">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="ca5c1-941">Сеть</span><span class="sxs-lookup"><span data-stu-id="ca5c1-941">Network</span></span>

* <span data-ttu-id="ca5c1-942">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-942">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="ca5c1-943">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--private-access-services` переименован в `--service-endpoints` в командах `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-943">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="ca5c1-944">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-944">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="ca5c1-945">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-945">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="ca5c1-946">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-946">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="ca5c1-947">Профиль</span><span class="sxs-lookup"><span data-stu-id="ca5c1-947">Profile</span></span>

* <span data-ttu-id="ca5c1-948">Предоставлены параметры `--msi` и `--msi-port` для входа с использованием удостоверения виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-948">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="ca5c1-949">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="ca5c1-949">Service Fabric</span></span>

* <span data-ttu-id="ca5c1-950">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-950">Preview release</span></span>
* <span data-ttu-id="ca5c1-951">Упрощены правила реестра для паролей и имен пользователя для команды.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-951">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="ca5c1-952">Исправлена строка для ввода пароля пользователем даже после передачи параметра.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-952">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="ca5c1-953">Добавлена поддержка пустого значения `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-953">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="ca5c1-954">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="ca5c1-954">Storage</span></span>

* <span data-ttu-id="ca5c1-955">Появилась возможность задавать уровень большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-955">Enabled setting blob tier</span></span>
* <span data-ttu-id="ca5c1-956">Добавлены аргументы `--bypass` и `--default-action` в командах `storage account [create|update]` для поддержки туннелирования службы.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-956">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="ca5c1-957">Добавлены команды для добавления правил виртуальной сети и правил на основе IP-адресов в `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-957">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="ca5c1-958">Разрешено шифрование службы с управляемым пользователем ключом.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-958">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="ca5c1-959">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--encryption` переименован в `--encryption-services` в команде `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-959">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="ca5c1-960">Исправление 4220. Несоответствие синтаксиса `az storage account update encryption`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-960">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="ca5c1-961">ВМ</span><span class="sxs-lookup"><span data-stu-id="ca5c1-961">VM</span></span>

* <span data-ttu-id="ca5c1-962">Исправлена проблема, из-за которой для команды `vmss get-instance-view` отображались лишние и неправильные сведения при использовании параметра `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-962">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="ca5c1-963">Добавлена поддержка параметра `--lb-sku` в команде `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-963">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="ca5c1-964">Из черного списка имен администраторов для команд `[vm|vmss] create` удалены имена людей.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-964">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="ca5c1-965">Исправлена проблема, из-за которой команда `[vm|vmss] create` выдавала ошибку, если из образа не удавалось извлечь сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-965">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="ca5c1-966">Исправлена проблема, которая приводила к сбою при создании масштабируемого набора виртуальных машин с внутренней подсистемой балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-966">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="ca5c1-967">Исправлена проблема, из-за которой аргумент `--no-wait` не работал с командой `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-967">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="ca5c1-968">15 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-968">August 15, 2017</span></span>

<span data-ttu-id="ca5c1-969">Версия 2.0.14</span><span class="sxs-lookup"><span data-stu-id="ca5c1-969">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="ca5c1-970">ACS</span><span class="sxs-lookup"><span data-stu-id="ca5c1-970">ACS</span></span>

* <span data-ttu-id="ca5c1-971">Исправлен номер порта sshMaster0 для Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-971">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="ca5c1-972">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ca5c1-972">Appservice</span></span>

* <span data-ttu-id="ca5c1-973">Исправлено исключение при создании веб-приложения Linux на основе Git.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-973">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="ca5c1-974">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="ca5c1-974">Event Grid</span></span>

* <span data-ttu-id="ca5c1-975">Добавлены зависимости пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-975">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="ca5c1-976">11 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-976">August 11, 2017</span></span>

<span data-ttu-id="ca5c1-977">Версия 2.0.13</span><span class="sxs-lookup"><span data-stu-id="ca5c1-977">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="ca5c1-978">ACS</span><span class="sxs-lookup"><span data-stu-id="ca5c1-978">ACS</span></span>

* <span data-ttu-id="ca5c1-979">Добавлены дополнительные регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-979">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="ca5c1-980">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="ca5c1-980">Batch</span></span>

* <span data-ttu-id="ca5c1-981">Пакет SDK для пакетной службы обновлен до версии 3.1.0, а пакет SDK для управления пакетной службой — до версии 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-981">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="ca5c1-982">Добавлена новая команда для отображения количества задач в задании.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-982">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="ca5c1-983">Исправлена ошибка при обработке URL-адреса SAS файла ресурсов.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-983">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="ca5c1-984">Для конечной точки учетной записи пакетной службы теперь поддерживается дополнительный префикс https://.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-984">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="ca5c1-985">Поддерживается добавление к заданию списков, содержащих более 100 задач.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-985">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="ca5c1-986">Добавлено ведение журнала отладки при загрузке командного модуля расширений.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-986">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="ca5c1-987">Компонент</span><span class="sxs-lookup"><span data-stu-id="ca5c1-987">Component</span></span>

* <span data-ttu-id="ca5c1-988">Добавлено предупреждение о прекращении поддержки в команды az component.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-988">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="ca5c1-989">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ca5c1-989">Container</span></span>

* <span data-ttu-id="ca5c1-990">`create`. Исправлена проблема, из-за которой запрещалось использовать знак равенства в переменной среды.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-990">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="ca5c1-991">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="ca5c1-991">Data Lake Store</span></span>

* <span data-ttu-id="ca5c1-992">Включен индикатор хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-992">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="ca5c1-993">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="ca5c1-993">Event Grid</span></span>

* <span data-ttu-id="ca5c1-994">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="ca5c1-994">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="ca5c1-995">Сеть</span><span class="sxs-lookup"><span data-stu-id="ca5c1-995">Network</span></span>

* <span data-ttu-id="ca5c1-996">`lb`. Исправлена проблема, из-за которой некоторые имена дочерних ресурсов не разрешались правильно, если не были указаны.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-996">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="ca5c1-997">`application-gateway {subresource} delete`. Исправлена проблема, из-за которой не учитывался параметр `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-997">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="ca5c1-998">`application-gateway http-settings update`. Исправлена проблема, из-за которой не удавалось отключить параметр `--connection-draining-timeout`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-998">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="ca5c1-999">Исправлена проблема с непредвиденным аргументом ключевого слова `sa_data_size_kilobyes` при использовании с командой `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-999">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="ca5c1-1000">Профиль</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1000">Profile</span></span>

* <span data-ttu-id="ca5c1-1001">`account list`. Добавлен параметр `--refresh` для синхронизации последних подписок с сервером.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1001">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="ca5c1-1002">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1002">Storage</span></span>

* <span data-ttu-id="ca5c1-1003">Включено обновление учетной записи хранения с помощью удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1003">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="ca5c1-1004">ВМ</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1004">VM</span></span>

* <span data-ttu-id="ca5c1-1005">`availability-set`. Предоставлено число доменов сбоя при преобразовании.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1005">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="ca5c1-1006">Предоставлена команда `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1006">Exposed `list-skus` command</span></span>
* <span data-ttu-id="ca5c1-1007">Поддерживается назначение удостоверений без создания назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1007">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="ca5c1-1008">При подключении дисков данных применяется номер SKU хранилища.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1008">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="ca5c1-1009">Удалено используемое по умолчанию имя диска ОС и номер SKU хранилища при использовании управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1009">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="ca5c1-1010">28 июля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1010">July 28, 2017</span></span>

<span data-ttu-id="ca5c1-1011">Версия 2.0.12</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1011">Version 2.0.12</span></span>

* <span data-ttu-id="ca5c1-1012">Добавлены команды для контейнеров.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1012">Added container commands</span></span>
* <span data-ttu-id="ca5c1-1013">Добавлены модули выставления счетов и потребления ресурсов.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1013">Added billing and consumption modules</span></span>

```text
azure-cli (2.0.12)

acr (2.0.9)
acs (2.0.11)
appservice (0.1.11)
batch (3.0.3)
billing (0.1.3)
cdn (0.0.6)
cloud (2.0.7)
cognitiveservices (0.1.6)
command-modules-nspkg (2.0.1)
component (2.0.6)
configure (2.0.10)
consumption (0.1.3)
container (0.1.7)
core (2.0.12)
cosmosdb (0.1.11)
dla (0.0.10)
dls (0.0.11)
feedback (2.0.6)
find (0.2.6)
interactive (0.3.7)
iot (0.1.10)
keyvault (2.0.8)
lab (0.0.9)
monitor (0.0.8)
network (2.0.11)
nspkg (3.0.1)
profile (2.0.9)
rdbms (0.0.5)
redis (0.2.7)
resource (2.0.11)
role (2.0.9)
sf (1.0.5)
sql (2.0.8)
storage (2.0.11)
vm (2.0.11)
```

### <a name="core"></a><span data-ttu-id="ca5c1-1014">Core</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1014">Core</span></span>

* <span data-ttu-id="ca5c1-1015">Вывод сведений о пакетах SDK для проверки подлинности субъектов-служб с помощью сертификатов.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1015">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="ca5c1-1016">Исправлены исключения в ходе выполнения развертывания.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1016">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="ca5c1-1017">Для создания клиента подписки используется конечная точка ARM текущего облака.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1017">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="ca5c1-1018">Улучшена параллельная обработка файла clouds.config (3636).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1018">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="ca5c1-1019">Обновление идентификатора клиентского запроса при каждом выполнении команды.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1019">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="ca5c1-1020">Создание клиентов подписки с правильным профилем SDK (3635).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1020">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="ca5c1-1021">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1021">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="ca5c1-1022">Добавлена поддержка выбора полей вывода в таблице с помощью запроса jmespath (3581).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1022">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="ca5c1-1023">Улучшено отключение аргументов анализа и добавлено ведение журналов с помощью жестов (3434).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1023">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="ca5c1-1024">Создание клиентов подписки с правильным профилем SDK.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1024">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="ca5c1-1025">Перемещение всех существующих файлов записи в последнюю папку.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1025">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="ca5c1-1026">Исправлена идемпотентность при создании виртуальной машины или масштабируемого набора виртуальных машин (3586).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1026">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="ca5c1-1027">В путях команд больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1027">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="ca5c1-1028">В определенных параметрах логического типа больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1028">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="ca5c1-1029">Поддержка входа на локальный сервер AD FS, например Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1029">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="ca5c1-1030">Исправлена параллельная запись в файл clouds.config (3255).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1030">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="ca5c1-1031">ACR</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1031">ACR</span></span>

* <span data-ttu-id="ca5c1-1032">Добавлена команда `show-usage` для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1032">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="ca5c1-1033">Поддержка обновления номера SKU для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1033">Support SKU update for managed registries</span></span>
* <span data-ttu-id="ca5c1-1034">Добавлены управляемые реестры с управляемыми номерами SKU.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1034">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="ca5c1-1035">Добавлены веб-перехватчики для управляемых реестров с использованием модуля для команды acr webhook.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1035">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="ca5c1-1036">Добавлена проверка подлинности с помощью AAD с использованием команды acr login.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1036">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="ca5c1-1037">Добавлена команда delete для репозиториев, манифестов и тегов Docker.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1037">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="ca5c1-1038">ACS</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1038">ACS</span></span>

* <span data-ttu-id="ca5c1-1039">Поддержка API версии 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1039">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="ca5c1-1040">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1040">Appservice</span></span>

* <span data-ttu-id="ca5c1-1041">Исправлена ошибка, из-за которой команда вывода списка в веб-приложениях Linux не возвращала данные.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1041">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="ca5c1-1042">Поддержка извлечения учетных данных из ACR.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1042">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="ca5c1-1043">Удаление всех команд группы `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1043">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="ca5c1-1044">Создание масок паролей для реестров Docker из выходных данных команды (3656).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1044">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="ca5c1-1045">Обеспечено использование браузера по умолчанию в macOS без ошибок (3623).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1045">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="ca5c1-1046">Улучшена справка по командам `webapp log tail` и `webapp log download` (3624).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1046">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="ca5c1-1047">Предоставлена команда `traffic-routing` для настройки статической маршрутизации (3566).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1047">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="ca5c1-1048">Добавлены исправления, связанные с надежностью, при настройке системы управления версиями (3245).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1048">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="ca5c1-1049">Удален неподдерживаемый аргумент `--node-version` из функции `webapp config update` для веб-приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1049">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="ca5c1-1050">Вместо него используется `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1050">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="ca5c1-1051">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1051">Batch</span></span>

* <span data-ttu-id="ca5c1-1052">Пакеты SDK для пакетной службы обновлены до версии 3.0.0 с поддержкой низкоприоритетных виртуальных машин в пулах.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1052">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="ca5c1-1053">Параметр команды `pool create` переименован с `--target-dedicated` в `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1053">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="ca5c1-1054">Для команды `pool create` добавлены параметры `--target-low-priority-nodes` и `--application-licenses`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1054">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="ca5c1-1055">CDN</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1055">CDN</span></span>

* <span data-ttu-id="ca5c1-1056">Предоставлено улучшенное сообщение об ошибке для команды `cdn endpoint list`, которое отображается, если заданный параметром `--profile-name` профиль не существует.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1056">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="ca5c1-1057">Облако</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1057">Cloud</span></span>

* <span data-ttu-id="ca5c1-1058">Формат версии API конечной точки метаданных облака изменен на следующий: ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1058">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="ca5c1-1059">Конечная точка коллекции не является обязательной.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1059">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="ca5c1-1060">Поддерживается регистрация облака только с конечной точкой диспетчера ARM.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1060">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="ca5c1-1061">Предоставлен параметр в команде `cloud set` для выбора профиля при выборе текущего облака.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1061">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="ca5c1-1062">Предоставлен параметр `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1062">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="ca5c1-1063">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1063">CosmosDB</span></span>

* <span data-ttu-id="ca5c1-1064">Внесены исправления, которые позволяют создавать коллекцию с пользовательским ключом секции.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1064">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="ca5c1-1065">Добавлена поддержка срока жизни по умолчанию для коллекции.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1065">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="ca5c1-1066">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1066">Data Lake Analytics</span></span>

* <span data-ttu-id="ca5c1-1067">Добавлены команды для управления политикой вычислений в разделе `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1067">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="ca5c1-1068">Добавлена команда `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1068">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="ca5c1-1069">Добавлена команда `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1069">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="ca5c1-1070">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1070">Data Lake Store</span></span>

* <span data-ttu-id="ca5c1-1071">Добавлена поддержка смены ключей пользовательского хранилища ключей в `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1071">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="ca5c1-1072">Обновлена версия пакета SDK для базовой файловой системы Data Lake Store из-за проблем с производительностью.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1072">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="ca5c1-1073">Добавлена команда `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1073">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="ca5c1-1074">Эта команда пытается активировать пользовательское хранилище ключей, предназначенное для шифрования данных в учетной записи Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1074">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="ca5c1-1075">Интерактивный режим</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1075">Interactive</span></span>

* <span data-ttu-id="ca5c1-1076">Улучшено время запуска с помощью кэшированных команд.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1076">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="ca5c1-1077">Увеличено тестовое покрытие.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1077">Increased test coverage</span></span>
* <span data-ttu-id="ca5c1-1078">Расширены возможности жеста "?", которые позволяют также вставить его в следующую команду.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1078">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="ca5c1-1079">Исправлены ошибки с интерактивными функциями в предварительной версии профиля 2017-03-09 (3587).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1079">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="ca5c1-1080">Разрешено использовать `--version` в качестве параметра в интерактивном режиме (3645).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1080">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="ca5c1-1081">В интерактивном режиме больше не возникают ошибки при выполнении проверки (3570).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1081">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="ca5c1-1082">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1082">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="ca5c1-1083">Добавлен флаг `--progress`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1083">Added `--progress` flag</span></span>
* <span data-ttu-id="ca5c1-1084">Из вариантов завершения удалены `--debug` и `--verbose`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1084">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="ca5c1-1085">Из вариантов завершения удален `interactive` (3324).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1085">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="ca5c1-1086">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1086">IoT</span></span>

* <span data-ttu-id="ca5c1-1087">Исправлено. При создании политики больше не удаляются существующие политики</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1087">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="ca5c1-1088">(3934).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1088">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="ca5c1-1089">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1089">Key vault</span></span>

* <span data-ttu-id="ca5c1-1090">Добавлены команды для функций восстановления хранилища ключей:</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1090">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="ca5c1-1091">`keyvault`, подкоманды `purge`, `recover` и `keyvault list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1091">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="ca5c1-1092">`keyvault secret`, подкоманды `backup`, `restore`, `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1092">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="ca5c1-1093">`keyvault certificate`, подкоманды `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1093">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="ca5c1-1094">`keyvault key`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1094">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="ca5c1-1095">Добавлена интеграция хранилища ключей с субъектом-службой (3133).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1095">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="ca5c1-1096">Обновлена плоскость данных хранилища ключей до версии 0.3.2</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1096">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="ca5c1-1097">(3307).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1097">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="ca5c1-1098">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1098">Lab</span></span>

* <span data-ttu-id="ca5c1-1099">Добавлена поддержка запросов ко всем виртуальным машинам в лаборатории с помощью `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1099">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="ca5c1-1100">Добавлен модуль форматирования табличных выходных данных команд `az lab vm list` и `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1100">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="ca5c1-1101">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1101">Monitor</span></span>

* <span data-ttu-id="ca5c1-1102">Исправлены ошибки с файлом шаблона с помощью команды `monitor autoscale-settings get-parameters-template` (3349).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1102">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="ca5c1-1103">Команда `monitor alert-rule-incidents list` переименована в `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1103">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="ca5c1-1104">Команда `monitor alert-rule-incidents show` переименована в `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1104">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="ca5c1-1105">Команда `monitor metric-defintions list` переименована в `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1105">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="ca5c1-1106">Команда `monitor alert-rules` переименована в `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1106">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="ca5c1-1107">В команду `monitor alert create` внесены следующие изменения:</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1107">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="ca5c1-1108">подкоманды `condition` и `action` больше не принимают данные JSON;</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1108">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="ca5c1-1109">добавлены различные параметры, которые упрощают процесс создания правила;</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1109">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="ca5c1-1110">параметр `location` больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1110">`location` no longer required</span></span>
  * <span data-ttu-id="ca5c1-1111">добавлена поддержка имени и идентификатора для целевого объекта;</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1111">Add name and ID support for target</span></span>
  * <span data-ttu-id="ca5c1-1112">удален параметр `--alert-rule-resource-name`;</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1112">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="ca5c1-1113">параметр `is-enabled` переименован в `enabled`, он больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1113">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="ca5c1-1114">значения по умолчанию для `description` теперь основаны на указанном условии;</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1114">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="ca5c1-1115">добавлены примеры, в которых подробно представлен новый формат.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1115">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="ca5c1-1116">Поддержка имен или идентификаторов для команд `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1116">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="ca5c1-1117">Добавлены вспомогательные аргументы и примеры использования команды `monitor alert rule update`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1117">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="ca5c1-1118">Сеть</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1118">Network</span></span>

* <span data-ttu-id="ca5c1-1119">Добавлена команда `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1119">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="ca5c1-1120">Добавлен аргумент `--private-access-services` в команды `vnet subnet create` и `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1120">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="ca5c1-1121">Исправлена проблема, из-за которой команда `application-gateway redirect-config create` завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1121">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="ca5c1-1122">Исправлена проблема, из-за которой команда `application-gateway redirect-config update` не работала с параметром `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1122">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="ca5c1-1123">Исправлена ошибка при использовании аргумента `--servers` с командами `application-gateway address-pool create` и `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1123">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="ca5c1-1124">Добавлены команды `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1124">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="ca5c1-1125">В команду `application-gateway ssl-policy` добавлены подкоманды `list-options`, `predefined list` и `predefined show`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1125">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="ca5c1-1126">В команду `application-gateway ssl-policy set` добавлены аргументы `--name`, `--cipher-suites` и `--min-protocol-version`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1126">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="ca5c1-1127">В команды `application-gateway http-settings create` и `application-gateway http-settings update` добавлены аргументы `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe` и `--path`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1127">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="ca5c1-1128">В команды `application-gateway url-path-map create` и `application-gateway url-path-map update` добавлены аргументы `--default-redirect-config` и `--redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1128">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="ca5c1-1129">Добавлен аргумент `--redirect-config` в команду `application-gateway url-path-map rule create`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1129">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="ca5c1-1130">Добавлена поддержка параметра `--no-wait` в команде `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1130">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="ca5c1-1131">В команды `application-gateway probe create` и `application-gateway probe update` добавлены аргументы `--host-name-from-http-settings`, `--min-servers`, `--match-body` и `--match-status-codes`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1131">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="ca5c1-1132">Добавлен аргумент `--redirect-config` в команды `application-gateway rule create` и `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1132">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="ca5c1-1133">Добавлена поддержка аргумента `--accelerated-networking` в командах `nic create` и `nic update`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1133">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="ca5c1-1134">Удален аргумент `--internal-dns-name-suffix` из команды `nic create`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1134">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="ca5c1-1135">Добавлена поддержка параметра `--dns-servers` в командах `nic update` и `nic create`. Добавлена поддержка параметра --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1135">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="ca5c1-1136">Исправлена ошибка, из-за которой команда `local-gateway create` игнорировала параметр `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1136">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="ca5c1-1137">Добавлена поддержка параметра `--dns-servers` в команде `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1137">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="ca5c1-1138">Исправлена ошибка при создании пиринга без фильтрации маршрутов с помощью команды `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1138">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="ca5c1-1139">Исправлена ошибка, из-за которой аргументы `--provider` и `--bandwidth` не работали с командой `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1139">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="ca5c1-1140">Исправлена ошибка с логикой установки значений по умолчанию в команде `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1140">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="ca5c1-1141">Улучшено форматирование выходных данных команды `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1141">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="ca5c1-1142">В команде `application-gateway http-listener create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1142">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="ca5c1-1143">В команде `application-gateway rule create` используются пул адресов, параметры HTTP и прослушиватель HTTP по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1143">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="ca5c1-1144">В команде `lb rule create` используются интерфейсный IP-адрес и серверный пул по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1144">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="ca5c1-1145">В команде `lb inbound-nat-rule create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1145">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="ca5c1-1146">Профиль</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1146">Profile</span></span>

* <span data-ttu-id="ca5c1-1147">Поддержка входа на виртуальную машину с использованием управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1147">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="ca5c1-1148">Поддержка вывода данных команды `account show` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1148">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="ca5c1-1149">При использовании параметра --expanded-view отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1149">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="ca5c1-1150">Добавлена команда `get-access-token` для предоставления необработанного токена AAD.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1150">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="ca5c1-1151">Поддержка входа с учетной записью пользователя без связанных подписок.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1151">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="ca5c1-1152">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1152">RDBMS</span></span>

* <span data-ttu-id="ca5c1-1153">Поддержка вывода списка серверов в подписке (3417).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1153">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="ca5c1-1154">Исправлена проблема, когда объект `%s` не обрабатывался из-за отсутствия `% server_type` (3393).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1154">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="ca5c1-1155">Исправлено сопоставление источника документа и добавлена задача непрерывной интеграции для проверки (3361).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1155">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="ca5c1-1156">Исправлена справка по MySQL и PostgreSQL (3369).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1156">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="ca5c1-1157">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1157">Resource</span></span>

* <span data-ttu-id="ca5c1-1158">Улучшены запросы на ввод отсутствующих параметров для команды `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1158">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="ca5c1-1159">Улучшен анализ синтаксиса `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1159">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="ca5c1-1160">Исправлены проблемы, из-за которых файлы параметров `group deployment create` не распознавались с использованием синтаксиса `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1160">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="ca5c1-1161">Поддержка аргумента `--ids` в командах `resource` и `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1161">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="ca5c1-1162">Исправлены некоторые сообщения об ошибках и анализе (3584).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1162">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="ca5c1-1163">Исправлены ошибки анализа параметра `--resource-type` в команде `lock`. Теперь принимаются `<resource-namespace>` и `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1163">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="ca5c1-1164">Добавлена проверка параметров для шаблонов для ссылок на шаблоны (3629).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1164">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="ca5c1-1165">Добавлена поддержка указания параметров развертывания с использованием синтаксиса `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1165">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="ca5c1-1166">Роль</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1166">Role</span></span>

* <span data-ttu-id="ca5c1-1167">Поддержка вывода данных команды `create-for-rbac` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1167">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="ca5c1-1168">Добавлена очистка назначений ролей и связанного приложения AAD при удалении субъекта-службы (3610).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1168">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="ca5c1-1169">В описания аргументов `--start-date` и `--end-date` команды `app create` добавлен формат времени.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1169">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="ca5c1-1170">При использовании параметра `--expanded-view` отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1170">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="ca5c1-1171">Добавлена интеграция хранилища ключей для команд `create-for-rbac` и `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1171">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="ca5c1-1172">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1172">Service Fabric</span></span>
* <span data-ttu-id="ca5c1-1173">Исправлена ошибка, из-за которой большие файлы в приложениях усекались при отправке (3666).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1173">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="ca5c1-1174">Добавлены тесты для команд Service Fabric (3424).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1174">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="ca5c1-1175">Исправлены многие команды Service Fabric (3234).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1175">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="ca5c1-1176">SQL</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1176">SQL</span></span>

* <span data-ttu-id="ca5c1-1177">Удален недействительный параметр `--identity` команды `sql server create`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1177">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="ca5c1-1178">Удалены значения паролей из выходных данных команд `sql server create` и `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1178">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="ca5c1-1179">Добавлены команды `sql db list-editions` и `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1179">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="ca5c1-1180">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1180">Storage</span></span>

* <span data-ttu-id="ca5c1-1181">Удален параметр `--marker` из команд `storage blob list`, `storage container list` и `storage share list` (3745).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1181">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="ca5c1-1182">Включено создание учетных записей хранения с поддержкой только HTTPS.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1182">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="ca5c1-1183">Обновлены метрики хранилища, команды входа и CORS (3495).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1183">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="ca5c1-1184">Перефразировано сообщение об исключении, которое выводит команда добавления CORS (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1184">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="ca5c1-1185">Генератор преобразован в список в режиме пробного выполнения команды пакетной загрузки (3592).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1185">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="ca5c1-1186">Исправлена проблема при пробном выполнении команды пакетной загрузки больших двоичных объектов (3640) (3592).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1186">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="ca5c1-1187">ВМ</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1187">VM</span></span>

* <span data-ttu-id="ca5c1-1188">Поддержка настройки NSG.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1188">Support configuring nsg</span></span>
* <span data-ttu-id="ca5c1-1189">Исправлена ошибка, из-за которой не удавалось правильно настроить DNS-сервер.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1189">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="ca5c1-1190">Поддержка удостоверений управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1190">Support managed service identities</span></span>
* <span data-ttu-id="ca5c1-1191">Исправлена проблема, из-за которой для команды `cmss create` с существующей подсистемой балансировки нагрузки требовался параметр `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1191">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="ca5c1-1192">Теперь нумерация LUN дисков данных, создаваемых с помощью команды `vm image create`, начинается с 0.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1192">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="ca5c1-1193">10 мая 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1193">May 10, 2017</span></span>

<span data-ttu-id="ca5c1-1194">Версия 2.0.6</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1194">Version 2.0.6</span></span>

* <span data-ttu-id="ca5c1-1195">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1195">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="ca5c1-1196">Добавлена реляционная СУБД (MySQL, Postgres).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1196">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="ca5c1-1197">Добавлены модули Data Lake Store и Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1197">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="ca5c1-1198">Добавлен модуль Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1198">Include Cognitive Services module</span></span>
* <span data-ttu-id="ca5c1-1199">Добавлен модуль Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1199">Include Service Fabric module</span></span>
* <span data-ttu-id="ca5c1-1200">Добавлен модуль Interactive (az-shell переименован).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1200">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="ca5c1-1201">Добавлена поддержка команд CDN.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1201">Add support for CDN commands</span></span>
* <span data-ttu-id="ca5c1-1202">Удален модуль Container.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1202">Remove Container module</span></span>
* <span data-ttu-id="ca5c1-1203">Добавлена команда az -v для az --version ([№ 2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1203">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="ca5c1-1204">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1204">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

```text
azure-cli (2.0.6)

acr (2.0.4)
acs (2.0.6)
appservice (0.1.6)
batch (2.0.4)
cdn (0.0.2)
cloud (2.0.2)
cognitiveservices (0.1.2)
command-modules-nspkg (2.0.0)
component (2.0.4)
configure (2.0.6)
core (2.0.6)
cosmosdb (0.1.6)
dla (0.0.6)
dls (0.0.6)
feedback (2.0.2)
find (0.2.2)
interactive (0.3.1)
iot (0.1.5)
keyvault (2.0.4)
lab (0.0.4)
monitor (0.0.4)
network (2.0.6)
nspkg (3.0.0)
profile (2.0.4)
rdbms (0.0.1)
redis (0.2.3)
resource (2.0.6)
role (2.0.4)
sf (1.0.1)
sql (2.0.3)
storage (2.0.6)
vm (2.0.6)
```

### <a name="core"></a><span data-ttu-id="ca5c1-1205">Core</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1205">Core</span></span>

* <span data-ttu-id="ca5c1-1206">Ядро: запись исключений, порожденных незарегистрированным поставщиком, и его автоматическая регистрация.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1206">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="ca5c1-1207">Производительность: сохранение кэша маркеров библиотеки ADAL в памяти до завершения работы процесса ([№ 2603](https://github.com/Azure/azure-cli/issues/2603)).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1207">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="ca5c1-1208">Исправление байтов, возвращаемых из шестнадцатеричных отпечатков -o tsv ([№ 3053](https://github.com/Azure/azure-cli/issues/3053)).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1208">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="ca5c1-1209">Улучшенное скачивание сертификатов Key Vault и интеграция субъектов-служб AAD ([№ 3003](https://github.com/Azure/azure-cli/issues/3003)).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1209">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="ca5c1-1210">Добавление расположения Python в az -version ([№ 2986](https://github.com/Azure/azure-cli/issues/2986)).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1210">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="ca5c1-1211">Вход: поддержка входа при отсутствии подписок ([№ 2929](https://github.com/Azure/azure-cli/issues/2929)).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1211">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="ca5c1-1212">Ядро: устранен сбой при двукратном входе с помощью субъекта-службы ([№ 2800](https://github.com/Azure/azure-cli/issues/2800)).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1212">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="ca5c1-1213">Ядро: возможность настроить путь к файлу accessTokens.json с помощью env var ([№ 2605](https://github.com/Azure/azure-cli/issues/2605)).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1213">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="ca5c1-1214">Ядро: возможность применять настроенные параметры по умолчанию к необязательным аргументам ([№ 2703](https://github.com/Azure/azure-cli/issues/2703)).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1214">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="ca5c1-1215">Ядро: повышение производительности.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1215">core: Improved performance</span></span>
* <span data-ttu-id="ca5c1-1216">Ядро: настаиваемые сертификаты ЦС — поддержка настройки переменной среды REQUESTS_CA_BUNDLE.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1216">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="ca5c1-1217">Ядро: облачная конфигурация — использование конечной точки Resource Manager, если не задана конечная точка управления.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1217">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="ca5c1-1218">ACS</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1218">ACS</span></span>

* <span data-ttu-id="ca5c1-1219">Исправление: теперь значение счетчика баз данных master и агентов — целое число, а не строка.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1219">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="ca5c1-1220">Предоставлены команды az acs create --no-wait и az acs wait для асинхронного создания.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1220">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="ca5c1-1221">Предоставлена команда az acs create --validate для пробного создания.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1221">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="ca5c1-1222">Удален профиль Windows перед вызовом метода PUT для команды scale ([№ 2755](https://github.com/Azure/azure-cli/issues/2755)).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1222">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="ca5c1-1223">AppService</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1223">AppService</span></span>

* <span data-ttu-id="ca5c1-1224">Приложение-функция: добавлена полная поддержка приложений-функций, включая создание, отображение, вывод списка, удаление, настройку имени узла, настройку протокола SSL и т. д.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1224">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="ca5c1-1225">Добавлены службы Team Services (VSTS) в качестве параметра непрерывной доставки в конфигурации веб-системы управления версиями службы приложений.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1225">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="ca5c1-1226">Создана команда az webapp, заменяющая команду az appservice web (для обеспечения обратной совместимости команда az appservice web будет оставлена еще в двух выпусках).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1226">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="ca5c1-1227">Предоставлены аргументы для настройки развертывания и стеков времени выполнения при создании веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1227">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="ca5c1-1228">Предоставлена команда webapp list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1228">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="ca5c1-1229">Поддержка настройки строк подключения ([№ 2647](https://github.com/Azure/azure-cli/issues/2647)).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1229">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="ca5c1-1230">Поддержка переключения слотов с предварительным просмотром.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1230">support slot swap with preview</span></span>
* <span data-ttu-id="ca5c1-1231">Устранены ошибки из команд службы приложений ([№ 2948](https://github.com/Azure/azure-cli/issues/2948)).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1231">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="ca5c1-1232">Использование группы ресурсов в плане служб приложений для операций с сертификатами ([№ 2750](https://github.com/Azure/azure-cli/issues/2750)).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1232">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="ca5c1-1233">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1233">CosmosDB</span></span>

* <span data-ttu-id="ca5c1-1234">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1234">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="ca5c1-1235">Добавлена поддержка интерфейсов API уровня данных DocumentDB: управление базами данных и коллекциями.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1235">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="ca5c1-1236">Добавлена поддержка включения автоматической отработки отказа для учетных записей базы данных.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1236">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="ca5c1-1237">Добавлена поддержка нового параметра ConsistentPrefix политики согласованности.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1237">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="ca5c1-1238">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1238">Data Lake Analytics</span></span>

* <span data-ttu-id="ca5c1-1239">Исправлена ошибка, из-за которой фильтрация списков заданий по результату и состоянию вызывала сбой.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1239">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="ca5c1-1240">Добавлена поддержка нового типа элемента каталога — пакета.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1240">Add support for new catalog item type: package.</span></span> <span data-ttu-id="ca5c1-1241">Для доступа к нему используется `az dla catalog package`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1241">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="ca5c1-1242">Появилась возможность вывести список следующих элементов каталога из базы данных (указание схемы не требуется):</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1242">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="ca5c1-1243">Таблица</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1243">Table</span></span>
  * <span data-ttu-id="ca5c1-1244">функция с табличным значением;</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1244">Table valued function</span></span>
  * <span data-ttu-id="ca5c1-1245">Просмотр</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1245">View</span></span>
  * <span data-ttu-id="ca5c1-1246">статистика таблицы.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1246">Table Statistics.</span></span> <span data-ttu-id="ca5c1-1247">Их можно также вывести с помощью схемы, но без указания имени таблицы.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1247">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="ca5c1-1248">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1248">Data Lake Store</span></span>

* <span data-ttu-id="ca5c1-1249">Обновлена версия пакета SDK базовой файловой системы, что обеспечивает лучшую поддержку сценариев регулирования на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1249">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="ca5c1-1250">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1250">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="ca5c1-1251">Отсутствовала справка для команды access show.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1251">missed help for access show.</span></span> <span data-ttu-id="ca5c1-1252">Теперь она добавлена.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1252">adding it.</span></span> <span data-ttu-id="ca5c1-1253">([№ 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1253">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="ca5c1-1254">Поиск</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1254">Find</span></span>

* <span data-ttu-id="ca5c1-1255">Улучшены результаты поиска и разрешено управление версиями индекса поиска.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1255">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="ca5c1-1256">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1256">KeyVault</span></span>

* <span data-ttu-id="ca5c1-1257">BC: в команде `az keyvault certificate download` параметр -e со строкового или двоичного значения изменен на PEM или DER, чтобы лучше представить параметры.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1257">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="ca5c1-1258">BC: из команды `keyvault certificate create` удалены параметры --expires и --not-before, так как они не поддерживаются службой.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1258">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="ca5c1-1259">В команду `keyvault certificate create` добавлен параметр --validity для выборочного переопределения значение в параметре --policy.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1259">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="ca5c1-1260">Исправлена ошибка в команде `keyvault certificate get-default-policy`, в которой были доступны параметры expires и not_before, а параметр validity_in_months — нет.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1260">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="ca5c1-1261">Добавлено исправление для модуля keyvault для импорта PEM- и PFX-файлов ([№ 2754](https://github.com/Azure/azure-cli/issues/2754)).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1261">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="ca5c1-1262">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1262">Lab</span></span>

* <span data-ttu-id="ca5c1-1263">Добавлены команды создания, отображения, удаления и вывода списка для среды в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1263">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="ca5c1-1264">Добавлены команды отображения и вывода списка для просмотра шаблонов ARM в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1264">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="ca5c1-1265">В команду `az lab vm list` добавлен флаг --environment для фильтрации виртуальных машин по среде в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1265">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="ca5c1-1266">Добавлена вспомогательная команда `az lab formula export-artifacts` для экспорта шаблона артефакта в формуле лаборатории.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1266">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="ca5c1-1267">Добавлены команды для управления секретами в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1267">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="ca5c1-1268">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1268">Monitor</span></span>

* <span data-ttu-id="ca5c1-1269">Исправление ошибки: моделирование `--actions` в `az alert-rules create` для использования строки в формате JSON ([№ 3009](https://github.com/Azure/azure-cli/issues/3009)).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1269">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="ca5c1-1270">Исправление ошибки: при создании параметров диагностики не принимались журналы и метрики из команды show ([№ 2913](https://github.com/Azure/azure-cli/issues/2913)).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1270">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="ca5c1-1271">Сеть</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1271">Network</span></span>

* <span data-ttu-id="ca5c1-1272">Добавлена команда `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1272">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="ca5c1-1273">Добавлена поддержка параметра `--filters` в команде `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1273">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="ca5c1-1274">Добавлена поддержка фильтрации подключений шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1274">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="ca5c1-1275">Добавлена поддержка конфигурации набора правил WAF шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1275">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="ca5c1-1276">Добавлена поддержка правил и фильтров маршрутов ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1276">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="ca5c1-1277">Добавлена поддержка географической маршрутизации диспетчера трафика.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1277">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="ca5c1-1278">Добавлена поддержка селекторов трафика на основе политик для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1278">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="ca5c1-1279">Добавлена поддержка политик IPSec для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1279">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="ca5c1-1280">Исправлена ошибка `vpn-connection create`, возникавшая при использовании параметра `--no-wait` или `--validate`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1280">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="ca5c1-1281">Добавлена поддержка шлюзов виртуальной сети "активный-активный".</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1281">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="ca5c1-1282">Удалены значения NULL из выходных данных команды `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1282">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="ca5c1-1283">BC: исправлена ошибка в выходных данных `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1283">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="ca5c1-1284">Исправлена ошибка, приводившая к неправильному анализу аргумента --key-length команды vpn-connection create.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1284">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="ca5c1-1285">Исправлена ошибка в `dns zone import`, из-за которой записи не импортировались правильно.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1285">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="ca5c1-1286">Исправлена ошибка, из-за которой команда `traffic-manager endpoint update` не работала.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1286">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="ca5c1-1287">Добавлены команды предварительного просмотра для Наблюдателя за сетями.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1287">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="ca5c1-1288">Профиль</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1288">Profile</span></span>

* <span data-ttu-id="ca5c1-1289">Поддержка входа при отсутствии подписок ([№ 2560](https://github.com/Azure/azure-cli/issues/2560)).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1289">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="ca5c1-1290">Поддержка сокращенных имен параметров в команде az account set --subscription ([№ 2980](https://github.com/Azure/azure-cli/issues/2980)).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1290">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="ca5c1-1291">Redis</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1291">Redis</span></span>

* <span data-ttu-id="ca5c1-1292">Добавлена команда update, которая также добавляет возможность масштабирования для кэша Redis.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1292">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="ca5c1-1293">Команда update-settings объявляется нерекомендуемой.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1293">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="ca5c1-1294">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1294">Resource</span></span>

* <span data-ttu-id="ca5c1-1295">Добавлены команды определения managedapp и managedapp ([№ 2985](https://github.com/Azure/azure-cli/issues/2985)).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1295">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="ca5c1-1296">Поддержка команд provider operation ([№ 2908](https://github.com/Azure/azure-cli/issues/2908)).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1296">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="ca5c1-1297">Поддержка создания универсального ресурса ([№ 2606](https://github.com/Azure/azure-cli/issues/2606)).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1297">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="ca5c1-1298">Исправлен анализ ресурсов и поиск версии API.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1298">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="ca5c1-1299">([№ 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1299">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="ca5c1-1300">Добавлены документы для команды az lock update.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1300">Add docs for az lock update.</span></span> <span data-ttu-id="ca5c1-1301">([№ 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1301">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="ca5c1-1302">Исправлена ошибка, возникавшая при попытке вывести список ресурсов группы, которая не существует.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1302">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="ca5c1-1303">([№ 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1303">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="ca5c1-1304">[Вычисления.] Устранены проблемы с масштабируемым набором виртуальных машин и обновлением группы доступности виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1304">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="ca5c1-1305">([№ 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1305">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="ca5c1-1306">Исправлена блокировка создания и удаления, возникающая, если параметр parent-resource-path не указан ([№ 2742](https://github.com/Azure/azure-cli/issues/2742)).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1306">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="ca5c1-1307">Роль</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1307">Role</span></span>

* <span data-ttu-id="ca5c1-1308">create-for-rbac: гарантируется, что дата завершения работы поставщика служб не может превышать срок действия сертификата ([№ 2989](https://github.com/Azure/azure-cli/issues/2989)).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1308">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="ca5c1-1309">RBAC: добавлена полная поддержка команды ad group ([№ 2016](https://github.com/Azure/azure-cli/issues/2016)).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1309">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="ca5c1-1310">Роль: устранены проблемы при обновлении определения роли ([№ 2745](https://github.com/Azure/azure-cli/issues/2745)).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1310">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="ca5c1-1311">create-for-rbac: обеспечен выбор введенного пользователем пароля.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1311">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="ca5c1-1312">SQL</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1312">SQL</span></span>

* <span data-ttu-id="ca5c1-1313">Добавлены команды az sql server list-usages и az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1313">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="ca5c1-1314">SQL: возможность прямого подключения к поставщику ресурса ([№ 2832](https://github.com/Azure/azure-cli/issues/2832)).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1314">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="ca5c1-1315">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1315">Storage</span></span>

* <span data-ttu-id="ca5c1-1316">Добавлено расположение по умолчанию группы ресурсов для `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1316">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="ca5c1-1317">Добавлена поддержка добавочного копирования больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1317">Add support for incremental blob copy</span></span>
* <span data-ttu-id="ca5c1-1318">Добавлена поддержка передачи больших блочных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1318">Add support for large block blob upload</span></span>
* <span data-ttu-id="ca5c1-1319">Размер блока изменяется и составляет 100 МБ, если передается файл, чей размер превышает 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1319">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="ca5c1-1320">ВМ</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1320">VM</span></span>

* <span data-ttu-id="ca5c1-1321">avail-set: число доменов обновления и доменов сбоя сделано необязательным.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1321">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="ca5c1-1322">Примечание. Команды виртуальной машины в независимых облаках: избегайте использовать функции, связанные с Управляемыми дисками, включая следующие:</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1322">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="ca5c1-1323">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1323">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="ca5c1-1324">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1324">az vm/vmss disk</span></span>
  3. <span data-ttu-id="ca5c1-1325">В команде az vm/vmss create используйте параметр --use-unmanaged-disk, чтобы избежать использования Управляемых дисков. Другие команды должны работать.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1325">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="ca5c1-1326">vm/vmss: улучшен текст предупреждения при создании пары ключей SSH.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1326">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="ca5c1-1327">vm/vmss: поддержка создания из образа Marketplace, для которого требуются сведения о плане ([№ 1209](https://github.com/Azure/azure-cli/issues/1209)).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1327">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="ca5c1-1328">3 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1328">April 3, 2017</span></span>

<span data-ttu-id="ca5c1-1329">Версия 2.0.2</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1329">Version 2.0.2</span></span>

<span data-ttu-id="ca5c1-1330">В этом выпуске мы добавили компоненты ACR, Batch, KeyVault и SQL.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1330">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

```text
azure-cli (2.0.2)

acr (2.0.0)
acs (2.0.2)
appservice (0.1.2)
batch (2.0.0)
cloud (2.0.0)
component (2.0.0)
configure (2.0.2)
container (0.1.2)
core (2.0.2)
documentdb (0.1.2)
feedback (2.0.0)
find (0.0.1b1)
iot (0.1.2)
keyvault (2.0.0)
lab (0.0.1)
monitor (0.0.1)
network (2.0.2)
nspkg (2.0.0)
profile (2.0.2)
redis (0.1.1b3)
resource (2.0.2)
role (2.0.1)
sql (2.0.0)
storage (2.0.2)
vm (2.0.2)
```

### <a name="core"></a><span data-ttu-id="ca5c1-1331">Core</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1331">Core</span></span>

* <span data-ttu-id="ca5c1-1332">Модули Acr, Lab, Monitor и Find добавлены в список по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1332">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="ca5c1-1333">Вход: пропуск неправильного клиента ([#2634](https://github.com/Azure/azure-cli/pull/2634)).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1333">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="ca5c1-1334">Вход: для подписки по умолчанию задано значение 1 с состоянием "Включено" ([#2575](https://github.com/Azure/azure-cli/pull/2575)).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1334">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="ca5c1-1335">Добавлена поддержка команд wait и --no-wait для дополнительных команд ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1335">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="ca5c1-1336">Core: поддержка входа при помощи субъекта-службы с использованием сертификата ([#2457](https://github.com/Azure/azure-cli/pull/2457)).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1336">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="ca5c1-1337">Добавлен запрос для отсутствующих параметров шаблона</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1337">Add prompting for missing template parameters.</span></span> <span data-ttu-id="ca5c1-1338">([#2364](https://github.com/Azure/azure-cli/pull/2364)).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1338">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="ca5c1-1339">Добавлена поддержка установки параметров по умолчанию для таких распространенных аргументов, как группа ресурсов по умолчанию, веб-страница по умолчанию, виртуальная машина по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1339">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="ca5c1-1340">Добавлена поддержка входа на конкретный клиент.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1340">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="ca5c1-1341">ACS</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1341">ACS</span></span>

* <span data-ttu-id="ca5c1-1342">[ACS] Добавлена поддержка настройки кластера ACS по умолчанию ([#2554](https://github.com/Azure/azure-cli/pull/2554)).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1342">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="ca5c1-1343">Добавлена поддержка запроса пароля для ключа SSH</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1343">Add support for ssh key password prompting.</span></span> <span data-ttu-id="ca5c1-1344">([#2044](https://github.com/Azure/azure-cli/pull/2044)).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1344">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="ca5c1-1345">Добавлена поддержка кластеров Windows</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1345">Add support for windows clusters.</span></span> <span data-ttu-id="ca5c1-1346">([#2211](https://github.com/Azure/azure-cli/pull/2211)).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1346">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="ca5c1-1347">Добавлена возможность изменения роли "Владелец" на роль "Участник"</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1347">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="ca5c1-1348">([#2321](https://github.com/Azure/azure-cli/pull/2321)).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1348">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="ca5c1-1349">AppService</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1349">AppService</span></span>

* <span data-ttu-id="ca5c1-1350">AppService: добавлена поддержка получения внешнего IP-адреса, используемого для записей DNS типа A ([#2627](https://github.com/Azure/azure-cli/pull/2627)).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1350">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="ca5c1-1351">AppService: добавлена поддержка привязки групповых сертификатов ([#2625](https://github.com/Azure/azure-cli/pull/2625)).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1351">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="ca5c1-1352">AppService: добавлена поддержка профилей для публикации списком ([#2504](https://github.com/Azure/azure-cli/pull/2504)).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1352">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="ca5c1-1353">AppService: добавлен триггер синхронизации с системой управления версиями после настройки ([#2326](https://github.com/Azure/azure-cli/pull/2326)).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1353">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="ca5c1-1354">Data Lake</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1354">DataLake</span></span>

* <span data-ttu-id="ca5c1-1355">Первый выпуск модуля Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1355">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="ca5c1-1356">Первый выпуск модуля Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1356">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="ca5c1-1357">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1357">DocuemntDB</span></span>

* <span data-ttu-id="ca5c1-1358">DocumentDB: добавлена поддержка для получения списка строк подключения ([#2580](https://github.com/Azure/azure-cli/pull/2580)).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1358">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="ca5c1-1359">ВМ</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1359">VM</span></span>

* <span data-ttu-id="ca5c1-1360">[Вычисления] Добавлена поддержка AppGateway для создания масштабируемого набора виртуальных машин ([#2570](https://github.com/Azure/azure-cli/pull/2570)).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1360">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="ca5c1-1361">[ВМ и VMSS] Улучшена поддержка кэширования диска ([#2522](https://github.com/Azure/azure-cli/pull/2522)).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1361">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="ca5c1-1362">ВМ и VMSS: внедрена логика проверки учетных данных, используемая на портале ([#2537](https://github.com/Azure/azure-cli/pull/2537)).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1362">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="ca5c1-1363">Добавлена поддержка команд wait и --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1363">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="ca5c1-1364">Масштабируемый набор виртуальных машин: добавлена поддержка \* для представления экземпляров на виртуальных машинах в виде списка ([#2467](https://github.com/Azure/azure-cli/pull/2467)).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1364">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="ca5c1-1365">Добавлен параметр --secrets для виртуальной машины и масштабируемого набора виртуальных машин ([#2212}(https://github.com/Azure/azure-cli/pull/2212)).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1365">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="ca5c1-1366">Добавлено разрешение на создание виртуальных машин на основе специализированного образа VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256)).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1366">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="ca5c1-1367">27 февраля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1367">February 27, 2017</span></span>

<span data-ttu-id="ca5c1-1368">Версия 2.0.0</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1368">Version 2.0.0</span></span>

<span data-ttu-id="ca5c1-1369">Этот первый общедоступный выпуск Azure CLI 2.0. Общедоступными являются такие командные модули:</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1369">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="ca5c1-1370">служба контейнеров (ACS);</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1370">Container Service (acs)</span></span>
- <span data-ttu-id="ca5c1-1371">вычисления (в том числе Resource Manager, виртуальная машина, масштабируемые наборы виртуальных машин, управляемые диски);</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1371">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="ca5c1-1372">Сеть</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1372">Networking</span></span>
- <span data-ttu-id="ca5c1-1373">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1373">Storage</span></span>

<span data-ttu-id="ca5c1-1374">Эти командные модули могут использоваться в рабочих средах. Они поддерживаются стандартными соглашениями Майкрософт об уровне обслуживания. Вы можете отправлять запросы непосредственно в службу технической поддержки Майкрософт или добавлять описание проблем в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/). Вы можете задавать вопросы на [сайте StackOverflow, используя тег azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), или обращаться к группе разработчиков по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Можно отправлять отзывы из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1374">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="ca5c1-1375">Команды в этих модулях стабильны, и предполагается, что в следующих выпусках этой версии Azure CLI их синтаксис не будет меняться.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1375">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="ca5c1-1376">Проверить версию CLI можно с помощью команды `az --version`. В выходных данных указана версия самого интерфейса командной строки (2.0.0 в этом выпуске), версии отдельных командных модулей и используемые вами версии Python и GCC.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1376">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

```text
azure-cli (2.0.0)

acs (2.0.0)
appservice (0.1.1b5)
batch (0.1.1b4)
cloud (2.0.0)
component (2.0.0)
configure (2.0.0)
container (0.1.1b4)
core (2.0.0)
documentdb (0.1.1b2)
feedback (2.0.0)
iot (0.1.1b3)
keyvault (0.1.1b5)
network (2.0.0)
nspkg (2.0.0)
profile (2.0.0)
redis (0.1.1b3)
resource (2.0.0)
role (2.0.0)
sql (0.1.1b5)
storage (2.0.0)
vm (2.0.0)

Python (Darwin) 2.7.10 (default, Jul 30 2016, 19:40:32)
[GCC 4.2.1 Compatible Apple LLVM 8.0.0 (clang-800.0.34)]
```

> [!Note]
> <span data-ttu-id="ca5c1-1377">Некоторые командные модули имеют постфикс b*n* или rc*n*. Эти командные модули все еще находятся на стадии предварительной версии и станут общедоступными в будущем.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1377">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="ca5c1-1378">У нас также есть предварительные ежедневные сборки CLI. Дополнительные сведения см. в инструкциях по [получению ежедневных сборок](https://github.com/Azure/azure-cli#nightly-builds), а также в инструкциях по [настройке среды разработки и участии в написании кода](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1378">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="ca5c1-1379">О проблемах с предварительными ежедневными сборками можно сообщить несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1379">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="ca5c1-1380">добавив информацию о проблемах в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/);</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1380">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="ca5c1-1381">Свяжитесь с командой разработчиков ([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)),</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1381">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="ca5c1-1382">отправив отзыв из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="ca5c1-1382">Provide feedback from the command line with the `az feedback` command</span></span>

