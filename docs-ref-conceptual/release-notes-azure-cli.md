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
ms.openlocfilehash: 57f13c7d17e2d248132e2e9c49bb0b4994f041f5
ms.sourcegitcommit: 80189ff103c91f8c47ab8ebf586df815fff5dd5d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2018
ms.locfileid: "34799266"
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="a1348-103">Заметки о выпуске Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="a1348-103">Azure CLI 2.0 release notes</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="a1348-104">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a1348-104">June 5, 2018</span></span>

<span data-ttu-id="a1348-105">Версия 2.0.34</span><span class="sxs-lookup"><span data-stu-id="a1348-105">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="a1348-106">Core</span><span class="sxs-lookup"><span data-stu-id="a1348-106">Core</span></span>

* <span data-ttu-id="a1348-107">Добавлена поддержка перекрестных ссылок на ресурсы клиента.</span><span class="sxs-lookup"><span data-stu-id="a1348-107">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="a1348-108">Улучшена надежность при передаче данных телеметрии.</span><span class="sxs-lookup"><span data-stu-id="a1348-108">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="a1348-109">ACR</span><span class="sxs-lookup"><span data-stu-id="a1348-109">ACR</span></span>

* <span data-ttu-id="a1348-110">Добавлена поддержка VSTS в качестве расположения удаленного источника.</span><span class="sxs-lookup"><span data-stu-id="a1348-110">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="a1348-111">Добавлена команда `acr import`.</span><span class="sxs-lookup"><span data-stu-id="a1348-111">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="a1348-112">AKS</span><span class="sxs-lookup"><span data-stu-id="a1348-112">AKS</span></span>

* <span data-ttu-id="a1348-113">Изменена команда `aks get-credentials` для создания файла конфигурации kube с более надежными разрешениями файловой системы.</span><span class="sxs-lookup"><span data-stu-id="a1348-113">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="a1348-114">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="a1348-114">Batch</span></span>

* <span data-ttu-id="a1348-115">Исправлена ошибка, связанная с форматированием таблиц при выполнении команды pool list. [[Ошибка #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="a1348-115">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="a1348-116">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="a1348-116">IOT</span></span>

* <span data-ttu-id="a1348-117">Добавлена возможность создания Центров Интернета вещей категории "Базовый".</span><span class="sxs-lookup"><span data-stu-id="a1348-117">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="a1348-118">Сеть</span><span class="sxs-lookup"><span data-stu-id="a1348-118">Network</span></span>

* <span data-ttu-id="a1348-119">Улучшена команда `network vnet peering`.</span><span class="sxs-lookup"><span data-stu-id="a1348-119">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="a1348-120">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="a1348-120">Policy Insights</span></span>

* <span data-ttu-id="a1348-121">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="a1348-121">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="a1348-122">ARM</span><span class="sxs-lookup"><span data-stu-id="a1348-122">ARM</span></span>

* <span data-ttu-id="a1348-123">Добавлены команды `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="a1348-123">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="a1348-124">SQL</span><span class="sxs-lookup"><span data-stu-id="a1348-124">SQL</span></span>

* <span data-ttu-id="a1348-125">Добавлены новые команды для управляемого экземпляра:</span><span class="sxs-lookup"><span data-stu-id="a1348-125">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="a1348-126">Добавлены новые команды для управляемой базы данных:</span><span class="sxs-lookup"><span data-stu-id="a1348-126">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="a1348-127">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="a1348-127">Storage</span></span>

* <span data-ttu-id="a1348-128">Добавлены типы MIME для JSON и JavaScript, выводимые из расширений файлов.</span><span class="sxs-lookup"><span data-stu-id="a1348-128">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="a1348-129">ВМ</span><span class="sxs-lookup"><span data-stu-id="a1348-129">VM</span></span>

* <span data-ttu-id="a1348-130">Изменена команда `vm list-skus` для использования фиксированных столбцов, а также добавлено предупреждение об удалении `Tier` и `Size`.</span><span class="sxs-lookup"><span data-stu-id="a1348-130">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="a1348-131">Добавлен параметр `--accelerated-networking` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="a1348-131">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="a1348-132">Добавлен параметр `--tags` для команды `identity create`.</span><span class="sxs-lookup"><span data-stu-id="a1348-132">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="a1348-133">22 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a1348-133">May 22, 2018</span></span>

<span data-ttu-id="a1348-134">Версия 2.0.33</span><span class="sxs-lookup"><span data-stu-id="a1348-134">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="a1348-135">Core</span><span class="sxs-lookup"><span data-stu-id="a1348-135">Core</span></span>

* <span data-ttu-id="a1348-136">Добавлена возможность включения символа `@` в имена файлов.</span><span class="sxs-lookup"><span data-stu-id="a1348-136">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="a1348-137">ACS</span><span class="sxs-lookup"><span data-stu-id="a1348-137">ACS</span></span>

* <span data-ttu-id="a1348-138">Добавлены новые команды для Dev Spaces: `aks use-dev-spaces` и `aks remove-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="a1348-138">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="a1348-139">Исправлена опечатка в справочном сообщении.</span><span class="sxs-lookup"><span data-stu-id="a1348-139">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="a1348-140">AppService</span><span class="sxs-lookup"><span data-stu-id="a1348-140">AppService</span></span>

* <span data-ttu-id="a1348-141">Улучшены команды общего обновления.</span><span class="sxs-lookup"><span data-stu-id="a1348-141">Improved generic update commands</span></span>
* <span data-ttu-id="a1348-142">Добавлена поддержка асинхронного выполнения для `webapp deployment source config-zip`.</span><span class="sxs-lookup"><span data-stu-id="a1348-142">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="a1348-143">Контейнер</span><span class="sxs-lookup"><span data-stu-id="a1348-143">Container</span></span>

* <span data-ttu-id="a1348-144">Добавлена возможность экспорта группы контейнеров в формате YAML.</span><span class="sxs-lookup"><span data-stu-id="a1348-144">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="a1348-145">Добавлена возможность использования файла YAML для создания или обновления группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="a1348-145">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="a1348-146">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="a1348-146">Extension</span></span>

* <span data-ttu-id="a1348-147">Улучшена операция удаления расширений.</span><span class="sxs-lookup"><span data-stu-id="a1348-147">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="a1348-148">Interactive</span><span class="sxs-lookup"><span data-stu-id="a1348-148">Interactive</span></span>

* <span data-ttu-id="a1348-149">Изменены параметры ведения журнала для отключения средства синтаксического анализа для завершенных операций.</span><span class="sxs-lookup"><span data-stu-id="a1348-149">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="a1348-150">Улучшена обработка поврежденных кэшей справки.</span><span class="sxs-lookup"><span data-stu-id="a1348-150">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="a1348-151">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="a1348-151">KeyVault</span></span>

* <span data-ttu-id="a1348-152">Исправлены команды хранилища ключей для работы с удостоверениями в Cloud Shell или виртуальных машинах.</span><span class="sxs-lookup"><span data-stu-id="a1348-152">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="a1348-153">Сеть</span><span class="sxs-lookup"><span data-stu-id="a1348-153">Network</span></span>

* <span data-ttu-id="a1348-154">Исправлена проблема, при которой `network watcher show-topology` не будет выполняться, если виртуальной сети или подсети присвоить имя. [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="a1348-154">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="a1348-155">Исправлена проблема, при которой некоторые команды `network watcher` выдают ошибку, что Наблюдатель за сетями не включен в определенных регионах. [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="a1348-155">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="a1348-156">SQL</span><span class="sxs-lookup"><span data-stu-id="a1348-156">SQL</span></span>

* <span data-ttu-id="a1348-157">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены объекты ответа, возвращаемые в результатах команд `db` и `dw`:</span><span class="sxs-lookup"><span data-stu-id="a1348-157">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="a1348-158">Свойство `serviceLevelObjective` переименовано на `currentServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="a1348-158">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="a1348-159">Удалены свойства `currentServiceObjectiveId` и `requestedServiceObjectiveId`.</span><span class="sxs-lookup"><span data-stu-id="a1348-159">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span> 
    * <span data-ttu-id="a1348-160">Тип свойства `maxSizeBytes` изменен со строкового на целое число.</span><span class="sxs-lookup"><span data-stu-id="a1348-160">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="a1348-161">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `db` и `dw` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="a1348-161">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="a1348-162">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="a1348-162">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="a1348-163">Для обновления используйте параметр `--service-objective` или задайте свойство `sku.name`.</span><span class="sxs-lookup"><span data-stu-id="a1348-163">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="a1348-164">`edition`.</span><span class="sxs-lookup"><span data-stu-id="a1348-164">`edition`.</span></span> <span data-ttu-id="a1348-165">Для обновления используйте параметр `--edition` или задайте свойство `sku.tier`.</span><span class="sxs-lookup"><span data-stu-id="a1348-165">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="a1348-166">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="a1348-166">`elasticPoolName`.</span></span> <span data-ttu-id="a1348-167">Для обновления используйте параметр `--elastic-pool` или задайте свойство `elasticPoolId`.</span><span class="sxs-lookup"><span data-stu-id="a1348-167">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="a1348-168">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `elastic-pool` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="a1348-168">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="a1348-169">`edition`.</span><span class="sxs-lookup"><span data-stu-id="a1348-169">`edition`.</span></span> <span data-ttu-id="a1348-170">Для обновления используйте параметр `--edition`.</span><span class="sxs-lookup"><span data-stu-id="a1348-170">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="a1348-171">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="a1348-171">`dtu`.</span></span> <span data-ttu-id="a1348-172">Для обновления используйте параметр `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="a1348-172">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="a1348-173">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="a1348-173">`databaseDtuMin`.</span></span> <span data-ttu-id="a1348-174">Для обновления используйте параметр `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="a1348-174">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="a1348-175">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="a1348-175">`databaseDtuMax`.</span></span> <span data-ttu-id="a1348-176">Для обновления используйте параметр `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="a1348-176">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="a1348-177">Добавлены параметры `--family` и `--capacity` для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="a1348-177">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="a1348-178">Добавлены модули форматирования таблиц для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="a1348-178">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="a1348-179">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="a1348-179">Storage</span></span>

* <span data-ttu-id="a1348-180">Добавлено средство заполнения для аргумента `--account-name`.</span><span class="sxs-lookup"><span data-stu-id="a1348-180">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="a1348-181">Устранена проблема, связанная с командой `storage entity query`.</span><span class="sxs-lookup"><span data-stu-id="a1348-181">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="a1348-182">ВМ</span><span class="sxs-lookup"><span data-stu-id="a1348-182">VM</span></span>

* <span data-ttu-id="a1348-183">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--write-accelerator` из команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="a1348-183">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="a1348-184">Такие же возможности предоставляет команда `vm update` или `vm disk attach`.</span><span class="sxs-lookup"><span data-stu-id="a1348-184">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="a1348-185">Устранена проблема с сопоставлением образов расширения в команде `[vm|vmss] extension`.</span><span class="sxs-lookup"><span data-stu-id="a1348-185">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="a1348-186">Добавлен параметр `--boot-diagnostics-storage` для команды `vm create` для записи журнала загрузки.</span><span class="sxs-lookup"><span data-stu-id="a1348-186">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="a1348-187">Добавлен параметр `--license-type` для команды `[vm|vmss] update`.</span><span class="sxs-lookup"><span data-stu-id="a1348-187">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="a1348-188">7 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a1348-188">May 7, 2018</span></span>

<span data-ttu-id="a1348-189">Версия 2.0.32</span><span class="sxs-lookup"><span data-stu-id="a1348-189">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="a1348-190">Core</span><span class="sxs-lookup"><span data-stu-id="a1348-190">Core</span></span>

* <span data-ttu-id="a1348-191">Исправлено необработанное исключение при получении секретов из основной учетной записи службы с сертификатом.</span><span class="sxs-lookup"><span data-stu-id="a1348-191">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="a1348-192">Добавлена ограниченная поддержка для позиционных аргументов.</span><span class="sxs-lookup"><span data-stu-id="a1348-192">Added limited support for positional arguments</span></span>
* <span data-ttu-id="a1348-193">Исправлена проблема, когда `--query` нельзя использовать с `--ids`.</span><span class="sxs-lookup"><span data-stu-id="a1348-193">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="a1348-194">#5591</span><span class="sxs-lookup"><span data-stu-id="a1348-194">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="a1348-195">Улучшены сценарии конвейерной передачи от команд при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="a1348-195">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="a1348-196">Добавлена поддержка `-o tsv` с указанием запроса или `-o json` без указания запроса.</span><span class="sxs-lookup"><span data-stu-id="a1348-196">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="a1348-197">Добавлена команда предложения в случае ошибки, если пользователи вводят команды с опечаткой.</span><span class="sxs-lookup"><span data-stu-id="a1348-197">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="a1348-198">Исправлена ошибка, когда пользователи вводят `az ''`.</span><span class="sxs-lookup"><span data-stu-id="a1348-198">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="a1348-199">Добавлена поддержка настраиваемого ресурса для командных модулей и расширений.</span><span class="sxs-lookup"><span data-stu-id="a1348-199">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="a1348-200">ACR</span><span class="sxs-lookup"><span data-stu-id="a1348-200">ACR</span></span>

* <span data-ttu-id="a1348-201">Добавлены команды сборки ACR.</span><span class="sxs-lookup"><span data-stu-id="a1348-201">Added ACR Build commands</span></span>
* <span data-ttu-id="a1348-202">Исправлена ошибка о не найденных сообщениях об ошибках.</span><span class="sxs-lookup"><span data-stu-id="a1348-202">Improved resource not found error messages</span></span>
* <span data-ttu-id="a1348-203">Оптимизированы производительность создания ресурсов и обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="a1348-203">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="a1348-204">Улучшены возможности входа ACR в нестандартные консоли и WSL.</span><span class="sxs-lookup"><span data-stu-id="a1348-204">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="a1348-205">Улучшены сообщения об ошибках команд репозитория.</span><span class="sxs-lookup"><span data-stu-id="a1348-205">Improved repository commands error messages</span></span>
* <span data-ttu-id="a1348-206">Обновлены столбцы таблиц и порядок их расположения.</span><span class="sxs-lookup"><span data-stu-id="a1348-206">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="a1348-207">ACS</span><span class="sxs-lookup"><span data-stu-id="a1348-207">ACS</span></span>

* <span data-ttu-id="a1348-208">Добавлено предупреждение о том, что `az aks` — это предварительная версия службы.</span><span class="sxs-lookup"><span data-stu-id="a1348-208">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="a1348-209">Исправлена проблема с разрешением в `aks install-connector`, когда `--aci-resource-group` не указывается.</span><span class="sxs-lookup"><span data-stu-id="a1348-209">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="a1348-210">AMS</span><span class="sxs-lookup"><span data-stu-id="a1348-210">AMS</span></span>

* <span data-ttu-id="a1348-211">Первоначальный выпуск. Управление ресурсами Служб мультимедиа Azure.</span><span class="sxs-lookup"><span data-stu-id="a1348-211">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="a1348-212">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a1348-212">Appservice</span></span>

* <span data-ttu-id="a1348-213">Исправлена ошибка в `webapp delete`, когда `--slot` предоставляется.</span><span class="sxs-lookup"><span data-stu-id="a1348-213">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="a1348-214">Удалено `--runtime-version` из `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="a1348-214">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="a1348-215">Добавлена поддержка min\_tls\_version и https2.0.</span><span class="sxs-lookup"><span data-stu-id="a1348-215">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="a1348-216">Добавлена поддержка нескольких контейнеров.</span><span class="sxs-lookup"><span data-stu-id="a1348-216">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="a1348-217">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="a1348-217">Batch AI</span></span>

* <span data-ttu-id="a1348-218">Изменено `batchai create cluster` с учетом приоритета виртуальной машины при настройке в файле конфигурации кластера.</span><span class="sxs-lookup"><span data-stu-id="a1348-218">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="a1348-219">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="a1348-219">Cognitive Services</span></span>

* <span data-ttu-id="a1348-220">Исправлена опечатка в примере для `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603).</span><span class="sxs-lookup"><span data-stu-id="a1348-220">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="a1348-221">Потребление</span><span class="sxs-lookup"><span data-stu-id="a1348-221">Consumption</span></span>

* <span data-ttu-id="a1348-222">Добавлены новые команды в API для управления бюджетом.</span><span class="sxs-lookup"><span data-stu-id="a1348-222">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="a1348-223">Контейнер</span><span class="sxs-lookup"><span data-stu-id="a1348-223">Container</span></span>

* <span data-ttu-id="a1348-224">Удалено требование `--registry-server` для `container create`, когда сервер реестра включен в имя образа.</span><span class="sxs-lookup"><span data-stu-id="a1348-224">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="a1348-225">База данных Cosmos</span><span class="sxs-lookup"><span data-stu-id="a1348-225">Cosmos DB</span></span>

* <span data-ttu-id="a1348-226">Добавлена поддержка VNET для Azure CLI в Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="a1348-226">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="a1348-227">DMS</span><span class="sxs-lookup"><span data-stu-id="a1348-227">DMS</span></span>

* <span data-ttu-id="a1348-228">Исходный выпуск. Добавлена поддержка сценария миграции SQL — Azure SQL.</span><span class="sxs-lookup"><span data-stu-id="a1348-228">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="a1348-229">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="a1348-229">Extension</span></span>

* <span data-ttu-id="a1348-230">Исправлена ошибка, когда метаданные остановленного расширения отображались.</span><span class="sxs-lookup"><span data-stu-id="a1348-230">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="a1348-231">Interactive</span><span class="sxs-lookup"><span data-stu-id="a1348-231">Interactive</span></span>

* <span data-ttu-id="a1348-232">Разрешена работа интерактивных средств завершения с позиционными аргументами.</span><span class="sxs-lookup"><span data-stu-id="a1348-232">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="a1348-233">Добавлены более понятные выходные данные, когда пользователи вводят \'.</span><span class="sxs-lookup"><span data-stu-id="a1348-233">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="a1348-234">Исправлены завершения для параметров без справки.</span><span class="sxs-lookup"><span data-stu-id="a1348-234">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="a1348-235">Исправлены описания для групп команд.</span><span class="sxs-lookup"><span data-stu-id="a1348-235">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="a1348-236">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="a1348-236">Lab</span></span>

* <span data-ttu-id="a1348-237">Исправлены регрессии из преобразования Knack.</span><span class="sxs-lookup"><span data-stu-id="a1348-237">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="a1348-238">Сеть</span><span class="sxs-lookup"><span data-stu-id="a1348-238">Network</span></span>

* <span data-ttu-id="a1348-239">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--ids` для:</span><span class="sxs-lookup"><span data-stu-id="a1348-239">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span> 
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="a1348-240">Профиль</span><span class="sxs-lookup"><span data-stu-id="a1348-240">Profile</span></span>

* <span data-ttu-id="a1348-241">Исправлено определение источника `disk create`.</span><span class="sxs-lookup"><span data-stu-id="a1348-241">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="a1348-242">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--msi-port` и `--identity-port`, так как они больше не используются.</span><span class="sxs-lookup"><span data-stu-id="a1348-242">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="a1348-243">Исправлена опечатка в кратком описании `account get-access-token`.</span><span class="sxs-lookup"><span data-stu-id="a1348-243">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="a1348-244">Redis</span><span class="sxs-lookup"><span data-stu-id="a1348-244">Redis</span></span>

* <span data-ttu-id="a1348-245">Вместо `redis patch-schedule patch-schedule show` теперь используется `redis patch-schedule show`.</span><span class="sxs-lookup"><span data-stu-id="a1348-245">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="a1348-246">`redis list-all` теперь не используется.</span><span class="sxs-lookup"><span data-stu-id="a1348-246">Deprecated `redis list-all`.</span></span> <span data-ttu-id="a1348-247">Эта функция включена в `redis list`.</span><span class="sxs-lookup"><span data-stu-id="a1348-247">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="a1348-248">Вместо `redis import-method` теперь используется `redis import`.</span><span class="sxs-lookup"><span data-stu-id="a1348-248">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="a1348-249">Добавлена поддержка `--ids` для разных команд.</span><span class="sxs-lookup"><span data-stu-id="a1348-249">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="a1348-250">Роль</span><span class="sxs-lookup"><span data-stu-id="a1348-250">Role</span></span>

* <span data-ttu-id="a1348-251">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `ad sp reset-credentials` по причине устаревания.</span><span class="sxs-lookup"><span data-stu-id="a1348-251">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="a1348-252">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="a1348-252">Storage</span></span>

* <span data-ttu-id="a1348-253">Разрешено применение SAS-токенов назначения к источнику для копирования BLOB-объектов, если SAS источника и ключ учетной записи не указаны.</span><span class="sxs-lookup"><span data-stu-id="a1348-253">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="a1348-254">Добавлено отображение времени ожидания сокета для отправки и скачивания большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="a1348-254">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="a1348-255">Добавлена обработка имен больших двоичных объектов, которые начинаются с разделителей пути, как относительных путей.</span><span class="sxs-lookup"><span data-stu-id="a1348-255">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="a1348-256">Разрешено использовать `storage blob copy --source-sas` с начальным символом запроса "?".</span><span class="sxs-lookup"><span data-stu-id="a1348-256">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="a1348-257">Исправлено `storage entity query --marker` для принятия списка пар "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="a1348-257">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="a1348-258">ВМ</span><span class="sxs-lookup"><span data-stu-id="a1348-258">VM</span></span>

* <span data-ttu-id="a1348-259">Исправлена недопустимая логика обнаружения в URI неуправляемого BLOB-объекта.</span><span class="sxs-lookup"><span data-stu-id="a1348-259">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="a1348-260">Добавлена поддержка шифрования диска без предоставления пользователем субъектов-служб.</span><span class="sxs-lookup"><span data-stu-id="a1348-260">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="a1348-261">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Не используйте ManagedIdentityExtension виртуальной машины для включения поддержки MSI</span><span class="sxs-lookup"><span data-stu-id="a1348-261">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="a1348-262">Добавлена поддержка политики вытеснения для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="a1348-262">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="a1348-263">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--ids` из:</span><span class="sxs-lookup"><span data-stu-id="a1348-263">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="a1348-264">Добавлена поддержка ускорителя записи.</span><span class="sxs-lookup"><span data-stu-id="a1348-264">Added write accelerator support</span></span> 
* <span data-ttu-id="a1348-265">Добавлена команда `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="a1348-265">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="a1348-266">Исправлено `vm diagnostics set` для надежного определения типа ОС виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="a1348-266">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="a1348-267">Изменено `vm resize` для проверки того, отличается ли запрошенный размер от установленного (с обновлением только при изменении).</span><span class="sxs-lookup"><span data-stu-id="a1348-267">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="a1348-268">10 апреля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a1348-268">April 10, 2018</span></span>

<span data-ttu-id="a1348-269">Версия 2.0.31</span><span class="sxs-lookup"><span data-stu-id="a1348-269">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="a1348-270">ACR</span><span class="sxs-lookup"><span data-stu-id="a1348-270">ACR</span></span>

* <span data-ttu-id="a1348-271">Улучшена обработка ошибок при откате wincred.</span><span class="sxs-lookup"><span data-stu-id="a1348-271">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="a1348-272">ACS</span><span class="sxs-lookup"><span data-stu-id="a1348-272">ACS</span></span>

* <span data-ttu-id="a1348-273">Срок действия имен субъектов-служб, созданных службой контейнеров Azure, изменен до 5 лет.</span><span class="sxs-lookup"><span data-stu-id="a1348-273">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="a1348-274">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a1348-274">Appservice</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="a1348-276">Исправлено неперехватываемое исключение для несуществующих планов веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="a1348-276">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="a1348-277">Batch AI</span><span class="sxs-lookup"><span data-stu-id="a1348-277">BatchAI</span></span>

* <span data-ttu-id="a1348-278">Добавлена поддержка API 2018-03-01.</span><span class="sxs-lookup"><span data-stu-id="a1348-278">Added support for 2018-03-01 API</span></span>

 - <span data-ttu-id="a1348-279">Подключение на уровне задания.</span><span class="sxs-lookup"><span data-stu-id="a1348-279">Job level mounting</span></span>
 - <span data-ttu-id="a1348-280">Переменные среды со значениями секретов.</span><span class="sxs-lookup"><span data-stu-id="a1348-280">Environment variables with secret values</span></span>
 - <span data-ttu-id="a1348-281">Параметры счетчиков производительности</span><span class="sxs-lookup"><span data-stu-id="a1348-281">Performance counters settings</span></span>
 - <span data-ttu-id="a1348-282">Предоставление информации о сегменте пути конкретного задания.</span><span class="sxs-lookup"><span data-stu-id="a1348-282">Reporting of job specific path segment</span></span>
 - <span data-ttu-id="a1348-283">Поддержка вложенных папок в API списка файлов.</span><span class="sxs-lookup"><span data-stu-id="a1348-283">Support for subfolders in list files api</span></span>
 - <span data-ttu-id="a1348-284">Предоставление информации об использовании и ограничениях.</span><span class="sxs-lookup"><span data-stu-id="a1348-284">Usage and limits reporting</span></span>
 - <span data-ttu-id="a1348-285">Возможность указать тип кэширования для NFS-серверов.</span><span class="sxs-lookup"><span data-stu-id="a1348-285">Allow to specify caching type for NFS servers</span></span>
 - <span data-ttu-id="a1348-286">Поддержка пользовательских образов.</span><span class="sxs-lookup"><span data-stu-id="a1348-286">Support for custom images</span></span>
 - <span data-ttu-id="a1348-287">Добавлена поддержка инструментария pyTorch.</span><span class="sxs-lookup"><span data-stu-id="a1348-287">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="a1348-288">Добавлена команда `job wait`, позволяющая дождаться завершения задания и сообщить код выхода задания.</span><span class="sxs-lookup"><span data-stu-id="a1348-288">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="a1348-289">Добавлена команда `usage show`, позволяющая получить актуальные сведения об использовании и ограничениях ресурсов Batch AI для различных регионов.</span><span class="sxs-lookup"><span data-stu-id="a1348-289">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="a1348-290">Поддержка национальных облаков.</span><span class="sxs-lookup"><span data-stu-id="a1348-290">National clouds are supported</span></span>
* <span data-ttu-id="a1348-291">Для заданий добавлены аргументы командной строки, которые позволяют подключать файловые системы на уровне заданий. Эти же действия можно выполнять в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="a1348-291">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="a1348-292">Добавлены дополнительные параметры для настройки кластеров: приоритет виртуальной машины, подсеть, исходное число узлов для кластеров с автоматическим масштабированием, выбор пользовательского образа.</span><span class="sxs-lookup"><span data-stu-id="a1348-292">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="a1348-293">Добавлен параметр командной строки, который позволяет указать тип кэширования для управляемой файловой системы NFS службы Batch AI.</span><span class="sxs-lookup"><span data-stu-id="a1348-293">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="a1348-294">Упрощена процедура выбора подключаемой файловой системы в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="a1348-294">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="a1348-295">Теперь учетные данные для общего файлового ресурса Azure и контейнеров BLOB-объектов Azure указывать не нужно: CLI получит отсутствующие учетные данные с помощью ключа учетной записи хранения, указанного в параметрах командной строки, или переменной среды либо запросит ключ из службы хранилища Azure (если учетная запись хранения относится к текущей подписке).</span><span class="sxs-lookup"><span data-stu-id="a1348-295">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="a1348-296">Команда задания потоковой передачи файлов теперь автоматически завершается при завершении задания (успешное выполнение, сбой, прерывание или удаление).</span><span class="sxs-lookup"><span data-stu-id="a1348-296">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="a1348-297">Улучшены выходные данные `table` для операций `show`.</span><span class="sxs-lookup"><span data-stu-id="a1348-297">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="a1348-298">Добавлен параметр `--use-auto-storage` для создания кластера.</span><span class="sxs-lookup"><span data-stu-id="a1348-298">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="a1348-299">Этот параметр упрощает управление учетными записями хранения, а также подключение общего файлового ресурса Azure и контейнеров BLOB-объектов Azure к кластеру.</span><span class="sxs-lookup"><span data-stu-id="a1348-299">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="a1348-300">Добавлен параметр `--generate-ssh-keys` для команд `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="a1348-300">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="a1348-301">Добавлена возможность запустить задачу настройки узла через командную строку.</span><span class="sxs-lookup"><span data-stu-id="a1348-301">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="a1348-302">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `job stream-file` и `job list-files` перемещены в группу `job file`.</span><span class="sxs-lookup"><span data-stu-id="a1348-302">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="a1348-303">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В команде `file-server create` параметр `--admin-user-name` переименован в `--user-name` для согласованности с командой `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="a1348-303">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="a1348-304">Выставление счетов</span><span class="sxs-lookup"><span data-stu-id="a1348-304">Billing</span></span>

* <span data-ttu-id="a1348-305">Добавлены команды для учетной записи регистрации.</span><span class="sxs-lookup"><span data-stu-id="a1348-305">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="a1348-306">Потребление</span><span class="sxs-lookup"><span data-stu-id="a1348-306">Consumption</span></span>

* <span data-ttu-id="a1348-307">Добавлены команды `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="a1348-307">Added `marketplace` commands</span></span>
* <span data-ttu-id="a1348-308">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations summaries` переименована в `reservation summary`.</span><span class="sxs-lookup"><span data-stu-id="a1348-308">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="a1348-309">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations details` переименована в `reservation detail`.</span><span class="sxs-lookup"><span data-stu-id="a1348-309">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="a1348-310">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation` удалены короткие параметры `--reservation-order-id` и `--reservation-id`.</span><span class="sxs-lookup"><span data-stu-id="a1348-310">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="a1348-311">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation summary` удалены короткие параметры `--grain`.</span><span class="sxs-lookup"><span data-stu-id="a1348-311">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="a1348-312">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `pricesheet` удалены короткие параметры `--include-meter-details`.</span><span class="sxs-lookup"><span data-stu-id="a1348-312">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="a1348-313">Контейнер</span><span class="sxs-lookup"><span data-stu-id="a1348-313">Container</span></span>

* <span data-ttu-id="a1348-314">Добавлены параметры подключения тома репозитория git: `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` и `--gitrepo-mount-path`.</span><span class="sxs-lookup"><span data-stu-id="a1348-314">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="a1348-315">Исправлена ошибка [#5926](https://github.com/Azure/azure-cli/issues/5926): команда `az container exec` возвращает ошибку, когда указан параметр --container-name.</span><span class="sxs-lookup"><span data-stu-id="a1348-315">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="a1348-316">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="a1348-316">Extension</span></span>

* <span data-ttu-id="a1348-317">Сообщение о проверке распространения перенесено на уровень отладки.</span><span class="sxs-lookup"><span data-stu-id="a1348-317">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="a1348-318">Interactive</span><span class="sxs-lookup"><span data-stu-id="a1348-318">Interactive</span></span>

* <span data-ttu-id="a1348-319">Если команда не распознана, выполнение прерывается.</span><span class="sxs-lookup"><span data-stu-id="a1348-319">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="a1348-320">Добавлены перехватчики событий, которые используются до и после создания поддерева команд.</span><span class="sxs-lookup"><span data-stu-id="a1348-320">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="a1348-321">Добавлены сведения о выполнении для параметров `--ids`.</span><span class="sxs-lookup"><span data-stu-id="a1348-321">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="a1348-322">Сеть</span><span class="sxs-lookup"><span data-stu-id="a1348-322">Network</span></span>

* <span data-ttu-id="a1348-323">Исправлена ошибка [#5936](https://github.com/Azure/azure-cli/issues/5936): не задаются теги `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="a1348-323">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="a1348-324">Добавлен аргумент `--auth-certs`, который позволяет подключать сертификаты аутентификации для `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="a1348-324">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> <span data-ttu-id="a1348-325">[#4910](https://github.com/Azure/azure-cli/issues/4910).</span><span class="sxs-lookup"><span data-stu-id="a1348-325">[#4910](https://github.com/Azure/azure-cli/issues/4910)</span></span>
* <span data-ttu-id="a1348-326">Добавлены команды `ddos-protection` для создания планов защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="a1348-326">Added `ddos-protection` commands to create DDoS protection plans</span></span> 
* <span data-ttu-id="a1348-327">В команду `vnet [create|update]` добавлена поддержка `--ddos-protection-plan` для связи виртуальной сети с планом защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="a1348-327">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="a1348-328">Исправлена ошибка с флагом `--disable-bgp-route-propagation` в команде `network route-table [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="a1348-328">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="a1348-329">Удалены фиктивные аргументы `--public-ip-address-type` и `--subnet-type` для команды `network lb [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="a1348-329">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="a1348-330">В `network dns zone [import|export]` и `network dns record-set txt add-record` добавлена поддержка записей типа TXT с escape-последовательностями RFC 1035.</span><span class="sxs-lookup"><span data-stu-id="a1348-330">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="a1348-331">Профиль</span><span class="sxs-lookup"><span data-stu-id="a1348-331">Profile</span></span>

* <span data-ttu-id="a1348-332">Добавлена поддержка классических учетных записей Azure для команды `account list`.</span><span class="sxs-lookup"><span data-stu-id="a1348-332">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="a1348-333">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены аргументы `--msi`  &  `--msi-port`.</span><span class="sxs-lookup"><span data-stu-id="a1348-333">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="a1348-334">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="a1348-334">RDBMS</span></span>

* <span data-ttu-id="a1348-335">Добавлена команда `georestore`.</span><span class="sxs-lookup"><span data-stu-id="a1348-335">Added `georestore` command</span></span>
* <span data-ttu-id="a1348-336">Из команды `create` исключено ограничение на размер хранилища.</span><span class="sxs-lookup"><span data-stu-id="a1348-336">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="a1348-337">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a1348-337">Resource</span></span>

* <span data-ttu-id="a1348-338">Добавлена поддержка параметра `--metadata` в команде `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="a1348-338">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="a1348-339">Добавлена поддержка `--metadata`, `--set`, `--add` и `--remove` для команды `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="a1348-339">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="a1348-340">SQL</span><span class="sxs-lookup"><span data-stu-id="a1348-340">SQL</span></span>

* <span data-ttu-id="a1348-341">Добавлены команды `sql elastic-pool op list` и `sql elastic-pool op cancel`.</span><span class="sxs-lookup"><span data-stu-id="a1348-341">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="a1348-342">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="a1348-342">Storage</span></span>

* <span data-ttu-id="a1348-343">Улучшены сообщения об ошибках для строк подключения, имеющих неправильный формат.</span><span class="sxs-lookup"><span data-stu-id="a1348-343">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="a1348-344">ВМ</span><span class="sxs-lookup"><span data-stu-id="a1348-344">VM</span></span>

* <span data-ttu-id="a1348-345">В команде `vmss create` добавлена возможность настроить для платформы количество доменов сбоя.</span><span class="sxs-lookup"><span data-stu-id="a1348-345">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="a1348-346">Команда `vmss create` теперь по умолчанию использует стандартную балансировку нагрузки для зональных и больших масштабируемых наборов, а также масштабируемых наборов, в которых отключена одна группа размещения.</span><span class="sxs-lookup"><span data-stu-id="a1348-346">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="a1348-348">Добавлена поддержка SKU общедоступного IP-адреса для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="a1348-348">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="a1348-349">В команду `vm secret format` добавлены аргументы `--keyvault` и `--resource-group` для тех случаев, когда команда не может разрешить идентификатор хранилища.</span><span class="sxs-lookup"><span data-stu-id="a1348-349">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> <span data-ttu-id="a1348-350">[#5718](https://github.com/Azure/azure-cli/issues/5718).</span><span class="sxs-lookup"><span data-stu-id="a1348-350">[#5718](https://github.com/Azure/azure-cli/issues/5718)</span></span>
* <span data-ttu-id="a1348-351">Улучшены сообщения об ошибках для команды `[vm|vmss create]`, когда расположение группы ресурсов не поддерживает зоны.</span><span class="sxs-lookup"><span data-stu-id="a1348-351">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="a1348-352">27 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a1348-352">March 27, 2018</span></span>

<span data-ttu-id="a1348-353">Версия 2.0.30</span><span class="sxs-lookup"><span data-stu-id="a1348-353">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="a1348-354">Core</span><span class="sxs-lookup"><span data-stu-id="a1348-354">Core</span></span>

* <span data-ttu-id="a1348-355">Отображение сообщения для расширений, которые отмечены в справке как предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="a1348-355">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="a1348-356">ACS</span><span class="sxs-lookup"><span data-stu-id="a1348-356">ACS</span></span>

* <span data-ttu-id="a1348-357">Устранена ошибка с проверкой SSL-сертификата для `aks install-cli` в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="a1348-357">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="a1348-358">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a1348-358">Appservice</span></span>

* <span data-ttu-id="a1348-359">Добавлена поддержка только протокола HTTPS для `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="a1348-359">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="a1348-360">Добавлена поддержка слотов для `az webapp identity [assign|show]` и `az functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="a1348-360">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="a1348-361">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="a1348-361">Backup</span></span>

* <span data-ttu-id="a1348-362">Добавлена новая команда `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="a1348-362">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="a1348-363">Эта команда используется для проверки резервного копирования виртуальной машины в любое хранилище в подписке.</span><span class="sxs-lookup"><span data-stu-id="a1348-363">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="a1348-364">Включены идентификаторы объектов Azure для параметров `--resource-group` и `--vault-name` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="a1348-364">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="a1348-365">Изменены параметры `--name` для поддержки формата вывода команд `backup ... show`.</span><span class="sxs-lookup"><span data-stu-id="a1348-365">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="a1348-366">Контейнер</span><span class="sxs-lookup"><span data-stu-id="a1348-366">Container</span></span>

* <span data-ttu-id="a1348-367">Добавлена команда `container exec`.</span><span class="sxs-lookup"><span data-stu-id="a1348-367">Added `container exec` command.</span></span> <span data-ttu-id="a1348-368">Выполнение команды в контейнере для выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="a1348-368">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="a1348-369">Разрешение выходной таблице создавать и обновлять группу контейнеров.</span><span class="sxs-lookup"><span data-stu-id="a1348-369">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="a1348-370">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="a1348-370">Extension</span></span>

* <span data-ttu-id="a1348-371">Добавлено сообщение для `extension add`, если расширение доступно в режиме предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="a1348-371">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="a1348-372">Изменен параметр `extension list-available` для отображения всех данных расширения с использованием `--show-details`.</span><span class="sxs-lookup"><span data-stu-id="a1348-372">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="a1348-373">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменена команда `extension list-available` для отображения упрощенных данных расширения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a1348-373">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="a1348-374">Interactive</span><span class="sxs-lookup"><span data-stu-id="a1348-374">Interactive</span></span>

* <span data-ttu-id="a1348-375">Изменены операции завершения, активируемые сразу после завершения загрузки таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="a1348-375">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="a1348-376">Исправлена ошибка с использованием параметра `--style`.</span><span class="sxs-lookup"><span data-stu-id="a1348-376">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="a1348-377">Отсутствующий интерактивный лексический анализатор создается после дампа таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="a1348-377">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="a1348-378">Улучшена поддержка средства заполнения.</span><span class="sxs-lookup"><span data-stu-id="a1348-378">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="a1348-379">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="a1348-379">Lab</span></span>

* <span data-ttu-id="a1348-380">Исправлены ошибки с командой `create environment`.</span><span class="sxs-lookup"><span data-stu-id="a1348-380">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="a1348-381">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="a1348-381">Monitor</span></span>

* <span data-ttu-id="a1348-382">Добавлена поддержка `--top`, `--orderby` и `--namespace` для `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="a1348-382">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="a1348-383">Исправлена ошибка [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` принимает разделенный пробелами список метрик для извлечения.</span><span class="sxs-lookup"><span data-stu-id="a1348-383">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="a1348-384">Добавлена поддержка `--namespace` для `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="a1348-384">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="a1348-385">Сеть</span><span class="sxs-lookup"><span data-stu-id="a1348-385">Network</span></span>

* <span data-ttu-id="a1348-386">Добавлена поддержка Частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="a1348-386">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="a1348-387">Профиль</span><span class="sxs-lookup"><span data-stu-id="a1348-387">Profile</span></span>

* <span data-ttu-id="a1348-388">Добавлено предупреждение для `--identity-port` и `--msi-port` в `login`.</span><span class="sxs-lookup"><span data-stu-id="a1348-388">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="a1348-389">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="a1348-389">RDBMS</span></span>

* <span data-ttu-id="a1348-390">Добавлена общедоступная версия 2017-12-01 бизнес-модели API.</span><span class="sxs-lookup"><span data-stu-id="a1348-390">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="a1348-391">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a1348-391">Resource</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="a1348-393">Роль</span><span class="sxs-lookup"><span data-stu-id="a1348-393">Role</span></span>

* <span data-ttu-id="a1348-394">Добавлена поддержка конфигурации требуемого уровня доступа и собственных клиентов для `az ad app create`.</span><span class="sxs-lookup"><span data-stu-id="a1348-394">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="a1348-395">Изменены команды `rbac`, чтобы возвращать не более 1000 идентификаторов в разрешении объекта.</span><span class="sxs-lookup"><span data-stu-id="a1348-395">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="a1348-396">Добавлены команды `ad sp credential [reset|list|delete]` для управления учетными данными.</span><span class="sxs-lookup"><span data-stu-id="a1348-396">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="a1348-397">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр properties из выходных данных `az role assignment [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="a1348-397">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="a1348-398">Добавлена поддержка разрешений `dataActions` и `notDataActions` для `role definition`.</span><span class="sxs-lookup"><span data-stu-id="a1348-398">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="a1348-399">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="a1348-399">Storage</span></span>

* <span data-ttu-id="a1348-400">Исправлена проблема с отправкой файла размером от 195 до 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="a1348-400">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="a1348-401">Исправлена ошибка [#4049](https://github.com/Azure/azure-cli/issues/4049): проблемы, когда при отправке добавочного большого двоичного объекта игнорируются параметры условия.</span><span class="sxs-lookup"><span data-stu-id="a1348-401">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="a1348-402">ВМ</span><span class="sxs-lookup"><span data-stu-id="a1348-402">VM</span></span>

* <span data-ttu-id="a1348-403">Добавлено предупреждение `vmss create` для предстоящих критически важных изменений для наборов из 100 и более экземпляров.</span><span class="sxs-lookup"><span data-stu-id="a1348-403">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="a1348-404">Добавлена поддержка устойчивости зон для `vm [snapshot|image]`.</span><span class="sxs-lookup"><span data-stu-id="a1348-404">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="a1348-405">Изменено представление экземпляра диска для улучшения отчета о состоянии шифрования.</span><span class="sxs-lookup"><span data-stu-id="a1348-405">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="a1348-406">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] `vm extension delete` Изменена команда, которая больше не возвращает выходные данные.</span><span class="sxs-lookup"><span data-stu-id="a1348-406">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="a1348-407">13 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a1348-407">March 13, 2018</span></span>

<span data-ttu-id="a1348-408">Версия 2.0.29</span><span class="sxs-lookup"><span data-stu-id="a1348-408">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="a1348-409">ACR</span><span class="sxs-lookup"><span data-stu-id="a1348-409">ACR</span></span>

* <span data-ttu-id="a1348-410">Добавлена поддержка параметра `--image` для `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="a1348-410">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="a1348-411">Параметры `--manifest` и `--tag` команды `repository delete` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="a1348-411">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="a1348-412">Добавлена команда `repository untag` для удаления тега без удаления данных.</span><span class="sxs-lookup"><span data-stu-id="a1348-412">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="a1348-413">ACS</span><span class="sxs-lookup"><span data-stu-id="a1348-413">ACS</span></span>

* <span data-ttu-id="a1348-414">Добавлена команда `aks upgrade-connector` для обновления существующего соединителя.</span><span class="sxs-lookup"><span data-stu-id="a1348-414">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="a1348-415">Изменены файлы конфигурации `kubectl`. Теперь используется более разборчивый стиль YAML с разбивкой на блоки.</span><span class="sxs-lookup"><span data-stu-id="a1348-415">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="a1348-416">Помощник</span><span class="sxs-lookup"><span data-stu-id="a1348-416">Advisor</span></span>

* <span data-ttu-id="a1348-417">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration get` переименована в `advisor configuration list`.</span><span class="sxs-lookup"><span data-stu-id="a1348-417">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="a1348-418">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration set` переименована в `advisor configuration update`.</span><span class="sxs-lookup"><span data-stu-id="a1348-418">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="a1348-419">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `advisor recommendation generate`.</span><span class="sxs-lookup"><span data-stu-id="a1348-419">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span> 
* <span data-ttu-id="a1348-420">Добавлен параметр `--refresh` для команды `advisor recommendation list`.</span><span class="sxs-lookup"><span data-stu-id="a1348-420">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="a1348-421">Добавлена команда `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="a1348-421">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="a1348-422">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a1348-422">Appservice</span></span>

* <span data-ttu-id="a1348-423">Команда `[webapp|functionapp] assign-identity` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="a1348-423">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="a1348-424">Добавлены команды управляемого удостоверения `webapp identity [assign|show]` и `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="a1348-424">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="a1348-425">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="a1348-425">Eventhubs</span></span>

* <span data-ttu-id="a1348-426">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="a1348-426">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="a1348-427">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="a1348-427">Extension</span></span>

* <span data-ttu-id="a1348-428">Добавлена проверка, позволяющая предупредить пользователя, если используемый дистрибутив отличается от хранящегося в исходном файле пакета, так как это может привести к возникновению ошибок.</span><span class="sxs-lookup"><span data-stu-id="a1348-428">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="a1348-429">Interactive</span><span class="sxs-lookup"><span data-stu-id="a1348-429">Interactive</span></span>

* <span data-ttu-id="a1348-430">Исправлена ошибка [#5625](https://github.com/Azure/azure-cli/issues/5625): теперь записи журнала сохраняются в разных сеансах.</span><span class="sxs-lookup"><span data-stu-id="a1348-430">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="a1348-431">Исправлена ошибка [#3016](https://github.com/Azure/azure-cli/issues/3016): при использовании области не создавались записи журнала.</span><span class="sxs-lookup"><span data-stu-id="a1348-431">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="a1348-432">Исправлена ошибка [#5688](https://github.com/Azure/azure-cli/issues/5688): если при загрузке таблицы команд возникало исключение, опережающий ввод не выполнялся.</span><span class="sxs-lookup"><span data-stu-id="a1348-432">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="a1348-433">Исправлен индикатор хода выполнения для длительных операций.</span><span class="sxs-lookup"><span data-stu-id="a1348-433">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="a1348-434">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="a1348-434">Monitor</span></span>

* <span data-ttu-id="a1348-435">Команды `monitor autoscale-settings` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="a1348-435">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="a1348-436">Добавлены команды `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="a1348-436">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="a1348-437">Добавлены команды `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="a1348-437">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="a1348-438">Добавлены команды `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="a1348-438">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="a1348-439">Сеть</span><span class="sxs-lookup"><span data-stu-id="a1348-439">Network</span></span>

* <span data-ttu-id="a1348-440">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--tags` из `route-filter rule create`.</span><span class="sxs-lookup"><span data-stu-id="a1348-440">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="a1348-441">Удалены некоторые ошибочные значения по умолчанию для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="a1348-441">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="a1348-442">Добавлены команды `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="a1348-442">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="a1348-443">Добавлены параметры `--vnet` и `--subnet` для `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="a1348-443">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="a1348-444">Профиль</span><span class="sxs-lookup"><span data-stu-id="a1348-444">Profile</span></span>

* <span data-ttu-id="a1348-445">Параметр `--msi` для `az login` отмечен как нерекомендуемый.</span><span class="sxs-lookup"><span data-stu-id="a1348-445">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="a1348-446">Добавлен параметр `--identity` для `az login`. Он заменяет `--msi`.</span><span class="sxs-lookup"><span data-stu-id="a1348-446">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="a1348-447">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="a1348-447">RDBMS</span></span>

* <span data-ttu-id="a1348-448">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Внесены изменения для использования предварительной версии API 2017-12-01.</span><span class="sxs-lookup"><span data-stu-id="a1348-448">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="a1348-449">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="a1348-449">Service Bus</span></span>

* <span data-ttu-id="a1348-450">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="a1348-450">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="a1348-451">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="a1348-451">Storage</span></span>

* <span data-ttu-id="a1348-452">Исправлена ошибка [#4971](https://github.com/Azure/azure-cli/issues/4971): теперь `storage blob copy` поддерживает другие облака Azure.</span><span class="sxs-lookup"><span data-stu-id="a1348-452">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="a1348-453">Исправлена ошибка [#5286](https://github.com/Azure/azure-cli/issues/5286): при пакетном выполнении команд `storage blob [delete-batch|download-batch|upload-batch]` больше не отображается сообщение об ошибке в предусловии.</span><span class="sxs-lookup"><span data-stu-id="a1348-453">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="a1348-454">ВМ</span><span class="sxs-lookup"><span data-stu-id="a1348-454">VM</span></span>

* <span data-ttu-id="a1348-455">В `[vm|vmss] create` добавлена поддержка присоединения неуправляемых дисков данных и настройки кэширования.</span><span class="sxs-lookup"><span data-stu-id="a1348-455">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="a1348-456">`[vm|vmss] assign-identity` и `[vm|vmss] remove-identity` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="a1348-456">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="a1348-457">Вместо нерекомендуемых команд добавлены команды `vm identity [assign|remove|show]` и `vmss identity [assign|remove|show]`.</span><span class="sxs-lookup"><span data-stu-id="a1348-457">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="a1348-458">Для приоритета `vmss create` по умолчанию установлено значение None.</span><span class="sxs-lookup"><span data-stu-id="a1348-458">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="a1348-459">27 февраля 2018 г</span><span class="sxs-lookup"><span data-stu-id="a1348-459">February 27, 2018</span></span>

<span data-ttu-id="a1348-460">Версия 2.0.28</span><span class="sxs-lookup"><span data-stu-id="a1348-460">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="a1348-461">Core</span><span class="sxs-lookup"><span data-stu-id="a1348-461">Core</span></span>

* <span data-ttu-id="a1348-462">Исправлена ошибка с установкой Homebrew [№ 5184](https://github.com/Azure/azure-cli/issues/5184).</span><span class="sxs-lookup"><span data-stu-id="a1348-462">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="a1348-463">Добавлена поддержка телеметрии расширения с применением пользовательских ключей.</span><span class="sxs-lookup"><span data-stu-id="a1348-463">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="a1348-464">Добавлена функция ведения журнала HTTP в `--debug`.</span><span class="sxs-lookup"><span data-stu-id="a1348-464">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="a1348-465">ACS</span><span class="sxs-lookup"><span data-stu-id="a1348-465">ACS</span></span>

* <span data-ttu-id="a1348-466">Изменено для использования диаграмм Helm `virtual-kubelet-for-aks` для `aks install-connector` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a1348-466">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="a1348-467">Исправлена ошибка с недостаточными разрешениями субъектов-служб на создание групп контейнеров ACI.</span><span class="sxs-lookup"><span data-stu-id="a1348-467">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="a1348-468">Добавлены параметры `--aci-container-group`, `--location` и `--image-tag` для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="a1348-468">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="a1348-469">Удалено уведомление об устаревании из `aks get-versions`.</span><span class="sxs-lookup"><span data-stu-id="a1348-469">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="a1348-470">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a1348-470">Appservice</span></span>

* <span data-ttu-id="a1348-471">Обновления для новой версии пакета SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="a1348-471">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="a1348-472">Исправлена ошибка с сообщением `Free` о недопустимом SKU [№ 5538](https://github.com/Azure/azure-cli/issues/5538)</span><span class="sxs-lookup"><span data-stu-id="a1348-472">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="a1348-473">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="a1348-473">Cognitive Services</span></span>

* <span data-ttu-id="a1348-474">Обновлено уведомление при создании новой учетной записи Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="a1348-474">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="a1348-475">Потребление</span><span class="sxs-lookup"><span data-stu-id="a1348-475">Consumption</span></span>

* <span data-ttu-id="a1348-476">Добавлены новые команды для резервирования API прейскуранта.</span><span class="sxs-lookup"><span data-stu-id="a1348-476">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="a1348-477">Обновлены существующие форматы сведений об использовании и резервировании.</span><span class="sxs-lookup"><span data-stu-id="a1348-477">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="a1348-478">Контейнер</span><span class="sxs-lookup"><span data-stu-id="a1348-478">Container</span></span>

* <span data-ttu-id="a1348-479">Добавлены аргументы `--secrets` и `--secrets-mount-path` в командах `container create` для использования секретов в ACI.</span><span class="sxs-lookup"><span data-stu-id="a1348-479">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="a1348-480">Сеть</span><span class="sxs-lookup"><span data-stu-id="a1348-480">Network</span></span>

* <span data-ttu-id="a1348-481">Исправлена ошибка с отсутствующим клиентом в `network vnet-gateway vpn-client generate` [№ 5559](https://github.com/Azure/azure-cli/issues/5559).</span><span class="sxs-lookup"><span data-stu-id="a1348-481">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="a1348-482">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a1348-482">Resource</span></span>

* <span data-ttu-id="a1348-483">Изменено `group deployment export` для отображения частичного шаблона и ошибок при сбое.</span><span class="sxs-lookup"><span data-stu-id="a1348-483">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="a1348-484">Роль</span><span class="sxs-lookup"><span data-stu-id="a1348-484">Role</span></span>

* <span data-ttu-id="a1348-485">Добавлено `role assignment list-changelogs` для включения аудита ролей субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="a1348-485">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="a1348-486">SQL</span><span class="sxs-lookup"><span data-stu-id="a1348-486">SQL</span></span>

* <span data-ttu-id="a1348-487">Добавлена поддержка избыточности зон для создания и обновления баз данных и эластичных пулов.</span><span class="sxs-lookup"><span data-stu-id="a1348-487">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="a1348-488">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="a1348-488">Storage</span></span>

* <span data-ttu-id="a1348-489">Включено определение пути назначения и префикса для `storage blob [upload-batch|download-batch]`.</span><span class="sxs-lookup"><span data-stu-id="a1348-489">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="a1348-490">ВМ</span><span class="sxs-lookup"><span data-stu-id="a1348-490">VM</span></span>

* <span data-ttu-id="a1348-491">Добавлена поддержка присоединения и отсоединения дисков на одном экземпляре VMSS.</span><span class="sxs-lookup"><span data-stu-id="a1348-491">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="a1348-492">13 февраля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a1348-492">February 13, 2018</span></span>

<span data-ttu-id="a1348-493">Версия 2.0.27</span><span class="sxs-lookup"><span data-stu-id="a1348-493">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="a1348-494">Core</span><span class="sxs-lookup"><span data-stu-id="a1348-494">Core</span></span>

* <span data-ttu-id="a1348-495">Изменен способ аутентификации при входе с помощью MSI: применяется ключ при использовании идентификатора подписки и имени.</span><span class="sxs-lookup"><span data-stu-id="a1348-495">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="a1348-496">ACS</span><span class="sxs-lookup"><span data-stu-id="a1348-496">ACS</span></span>

* <span data-ttu-id="a1348-497">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименовано `aks get-versions` на `aks get-upgrades` для точности.</span><span class="sxs-lookup"><span data-stu-id="a1348-497">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="a1348-498">Изменено `aks get-versions` для отображения версий Kubernetes, доступных для `aks create`.</span><span class="sxs-lookup"><span data-stu-id="a1348-498">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="a1348-499">Изменены значения по умолчанию `aks create`, чтобы разрешить серверу выбирать версию Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="a1348-499">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="a1348-500">Обновлены справочные сообщения, связанные с субъектом-службой и создаваемые AKS.</span><span class="sxs-lookup"><span data-stu-id="a1348-500">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="a1348-501">Изменены стандартные размеры узла для `aks create` с уровня Standard\_D1\_v2 на уровень Standard\_DS1\_v2.</span><span class="sxs-lookup"><span data-stu-id="a1348-501">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="a1348-502">Улучшена надежность при поиске панели мониторинга для группы pod для `az aks browse`.</span><span class="sxs-lookup"><span data-stu-id="a1348-502">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="a1348-503">Исправлена команда `aks get-credentials` для обработки ошибок Юникода при загрузке файлов конфигурации Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="a1348-503">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="a1348-504">Добавлено сообщение в `az aks install-cli`, чтобы помочь получить `kubectl` в `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="a1348-504">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="a1348-505">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a1348-505">Appservice</span></span>

* <span data-ttu-id="a1348-506">Исправлена проблема со сбоем `webapp [backup|restore]` из-за пустой ссылки.</span><span class="sxs-lookup"><span data-stu-id="a1348-506">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="a1348-507">Добавлена поддержка стандартных планов службы приложений с помощью `az configure --defaults appserviceplan=my-asp`.</span><span class="sxs-lookup"><span data-stu-id="a1348-507">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="a1348-508">CDN</span><span class="sxs-lookup"><span data-stu-id="a1348-508">CDN</span></span>

* <span data-ttu-id="a1348-509">Добавлены команды `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="a1348-509">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="a1348-510">Контейнер</span><span class="sxs-lookup"><span data-stu-id="a1348-510">Container</span></span>

* <span data-ttu-id="a1348-511">Добавлен параметр `--follow` для `az container logs` для журналов потоковой передачи.</span><span class="sxs-lookup"><span data-stu-id="a1348-511">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="a1348-512">Добавлена команда `container attach`, которая добавляет локальный стандартный поток вывода и поток вывода сообщений об ошибках к контейнеру в группе контейнеров.</span><span class="sxs-lookup"><span data-stu-id="a1348-512">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a1348-513">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="a1348-513">CosmosDB</span></span>

* <span data-ttu-id="a1348-514">Добавлена поддержка настройки параметров.</span><span class="sxs-lookup"><span data-stu-id="a1348-514">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="a1348-515">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="a1348-515">Extension</span></span>

* <span data-ttu-id="a1348-516">Добавлена поддержка параметра `--pip-proxy` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="a1348-516">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="a1348-517">Добавлена поддержка аргумента `--pip-extra-index-urls` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="a1348-517">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="a1348-518">Отзыв</span><span class="sxs-lookup"><span data-stu-id="a1348-518">Feedback</span></span>

* <span data-ttu-id="a1348-519">Добавлены сведения о расширении к данным телеметрии.</span><span class="sxs-lookup"><span data-stu-id="a1348-519">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="a1348-520">Interactive</span><span class="sxs-lookup"><span data-stu-id="a1348-520">Interactive</span></span>

* <span data-ttu-id="a1348-521">Исправлена проблема, когда пользователю предлагалось войти в интерактивном режиме в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="a1348-521">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="a1348-522">Исправлена регрессия с отсутствующей функцией заполнения параметров.</span><span class="sxs-lookup"><span data-stu-id="a1348-522">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="a1348-523">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="a1348-523">IoT</span></span>

* <span data-ttu-id="a1348-524">Исправлена проблема, когда `iot dps access policy [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="a1348-524">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="a1348-525">Исправлена проблема, когда `iot dps linked-hub [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="a1348-525">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="a1348-526">Добавлена поддержка параметра `--no-wait` для `iot dps access policy [create|update]` и `iot dps linked-hub [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="a1348-526">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="a1348-527">Изменена команда `iot hub create` для указания числа секций.</span><span class="sxs-lookup"><span data-stu-id="a1348-527">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="a1348-528">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="a1348-528">Monitor</span></span>

* <span data-ttu-id="a1348-529">Исправлена команда `az monitor log-profiles create`.</span><span class="sxs-lookup"><span data-stu-id="a1348-529">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="a1348-530">Сеть</span><span class="sxs-lookup"><span data-stu-id="a1348-530">Network</span></span>

* <span data-ttu-id="a1348-531">Исправлен параметр `--tags` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="a1348-531">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="a1348-532">Профиль</span><span class="sxs-lookup"><span data-stu-id="a1348-532">Profile</span></span>

* <span data-ttu-id="a1348-533">Включена команда `az login` для использования в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="a1348-533">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="a1348-534">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a1348-534">Resource</span></span>

* <span data-ttu-id="a1348-535">Снова добавлена команда `feature show`.</span><span class="sxs-lookup"><span data-stu-id="a1348-535">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="a1348-536">Роль</span><span class="sxs-lookup"><span data-stu-id="a1348-536">Role</span></span>

* <span data-ttu-id="a1348-537">Добавлен аргумент `--available-to-other-tenants` для команды `ad app update`</span><span class="sxs-lookup"><span data-stu-id="a1348-537">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="a1348-538">SQL</span><span class="sxs-lookup"><span data-stu-id="a1348-538">SQL</span></span>

* <span data-ttu-id="a1348-539">Добавлены команды `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="a1348-539">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="a1348-540">Добавлена команда `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="a1348-540">Added `sql db rename`</span></span>
* <span data-ttu-id="a1348-541">Добавлена поддержка аргумента `--ids` для команд SQL.</span><span class="sxs-lookup"><span data-stu-id="a1348-541">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="a1348-542">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="a1348-542">Storage</span></span>

* <span data-ttu-id="a1348-543">Добавлены команды `storage blob service-properties delete-policy` и `storage blob undelete` для включения обратимого удаления.</span><span class="sxs-lookup"><span data-stu-id="a1348-543">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="a1348-544">ВМ</span><span class="sxs-lookup"><span data-stu-id="a1348-544">VM</span></span>

* <span data-ttu-id="a1348-545">Исправлена ошибка, когда шифрование виртуальной машины инициализировалось не полностью.</span><span class="sxs-lookup"><span data-stu-id="a1348-545">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="a1348-546">Добавлены выходные данные идентификатора субъекта для включения MSI.</span><span class="sxs-lookup"><span data-stu-id="a1348-546">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="a1348-547">Фиксированное значение `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="a1348-547">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="a1348-548">31 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a1348-548">January 31, 2018</span></span>

<span data-ttu-id="a1348-549">Версия 2.0.26</span><span class="sxs-lookup"><span data-stu-id="a1348-549">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="a1348-550">Core</span><span class="sxs-lookup"><span data-stu-id="a1348-550">Core</span></span>

* <span data-ttu-id="a1348-551">Добавлена поддержка получения необработанного маркера в контексте MSI.</span><span class="sxs-lookup"><span data-stu-id="a1348-551">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="a1348-552">Удалена строка индикатора опроса после завершения LRO при выполнении cmd.exe в Windows.</span><span class="sxs-lookup"><span data-stu-id="a1348-552">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="a1348-553">Добавлено предупреждение, которое появляется при использовании настроенных по умолчанию параметров, измененных на запись уровня INFO.</span><span class="sxs-lookup"><span data-stu-id="a1348-553">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="a1348-554">Используйте `--verbose` для просмотра.</span><span class="sxs-lookup"><span data-stu-id="a1348-554">Use `--verbose` to see</span></span>
* <span data-ttu-id="a1348-555">Добавьте индикатор хода выполнения для ожидания команд.</span><span class="sxs-lookup"><span data-stu-id="a1348-555">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="a1348-556">ACS</span><span class="sxs-lookup"><span data-stu-id="a1348-556">ACS</span></span>

* <span data-ttu-id="a1348-557">Добавлено описание аргумента `--disable-browser`.</span><span class="sxs-lookup"><span data-stu-id="a1348-557">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="a1348-558">Улучшено заполнение нажатием клавиши TAB для аргументов `--vm-size`.</span><span class="sxs-lookup"><span data-stu-id="a1348-558">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="a1348-559">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a1348-559">Appservice</span></span>

* <span data-ttu-id="a1348-560">Фиксированное значение `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="a1348-560">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="a1348-561">Удалена проверка `kind` в веб-приложениях и функциях.</span><span class="sxs-lookup"><span data-stu-id="a1348-561">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="a1348-562">CDN</span><span class="sxs-lookup"><span data-stu-id="a1348-562">CDN</span></span>

* <span data-ttu-id="a1348-563">Устранена проблема с отсутствием клиента для команды `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="a1348-563">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a1348-564">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="a1348-564">CosmosDB</span></span>

* <span data-ttu-id="a1348-565">Исправлено описание параметров для политик отработки отказа.</span><span class="sxs-lookup"><span data-stu-id="a1348-565">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="a1348-566">Interactive</span><span class="sxs-lookup"><span data-stu-id="a1348-566">Interactive</span></span>

* <span data-ttu-id="a1348-567">Исправлена проблема, когда заполнение параметров команд больше не выполнялось.</span><span class="sxs-lookup"><span data-stu-id="a1348-567">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="a1348-568">Сеть</span><span class="sxs-lookup"><span data-stu-id="a1348-568">Network</span></span>

* <span data-ttu-id="a1348-569">Добавлена защита `--cert-password` для `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="a1348-569">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="a1348-570">Исправлена проблема с `application-gateway update`, когда команда `--sku` ошибочно применяла значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a1348-570">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="a1348-571">Добавлена защита `--shared-key` и `--authorization-key` для `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="a1348-571">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="a1348-572">Устранена проблема с отсутствием клиента для команды `asg create`.</span><span class="sxs-lookup"><span data-stu-id="a1348-572">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="a1348-573">Добавлен параметр `--file-name / -f` для экспортируемых имен в `dns zone export`.</span><span class="sxs-lookup"><span data-stu-id="a1348-573">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="a1348-574">Исправлены следующие ошибки для `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="a1348-574">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="a1348-575">Исправлена проблема, когда длинные записи ТХТ неправильно экспортировались.</span><span class="sxs-lookup"><span data-stu-id="a1348-575">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="a1348-576">Исправлена проблема, когда записи ТХТ в кавычках неправильно экспортировались без символов экранирования.</span><span class="sxs-lookup"><span data-stu-id="a1348-576">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="a1348-577">Исправлена проблема, когда некоторые записи импортировались дважды с помощью `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="a1348-577">Fixed issue where certain records were imported twice with `dns zone import`</span></span> 
* <span data-ttu-id="a1348-578">Восстановлены команды `vnet-gateway root-cert` и `vnet-gateway revoked-cert`.</span><span class="sxs-lookup"><span data-stu-id="a1348-578">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="a1348-579">Профиль</span><span class="sxs-lookup"><span data-stu-id="a1348-579">Profile</span></span>

* <span data-ttu-id="a1348-580">Исправлена команда `get-access-token` для работы в виртуальной машине с идентификатором.</span><span class="sxs-lookup"><span data-stu-id="a1348-580">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="a1348-581">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a1348-581">Resource</span></span>

* <span data-ttu-id="a1348-582">Исправлена ошибка с `deployment [create|validate]`, когда предупреждение неправильно отображалось, если поле type шаблона содержало значения в верхнем регистре.</span><span class="sxs-lookup"><span data-stu-id="a1348-582">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="a1348-583">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="a1348-583">Storage</span></span>

* <span data-ttu-id="a1348-584">Исправлена проблема с переносом учетных записей хранения из версии 1 в версию 2.</span><span class="sxs-lookup"><span data-stu-id="a1348-584">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="a1348-585">Добавлены отчеты о ходе выполнения всех команд отправки или скачивания.</span><span class="sxs-lookup"><span data-stu-id="a1348-585">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="a1348-586">Исправлена ошибка, которая препятствовала использованию параметра аргумента -n с `storage account check-name`.</span><span class="sxs-lookup"><span data-stu-id="a1348-586">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>  
* <span data-ttu-id="a1348-587">Добавлен столбец snapshot в табличные выходные данные для `blob [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="a1348-587">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="a1348-588">Исправлены ошибки с разными параметрами, которые должны были анализироваться как целые числа.</span><span class="sxs-lookup"><span data-stu-id="a1348-588">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="a1348-589">ВМ</span><span class="sxs-lookup"><span data-stu-id="a1348-589">VM</span></span>

* <span data-ttu-id="a1348-590">Добавлена команда `vm image accept-terms` для разрешения создания виртуальных машин из образов с дополнительными расходами.</span><span class="sxs-lookup"><span data-stu-id="a1348-590">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="a1348-591">Исправлена команда `[vm|vmss create]` для выполнения команд с прокси-сервера с помощью неподписанных сертификатов.</span><span class="sxs-lookup"><span data-stu-id="a1348-591">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="a1348-592">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка режима низкого приоритета для VMSS.</span><span class="sxs-lookup"><span data-stu-id="a1348-592">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="a1348-593">Добавлена защита `--admin-password` для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="a1348-593">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="a1348-594">17 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a1348-594">January 17, 2018</span></span>

<span data-ttu-id="a1348-595">Версия 2.0.25</span><span class="sxs-lookup"><span data-stu-id="a1348-595">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="a1348-596">ACR</span><span class="sxs-lookup"><span data-stu-id="a1348-596">ACR</span></span>

* <span data-ttu-id="a1348-597">Добавлена возможность отката входа ACR при ошибках учетных данных в Windows.</span><span class="sxs-lookup"><span data-stu-id="a1348-597">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="a1348-598">Включены журналы реестра.</span><span class="sxs-lookup"><span data-stu-id="a1348-598">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="a1348-599">ACS</span><span class="sxs-lookup"><span data-stu-id="a1348-599">ACS</span></span>

* <span data-ttu-id="a1348-600">Исправлена команда `get-credentials`.</span><span class="sxs-lookup"><span data-stu-id="a1348-600">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="a1348-601">Удалено требование роли для имени субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="a1348-601">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="a1348-602">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a1348-602">Appservice</span></span>

* <span data-ttu-id="a1348-603">Исправлена ошибка с `config ssl upload`, при которой значение `hosting_environment_profile` было NULL.</span><span class="sxs-lookup"><span data-stu-id="a1348-603">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="a1348-604">В `browse` добавлена поддержка для пользовательских URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="a1348-604">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="a1348-605">Исправлена поддержка слотов для `log tail`.</span><span class="sxs-lookup"><span data-stu-id="a1348-605">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="a1348-606">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="a1348-606">Backup</span></span>

* <span data-ttu-id="a1348-607">Параметр `--container-name` для `backup item list` теперь не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="a1348-607">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="a1348-608">В `backup restore restore-disks` добавлены варианты учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="a1348-608">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="a1348-609">Для проверки расположения в `backup protection enable-for-vm` добавлена чувствительность к регистру.</span><span class="sxs-lookup"><span data-stu-id="a1348-609">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="a1348-610">Устранена проблема, при которой команды завершались сбоем с указанием недопустимого имени контейнера.</span><span class="sxs-lookup"><span data-stu-id="a1348-610">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="a1348-611">В `backup item list` теперь по умолчанию включен параметр Health Status.</span><span class="sxs-lookup"><span data-stu-id="a1348-611">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="a1348-612">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="a1348-612">Batch</span></span>

* <span data-ttu-id="a1348-613">`batch login` теперь возвращает сведения об аутентификации.</span><span class="sxs-lookup"><span data-stu-id="a1348-613">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="a1348-614">Облако</span><span class="sxs-lookup"><span data-stu-id="a1348-614">Cloud</span></span>

* <span data-ttu-id="a1348-615">При установке `--profile` в облаке теперь не требуется указывать конечные точки.</span><span class="sxs-lookup"><span data-stu-id="a1348-615">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="a1348-616">Потребление</span><span class="sxs-lookup"><span data-stu-id="a1348-616">Consumption</span></span>

* <span data-ttu-id="a1348-617">Добавлены новые команды для резервирования: `consumption reservations summaries` и `consumption reservations details`.</span><span class="sxs-lookup"><span data-stu-id="a1348-617">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="a1348-618">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="a1348-618">Event Grid</span></span>

* <span data-ttu-id="a1348-619">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid topic event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="a1348-619">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="a1348-620">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid resource event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="a1348-620">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="a1348-621">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="a1348-621">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="a1348-622">Вместо нее следует использовать `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="a1348-622">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="a1348-623">Добавлена команда `eventgrid topic update`.</span><span class="sxs-lookup"><span data-stu-id="a1348-623">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="a1348-624">Добавлена команда `eventgrid event-subscription update`.</span><span class="sxs-lookup"><span data-stu-id="a1348-624">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="a1348-625">Добавлен параметр `--ids` для команд `eventgrid topic`.</span><span class="sxs-lookup"><span data-stu-id="a1348-625">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="a1348-626">Добавлена поддержка заполнения нажатием клавиши TAB для имен разделов.</span><span class="sxs-lookup"><span data-stu-id="a1348-626">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="a1348-627">Interactive</span><span class="sxs-lookup"><span data-stu-id="a1348-627">Interactive</span></span>

* <span data-ttu-id="a1348-628">Устранена проблема, при которой интерактивный режим не работал с Python 2.x.</span><span class="sxs-lookup"><span data-stu-id="a1348-628">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="a1348-629">Исправлены ошибки при запуске.</span><span class="sxs-lookup"><span data-stu-id="a1348-629">Fixed errors on startup</span></span>
* <span data-ttu-id="a1348-630">Устранена проблема, при которой некоторые команды не работали в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="a1348-630">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="a1348-631">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="a1348-631">IoT</span></span>

* <span data-ttu-id="a1348-632">Добавлена поддержка службы подготовки устройств.</span><span class="sxs-lookup"><span data-stu-id="a1348-632">Added support for device provisioning service</span></span>
* <span data-ttu-id="a1348-633">В команды и справочную информацию о них добавлены сообщения о нерекомендуемых версиях.</span><span class="sxs-lookup"><span data-stu-id="a1348-633">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="a1348-634">Теперь при проверке Интернета вещей указывается расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="a1348-634">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="a1348-635">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="a1348-635">Monitor</span></span>

* <span data-ttu-id="a1348-636">Добавлена поддержка параметра нескольких диагностических операций.</span><span class="sxs-lookup"><span data-stu-id="a1348-636">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="a1348-637">Теперь параметр `--name` является обязательным для `az monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="a1348-637">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="a1348-638">Добавлена команда `monitor diagnostic-settings categories` для получения категории параметров диагностики.</span><span class="sxs-lookup"><span data-stu-id="a1348-638">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="a1348-639">Сеть</span><span class="sxs-lookup"><span data-stu-id="a1348-639">Network</span></span>

* <span data-ttu-id="a1348-640">Устранена проблема с `vnet-gateway update` при попытке входа в активный режим и режим ожидания или выхода из них.</span><span class="sxs-lookup"><span data-stu-id="a1348-640">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="a1348-641">Для `application-gateway [create|update]` добавлена поддержка HTTP2.</span><span class="sxs-lookup"><span data-stu-id="a1348-641">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="a1348-642">Профиль</span><span class="sxs-lookup"><span data-stu-id="a1348-642">Profile</span></span>

* <span data-ttu-id="a1348-643">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="a1348-643">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="a1348-644">Роль</span><span class="sxs-lookup"><span data-stu-id="a1348-644">Role</span></span>

* <span data-ttu-id="a1348-645">В `role assignment create` добавлен аргумент `--assignee-object-id`, чтобы обойти запрос графов.</span><span class="sxs-lookup"><span data-stu-id="a1348-645">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="a1348-646">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="a1348-646">Service Fabric</span></span>

* <span data-ttu-id="a1348-647">В результат проверки при создании кластера добавлены подробные сведения об ошибках.</span><span class="sxs-lookup"><span data-stu-id="a1348-647">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="a1348-648">Устранена проблема отсутствия клиента при выполнении некоторых команд.</span><span class="sxs-lookup"><span data-stu-id="a1348-648">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="a1348-649">ВМ</span><span class="sxs-lookup"><span data-stu-id="a1348-649">VM</span></span>

* <span data-ttu-id="a1348-650">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Поддержка разных зон для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="a1348-650">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="a1348-651">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию `vmss` для одной зоны заменено данными подсистемы балансировки нагрузки уровня "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="a1348-651">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="a1348-652">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для EMSI параметр `externalIdentities` изменен на `userAssignedIdentities`.</span><span class="sxs-lookup"><span data-stu-id="a1348-652">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="a1348-653">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка переключения дисков ОС.</span><span class="sxs-lookup"><span data-stu-id="a1348-653">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="a1348-654">Добавлена поддержка использования образов виртуальных машин из других подписок.</span><span class="sxs-lookup"><span data-stu-id="a1348-654">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="a1348-655">В `[vm|vmss] create` добавлены аргументы `--plan-name`, `--plan-product`, `--plan-promotion-code` и `--plan-publisher`.</span><span class="sxs-lookup"><span data-stu-id="a1348-655">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="a1348-656">Устранены проблемы с `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="a1348-656">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="a1348-657">Устранена проблема чрезмерного использования ресурсов из-за `vm image list --all`.</span><span class="sxs-lookup"><span data-stu-id="a1348-657">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="a1348-658">19 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="a1348-658">December 19, 2017</span></span>

<span data-ttu-id="a1348-659">Версия 2.0.23</span><span class="sxs-lookup"><span data-stu-id="a1348-659">Version 2.0.23</span></span>

* <span data-ttu-id="a1348-660">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="a1348-660">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="a1348-661">Контейнер</span><span class="sxs-lookup"><span data-stu-id="a1348-661">Container</span></span>

* <span data-ttu-id="a1348-662">Исправлен неправильный порядок параметров для журналов контейнеров.</span><span class="sxs-lookup"><span data-stu-id="a1348-662">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="a1348-663">Сеть</span><span class="sxs-lookup"><span data-stu-id="a1348-663">Network</span></span>

* <span data-ttu-id="a1348-664">Добавлен аргумент `--disable-bgp-route-propagation` для команды `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a1348-664">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="a1348-665">Добавлен аргумент `--ip-tags` для команды `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a1348-665">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="a1348-666">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="a1348-666">Storage</span></span>

* <span data-ttu-id="a1348-667">Добавлена поддержка хранилища версии 2.</span><span class="sxs-lookup"><span data-stu-id="a1348-667">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="a1348-668">ВМ</span><span class="sxs-lookup"><span data-stu-id="a1348-668">VM</span></span>

* <span data-ttu-id="a1348-669">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для назначенных пользователям удостоверений для виртуальных машин и VMSS.</span><span class="sxs-lookup"><span data-stu-id="a1348-669">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="a1348-670">5 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="a1348-670">December 5, 2017</span></span>

<span data-ttu-id="a1348-671">Версия 2.0.22</span><span class="sxs-lookup"><span data-stu-id="a1348-671">Version 2.0.22</span></span>

* <span data-ttu-id="a1348-672">Удалена команда `az component`.</span><span class="sxs-lookup"><span data-stu-id="a1348-672">Removed `az component` commands.</span></span> <span data-ttu-id="a1348-673">Вместо нее следует использовать `az extension`.</span><span class="sxs-lookup"><span data-stu-id="a1348-673">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="a1348-674">Core</span><span class="sxs-lookup"><span data-stu-id="a1348-674">Core</span></span>
* <span data-ttu-id="a1348-675">Конечная точка `AZURE_US_GOV_CLOUD` центра AAD изменена с login.microsoftonline.com на login.microsoftonline.us.</span><span class="sxs-lookup"><span data-stu-id="a1348-675">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="a1348-676">Исправлена проблема с непрерывной отправкой телеметрии.</span><span class="sxs-lookup"><span data-stu-id="a1348-676">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="a1348-677">ACS</span><span class="sxs-lookup"><span data-stu-id="a1348-677">ACS</span></span>

* <span data-ttu-id="a1348-678">Добавлены команды `aks install-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="a1348-678">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="a1348-679">Улучшены сообщения об ошибках для команды `acs create`.</span><span class="sxs-lookup"><span data-stu-id="a1348-679">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="a1348-680">Добавлена возможность использования команды `aks get-credentials -f` без полного пути.</span><span class="sxs-lookup"><span data-stu-id="a1348-680">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="a1348-681">Помощник</span><span class="sxs-lookup"><span data-stu-id="a1348-681">Advisor</span></span>

* <span data-ttu-id="a1348-682">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="a1348-682">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="a1348-683">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a1348-683">Appservice</span></span>

* <span data-ttu-id="a1348-684">Добавлена возможность создания имени сертификата с помощью команды `webapp config ssl upload`.</span><span class="sxs-lookup"><span data-stu-id="a1348-684">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="a1348-685">Исправлены команды `webapp [list|show]` и `functionapp [list|show]` для отображения правильных приложений.</span><span class="sxs-lookup"><span data-stu-id="a1348-685">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="a1348-686">Добавлено стандартное значение для переменной `WEBSITE_NODE_DEFAULT_VERSION`.</span><span class="sxs-lookup"><span data-stu-id="a1348-686">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="a1348-687">Потребление</span><span class="sxs-lookup"><span data-stu-id="a1348-687">Consumption</span></span>

* <span data-ttu-id="a1348-688">Добавлена поддержка API версии 2017-11-30.</span><span class="sxs-lookup"><span data-stu-id="a1348-688">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="a1348-689">Контейнер</span><span class="sxs-lookup"><span data-stu-id="a1348-689">Container</span></span>

* <span data-ttu-id="a1348-690">Исправлены стандартные порты регрессии.</span><span class="sxs-lookup"><span data-stu-id="a1348-690">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="a1348-691">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="a1348-691">Monitor</span></span>

* <span data-ttu-id="a1348-692">Добавлена поддержка нескольких измерений для команд метрик.</span><span class="sxs-lookup"><span data-stu-id="a1348-692">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="a1348-693">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a1348-693">Resource</span></span>

* <span data-ttu-id="a1348-694">Добавлен аргумент `--include-response-body` для команды `resource show`</span><span class="sxs-lookup"><span data-stu-id="a1348-694">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="a1348-695">Роль</span><span class="sxs-lookup"><span data-stu-id="a1348-695">Role</span></span>

* <span data-ttu-id="a1348-696">Добавлено отображение стандартных назначений "классических" администраторов для команды `role assignment list`.</span><span class="sxs-lookup"><span data-stu-id="a1348-696">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="a1348-697">Добавлена поддержка команды `ad sp reset-credentials` для добавления учетных данных вместо перезаписи.</span><span class="sxs-lookup"><span data-stu-id="a1348-697">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="a1348-698">Улучшены сообщения об ошибках для команды `ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="a1348-698">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="a1348-699">SQL</span><span class="sxs-lookup"><span data-stu-id="a1348-699">SQL</span></span>

* <span data-ttu-id="a1348-700">Добавлены команды `sql db list-usages` и `sql db show-usage`.</span><span class="sxs-lookup"><span data-stu-id="a1348-700">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="a1348-701">Добавлены команды `sql server conn-policy show` и `sql server conn-policy update`.</span><span class="sxs-lookup"><span data-stu-id="a1348-701">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="a1348-702">ВМ</span><span class="sxs-lookup"><span data-stu-id="a1348-702">VM</span></span>

* <span data-ttu-id="a1348-703">Добавлены сведения о зонах для команды `az vm list-skus`.</span><span class="sxs-lookup"><span data-stu-id="a1348-703">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="a1348-704">14 ноября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="a1348-704">November 14, 2017</span></span>

<span data-ttu-id="a1348-705">Версия 2.0.21</span><span class="sxs-lookup"><span data-stu-id="a1348-705">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="a1348-706">ACR</span><span class="sxs-lookup"><span data-stu-id="a1348-706">ACR</span></span>

* <span data-ttu-id="a1348-707">Добавлена поддержка создания веб-перехватчиков в регионах репликации.</span><span class="sxs-lookup"><span data-stu-id="a1348-707">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="a1348-708">ACS</span><span class="sxs-lookup"><span data-stu-id="a1348-708">ACS</span></span>

* <span data-ttu-id="a1348-709">В AKS агент теперь называется узлом.</span><span class="sxs-lookup"><span data-stu-id="a1348-709">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="a1348-710">Параметр `--orchestrator-release` для командлета `acs create` не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="a1348-710">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="a1348-711">Изменен размер виртуальной машины для AKS по умолчанию на `Standard_D1_v2`.</span><span class="sxs-lookup"><span data-stu-id="a1348-711">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="a1348-712">Исправлена команда `az aks browse` для Windows.</span><span class="sxs-lookup"><span data-stu-id="a1348-712">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="a1348-713">Исправлена команда `az aks get-credentials` для Windows.</span><span class="sxs-lookup"><span data-stu-id="a1348-713">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="a1348-714">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a1348-714">Appservice</span></span>

* <span data-ttu-id="a1348-715">Добавлен источник развертывания `config-zip` для веб-приложений и приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="a1348-715">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="a1348-716">Добавлен параметр `--docker-container-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="a1348-716">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="a1348-717">Удален параметр `storage` из параметра `--web-server-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="a1348-717">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="a1348-718">Улучшены сообщения об ошибках для команды `deployment user set`.</span><span class="sxs-lookup"><span data-stu-id="a1348-718">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="a1348-719">Добавлена поддержка создания приложений-функций Linux</span><span class="sxs-lookup"><span data-stu-id="a1348-719">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="a1348-720">Фиксированное значение `list-locations`</span><span class="sxs-lookup"><span data-stu-id="a1348-720">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="a1348-721">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="a1348-721">Batch</span></span>

* <span data-ttu-id="a1348-722">Исправлена ошибка в команде создания пула, когда идентификатор ресурса использовался с флагом `--image`.</span><span class="sxs-lookup"><span data-stu-id="a1348-722">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="a1348-723">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="a1348-723">Batchai</span></span>

* <span data-ttu-id="a1348-724">Добавлен короткий параметр `-s` для параметра `--vm-size` при указании размера виртуальной машины в команде `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="a1348-724">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="a1348-725">Добавлены аргументы ключа и имени учетной записи хранения в параметры команды `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="a1348-725">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="a1348-726">Исправлена документация по командам `job list-files` и `job stream-file`.</span><span class="sxs-lookup"><span data-stu-id="a1348-726">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="a1348-727">Добавлен короткий параметр `-r` для параметра `--cluster-name` при указании имени кластера в команде `job create`.</span><span class="sxs-lookup"><span data-stu-id="a1348-727">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="a1348-728">Облако</span><span class="sxs-lookup"><span data-stu-id="a1348-728">Cloud</span></span>

* <span data-ttu-id="a1348-729">Изменена команда `cloud [register|update]` для предотвращения регистрации облаков, для которых отсутствуют необходимые конечные точки.</span><span class="sxs-lookup"><span data-stu-id="a1348-729">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="a1348-730">Контейнер</span><span class="sxs-lookup"><span data-stu-id="a1348-730">Container</span></span>

* <span data-ttu-id="a1348-731">Добавлена поддержка открытия нескольких портов.</span><span class="sxs-lookup"><span data-stu-id="a1348-731">Added support to open multiple ports</span></span>
* <span data-ttu-id="a1348-732">Добавлена политика перезапуска группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="a1348-732">Added container group restart policy</span></span>
* <span data-ttu-id="a1348-733">Добавлена поддержка подключения файлового ресурса Azure в качестве тома.</span><span class="sxs-lookup"><span data-stu-id="a1348-733">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="a1348-734">Обновлена вспомогательная документация.</span><span class="sxs-lookup"><span data-stu-id="a1348-734">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="a1348-735">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="a1348-735">Data Lake Analytics</span></span>

* <span data-ttu-id="a1348-736">Изменена команда `[job|account] list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="a1348-736">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="a1348-737">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a1348-737">Data Lake Store</span></span>

* <span data-ttu-id="a1348-738">Изменена команда `account list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="a1348-738">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="a1348-739">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="a1348-739">Extension</span></span>

* <span data-ttu-id="a1348-740">Добавлена команда `extension list-available` для отображения официальных расширений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="a1348-740">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="a1348-741">Добавлен параметр `--name` для команды `extension [add|update]` для установки расширений по имени.</span><span class="sxs-lookup"><span data-stu-id="a1348-741">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="a1348-742">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="a1348-742">IoT</span></span>

* <span data-ttu-id="a1348-743">Добавлена поддержка центров сертификации (ЦС) и цепочек сертификатов.</span><span class="sxs-lookup"><span data-stu-id="a1348-743">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="a1348-744">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="a1348-744">Monitor</span></span>

* <span data-ttu-id="a1348-745">Добавлены команды `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="a1348-745">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="a1348-746">Сеть</span><span class="sxs-lookup"><span data-stu-id="a1348-746">Network</span></span>

* <span data-ttu-id="a1348-747">Добавлена поддержка DNS-записей типа CAA.</span><span class="sxs-lookup"><span data-stu-id="a1348-747">Added support for CAA DNS records</span></span>
* <span data-ttu-id="a1348-748">Исправлена проблема, когда конечные точки могли не обновляться с помощью команды `traffic-manager profile update`.</span><span class="sxs-lookup"><span data-stu-id="a1348-748">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="a1348-749">Исправлена проблема, когда команда `vnet update --dns-servers` не работала в зависимости от способа создания виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="a1348-749">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="a1348-750">Исправлена проблема, когда относительные DNS-имена неправильно импортировались с помощью команды `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="a1348-750">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="a1348-751">Резервирование</span><span class="sxs-lookup"><span data-stu-id="a1348-751">Reservations</span></span>

* <span data-ttu-id="a1348-752">Первоначальный выпуск предварительной версии</span><span class="sxs-lookup"><span data-stu-id="a1348-752">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="a1348-753">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a1348-753">Resource</span></span>

* <span data-ttu-id="a1348-754">Добавлена поддержка идентификаторов ресурсов для блокировок на уровне ресурсов и параметра `--resource`.</span><span class="sxs-lookup"><span data-stu-id="a1348-754">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="a1348-755">SQL</span><span class="sxs-lookup"><span data-stu-id="a1348-755">SQL</span></span>

* <span data-ttu-id="a1348-756">Добавлен параметр `--ignore-missing-vnet-service-endpoint` для команды `sql server vnet-rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="a1348-756">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="a1348-757">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="a1348-757">Storage</span></span>

* <span data-ttu-id="a1348-758">Изменена команда `storage account create` для использования номера SKU `Standard_RAGRS` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a1348-758">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="a1348-759">Исправлены ошибки при обработке имени файла или большого двоичного объекта, содержащего символы, отличные от ASCII.</span><span class="sxs-lookup"><span data-stu-id="a1348-759">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="a1348-760">Исправлена ошибка, препятствующая использованию параметра `--source-uri` с командой `storage [blob|file] copy start-batch`.</span><span class="sxs-lookup"><span data-stu-id="a1348-760">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="a1348-761">Добавлены команды для удаления нескольких объектов с помощью команды `storage [blob|file] delete-batch`.</span><span class="sxs-lookup"><span data-stu-id="a1348-761">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="a1348-762">Исправлена проблема с включением метрик с помощью команды `storage metrics update`.</span><span class="sxs-lookup"><span data-stu-id="a1348-762">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="a1348-763">Исправлена проблема с файлами более 200 ГБ при использовании команды `storage blob upload-batch`.</span><span class="sxs-lookup"><span data-stu-id="a1348-763">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="a1348-764">Исправлена проблема, когда параметры `--bypass` и `--default-action` игнорировались командой `storage account [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="a1348-764">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="a1348-765">ВМ</span><span class="sxs-lookup"><span data-stu-id="a1348-765">VM</span></span>

* <span data-ttu-id="a1348-766">Исправлена ошибка с командой `vmss create`, препятствующая использованию уровня `Basic`.</span><span class="sxs-lookup"><span data-stu-id="a1348-766">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="a1348-767">Добавлены аргументы `--plan` для команды `[vm|vmss] create` для пользовательских образов с информацией о выставлении счетов.</span><span class="sxs-lookup"><span data-stu-id="a1348-767">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="a1348-768">Добавлены команды `vm secret `[add|remove|list]\`.</span><span class="sxs-lookup"><span data-stu-id="a1348-768">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="a1348-769">Команда `vm format-secret` переименована в `vm secret format`.</span><span class="sxs-lookup"><span data-stu-id="a1348-769">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="a1348-770">Добавлен аргумент `--encrypt format` для команды `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="a1348-770">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="a1348-771">24 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="a1348-771">October 24, 2017</span></span>

<span data-ttu-id="a1348-772">Версия 2.0.20</span><span class="sxs-lookup"><span data-stu-id="a1348-772">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="a1348-773">Core</span><span class="sxs-lookup"><span data-stu-id="a1348-773">Core</span></span>

* <span data-ttu-id="a1348-774">Обновление `2017-03-09-profile` для использования API `MGMT_STORAGE` версии `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="a1348-774">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="a1348-775">ACR</span><span class="sxs-lookup"><span data-stu-id="a1348-775">ACR</span></span>

* <span data-ttu-id="a1348-776">Обновление службы управления ресурсами для указания API версии `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="a1348-776">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="a1348-777">Изменение номера SKU BYOS-хранилища на "Классический"</span><span class="sxs-lookup"><span data-stu-id="a1348-777">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="a1348-778">Переименование номеров SKU реестра на "Базовый", "Стандартный" и "Премиум"</span><span class="sxs-lookup"><span data-stu-id="a1348-778">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="a1348-779">ACS</span><span class="sxs-lookup"><span data-stu-id="a1348-779">ACS</span></span>

* <span data-ttu-id="a1348-780">[ПРЕДВАРИЕТЛЬНАЯ ВЕРСИЯ] Добавление команд `az aks`</span><span class="sxs-lookup"><span data-stu-id="a1348-780">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="a1348-781">Исправление Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="a1348-781">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="a1348-782">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a1348-782">Appservice</span></span>

* <span data-ttu-id="a1348-783">Исправление проблемы с недопустимыми скачанными журналами `webapp`</span><span class="sxs-lookup"><span data-stu-id="a1348-783">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="a1348-784">Компонент</span><span class="sxs-lookup"><span data-stu-id="a1348-784">Component</span></span>

* <span data-ttu-id="a1348-785">Добавление более понятного сообщения об устаревании для всех установщиков, а также запроса на подтверждение</span><span class="sxs-lookup"><span data-stu-id="a1348-785">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="a1348-786">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="a1348-786">Monitor</span></span>

* <span data-ttu-id="a1348-787">Добавлены команды `action-group`.</span><span class="sxs-lookup"><span data-stu-id="a1348-787">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="a1348-788">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a1348-788">Resource</span></span>

* <span data-ttu-id="a1348-789">Исправление несовместимости с самой последней версии зависимости msrest в `group export`</span><span class="sxs-lookup"><span data-stu-id="a1348-789">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="a1348-790">Исправление `policy assignment create` для работы с определениями встроенных политик и наборов политик</span><span class="sxs-lookup"><span data-stu-id="a1348-790">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="a1348-791">ВМ</span><span class="sxs-lookup"><span data-stu-id="a1348-791">VM</span></span>

* <span data-ttu-id="a1348-792">Добавлен аргумент `--accelerated-networking` для команды `vmss create`</span><span class="sxs-lookup"><span data-stu-id="a1348-792">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="a1348-793">9 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="a1348-793">October 9, 2017</span></span>

<span data-ttu-id="a1348-794">Версия 2.0.19</span><span class="sxs-lookup"><span data-stu-id="a1348-794">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="a1348-795">Core</span><span class="sxs-lookup"><span data-stu-id="a1348-795">Core</span></span>

* <span data-ttu-id="a1348-796">В Azure Stack добавлена обработка URL-адресов центра ADFS с завершающей косой чертой.</span><span class="sxs-lookup"><span data-stu-id="a1348-796">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="a1348-797">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a1348-797">Appservice</span></span>

* <span data-ttu-id="a1348-798">Добавлена возможность общего обновления с помощью новой команды `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="a1348-798">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="a1348-799">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="a1348-799">Batch</span></span>

* <span data-ttu-id="a1348-800">Обновление до пакета SDK для пакетной службы версии 4.0.0</span><span class="sxs-lookup"><span data-stu-id="a1348-800">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="a1348-801">Обновлен параметр `--image` для команды VirtualMachineConfiguration, обеспечивающий поддержку ссылок на образы ARM в дополнение к publish:offer:sku:version.</span><span class="sxs-lookup"><span data-stu-id="a1348-801">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="a1348-802">Добавлена поддержка новой модели расширений CLI для команд расширений пакетной службы.</span><span class="sxs-lookup"><span data-stu-id="a1348-802">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="a1348-803">Удалена поддержка пакетной службы для модели компонентов.</span><span class="sxs-lookup"><span data-stu-id="a1348-803">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="a1348-804">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="a1348-804">Batchai</span></span>

* <span data-ttu-id="a1348-805">Исходный выпуск модуля искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="a1348-805">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="a1348-806">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="a1348-806">Keyvault</span></span>

* <span data-ttu-id="a1348-807">Исправлена проблема с аутентификацией Key Vault при использовании ADFS в Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="a1348-807">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="a1348-808">(#4448)</span><span class="sxs-lookup"><span data-stu-id="a1348-808">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="a1348-809">Сеть</span><span class="sxs-lookup"><span data-stu-id="a1348-809">Network</span></span>

* <span data-ttu-id="a1348-810">Аргумент `--server` для `application-gateway address-pool create` изменен на необязательный (разрешено использование пустых пулов адресов).</span><span class="sxs-lookup"><span data-stu-id="a1348-810">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="a1348-811">Обновлен элемент `traffic-manager` для поддержки последних функций.</span><span class="sxs-lookup"><span data-stu-id="a1348-811">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="a1348-812">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a1348-812">Resource</span></span>

* <span data-ttu-id="a1348-813">Добавлена поддержка параметров `--resource-group/-g` для изменения имени группы ресурсов на `group`.</span><span class="sxs-lookup"><span data-stu-id="a1348-813">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="a1348-814">Добавлены команды для `account lock` для работы с блокировками на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="a1348-814">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="a1348-815">Добавлены команды для `group lock` для работы с блокировками на уровне группы.</span><span class="sxs-lookup"><span data-stu-id="a1348-815">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="a1348-816">Добавлены команды для `resource lock` для работы с блокировками на уровне ресурса.</span><span class="sxs-lookup"><span data-stu-id="a1348-816">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="a1348-817">SQL</span><span class="sxs-lookup"><span data-stu-id="a1348-817">Sql</span></span>

* <span data-ttu-id="a1348-818">Добавлена поддержка SQL TDE и BYOK TDE.</span><span class="sxs-lookup"><span data-stu-id="a1348-818">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="a1348-819">Добавлена команда `db list-deleted` и параметр `db restore --deleted-time` для поиска и восстановления удаленных баз данных.</span><span class="sxs-lookup"><span data-stu-id="a1348-819">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="a1348-820">Добавлено `db op list` и `db op cancel` для отображения и отмены выполняющихся операций в базе данных.</span><span class="sxs-lookup"><span data-stu-id="a1348-820">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="a1348-821">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="a1348-821">Storage</span></span>

* <span data-ttu-id="a1348-822">Добавлена поддержка моментальных снимков файловых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="a1348-822">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="a1348-823">Виртуальные машины</span><span class="sxs-lookup"><span data-stu-id="a1348-823">Vm</span></span>

* <span data-ttu-id="a1348-824">Исправлена ошибка в команде `vm show`, когда использование `-d` вызывало сбой отсутствующих частных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="a1348-824">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="a1348-825">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка последовательного обновления для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="a1348-825">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="a1348-826">Добавлена поддержка обновления параметров шифрования с помощью команды `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="a1348-826">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="a1348-827">Добавлен параметр `--os-disk-size-gb` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="a1348-827">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="a1348-828">Добавлен параметр `--license-type` для команды `vmss create` (для Windows).</span><span class="sxs-lookup"><span data-stu-id="a1348-828">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="a1348-829">22 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="a1348-829">September 22, 2017</span></span>

<span data-ttu-id="a1348-830">Версия 2.0.18</span><span class="sxs-lookup"><span data-stu-id="a1348-830">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="a1348-831">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a1348-831">Resource</span></span>

* <span data-ttu-id="a1348-832">Добавлена поддержка отображения определений встроенных политик</span><span class="sxs-lookup"><span data-stu-id="a1348-832">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="a1348-833">Добавлена поддержка параметра mode для создания определения политик</span><span class="sxs-lookup"><span data-stu-id="a1348-833">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="a1348-834">Добавлена поддержка шаблонов и определений пользовательского интерфейса для команды `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="a1348-834">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="a1348-835">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен тип ресурса `managedapp` с `appliances` на `applications` и с `applianceDefinitions` на `applicationDefinitions`.</span><span class="sxs-lookup"><span data-stu-id="a1348-835">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="a1348-836">Сеть</span><span class="sxs-lookup"><span data-stu-id="a1348-836">Network</span></span>

* <span data-ttu-id="a1348-837">Добавлена поддержка зоны доступности для подкоманд `network lb` и `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="a1348-837">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="a1348-838">Добавлена поддержка IPv6 (пиринг Майкрософт) для `express-route`</span><span class="sxs-lookup"><span data-stu-id="a1348-838">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="a1348-839">Добавлены команды группы безопасности приложения `asg`</span><span class="sxs-lookup"><span data-stu-id="a1348-839">Added `asg` application security group commands</span></span>
* <span data-ttu-id="a1348-840">Добавлен аргумент `--application-security-groups` для команды `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="a1348-840">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="a1348-841">Добавлены аргументы `--source-asgs` и `--destination-asgs` для команды `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a1348-841">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="a1348-842">Добавлены аргументы `--ddos-protection` и `--vm-protection` для команды `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a1348-842">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="a1348-843">Добавлены команды `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="a1348-843">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="a1348-844">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="a1348-844">Storage</span></span>

* <span data-ttu-id="a1348-845">Исправлена проблема, когда команды `storage account network-rule` могут не работать после обновления пакета SDK</span><span class="sxs-lookup"><span data-stu-id="a1348-845">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="a1348-846">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="a1348-846">Eventgrid</span></span>

* <span data-ttu-id="a1348-847">Обновлен пакет SDK Python для службы "Сетка событий Azure" для использования новой версии API 2017-09-15-preview</span><span class="sxs-lookup"><span data-stu-id="a1348-847">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="a1348-848">SQL</span><span class="sxs-lookup"><span data-stu-id="a1348-848">SQL</span></span>

* <span data-ttu-id="a1348-849">Аргумент `--resource-group` для команды `sql server list` сделан необязательным.</span><span class="sxs-lookup"><span data-stu-id="a1348-849">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="a1348-850">Если он не указан, возвращаются все серверы SQL Server в подписке</span><span class="sxs-lookup"><span data-stu-id="a1348-850">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="a1348-851">Добавлен параметр `--no-wait` для команд `db [create|copy|restore|update|replica create|create|update]` и `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a1348-851">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="a1348-852">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="a1348-852">Keyvault</span></span>

* <span data-ttu-id="a1348-853">Добавлена поддержка команд хранилища ключей за прокси-сервером</span><span class="sxs-lookup"><span data-stu-id="a1348-853">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="a1348-854">ВМ</span><span class="sxs-lookup"><span data-stu-id="a1348-854">VM</span></span>

* <span data-ttu-id="a1348-855">Добавлена поддержка зоны доступности для команды `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="a1348-855">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="a1348-856">Исправлена проблема, когда использование аргумента `--app-gateway ID` с командой `vmss create` приводило к сбою</span><span class="sxs-lookup"><span data-stu-id="a1348-856">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="a1348-857">Добавлен аргумент `--asgs` для команды `vm create`</span><span class="sxs-lookup"><span data-stu-id="a1348-857">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="a1348-858">Добавлена поддержка выполнения команд на виртуальных машинах с помощью команды `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="a1348-858">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="a1348-859">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка шифрования диска VMSS с помощью команды `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="a1348-859">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="a1348-860">Добавлена поддержка обслуживания виртуальных машин с помощью команды `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="a1348-860">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="a1348-861">ACS</span><span class="sxs-lookup"><span data-stu-id="a1348-861">ACS</span></span>

* <span data-ttu-id="a1348-862">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлен аргумент `--orchestrator-release` для команды `acs create` для регионов служб ACS (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="a1348-862">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="a1348-863">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a1348-863">Appservice</span></span>

* <span data-ttu-id="a1348-864">Добавлена возможность обновлять и отображать параметры аутентификации с помощью команды `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="a1348-864">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="a1348-865">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="a1348-865">Backup</span></span>

* <span data-ttu-id="a1348-866">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="a1348-866">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="a1348-867">11 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="a1348-867">September 11, 2017</span></span>

<span data-ttu-id="a1348-868">Версия 2.0.17</span><span class="sxs-lookup"><span data-stu-id="a1348-868">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="a1348-869">Core</span><span class="sxs-lookup"><span data-stu-id="a1348-869">Core</span></span>

* <span data-ttu-id="a1348-870">Включен командный модуль для настройки собственного идентификатора корреляции в телеметрии.</span><span class="sxs-lookup"><span data-stu-id="a1348-870">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="a1348-871">Исправлена проблема с дампом JSON, когда для телеметрии настроен режим диагностики.</span><span class="sxs-lookup"><span data-stu-id="a1348-871">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="a1348-872">ACS</span><span class="sxs-lookup"><span data-stu-id="a1348-872">Acs</span></span>

* <span data-ttu-id="a1348-873">Добавлена команда `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="a1348-873">Added `acs list-locations` command</span></span>
* <span data-ttu-id="a1348-874">Для `ssh-key-file` предоставляется ожидаемое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a1348-874">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="a1348-875">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a1348-875">Appservice</span></span>

* <span data-ttu-id="a1348-876">Добавлена возможность создавать веб-приложения в группе ресурсов в рамках плана службы, отличной от активной.</span><span class="sxs-lookup"><span data-stu-id="a1348-876">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="a1348-877">CDN</span><span class="sxs-lookup"><span data-stu-id="a1348-877">CDN</span></span>

* <span data-ttu-id="a1348-878">Исправлена ошибка "CustomDomain не пригоден к итерации" для `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="a1348-878">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="a1348-879">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="a1348-879">Extension</span></span>

* <span data-ttu-id="a1348-880">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="a1348-880">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="a1348-881">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="a1348-881">Keyvault</span></span>

* <span data-ttu-id="a1348-882">Исправлена проблема с зависимостью разрешений от регистра для `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="a1348-882">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="a1348-883">Сеть</span><span class="sxs-lookup"><span data-stu-id="a1348-883">Network</span></span>

* <span data-ttu-id="a1348-884">Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="a1348-884">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="a1348-885">Аргумент `--private-access-services` переименован в `--service-endpoints` для команды `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="a1348-885">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="a1348-886">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="a1348-886">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="a1348-887">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="a1348-887">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="a1348-888">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="a1348-888">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="a1348-889">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a1348-889">Resource</span></span>

* <span data-ttu-id="a1348-890">Разрешена передача в определениях параметров политики ресурсов в командах `policy definition create` и `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="a1348-890">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="a1348-891">Разрешена передача значений параметров для команды `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="a1348-891">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="a1348-892">Разрешена передача JSON или файла для всех параметров.</span><span class="sxs-lookup"><span data-stu-id="a1348-892">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="a1348-893">Версия API изменена на более позднюю.</span><span class="sxs-lookup"><span data-stu-id="a1348-893">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="a1348-894">SQL</span><span class="sxs-lookup"><span data-stu-id="a1348-894">SQL</span></span>

* <span data-ttu-id="a1348-895">Добавлены команды `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="a1348-895">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="a1348-896">ВМ</span><span class="sxs-lookup"><span data-stu-id="a1348-896">VM</span></span>

* <span data-ttu-id="a1348-897">Исправлено: не назначать доступ, если `--scope` не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="a1348-897">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="a1348-898">Исправлено: использование тех же расширений имен, что и для портала.</span><span class="sxs-lookup"><span data-stu-id="a1348-898">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="a1348-899">Удалено `subscription` из выходных данных `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="a1348-899">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="a1348-900">Исправлено: номер SKU хранилища `[vm|vmss] create` неприменим для дисков данных с образом.</span><span class="sxs-lookup"><span data-stu-id="a1348-900">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="a1348-901">Исправлено: `vm format-secret --secrets` не принимает идентификаторы, разделенные строками.</span><span class="sxs-lookup"><span data-stu-id="a1348-901">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="a1348-902">31 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="a1348-902">August 31, 2017</span></span>

<span data-ttu-id="a1348-903">Версия 2.0.16</span><span class="sxs-lookup"><span data-stu-id="a1348-903">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="a1348-904">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="a1348-904">Keyvault</span></span>

* <span data-ttu-id="a1348-905">Исправлена ошибка при попытке автоматически разрешить шифрование секрета с помощью `secret download`.</span><span class="sxs-lookup"><span data-stu-id="a1348-905">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="a1348-906">Sf</span><span class="sxs-lookup"><span data-stu-id="a1348-906">Sf</span></span>

* <span data-ttu-id="a1348-907">Объявлены неподдерживаемыми все команды; вместо них используется Service Fabric CLI (sfctl).</span><span class="sxs-lookup"><span data-stu-id="a1348-907">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="a1348-908">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="a1348-908">Storage</span></span>

* <span data-ttu-id="a1348-909">Исправлена проблема, когда учетные записи хранения нельзя было создавать в регионах, которые не поддерживают функцию NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="a1348-909">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="a1348-910">Определение типа и кодировки содержимого во время передачи больших двоичных объектов и файла, если оба свойства не указаны.</span><span class="sxs-lookup"><span data-stu-id="a1348-910">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="a1348-911">28 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="a1348-911">August 28, 2017</span></span>

<span data-ttu-id="a1348-912">Версия 2.0.15</span><span class="sxs-lookup"><span data-stu-id="a1348-912">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="a1348-913">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="a1348-913">CLI</span></span>

* <span data-ttu-id="a1348-914">Для `--version` добавлено юридическое примечание.</span><span class="sxs-lookup"><span data-stu-id="a1348-914">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="a1348-915">ACS</span><span class="sxs-lookup"><span data-stu-id="a1348-915">ACS</span></span>

* <span data-ttu-id="a1348-916">Исправлены регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="a1348-916">Corrected preview regions</span></span>
* <span data-ttu-id="a1348-917">Правильно отформатирован параметр по умолчанию `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="a1348-917">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="a1348-918">Оптимизированы выходные данные команды ACS.</span><span class="sxs-lookup"><span data-stu-id="a1348-918">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="a1348-919">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a1348-919">Appservice</span></span>

* <span data-ttu-id="a1348-920">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправлены несоответствия в выходных данных `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="a1348-920">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="a1348-921">Добавлен новый псевдоним `-i` в команду `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="a1348-921">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="a1348-922">Предоставлена команда `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="a1348-922">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="a1348-923">Предоставлены новые аргументы команды `az webapp delete`, которые позволяют сохранить план службы приложений, метрики и данные регистрации DNS.</span><span class="sxs-lookup"><span data-stu-id="a1348-923">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="a1348-924">Исправление. Параметры слота определяются правильно.</span><span class="sxs-lookup"><span data-stu-id="a1348-924">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="a1348-925">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="a1348-925">IoT</span></span>

* <span data-ttu-id="a1348-926">Исправление 3934. При создании политики существующие политики больше не удаляются.</span><span class="sxs-lookup"><span data-stu-id="a1348-926">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="a1348-927">Сеть</span><span class="sxs-lookup"><span data-stu-id="a1348-927">Network</span></span>

* <span data-ttu-id="a1348-928">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="a1348-928">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="a1348-929">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--private-access-services` переименован в `--service-endpoints` в командах `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="a1348-929">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="a1348-930">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="a1348-930">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="a1348-931">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="a1348-931">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="a1348-932">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="a1348-932">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="a1348-933">Профиль</span><span class="sxs-lookup"><span data-stu-id="a1348-933">Profile</span></span>

* <span data-ttu-id="a1348-934">Предоставлены параметры `--msi` и `--msi-port` для входа с использованием удостоверения виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="a1348-934">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="a1348-935">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="a1348-935">Service Fabric</span></span>

* <span data-ttu-id="a1348-936">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="a1348-936">Preview release</span></span>
* <span data-ttu-id="a1348-937">Упрощены правила реестра для паролей и имен пользователя для команды.</span><span class="sxs-lookup"><span data-stu-id="a1348-937">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="a1348-938">Исправлена строка для ввода пароля пользователем даже после передачи параметра.</span><span class="sxs-lookup"><span data-stu-id="a1348-938">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="a1348-939">Добавлена поддержка пустого значения `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="a1348-939">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="a1348-940">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="a1348-940">Storage</span></span>

* <span data-ttu-id="a1348-941">Появилась возможность задавать уровень большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="a1348-941">Enabled setting blob tier</span></span>
* <span data-ttu-id="a1348-942">Добавлены аргументы `--bypass` и `--default-action` в командах `storage account [create|update]` для поддержки туннелирования службы.</span><span class="sxs-lookup"><span data-stu-id="a1348-942">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="a1348-943">Добавлены команды для добавления правил виртуальной сети и правил на основе IP-адресов в `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="a1348-943">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="a1348-944">Разрешено шифрование службы с управляемым пользователем ключом.</span><span class="sxs-lookup"><span data-stu-id="a1348-944">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="a1348-945">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--encryption` переименован в `--encryption-services` в команде `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="a1348-945">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="a1348-946">Исправление 4220. Несоответствие синтаксиса `az storage account update encryption`.</span><span class="sxs-lookup"><span data-stu-id="a1348-946">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="a1348-947">ВМ</span><span class="sxs-lookup"><span data-stu-id="a1348-947">VM</span></span>

* <span data-ttu-id="a1348-948">Исправлена проблема, из-за которой для команды `vmss get-instance-view` отображались лишние и неправильные сведения при использовании параметра `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="a1348-948">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="a1348-949">Добавлена поддержка параметра `--lb-sku` в команде `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="a1348-949">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="a1348-950">Из черного списка имен администраторов для команд `[vm|vmss] create` удалены имена людей.</span><span class="sxs-lookup"><span data-stu-id="a1348-950">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="a1348-951">Исправлена проблема, из-за которой команда `[vm|vmss] create` выдавала ошибку, если из образа не удавалось извлечь сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="a1348-951">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="a1348-952">Исправлена проблема, которая приводила к сбою при создании масштабируемого набора виртуальных машин с внутренней подсистемой балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="a1348-952">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="a1348-953">Исправлена проблема, из-за которой аргумент `--no-wait` не работал с командой `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="a1348-953">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="a1348-954">15 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="a1348-954">August 15, 2017</span></span>

<span data-ttu-id="a1348-955">Версия 2.0.14</span><span class="sxs-lookup"><span data-stu-id="a1348-955">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="a1348-956">ACS</span><span class="sxs-lookup"><span data-stu-id="a1348-956">ACS</span></span>

* <span data-ttu-id="a1348-957">Исправлен номер порта sshMaster0 для Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="a1348-957">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="a1348-958">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a1348-958">Appservice</span></span>

* <span data-ttu-id="a1348-959">Исправлено исключение при создании веб-приложения Linux на основе Git.</span><span class="sxs-lookup"><span data-stu-id="a1348-959">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="a1348-960">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="a1348-960">Event Grid</span></span>

* <span data-ttu-id="a1348-961">Добавлены зависимости пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="a1348-961">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="a1348-962">11 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="a1348-962">August 11, 2017</span></span>

<span data-ttu-id="a1348-963">Версия 2.0.13</span><span class="sxs-lookup"><span data-stu-id="a1348-963">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="a1348-964">ACS</span><span class="sxs-lookup"><span data-stu-id="a1348-964">ACS</span></span>

* <span data-ttu-id="a1348-965">Добавлены дополнительные регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="a1348-965">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="a1348-966">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="a1348-966">Batch</span></span>

* <span data-ttu-id="a1348-967">Пакет SDK для пакетной службы обновлен до версии 3.1.0, а пакет SDK для управления пакетной службой — до версии 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="a1348-967">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="a1348-968">Добавлена новая команда для отображения количества задач в задании.</span><span class="sxs-lookup"><span data-stu-id="a1348-968">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="a1348-969">Исправлена ошибка при обработке URL-адреса SAS файла ресурсов.</span><span class="sxs-lookup"><span data-stu-id="a1348-969">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="a1348-970">Для конечной точки учетной записи пакетной службы теперь поддерживается дополнительный префикс https://.</span><span class="sxs-lookup"><span data-stu-id="a1348-970">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="a1348-971">Поддерживается добавление к заданию списков, содержащих более 100 задач.</span><span class="sxs-lookup"><span data-stu-id="a1348-971">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="a1348-972">Добавлено ведение журнала отладки при загрузке командного модуля расширений.</span><span class="sxs-lookup"><span data-stu-id="a1348-972">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="a1348-973">Компонент</span><span class="sxs-lookup"><span data-stu-id="a1348-973">Component</span></span>

* <span data-ttu-id="a1348-974">Добавлено предупреждение о прекращении поддержки в команды az component.</span><span class="sxs-lookup"><span data-stu-id="a1348-974">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="a1348-975">Контейнер</span><span class="sxs-lookup"><span data-stu-id="a1348-975">Container</span></span>

* <span data-ttu-id="a1348-976">`create`. Исправлена проблема, из-за которой запрещалось использовать знак равенства в переменной среды.</span><span class="sxs-lookup"><span data-stu-id="a1348-976">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="a1348-977">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a1348-977">Data Lake Store</span></span>

* <span data-ttu-id="a1348-978">Включен индикатор хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="a1348-978">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="a1348-979">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="a1348-979">Event Grid</span></span>

* <span data-ttu-id="a1348-980">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="a1348-980">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="a1348-981">Сеть</span><span class="sxs-lookup"><span data-stu-id="a1348-981">Network</span></span>

* <span data-ttu-id="a1348-982">`lb`. Исправлена проблема, из-за которой некоторые имена дочерних ресурсов не разрешались правильно, если не были указаны.</span><span class="sxs-lookup"><span data-stu-id="a1348-982">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="a1348-983">`application-gateway {subresource} delete`. Исправлена проблема, из-за которой не учитывался параметр `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="a1348-983">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="a1348-984">`application-gateway http-settings update`. Исправлена проблема, из-за которой не удавалось отключить параметр `--connection-draining-timeout`.</span><span class="sxs-lookup"><span data-stu-id="a1348-984">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="a1348-985">Исправлена проблема с непредвиденным аргументом ключевого слова `sa_data_size_kilobyes` при использовании с командой `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="a1348-985">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="a1348-986">Профиль</span><span class="sxs-lookup"><span data-stu-id="a1348-986">Profile</span></span>

* <span data-ttu-id="a1348-987">`account list`. Добавлен параметр `--refresh` для синхронизации последних подписок с сервером.</span><span class="sxs-lookup"><span data-stu-id="a1348-987">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="a1348-988">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="a1348-988">Storage</span></span>

* <span data-ttu-id="a1348-989">Включено обновление учетной записи хранения с помощью удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="a1348-989">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="a1348-990">ВМ</span><span class="sxs-lookup"><span data-stu-id="a1348-990">VM</span></span>

* <span data-ttu-id="a1348-991">`availability-set`. Предоставлено число доменов сбоя при преобразовании.</span><span class="sxs-lookup"><span data-stu-id="a1348-991">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="a1348-992">Предоставлена команда `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="a1348-992">Exposed `list-skus` command</span></span>
* <span data-ttu-id="a1348-993">Поддерживается назначение удостоверений без создания назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="a1348-993">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="a1348-994">При подключении дисков данных применяется номер SKU хранилища.</span><span class="sxs-lookup"><span data-stu-id="a1348-994">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="a1348-995">Удалено используемое по умолчанию имя диска ОС и номер SKU хранилища при использовании управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="a1348-995">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="a1348-996">28 июля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="a1348-996">July 28, 2017</span></span>

<span data-ttu-id="a1348-997">Версия 2.0.12</span><span class="sxs-lookup"><span data-stu-id="a1348-997">Version 2.0.12</span></span>

* <span data-ttu-id="a1348-998">Добавлены команды для контейнеров.</span><span class="sxs-lookup"><span data-stu-id="a1348-998">Added container commands</span></span>
* <span data-ttu-id="a1348-999">Добавлены модули выставления счетов и потребления ресурсов.</span><span class="sxs-lookup"><span data-stu-id="a1348-999">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="a1348-1000">Core</span><span class="sxs-lookup"><span data-stu-id="a1348-1000">Core</span></span>

* <span data-ttu-id="a1348-1001">Вывод сведений о пакетах SDK для проверки подлинности субъектов-служб с помощью сертификатов.</span><span class="sxs-lookup"><span data-stu-id="a1348-1001">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="a1348-1002">Исправлены исключения в ходе выполнения развертывания.</span><span class="sxs-lookup"><span data-stu-id="a1348-1002">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="a1348-1003">Для создания клиента подписки используется конечная точка ARM текущего облака.</span><span class="sxs-lookup"><span data-stu-id="a1348-1003">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="a1348-1004">Улучшена параллельная обработка файла clouds.config (3636).</span><span class="sxs-lookup"><span data-stu-id="a1348-1004">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="a1348-1005">Обновление идентификатора клиентского запроса при каждом выполнении команды.</span><span class="sxs-lookup"><span data-stu-id="a1348-1005">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="a1348-1006">Создание клиентов подписки с правильным профилем SDK (3635).</span><span class="sxs-lookup"><span data-stu-id="a1348-1006">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="a1348-1007">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="a1348-1007">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="a1348-1008">Добавлена поддержка выбора полей вывода в таблице с помощью запроса jmespath (3581).</span><span class="sxs-lookup"><span data-stu-id="a1348-1008">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="a1348-1009">Улучшено отключение аргументов анализа и добавлено ведение журналов с помощью жестов (3434).</span><span class="sxs-lookup"><span data-stu-id="a1348-1009">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="a1348-1010">Создание клиентов подписки с правильным профилем SDK.</span><span class="sxs-lookup"><span data-stu-id="a1348-1010">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="a1348-1011">Перемещение всех существующих файлов записи в последнюю папку.</span><span class="sxs-lookup"><span data-stu-id="a1348-1011">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="a1348-1012">Исправлена идемпотентность при создании виртуальной машины или масштабируемого набора виртуальных машин (3586).</span><span class="sxs-lookup"><span data-stu-id="a1348-1012">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="a1348-1013">В путях команд больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="a1348-1013">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="a1348-1014">В определенных параметрах логического типа больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="a1348-1014">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="a1348-1015">Поддержка входа на локальный сервер AD FS, например Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="a1348-1015">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="a1348-1016">Исправлена параллельная запись в файл clouds.config (3255).</span><span class="sxs-lookup"><span data-stu-id="a1348-1016">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="a1348-1017">ACR</span><span class="sxs-lookup"><span data-stu-id="a1348-1017">ACR</span></span>

* <span data-ttu-id="a1348-1018">Добавлена команда `show-usage` для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="a1348-1018">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="a1348-1019">Поддержка обновления номера SKU для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="a1348-1019">Support SKU update for managed registries</span></span>
* <span data-ttu-id="a1348-1020">Добавлены управляемые реестры с управляемыми номерами SKU.</span><span class="sxs-lookup"><span data-stu-id="a1348-1020">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="a1348-1021">Добавлены веб-перехватчики для управляемых реестров с использованием модуля для команды acr webhook.</span><span class="sxs-lookup"><span data-stu-id="a1348-1021">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="a1348-1022">Добавлена проверка подлинности с помощью AAD с использованием команды acr login.</span><span class="sxs-lookup"><span data-stu-id="a1348-1022">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="a1348-1023">Добавлена команда delete для репозиториев, манифестов и тегов Docker.</span><span class="sxs-lookup"><span data-stu-id="a1348-1023">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="a1348-1024">ACS</span><span class="sxs-lookup"><span data-stu-id="a1348-1024">ACS</span></span>

* <span data-ttu-id="a1348-1025">Поддержка API версии 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="a1348-1025">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="a1348-1026">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a1348-1026">Appservice</span></span>

* <span data-ttu-id="a1348-1027">Исправлена ошибка, из-за которой команда вывода списка в веб-приложениях Linux не возвращала данные.</span><span class="sxs-lookup"><span data-stu-id="a1348-1027">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="a1348-1028">Поддержка извлечения учетных данных из ACR.</span><span class="sxs-lookup"><span data-stu-id="a1348-1028">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="a1348-1029">Удаление всех команд группы `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1029">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="a1348-1030">Создание масок паролей для реестров Docker из выходных данных команды (3656).</span><span class="sxs-lookup"><span data-stu-id="a1348-1030">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="a1348-1031">Обеспечено использование браузера по умолчанию в macOS без ошибок (3623).</span><span class="sxs-lookup"><span data-stu-id="a1348-1031">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="a1348-1032">Улучшена справка по командам `webapp log tail` и `webapp log download` (3624).</span><span class="sxs-lookup"><span data-stu-id="a1348-1032">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="a1348-1033">Предоставлена команда `traffic-routing` для настройки статической маршрутизации (3566).</span><span class="sxs-lookup"><span data-stu-id="a1348-1033">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="a1348-1034">Добавлены исправления, связанные с надежностью, при настройке системы управления версиями (3245).</span><span class="sxs-lookup"><span data-stu-id="a1348-1034">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="a1348-1035">Удален неподдерживаемый аргумент `--node-version` из функции `webapp config update` для веб-приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="a1348-1035">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="a1348-1036">Вместо него используется `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1036">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="a1348-1037">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="a1348-1037">Batch</span></span>

* <span data-ttu-id="a1348-1038">Пакеты SDK для пакетной службы обновлены до версии 3.0.0 с поддержкой низкоприоритетных виртуальных машин в пулах.</span><span class="sxs-lookup"><span data-stu-id="a1348-1038">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="a1348-1039">Параметр команды `pool create` переименован с `--target-dedicated` в `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1039">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="a1348-1040">Для команды `pool create` добавлены параметры `--target-low-priority-nodes` и `--application-licenses`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1040">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="a1348-1041">CDN</span><span class="sxs-lookup"><span data-stu-id="a1348-1041">CDN</span></span>

* <span data-ttu-id="a1348-1042">Предоставлено улучшенное сообщение об ошибке для команды `cdn endpoint list`, которое отображается, если заданный параметром `--profile-name` профиль не существует.</span><span class="sxs-lookup"><span data-stu-id="a1348-1042">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="a1348-1043">Облако</span><span class="sxs-lookup"><span data-stu-id="a1348-1043">Cloud</span></span>

* <span data-ttu-id="a1348-1044">Формат версии API конечной точки метаданных облака изменен на следующий: ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="a1348-1044">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="a1348-1045">Конечная точка коллекции не является обязательной.</span><span class="sxs-lookup"><span data-stu-id="a1348-1045">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="a1348-1046">Поддерживается регистрация облака только с конечной точкой диспетчера ARM.</span><span class="sxs-lookup"><span data-stu-id="a1348-1046">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="a1348-1047">Предоставлен параметр в команде `cloud set` для выбора профиля при выборе текущего облака.</span><span class="sxs-lookup"><span data-stu-id="a1348-1047">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="a1348-1048">Предоставлен параметр `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1048">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a1348-1049">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="a1348-1049">CosmosDB</span></span>

* <span data-ttu-id="a1348-1050">Внесены исправления, которые позволяют создавать коллекцию с пользовательским ключом секции.</span><span class="sxs-lookup"><span data-stu-id="a1348-1050">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="a1348-1051">Добавлена поддержка срока жизни по умолчанию для коллекции.</span><span class="sxs-lookup"><span data-stu-id="a1348-1051">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="a1348-1052">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="a1348-1052">Data Lake Analytics</span></span>

* <span data-ttu-id="a1348-1053">Добавлены команды для управления политикой вычислений в разделе `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1053">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="a1348-1054">Добавлена команда `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1054">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="a1348-1055">Добавлена команда `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1055">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="a1348-1056">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a1348-1056">Data Lake Store</span></span>

* <span data-ttu-id="a1348-1057">Добавлена поддержка смены ключей пользовательского хранилища ключей в `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1057">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="a1348-1058">Обновлена версия пакета SDK для базовой файловой системы Data Lake Store из-за проблем с производительностью.</span><span class="sxs-lookup"><span data-stu-id="a1348-1058">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="a1348-1059">Добавлена команда `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1059">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="a1348-1060">Эта команда пытается активировать пользовательское хранилище ключей, предназначенное для шифрования данных в учетной записи Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="a1348-1060">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="a1348-1061">Интерактивный режим</span><span class="sxs-lookup"><span data-stu-id="a1348-1061">Interactive</span></span>

* <span data-ttu-id="a1348-1062">Улучшено время запуска с помощью кэшированных команд.</span><span class="sxs-lookup"><span data-stu-id="a1348-1062">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="a1348-1063">Увеличено тестовое покрытие.</span><span class="sxs-lookup"><span data-stu-id="a1348-1063">Increased test coverage</span></span>
* <span data-ttu-id="a1348-1064">Расширены возможности жеста "?", которые позволяют также вставить его в следующую команду.</span><span class="sxs-lookup"><span data-stu-id="a1348-1064">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="a1348-1065">Исправлены ошибки с интерактивными функциями в предварительной версии профиля 2017-03-09 (3587).</span><span class="sxs-lookup"><span data-stu-id="a1348-1065">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="a1348-1066">Разрешено использовать `--version` в качестве параметра в интерактивном режиме (3645).</span><span class="sxs-lookup"><span data-stu-id="a1348-1066">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="a1348-1067">В интерактивном режиме больше не возникают ошибки при выполнении проверки (3570).</span><span class="sxs-lookup"><span data-stu-id="a1348-1067">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="a1348-1068">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="a1348-1068">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="a1348-1069">Добавлен флаг `--progress`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1069">Added `--progress` flag</span></span>
* <span data-ttu-id="a1348-1070">Из вариантов завершения удалены `--debug` и `--verbose`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1070">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="a1348-1071">Из вариантов завершения удален `interactive` (3324).</span><span class="sxs-lookup"><span data-stu-id="a1348-1071">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="a1348-1072">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="a1348-1072">IoT</span></span>

* <span data-ttu-id="a1348-1073">Исправлено. При создании политики больше не удаляются существующие политики</span><span class="sxs-lookup"><span data-stu-id="a1348-1073">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="a1348-1074">(3934).</span><span class="sxs-lookup"><span data-stu-id="a1348-1074">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="a1348-1075">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="a1348-1075">Key vault</span></span>

* <span data-ttu-id="a1348-1076">Добавлены команды для функций восстановления хранилища ключей:</span><span class="sxs-lookup"><span data-stu-id="a1348-1076">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="a1348-1077">`keyvault`, подкоманды `purge`, `recover` и `keyvault list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1077">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="a1348-1078">`keyvault secret`, подкоманды `backup`, `restore`, `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="a1348-1078">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="a1348-1079">`keyvault certificate`, подкоманды `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="a1348-1079">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="a1348-1080">`keyvault key`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1080">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="a1348-1081">Добавлена интеграция хранилища ключей с субъектом-службой (3133).</span><span class="sxs-lookup"><span data-stu-id="a1348-1081">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="a1348-1082">Обновлена плоскость данных хранилища ключей до версии 0.3.2</span><span class="sxs-lookup"><span data-stu-id="a1348-1082">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="a1348-1083">(3307).</span><span class="sxs-lookup"><span data-stu-id="a1348-1083">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="a1348-1084">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="a1348-1084">Lab</span></span>

* <span data-ttu-id="a1348-1085">Добавлена поддержка запросов ко всем виртуальным машинам в лаборатории с помощью `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1085">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="a1348-1086">Добавлен модуль форматирования табличных выходных данных команд `az lab vm list` и `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1086">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="a1348-1087">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="a1348-1087">Monitor</span></span>

* <span data-ttu-id="a1348-1088">Исправлены ошибки с файлом шаблона с помощью команды `monitor autoscale-settings get-parameters-template` (3349).</span><span class="sxs-lookup"><span data-stu-id="a1348-1088">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="a1348-1089">Команда `monitor alert-rule-incidents list` переименована в `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1089">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="a1348-1090">Команда `monitor alert-rule-incidents show` переименована в `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1090">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="a1348-1091">Команда `monitor metric-defintions list` переименована в `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1091">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="a1348-1092">Команда `monitor alert-rules` переименована в `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1092">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="a1348-1093">В команду `monitor alert create` внесены следующие изменения:</span><span class="sxs-lookup"><span data-stu-id="a1348-1093">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="a1348-1094">подкоманды `condition` и `action` больше не принимают данные JSON;</span><span class="sxs-lookup"><span data-stu-id="a1348-1094">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="a1348-1095">добавлены различные параметры, которые упрощают процесс создания правила;</span><span class="sxs-lookup"><span data-stu-id="a1348-1095">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="a1348-1096">параметр `location` больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="a1348-1096">`location` no longer required</span></span>
  * <span data-ttu-id="a1348-1097">добавлена поддержка имени и идентификатора для целевого объекта;</span><span class="sxs-lookup"><span data-stu-id="a1348-1097">Add name and ID support for target</span></span>
  * <span data-ttu-id="a1348-1098">удален параметр `--alert-rule-resource-name`;</span><span class="sxs-lookup"><span data-stu-id="a1348-1098">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="a1348-1099">параметр `is-enabled` переименован в `enabled`, он больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="a1348-1099">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="a1348-1100">значения по умолчанию для `description` теперь основаны на указанном условии;</span><span class="sxs-lookup"><span data-stu-id="a1348-1100">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="a1348-1101">добавлены примеры, в которых подробно представлен новый формат.</span><span class="sxs-lookup"><span data-stu-id="a1348-1101">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="a1348-1102">Поддержка имен или идентификаторов для команд `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1102">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="a1348-1103">Добавлены вспомогательные аргументы и примеры использования команды `monitor alert rule update`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1103">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="a1348-1104">Сеть</span><span class="sxs-lookup"><span data-stu-id="a1348-1104">Network</span></span>

* <span data-ttu-id="a1348-1105">Добавлена команда `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1105">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="a1348-1106">Добавлен аргумент `--private-access-services` в команды `vnet subnet create` и `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1106">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="a1348-1107">Исправлена проблема, из-за которой команда `application-gateway redirect-config create` завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="a1348-1107">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="a1348-1108">Исправлена проблема, из-за которой команда `application-gateway redirect-config update` не работала с параметром `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1108">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="a1348-1109">Исправлена ошибка при использовании аргумента `--servers` с командами `application-gateway address-pool create` и `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1109">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="a1348-1110">Добавлены команды `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1110">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="a1348-1111">В команду `application-gateway ssl-policy` добавлены подкоманды `list-options`, `predefined list` и `predefined show`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1111">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="a1348-1112">В команду `application-gateway ssl-policy set` добавлены аргументы `--name`, `--cipher-suites` и `--min-protocol-version`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1112">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="a1348-1113">В команды `application-gateway http-settings create` и `application-gateway http-settings update` добавлены аргументы `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe` и `--path`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1113">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="a1348-1114">В команды `application-gateway url-path-map create` и `application-gateway url-path-map update` добавлены аргументы `--default-redirect-config` и `--redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1114">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="a1348-1115">Добавлен аргумент `--redirect-config` в команду `application-gateway url-path-map rule create`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1115">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="a1348-1116">Добавлена поддержка параметра `--no-wait` в команде `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1116">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="a1348-1117">В команды `application-gateway probe create` и `application-gateway probe update` добавлены аргументы `--host-name-from-http-settings`, `--min-servers`, `--match-body` и `--match-status-codes`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1117">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="a1348-1118">Добавлен аргумент `--redirect-config` в команды `application-gateway rule create` и `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1118">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="a1348-1119">Добавлена поддержка аргумента `--accelerated-networking` в командах `nic create` и `nic update`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1119">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="a1348-1120">Удален аргумент `--internal-dns-name-suffix` из команды `nic create`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1120">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="a1348-1121">Добавлена поддержка параметра `--dns-servers` в командах `nic update` и `nic create`. Добавлена поддержка параметра --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="a1348-1121">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="a1348-1122">Исправлена ошибка, из-за которой команда `local-gateway create` игнорировала параметр `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1122">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="a1348-1123">Добавлена поддержка параметра `--dns-servers` в команде `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1123">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="a1348-1124">Исправлена ошибка при создании пиринга без фильтрации маршрутов с помощью команды `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1124">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="a1348-1125">Исправлена ошибка, из-за которой аргументы `--provider` и `--bandwidth` не работали с командой `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1125">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="a1348-1126">Исправлена ошибка с логикой установки значений по умолчанию в команде `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1126">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="a1348-1127">Улучшено форматирование выходных данных команды `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1127">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="a1348-1128">В команде `application-gateway http-listener create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="a1348-1128">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="a1348-1129">В команде `application-gateway rule create` используются пул адресов, параметры HTTP и прослушиватель HTTP по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="a1348-1129">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="a1348-1130">В команде `lb rule create` используются интерфейсный IP-адрес и серверный пул по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="a1348-1130">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="a1348-1131">В команде `lb inbound-nat-rule create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="a1348-1131">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="a1348-1132">Профиль</span><span class="sxs-lookup"><span data-stu-id="a1348-1132">Profile</span></span>

* <span data-ttu-id="a1348-1133">Поддержка входа на виртуальную машину с использованием управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="a1348-1133">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="a1348-1134">Поддержка вывода данных команды `account show` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="a1348-1134">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="a1348-1135">При использовании параметра --expanded-view отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="a1348-1135">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="a1348-1136">Добавлена команда `get-access-token` для предоставления необработанного токена AAD.</span><span class="sxs-lookup"><span data-stu-id="a1348-1136">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="a1348-1137">Поддержка входа с учетной записью пользователя без связанных подписок.</span><span class="sxs-lookup"><span data-stu-id="a1348-1137">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="a1348-1138">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="a1348-1138">RDBMS</span></span>

* <span data-ttu-id="a1348-1139">Поддержка вывода списка серверов в подписке (3417).</span><span class="sxs-lookup"><span data-stu-id="a1348-1139">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="a1348-1140">Исправлена проблема, когда объект `%s` не обрабатывался из-за отсутствия `% server_type` (3393).</span><span class="sxs-lookup"><span data-stu-id="a1348-1140">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="a1348-1141">Исправлено сопоставление источника документа и добавлена задача непрерывной интеграции для проверки (3361).</span><span class="sxs-lookup"><span data-stu-id="a1348-1141">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="a1348-1142">Исправлена справка по MySQL и PostgreSQL (3369).</span><span class="sxs-lookup"><span data-stu-id="a1348-1142">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="a1348-1143">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a1348-1143">Resource</span></span>

* <span data-ttu-id="a1348-1144">Улучшены запросы на ввод отсутствующих параметров для команды `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1144">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="a1348-1145">Улучшен анализ синтаксиса `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1145">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="a1348-1146">Исправлены проблемы, из-за которых файлы параметров `group deployment create` не распознавались с использованием синтаксиса `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1146">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="a1348-1147">Поддержка аргумента `--ids` в командах `resource` и `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1147">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="a1348-1148">Исправлены некоторые сообщения об ошибках и анализе (3584).</span><span class="sxs-lookup"><span data-stu-id="a1348-1148">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="a1348-1149">Исправлены ошибки анализа параметра `--resource-type` в команде `lock`. Теперь принимаются `<resource-namespace>` и `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1149">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="a1348-1150">Добавлена проверка параметров для шаблонов для ссылок на шаблоны (3629).</span><span class="sxs-lookup"><span data-stu-id="a1348-1150">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="a1348-1151">Добавлена поддержка указания параметров развертывания с использованием синтаксиса `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1151">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="a1348-1152">Роль</span><span class="sxs-lookup"><span data-stu-id="a1348-1152">Role</span></span>

* <span data-ttu-id="a1348-1153">Поддержка вывода данных команды `create-for-rbac` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="a1348-1153">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="a1348-1154">Добавлена очистка назначений ролей и связанного приложения AAD при удалении субъекта-службы (3610).</span><span class="sxs-lookup"><span data-stu-id="a1348-1154">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="a1348-1155">В описания аргументов `--start-date` и `--end-date` команды `app create` добавлен формат времени.</span><span class="sxs-lookup"><span data-stu-id="a1348-1155">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="a1348-1156">При использовании параметра `--expanded-view` отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="a1348-1156">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="a1348-1157">Добавлена интеграция хранилища ключей для команд `create-for-rbac` и `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1157">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="a1348-1158">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="a1348-1158">Service Fabric</span></span>
* <span data-ttu-id="a1348-1159">Исправлена ошибка, из-за которой большие файлы в приложениях усекались при отправке (3666).</span><span class="sxs-lookup"><span data-stu-id="a1348-1159">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="a1348-1160">Добавлены тесты для команд Service Fabric (3424).</span><span class="sxs-lookup"><span data-stu-id="a1348-1160">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="a1348-1161">Исправлены многие команды Service Fabric (3234).</span><span class="sxs-lookup"><span data-stu-id="a1348-1161">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="a1348-1162">SQL</span><span class="sxs-lookup"><span data-stu-id="a1348-1162">SQL</span></span>

* <span data-ttu-id="a1348-1163">Удален недействительный параметр `--identity` команды `sql server create`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1163">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="a1348-1164">Удалены значения паролей из выходных данных команд `sql server create` и `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1164">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="a1348-1165">Добавлены команды `sql db list-editions` и `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1165">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="a1348-1166">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="a1348-1166">Storage</span></span>

* <span data-ttu-id="a1348-1167">Удален параметр `--marker` из команд `storage blob list`, `storage container list` и `storage share list` (3745).</span><span class="sxs-lookup"><span data-stu-id="a1348-1167">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="a1348-1168">Включено создание учетных записей хранения с поддержкой только HTTPS.</span><span class="sxs-lookup"><span data-stu-id="a1348-1168">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="a1348-1169">Обновлены метрики хранилища, команды входа и CORS (3495).</span><span class="sxs-lookup"><span data-stu-id="a1348-1169">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="a1348-1170">Перефразировано сообщение об исключении, которое выводит команда добавления CORS (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="a1348-1170">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="a1348-1171">Генератор преобразован в список в режиме пробного выполнения команды пакетной загрузки (3592).</span><span class="sxs-lookup"><span data-stu-id="a1348-1171">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="a1348-1172">Исправлена проблема при пробном выполнении команды пакетной загрузки больших двоичных объектов (3640) (3592).</span><span class="sxs-lookup"><span data-stu-id="a1348-1172">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="a1348-1173">ВМ</span><span class="sxs-lookup"><span data-stu-id="a1348-1173">VM</span></span>

* <span data-ttu-id="a1348-1174">Поддержка настройки NSG.</span><span class="sxs-lookup"><span data-stu-id="a1348-1174">Support configuring nsg</span></span>
* <span data-ttu-id="a1348-1175">Исправлена ошибка, из-за которой не удавалось правильно настроить DNS-сервер.</span><span class="sxs-lookup"><span data-stu-id="a1348-1175">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="a1348-1176">Поддержка удостоверений управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="a1348-1176">Support managed service identities</span></span>
* <span data-ttu-id="a1348-1177">Исправлена проблема, из-за которой для команды `cmss create` с существующей подсистемой балансировки нагрузки требовался параметр `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1177">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="a1348-1178">Теперь нумерация LUN дисков данных, создаваемых с помощью команды `vm image create`, начинается с 0.</span><span class="sxs-lookup"><span data-stu-id="a1348-1178">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="a1348-1179">10 мая 2017 г.</span><span class="sxs-lookup"><span data-stu-id="a1348-1179">May 10, 2017</span></span>

<span data-ttu-id="a1348-1180">Версия 2.0.6</span><span class="sxs-lookup"><span data-stu-id="a1348-1180">Version 2.0.6</span></span>

* <span data-ttu-id="a1348-1181">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="a1348-1181">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="a1348-1182">Добавлена реляционная СУБД (MySQL, Postgres).</span><span class="sxs-lookup"><span data-stu-id="a1348-1182">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="a1348-1183">Добавлены модули Data Lake Store и Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="a1348-1183">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="a1348-1184">Добавлен модуль Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="a1348-1184">Include Cognitive Services module</span></span>
* <span data-ttu-id="a1348-1185">Добавлен модуль Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="a1348-1185">Include Service Fabric module</span></span>
* <span data-ttu-id="a1348-1186">Добавлен модуль Interactive (az-shell переименован).</span><span class="sxs-lookup"><span data-stu-id="a1348-1186">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="a1348-1187">Добавлена поддержка команд CDN.</span><span class="sxs-lookup"><span data-stu-id="a1348-1187">Add support for CDN commands</span></span>
* <span data-ttu-id="a1348-1188">Удален модуль Container.</span><span class="sxs-lookup"><span data-stu-id="a1348-1188">Remove Container module</span></span>
* <span data-ttu-id="a1348-1189">Добавлена команда az -v для az --version ([№ 2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="a1348-1189">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="a1348-1190">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="a1348-1190">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="a1348-1191">Core</span><span class="sxs-lookup"><span data-stu-id="a1348-1191">Core</span></span>

* <span data-ttu-id="a1348-1192">Ядро: запись исключений, порожденных незарегистрированным поставщиком, и его автоматическая регистрация.</span><span class="sxs-lookup"><span data-stu-id="a1348-1192">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="a1348-1193">Производительность: сохранение кэша маркеров библиотеки ADAL в памяти до завершения работы процесса ([№ 2603](https://github.com/Azure/azure-cli/issues/2603)).</span><span class="sxs-lookup"><span data-stu-id="a1348-1193">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="a1348-1194">Исправление байтов, возвращаемых из шестнадцатеричных отпечатков -o tsv ([№ 3053](https://github.com/Azure/azure-cli/issues/3053)).</span><span class="sxs-lookup"><span data-stu-id="a1348-1194">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="a1348-1195">Улучшенное скачивание сертификатов Key Vault и интеграция субъектов-служб AAD ([№ 3003](https://github.com/Azure/azure-cli/issues/3003)).</span><span class="sxs-lookup"><span data-stu-id="a1348-1195">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="a1348-1196">Добавление расположения Python в az -version ([№ 2986](https://github.com/Azure/azure-cli/issues/2986)).</span><span class="sxs-lookup"><span data-stu-id="a1348-1196">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="a1348-1197">Вход: поддержка входа при отсутствии подписок ([№ 2929](https://github.com/Azure/azure-cli/issues/2929)).</span><span class="sxs-lookup"><span data-stu-id="a1348-1197">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="a1348-1198">Ядро: устранен сбой при двукратном входе с помощью субъекта-службы ([№ 2800](https://github.com/Azure/azure-cli/issues/2800)).</span><span class="sxs-lookup"><span data-stu-id="a1348-1198">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="a1348-1199">Ядро: возможность настроить путь к файлу accessTokens.json с помощью env var ([№ 2605](https://github.com/Azure/azure-cli/issues/2605)).</span><span class="sxs-lookup"><span data-stu-id="a1348-1199">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="a1348-1200">Ядро: возможность применять настроенные параметры по умолчанию к необязательным аргументам ([№ 2703](https://github.com/Azure/azure-cli/issues/2703)).</span><span class="sxs-lookup"><span data-stu-id="a1348-1200">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="a1348-1201">Ядро: повышение производительности.</span><span class="sxs-lookup"><span data-stu-id="a1348-1201">core: Improved performance</span></span>
* <span data-ttu-id="a1348-1202">Ядро: настаиваемые сертификаты ЦС — поддержка настройки переменной среды REQUESTS_CA_BUNDLE.</span><span class="sxs-lookup"><span data-stu-id="a1348-1202">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="a1348-1203">Ядро: облачная конфигурация — использование конечной точки Resource Manager, если не задана конечная точка управления.</span><span class="sxs-lookup"><span data-stu-id="a1348-1203">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="a1348-1204">ACS</span><span class="sxs-lookup"><span data-stu-id="a1348-1204">ACS</span></span>

* <span data-ttu-id="a1348-1205">Исправление: теперь значение счетчика баз данных master и агентов — целое число, а не строка.</span><span class="sxs-lookup"><span data-stu-id="a1348-1205">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="a1348-1206">Предоставлены команды az acs create --no-wait и az acs wait для асинхронного создания.</span><span class="sxs-lookup"><span data-stu-id="a1348-1206">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="a1348-1207">Предоставлена команда az acs create --validate для пробного создания.</span><span class="sxs-lookup"><span data-stu-id="a1348-1207">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="a1348-1208">Удален профиль Windows перед вызовом метода PUT для команды scale ([№ 2755](https://github.com/Azure/azure-cli/issues/2755)).</span><span class="sxs-lookup"><span data-stu-id="a1348-1208">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="a1348-1209">AppService</span><span class="sxs-lookup"><span data-stu-id="a1348-1209">AppService</span></span>

* <span data-ttu-id="a1348-1210">Приложение-функция: добавлена полная поддержка приложений-функций, включая создание, отображение, вывод списка, удаление, настройку имени узла, настройку протокола SSL и т. д.</span><span class="sxs-lookup"><span data-stu-id="a1348-1210">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="a1348-1211">Добавлены службы Team Services (VSTS) в качестве параметра непрерывной доставки в конфигурации веб-системы управления версиями службы приложений.</span><span class="sxs-lookup"><span data-stu-id="a1348-1211">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="a1348-1212">Создана команда az webapp, заменяющая команду az appservice web (для обеспечения обратной совместимости команда az appservice web будет оставлена еще в двух выпусках).</span><span class="sxs-lookup"><span data-stu-id="a1348-1212">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="a1348-1213">Предоставлены аргументы для настройки развертывания и стеков времени выполнения при создании веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="a1348-1213">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="a1348-1214">Предоставлена команда webapp list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="a1348-1214">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="a1348-1215">Поддержка настройки строк подключения ([№ 2647](https://github.com/Azure/azure-cli/issues/2647)).</span><span class="sxs-lookup"><span data-stu-id="a1348-1215">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="a1348-1216">Поддержка переключения слотов с предварительным просмотром.</span><span class="sxs-lookup"><span data-stu-id="a1348-1216">support slot swap with preview</span></span>
* <span data-ttu-id="a1348-1217">Устранены ошибки из команд службы приложений ([№ 2948](https://github.com/Azure/azure-cli/issues/2948)).</span><span class="sxs-lookup"><span data-stu-id="a1348-1217">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="a1348-1218">Использование группы ресурсов в плане служб приложений для операций с сертификатами ([№ 2750](https://github.com/Azure/azure-cli/issues/2750)).</span><span class="sxs-lookup"><span data-stu-id="a1348-1218">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a1348-1219">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="a1348-1219">CosmosDB</span></span>

* <span data-ttu-id="a1348-1220">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="a1348-1220">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="a1348-1221">Добавлена поддержка интерфейсов API уровня данных DocumentDB: управление базами данных и коллекциями.</span><span class="sxs-lookup"><span data-stu-id="a1348-1221">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="a1348-1222">Добавлена поддержка включения автоматической отработки отказа для учетных записей базы данных.</span><span class="sxs-lookup"><span data-stu-id="a1348-1222">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="a1348-1223">Добавлена поддержка нового параметра ConsistentPrefix политики согласованности.</span><span class="sxs-lookup"><span data-stu-id="a1348-1223">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="a1348-1224">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="a1348-1224">Data Lake Analytics</span></span>

* <span data-ttu-id="a1348-1225">Исправлена ошибка, из-за которой фильтрация списков заданий по результату и состоянию вызывала сбой.</span><span class="sxs-lookup"><span data-stu-id="a1348-1225">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="a1348-1226">Добавлена поддержка нового типа элемента каталога — пакета.</span><span class="sxs-lookup"><span data-stu-id="a1348-1226">Add support for new catalog item type: package.</span></span> <span data-ttu-id="a1348-1227">Для доступа к нему используется `az dla catalog package`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1227">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="a1348-1228">Появилась возможность вывести список следующих элементов каталога из базы данных (указание схемы не требуется):</span><span class="sxs-lookup"><span data-stu-id="a1348-1228">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="a1348-1229">Таблица</span><span class="sxs-lookup"><span data-stu-id="a1348-1229">Table</span></span>
  * <span data-ttu-id="a1348-1230">функция с табличным значением;</span><span class="sxs-lookup"><span data-stu-id="a1348-1230">Table valued function</span></span>
  * <span data-ttu-id="a1348-1231">Просмотр</span><span class="sxs-lookup"><span data-stu-id="a1348-1231">View</span></span>
  * <span data-ttu-id="a1348-1232">статистика таблицы.</span><span class="sxs-lookup"><span data-stu-id="a1348-1232">Table Statistics.</span></span> <span data-ttu-id="a1348-1233">Их можно также вывести с помощью схемы, но без указания имени таблицы.</span><span class="sxs-lookup"><span data-stu-id="a1348-1233">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="a1348-1234">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a1348-1234">Data Lake Store</span></span>

* <span data-ttu-id="a1348-1235">Обновлена версия пакета SDK базовой файловой системы, что обеспечивает лучшую поддержку сценариев регулирования на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="a1348-1235">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="a1348-1236">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="a1348-1236">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="a1348-1237">Отсутствовала справка для команды access show.</span><span class="sxs-lookup"><span data-stu-id="a1348-1237">missed help for access show.</span></span> <span data-ttu-id="a1348-1238">Теперь она добавлена.</span><span class="sxs-lookup"><span data-stu-id="a1348-1238">adding it.</span></span> <span data-ttu-id="a1348-1239">([№ 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="a1348-1239">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="a1348-1240">Поиск</span><span class="sxs-lookup"><span data-stu-id="a1348-1240">Find</span></span>

* <span data-ttu-id="a1348-1241">Улучшены результаты поиска и разрешено управление версиями индекса поиска.</span><span class="sxs-lookup"><span data-stu-id="a1348-1241">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="a1348-1242">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="a1348-1242">KeyVault</span></span>

* <span data-ttu-id="a1348-1243">BC: в команде `az keyvault certificate download` параметр -e со строкового или двоичного значения изменен на PEM или DER, чтобы лучше представить параметры.</span><span class="sxs-lookup"><span data-stu-id="a1348-1243">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="a1348-1244">BC: из команды `keyvault certificate create` удалены параметры --expires и --not-before, так как они не поддерживаются службой.</span><span class="sxs-lookup"><span data-stu-id="a1348-1244">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="a1348-1245">В команду `keyvault certificate create` добавлен параметр --validity для выборочного переопределения значение в параметре --policy.</span><span class="sxs-lookup"><span data-stu-id="a1348-1245">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="a1348-1246">Исправлена ошибка в команде `keyvault certificate get-default-policy`, в которой были доступны параметры expires и not_before, а параметр validity_in_months — нет.</span><span class="sxs-lookup"><span data-stu-id="a1348-1246">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="a1348-1247">Добавлено исправление для модуля keyvault для импорта PEM- и PFX-файлов ([№ 2754](https://github.com/Azure/azure-cli/issues/2754)).</span><span class="sxs-lookup"><span data-stu-id="a1348-1247">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="a1348-1248">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="a1348-1248">Lab</span></span>

* <span data-ttu-id="a1348-1249">Добавлены команды создания, отображения, удаления и вывода списка для среды в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="a1348-1249">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="a1348-1250">Добавлены команды отображения и вывода списка для просмотра шаблонов ARM в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="a1348-1250">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="a1348-1251">В команду `az lab vm list` добавлен флаг --environment для фильтрации виртуальных машин по среде в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="a1348-1251">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="a1348-1252">Добавлена вспомогательная команда `az lab formula export-artifacts` для экспорта шаблона артефакта в формуле лаборатории.</span><span class="sxs-lookup"><span data-stu-id="a1348-1252">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="a1348-1253">Добавлены команды для управления секретами в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="a1348-1253">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="a1348-1254">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="a1348-1254">Monitor</span></span>

* <span data-ttu-id="a1348-1255">Исправление ошибки: моделирование `--actions` в `az alert-rules create` для использования строки в формате JSON ([№ 3009](https://github.com/Azure/azure-cli/issues/3009)).</span><span class="sxs-lookup"><span data-stu-id="a1348-1255">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="a1348-1256">Исправление ошибки: при создании параметров диагностики не принимались журналы и метрики из команды show ([№ 2913](https://github.com/Azure/azure-cli/issues/2913)).</span><span class="sxs-lookup"><span data-stu-id="a1348-1256">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="a1348-1257">Сеть</span><span class="sxs-lookup"><span data-stu-id="a1348-1257">Network</span></span>

* <span data-ttu-id="a1348-1258">Добавлена команда `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1258">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="a1348-1259">Добавлена поддержка параметра `--filters` в команде `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1259">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="a1348-1260">Добавлена поддержка фильтрации подключений шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="a1348-1260">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="a1348-1261">Добавлена поддержка конфигурации набора правил WAF шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="a1348-1261">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="a1348-1262">Добавлена поддержка правил и фильтров маршрутов ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="a1348-1262">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="a1348-1263">Добавлена поддержка географической маршрутизации диспетчера трафика.</span><span class="sxs-lookup"><span data-stu-id="a1348-1263">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="a1348-1264">Добавлена поддержка селекторов трафика на основе политик для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="a1348-1264">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="a1348-1265">Добавлена поддержка политик IPSec для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="a1348-1265">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="a1348-1266">Исправлена ошибка `vpn-connection create`, возникавшая при использовании параметра `--no-wait` или `--validate`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1266">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="a1348-1267">Добавлена поддержка шлюзов виртуальной сети "активный-активный".</span><span class="sxs-lookup"><span data-stu-id="a1348-1267">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="a1348-1268">Удалены значения NULL из выходных данных команды `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1268">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="a1348-1269">BC: исправлена ошибка в выходных данных `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1269">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="a1348-1270">Исправлена ошибка, приводившая к неправильному анализу аргумента --key-length команды vpn-connection create.</span><span class="sxs-lookup"><span data-stu-id="a1348-1270">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="a1348-1271">Исправлена ошибка в `dns zone import`, из-за которой записи не импортировались правильно.</span><span class="sxs-lookup"><span data-stu-id="a1348-1271">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="a1348-1272">Исправлена ошибка, из-за которой команда `traffic-manager endpoint update` не работала.</span><span class="sxs-lookup"><span data-stu-id="a1348-1272">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="a1348-1273">Добавлены команды предварительного просмотра для Наблюдателя за сетями.</span><span class="sxs-lookup"><span data-stu-id="a1348-1273">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="a1348-1274">Профиль</span><span class="sxs-lookup"><span data-stu-id="a1348-1274">Profile</span></span>

* <span data-ttu-id="a1348-1275">Поддержка входа при отсутствии подписок ([№ 2560](https://github.com/Azure/azure-cli/issues/2560)).</span><span class="sxs-lookup"><span data-stu-id="a1348-1275">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="a1348-1276">Поддержка сокращенных имен параметров в команде az account set --subscription ([№ 2980](https://github.com/Azure/azure-cli/issues/2980)).</span><span class="sxs-lookup"><span data-stu-id="a1348-1276">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="a1348-1277">Redis</span><span class="sxs-lookup"><span data-stu-id="a1348-1277">Redis</span></span>

* <span data-ttu-id="a1348-1278">Добавлена команда update, которая также добавляет возможность масштабирования для кэша Redis.</span><span class="sxs-lookup"><span data-stu-id="a1348-1278">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="a1348-1279">Команда update-settings объявляется нерекомендуемой.</span><span class="sxs-lookup"><span data-stu-id="a1348-1279">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="a1348-1280">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a1348-1280">Resource</span></span>

* <span data-ttu-id="a1348-1281">Добавлены команды определения managedapp и managedapp ([№ 2985](https://github.com/Azure/azure-cli/issues/2985)).</span><span class="sxs-lookup"><span data-stu-id="a1348-1281">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="a1348-1282">Поддержка команд provider operation ([№ 2908](https://github.com/Azure/azure-cli/issues/2908)).</span><span class="sxs-lookup"><span data-stu-id="a1348-1282">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="a1348-1283">Поддержка создания универсального ресурса ([№ 2606](https://github.com/Azure/azure-cli/issues/2606)).</span><span class="sxs-lookup"><span data-stu-id="a1348-1283">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="a1348-1284">Исправлен анализ ресурсов и поиск версии API.</span><span class="sxs-lookup"><span data-stu-id="a1348-1284">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="a1348-1285">([№ 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="a1348-1285">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="a1348-1286">Добавлены документы для команды az lock update.</span><span class="sxs-lookup"><span data-stu-id="a1348-1286">Add docs for az lock update.</span></span> <span data-ttu-id="a1348-1287">([№ 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="a1348-1287">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="a1348-1288">Исправлена ошибка, возникавшая при попытке вывести список ресурсов группы, которая не существует.</span><span class="sxs-lookup"><span data-stu-id="a1348-1288">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="a1348-1289">([№ 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="a1348-1289">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="a1348-1290">[Вычисления.] Устранены проблемы с масштабируемым набором виртуальных машин и обновлением группы доступности виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="a1348-1290">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="a1348-1291">([№ 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="a1348-1291">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="a1348-1292">Исправлена блокировка создания и удаления, возникающая, если параметр parent-resource-path не указан ([№ 2742](https://github.com/Azure/azure-cli/issues/2742)).</span><span class="sxs-lookup"><span data-stu-id="a1348-1292">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="a1348-1293">Роль</span><span class="sxs-lookup"><span data-stu-id="a1348-1293">Role</span></span>

* <span data-ttu-id="a1348-1294">create-for-rbac: гарантируется, что дата завершения работы поставщика служб не может превышать срок действия сертификата ([№ 2989](https://github.com/Azure/azure-cli/issues/2989)).</span><span class="sxs-lookup"><span data-stu-id="a1348-1294">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="a1348-1295">RBAC: добавлена полная поддержка команды ad group ([№ 2016](https://github.com/Azure/azure-cli/issues/2016)).</span><span class="sxs-lookup"><span data-stu-id="a1348-1295">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="a1348-1296">Роль: устранены проблемы при обновлении определения роли ([№ 2745](https://github.com/Azure/azure-cli/issues/2745)).</span><span class="sxs-lookup"><span data-stu-id="a1348-1296">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="a1348-1297">create-for-rbac: обеспечен выбор введенного пользователем пароля.</span><span class="sxs-lookup"><span data-stu-id="a1348-1297">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="a1348-1298">SQL</span><span class="sxs-lookup"><span data-stu-id="a1348-1298">SQL</span></span>

* <span data-ttu-id="a1348-1299">Добавлены команды az sql server list-usages и az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="a1348-1299">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="a1348-1300">SQL: возможность прямого подключения к поставщику ресурса ([№ 2832](https://github.com/Azure/azure-cli/issues/2832)).</span><span class="sxs-lookup"><span data-stu-id="a1348-1300">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="a1348-1301">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="a1348-1301">Storage</span></span>

* <span data-ttu-id="a1348-1302">Добавлено расположение по умолчанию группы ресурсов для `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1302">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="a1348-1303">Добавлена поддержка добавочного копирования больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="a1348-1303">Add support for incremental blob copy</span></span>
* <span data-ttu-id="a1348-1304">Добавлена поддержка передачи больших блочных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="a1348-1304">Add support for large block blob upload</span></span>
* <span data-ttu-id="a1348-1305">Размер блока изменяется и составляет 100 МБ, если передается файл, чей размер превышает 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="a1348-1305">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="a1348-1306">ВМ</span><span class="sxs-lookup"><span data-stu-id="a1348-1306">VM</span></span>

* <span data-ttu-id="a1348-1307">avail-set: число доменов обновления и доменов сбоя сделано необязательным.</span><span class="sxs-lookup"><span data-stu-id="a1348-1307">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="a1348-1308">Примечание. Команды виртуальной машины в независимых облаках: избегайте использовать функции, связанные с Управляемыми дисками, включая следующие:</span><span class="sxs-lookup"><span data-stu-id="a1348-1308">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="a1348-1309">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="a1348-1309">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="a1348-1310">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="a1348-1310">az vm/vmss disk</span></span>
  3. <span data-ttu-id="a1348-1311">В команде az vm/vmss create используйте параметр --use-unmanaged-disk, чтобы избежать использования Управляемых дисков. Другие команды должны работать.</span><span class="sxs-lookup"><span data-stu-id="a1348-1311">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="a1348-1312">vm/vmss: улучшен текст предупреждения при создании пары ключей SSH.</span><span class="sxs-lookup"><span data-stu-id="a1348-1312">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="a1348-1313">vm/vmss: поддержка создания из образа Marketplace, для которого требуются сведения о плане ([№ 1209](https://github.com/Azure/azure-cli/issues/1209)).</span><span class="sxs-lookup"><span data-stu-id="a1348-1313">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="a1348-1314">3 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="a1348-1314">April 3, 2017</span></span>

<span data-ttu-id="a1348-1315">Версия 2.0.2</span><span class="sxs-lookup"><span data-stu-id="a1348-1315">Version 2.0.2</span></span>

<span data-ttu-id="a1348-1316">В этом выпуске мы добавили компоненты ACR, Batch, KeyVault и SQL.</span><span class="sxs-lookup"><span data-stu-id="a1348-1316">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="a1348-1317">Core</span><span class="sxs-lookup"><span data-stu-id="a1348-1317">Core</span></span>

* <span data-ttu-id="a1348-1318">Модули Acr, Lab, Monitor и Find добавлены в список по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a1348-1318">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="a1348-1319">Вход: пропуск неправильного клиента ([#2634](https://github.com/Azure/azure-cli/pull/2634)).</span><span class="sxs-lookup"><span data-stu-id="a1348-1319">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="a1348-1320">Вход: для подписки по умолчанию задано значение 1 с состоянием "Включено" ([#2575](https://github.com/Azure/azure-cli/pull/2575)).</span><span class="sxs-lookup"><span data-stu-id="a1348-1320">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="a1348-1321">Добавлена поддержка команд wait и --no-wait для дополнительных команд ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="a1348-1321">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="a1348-1322">Core: поддержка входа при помощи субъекта-службы с использованием сертификата ([#2457](https://github.com/Azure/azure-cli/pull/2457)).</span><span class="sxs-lookup"><span data-stu-id="a1348-1322">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="a1348-1323">Добавлен запрос для отсутствующих параметров шаблона</span><span class="sxs-lookup"><span data-stu-id="a1348-1323">Add prompting for missing template parameters.</span></span> <span data-ttu-id="a1348-1324">([#2364](https://github.com/Azure/azure-cli/pull/2364)).</span><span class="sxs-lookup"><span data-stu-id="a1348-1324">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="a1348-1325">Добавлена поддержка установки параметров по умолчанию для таких распространенных аргументов, как группа ресурсов по умолчанию, веб-страница по умолчанию, виртуальная машина по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a1348-1325">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="a1348-1326">Добавлена поддержка входа на конкретный клиент.</span><span class="sxs-lookup"><span data-stu-id="a1348-1326">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="a1348-1327">ACS</span><span class="sxs-lookup"><span data-stu-id="a1348-1327">ACS</span></span>

* <span data-ttu-id="a1348-1328">[ACS] Добавлена поддержка настройки кластера ACS по умолчанию ([#2554](https://github.com/Azure/azure-cli/pull/2554)).</span><span class="sxs-lookup"><span data-stu-id="a1348-1328">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="a1348-1329">Добавлена поддержка запроса пароля для ключа SSH</span><span class="sxs-lookup"><span data-stu-id="a1348-1329">Add support for ssh key password prompting.</span></span> <span data-ttu-id="a1348-1330">([#2044](https://github.com/Azure/azure-cli/pull/2044)).</span><span class="sxs-lookup"><span data-stu-id="a1348-1330">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="a1348-1331">Добавлена поддержка кластеров Windows</span><span class="sxs-lookup"><span data-stu-id="a1348-1331">Add support for windows clusters.</span></span> <span data-ttu-id="a1348-1332">([#2211](https://github.com/Azure/azure-cli/pull/2211)).</span><span class="sxs-lookup"><span data-stu-id="a1348-1332">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="a1348-1333">Добавлена возможность изменения роли "Владелец" на роль "Участник"</span><span class="sxs-lookup"><span data-stu-id="a1348-1333">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="a1348-1334">([#2321](https://github.com/Azure/azure-cli/pull/2321)).</span><span class="sxs-lookup"><span data-stu-id="a1348-1334">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="a1348-1335">AppService</span><span class="sxs-lookup"><span data-stu-id="a1348-1335">AppService</span></span>

* <span data-ttu-id="a1348-1336">AppService: добавлена поддержка получения внешнего IP-адреса, используемого для записей DNS типа A ([#2627](https://github.com/Azure/azure-cli/pull/2627)).</span><span class="sxs-lookup"><span data-stu-id="a1348-1336">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="a1348-1337">AppService: добавлена поддержка привязки групповых сертификатов ([#2625](https://github.com/Azure/azure-cli/pull/2625)).</span><span class="sxs-lookup"><span data-stu-id="a1348-1337">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="a1348-1338">AppService: добавлена поддержка профилей для публикации списком ([#2504](https://github.com/Azure/azure-cli/pull/2504)).</span><span class="sxs-lookup"><span data-stu-id="a1348-1338">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="a1348-1339">AppService: добавлен триггер синхронизации с системой управления версиями после настройки ([#2326](https://github.com/Azure/azure-cli/pull/2326)).</span><span class="sxs-lookup"><span data-stu-id="a1348-1339">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="a1348-1340">Data Lake</span><span class="sxs-lookup"><span data-stu-id="a1348-1340">DataLake</span></span>

* <span data-ttu-id="a1348-1341">Первый выпуск модуля Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="a1348-1341">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="a1348-1342">Первый выпуск модуля Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="a1348-1342">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="a1348-1343">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="a1348-1343">DocuemntDB</span></span>

* <span data-ttu-id="a1348-1344">DocumentDB: добавлена поддержка для получения списка строк подключения ([#2580](https://github.com/Azure/azure-cli/pull/2580)).</span><span class="sxs-lookup"><span data-stu-id="a1348-1344">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="a1348-1345">ВМ</span><span class="sxs-lookup"><span data-stu-id="a1348-1345">VM</span></span>

* <span data-ttu-id="a1348-1346">[Вычисления] Добавлена поддержка AppGateway для создания масштабируемого набора виртуальных машин ([#2570](https://github.com/Azure/azure-cli/pull/2570)).</span><span class="sxs-lookup"><span data-stu-id="a1348-1346">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="a1348-1347">[ВМ и VMSS] Улучшена поддержка кэширования диска ([#2522](https://github.com/Azure/azure-cli/pull/2522)).</span><span class="sxs-lookup"><span data-stu-id="a1348-1347">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="a1348-1348">ВМ и VMSS: внедрена логика проверки учетных данных, используемая на портале ([#2537](https://github.com/Azure/azure-cli/pull/2537)).</span><span class="sxs-lookup"><span data-stu-id="a1348-1348">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="a1348-1349">Добавлена поддержка команд wait и --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="a1348-1349">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="a1348-1350">Масштабируемый набор виртуальных машин: добавлена поддержка \* для представления экземпляров на виртуальных машинах в виде списка ([#2467](https://github.com/Azure/azure-cli/pull/2467)).</span><span class="sxs-lookup"><span data-stu-id="a1348-1350">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="a1348-1351">Добавлен параметр --secrets для виртуальной машины и масштабируемого набора виртуальных машин ([#2212}(https://github.com/Azure/azure-cli/pull/2212)).</span><span class="sxs-lookup"><span data-stu-id="a1348-1351">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="a1348-1352">Добавлено разрешение на создание виртуальных машин на основе специализированного образа VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256)).</span><span class="sxs-lookup"><span data-stu-id="a1348-1352">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="a1348-1353">27 февраля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="a1348-1353">February 27, 2017</span></span>

<span data-ttu-id="a1348-1354">Версия 2.0.0</span><span class="sxs-lookup"><span data-stu-id="a1348-1354">Version 2.0.0</span></span>

<span data-ttu-id="a1348-1355">Этот первый общедоступный выпуск Azure CLI 2.0. Общедоступными являются такие командные модули:</span><span class="sxs-lookup"><span data-stu-id="a1348-1355">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="a1348-1356">служба контейнеров (ACS);</span><span class="sxs-lookup"><span data-stu-id="a1348-1356">Container Service (acs)</span></span>
- <span data-ttu-id="a1348-1357">вычисления (в том числе Resource Manager, виртуальная машина, масштабируемые наборы виртуальных машин, управляемые диски);</span><span class="sxs-lookup"><span data-stu-id="a1348-1357">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="a1348-1358">Сеть</span><span class="sxs-lookup"><span data-stu-id="a1348-1358">Networking</span></span>
- <span data-ttu-id="a1348-1359">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="a1348-1359">Storage</span></span>

<span data-ttu-id="a1348-1360">Эти командные модули могут использоваться в рабочих средах. Они поддерживаются стандартными соглашениями Майкрософт об уровне обслуживания. Вы можете отправлять запросы непосредственно в службу технической поддержки Майкрософт или добавлять описание проблем в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/). Вы можете задавать вопросы на [сайте StackOverflow, используя тег azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), или обращаться к группе разработчиков по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Можно отправлять отзывы из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1360">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="a1348-1361">Команды в этих модулях стабильны, и предполагается, что в следующих выпусках этой версии Azure CLI их синтаксис не будет меняться.</span><span class="sxs-lookup"><span data-stu-id="a1348-1361">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="a1348-1362">Проверить версию CLI можно с помощью команды `az --version`. В выходных данных указана версия самого интерфейса командной строки (2.0.0 в этом выпуске), версии отдельных командных модулей и используемые вами версии Python и GCC.</span><span class="sxs-lookup"><span data-stu-id="a1348-1362">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="a1348-1363">Некоторые командные модули имеют постфикс b*n* или rc*n*. Эти командные модули все еще находятся на стадии предварительной версии и станут общедоступными в будущем.</span><span class="sxs-lookup"><span data-stu-id="a1348-1363">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="a1348-1364">У нас также есть предварительные ежедневные сборки CLI. Дополнительные сведения см. в инструкциях по [получению ежедневных сборок](https://github.com/Azure/azure-cli#nightly-builds), а также в инструкциях по [настройке среды разработки и участии в написании кода](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="a1348-1364">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="a1348-1365">О проблемах с предварительными ежедневными сборками можно сообщить несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="a1348-1365">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="a1348-1366">добавив информацию о проблемах в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/);</span><span class="sxs-lookup"><span data-stu-id="a1348-1366">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="a1348-1367">Свяжитесь с командой разработчиков ([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)),</span><span class="sxs-lookup"><span data-stu-id="a1348-1367">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="a1348-1368">отправив отзыв из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="a1348-1368">Provide feedback from the command line with the `az feedback` command</span></span>

