---
title: Заметки о выпуске Azure CLI 2.0
description: Узнайте о последних обновлениях в Azure CLI 2.0
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 04/10/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 254c7b306440d921cef6b611268839150fdf3196
ms.sourcegitcommit: 15d6dfaee2075d0abceb2aa2423f0b6ef7b2ac9b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2018
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="65a08-103">Заметки о выпуске Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="65a08-103">Azure CLI 2.0 release notes</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="65a08-104">7 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="65a08-104">May 7, 2018</span></span>

<span data-ttu-id="65a08-105">Версия 2.0.32</span><span class="sxs-lookup"><span data-stu-id="65a08-105">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="65a08-106">Core</span><span class="sxs-lookup"><span data-stu-id="65a08-106">Core</span></span>

* <span data-ttu-id="65a08-107">Исправлено необработанное исключение при получении секретов из основной учетной записи службы с сертификатом.</span><span class="sxs-lookup"><span data-stu-id="65a08-107">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="65a08-108">Добавлена ограниченная поддержка для позиционных аргументов.</span><span class="sxs-lookup"><span data-stu-id="65a08-108">Added limited support for positional arguments</span></span>
* <span data-ttu-id="65a08-109">Исправлена проблема, когда `--query` нельзя использовать с `--ids`.</span><span class="sxs-lookup"><span data-stu-id="65a08-109">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="65a08-110">#5591</span><span class="sxs-lookup"><span data-stu-id="65a08-110">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="65a08-111">Улучшены сценарии конвейерной передачи от команд при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="65a08-111">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="65a08-112">Добавлена поддержка `-o tsv` с указанием запроса или `-o json` без указания запроса.</span><span class="sxs-lookup"><span data-stu-id="65a08-112">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="65a08-113">Добавлена команда предложения в случае ошибки, если пользователи вводят команды с опечаткой.</span><span class="sxs-lookup"><span data-stu-id="65a08-113">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="65a08-114">Исправлена ошибка, когда пользователи вводят `az ''`.</span><span class="sxs-lookup"><span data-stu-id="65a08-114">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="65a08-115">Добавлена поддержка настраиваемого ресурса для командных модулей и расширений.</span><span class="sxs-lookup"><span data-stu-id="65a08-115">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="65a08-116">ACR</span><span class="sxs-lookup"><span data-stu-id="65a08-116">ACR</span></span>

* <span data-ttu-id="65a08-117">Добавлены команды сборки ACR.</span><span class="sxs-lookup"><span data-stu-id="65a08-117">Added ACR Build commands</span></span>
* <span data-ttu-id="65a08-118">Исправлена ошибка о не найденных сообщениях об ошибках.</span><span class="sxs-lookup"><span data-stu-id="65a08-118">Improved resource not found error messages</span></span>
* <span data-ttu-id="65a08-119">Оптимизированы производительность создания ресурсов и обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="65a08-119">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="65a08-120">Улучшены возможности входа ACR в нестандартные консоли и WSL.</span><span class="sxs-lookup"><span data-stu-id="65a08-120">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="65a08-121">Улучшены сообщения об ошибках команд репозитория.</span><span class="sxs-lookup"><span data-stu-id="65a08-121">Improved repository commands error messages</span></span>
* <span data-ttu-id="65a08-122">Обновлены столбцы таблиц и порядок их расположения.</span><span class="sxs-lookup"><span data-stu-id="65a08-122">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="65a08-123">ACS</span><span class="sxs-lookup"><span data-stu-id="65a08-123">ACS</span></span>

* <span data-ttu-id="65a08-124">Добавлено предупреждение о том, что `az aks` — это предварительная версия службы.</span><span class="sxs-lookup"><span data-stu-id="65a08-124">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="65a08-125">Исправлена проблема с разрешением в `aks install-connector`, когда `--aci-resource-group` не указывается.</span><span class="sxs-lookup"><span data-stu-id="65a08-125">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="65a08-126">AMS</span><span class="sxs-lookup"><span data-stu-id="65a08-126">AMS</span></span>

* <span data-ttu-id="65a08-127">Первоначальный выпуск. Управление ресурсами Служб мультимедиа Azure.</span><span class="sxs-lookup"><span data-stu-id="65a08-127">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="65a08-128">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="65a08-128">Appservice</span></span>

* <span data-ttu-id="65a08-129">Исправлена ошибка в `webapp delete`, когда `--slot` предоставляется.</span><span class="sxs-lookup"><span data-stu-id="65a08-129">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="65a08-130">Удалено `--runtime-version` из `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="65a08-130">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="65a08-131">Добавлена поддержка min\_tls\_version и https2.0.</span><span class="sxs-lookup"><span data-stu-id="65a08-131">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="65a08-132">Добавлена поддержка нескольких контейнеров.</span><span class="sxs-lookup"><span data-stu-id="65a08-132">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="65a08-133">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="65a08-133">Batch AI</span></span>

* <span data-ttu-id="65a08-134">Изменено `batchai create cluster` с учетом приоритета виртуальной машины при настройке в файле конфигурации кластера.</span><span class="sxs-lookup"><span data-stu-id="65a08-134">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="65a08-135">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="65a08-135">Cognitive Services</span></span>

* <span data-ttu-id="65a08-136">Исправлена опечатка в примере для `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603).</span><span class="sxs-lookup"><span data-stu-id="65a08-136">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="65a08-137">Потребление</span><span class="sxs-lookup"><span data-stu-id="65a08-137">Consumption</span></span>

* <span data-ttu-id="65a08-138">Добавлены новые команды в API для управления бюджетом.</span><span class="sxs-lookup"><span data-stu-id="65a08-138">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="65a08-139">Контейнер</span><span class="sxs-lookup"><span data-stu-id="65a08-139">Container</span></span>

* <span data-ttu-id="65a08-140">Удалено требование `--registry-server` для `container create`, когда сервер реестра включен в имя образа.</span><span class="sxs-lookup"><span data-stu-id="65a08-140">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="65a08-141">База данных Cosmos</span><span class="sxs-lookup"><span data-stu-id="65a08-141">Cosmos DB</span></span>

* <span data-ttu-id="65a08-142">Добавлена поддержка VNET для Azure CLI в Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="65a08-142">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="65a08-143">DMS</span><span class="sxs-lookup"><span data-stu-id="65a08-143">DMS</span></span>

* <span data-ttu-id="65a08-144">Исходный выпуск. Добавлена поддержка сценария миграции SQL — Azure SQL.</span><span class="sxs-lookup"><span data-stu-id="65a08-144">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="65a08-145">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="65a08-145">Extension</span></span>

* <span data-ttu-id="65a08-146">Исправлена ошибка, когда метаданные остановленного расширения отображались.</span><span class="sxs-lookup"><span data-stu-id="65a08-146">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="65a08-147">Interactive</span><span class="sxs-lookup"><span data-stu-id="65a08-147">Interactive</span></span>

* <span data-ttu-id="65a08-148">Разрешена работа интерактивных средств завершения с позиционными аргументами.</span><span class="sxs-lookup"><span data-stu-id="65a08-148">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="65a08-149">Добавлены более понятные выходные данные, когда пользователи вводят \'.</span><span class="sxs-lookup"><span data-stu-id="65a08-149">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="65a08-150">Исправлены завершения для параметров без справки.</span><span class="sxs-lookup"><span data-stu-id="65a08-150">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="65a08-151">Исправлены описания для групп команд.</span><span class="sxs-lookup"><span data-stu-id="65a08-151">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="65a08-152">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="65a08-152">Lab</span></span>

* <span data-ttu-id="65a08-153">Исправлены регрессии из преобразования Knack.</span><span class="sxs-lookup"><span data-stu-id="65a08-153">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="65a08-154">Сеть</span><span class="sxs-lookup"><span data-stu-id="65a08-154">Network</span></span>

* <span data-ttu-id="65a08-155">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕИЕ] Удален параметр `--ids` для:</span><span class="sxs-lookup"><span data-stu-id="65a08-155">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span> 
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="65a08-156">Профиль</span><span class="sxs-lookup"><span data-stu-id="65a08-156">Profile</span></span>

* <span data-ttu-id="65a08-157">Исправлено определение источника `disk create`.</span><span class="sxs-lookup"><span data-stu-id="65a08-157">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="65a08-158">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕИЕ] Удалено `--msi-port` и `--identity-port`, так как они больше не используются.</span><span class="sxs-lookup"><span data-stu-id="65a08-158">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="65a08-159">Исправлена опечатка в кратком описании `account get-access-token`.</span><span class="sxs-lookup"><span data-stu-id="65a08-159">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="65a08-160">Redis</span><span class="sxs-lookup"><span data-stu-id="65a08-160">Redis</span></span>

* <span data-ttu-id="65a08-161">Вместо `redis patch-schedule patch-schedule show` теперь используется `redis patch-schedule show`.</span><span class="sxs-lookup"><span data-stu-id="65a08-161">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="65a08-162">`redis list-all` теперь не используется.</span><span class="sxs-lookup"><span data-stu-id="65a08-162">Deprecated `redis list-all`.</span></span> <span data-ttu-id="65a08-163">Эта функция включена в `redis list`.</span><span class="sxs-lookup"><span data-stu-id="65a08-163">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="65a08-164">Вместо `redis import-method` теперь используется `redis import`.</span><span class="sxs-lookup"><span data-stu-id="65a08-164">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="65a08-165">Добавлена поддержка `--ids` для разных команд.</span><span class="sxs-lookup"><span data-stu-id="65a08-165">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="65a08-166">Роль</span><span class="sxs-lookup"><span data-stu-id="65a08-166">Role</span></span>

* <span data-ttu-id="65a08-167">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕИЕ] Удалено `ad sp reset-credentials` по причине устаревания.</span><span class="sxs-lookup"><span data-stu-id="65a08-167">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="65a08-168">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="65a08-168">Storage</span></span>

* <span data-ttu-id="65a08-169">Разрешено применение SAS-токенов назначения к источнику для копирования BLOB-объектов, если SAS источника и ключ учетной записи не указаны.</span><span class="sxs-lookup"><span data-stu-id="65a08-169">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="65a08-170">Добавлено отображение времени ожидания сокета для отправки и скачивания большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="65a08-170">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="65a08-171">Добавлена обработка имен больших двоичных объектов, которые начинаются с разделителей пути, как относительных путей.</span><span class="sxs-lookup"><span data-stu-id="65a08-171">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="65a08-172">Разрешено использовать `storage blob copy --source-sas` с начальным символом запроса "?".</span><span class="sxs-lookup"><span data-stu-id="65a08-172">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="65a08-173">Исправлено `storage entity query --marker` для принятия списка пар "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="65a08-173">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="65a08-174">ВМ</span><span class="sxs-lookup"><span data-stu-id="65a08-174">VM</span></span>

* <span data-ttu-id="65a08-175">Исправлена недопустимая логика обнаружения в URI неуправляемого BLOB-объекта.</span><span class="sxs-lookup"><span data-stu-id="65a08-175">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="65a08-176">Добавлена поддержка шифрования диска без предоставления пользователем субъектов-служб.</span><span class="sxs-lookup"><span data-stu-id="65a08-176">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="65a08-177">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕИЕ]. Не используйте ManagedIdentityExtension виртуальной машины для включения поддержки MSI.</span><span class="sxs-lookup"><span data-stu-id="65a08-177">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="65a08-178">Добавлена поддержка политики вытеснения для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="65a08-178">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="65a08-179">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕИЕ] Удалено `--ids` из:</span><span class="sxs-lookup"><span data-stu-id="65a08-179">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="65a08-180">Добавлена поддержка ускорителя записи.</span><span class="sxs-lookup"><span data-stu-id="65a08-180">Added write accelerator support</span></span> 
* <span data-ttu-id="65a08-181">Добавлена команда `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="65a08-181">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="65a08-182">Исправлено `vm diagnostics set` для надежного определения типа ОС виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="65a08-182">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="65a08-183">Изменено `vm resize` для проверки того, отличается ли запрошенный размер от установленного (с обновлением только при изменении).</span><span class="sxs-lookup"><span data-stu-id="65a08-183">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="65a08-184">10 апреля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="65a08-184">April 10, 2018</span></span>

<span data-ttu-id="65a08-185">Версия 2.0.31</span><span class="sxs-lookup"><span data-stu-id="65a08-185">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="65a08-186">ACR</span><span class="sxs-lookup"><span data-stu-id="65a08-186">ACR</span></span>

* <span data-ttu-id="65a08-187">Улучшена обработка ошибок при откате wincred.</span><span class="sxs-lookup"><span data-stu-id="65a08-187">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="65a08-188">ACS</span><span class="sxs-lookup"><span data-stu-id="65a08-188">ACS</span></span>

* <span data-ttu-id="65a08-189">Срок действия имен субъектов-служб, созданных службой контейнеров Azure, изменен до 5 лет.</span><span class="sxs-lookup"><span data-stu-id="65a08-189">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="65a08-190">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="65a08-190">Appservice</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕИЕ]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="65a08-192">Исправлено неперехватываемое исключение для несуществующих планов веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="65a08-192">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="65a08-193">Batch AI</span><span class="sxs-lookup"><span data-stu-id="65a08-193">BatchAI</span></span>

* <span data-ttu-id="65a08-194">Добавлена поддержка API 2018-03-01.</span><span class="sxs-lookup"><span data-stu-id="65a08-194">Added support for 2018-03-01 API</span></span>

 - <span data-ttu-id="65a08-195">Подключение на уровне задания.</span><span class="sxs-lookup"><span data-stu-id="65a08-195">Job level mounting</span></span>
 - <span data-ttu-id="65a08-196">Переменные среды со значениями секретов.</span><span class="sxs-lookup"><span data-stu-id="65a08-196">Environment variables with secret values</span></span>
 - <span data-ttu-id="65a08-197">Параметры счетчиков производительности</span><span class="sxs-lookup"><span data-stu-id="65a08-197">Performance counters settings</span></span>
 - <span data-ttu-id="65a08-198">Предоставление информации о сегменте пути конкретного задания.</span><span class="sxs-lookup"><span data-stu-id="65a08-198">Reporting of job specific path segment</span></span>
 - <span data-ttu-id="65a08-199">Поддержка вложенных папок в API списка файлов.</span><span class="sxs-lookup"><span data-stu-id="65a08-199">Support for subfolders in list files api</span></span>
 - <span data-ttu-id="65a08-200">Предоставление информации об использовании и ограничениях.</span><span class="sxs-lookup"><span data-stu-id="65a08-200">Usage and limits reporting</span></span>
 - <span data-ttu-id="65a08-201">Возможность указать тип кэширования для NFS-серверов.</span><span class="sxs-lookup"><span data-stu-id="65a08-201">Allow to specify caching type for NFS servers</span></span>
 - <span data-ttu-id="65a08-202">Поддержка пользовательских образов.</span><span class="sxs-lookup"><span data-stu-id="65a08-202">Support for custom images</span></span>
 - <span data-ttu-id="65a08-203">Добавлена поддержка инструментария pyTorch.</span><span class="sxs-lookup"><span data-stu-id="65a08-203">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="65a08-204">Добавлена команда `job wait`, позволяющая дождаться завершения задания и сообщить код выхода задания.</span><span class="sxs-lookup"><span data-stu-id="65a08-204">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="65a08-205">Добавлена команда `usage show`, позволяющая получить актуальные сведения об использовании и ограничениях ресурсов Batch AI для различных регионов.</span><span class="sxs-lookup"><span data-stu-id="65a08-205">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="65a08-206">Поддержка национальных облаков.</span><span class="sxs-lookup"><span data-stu-id="65a08-206">National clouds are supported</span></span>
* <span data-ttu-id="65a08-207">Для заданий добавлены аргументы командной строки, которые позволяют подключать файловые системы на уровне заданий. Эти же действия можно выполнять в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="65a08-207">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="65a08-208">Добавлены дополнительные параметры для настройки кластеров: приоритет виртуальной машины, подсеть, исходное число узлов для кластеров с автоматическим масштабированием, выбор пользовательского образа.</span><span class="sxs-lookup"><span data-stu-id="65a08-208">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="65a08-209">Добавлен параметр командной строки, который позволяет указать тип кэширования для управляемой файловой системы NFS службы Batch AI.</span><span class="sxs-lookup"><span data-stu-id="65a08-209">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="65a08-210">Упрощена процедура выбора подключаемой файловой системы в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="65a08-210">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="65a08-211">Теперь учетные данные для общего файлового ресурса Azure и контейнеров BLOB-объектов Azure указывать не нужно: CLI получит отсутствующие учетные данные с помощью ключа учетной записи хранения, указанного в параметрах командной строки, или переменной среды либо запросит ключ из службы хранилища Azure (если учетная запись хранения относится к текущей подписке).</span><span class="sxs-lookup"><span data-stu-id="65a08-211">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="65a08-212">Команда задания потоковой передачи файлов теперь автоматически завершается при завершении задания (успешное выполнение, сбой, прерывание или удаление).</span><span class="sxs-lookup"><span data-stu-id="65a08-212">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="65a08-213">Улучшены выходные данные `table` для операций `show`.</span><span class="sxs-lookup"><span data-stu-id="65a08-213">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="65a08-214">Добавлен параметр `--use-auto-storage` для создания кластера.</span><span class="sxs-lookup"><span data-stu-id="65a08-214">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="65a08-215">Этот параметр упрощает управление учетными записями хранения, а также подключение общего файлового ресурса Azure и контейнеров BLOB-объектов Azure к кластеру.</span><span class="sxs-lookup"><span data-stu-id="65a08-215">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="65a08-216">Добавлен параметр `--generate-ssh-keys` для команд `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="65a08-216">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="65a08-217">Добавлена возможность запустить задачу настройки узла через командную строку.</span><span class="sxs-lookup"><span data-stu-id="65a08-217">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="65a08-218">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕИЕ] Команды `job stream-file` и `job list-files` перемещены в группу `job file`.</span><span class="sxs-lookup"><span data-stu-id="65a08-218">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="65a08-219">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕИЕ] В команде `file-server create` параметр `--admin-user-name` переименован в `--user-name` для согласованности с командой `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="65a08-219">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="65a08-220">Выставление счетов</span><span class="sxs-lookup"><span data-stu-id="65a08-220">Billing</span></span>

* <span data-ttu-id="65a08-221">Добавлены команды для учетной записи регистрации.</span><span class="sxs-lookup"><span data-stu-id="65a08-221">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="65a08-222">Потребление</span><span class="sxs-lookup"><span data-stu-id="65a08-222">Consumption</span></span>

* <span data-ttu-id="65a08-223">Добавлены команды `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="65a08-223">Added `marketplace` commands</span></span>
* <span data-ttu-id="65a08-224">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕИЕ] Команда `reservations summaries` переименована в `reservation summary`.</span><span class="sxs-lookup"><span data-stu-id="65a08-224">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="65a08-225">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕИЕ] Команда `reservations details` переименована в `reservation detail`.</span><span class="sxs-lookup"><span data-stu-id="65a08-225">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="65a08-226">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕИЕ] В командах `reservation` удалены короткие параметры `--reservation-order-id` и `--reservation-id`.</span><span class="sxs-lookup"><span data-stu-id="65a08-226">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="65a08-227">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕИЕ] В командах `reservation summary` удалены короткие параметры `--grain`.</span><span class="sxs-lookup"><span data-stu-id="65a08-227">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="65a08-228">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕИЕ] В командах `pricesheet` удалены короткие параметры `--include-meter-details`.</span><span class="sxs-lookup"><span data-stu-id="65a08-228">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="65a08-229">Контейнер</span><span class="sxs-lookup"><span data-stu-id="65a08-229">Container</span></span>

* <span data-ttu-id="65a08-230">Добавлены параметры подключения тома репозитория git: `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` и `--gitrepo-mount-path`.</span><span class="sxs-lookup"><span data-stu-id="65a08-230">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="65a08-231">Исправлена ошибка [#5926](https://github.com/Azure/azure-cli/issues/5926): команда `az container exec` возвращает ошибку, когда указан параметр --container-name.</span><span class="sxs-lookup"><span data-stu-id="65a08-231">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="65a08-232">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="65a08-232">Extension</span></span>

* <span data-ttu-id="65a08-233">Сообщение о проверке распространения перенесено на уровень отладки.</span><span class="sxs-lookup"><span data-stu-id="65a08-233">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="65a08-234">Interactive</span><span class="sxs-lookup"><span data-stu-id="65a08-234">Interactive</span></span>

* <span data-ttu-id="65a08-235">Если команда не распознана, выполнение прерывается.</span><span class="sxs-lookup"><span data-stu-id="65a08-235">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="65a08-236">Добавлены перехватчики событий, которые используются до и после создания поддерева команд.</span><span class="sxs-lookup"><span data-stu-id="65a08-236">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="65a08-237">Добавлены сведения о выполнении для параметров `--ids`.</span><span class="sxs-lookup"><span data-stu-id="65a08-237">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="65a08-238">Сеть</span><span class="sxs-lookup"><span data-stu-id="65a08-238">Network</span></span>

* <span data-ttu-id="65a08-239">Исправлена ошибка [#5936](https://github.com/Azure/azure-cli/issues/5936): не задаются теги `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="65a08-239">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="65a08-240">Добавлен аргумент `--auth-certs`, который позволяет подключать сертификаты аутентификации для `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="65a08-240">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> <span data-ttu-id="65a08-241">[#4910](https://github.com/Azure/azure-cli/issues/4910).</span><span class="sxs-lookup"><span data-stu-id="65a08-241">[#4910](https://github.com/Azure/azure-cli/issues/4910)</span></span>
* <span data-ttu-id="65a08-242">Добавлены команды `ddos-protection` для создания планов защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="65a08-242">Added `ddos-protection` commands to create DDoS protection plans</span></span> 
* <span data-ttu-id="65a08-243">В команду `vnet [create|update]` добавлена поддержка `--ddos-protection-plan` для связи виртуальной сети с планом защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="65a08-243">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="65a08-244">Исправлена ошибка с флагом `--disable-bgp-route-propagation` в команде `network route-table [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="65a08-244">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="65a08-245">Удалены фиктивные аргументы `--public-ip-address-type` и `--subnet-type` для команды `network lb [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="65a08-245">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="65a08-246">В `network dns zone [import|export]` и `network dns record-set txt add-record` добавлена поддержка записей типа TXT с escape-последовательностями RFC 1035.</span><span class="sxs-lookup"><span data-stu-id="65a08-246">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="65a08-247">Профиль</span><span class="sxs-lookup"><span data-stu-id="65a08-247">Profile</span></span>

* <span data-ttu-id="65a08-248">Добавлена поддержка классических учетных записей Azure для команды `account list`.</span><span class="sxs-lookup"><span data-stu-id="65a08-248">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="65a08-249">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕИЕ] Удалены аргументы `--msi`  &  `--msi-port`.</span><span class="sxs-lookup"><span data-stu-id="65a08-249">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="65a08-250">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="65a08-250">RDBMS</span></span>

* <span data-ttu-id="65a08-251">Добавлена команда `georestore`.</span><span class="sxs-lookup"><span data-stu-id="65a08-251">Added `georestore` command</span></span>
* <span data-ttu-id="65a08-252">Из команды `create` исключено ограничение на размер хранилища.</span><span class="sxs-lookup"><span data-stu-id="65a08-252">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="65a08-253">Ресурс</span><span class="sxs-lookup"><span data-stu-id="65a08-253">Resource</span></span>

* <span data-ttu-id="65a08-254">Добавлена поддержка параметра `--metadata` в команде `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="65a08-254">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="65a08-255">Добавлена поддержка `--metadata`, `--set`, `--add` и `--remove` для команды `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="65a08-255">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="65a08-256">SQL</span><span class="sxs-lookup"><span data-stu-id="65a08-256">SQL</span></span>

* <span data-ttu-id="65a08-257">Добавлены команды `sql elastic-pool op list` и `sql elastic-pool op cancel`.</span><span class="sxs-lookup"><span data-stu-id="65a08-257">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="65a08-258">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="65a08-258">Storage</span></span>

* <span data-ttu-id="65a08-259">Улучшены сообщения об ошибках для строк подключения, имеющих неправильный формат.</span><span class="sxs-lookup"><span data-stu-id="65a08-259">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="65a08-260">ВМ</span><span class="sxs-lookup"><span data-stu-id="65a08-260">VM</span></span>

* <span data-ttu-id="65a08-261">В команде `vmss create` добавлена возможность настроить для платформы количество доменов сбоя.</span><span class="sxs-lookup"><span data-stu-id="65a08-261">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="65a08-262">Команда `vmss create` теперь по умолчанию использует стандартную балансировку нагрузки для зональных и больших масштабируемых наборов, а также масштабируемых наборов, в которых отключена одна группа размещения.</span><span class="sxs-lookup"><span data-stu-id="65a08-262">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="65a08-264">Добавлена поддержка SKU общедоступного IP-адреса для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="65a08-264">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="65a08-265">В команду `vm secret format` добавлены аргументы `--keyvault` и `--resource-group` для тех случаев, когда команда не может разрешить идентификатор хранилища.</span><span class="sxs-lookup"><span data-stu-id="65a08-265">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> <span data-ttu-id="65a08-266">[#5718](https://github.com/Azure/azure-cli/issues/5718).</span><span class="sxs-lookup"><span data-stu-id="65a08-266">[#5718](https://github.com/Azure/azure-cli/issues/5718)</span></span>
* <span data-ttu-id="65a08-267">Улучшены сообщения об ошибках для команды `[vm|vmss create]`, когда расположение группы ресурсов не поддерживает зоны.</span><span class="sxs-lookup"><span data-stu-id="65a08-267">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="65a08-268">27 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="65a08-268">March 27, 2018</span></span>

<span data-ttu-id="65a08-269">Версия 2.0.30</span><span class="sxs-lookup"><span data-stu-id="65a08-269">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="65a08-270">Core</span><span class="sxs-lookup"><span data-stu-id="65a08-270">Core</span></span>

* <span data-ttu-id="65a08-271">Отображение сообщения для расширений, которые отмечены в справке как предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="65a08-271">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="65a08-272">ACS</span><span class="sxs-lookup"><span data-stu-id="65a08-272">ACS</span></span>

* <span data-ttu-id="65a08-273">Устранена ошибка с проверкой SSL-сертификата для `aks install-cli` в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="65a08-273">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="65a08-274">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="65a08-274">Appservice</span></span>

* <span data-ttu-id="65a08-275">Добавлена поддержка только протокола HTTPS для `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="65a08-275">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="65a08-276">Добавлена поддержка слотов для `az webapp identity [assign|show]` и `az functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="65a08-276">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="65a08-277">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="65a08-277">Backup</span></span>

* <span data-ttu-id="65a08-278">Добавлена новая команда `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="65a08-278">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="65a08-279">Эта команда используется для проверки резервного копирования виртуальной машины в любое хранилище в подписке.</span><span class="sxs-lookup"><span data-stu-id="65a08-279">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="65a08-280">Включены идентификаторы объектов Azure для параметров `--resource-group` и `--vault-name` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="65a08-280">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="65a08-281">Изменены параметры `--name` для поддержки формата вывода команд `backup ... show`.</span><span class="sxs-lookup"><span data-stu-id="65a08-281">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="65a08-282">Контейнер</span><span class="sxs-lookup"><span data-stu-id="65a08-282">Container</span></span>

* <span data-ttu-id="65a08-283">Добавлена команда `container exec`.</span><span class="sxs-lookup"><span data-stu-id="65a08-283">Added `container exec` command.</span></span> <span data-ttu-id="65a08-284">Выполнение команды в контейнере для выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="65a08-284">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="65a08-285">Разрешение выходной таблице создавать и обновлять группу контейнеров.</span><span class="sxs-lookup"><span data-stu-id="65a08-285">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="65a08-286">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="65a08-286">Extension</span></span>

* <span data-ttu-id="65a08-287">Добавлено сообщение для `extension add`, если расширение доступно в режиме предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="65a08-287">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="65a08-288">Изменен параметр `extension list-available` для отображения всех данных расширения с использованием `--show-details`.</span><span class="sxs-lookup"><span data-stu-id="65a08-288">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="65a08-289">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕИЕ] Изменена команда `extension list-available` для отображения упрощенных данных расширения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="65a08-289">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="65a08-290">Interactive</span><span class="sxs-lookup"><span data-stu-id="65a08-290">Interactive</span></span>

* <span data-ttu-id="65a08-291">Изменены операции завершения, активируемые сразу после завершения загрузки таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="65a08-291">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="65a08-292">Исправлена ошибка с использованием параметра `--style`.</span><span class="sxs-lookup"><span data-stu-id="65a08-292">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="65a08-293">Отсутствующий интерактивный лексический анализатор создается после дампа таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="65a08-293">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="65a08-294">Улучшена поддержка средства заполнения.</span><span class="sxs-lookup"><span data-stu-id="65a08-294">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="65a08-295">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="65a08-295">Lab</span></span>

* <span data-ttu-id="65a08-296">Исправлены ошибки с командой `create environment`.</span><span class="sxs-lookup"><span data-stu-id="65a08-296">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="65a08-297">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="65a08-297">Monitor</span></span>

* <span data-ttu-id="65a08-298">Добавлена поддержка `--top`, `--orderby` и `--namespace` для `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="65a08-298">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="65a08-299">Исправлена ошибка [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` принимает разделенный пробелами список метрик для извлечения.</span><span class="sxs-lookup"><span data-stu-id="65a08-299">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="65a08-300">Добавлена поддержка `--namespace` для `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="65a08-300">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="65a08-301">Сеть</span><span class="sxs-lookup"><span data-stu-id="65a08-301">Network</span></span>

* <span data-ttu-id="65a08-302">Добавлена поддержка Частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="65a08-302">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="65a08-303">Профиль</span><span class="sxs-lookup"><span data-stu-id="65a08-303">Profile</span></span>

* <span data-ttu-id="65a08-304">Добавлено предупреждение для `--identity-port` и `--msi-port` в `login`.</span><span class="sxs-lookup"><span data-stu-id="65a08-304">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="65a08-305">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="65a08-305">RDBMS</span></span>

* <span data-ttu-id="65a08-306">Добавлена общедоступная версия 2017-12-01 бизнес-модели API.</span><span class="sxs-lookup"><span data-stu-id="65a08-306">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="65a08-307">Ресурс</span><span class="sxs-lookup"><span data-stu-id="65a08-307">Resource</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="65a08-309">Роль</span><span class="sxs-lookup"><span data-stu-id="65a08-309">Role</span></span>

* <span data-ttu-id="65a08-310">Добавлена поддержка конфигурации требуемого уровня доступа и собственных клиентов для `az ad app create`.</span><span class="sxs-lookup"><span data-stu-id="65a08-310">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="65a08-311">Изменены команды `rbac`, чтобы возвращать не более 1000 идентификаторов в разрешении объекта.</span><span class="sxs-lookup"><span data-stu-id="65a08-311">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="65a08-312">Добавлены команды `ad sp credential [reset|list|delete]` для управления учетными данными.</span><span class="sxs-lookup"><span data-stu-id="65a08-312">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="65a08-313">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕИЕ] Удален параметр properties из выходных данных `az role assignment [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="65a08-313">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="65a08-314">Добавлена поддержка разрешений `dataActions` и `notDataActions` для `role definition`.</span><span class="sxs-lookup"><span data-stu-id="65a08-314">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="65a08-315">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="65a08-315">Storage</span></span>

* <span data-ttu-id="65a08-316">Исправлена проблема с отправкой файла размером от 195 до 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="65a08-316">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="65a08-317">Исправлена ошибка [#4049](https://github.com/Azure/azure-cli/issues/4049): проблемы, когда при отправке добавочного большого двоичного объекта игнорируются параметры условия.</span><span class="sxs-lookup"><span data-stu-id="65a08-317">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="65a08-318">ВМ</span><span class="sxs-lookup"><span data-stu-id="65a08-318">VM</span></span>

* <span data-ttu-id="65a08-319">Добавлено предупреждение `vmss create` для предстоящих критически важных изменений для наборов из 100 и более экземпляров.</span><span class="sxs-lookup"><span data-stu-id="65a08-319">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="65a08-320">Добавлена поддержка устойчивости зон для `vm [snapshot|image]`.</span><span class="sxs-lookup"><span data-stu-id="65a08-320">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="65a08-321">Изменено представление экземпляра диска для улучшения отчета о состоянии шифрования.</span><span class="sxs-lookup"><span data-stu-id="65a08-321">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="65a08-322">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕИЕ] `vm extension delete` Изменена команда, которая больше не возвращает выходные данные.</span><span class="sxs-lookup"><span data-stu-id="65a08-322">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="65a08-323">13 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="65a08-323">March 13, 2018</span></span>

<span data-ttu-id="65a08-324">Версия 2.0.29</span><span class="sxs-lookup"><span data-stu-id="65a08-324">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="65a08-325">ACR</span><span class="sxs-lookup"><span data-stu-id="65a08-325">ACR</span></span>

* <span data-ttu-id="65a08-326">Добавлена поддержка параметра `--image` для `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="65a08-326">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="65a08-327">Параметры `--manifest` и `--tag` команды `repository delete` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="65a08-327">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="65a08-328">Добавлена команда `repository untag` для удаления тега без удаления данных.</span><span class="sxs-lookup"><span data-stu-id="65a08-328">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="65a08-329">ACS</span><span class="sxs-lookup"><span data-stu-id="65a08-329">ACS</span></span>

* <span data-ttu-id="65a08-330">Добавлена команда `aks upgrade-connector` для обновления существующего соединителя.</span><span class="sxs-lookup"><span data-stu-id="65a08-330">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="65a08-331">Изменены файлы конфигурации `kubectl`. Теперь используется более разборчивый стиль YAML с разбивкой на блоки.</span><span class="sxs-lookup"><span data-stu-id="65a08-331">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="65a08-332">Помощник</span><span class="sxs-lookup"><span data-stu-id="65a08-332">Advisor</span></span>

* <span data-ttu-id="65a08-333">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕИЕ] Команда `advisor configuration get` переименована в `advisor configuration list`.</span><span class="sxs-lookup"><span data-stu-id="65a08-333">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="65a08-334">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕИЕ] Команда `advisor configuration set` переименована в `advisor configuration update`.</span><span class="sxs-lookup"><span data-stu-id="65a08-334">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="65a08-335">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕИЕ] Удалена команда `advisor recommendation generate`.</span><span class="sxs-lookup"><span data-stu-id="65a08-335">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span> 
* <span data-ttu-id="65a08-336">Добавлен параметр `--refresh` для команды `advisor recommendation list`.</span><span class="sxs-lookup"><span data-stu-id="65a08-336">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="65a08-337">Добавлена команда `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="65a08-337">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="65a08-338">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="65a08-338">Appservice</span></span>

* <span data-ttu-id="65a08-339">Команда `[webapp|functionapp] assign-identity` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="65a08-339">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="65a08-340">Добавлены команды управляемого удостоверения `webapp identity [assign|show]` и `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="65a08-340">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="65a08-341">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="65a08-341">Eventhubs</span></span>

* <span data-ttu-id="65a08-342">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="65a08-342">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="65a08-343">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="65a08-343">Extension</span></span>

* <span data-ttu-id="65a08-344">Добавлена проверка, позволяющая предупредить пользователя, если используемый дистрибутив отличается от хранящегося в исходном файле пакета, так как это может привести к возникновению ошибок.</span><span class="sxs-lookup"><span data-stu-id="65a08-344">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="65a08-345">Interactive</span><span class="sxs-lookup"><span data-stu-id="65a08-345">Interactive</span></span>

* <span data-ttu-id="65a08-346">Исправлена ошибка [#5625](https://github.com/Azure/azure-cli/issues/5625): теперь записи журнала сохраняются в разных сеансах.</span><span class="sxs-lookup"><span data-stu-id="65a08-346">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="65a08-347">Исправлена ошибка [#3016](https://github.com/Azure/azure-cli/issues/3016): при использовании области не создавались записи журнала.</span><span class="sxs-lookup"><span data-stu-id="65a08-347">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="65a08-348">Исправлена ошибка [#5688](https://github.com/Azure/azure-cli/issues/5688): если при загрузке таблицы команд возникало исключение, опережающий ввод не выполнялся.</span><span class="sxs-lookup"><span data-stu-id="65a08-348">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="65a08-349">Исправлен индикатор хода выполнения для длительных операций.</span><span class="sxs-lookup"><span data-stu-id="65a08-349">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="65a08-350">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="65a08-350">Monitor</span></span>

* <span data-ttu-id="65a08-351">Команды `monitor autoscale-settings` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="65a08-351">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="65a08-352">Добавлены команды `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="65a08-352">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="65a08-353">Добавлены команды `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="65a08-353">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="65a08-354">Добавлены команды `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="65a08-354">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="65a08-355">Сеть</span><span class="sxs-lookup"><span data-stu-id="65a08-355">Network</span></span>

* <span data-ttu-id="65a08-356">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕИЕ] Удален параметр `--tags` из `route-filter rule create`.</span><span class="sxs-lookup"><span data-stu-id="65a08-356">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="65a08-357">Удалены некоторые ошибочные значения по умолчанию для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="65a08-357">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="65a08-358">Добавлены команды `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="65a08-358">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="65a08-359">Добавлены параметры `--vnet` и `--subnet` для `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="65a08-359">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="65a08-360">Профиль</span><span class="sxs-lookup"><span data-stu-id="65a08-360">Profile</span></span>

* <span data-ttu-id="65a08-361">Параметр `--msi` для `az login` отмечен как нерекомендуемый.</span><span class="sxs-lookup"><span data-stu-id="65a08-361">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="65a08-362">Добавлен параметр `--identity` для `az login`. Он заменяет `--msi`.</span><span class="sxs-lookup"><span data-stu-id="65a08-362">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="65a08-363">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="65a08-363">RDBMS</span></span>

* <span data-ttu-id="65a08-364">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Внесены изменения для использования предварительной версии API 2017-12-01.</span><span class="sxs-lookup"><span data-stu-id="65a08-364">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="65a08-365">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="65a08-365">Service Bus</span></span>

* <span data-ttu-id="65a08-366">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="65a08-366">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="65a08-367">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="65a08-367">Storage</span></span>

* <span data-ttu-id="65a08-368">Исправлена ошибка [#4971](https://github.com/Azure/azure-cli/issues/4971): теперь `storage blob copy` поддерживает другие облака Azure.</span><span class="sxs-lookup"><span data-stu-id="65a08-368">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="65a08-369">Исправлена ошибка [#5286](https://github.com/Azure/azure-cli/issues/5286): при пакетном выполнении команд `storage blob [delete-batch|download-batch|upload-batch]` больше не отображается сообщение об ошибке в предусловии.</span><span class="sxs-lookup"><span data-stu-id="65a08-369">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="65a08-370">ВМ</span><span class="sxs-lookup"><span data-stu-id="65a08-370">VM</span></span>

* <span data-ttu-id="65a08-371">В `[vm|vmss] create` добавлена поддержка присоединения неуправляемых дисков данных и настройки кэширования.</span><span class="sxs-lookup"><span data-stu-id="65a08-371">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="65a08-372">`[vm|vmss] assign-identity` и `[vm|vmss] remove-identity` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="65a08-372">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="65a08-373">Вместо нерекомендуемых команд добавлены команды `vm identity [assign|remove|show]` и `vmss identity [assign|remove|show]`.</span><span class="sxs-lookup"><span data-stu-id="65a08-373">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="65a08-374">Для приоритета `vmss create` по умолчанию установлено значение None.</span><span class="sxs-lookup"><span data-stu-id="65a08-374">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="65a08-375">27 февраля 2018 г</span><span class="sxs-lookup"><span data-stu-id="65a08-375">February 27, 2018</span></span>

<span data-ttu-id="65a08-376">Версия 2.0.28</span><span class="sxs-lookup"><span data-stu-id="65a08-376">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="65a08-377">Core</span><span class="sxs-lookup"><span data-stu-id="65a08-377">Core</span></span>

* <span data-ttu-id="65a08-378">Исправлена ошибка с установкой Homebrew [№ 5184](https://github.com/Azure/azure-cli/issues/5184).</span><span class="sxs-lookup"><span data-stu-id="65a08-378">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="65a08-379">Добавлена поддержка телеметрии расширения с применением пользовательских ключей.</span><span class="sxs-lookup"><span data-stu-id="65a08-379">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="65a08-380">Добавлена функция ведения журнала HTTP в `--debug`.</span><span class="sxs-lookup"><span data-stu-id="65a08-380">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="65a08-381">ACS</span><span class="sxs-lookup"><span data-stu-id="65a08-381">ACS</span></span>

* <span data-ttu-id="65a08-382">Изменено для использования диаграмм Helm `virtual-kubelet-for-aks` для `aks install-connector` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="65a08-382">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="65a08-383">Исправлена ошибка с недостаточными разрешениями субъектов-служб на создание групп контейнеров ACI.</span><span class="sxs-lookup"><span data-stu-id="65a08-383">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="65a08-384">Добавлены параметры `--aci-container-group`, `--location` и `--image-tag` для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="65a08-384">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="65a08-385">Удалено уведомление об устаревании из `aks get-versions`.</span><span class="sxs-lookup"><span data-stu-id="65a08-385">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="65a08-386">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="65a08-386">Appservice</span></span>

* <span data-ttu-id="65a08-387">Обновления для новой версии пакета SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="65a08-387">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="65a08-388">Исправлена ошибка с сообщением `Free` о недопустимом SKU [№ 5538](https://github.com/Azure/azure-cli/issues/5538)</span><span class="sxs-lookup"><span data-stu-id="65a08-388">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="65a08-389">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="65a08-389">Cognitive Services</span></span>

* <span data-ttu-id="65a08-390">Обновлено уведомление при создании новой учетной записи Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="65a08-390">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="65a08-391">Потребление</span><span class="sxs-lookup"><span data-stu-id="65a08-391">Consumption</span></span>

* <span data-ttu-id="65a08-392">Добавлены новые команды для резервирования API прейскуранта.</span><span class="sxs-lookup"><span data-stu-id="65a08-392">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="65a08-393">Обновлены существующие форматы сведений об использовании и резервировании.</span><span class="sxs-lookup"><span data-stu-id="65a08-393">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="65a08-394">Контейнер</span><span class="sxs-lookup"><span data-stu-id="65a08-394">Container</span></span>

* <span data-ttu-id="65a08-395">Добавлены аргументы `--secrets` и `--secrets-mount-path` в командах `container create` для использования секретов в ACI.</span><span class="sxs-lookup"><span data-stu-id="65a08-395">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="65a08-396">Сеть</span><span class="sxs-lookup"><span data-stu-id="65a08-396">Network</span></span>

* <span data-ttu-id="65a08-397">Исправлена ошибка с отсутствующим клиентом в `network vnet-gateway vpn-client generate` [№ 5559](https://github.com/Azure/azure-cli/issues/5559).</span><span class="sxs-lookup"><span data-stu-id="65a08-397">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="65a08-398">Ресурс</span><span class="sxs-lookup"><span data-stu-id="65a08-398">Resource</span></span>

* <span data-ttu-id="65a08-399">Изменено `group deployment export` для отображения частичного шаблона и ошибок при сбое.</span><span class="sxs-lookup"><span data-stu-id="65a08-399">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="65a08-400">Роль</span><span class="sxs-lookup"><span data-stu-id="65a08-400">Role</span></span>

* <span data-ttu-id="65a08-401">Добавлено `role assignment list-changelogs` для включения аудита ролей субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="65a08-401">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="65a08-402">SQL</span><span class="sxs-lookup"><span data-stu-id="65a08-402">SQL</span></span>

* <span data-ttu-id="65a08-403">Добавлена поддержка избыточности зон для создания и обновления баз данных и эластичных пулов.</span><span class="sxs-lookup"><span data-stu-id="65a08-403">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="65a08-404">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="65a08-404">Storage</span></span>

* <span data-ttu-id="65a08-405">Включено определение пути назначения и префикса для `storage blob [upload-batch|download-batch]`.</span><span class="sxs-lookup"><span data-stu-id="65a08-405">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="65a08-406">ВМ</span><span class="sxs-lookup"><span data-stu-id="65a08-406">VM</span></span>

* <span data-ttu-id="65a08-407">Добавлена поддержка присоединения и отсоединения дисков на одном экземпляре VMSS.</span><span class="sxs-lookup"><span data-stu-id="65a08-407">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="65a08-408">13 февраля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="65a08-408">February 13, 2018</span></span>

<span data-ttu-id="65a08-409">Версия 2.0.27</span><span class="sxs-lookup"><span data-stu-id="65a08-409">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="65a08-410">Core</span><span class="sxs-lookup"><span data-stu-id="65a08-410">Core</span></span>

* <span data-ttu-id="65a08-411">Изменен способ аутентификации при входе с помощью MSI: применяется ключ при использовании идентификатора подписки и имени.</span><span class="sxs-lookup"><span data-stu-id="65a08-411">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="65a08-412">ACS</span><span class="sxs-lookup"><span data-stu-id="65a08-412">ACS</span></span>

* <span data-ttu-id="65a08-413">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕИЕ] Переименовано `aks get-versions` на `aks get-upgrades` для точности.</span><span class="sxs-lookup"><span data-stu-id="65a08-413">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="65a08-414">Изменено `aks get-versions` для отображения версий Kubernetes, доступных для `aks create`.</span><span class="sxs-lookup"><span data-stu-id="65a08-414">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="65a08-415">Изменены значения по умолчанию `aks create`, чтобы разрешить серверу выбирать версию Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="65a08-415">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="65a08-416">Обновлены справочные сообщения, связанные с субъектом-службой и создаваемые AKS.</span><span class="sxs-lookup"><span data-stu-id="65a08-416">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="65a08-417">Изменены стандартные размеры узла для `aks create` с уровня Standard\_D1\_v2 на уровень Standard\_DS1\_v2.</span><span class="sxs-lookup"><span data-stu-id="65a08-417">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="65a08-418">Улучшена надежность при поиске панели мониторинга для группы pod для `az aks browse`.</span><span class="sxs-lookup"><span data-stu-id="65a08-418">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="65a08-419">Исправлена команда `aks get-credentials` для обработки ошибок Юникода при загрузке файлов конфигурации Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="65a08-419">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="65a08-420">Добавлено сообщение в `az aks install-cli`, чтобы помочь получить `kubectl` в `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="65a08-420">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="65a08-421">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="65a08-421">Appservice</span></span>

* <span data-ttu-id="65a08-422">Исправлена проблема со сбоем `webapp [backup|restore]` из-за пустой ссылки.</span><span class="sxs-lookup"><span data-stu-id="65a08-422">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="65a08-423">Добавлена поддержка стандартных планов службы приложений с помощью `az configure --defaults appserviceplan=my-asp`.</span><span class="sxs-lookup"><span data-stu-id="65a08-423">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="65a08-424">CDN</span><span class="sxs-lookup"><span data-stu-id="65a08-424">CDN</span></span>

* <span data-ttu-id="65a08-425">Добавлены команды `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="65a08-425">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="65a08-426">Контейнер</span><span class="sxs-lookup"><span data-stu-id="65a08-426">Container</span></span>

* <span data-ttu-id="65a08-427">Добавлен параметр `--follow` для `az container logs` для журналов потоковой передачи.</span><span class="sxs-lookup"><span data-stu-id="65a08-427">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="65a08-428">Добавлена команда `container attach`, которая добавляет локальный стандартный поток вывода и поток вывода сообщений об ошибках к контейнеру в группе контейнеров.</span><span class="sxs-lookup"><span data-stu-id="65a08-428">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="65a08-429">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="65a08-429">CosmosDB</span></span>

* <span data-ttu-id="65a08-430">Добавлена поддержка настройки параметров.</span><span class="sxs-lookup"><span data-stu-id="65a08-430">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="65a08-431">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="65a08-431">Extension</span></span>

* <span data-ttu-id="65a08-432">Добавлена поддержка параметра `--pip-proxy` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="65a08-432">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="65a08-433">Добавлена поддержка аргумента `--pip-extra-index-urls` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="65a08-433">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="65a08-434">Отзыв</span><span class="sxs-lookup"><span data-stu-id="65a08-434">Feedback</span></span>

* <span data-ttu-id="65a08-435">Добавлены сведения о расширении к данным телеметрии.</span><span class="sxs-lookup"><span data-stu-id="65a08-435">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="65a08-436">Interactive</span><span class="sxs-lookup"><span data-stu-id="65a08-436">Interactive</span></span>

* <span data-ttu-id="65a08-437">Исправлена проблема, когда пользователю предлагалось войти в интерактивном режиме в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="65a08-437">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="65a08-438">Исправлена регрессия с отсутствующей функцией заполнения параметров.</span><span class="sxs-lookup"><span data-stu-id="65a08-438">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="65a08-439">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="65a08-439">IoT</span></span>

* <span data-ttu-id="65a08-440">Исправлена проблема, когда `iot dps access policy [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="65a08-440">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="65a08-441">Исправлена проблема, когда `iot dps linked-hub [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="65a08-441">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="65a08-442">Добавлена поддержка параметра `--no-wait` для `iot dps access policy [create|update]` и `iot dps linked-hub [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="65a08-442">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="65a08-443">Изменена команда `iot hub create` для указания числа секций.</span><span class="sxs-lookup"><span data-stu-id="65a08-443">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="65a08-444">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="65a08-444">Monitor</span></span>

* <span data-ttu-id="65a08-445">Исправлена команда `az monitor log-profiles create`.</span><span class="sxs-lookup"><span data-stu-id="65a08-445">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="65a08-446">Сеть</span><span class="sxs-lookup"><span data-stu-id="65a08-446">Network</span></span>

* <span data-ttu-id="65a08-447">Исправлен параметр `--tags` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="65a08-447">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="65a08-448">Профиль</span><span class="sxs-lookup"><span data-stu-id="65a08-448">Profile</span></span>

* <span data-ttu-id="65a08-449">Включена команда `az login` для использования в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="65a08-449">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="65a08-450">Ресурс</span><span class="sxs-lookup"><span data-stu-id="65a08-450">Resource</span></span>

* <span data-ttu-id="65a08-451">Снова добавлена команда `feature show`.</span><span class="sxs-lookup"><span data-stu-id="65a08-451">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="65a08-452">Роль</span><span class="sxs-lookup"><span data-stu-id="65a08-452">Role</span></span>

* <span data-ttu-id="65a08-453">Добавлен аргумент `--available-to-other-tenants` для команды `ad app update`</span><span class="sxs-lookup"><span data-stu-id="65a08-453">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="65a08-454">SQL</span><span class="sxs-lookup"><span data-stu-id="65a08-454">SQL</span></span>

* <span data-ttu-id="65a08-455">Добавлены команды `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="65a08-455">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="65a08-456">Добавлена команда `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="65a08-456">Added `sql db rename`</span></span>
* <span data-ttu-id="65a08-457">Добавлена поддержка аргумента `--ids` для команд SQL.</span><span class="sxs-lookup"><span data-stu-id="65a08-457">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="65a08-458">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="65a08-458">Storage</span></span>

* <span data-ttu-id="65a08-459">Добавлены команды `storage blob service-properties delete-policy` и `storage blob undelete` для включения обратимого удаления.</span><span class="sxs-lookup"><span data-stu-id="65a08-459">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="65a08-460">ВМ</span><span class="sxs-lookup"><span data-stu-id="65a08-460">VM</span></span>

* <span data-ttu-id="65a08-461">Исправлена ошибка, когда шифрование виртуальной машины инициализировалось не полностью.</span><span class="sxs-lookup"><span data-stu-id="65a08-461">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="65a08-462">Добавлены выходные данные идентификатора субъекта для включения MSI.</span><span class="sxs-lookup"><span data-stu-id="65a08-462">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="65a08-463">Фиксированное значение `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="65a08-463">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="65a08-464">31 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="65a08-464">January 31, 2018</span></span>

<span data-ttu-id="65a08-465">Версия 2.0.26</span><span class="sxs-lookup"><span data-stu-id="65a08-465">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="65a08-466">Core</span><span class="sxs-lookup"><span data-stu-id="65a08-466">Core</span></span>

* <span data-ttu-id="65a08-467">Добавлена поддержка получения необработанного маркера в контексте MSI.</span><span class="sxs-lookup"><span data-stu-id="65a08-467">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="65a08-468">Удалена строка индикатора опроса после завершения LRO при выполнении cmd.exe в Windows.</span><span class="sxs-lookup"><span data-stu-id="65a08-468">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="65a08-469">Добавлено предупреждение, которое появляется при использовании настроенных по умолчанию параметров, измененных на запись уровня INFO.</span><span class="sxs-lookup"><span data-stu-id="65a08-469">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="65a08-470">Используйте `--verbose` для просмотра.</span><span class="sxs-lookup"><span data-stu-id="65a08-470">Use `--verbose` to see</span></span>
* <span data-ttu-id="65a08-471">Добавьте индикатор хода выполнения для ожидания команд.</span><span class="sxs-lookup"><span data-stu-id="65a08-471">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="65a08-472">ACS</span><span class="sxs-lookup"><span data-stu-id="65a08-472">ACS</span></span>

* <span data-ttu-id="65a08-473">Добавлено описание аргумента `--disable-browser`.</span><span class="sxs-lookup"><span data-stu-id="65a08-473">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="65a08-474">Улучшено заполнение нажатием клавиши TAB для аргументов `--vm-size`.</span><span class="sxs-lookup"><span data-stu-id="65a08-474">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="65a08-475">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="65a08-475">Appservice</span></span>

* <span data-ttu-id="65a08-476">Фиксированное значение `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="65a08-476">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="65a08-477">Удалена проверка `kind` в веб-приложениях и функциях.</span><span class="sxs-lookup"><span data-stu-id="65a08-477">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="65a08-478">CDN</span><span class="sxs-lookup"><span data-stu-id="65a08-478">CDN</span></span>

* <span data-ttu-id="65a08-479">Устранена проблема с отсутствием клиента для команды `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="65a08-479">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="65a08-480">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="65a08-480">CosmosDB</span></span>

* <span data-ttu-id="65a08-481">Исправлено описание параметров для политик отработки отказа.</span><span class="sxs-lookup"><span data-stu-id="65a08-481">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="65a08-482">Interactive</span><span class="sxs-lookup"><span data-stu-id="65a08-482">Interactive</span></span>

* <span data-ttu-id="65a08-483">Исправлена проблема, когда заполнение параметров команд больше не выполнялось.</span><span class="sxs-lookup"><span data-stu-id="65a08-483">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="65a08-484">Сеть</span><span class="sxs-lookup"><span data-stu-id="65a08-484">Network</span></span>

* <span data-ttu-id="65a08-485">Добавлена защита `--cert-password` для `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="65a08-485">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="65a08-486">Исправлена проблема с `application-gateway update`, когда команда `--sku` ошибочно применяла значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="65a08-486">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="65a08-487">Добавлена защита `--shared-key` и `--authorization-key` для `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="65a08-487">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="65a08-488">Устранена проблема с отсутствием клиента для команды `asg create`.</span><span class="sxs-lookup"><span data-stu-id="65a08-488">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="65a08-489">Добавлен параметр `--file-name / -f` для экспортируемых имен в `dns zone export`.</span><span class="sxs-lookup"><span data-stu-id="65a08-489">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="65a08-490">Исправлены следующие ошибки для `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="65a08-490">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="65a08-491">Исправлена проблема, когда длинные записи ТХТ неправильно экспортировались.</span><span class="sxs-lookup"><span data-stu-id="65a08-491">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="65a08-492">Исправлена проблема, когда записи ТХТ в кавычках неправильно экспортировались без символов экранирования.</span><span class="sxs-lookup"><span data-stu-id="65a08-492">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="65a08-493">Исправлена проблема, когда некоторые записи импортировались дважды с помощью `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="65a08-493">Fixed issue where certain records were imported twice with `dns zone import`</span></span> 
* <span data-ttu-id="65a08-494">Восстановлены команды `vnet-gateway root-cert` и `vnet-gateway revoked-cert`.</span><span class="sxs-lookup"><span data-stu-id="65a08-494">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="65a08-495">Профиль</span><span class="sxs-lookup"><span data-stu-id="65a08-495">Profile</span></span>

* <span data-ttu-id="65a08-496">Исправлена команда `get-access-token` для работы в виртуальной машине с идентификатором.</span><span class="sxs-lookup"><span data-stu-id="65a08-496">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="65a08-497">Ресурс</span><span class="sxs-lookup"><span data-stu-id="65a08-497">Resource</span></span>

* <span data-ttu-id="65a08-498">Исправлена ошибка с `deployment [create|validate]`, когда предупреждение неправильно отображалось, если поле type шаблона содержало значения в верхнем регистре.</span><span class="sxs-lookup"><span data-stu-id="65a08-498">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="65a08-499">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="65a08-499">Storage</span></span>

* <span data-ttu-id="65a08-500">Исправлена проблема с переносом учетных записей хранения из версии 1 в версию 2.</span><span class="sxs-lookup"><span data-stu-id="65a08-500">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="65a08-501">Добавлены отчеты о ходе выполнения всех команд отправки или скачивания.</span><span class="sxs-lookup"><span data-stu-id="65a08-501">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="65a08-502">Исправлена ошибка, которая препятствовала использованию параметра аргумента -n с `storage account check-name`.</span><span class="sxs-lookup"><span data-stu-id="65a08-502">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>  
* <span data-ttu-id="65a08-503">Добавлен столбец snapshot в табличные выходные данные для `blob [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="65a08-503">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="65a08-504">Исправлены ошибки с разными параметрами, которые должны были анализироваться как целые числа.</span><span class="sxs-lookup"><span data-stu-id="65a08-504">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="65a08-505">ВМ</span><span class="sxs-lookup"><span data-stu-id="65a08-505">VM</span></span>

* <span data-ttu-id="65a08-506">Добавлена команда `vm image accept-terms` для разрешения создания виртуальных машин из образов с дополнительными расходами.</span><span class="sxs-lookup"><span data-stu-id="65a08-506">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="65a08-507">Исправлена команда `[vm|vmss create]` для выполнения команд с прокси-сервера с помощью неподписанных сертификатов.</span><span class="sxs-lookup"><span data-stu-id="65a08-507">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="65a08-508">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка режима низкого приоритета для VMSS.</span><span class="sxs-lookup"><span data-stu-id="65a08-508">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="65a08-509">Добавлена защита `--admin-password` для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="65a08-509">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="65a08-510">17 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="65a08-510">January 17, 2018</span></span>

<span data-ttu-id="65a08-511">Версия 2.0.25</span><span class="sxs-lookup"><span data-stu-id="65a08-511">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="65a08-512">ACR</span><span class="sxs-lookup"><span data-stu-id="65a08-512">ACR</span></span>

* <span data-ttu-id="65a08-513">Добавлена возможность отката входа ACR при ошибках учетных данных в Windows.</span><span class="sxs-lookup"><span data-stu-id="65a08-513">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="65a08-514">Включены журналы реестра.</span><span class="sxs-lookup"><span data-stu-id="65a08-514">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="65a08-515">ACS</span><span class="sxs-lookup"><span data-stu-id="65a08-515">ACS</span></span>

* <span data-ttu-id="65a08-516">Исправлена команда `get-credentials`.</span><span class="sxs-lookup"><span data-stu-id="65a08-516">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="65a08-517">Удалено требование роли для имени субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="65a08-517">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="65a08-518">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="65a08-518">Appservice</span></span>

* <span data-ttu-id="65a08-519">Исправлена ошибка с `config ssl upload`, при которой значение `hosting_environment_profile` было NULL.</span><span class="sxs-lookup"><span data-stu-id="65a08-519">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="65a08-520">В `browse` добавлена поддержка для пользовательских URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="65a08-520">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="65a08-521">Исправлена поддержка слотов для `log tail`.</span><span class="sxs-lookup"><span data-stu-id="65a08-521">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="65a08-522">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="65a08-522">Backup</span></span>

* <span data-ttu-id="65a08-523">Параметр `--container-name` для `backup item list` теперь не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="65a08-523">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="65a08-524">В `backup restore restore-disks` добавлены варианты учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="65a08-524">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="65a08-525">Для проверки расположения в `backup protection enable-for-vm` добавлена чувствительность к регистру.</span><span class="sxs-lookup"><span data-stu-id="65a08-525">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="65a08-526">Устранена проблема, при которой команды завершались сбоем с указанием недопустимого имени контейнера.</span><span class="sxs-lookup"><span data-stu-id="65a08-526">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="65a08-527">В `backup item list` теперь по умолчанию включен параметр Health Status.</span><span class="sxs-lookup"><span data-stu-id="65a08-527">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="65a08-528">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="65a08-528">Batch</span></span>

* <span data-ttu-id="65a08-529">`batch login` теперь возвращает сведения об аутентификации.</span><span class="sxs-lookup"><span data-stu-id="65a08-529">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="65a08-530">Облако</span><span class="sxs-lookup"><span data-stu-id="65a08-530">Cloud</span></span>

* <span data-ttu-id="65a08-531">При установке `--profile` в облаке теперь не требуется указывать конечные точки.</span><span class="sxs-lookup"><span data-stu-id="65a08-531">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="65a08-532">Потребление</span><span class="sxs-lookup"><span data-stu-id="65a08-532">Consumption</span></span>

* <span data-ttu-id="65a08-533">Добавлены новые команды для резервирования: `consumption reservations summaries` и `consumption reservations details`.</span><span class="sxs-lookup"><span data-stu-id="65a08-533">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="65a08-534">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="65a08-534">Event Grid</span></span>

* <span data-ttu-id="65a08-535">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕИЕ] Команды `az eventgrid topic event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="65a08-535">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="65a08-536">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕИЕ] Команды `az eventgrid resource event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="65a08-536">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="65a08-537">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕИЕ] Удалена команда `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="65a08-537">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="65a08-538">Вместо нее следует использовать `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="65a08-538">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="65a08-539">Добавлена команда `eventgrid topic update`.</span><span class="sxs-lookup"><span data-stu-id="65a08-539">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="65a08-540">Добавлена команда `eventgrid event-subscription update`.</span><span class="sxs-lookup"><span data-stu-id="65a08-540">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="65a08-541">Добавлен параметр `--ids` для команд `eventgrid topic`.</span><span class="sxs-lookup"><span data-stu-id="65a08-541">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="65a08-542">Добавлена поддержка заполнения нажатием клавиши TAB для имен разделов.</span><span class="sxs-lookup"><span data-stu-id="65a08-542">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="65a08-543">Interactive</span><span class="sxs-lookup"><span data-stu-id="65a08-543">Interactive</span></span>

* <span data-ttu-id="65a08-544">Устранена проблема, при которой интерактивный режим не работал с Python 2.x.</span><span class="sxs-lookup"><span data-stu-id="65a08-544">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="65a08-545">Исправлены ошибки при запуске.</span><span class="sxs-lookup"><span data-stu-id="65a08-545">Fixed errors on startup</span></span>
* <span data-ttu-id="65a08-546">Устранена проблема, при которой некоторые команды не работали в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="65a08-546">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="65a08-547">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="65a08-547">IoT</span></span>

* <span data-ttu-id="65a08-548">Добавлена поддержка службы подготовки устройств.</span><span class="sxs-lookup"><span data-stu-id="65a08-548">Added support for device provisioning service</span></span>
* <span data-ttu-id="65a08-549">В команды и справочную информацию о них добавлены сообщения о нерекомендуемых версиях.</span><span class="sxs-lookup"><span data-stu-id="65a08-549">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="65a08-550">Теперь при проверке Интернета вещей указывается расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="65a08-550">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="65a08-551">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="65a08-551">Monitor</span></span>

* <span data-ttu-id="65a08-552">Добавлена поддержка параметра нескольких диагностических операций.</span><span class="sxs-lookup"><span data-stu-id="65a08-552">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="65a08-553">Теперь параметр `--name` является обязательным для `az monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="65a08-553">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="65a08-554">Добавлена команда `monitor diagnostic-settings categories` для получения категории параметров диагностики.</span><span class="sxs-lookup"><span data-stu-id="65a08-554">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="65a08-555">Сеть</span><span class="sxs-lookup"><span data-stu-id="65a08-555">Network</span></span>

* <span data-ttu-id="65a08-556">Устранена проблема с `vnet-gateway update` при попытке входа в активный режим и режим ожидания или выхода из них.</span><span class="sxs-lookup"><span data-stu-id="65a08-556">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="65a08-557">Для `application-gateway [create|update]` добавлена поддержка HTTP2.</span><span class="sxs-lookup"><span data-stu-id="65a08-557">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="65a08-558">Профиль</span><span class="sxs-lookup"><span data-stu-id="65a08-558">Profile</span></span>

* <span data-ttu-id="65a08-559">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="65a08-559">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="65a08-560">Роль</span><span class="sxs-lookup"><span data-stu-id="65a08-560">Role</span></span>

* <span data-ttu-id="65a08-561">В `role assignment create` добавлен аргумент `--assignee-object-id`, чтобы обойти запрос графов.</span><span class="sxs-lookup"><span data-stu-id="65a08-561">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="65a08-562">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="65a08-562">Service Fabric</span></span>

* <span data-ttu-id="65a08-563">В результат проверки при создании кластера добавлены подробные сведения об ошибках.</span><span class="sxs-lookup"><span data-stu-id="65a08-563">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="65a08-564">Устранена проблема отсутствия клиента при выполнении некоторых команд.</span><span class="sxs-lookup"><span data-stu-id="65a08-564">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="65a08-565">ВМ</span><span class="sxs-lookup"><span data-stu-id="65a08-565">VM</span></span>

* <span data-ttu-id="65a08-566">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Поддержка разных зон для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="65a08-566">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="65a08-567">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕИЕ] Значение по умолчанию `vmss` для одной зоны заменено данными подсистемы балансировки нагрузки уровня "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="65a08-567">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="65a08-568">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕИЕ] Для EMSI параметр `externalIdentities` изменен на `userAssignedIdentities`.</span><span class="sxs-lookup"><span data-stu-id="65a08-568">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="65a08-569">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка переключения дисков ОС.</span><span class="sxs-lookup"><span data-stu-id="65a08-569">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="65a08-570">Добавлена поддержка использования образов виртуальных машин из других подписок.</span><span class="sxs-lookup"><span data-stu-id="65a08-570">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="65a08-571">В `[vm|vmss] create` добавлены аргументы `--plan-name`, `--plan-product`, `--plan-promotion-code` и `--plan-publisher`.</span><span class="sxs-lookup"><span data-stu-id="65a08-571">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="65a08-572">Устранены проблемы с `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="65a08-572">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="65a08-573">Устранена проблема чрезмерного использования ресурсов из-за `vm image list --all`.</span><span class="sxs-lookup"><span data-stu-id="65a08-573">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="65a08-574">19 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="65a08-574">December 19, 2017</span></span>

<span data-ttu-id="65a08-575">Версия 2.0.23</span><span class="sxs-lookup"><span data-stu-id="65a08-575">Version 2.0.23</span></span>

* <span data-ttu-id="65a08-576">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="65a08-576">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="65a08-577">Контейнер</span><span class="sxs-lookup"><span data-stu-id="65a08-577">Container</span></span>

* <span data-ttu-id="65a08-578">Исправлен неправильный порядок параметров для журналов контейнеров.</span><span class="sxs-lookup"><span data-stu-id="65a08-578">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="65a08-579">Сеть</span><span class="sxs-lookup"><span data-stu-id="65a08-579">Network</span></span>

* <span data-ttu-id="65a08-580">Добавлен аргумент `--disable-bgp-route-propagation` для команды `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="65a08-580">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="65a08-581">Добавлен аргумент `--ip-tags` для команды `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="65a08-581">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="65a08-582">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="65a08-582">Storage</span></span>

* <span data-ttu-id="65a08-583">Добавлена поддержка хранилища версии 2.</span><span class="sxs-lookup"><span data-stu-id="65a08-583">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="65a08-584">ВМ</span><span class="sxs-lookup"><span data-stu-id="65a08-584">VM</span></span>

* <span data-ttu-id="65a08-585">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для назначенных пользователям удостоверений для виртуальных машин и VMSS.</span><span class="sxs-lookup"><span data-stu-id="65a08-585">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="65a08-586">5 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="65a08-586">December 5, 2017</span></span>

<span data-ttu-id="65a08-587">Версия 2.0.22</span><span class="sxs-lookup"><span data-stu-id="65a08-587">Version 2.0.22</span></span>

* <span data-ttu-id="65a08-588">Удалена команда `az component`.</span><span class="sxs-lookup"><span data-stu-id="65a08-588">Removed `az component` commands.</span></span> <span data-ttu-id="65a08-589">Вместо нее следует использовать `az extension`.</span><span class="sxs-lookup"><span data-stu-id="65a08-589">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="65a08-590">Core</span><span class="sxs-lookup"><span data-stu-id="65a08-590">Core</span></span>
* <span data-ttu-id="65a08-591">Конечная точка `AZURE_US_GOV_CLOUD` центра AAD изменена с login.microsoftonline.com на login.microsoftonline.us.</span><span class="sxs-lookup"><span data-stu-id="65a08-591">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="65a08-592">Исправлена проблема с непрерывной отправкой телеметрии.</span><span class="sxs-lookup"><span data-stu-id="65a08-592">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="65a08-593">ACS</span><span class="sxs-lookup"><span data-stu-id="65a08-593">ACS</span></span>

* <span data-ttu-id="65a08-594">Добавлены команды `aks install-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="65a08-594">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="65a08-595">Улучшены сообщения об ошибках для команды `acs create`.</span><span class="sxs-lookup"><span data-stu-id="65a08-595">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="65a08-596">Добавлена возможность использования команды `aks get-credentials -f` без полного пути.</span><span class="sxs-lookup"><span data-stu-id="65a08-596">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="65a08-597">Помощник</span><span class="sxs-lookup"><span data-stu-id="65a08-597">Advisor</span></span>

* <span data-ttu-id="65a08-598">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="65a08-598">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="65a08-599">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="65a08-599">Appservice</span></span>

* <span data-ttu-id="65a08-600">Добавлена возможность создания имени сертификата с помощью команды `webapp config ssl upload`.</span><span class="sxs-lookup"><span data-stu-id="65a08-600">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="65a08-601">Исправлены команды `webapp [list|show]` и `functionapp [list|show]` для отображения правильных приложений.</span><span class="sxs-lookup"><span data-stu-id="65a08-601">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="65a08-602">Добавлено стандартное значение для переменной `WEBSITE_NODE_DEFAULT_VERSION`.</span><span class="sxs-lookup"><span data-stu-id="65a08-602">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="65a08-603">Потребление</span><span class="sxs-lookup"><span data-stu-id="65a08-603">Consumption</span></span>

* <span data-ttu-id="65a08-604">Добавлена поддержка API версии 2017-11-30.</span><span class="sxs-lookup"><span data-stu-id="65a08-604">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="65a08-605">Контейнер</span><span class="sxs-lookup"><span data-stu-id="65a08-605">Container</span></span>

* <span data-ttu-id="65a08-606">Исправлены стандартные порты регрессии.</span><span class="sxs-lookup"><span data-stu-id="65a08-606">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="65a08-607">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="65a08-607">Monitor</span></span>

* <span data-ttu-id="65a08-608">Добавлена поддержка нескольких измерений для команд метрик.</span><span class="sxs-lookup"><span data-stu-id="65a08-608">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="65a08-609">Ресурс</span><span class="sxs-lookup"><span data-stu-id="65a08-609">Resource</span></span>

* <span data-ttu-id="65a08-610">Добавлен аргумент `--include-response-body` для команды `resource show`</span><span class="sxs-lookup"><span data-stu-id="65a08-610">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="65a08-611">Роль</span><span class="sxs-lookup"><span data-stu-id="65a08-611">Role</span></span>

* <span data-ttu-id="65a08-612">Добавлено отображение стандартных назначений "классических" администраторов для команды `role assignment list`.</span><span class="sxs-lookup"><span data-stu-id="65a08-612">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="65a08-613">Добавлена поддержка команды `ad sp reset-credentials` для добавления учетных данных вместо перезаписи.</span><span class="sxs-lookup"><span data-stu-id="65a08-613">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="65a08-614">Улучшены сообщения об ошибках для команды `ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="65a08-614">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="65a08-615">SQL</span><span class="sxs-lookup"><span data-stu-id="65a08-615">SQL</span></span>

* <span data-ttu-id="65a08-616">Добавлены команды `sql db list-usages` и `sql db show-usage`.</span><span class="sxs-lookup"><span data-stu-id="65a08-616">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="65a08-617">Добавлены команды `sql server conn-policy show` и `sql server conn-policy update`.</span><span class="sxs-lookup"><span data-stu-id="65a08-617">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="65a08-618">ВМ</span><span class="sxs-lookup"><span data-stu-id="65a08-618">VM</span></span>

* <span data-ttu-id="65a08-619">Добавлены сведения о зонах для команды `az vm list-skus`.</span><span class="sxs-lookup"><span data-stu-id="65a08-619">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="65a08-620">14 ноября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="65a08-620">November 14, 2017</span></span>

<span data-ttu-id="65a08-621">Версия 2.0.21</span><span class="sxs-lookup"><span data-stu-id="65a08-621">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="65a08-622">ACR</span><span class="sxs-lookup"><span data-stu-id="65a08-622">ACR</span></span>

* <span data-ttu-id="65a08-623">Добавлена поддержка создания веб-перехватчиков в регионах репликации.</span><span class="sxs-lookup"><span data-stu-id="65a08-623">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="65a08-624">ACS</span><span class="sxs-lookup"><span data-stu-id="65a08-624">ACS</span></span>

* <span data-ttu-id="65a08-625">В AKS агент теперь называется узлом.</span><span class="sxs-lookup"><span data-stu-id="65a08-625">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="65a08-626">Параметр `--orchestrator-release` для командлета `acs create` не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="65a08-626">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="65a08-627">Изменен размер виртуальной машины для AKS по умолчанию на `Standard_D1_v2`.</span><span class="sxs-lookup"><span data-stu-id="65a08-627">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="65a08-628">Исправлена команда `az aks browse` для Windows.</span><span class="sxs-lookup"><span data-stu-id="65a08-628">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="65a08-629">Исправлена команда `az aks get-credentials` для Windows.</span><span class="sxs-lookup"><span data-stu-id="65a08-629">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="65a08-630">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="65a08-630">Appservice</span></span>

* <span data-ttu-id="65a08-631">Добавлен источник развертывания `config-zip` для веб-приложений и приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="65a08-631">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="65a08-632">Добавлен параметр `--docker-container-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="65a08-632">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="65a08-633">Удален параметр `storage` из параметра `--web-server-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="65a08-633">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="65a08-634">Улучшены сообщения об ошибках для команды `deployment user set`.</span><span class="sxs-lookup"><span data-stu-id="65a08-634">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="65a08-635">Добавлена поддержка создания приложений-функций Linux</span><span class="sxs-lookup"><span data-stu-id="65a08-635">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="65a08-636">Фиксированное значение `list-locations`</span><span class="sxs-lookup"><span data-stu-id="65a08-636">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="65a08-637">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="65a08-637">Batch</span></span>

* <span data-ttu-id="65a08-638">Исправлена ошибка в команде создания пула, когда идентификатор ресурса использовался с флагом `--image`.</span><span class="sxs-lookup"><span data-stu-id="65a08-638">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="65a08-639">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="65a08-639">Batchai</span></span>

* <span data-ttu-id="65a08-640">Добавлен короткий параметр `-s` для параметра `--vm-size` при указании размера виртуальной машины в команде `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="65a08-640">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="65a08-641">Добавлены аргументы ключа и имени учетной записи хранения в параметры команды `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="65a08-641">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="65a08-642">Исправлена документация по командам `job list-files` и `job stream-file`.</span><span class="sxs-lookup"><span data-stu-id="65a08-642">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="65a08-643">Добавлен короткий параметр `-r` для параметра `--cluster-name` при указании имени кластера в команде `job create`.</span><span class="sxs-lookup"><span data-stu-id="65a08-643">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="65a08-644">Облако</span><span class="sxs-lookup"><span data-stu-id="65a08-644">Cloud</span></span>

* <span data-ttu-id="65a08-645">Изменена команда `cloud [register|update]` для предотвращения регистрации облаков, для которых отсутствуют необходимые конечные точки.</span><span class="sxs-lookup"><span data-stu-id="65a08-645">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="65a08-646">Контейнер</span><span class="sxs-lookup"><span data-stu-id="65a08-646">Container</span></span>

* <span data-ttu-id="65a08-647">Добавлена поддержка открытия нескольких портов.</span><span class="sxs-lookup"><span data-stu-id="65a08-647">Added support to open multiple ports</span></span>
* <span data-ttu-id="65a08-648">Добавлена политика перезапуска группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="65a08-648">Added container group restart policy</span></span>
* <span data-ttu-id="65a08-649">Добавлена поддержка подключения файлового ресурса Azure в качестве тома.</span><span class="sxs-lookup"><span data-stu-id="65a08-649">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="65a08-650">Обновлена вспомогательная документация.</span><span class="sxs-lookup"><span data-stu-id="65a08-650">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="65a08-651">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="65a08-651">Data Lake Analytics</span></span>

* <span data-ttu-id="65a08-652">Изменена команда `[job|account] list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="65a08-652">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="65a08-653">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="65a08-653">Data Lake Store</span></span>

* <span data-ttu-id="65a08-654">Изменена команда `account list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="65a08-654">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="65a08-655">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="65a08-655">Extension</span></span>

* <span data-ttu-id="65a08-656">Добавлена команда `extension list-available` для отображения официальных расширений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="65a08-656">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="65a08-657">Добавлен параметр `--name` для команды `extension [add|update]` для установки расширений по имени.</span><span class="sxs-lookup"><span data-stu-id="65a08-657">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="65a08-658">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="65a08-658">IoT</span></span>

* <span data-ttu-id="65a08-659">Добавлена поддержка центров сертификации (ЦС) и цепочек сертификатов.</span><span class="sxs-lookup"><span data-stu-id="65a08-659">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="65a08-660">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="65a08-660">Monitor</span></span>

* <span data-ttu-id="65a08-661">Добавлены команды `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="65a08-661">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="65a08-662">Сеть</span><span class="sxs-lookup"><span data-stu-id="65a08-662">Network</span></span>

* <span data-ttu-id="65a08-663">Добавлена поддержка DNS-записей типа CAA.</span><span class="sxs-lookup"><span data-stu-id="65a08-663">Added support for CAA DNS records</span></span>
* <span data-ttu-id="65a08-664">Исправлена проблема, когда конечные точки могли не обновляться с помощью команды `traffic-manager profile update`.</span><span class="sxs-lookup"><span data-stu-id="65a08-664">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="65a08-665">Исправлена проблема, когда команда `vnet update --dns-servers` не работала в зависимости от способа создания виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="65a08-665">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="65a08-666">Исправлена проблема, когда относительные DNS-имена неправильно импортировались с помощью команды `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="65a08-666">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="65a08-667">Резервирование</span><span class="sxs-lookup"><span data-stu-id="65a08-667">Reservations</span></span>

* <span data-ttu-id="65a08-668">Первоначальный выпуск предварительной версии</span><span class="sxs-lookup"><span data-stu-id="65a08-668">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="65a08-669">Ресурс</span><span class="sxs-lookup"><span data-stu-id="65a08-669">Resource</span></span>

* <span data-ttu-id="65a08-670">Добавлена поддержка идентификаторов ресурсов для блокировок на уровне ресурсов и параметра `--resource`.</span><span class="sxs-lookup"><span data-stu-id="65a08-670">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="65a08-671">SQL</span><span class="sxs-lookup"><span data-stu-id="65a08-671">SQL</span></span>

* <span data-ttu-id="65a08-672">Добавлен параметр `--ignore-missing-vnet-service-endpoint` для команды `sql server vnet-rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="65a08-672">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="65a08-673">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="65a08-673">Storage</span></span>

* <span data-ttu-id="65a08-674">Изменена команда `storage account create` для использования номера SKU `Standard_RAGRS` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="65a08-674">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="65a08-675">Исправлены ошибки при обработке имени файла или большого двоичного объекта, содержащего символы, отличные от ASCII.</span><span class="sxs-lookup"><span data-stu-id="65a08-675">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="65a08-676">Исправлена ошибка, препятствующая использованию параметра `--source-uri` с командой `storage [blob|file] copy start-batch`.</span><span class="sxs-lookup"><span data-stu-id="65a08-676">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="65a08-677">Добавлены команды для удаления нескольких объектов с помощью команды `storage [blob|file] delete-batch`.</span><span class="sxs-lookup"><span data-stu-id="65a08-677">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="65a08-678">Исправлена проблема с включением метрик с помощью команды `storage metrics update`.</span><span class="sxs-lookup"><span data-stu-id="65a08-678">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="65a08-679">Исправлена проблема с файлами более 200 ГБ при использовании команды `storage blob upload-batch`.</span><span class="sxs-lookup"><span data-stu-id="65a08-679">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="65a08-680">Исправлена проблема, когда параметры `--bypass` и `--default-action` игнорировались командой `storage account [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="65a08-680">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="65a08-681">ВМ</span><span class="sxs-lookup"><span data-stu-id="65a08-681">VM</span></span>

* <span data-ttu-id="65a08-682">Исправлена ошибка с командой `vmss create`, препятствующая использованию уровня `Basic`.</span><span class="sxs-lookup"><span data-stu-id="65a08-682">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="65a08-683">Добавлены аргументы `--plan` для команды `[vm|vmss] create` для пользовательских образов с информацией о выставлении счетов.</span><span class="sxs-lookup"><span data-stu-id="65a08-683">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="65a08-684">Добавлены команды `vm secret `[add|remove|list]\`.</span><span class="sxs-lookup"><span data-stu-id="65a08-684">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="65a08-685">Команда `vm format-secret` переименована в `vm secret format`.</span><span class="sxs-lookup"><span data-stu-id="65a08-685">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="65a08-686">Добавлен аргумент `--encrypt format` для команды `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="65a08-686">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="65a08-687">24 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="65a08-687">October 24, 2017</span></span>

<span data-ttu-id="65a08-688">Версия 2.0.20</span><span class="sxs-lookup"><span data-stu-id="65a08-688">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="65a08-689">Core</span><span class="sxs-lookup"><span data-stu-id="65a08-689">Core</span></span>

* <span data-ttu-id="65a08-690">Обновление `2017-03-09-profile` для использования API `MGMT_STORAGE` версии `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="65a08-690">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="65a08-691">ACR</span><span class="sxs-lookup"><span data-stu-id="65a08-691">ACR</span></span>

* <span data-ttu-id="65a08-692">Обновление службы управления ресурсами для указания API версии `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="65a08-692">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="65a08-693">Изменение номера SKU BYOS-хранилища на "Классический"</span><span class="sxs-lookup"><span data-stu-id="65a08-693">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="65a08-694">Переименование номеров SKU реестра на "Базовый", "Стандартный" и "Премиум"</span><span class="sxs-lookup"><span data-stu-id="65a08-694">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="65a08-695">ACS</span><span class="sxs-lookup"><span data-stu-id="65a08-695">ACS</span></span>

* <span data-ttu-id="65a08-696">[ПРЕДВАРИЕТЛЬНАЯ ВЕРСИЯ] Добавление команд `az aks`</span><span class="sxs-lookup"><span data-stu-id="65a08-696">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="65a08-697">Исправление Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="65a08-697">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="65a08-698">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="65a08-698">Appservice</span></span>

* <span data-ttu-id="65a08-699">Исправление проблемы с недопустимыми скачанными журналами `webapp`</span><span class="sxs-lookup"><span data-stu-id="65a08-699">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="65a08-700">Компонент</span><span class="sxs-lookup"><span data-stu-id="65a08-700">Component</span></span>

* <span data-ttu-id="65a08-701">Добавление более понятного сообщения об устаревании для всех установщиков, а также запроса на подтверждение</span><span class="sxs-lookup"><span data-stu-id="65a08-701">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="65a08-702">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="65a08-702">Monitor</span></span>

* <span data-ttu-id="65a08-703">Добавлены команды `action-group`.</span><span class="sxs-lookup"><span data-stu-id="65a08-703">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="65a08-704">Ресурс</span><span class="sxs-lookup"><span data-stu-id="65a08-704">Resource</span></span>

* <span data-ttu-id="65a08-705">Исправление несовместимости с самой последней версии зависимости msrest в `group export`</span><span class="sxs-lookup"><span data-stu-id="65a08-705">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="65a08-706">Исправление `policy assignment create` для работы с определениями встроенных политик и наборов политик</span><span class="sxs-lookup"><span data-stu-id="65a08-706">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="65a08-707">ВМ</span><span class="sxs-lookup"><span data-stu-id="65a08-707">VM</span></span>

* <span data-ttu-id="65a08-708">Добавлен аргумент `--accelerated-networking` для команды `vmss create`</span><span class="sxs-lookup"><span data-stu-id="65a08-708">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="65a08-709">9 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="65a08-709">October 9, 2017</span></span>

<span data-ttu-id="65a08-710">Версия 2.0.19</span><span class="sxs-lookup"><span data-stu-id="65a08-710">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="65a08-711">Core</span><span class="sxs-lookup"><span data-stu-id="65a08-711">Core</span></span>

* <span data-ttu-id="65a08-712">В Azure Stack добавлена обработка URL-адресов центра ADFS с завершающей косой чертой.</span><span class="sxs-lookup"><span data-stu-id="65a08-712">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="65a08-713">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="65a08-713">Appservice</span></span>

* <span data-ttu-id="65a08-714">Добавлена возможность общего обновления с помощью новой команды `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="65a08-714">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="65a08-715">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="65a08-715">Batch</span></span>

* <span data-ttu-id="65a08-716">Обновление до пакета SDK для пакетной службы версии 4.0.0</span><span class="sxs-lookup"><span data-stu-id="65a08-716">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="65a08-717">Обновлен параметр `--image` для команды VirtualMachineConfiguration, обеспечивающий поддержку ссылок на образы ARM в дополнение к publish:offer:sku:version.</span><span class="sxs-lookup"><span data-stu-id="65a08-717">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="65a08-718">Добавлена поддержка новой модели расширений CLI для команд расширений пакетной службы.</span><span class="sxs-lookup"><span data-stu-id="65a08-718">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="65a08-719">Удалена поддержка пакетной службы для модели компонентов.</span><span class="sxs-lookup"><span data-stu-id="65a08-719">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="65a08-720">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="65a08-720">Batchai</span></span>

* <span data-ttu-id="65a08-721">Исходный выпуск модуля искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="65a08-721">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="65a08-722">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="65a08-722">Keyvault</span></span>

* <span data-ttu-id="65a08-723">Исправлена проблема с аутентификацией Key Vault при использовании ADFS в Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="65a08-723">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="65a08-724">(#4448)</span><span class="sxs-lookup"><span data-stu-id="65a08-724">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="65a08-725">Сеть</span><span class="sxs-lookup"><span data-stu-id="65a08-725">Network</span></span>

* <span data-ttu-id="65a08-726">Аргумент `--server` для `application-gateway address-pool create` изменен на необязательный (разрешено использование пустых пулов адресов).</span><span class="sxs-lookup"><span data-stu-id="65a08-726">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="65a08-727">Обновлен элемент `traffic-manager` для поддержки последних функций.</span><span class="sxs-lookup"><span data-stu-id="65a08-727">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="65a08-728">Ресурс</span><span class="sxs-lookup"><span data-stu-id="65a08-728">Resource</span></span>

* <span data-ttu-id="65a08-729">Добавлена поддержка параметров `--resource-group/-g` для изменения имени группы ресурсов на `group`.</span><span class="sxs-lookup"><span data-stu-id="65a08-729">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="65a08-730">Добавлены команды для `account lock` для работы с блокировками на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="65a08-730">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="65a08-731">Добавлены команды для `group lock` для работы с блокировками на уровне группы.</span><span class="sxs-lookup"><span data-stu-id="65a08-731">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="65a08-732">Добавлены команды для `resource lock` для работы с блокировками на уровне ресурса.</span><span class="sxs-lookup"><span data-stu-id="65a08-732">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="65a08-733">SQL</span><span class="sxs-lookup"><span data-stu-id="65a08-733">Sql</span></span>

* <span data-ttu-id="65a08-734">Добавлена поддержка SQL TDE и BYOK TDE.</span><span class="sxs-lookup"><span data-stu-id="65a08-734">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="65a08-735">Добавлена команда `db list-deleted` и параметр `db restore --deleted-time` для поиска и восстановления удаленных баз данных.</span><span class="sxs-lookup"><span data-stu-id="65a08-735">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="65a08-736">Добавлено `db op list` и `db op cancel` для отображения и отмены выполняющихся операций в базе данных.</span><span class="sxs-lookup"><span data-stu-id="65a08-736">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="65a08-737">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="65a08-737">Storage</span></span>

* <span data-ttu-id="65a08-738">Добавлена поддержка моментальных снимков файловых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="65a08-738">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="65a08-739">Виртуальные машины</span><span class="sxs-lookup"><span data-stu-id="65a08-739">Vm</span></span>

* <span data-ttu-id="65a08-740">Исправлена ошибка в команде `vm show`, когда использование `-d` вызывало сбой отсутствующих частных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="65a08-740">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="65a08-741">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка последовательного обновления для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="65a08-741">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="65a08-742">Добавлена поддержка обновления параметров шифрования с помощью команды `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="65a08-742">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="65a08-743">Добавлен параметр `--os-disk-size-gb` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="65a08-743">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="65a08-744">Добавлен параметр `--license-type` для команды `vmss create` (для Windows).</span><span class="sxs-lookup"><span data-stu-id="65a08-744">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="65a08-745">22 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="65a08-745">September 22, 2017</span></span>

<span data-ttu-id="65a08-746">Версия 2.0.18</span><span class="sxs-lookup"><span data-stu-id="65a08-746">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="65a08-747">Ресурс</span><span class="sxs-lookup"><span data-stu-id="65a08-747">Resource</span></span>

* <span data-ttu-id="65a08-748">Добавлена поддержка отображения определений встроенных политик</span><span class="sxs-lookup"><span data-stu-id="65a08-748">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="65a08-749">Добавлена поддержка параметра mode для создания определения политик</span><span class="sxs-lookup"><span data-stu-id="65a08-749">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="65a08-750">Добавлена поддержка шаблонов и определений пользовательского интерфейса для команды `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="65a08-750">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="65a08-751">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕИЕ] Изменен тип ресурса `managedapp` с `appliances` на `applications` и с `applianceDefinitions` на `applicationDefinitions`.</span><span class="sxs-lookup"><span data-stu-id="65a08-751">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="65a08-752">Сеть</span><span class="sxs-lookup"><span data-stu-id="65a08-752">Network</span></span>

* <span data-ttu-id="65a08-753">Добавлена поддержка зоны доступности для подкоманд `network lb` и `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="65a08-753">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="65a08-754">Добавлена поддержка IPv6 (пиринг Майкрософт) для `express-route`</span><span class="sxs-lookup"><span data-stu-id="65a08-754">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="65a08-755">Добавлены команды группы безопасности приложения `asg`</span><span class="sxs-lookup"><span data-stu-id="65a08-755">Added `asg` application security group commands</span></span>
* <span data-ttu-id="65a08-756">Добавлен аргумент `--application-security-groups` для команды `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="65a08-756">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="65a08-757">Добавлены аргументы `--source-asgs` и `--destination-asgs` для команды `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="65a08-757">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="65a08-758">Добавлены аргументы `--ddos-protection` и `--vm-protection` для команды `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="65a08-758">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="65a08-759">Добавлены команды `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="65a08-759">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="65a08-760">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="65a08-760">Storage</span></span>

* <span data-ttu-id="65a08-761">Исправлена проблема, когда команды `storage account network-rule` могут не работать после обновления пакета SDK</span><span class="sxs-lookup"><span data-stu-id="65a08-761">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="65a08-762">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="65a08-762">Eventgrid</span></span>

* <span data-ttu-id="65a08-763">Обновлен пакет SDK Python для службы "Сетка событий Azure" для использования новой версии API 2017-09-15-preview</span><span class="sxs-lookup"><span data-stu-id="65a08-763">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="65a08-764">SQL</span><span class="sxs-lookup"><span data-stu-id="65a08-764">SQL</span></span>

* <span data-ttu-id="65a08-765">Аргумент `--resource-group` для команды `sql server list` сделан необязательным.</span><span class="sxs-lookup"><span data-stu-id="65a08-765">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="65a08-766">Если он не указан, возвращаются все серверы SQL Server в подписке</span><span class="sxs-lookup"><span data-stu-id="65a08-766">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="65a08-767">Добавлен параметр `--no-wait` для команд `db [create|copy|restore|update|replica create|create|update]` и `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="65a08-767">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="65a08-768">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="65a08-768">Keyvault</span></span>

* <span data-ttu-id="65a08-769">Добавлена поддержка команд хранилища ключей за прокси-сервером</span><span class="sxs-lookup"><span data-stu-id="65a08-769">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="65a08-770">ВМ</span><span class="sxs-lookup"><span data-stu-id="65a08-770">VM</span></span>

* <span data-ttu-id="65a08-771">Добавлена поддержка зоны доступности для команды `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="65a08-771">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="65a08-772">Исправлена проблема, когда использование аргумента `--app-gateway ID` с командой `vmss create` приводило к сбою</span><span class="sxs-lookup"><span data-stu-id="65a08-772">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="65a08-773">Добавлен аргумент `--asgs` для команды `vm create`</span><span class="sxs-lookup"><span data-stu-id="65a08-773">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="65a08-774">Добавлена поддержка выполнения команд на виртуальных машинах с помощью команды `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="65a08-774">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="65a08-775">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка шифрования диска VMSS с помощью команды `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="65a08-775">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="65a08-776">Добавлена поддержка обслуживания виртуальных машин с помощью команды `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="65a08-776">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="65a08-777">ACS</span><span class="sxs-lookup"><span data-stu-id="65a08-777">ACS</span></span>

* <span data-ttu-id="65a08-778">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлен аргумент `--orchestrator-release` для команды `acs create` для регионов служб ACS (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="65a08-778">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="65a08-779">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="65a08-779">Appservice</span></span>

* <span data-ttu-id="65a08-780">Добавлена возможность обновлять и отображать параметры аутентификации с помощью команды `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="65a08-780">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="65a08-781">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="65a08-781">Backup</span></span>

* <span data-ttu-id="65a08-782">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="65a08-782">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="65a08-783">11 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="65a08-783">September 11, 2017</span></span>

<span data-ttu-id="65a08-784">Версия 2.0.17</span><span class="sxs-lookup"><span data-stu-id="65a08-784">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="65a08-785">Core</span><span class="sxs-lookup"><span data-stu-id="65a08-785">Core</span></span>

* <span data-ttu-id="65a08-786">Включен командный модуль для настройки собственного идентификатора корреляции в телеметрии.</span><span class="sxs-lookup"><span data-stu-id="65a08-786">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="65a08-787">Исправлена проблема с дампом JSON, когда для телеметрии настроен режим диагностики.</span><span class="sxs-lookup"><span data-stu-id="65a08-787">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="65a08-788">ACS</span><span class="sxs-lookup"><span data-stu-id="65a08-788">Acs</span></span>

* <span data-ttu-id="65a08-789">Добавлена команда `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="65a08-789">Added `acs list-locations` command</span></span>
* <span data-ttu-id="65a08-790">Для `ssh-key-file` предоставляется ожидаемое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="65a08-790">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="65a08-791">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="65a08-791">Appservice</span></span>

* <span data-ttu-id="65a08-792">Добавлена возможность создавать веб-приложения в группе ресурсов в рамках плана службы, отличной от активной.</span><span class="sxs-lookup"><span data-stu-id="65a08-792">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="65a08-793">CDN</span><span class="sxs-lookup"><span data-stu-id="65a08-793">CDN</span></span>

* <span data-ttu-id="65a08-794">Исправлена ошибка "CustomDomain не пригоден к итерации" для `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="65a08-794">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="65a08-795">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="65a08-795">Extension</span></span>

* <span data-ttu-id="65a08-796">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="65a08-796">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="65a08-797">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="65a08-797">Keyvault</span></span>

* <span data-ttu-id="65a08-798">Исправлена проблема с зависимостью разрешений от регистра для `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="65a08-798">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="65a08-799">Сеть</span><span class="sxs-lookup"><span data-stu-id="65a08-799">Network</span></span>

* <span data-ttu-id="65a08-800">Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="65a08-800">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="65a08-801">Аргумент `--private-access-services` переименован в `--service-endpoints` для команды `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="65a08-801">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="65a08-802">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="65a08-802">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="65a08-803">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="65a08-803">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="65a08-804">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="65a08-804">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="65a08-805">Ресурс</span><span class="sxs-lookup"><span data-stu-id="65a08-805">Resource</span></span>

* <span data-ttu-id="65a08-806">Разрешена передача в определениях параметров политики ресурсов в командах `policy definition create` и `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="65a08-806">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="65a08-807">Разрешена передача значений параметров для команды `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="65a08-807">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="65a08-808">Разрешена передача JSON или файла для всех параметров.</span><span class="sxs-lookup"><span data-stu-id="65a08-808">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="65a08-809">Версия API изменена на более позднюю.</span><span class="sxs-lookup"><span data-stu-id="65a08-809">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="65a08-810">SQL</span><span class="sxs-lookup"><span data-stu-id="65a08-810">SQL</span></span>

* <span data-ttu-id="65a08-811">Добавлены команды `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="65a08-811">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="65a08-812">ВМ</span><span class="sxs-lookup"><span data-stu-id="65a08-812">VM</span></span>

* <span data-ttu-id="65a08-813">Исправлено: не назначать доступ, если `--scope` не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="65a08-813">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="65a08-814">Исправлено: использование тех же расширений имен, что и для портала.</span><span class="sxs-lookup"><span data-stu-id="65a08-814">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="65a08-815">Удалено `subscription` из выходных данных `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="65a08-815">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="65a08-816">Исправлено: номер SKU хранилища `[vm|vmss] create` неприменим для дисков данных с образом.</span><span class="sxs-lookup"><span data-stu-id="65a08-816">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="65a08-817">Исправлено: `vm format-secret --secrets` не принимает идентификаторы, разделенные строками.</span><span class="sxs-lookup"><span data-stu-id="65a08-817">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="65a08-818">31 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="65a08-818">August 31, 2017</span></span>

<span data-ttu-id="65a08-819">Версия 2.0.16</span><span class="sxs-lookup"><span data-stu-id="65a08-819">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="65a08-820">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="65a08-820">Keyvault</span></span>

* <span data-ttu-id="65a08-821">Исправлена ошибка при попытке автоматически разрешить шифрование секрета с помощью `secret download`.</span><span class="sxs-lookup"><span data-stu-id="65a08-821">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="65a08-822">Sf</span><span class="sxs-lookup"><span data-stu-id="65a08-822">Sf</span></span>

* <span data-ttu-id="65a08-823">Объявлены неподдерживаемыми все команды; вместо них используется Service Fabric CLI (sfctl).</span><span class="sxs-lookup"><span data-stu-id="65a08-823">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="65a08-824">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="65a08-824">Storage</span></span>

* <span data-ttu-id="65a08-825">Исправлена проблема, когда учетные записи хранения нельзя было создавать в регионах, которые не поддерживают функцию NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="65a08-825">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="65a08-826">Определение типа и кодировки содержимого во время передачи больших двоичных объектов и файла, если оба свойства не указаны.</span><span class="sxs-lookup"><span data-stu-id="65a08-826">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="65a08-827">28 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="65a08-827">August 28, 2017</span></span>

<span data-ttu-id="65a08-828">Версия 2.0.15</span><span class="sxs-lookup"><span data-stu-id="65a08-828">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="65a08-829">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="65a08-829">CLI</span></span>

* <span data-ttu-id="65a08-830">Для `--version` добавлено юридическое примечание.</span><span class="sxs-lookup"><span data-stu-id="65a08-830">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="65a08-831">ACS</span><span class="sxs-lookup"><span data-stu-id="65a08-831">ACS</span></span>

* <span data-ttu-id="65a08-832">Исправлены регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="65a08-832">Corrected preview regions</span></span>
* <span data-ttu-id="65a08-833">Правильно отформатирован параметр по умолчанию `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="65a08-833">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="65a08-834">Оптимизированы выходные данные команды ACS.</span><span class="sxs-lookup"><span data-stu-id="65a08-834">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="65a08-835">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="65a08-835">Appservice</span></span>

* <span data-ttu-id="65a08-836">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕИЕ] Исправлены несоответствия в выходных данных `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="65a08-836">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="65a08-837">Добавлен новый псевдоним `-i` в команду `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="65a08-837">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="65a08-838">Предоставлена команда `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="65a08-838">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="65a08-839">Предоставлены новые аргументы команды `az webapp delete`, которые позволяют сохранить план службы приложений, метрики и данные регистрации DNS.</span><span class="sxs-lookup"><span data-stu-id="65a08-839">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="65a08-840">Исправление. Параметры слота определяются правильно.</span><span class="sxs-lookup"><span data-stu-id="65a08-840">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="65a08-841">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="65a08-841">IoT</span></span>

* <span data-ttu-id="65a08-842">Исправление 3934. При создании политики существующие политики больше не удаляются.</span><span class="sxs-lookup"><span data-stu-id="65a08-842">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="65a08-843">Сеть</span><span class="sxs-lookup"><span data-stu-id="65a08-843">Network</span></span>

* <span data-ttu-id="65a08-844">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕИЕ] Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="65a08-844">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="65a08-845">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕИЕ] Параметр `--private-access-services` переименован в `--service-endpoints` в командах `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="65a08-845">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="65a08-846">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="65a08-846">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="65a08-847">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="65a08-847">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="65a08-848">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="65a08-848">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="65a08-849">Профиль</span><span class="sxs-lookup"><span data-stu-id="65a08-849">Profile</span></span>

* <span data-ttu-id="65a08-850">Предоставлены параметры `--msi` и `--msi-port` для входа с использованием удостоверения виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="65a08-850">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="65a08-851">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="65a08-851">Service Fabric</span></span>

* <span data-ttu-id="65a08-852">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="65a08-852">Preview release</span></span>
* <span data-ttu-id="65a08-853">Упрощены правила реестра для паролей и имен пользователя для команды.</span><span class="sxs-lookup"><span data-stu-id="65a08-853">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="65a08-854">Исправлена строка для ввода пароля пользователем даже после передачи параметра.</span><span class="sxs-lookup"><span data-stu-id="65a08-854">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="65a08-855">Добавлена поддержка пустого значения `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="65a08-855">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="65a08-856">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="65a08-856">Storage</span></span>

* <span data-ttu-id="65a08-857">Появилась возможность задавать уровень большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="65a08-857">Enabled setting blob tier</span></span>
* <span data-ttu-id="65a08-858">Добавлены аргументы `--bypass` и `--default-action` в командах `storage account [create|update]` для поддержки туннелирования службы.</span><span class="sxs-lookup"><span data-stu-id="65a08-858">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="65a08-859">Добавлены команды для добавления правил виртуальной сети и правил на основе IP-адресов в `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="65a08-859">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="65a08-860">Разрешено шифрование службы с управляемым пользователем ключом.</span><span class="sxs-lookup"><span data-stu-id="65a08-860">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="65a08-861">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕИЕ] Параметр `--encryption` переименован в `--encryption-services` в команде `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="65a08-861">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="65a08-862">Исправление 4220. Несоответствие синтаксиса `az storage account update encryption`.</span><span class="sxs-lookup"><span data-stu-id="65a08-862">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="65a08-863">ВМ</span><span class="sxs-lookup"><span data-stu-id="65a08-863">VM</span></span>

* <span data-ttu-id="65a08-864">Исправлена проблема, из-за которой для команды `vmss get-instance-view` отображались лишние и неправильные сведения при использовании параметра `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="65a08-864">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="65a08-865">Добавлена поддержка параметра `--lb-sku` в команде `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="65a08-865">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="65a08-866">Из черного списка имен администраторов для команд `[vm|vmss] create` удалены имена людей.</span><span class="sxs-lookup"><span data-stu-id="65a08-866">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="65a08-867">Исправлена проблема, из-за которой команда `[vm|vmss] create` выдавала ошибку, если из образа не удавалось извлечь сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="65a08-867">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="65a08-868">Исправлена проблема, которая приводила к сбою при создании масштабируемого набора виртуальных машин с внутренней подсистемой балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="65a08-868">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="65a08-869">Исправлена проблема, из-за которой аргумент `--no-wait` не работал с командой `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="65a08-869">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="65a08-870">15 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="65a08-870">August 15, 2017</span></span>

<span data-ttu-id="65a08-871">Версия 2.0.14</span><span class="sxs-lookup"><span data-stu-id="65a08-871">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="65a08-872">ACS</span><span class="sxs-lookup"><span data-stu-id="65a08-872">ACS</span></span>

* <span data-ttu-id="65a08-873">Исправлен номер порта sshMaster0 для Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="65a08-873">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="65a08-874">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="65a08-874">Appservice</span></span>

* <span data-ttu-id="65a08-875">Исправлено исключение при создании веб-приложения Linux на основе Git.</span><span class="sxs-lookup"><span data-stu-id="65a08-875">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="65a08-876">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="65a08-876">Event Grid</span></span>

* <span data-ttu-id="65a08-877">Добавлены зависимости пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="65a08-877">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="65a08-878">11 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="65a08-878">August 11, 2017</span></span>

<span data-ttu-id="65a08-879">Версия 2.0.13</span><span class="sxs-lookup"><span data-stu-id="65a08-879">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="65a08-880">ACS</span><span class="sxs-lookup"><span data-stu-id="65a08-880">ACS</span></span>

* <span data-ttu-id="65a08-881">Добавлены дополнительные регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="65a08-881">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="65a08-882">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="65a08-882">Batch</span></span>

* <span data-ttu-id="65a08-883">Пакет SDK для пакетной службы обновлен до версии 3.1.0, а пакет SDK для управления пакетной службой — до версии 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="65a08-883">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="65a08-884">Добавлена новая команда для отображения количества задач в задании.</span><span class="sxs-lookup"><span data-stu-id="65a08-884">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="65a08-885">Исправлена ошибка при обработке URL-адреса SAS файла ресурсов.</span><span class="sxs-lookup"><span data-stu-id="65a08-885">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="65a08-886">Для конечной точки учетной записи пакетной службы теперь поддерживается дополнительный префикс https://.</span><span class="sxs-lookup"><span data-stu-id="65a08-886">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="65a08-887">Поддерживается добавление к заданию списков, содержащих более 100 задач.</span><span class="sxs-lookup"><span data-stu-id="65a08-887">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="65a08-888">Добавлено ведение журнала отладки при загрузке командного модуля расширений.</span><span class="sxs-lookup"><span data-stu-id="65a08-888">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="65a08-889">Компонент</span><span class="sxs-lookup"><span data-stu-id="65a08-889">Component</span></span>

* <span data-ttu-id="65a08-890">Добавлено предупреждение о прекращении поддержки в команды az component.</span><span class="sxs-lookup"><span data-stu-id="65a08-890">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="65a08-891">Контейнер</span><span class="sxs-lookup"><span data-stu-id="65a08-891">Container</span></span>

* <span data-ttu-id="65a08-892">`create`. Исправлена проблема, из-за которой запрещалось использовать знак равенства в переменной среды.</span><span class="sxs-lookup"><span data-stu-id="65a08-892">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="65a08-893">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="65a08-893">Data Lake Store</span></span>

* <span data-ttu-id="65a08-894">Включен индикатор хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="65a08-894">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="65a08-895">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="65a08-895">Event Grid</span></span>

* <span data-ttu-id="65a08-896">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="65a08-896">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="65a08-897">Сеть</span><span class="sxs-lookup"><span data-stu-id="65a08-897">Network</span></span>

* <span data-ttu-id="65a08-898">`lb`. Исправлена проблема, из-за которой некоторые имена дочерних ресурсов не разрешались правильно, если не были указаны.</span><span class="sxs-lookup"><span data-stu-id="65a08-898">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="65a08-899">`application-gateway {subresource} delete`. Исправлена проблема, из-за которой не учитывался параметр `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="65a08-899">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="65a08-900">`application-gateway http-settings update`. Исправлена проблема, из-за которой не удавалось отключить параметр `--connection-draining-timeout`.</span><span class="sxs-lookup"><span data-stu-id="65a08-900">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="65a08-901">Исправлена проблема с непредвиденным аргументом ключевого слова `sa_data_size_kilobyes` при использовании с командой `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="65a08-901">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="65a08-902">Профиль</span><span class="sxs-lookup"><span data-stu-id="65a08-902">Profile</span></span>

* <span data-ttu-id="65a08-903">`account list`. Добавлен параметр `--refresh` для синхронизации последних подписок с сервером.</span><span class="sxs-lookup"><span data-stu-id="65a08-903">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="65a08-904">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="65a08-904">Storage</span></span>

* <span data-ttu-id="65a08-905">Включено обновление учетной записи хранения с помощью удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="65a08-905">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="65a08-906">ВМ</span><span class="sxs-lookup"><span data-stu-id="65a08-906">VM</span></span>

* <span data-ttu-id="65a08-907">`availability-set`. Предоставлено число доменов сбоя при преобразовании.</span><span class="sxs-lookup"><span data-stu-id="65a08-907">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="65a08-908">Предоставлена команда `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="65a08-908">Exposed `list-skus` command</span></span>
* <span data-ttu-id="65a08-909">Поддерживается назначение удостоверений без создания назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="65a08-909">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="65a08-910">При подключении дисков данных применяется номер SKU хранилища.</span><span class="sxs-lookup"><span data-stu-id="65a08-910">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="65a08-911">Удалено используемое по умолчанию имя диска ОС и номер SKU хранилища при использовании управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="65a08-911">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="65a08-912">28 июля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="65a08-912">July 28, 2017</span></span>

<span data-ttu-id="65a08-913">Версия 2.0.12</span><span class="sxs-lookup"><span data-stu-id="65a08-913">Version 2.0.12</span></span>

* <span data-ttu-id="65a08-914">Добавлены команды для контейнеров.</span><span class="sxs-lookup"><span data-stu-id="65a08-914">Added container commands</span></span>
* <span data-ttu-id="65a08-915">Добавлены модули выставления счетов и потребления ресурсов.</span><span class="sxs-lookup"><span data-stu-id="65a08-915">Added billing and consumption modules</span></span>

```
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

### <a name="core"></a><span data-ttu-id="65a08-916">Core</span><span class="sxs-lookup"><span data-stu-id="65a08-916">Core</span></span>

* <span data-ttu-id="65a08-917">Вывод сведений о пакетах SDK для проверки подлинности субъектов-служб с помощью сертификатов.</span><span class="sxs-lookup"><span data-stu-id="65a08-917">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="65a08-918">Исправлены исключения в ходе выполнения развертывания.</span><span class="sxs-lookup"><span data-stu-id="65a08-918">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="65a08-919">Для создания клиента подписки используется конечная точка ARM текущего облака.</span><span class="sxs-lookup"><span data-stu-id="65a08-919">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="65a08-920">Улучшена параллельная обработка файла clouds.config (3636).</span><span class="sxs-lookup"><span data-stu-id="65a08-920">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="65a08-921">Обновление идентификатора клиентского запроса при каждом выполнении команды.</span><span class="sxs-lookup"><span data-stu-id="65a08-921">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="65a08-922">Создание клиентов подписки с правильным профилем SDK (3635).</span><span class="sxs-lookup"><span data-stu-id="65a08-922">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="65a08-923">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="65a08-923">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="65a08-924">Добавлена поддержка выбора полей вывода в таблице с помощью запроса jmespath (3581).</span><span class="sxs-lookup"><span data-stu-id="65a08-924">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="65a08-925">Улучшено отключение аргументов анализа и добавлено ведение журналов с помощью жестов (3434).</span><span class="sxs-lookup"><span data-stu-id="65a08-925">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="65a08-926">Создание клиентов подписки с правильным профилем SDK.</span><span class="sxs-lookup"><span data-stu-id="65a08-926">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="65a08-927">Перемещение всех существующих файлов записи в последнюю папку.</span><span class="sxs-lookup"><span data-stu-id="65a08-927">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="65a08-928">Исправлена идемпотентность при создании виртуальной машины или масштабируемого набора виртуальных машин (3586).</span><span class="sxs-lookup"><span data-stu-id="65a08-928">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="65a08-929">В путях команд больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="65a08-929">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="65a08-930">В определенных параметрах логического типа больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="65a08-930">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="65a08-931">Поддержка входа на локальный сервер AD FS, например Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="65a08-931">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="65a08-932">Исправлена параллельная запись в файл clouds.config (3255).</span><span class="sxs-lookup"><span data-stu-id="65a08-932">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="65a08-933">ACR</span><span class="sxs-lookup"><span data-stu-id="65a08-933">ACR</span></span>

* <span data-ttu-id="65a08-934">Добавлена команда `show-usage` для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="65a08-934">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="65a08-935">Поддержка обновления номера SKU для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="65a08-935">Support SKU update for managed registries</span></span>
* <span data-ttu-id="65a08-936">Добавлены управляемые реестры с управляемыми номерами SKU.</span><span class="sxs-lookup"><span data-stu-id="65a08-936">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="65a08-937">Добавлены веб-перехватчики для управляемых реестров с использованием модуля для команды acr webhook.</span><span class="sxs-lookup"><span data-stu-id="65a08-937">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="65a08-938">Добавлена проверка подлинности с помощью AAD с использованием команды acr login.</span><span class="sxs-lookup"><span data-stu-id="65a08-938">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="65a08-939">Добавлена команда delete для репозиториев, манифестов и тегов Docker.</span><span class="sxs-lookup"><span data-stu-id="65a08-939">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="65a08-940">ACS</span><span class="sxs-lookup"><span data-stu-id="65a08-940">ACS</span></span>

* <span data-ttu-id="65a08-941">Поддержка API версии 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="65a08-941">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="65a08-942">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="65a08-942">Appservice</span></span>

* <span data-ttu-id="65a08-943">Исправлена ошибка, из-за которой команда вывода списка в веб-приложениях Linux не возвращала данные.</span><span class="sxs-lookup"><span data-stu-id="65a08-943">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="65a08-944">Поддержка извлечения учетных данных из ACR.</span><span class="sxs-lookup"><span data-stu-id="65a08-944">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="65a08-945">Удаление всех команд группы `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="65a08-945">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="65a08-946">Создание масок паролей для реестров Docker из выходных данных команды (3656).</span><span class="sxs-lookup"><span data-stu-id="65a08-946">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="65a08-947">Обеспечено использование браузера по умолчанию в macOS без ошибок (3623).</span><span class="sxs-lookup"><span data-stu-id="65a08-947">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="65a08-948">Улучшена справка по командам `webapp log tail` и `webapp log download` (3624).</span><span class="sxs-lookup"><span data-stu-id="65a08-948">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="65a08-949">Предоставлена команда `traffic-routing` для настройки статической маршрутизации (3566).</span><span class="sxs-lookup"><span data-stu-id="65a08-949">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="65a08-950">Добавлены исправления, связанные с надежностью, при настройке системы управления версиями (3245).</span><span class="sxs-lookup"><span data-stu-id="65a08-950">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="65a08-951">Удален неподдерживаемый аргумент `--node-version` из функции `webapp config update` для веб-приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="65a08-951">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="65a08-952">Вместо него используется `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="65a08-952">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="65a08-953">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="65a08-953">Batch</span></span>

* <span data-ttu-id="65a08-954">Пакеты SDK для пакетной службы обновлены до версии 3.0.0 с поддержкой низкоприоритетных виртуальных машин в пулах.</span><span class="sxs-lookup"><span data-stu-id="65a08-954">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="65a08-955">Параметр команды `pool create` переименован с `--target-dedicated` в `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="65a08-955">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="65a08-956">Для команды `pool create` добавлены параметры `--target-low-priority-nodes` и `--application-licenses`.</span><span class="sxs-lookup"><span data-stu-id="65a08-956">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="65a08-957">CDN</span><span class="sxs-lookup"><span data-stu-id="65a08-957">CDN</span></span>

* <span data-ttu-id="65a08-958">Предоставлено улучшенное сообщение об ошибке для команды `cdn endpoint list`, которое отображается, если заданный параметром `--profile-name` профиль не существует.</span><span class="sxs-lookup"><span data-stu-id="65a08-958">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="65a08-959">Облако</span><span class="sxs-lookup"><span data-stu-id="65a08-959">Cloud</span></span>

* <span data-ttu-id="65a08-960">Формат версии API конечной точки метаданных облака изменен на следующий: ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="65a08-960">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="65a08-961">Конечная точка коллекции не является обязательной.</span><span class="sxs-lookup"><span data-stu-id="65a08-961">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="65a08-962">Поддерживается регистрация облака только с конечной точкой диспетчера ARM.</span><span class="sxs-lookup"><span data-stu-id="65a08-962">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="65a08-963">Предоставлен параметр в команде `cloud set` для выбора профиля при выборе текущего облака.</span><span class="sxs-lookup"><span data-stu-id="65a08-963">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="65a08-964">Предоставлен параметр `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="65a08-964">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="65a08-965">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="65a08-965">CosmosDB</span></span>

* <span data-ttu-id="65a08-966">Внесены исправления, которые позволяют создавать коллекцию с пользовательским ключом секции.</span><span class="sxs-lookup"><span data-stu-id="65a08-966">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="65a08-967">Добавлена поддержка срока жизни по умолчанию для коллекции.</span><span class="sxs-lookup"><span data-stu-id="65a08-967">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="65a08-968">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="65a08-968">Data Lake Analytics</span></span>

* <span data-ttu-id="65a08-969">Добавлены команды для управления политикой вычислений в разделе `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="65a08-969">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="65a08-970">Добавлена команда `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="65a08-970">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="65a08-971">Добавлена команда `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="65a08-971">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="65a08-972">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="65a08-972">Data Lake Store</span></span>

* <span data-ttu-id="65a08-973">Добавлена поддержка смены ключей пользовательского хранилища ключей в `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="65a08-973">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="65a08-974">Обновлена версия пакета SDK для базовой файловой системы Data Lake Store из-за проблем с производительностью.</span><span class="sxs-lookup"><span data-stu-id="65a08-974">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="65a08-975">Добавлена команда `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="65a08-975">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="65a08-976">Эта команда пытается активировать пользовательское хранилище ключей, предназначенное для шифрования данных в учетной записи Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="65a08-976">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="65a08-977">Интерактивный режим</span><span class="sxs-lookup"><span data-stu-id="65a08-977">Interactive</span></span>

* <span data-ttu-id="65a08-978">Улучшено время запуска с помощью кэшированных команд.</span><span class="sxs-lookup"><span data-stu-id="65a08-978">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="65a08-979">Увеличено тестовое покрытие.</span><span class="sxs-lookup"><span data-stu-id="65a08-979">Increased test coverage</span></span>
* <span data-ttu-id="65a08-980">Расширены возможности жеста "?", которые позволяют также вставить его в следующую команду.</span><span class="sxs-lookup"><span data-stu-id="65a08-980">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="65a08-981">Исправлены ошибки с интерактивными функциями в предварительной версии профиля 2017-03-09 (3587).</span><span class="sxs-lookup"><span data-stu-id="65a08-981">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="65a08-982">Разрешено использовать `--version` в качестве параметра в интерактивном режиме (3645).</span><span class="sxs-lookup"><span data-stu-id="65a08-982">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="65a08-983">В интерактивном режиме больше не возникают ошибки при выполнении проверки (3570).</span><span class="sxs-lookup"><span data-stu-id="65a08-983">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="65a08-984">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="65a08-984">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="65a08-985">Добавлен флаг `--progress`.</span><span class="sxs-lookup"><span data-stu-id="65a08-985">Added `--progress` flag</span></span>
* <span data-ttu-id="65a08-986">Из вариантов завершения удалены `--debug` и `--verbose`.</span><span class="sxs-lookup"><span data-stu-id="65a08-986">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="65a08-987">Из вариантов завершения удален `interactive` (3324).</span><span class="sxs-lookup"><span data-stu-id="65a08-987">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="65a08-988">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="65a08-988">IoT</span></span>

* <span data-ttu-id="65a08-989">Исправлено. При создании политики больше не удаляются существующие политики</span><span class="sxs-lookup"><span data-stu-id="65a08-989">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="65a08-990">(3934).</span><span class="sxs-lookup"><span data-stu-id="65a08-990">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="65a08-991">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="65a08-991">Key vault</span></span>

* <span data-ttu-id="65a08-992">Добавлены команды для функций восстановления хранилища ключей:</span><span class="sxs-lookup"><span data-stu-id="65a08-992">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="65a08-993">`keyvault`, подкоманды `purge`, `recover` и `keyvault list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="65a08-993">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="65a08-994">`keyvault secret`, подкоманды `backup`, `restore`, `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="65a08-994">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="65a08-995">`keyvault certificate`, подкоманды `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="65a08-995">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="65a08-996">`keyvault key`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="65a08-996">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="65a08-997">Добавлена интеграция хранилища ключей с субъектом-службой (3133).</span><span class="sxs-lookup"><span data-stu-id="65a08-997">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="65a08-998">Обновлена плоскость данных хранилища ключей до версии 0.3.2</span><span class="sxs-lookup"><span data-stu-id="65a08-998">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="65a08-999">(3307).</span><span class="sxs-lookup"><span data-stu-id="65a08-999">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="65a08-1000">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="65a08-1000">Lab</span></span>

* <span data-ttu-id="65a08-1001">Добавлена поддержка запросов ко всем виртуальным машинам в лаборатории с помощью `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="65a08-1001">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="65a08-1002">Добавлен модуль форматирования табличных выходных данных команд `az lab vm list` и `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="65a08-1002">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="65a08-1003">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="65a08-1003">Monitor</span></span>

* <span data-ttu-id="65a08-1004">Исправлены ошибки с файлом шаблона с помощью команды `monitor autoscale-settings get-parameters-template` (3349).</span><span class="sxs-lookup"><span data-stu-id="65a08-1004">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="65a08-1005">Команда `monitor alert-rule-incidents list` переименована в `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="65a08-1005">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="65a08-1006">Команда `monitor alert-rule-incidents show` переименована в `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="65a08-1006">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="65a08-1007">Команда `monitor metric-defintions list` переименована в `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="65a08-1007">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="65a08-1008">Команда `monitor alert-rules` переименована в `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="65a08-1008">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="65a08-1009">В команду `monitor alert create` внесены следующие изменения:</span><span class="sxs-lookup"><span data-stu-id="65a08-1009">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="65a08-1010">подкоманды `condition` и `action` больше не принимают данные JSON;</span><span class="sxs-lookup"><span data-stu-id="65a08-1010">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="65a08-1011">добавлены различные параметры, которые упрощают процесс создания правила;</span><span class="sxs-lookup"><span data-stu-id="65a08-1011">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="65a08-1012">параметр `location` больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="65a08-1012">`location` no longer required</span></span>
  * <span data-ttu-id="65a08-1013">добавлена поддержка имени и идентификатора для целевого объекта;</span><span class="sxs-lookup"><span data-stu-id="65a08-1013">Add name and ID support for target</span></span>
  * <span data-ttu-id="65a08-1014">удален параметр `--alert-rule-resource-name`;</span><span class="sxs-lookup"><span data-stu-id="65a08-1014">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="65a08-1015">параметр `is-enabled` переименован в `enabled`, он больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="65a08-1015">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="65a08-1016">значения по умолчанию для `description` теперь основаны на указанном условии;</span><span class="sxs-lookup"><span data-stu-id="65a08-1016">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="65a08-1017">добавлены примеры, в которых подробно представлен новый формат.</span><span class="sxs-lookup"><span data-stu-id="65a08-1017">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="65a08-1018">Поддержка имен или идентификаторов для команд `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="65a08-1018">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="65a08-1019">Добавлены вспомогательные аргументы и примеры использования команды `monitor alert rule update`.</span><span class="sxs-lookup"><span data-stu-id="65a08-1019">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="65a08-1020">Сеть</span><span class="sxs-lookup"><span data-stu-id="65a08-1020">Network</span></span>

* <span data-ttu-id="65a08-1021">Добавлена команда `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="65a08-1021">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="65a08-1022">Добавлен аргумент `--private-access-services` в команды `vnet subnet create` и `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="65a08-1022">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="65a08-1023">Исправлена проблема, из-за которой команда `application-gateway redirect-config create` завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="65a08-1023">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="65a08-1024">Исправлена проблема, из-за которой команда `application-gateway redirect-config update` не работала с параметром `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="65a08-1024">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="65a08-1025">Исправлена ошибка при использовании аргумента `--servers` с командами `application-gateway address-pool create` и `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="65a08-1025">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="65a08-1026">Добавлены команды `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="65a08-1026">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="65a08-1027">В команду `application-gateway ssl-policy` добавлены подкоманды `list-options`, `predefined list` и `predefined show`.</span><span class="sxs-lookup"><span data-stu-id="65a08-1027">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="65a08-1028">В команду `application-gateway ssl-policy set` добавлены аргументы `--name`, `--cipher-suites` и `--min-protocol-version`.</span><span class="sxs-lookup"><span data-stu-id="65a08-1028">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="65a08-1029">В команды `application-gateway http-settings create` и `application-gateway http-settings update` добавлены аргументы `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe` и `--path`.</span><span class="sxs-lookup"><span data-stu-id="65a08-1029">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="65a08-1030">В команды `application-gateway url-path-map create` и `application-gateway url-path-map update` добавлены аргументы `--default-redirect-config` и `--redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="65a08-1030">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="65a08-1031">Добавлен аргумент `--redirect-config` в команду `application-gateway url-path-map rule create`.</span><span class="sxs-lookup"><span data-stu-id="65a08-1031">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="65a08-1032">Добавлена поддержка параметра `--no-wait` в команде `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="65a08-1032">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="65a08-1033">В команды `application-gateway probe create` и `application-gateway probe update` добавлены аргументы `--host-name-from-http-settings`, `--min-servers`, `--match-body` и `--match-status-codes`.</span><span class="sxs-lookup"><span data-stu-id="65a08-1033">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="65a08-1034">Добавлен аргумент `--redirect-config` в команды `application-gateway rule create` и `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="65a08-1034">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="65a08-1035">Добавлена поддержка аргумента `--accelerated-networking` в командах `nic create` и `nic update`.</span><span class="sxs-lookup"><span data-stu-id="65a08-1035">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="65a08-1036">Удален аргумент `--internal-dns-name-suffix` из команды `nic create`.</span><span class="sxs-lookup"><span data-stu-id="65a08-1036">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="65a08-1037">Добавлена поддержка параметра `--dns-servers` в командах `nic update` и `nic create`. Добавлена поддержка параметра --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="65a08-1037">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="65a08-1038">Исправлена ошибка, из-за которой команда `local-gateway create` игнорировала параметр `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="65a08-1038">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="65a08-1039">Добавлена поддержка параметра `--dns-servers` в команде `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="65a08-1039">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="65a08-1040">Исправлена ошибка при создании пиринга без фильтрации маршрутов с помощью команды `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="65a08-1040">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="65a08-1041">Исправлена ошибка, из-за которой аргументы `--provider` и `--bandwidth` не работали с командой `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="65a08-1041">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="65a08-1042">Исправлена ошибка с логикой установки значений по умолчанию в команде `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="65a08-1042">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="65a08-1043">Улучшено форматирование выходных данных команды `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="65a08-1043">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="65a08-1044">В команде `application-gateway http-listener create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="65a08-1044">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="65a08-1045">В команде `application-gateway rule create` используются пул адресов, параметры HTTP и прослушиватель HTTP по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="65a08-1045">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="65a08-1046">В команде `lb rule create` используются интерфейсный IP-адрес и серверный пул по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="65a08-1046">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="65a08-1047">В команде `lb inbound-nat-rule create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="65a08-1047">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="65a08-1048">Профиль</span><span class="sxs-lookup"><span data-stu-id="65a08-1048">Profile</span></span>

* <span data-ttu-id="65a08-1049">Поддержка входа на виртуальную машину с использованием управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="65a08-1049">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="65a08-1050">Поддержка вывода данных команды `account show` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="65a08-1050">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="65a08-1051">При использовании параметра --expanded-view отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="65a08-1051">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="65a08-1052">Добавлена команда `get-access-token` для предоставления необработанного токена AAD.</span><span class="sxs-lookup"><span data-stu-id="65a08-1052">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="65a08-1053">Поддержка входа с учетной записью пользователя без связанных подписок.</span><span class="sxs-lookup"><span data-stu-id="65a08-1053">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="65a08-1054">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="65a08-1054">RDBMS</span></span>

* <span data-ttu-id="65a08-1055">Поддержка вывода списка серверов в подписке (3417).</span><span class="sxs-lookup"><span data-stu-id="65a08-1055">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="65a08-1056">Исправлена проблема, когда объект `%s` не обрабатывался из-за отсутствия `% server_type` (3393).</span><span class="sxs-lookup"><span data-stu-id="65a08-1056">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="65a08-1057">Исправлено сопоставление источника документа и добавлена задача непрерывной интеграции для проверки (3361).</span><span class="sxs-lookup"><span data-stu-id="65a08-1057">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="65a08-1058">Исправлена справка по MySQL и PostgreSQL (3369).</span><span class="sxs-lookup"><span data-stu-id="65a08-1058">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="65a08-1059">Ресурс</span><span class="sxs-lookup"><span data-stu-id="65a08-1059">Resource</span></span>

* <span data-ttu-id="65a08-1060">Улучшены запросы на ввод отсутствующих параметров для команды `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="65a08-1060">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="65a08-1061">Улучшен анализ синтаксиса `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="65a08-1061">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="65a08-1062">Исправлены проблемы, из-за которых файлы параметров `group deployment create` не распознавались с использованием синтаксиса `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="65a08-1062">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="65a08-1063">Поддержка аргумента `--ids` в командах `resource` и `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="65a08-1063">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="65a08-1064">Исправлены некоторые сообщения об ошибках и анализе (3584).</span><span class="sxs-lookup"><span data-stu-id="65a08-1064">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="65a08-1065">Исправлены ошибки анализа параметра `--resource-type` в команде `lock`. Теперь принимаются `<resource-namespace>` и `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="65a08-1065">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="65a08-1066">Добавлена проверка параметров для шаблонов для ссылок на шаблоны (3629).</span><span class="sxs-lookup"><span data-stu-id="65a08-1066">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="65a08-1067">Добавлена поддержка указания параметров развертывания с использованием синтаксиса `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="65a08-1067">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="65a08-1068">Роль</span><span class="sxs-lookup"><span data-stu-id="65a08-1068">Role</span></span>

* <span data-ttu-id="65a08-1069">Поддержка вывода данных команды `create-for-rbac` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="65a08-1069">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="65a08-1070">Добавлена очистка назначений ролей и связанного приложения AAD при удалении субъекта-службы (3610).</span><span class="sxs-lookup"><span data-stu-id="65a08-1070">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="65a08-1071">В описания аргументов `--start-date` и `--end-date` команды `app create` добавлен формат времени.</span><span class="sxs-lookup"><span data-stu-id="65a08-1071">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="65a08-1072">При использовании параметра `--expanded-view` отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="65a08-1072">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="65a08-1073">Добавлена интеграция хранилища ключей для команд `create-for-rbac` и `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="65a08-1073">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="65a08-1074">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="65a08-1074">Service Fabric</span></span>
* <span data-ttu-id="65a08-1075">Исправлена ошибка, из-за которой большие файлы в приложениях усекались при отправке (3666).</span><span class="sxs-lookup"><span data-stu-id="65a08-1075">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="65a08-1076">Добавлены тесты для команд Service Fabric (3424).</span><span class="sxs-lookup"><span data-stu-id="65a08-1076">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="65a08-1077">Исправлены многие команды Service Fabric (3234).</span><span class="sxs-lookup"><span data-stu-id="65a08-1077">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="65a08-1078">SQL</span><span class="sxs-lookup"><span data-stu-id="65a08-1078">SQL</span></span>

* <span data-ttu-id="65a08-1079">Удален недействительный параметр `--identity` команды `sql server create`.</span><span class="sxs-lookup"><span data-stu-id="65a08-1079">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="65a08-1080">Удалены значения паролей из выходных данных команд `sql server create` и `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="65a08-1080">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="65a08-1081">Добавлены команды `sql db list-editions` и `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="65a08-1081">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="65a08-1082">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="65a08-1082">Storage</span></span>

* <span data-ttu-id="65a08-1083">Удален параметр `--marker` из команд `storage blob list`, `storage container list` и `storage share list` (3745).</span><span class="sxs-lookup"><span data-stu-id="65a08-1083">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="65a08-1084">Включено создание учетных записей хранения с поддержкой только HTTPS.</span><span class="sxs-lookup"><span data-stu-id="65a08-1084">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="65a08-1085">Обновлены метрики хранилища, команды входа и CORS (3495).</span><span class="sxs-lookup"><span data-stu-id="65a08-1085">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="65a08-1086">Перефразировано сообщение об исключении, которое выводит команда добавления CORS (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="65a08-1086">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="65a08-1087">Генератор преобразован в список в режиме пробного выполнения команды пакетной загрузки (3592).</span><span class="sxs-lookup"><span data-stu-id="65a08-1087">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="65a08-1088">Исправлена проблема при пробном выполнении команды пакетной загрузки больших двоичных объектов (3640) (3592).</span><span class="sxs-lookup"><span data-stu-id="65a08-1088">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="65a08-1089">ВМ</span><span class="sxs-lookup"><span data-stu-id="65a08-1089">VM</span></span>

* <span data-ttu-id="65a08-1090">Поддержка настройки NSG.</span><span class="sxs-lookup"><span data-stu-id="65a08-1090">Support configuring nsg</span></span>
* <span data-ttu-id="65a08-1091">Исправлена ошибка, из-за которой не удавалось правильно настроить DNS-сервер.</span><span class="sxs-lookup"><span data-stu-id="65a08-1091">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="65a08-1092">Поддержка удостоверений управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="65a08-1092">Support managed service identities</span></span>
* <span data-ttu-id="65a08-1093">Исправлена проблема, из-за которой для команды `cmss create` с существующей подсистемой балансировки нагрузки требовался параметр `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="65a08-1093">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="65a08-1094">Теперь нумерация LUN дисков данных, создаваемых с помощью команды `vm image create`, начинается с 0.</span><span class="sxs-lookup"><span data-stu-id="65a08-1094">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="65a08-1095">10 мая 2017 г.</span><span class="sxs-lookup"><span data-stu-id="65a08-1095">May 10, 2017</span></span>

<span data-ttu-id="65a08-1096">Версия 2.0.6</span><span class="sxs-lookup"><span data-stu-id="65a08-1096">Version 2.0.6</span></span>

* <span data-ttu-id="65a08-1097">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="65a08-1097">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="65a08-1098">Добавлена реляционная СУБД (MySQL, Postgres).</span><span class="sxs-lookup"><span data-stu-id="65a08-1098">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="65a08-1099">Добавлены модули Data Lake Store и Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="65a08-1099">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="65a08-1100">Добавлен модуль Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="65a08-1100">Include Cognitive Services module</span></span>
* <span data-ttu-id="65a08-1101">Добавлен модуль Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="65a08-1101">Include Service Fabric module</span></span>
* <span data-ttu-id="65a08-1102">Добавлен модуль Interactive (az-shell переименован).</span><span class="sxs-lookup"><span data-stu-id="65a08-1102">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="65a08-1103">Добавлена поддержка команд CDN.</span><span class="sxs-lookup"><span data-stu-id="65a08-1103">Add support for CDN commands</span></span>
* <span data-ttu-id="65a08-1104">Удален модуль Container.</span><span class="sxs-lookup"><span data-stu-id="65a08-1104">Remove Container module</span></span>
* <span data-ttu-id="65a08-1105">Добавлена команда az -v для az --version ([№ 2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="65a08-1105">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="65a08-1106">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="65a08-1106">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

```
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

### <a name="core"></a><span data-ttu-id="65a08-1107">Core</span><span class="sxs-lookup"><span data-stu-id="65a08-1107">Core</span></span>

* <span data-ttu-id="65a08-1108">Ядро: запись исключений, порожденных незарегистрированным поставщиком, и его автоматическая регистрация.</span><span class="sxs-lookup"><span data-stu-id="65a08-1108">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="65a08-1109">Производительность: сохранение кэша маркеров библиотеки ADAL в памяти до завершения работы процесса ([№ 2603](https://github.com/Azure/azure-cli/issues/2603)).</span><span class="sxs-lookup"><span data-stu-id="65a08-1109">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="65a08-1110">Исправление байтов, возвращаемых из шестнадцатеричных отпечатков -o tsv ([№ 3053](https://github.com/Azure/azure-cli/issues/3053)).</span><span class="sxs-lookup"><span data-stu-id="65a08-1110">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="65a08-1111">Улучшенное скачивание сертификатов Key Vault и интеграция субъектов-служб AAD ([№ 3003](https://github.com/Azure/azure-cli/issues/3003)).</span><span class="sxs-lookup"><span data-stu-id="65a08-1111">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="65a08-1112">Добавление расположения Python в az -version ([№ 2986](https://github.com/Azure/azure-cli/issues/2986)).</span><span class="sxs-lookup"><span data-stu-id="65a08-1112">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="65a08-1113">Вход: поддержка входа при отсутствии подписок ([№ 2929](https://github.com/Azure/azure-cli/issues/2929)).</span><span class="sxs-lookup"><span data-stu-id="65a08-1113">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="65a08-1114">Ядро: устранен сбой при двукратном входе с помощью субъекта-службы ([№ 2800](https://github.com/Azure/azure-cli/issues/2800)).</span><span class="sxs-lookup"><span data-stu-id="65a08-1114">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="65a08-1115">Ядро: возможность настроить путь к файлу accessTokens.json с помощью env var ([№ 2605](https://github.com/Azure/azure-cli/issues/2605)).</span><span class="sxs-lookup"><span data-stu-id="65a08-1115">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="65a08-1116">Ядро: возможность применять настроенные параметры по умолчанию к необязательным аргументам ([№ 2703](https://github.com/Azure/azure-cli/issues/2703)).</span><span class="sxs-lookup"><span data-stu-id="65a08-1116">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="65a08-1117">Ядро: повышение производительности.</span><span class="sxs-lookup"><span data-stu-id="65a08-1117">core: Improved performance</span></span>
* <span data-ttu-id="65a08-1118">Ядро: настаиваемые сертификаты ЦС — поддержка настройки переменной среды REQUESTS_CA_BUNDLE.</span><span class="sxs-lookup"><span data-stu-id="65a08-1118">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="65a08-1119">Ядро: облачная конфигурация — использование конечной точки Resource Manager, если не задана конечная точка управления.</span><span class="sxs-lookup"><span data-stu-id="65a08-1119">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="65a08-1120">ACS</span><span class="sxs-lookup"><span data-stu-id="65a08-1120">ACS</span></span>

* <span data-ttu-id="65a08-1121">Исправление: теперь значение счетчика баз данных master и агентов — целое число, а не строка.</span><span class="sxs-lookup"><span data-stu-id="65a08-1121">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="65a08-1122">Предоставлены команды az acs create --no-wait и az acs wait для асинхронного создания.</span><span class="sxs-lookup"><span data-stu-id="65a08-1122">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="65a08-1123">Предоставлена команда az acs create --validate для пробного создания.</span><span class="sxs-lookup"><span data-stu-id="65a08-1123">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="65a08-1124">Удален профиль Windows перед вызовом метода PUT для команды scale ([№ 2755](https://github.com/Azure/azure-cli/issues/2755)).</span><span class="sxs-lookup"><span data-stu-id="65a08-1124">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="65a08-1125">AppService</span><span class="sxs-lookup"><span data-stu-id="65a08-1125">AppService</span></span>

* <span data-ttu-id="65a08-1126">Приложение-функция: добавлена полная поддержка приложений-функций, включая создание, отображение, вывод списка, удаление, настройку имени узла, настройку протокола SSL и т. д.</span><span class="sxs-lookup"><span data-stu-id="65a08-1126">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="65a08-1127">Добавлены службы Team Services (VSTS) в качестве параметра непрерывной доставки в конфигурации веб-системы управления версиями службы приложений.</span><span class="sxs-lookup"><span data-stu-id="65a08-1127">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="65a08-1128">Создана команда az webapp, заменяющая команду az appservice web (для обеспечения обратной совместимости команда az appservice web будет оставлена еще в двух выпусках).</span><span class="sxs-lookup"><span data-stu-id="65a08-1128">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="65a08-1129">Предоставлены аргументы для настройки развертывания и стеков времени выполнения при создании веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="65a08-1129">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="65a08-1130">Предоставлена команда webapp list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="65a08-1130">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="65a08-1131">Поддержка настройки строк подключения ([№ 2647](https://github.com/Azure/azure-cli/issues/2647)).</span><span class="sxs-lookup"><span data-stu-id="65a08-1131">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="65a08-1132">Поддержка переключения слотов с предварительным просмотром.</span><span class="sxs-lookup"><span data-stu-id="65a08-1132">support slot swap with preview</span></span>
* <span data-ttu-id="65a08-1133">Устранены ошибки из команд службы приложений ([№ 2948](https://github.com/Azure/azure-cli/issues/2948)).</span><span class="sxs-lookup"><span data-stu-id="65a08-1133">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="65a08-1134">Использование группы ресурсов в плане служб приложений для операций с сертификатами ([№ 2750](https://github.com/Azure/azure-cli/issues/2750)).</span><span class="sxs-lookup"><span data-stu-id="65a08-1134">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="65a08-1135">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="65a08-1135">CosmosDB</span></span>

* <span data-ttu-id="65a08-1136">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="65a08-1136">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="65a08-1137">Добавлена поддержка интерфейсов API уровня данных DocumentDB: управление базами данных и коллекциями.</span><span class="sxs-lookup"><span data-stu-id="65a08-1137">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="65a08-1138">Добавлена поддержка включения автоматической отработки отказа для учетных записей базы данных.</span><span class="sxs-lookup"><span data-stu-id="65a08-1138">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="65a08-1139">Добавлена поддержка нового параметра ConsistentPrefix политики согласованности.</span><span class="sxs-lookup"><span data-stu-id="65a08-1139">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="65a08-1140">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="65a08-1140">Data Lake Analytics</span></span>

* <span data-ttu-id="65a08-1141">Исправлена ошибка, из-за которой фильтрация списков заданий по результату и состоянию вызывала сбой.</span><span class="sxs-lookup"><span data-stu-id="65a08-1141">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="65a08-1142">Добавлена поддержка нового типа элемента каталога — пакета.</span><span class="sxs-lookup"><span data-stu-id="65a08-1142">Add support for new catalog item type: package.</span></span> <span data-ttu-id="65a08-1143">Для доступа к нему используется `az dla catalog package`.</span><span class="sxs-lookup"><span data-stu-id="65a08-1143">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="65a08-1144">Появилась возможность вывести список следующих элементов каталога из базы данных (указание схемы не требуется):</span><span class="sxs-lookup"><span data-stu-id="65a08-1144">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="65a08-1145">Таблица</span><span class="sxs-lookup"><span data-stu-id="65a08-1145">Table</span></span>
  * <span data-ttu-id="65a08-1146">функция с табличным значением;</span><span class="sxs-lookup"><span data-stu-id="65a08-1146">Table valued function</span></span>
  * <span data-ttu-id="65a08-1147">Просмотр</span><span class="sxs-lookup"><span data-stu-id="65a08-1147">View</span></span>
  * <span data-ttu-id="65a08-1148">статистика таблицы.</span><span class="sxs-lookup"><span data-stu-id="65a08-1148">Table Statistics.</span></span> <span data-ttu-id="65a08-1149">Их можно также вывести с помощью схемы, но без указания имени таблицы.</span><span class="sxs-lookup"><span data-stu-id="65a08-1149">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="65a08-1150">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="65a08-1150">Data Lake Store</span></span>

* <span data-ttu-id="65a08-1151">Обновлена версия пакета SDK базовой файловой системы, что обеспечивает лучшую поддержку сценариев регулирования на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="65a08-1151">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="65a08-1152">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="65a08-1152">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="65a08-1153">Отсутствовала справка для команды access show.</span><span class="sxs-lookup"><span data-stu-id="65a08-1153">missed help for access show.</span></span> <span data-ttu-id="65a08-1154">Теперь она добавлена.</span><span class="sxs-lookup"><span data-stu-id="65a08-1154">adding it.</span></span> <span data-ttu-id="65a08-1155">([№ 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="65a08-1155">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="65a08-1156">Поиск</span><span class="sxs-lookup"><span data-stu-id="65a08-1156">Find</span></span>

* <span data-ttu-id="65a08-1157">Улучшены результаты поиска и разрешено управление версиями индекса поиска.</span><span class="sxs-lookup"><span data-stu-id="65a08-1157">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="65a08-1158">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="65a08-1158">KeyVault</span></span>

* <span data-ttu-id="65a08-1159">BC: в команде `az keyvault certificate download` параметр -e со строкового или двоичного значения изменен на PEM или DER, чтобы лучше представить параметры.</span><span class="sxs-lookup"><span data-stu-id="65a08-1159">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="65a08-1160">BC: из команды `keyvault certificate create` удалены параметры --expires и --not-before, так как они не поддерживаются службой.</span><span class="sxs-lookup"><span data-stu-id="65a08-1160">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="65a08-1161">В команду `keyvault certificate create` добавлен параметр --validity для выборочного переопределения значение в параметре --policy.</span><span class="sxs-lookup"><span data-stu-id="65a08-1161">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="65a08-1162">Исправлена ошибка в команде `keyvault certificate get-default-policy`, в которой были доступны параметры expires и not_before, а параметр validity_in_months — нет.</span><span class="sxs-lookup"><span data-stu-id="65a08-1162">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="65a08-1163">Добавлено исправление для модуля keyvault для импорта PEM- и PFX-файлов ([№ 2754](https://github.com/Azure/azure-cli/issues/2754)).</span><span class="sxs-lookup"><span data-stu-id="65a08-1163">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="65a08-1164">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="65a08-1164">Lab</span></span>

* <span data-ttu-id="65a08-1165">Добавлены команды создания, отображения, удаления и вывода списка для среды в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="65a08-1165">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="65a08-1166">Добавлены команды отображения и вывода списка для просмотра шаблонов ARM в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="65a08-1166">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="65a08-1167">В команду `az lab vm list` добавлен флаг --environment для фильтрации виртуальных машин по среде в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="65a08-1167">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="65a08-1168">Добавлена вспомогательная команда `az lab formula export-artifacts` для экспорта шаблона артефакта в формуле лаборатории.</span><span class="sxs-lookup"><span data-stu-id="65a08-1168">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="65a08-1169">Добавлены команды для управления секретами в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="65a08-1169">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="65a08-1170">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="65a08-1170">Monitor</span></span>

* <span data-ttu-id="65a08-1171">Исправление ошибки: моделирование `--actions` в `az alert-rules create` для использования строки в формате JSON ([№ 3009](https://github.com/Azure/azure-cli/issues/3009)).</span><span class="sxs-lookup"><span data-stu-id="65a08-1171">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="65a08-1172">Исправление ошибки: при создании параметров диагностики не принимались журналы и метрики из команды show ([№ 2913](https://github.com/Azure/azure-cli/issues/2913)).</span><span class="sxs-lookup"><span data-stu-id="65a08-1172">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="65a08-1173">Сеть</span><span class="sxs-lookup"><span data-stu-id="65a08-1173">Network</span></span>

* <span data-ttu-id="65a08-1174">Добавлена команда `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="65a08-1174">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="65a08-1175">Добавлена поддержка параметра `--filters` в команде `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="65a08-1175">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="65a08-1176">Добавлена поддержка фильтрации подключений шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="65a08-1176">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="65a08-1177">Добавлена поддержка конфигурации набора правил WAF шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="65a08-1177">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="65a08-1178">Добавлена поддержка правил и фильтров маршрутов ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="65a08-1178">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="65a08-1179">Добавлена поддержка географической маршрутизации диспетчера трафика.</span><span class="sxs-lookup"><span data-stu-id="65a08-1179">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="65a08-1180">Добавлена поддержка селекторов трафика на основе политик для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="65a08-1180">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="65a08-1181">Добавлена поддержка политик IPSec для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="65a08-1181">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="65a08-1182">Исправлена ошибка `vpn-connection create`, возникавшая при использовании параметра `--no-wait` или `--validate`.</span><span class="sxs-lookup"><span data-stu-id="65a08-1182">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="65a08-1183">Добавлена поддержка шлюзов виртуальной сети "активный-активный".</span><span class="sxs-lookup"><span data-stu-id="65a08-1183">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="65a08-1184">Удалены значения NULL из выходных данных команды `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="65a08-1184">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="65a08-1185">BC: исправлена ошибка в выходных данных `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="65a08-1185">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="65a08-1186">Исправлена ошибка, приводившая к неправильному анализу аргумента --key-length команды vpn-connection create.</span><span class="sxs-lookup"><span data-stu-id="65a08-1186">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="65a08-1187">Исправлена ошибка в `dns zone import`, из-за которой записи не импортировались правильно.</span><span class="sxs-lookup"><span data-stu-id="65a08-1187">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="65a08-1188">Исправлена ошибка, из-за которой команда `traffic-manager endpoint update` не работала.</span><span class="sxs-lookup"><span data-stu-id="65a08-1188">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="65a08-1189">Добавлены команды предварительного просмотра для Наблюдателя за сетями.</span><span class="sxs-lookup"><span data-stu-id="65a08-1189">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="65a08-1190">Профиль</span><span class="sxs-lookup"><span data-stu-id="65a08-1190">Profile</span></span>

* <span data-ttu-id="65a08-1191">Поддержка входа при отсутствии подписок ([№ 2560](https://github.com/Azure/azure-cli/issues/2560)).</span><span class="sxs-lookup"><span data-stu-id="65a08-1191">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="65a08-1192">Поддержка сокращенных имен параметров в команде az account set --subscription ([№ 2980](https://github.com/Azure/azure-cli/issues/2980)).</span><span class="sxs-lookup"><span data-stu-id="65a08-1192">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="65a08-1193">Redis</span><span class="sxs-lookup"><span data-stu-id="65a08-1193">Redis</span></span>

* <span data-ttu-id="65a08-1194">Добавлена команда update, которая также добавляет возможность масштабирования для кэша Redis.</span><span class="sxs-lookup"><span data-stu-id="65a08-1194">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="65a08-1195">Команда update-settings объявляется нерекомендуемой.</span><span class="sxs-lookup"><span data-stu-id="65a08-1195">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="65a08-1196">Ресурс</span><span class="sxs-lookup"><span data-stu-id="65a08-1196">Resource</span></span>

* <span data-ttu-id="65a08-1197">Добавлены команды определения managedapp и managedapp ([№ 2985](https://github.com/Azure/azure-cli/issues/2985)).</span><span class="sxs-lookup"><span data-stu-id="65a08-1197">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="65a08-1198">Поддержка команд provider operation ([№ 2908](https://github.com/Azure/azure-cli/issues/2908)).</span><span class="sxs-lookup"><span data-stu-id="65a08-1198">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="65a08-1199">Поддержка создания универсального ресурса ([№ 2606](https://github.com/Azure/azure-cli/issues/2606)).</span><span class="sxs-lookup"><span data-stu-id="65a08-1199">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="65a08-1200">Исправлен анализ ресурсов и поиск версии API.</span><span class="sxs-lookup"><span data-stu-id="65a08-1200">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="65a08-1201">([№ 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="65a08-1201">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="65a08-1202">Добавлены документы для команды az lock update.</span><span class="sxs-lookup"><span data-stu-id="65a08-1202">Add docs for az lock update.</span></span> <span data-ttu-id="65a08-1203">([№ 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="65a08-1203">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="65a08-1204">Исправлена ошибка, возникавшая при попытке вывести список ресурсов группы, которая не существует.</span><span class="sxs-lookup"><span data-stu-id="65a08-1204">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="65a08-1205">([№ 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="65a08-1205">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="65a08-1206">[Вычисления.] Устранены проблемы с масштабируемым набором виртуальных машин и обновлением группы доступности виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="65a08-1206">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="65a08-1207">([№ 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="65a08-1207">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="65a08-1208">Исправлена блокировка создания и удаления, возникающая, если параметр parent-resource-path не указан ([№ 2742](https://github.com/Azure/azure-cli/issues/2742)).</span><span class="sxs-lookup"><span data-stu-id="65a08-1208">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="65a08-1209">Роль</span><span class="sxs-lookup"><span data-stu-id="65a08-1209">Role</span></span>

* <span data-ttu-id="65a08-1210">create-for-rbac: гарантируется, что дата завершения работы поставщика служб не может превышать срок действия сертификата ([№ 2989](https://github.com/Azure/azure-cli/issues/2989)).</span><span class="sxs-lookup"><span data-stu-id="65a08-1210">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="65a08-1211">RBAC: добавлена полная поддержка команды ad group ([№ 2016](https://github.com/Azure/azure-cli/issues/2016)).</span><span class="sxs-lookup"><span data-stu-id="65a08-1211">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="65a08-1212">Роль: устранены проблемы при обновлении определения роли ([№ 2745](https://github.com/Azure/azure-cli/issues/2745)).</span><span class="sxs-lookup"><span data-stu-id="65a08-1212">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="65a08-1213">create-for-rbac: обеспечен выбор введенного пользователем пароля.</span><span class="sxs-lookup"><span data-stu-id="65a08-1213">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="65a08-1214">SQL</span><span class="sxs-lookup"><span data-stu-id="65a08-1214">SQL</span></span>

* <span data-ttu-id="65a08-1215">Добавлены команды az sql server list-usages и az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="65a08-1215">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="65a08-1216">SQL: возможность прямого подключения к поставщику ресурса ([№ 2832](https://github.com/Azure/azure-cli/issues/2832)).</span><span class="sxs-lookup"><span data-stu-id="65a08-1216">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="65a08-1217">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="65a08-1217">Storage</span></span>

* <span data-ttu-id="65a08-1218">Добавлено расположение по умолчанию группы ресурсов для `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="65a08-1218">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="65a08-1219">Добавлена поддержка добавочного копирования больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="65a08-1219">Add support for incremental blob copy</span></span>
* <span data-ttu-id="65a08-1220">Добавлена поддержка передачи больших блочных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="65a08-1220">Add support for large block blob upload</span></span>
* <span data-ttu-id="65a08-1221">Размер блока изменяется и составляет 100 МБ, если передается файл, чей размер превышает 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="65a08-1221">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="65a08-1222">ВМ</span><span class="sxs-lookup"><span data-stu-id="65a08-1222">VM</span></span>

* <span data-ttu-id="65a08-1223">avail-set: число доменов обновления и доменов сбоя сделано необязательным.</span><span class="sxs-lookup"><span data-stu-id="65a08-1223">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="65a08-1224">Примечание. Команды виртуальной машины в независимых облаках: избегайте использовать функции, связанные с Управляемыми дисками, включая следующие:</span><span class="sxs-lookup"><span data-stu-id="65a08-1224">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="65a08-1225">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="65a08-1225">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="65a08-1226">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="65a08-1226">az vm/vmss disk</span></span>
  3. <span data-ttu-id="65a08-1227">В команде az vm/vmss create используйте параметр --use-unmanaged-disk, чтобы избежать использования Управляемых дисков. Другие команды должны работать.</span><span class="sxs-lookup"><span data-stu-id="65a08-1227">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="65a08-1228">vm/vmss: улучшен текст предупреждения при создании пары ключей SSH.</span><span class="sxs-lookup"><span data-stu-id="65a08-1228">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="65a08-1229">vm/vmss: поддержка создания из образа Marketplace, для которого требуются сведения о плане ([№ 1209](https://github.com/Azure/azure-cli/issues/1209)).</span><span class="sxs-lookup"><span data-stu-id="65a08-1229">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="65a08-1230">3 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="65a08-1230">April 3, 2017</span></span>

<span data-ttu-id="65a08-1231">Версия 2.0.2</span><span class="sxs-lookup"><span data-stu-id="65a08-1231">Version 2.0.2</span></span>

<span data-ttu-id="65a08-1232">В этом выпуске мы добавили компоненты ACR, Batch, KeyVault и SQL.</span><span class="sxs-lookup"><span data-stu-id="65a08-1232">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

```
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

### <a name="core"></a><span data-ttu-id="65a08-1233">Core</span><span class="sxs-lookup"><span data-stu-id="65a08-1233">Core</span></span>

* <span data-ttu-id="65a08-1234">Модули Acr, Lab, Monitor и Find добавлены в список по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="65a08-1234">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="65a08-1235">Вход: пропуск неправильного клиента ([#2634](https://github.com/Azure/azure-cli/pull/2634)).</span><span class="sxs-lookup"><span data-stu-id="65a08-1235">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="65a08-1236">Вход: для подписки по умолчанию задано значение 1 с состоянием "Включено" ([#2575](https://github.com/Azure/azure-cli/pull/2575)).</span><span class="sxs-lookup"><span data-stu-id="65a08-1236">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="65a08-1237">Добавлена поддержка команд wait и --no-wait для дополнительных команд ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="65a08-1237">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="65a08-1238">Core: поддержка входа при помощи субъекта-службы с использованием сертификата ([#2457](https://github.com/Azure/azure-cli/pull/2457)).</span><span class="sxs-lookup"><span data-stu-id="65a08-1238">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="65a08-1239">Добавлен запрос для отсутствующих параметров шаблона</span><span class="sxs-lookup"><span data-stu-id="65a08-1239">Add prompting for missing template parameters.</span></span> <span data-ttu-id="65a08-1240">([#2364](https://github.com/Azure/azure-cli/pull/2364)).</span><span class="sxs-lookup"><span data-stu-id="65a08-1240">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="65a08-1241">Добавлена поддержка установки параметров по умолчанию для таких распространенных аргументов, как группа ресурсов по умолчанию, веб-страница по умолчанию, виртуальная машина по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="65a08-1241">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="65a08-1242">Добавлена поддержка входа на конкретный клиент.</span><span class="sxs-lookup"><span data-stu-id="65a08-1242">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="65a08-1243">ACS</span><span class="sxs-lookup"><span data-stu-id="65a08-1243">ACS</span></span>

* <span data-ttu-id="65a08-1244">[ACS] Добавлена поддержка настройки кластера ACS по умолчанию ([#2554](https://github.com/Azure/azure-cli/pull/2554)).</span><span class="sxs-lookup"><span data-stu-id="65a08-1244">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="65a08-1245">Добавлена поддержка запроса пароля для ключа SSH</span><span class="sxs-lookup"><span data-stu-id="65a08-1245">Add support for ssh key password prompting.</span></span> <span data-ttu-id="65a08-1246">([#2044](https://github.com/Azure/azure-cli/pull/2044)).</span><span class="sxs-lookup"><span data-stu-id="65a08-1246">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="65a08-1247">Добавлена поддержка кластеров Windows</span><span class="sxs-lookup"><span data-stu-id="65a08-1247">Add support for windows clusters.</span></span> <span data-ttu-id="65a08-1248">([#2211](https://github.com/Azure/azure-cli/pull/2211)).</span><span class="sxs-lookup"><span data-stu-id="65a08-1248">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="65a08-1249">Добавлена возможность изменения роли "Владелец" на роль "Участник"</span><span class="sxs-lookup"><span data-stu-id="65a08-1249">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="65a08-1250">([#2321](https://github.com/Azure/azure-cli/pull/2321)).</span><span class="sxs-lookup"><span data-stu-id="65a08-1250">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="65a08-1251">AppService</span><span class="sxs-lookup"><span data-stu-id="65a08-1251">AppService</span></span>

* <span data-ttu-id="65a08-1252">AppService: добавлена поддержка получения внешнего IP-адреса, используемого для записей DNS типа A ([#2627](https://github.com/Azure/azure-cli/pull/2627)).</span><span class="sxs-lookup"><span data-stu-id="65a08-1252">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="65a08-1253">AppService: добавлена поддержка привязки групповых сертификатов ([#2625](https://github.com/Azure/azure-cli/pull/2625)).</span><span class="sxs-lookup"><span data-stu-id="65a08-1253">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="65a08-1254">AppService: добавлена поддержка профилей для публикации списком ([#2504](https://github.com/Azure/azure-cli/pull/2504)).</span><span class="sxs-lookup"><span data-stu-id="65a08-1254">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="65a08-1255">AppService: добавлен триггер синхронизации с системой управления версиями после настройки ([#2326](https://github.com/Azure/azure-cli/pull/2326)).</span><span class="sxs-lookup"><span data-stu-id="65a08-1255">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="65a08-1256">Data Lake</span><span class="sxs-lookup"><span data-stu-id="65a08-1256">DataLake</span></span>

* <span data-ttu-id="65a08-1257">Первый выпуск модуля Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="65a08-1257">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="65a08-1258">Первый выпуск модуля Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="65a08-1258">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="65a08-1259">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="65a08-1259">DocuemntDB</span></span>

* <span data-ttu-id="65a08-1260">DocumentDB: добавлена поддержка для получения списка строк подключения ([#2580](https://github.com/Azure/azure-cli/pull/2580)).</span><span class="sxs-lookup"><span data-stu-id="65a08-1260">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="65a08-1261">ВМ</span><span class="sxs-lookup"><span data-stu-id="65a08-1261">VM</span></span>

* <span data-ttu-id="65a08-1262">[Вычисления] Добавлена поддержка AppGateway для создания масштабируемого набора виртуальных машин ([#2570](https://github.com/Azure/azure-cli/pull/2570)).</span><span class="sxs-lookup"><span data-stu-id="65a08-1262">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="65a08-1263">[ВМ и VMSS] Улучшена поддержка кэширования диска ([#2522](https://github.com/Azure/azure-cli/pull/2522)).</span><span class="sxs-lookup"><span data-stu-id="65a08-1263">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="65a08-1264">ВМ и VMSS: внедрена логика проверки учетных данных, используемая на портале ([#2537](https://github.com/Azure/azure-cli/pull/2537)).</span><span class="sxs-lookup"><span data-stu-id="65a08-1264">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="65a08-1265">Добавлена поддержка команд wait и --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="65a08-1265">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="65a08-1266">Масштабируемый набор виртуальных машин: добавлена поддержка \* для представления экземпляров на виртуальных машинах в виде списка ([#2467](https://github.com/Azure/azure-cli/pull/2467)).</span><span class="sxs-lookup"><span data-stu-id="65a08-1266">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="65a08-1267">Добавлен параметр --secrets для виртуальной машины и масштабируемого набора виртуальных машин ([#2212}(https://github.com/Azure/azure-cli/pull/2212)).</span><span class="sxs-lookup"><span data-stu-id="65a08-1267">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="65a08-1268">Добавлено разрешение на создание виртуальных машин на основе специализированного образа VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256)).</span><span class="sxs-lookup"><span data-stu-id="65a08-1268">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="65a08-1269">27 февраля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="65a08-1269">February 27, 2017</span></span>

<span data-ttu-id="65a08-1270">Версия 2.0.0</span><span class="sxs-lookup"><span data-stu-id="65a08-1270">Version 2.0.0</span></span>

<span data-ttu-id="65a08-1271">Этот первый общедоступный выпуск Azure CLI 2.0. Общедоступными являются такие командные модули:</span><span class="sxs-lookup"><span data-stu-id="65a08-1271">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="65a08-1272">служба контейнеров (ACS);</span><span class="sxs-lookup"><span data-stu-id="65a08-1272">Container Service (acs)</span></span>
- <span data-ttu-id="65a08-1273">вычисления (в том числе Resource Manager, виртуальная машина, масштабируемые наборы виртуальных машин, управляемые диски);</span><span class="sxs-lookup"><span data-stu-id="65a08-1273">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="65a08-1274">Сеть</span><span class="sxs-lookup"><span data-stu-id="65a08-1274">Networking</span></span>
- <span data-ttu-id="65a08-1275">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="65a08-1275">Storage</span></span>

<span data-ttu-id="65a08-1276">Эти командные модули могут использоваться в рабочих средах. Они поддерживаются стандартными соглашениями Майкрософт об уровне обслуживания. Вы можете отправлять запросы непосредственно в службу технической поддержки Майкрософт или добавлять описание проблем в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/). Вы можете задавать вопросы на [сайте StackOverflow, используя тег azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), или обращаться к группе разработчиков по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Можно отправлять отзывы из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="65a08-1276">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="65a08-1277">Команды в этих модулях стабильны, и предполагается, что в следующих выпусках этой версии Azure CLI их синтаксис не будет меняться.</span><span class="sxs-lookup"><span data-stu-id="65a08-1277">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="65a08-1278">Проверить версию CLI можно с помощью команды `az --version`. В выходных данных указана версия самого интерфейса командной строки (2.0.0 в этом выпуске), версии отдельных командных модулей и используемые вами версии Python и GCC.</span><span class="sxs-lookup"><span data-stu-id="65a08-1278">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

```
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
> <span data-ttu-id="65a08-1279">Некоторые командные модули имеют постфикс b*n* или rc*n*. Эти командные модули все еще находятся на стадии предварительной версии и станут общедоступными в будущем.</span><span class="sxs-lookup"><span data-stu-id="65a08-1279">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="65a08-1280">У нас также есть предварительные ежедневные сборки CLI. Дополнительные сведения см. в инструкциях по [получению ежедневных сборок](https://github.com/Azure/azure-cli#nightly-builds), а также в инструкциях по [настройке среды разработки и участии в написании кода](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="65a08-1280">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="65a08-1281">О проблемах с предварительными ежедневными сборками можно сообщить несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="65a08-1281">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="65a08-1282">добавив информацию о проблемах в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/);</span><span class="sxs-lookup"><span data-stu-id="65a08-1282">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="65a08-1283">Свяжитесь с командой разработчиков ([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)),</span><span class="sxs-lookup"><span data-stu-id="65a08-1283">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="65a08-1284">отправив отзыв из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="65a08-1284">Provide feedback from the command line with the `az feedback` command</span></span>

