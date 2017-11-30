---
title: "Заметки о выпуске Azure CLI 2.0"
description: "Узнайте о последних обновлениях в Azure CLI 2.0"
keywords: "Azure CLI 2.0, заметки о выпуске"
author: sptramer
ms.author: sttramer
manager: douge
ms.date: 04/03/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: ce0428f7-0a59-4e72-9237-d907b171af51
ms.openlocfilehash: 761bd61474e7c72fb2daeb756828f00196b56c3a
ms.sourcegitcommit: 905939cc44764b4d1cc79a9b36c0793f7055a686
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/20/2017
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="4d3dd-104">Заметки о выпуске Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="4d3dd-104">Azure CLI 2.0 release notes</span></span>

## <a name="november-14-2017"></a><span data-ttu-id="4d3dd-105">14 ноября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-105">November 14, 2017</span></span>

<span data-ttu-id="4d3dd-106">Версия 2.0.21</span><span class="sxs-lookup"><span data-stu-id="4d3dd-106">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="4d3dd-107">ACR</span><span class="sxs-lookup"><span data-stu-id="4d3dd-107">ACR</span></span>

* <span data-ttu-id="4d3dd-108">Добавлена поддержка создания веб-перехватчиков в регионах репликации.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-108">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="4d3dd-109">ACS</span><span class="sxs-lookup"><span data-stu-id="4d3dd-109">ACS</span></span>

* <span data-ttu-id="4d3dd-110">В AKS агент теперь называется узлом.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-110">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="4d3dd-111">Параметр `--orchestrator-release` для командлета `acs create` не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-111">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="4d3dd-112">Изменен размер виртуальной машины для AKS по умолчанию на `Standard_D1_v2`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-112">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="4d3dd-113">Исправлена команда `az aks browse` для Windows.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-113">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="4d3dd-114">Исправлена команда `az aks get-credentials` для Windows.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-114">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="4d3dd-115">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4d3dd-115">Appservice</span></span>

* <span data-ttu-id="4d3dd-116">Добавлен источник развертывания `config-zip` для веб-приложений и приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-116">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="4d3dd-117">Добавлен параметр `--docker-container-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-117">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="4d3dd-118">Удален параметр `storage` из параметра `--web-server-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-118">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="4d3dd-119">Улучшены сообщения об ошибках для команды `deployment user set`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-119">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="4d3dd-120">Добавлена поддержка создания приложений-функций Linux</span><span class="sxs-lookup"><span data-stu-id="4d3dd-120">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="4d3dd-121">Фиксированное значение `list-locations`</span><span class="sxs-lookup"><span data-stu-id="4d3dd-121">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="4d3dd-122">Пакетная служба</span><span class="sxs-lookup"><span data-stu-id="4d3dd-122">Batch</span></span>

* <span data-ttu-id="4d3dd-123">Исправлена ошибка в команде создания пула, когда идентификатор ресурса использовался с флагом `--image`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-123">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="4d3dd-124">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="4d3dd-124">Batchai</span></span>

* <span data-ttu-id="4d3dd-125">Добавлен короткий параметр `-s` для параметра `--vm-size` при указании размера виртуальной машины в команде `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-125">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="4d3dd-126">Добавлены аргументы ключа и имени учетной записи хранения в параметры команды `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-126">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="4d3dd-127">Исправлена документация по командам `job list-files` и `job stream-file`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-127">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="4d3dd-128">Добавлен короткий параметр `-r` для параметра `--cluster-name` при указании имени кластера в команде `job create`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-128">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="4d3dd-129">Облако</span><span class="sxs-lookup"><span data-stu-id="4d3dd-129">Cloud</span></span>

* <span data-ttu-id="4d3dd-130">Изменена команда `cloud [register|update]` для предотвращения регистрации облаков, для которых отсутствуют необходимые конечные точки.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-130">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="4d3dd-131">Контейнер</span><span class="sxs-lookup"><span data-stu-id="4d3dd-131">Container</span></span>

* <span data-ttu-id="4d3dd-132">Добавлена поддержка открытия нескольких портов.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-132">Added support to open multiple ports</span></span>
* <span data-ttu-id="4d3dd-133">Добавлена политика перезапуска группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-133">Added container group restart policy</span></span>
* <span data-ttu-id="4d3dd-134">Добавлена поддержка подключения файлового ресурса Azure в качестве тома.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-134">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="4d3dd-135">Обновлена вспомогательная документация.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-135">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="4d3dd-136">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="4d3dd-136">Data Lake Analytics</span></span>

* <span data-ttu-id="4d3dd-137">Изменена команда `[job|account] list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-137">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="4d3dd-138">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="4d3dd-138">Data Lake Store</span></span>

* <span data-ttu-id="4d3dd-139">Изменена команда `account list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-139">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="4d3dd-140">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="4d3dd-140">Extension</span></span>

* <span data-ttu-id="4d3dd-141">Добавлена команда `extension list-available` для отображения официальных расширений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-141">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="4d3dd-142">Добавлен параметр `--name` для команды `extension [add|update]` для установки расширений по имени.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-142">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="4d3dd-143">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="4d3dd-143">IoT</span></span>

* <span data-ttu-id="4d3dd-144">Добавлена поддержка центров сертификации (ЦС) и цепочек сертификатов.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-144">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="4d3dd-145">Монитор</span><span class="sxs-lookup"><span data-stu-id="4d3dd-145">Monitor</span></span>

* <span data-ttu-id="4d3dd-146">Добавлены команды `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-146">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="4d3dd-147">Сеть</span><span class="sxs-lookup"><span data-stu-id="4d3dd-147">Network</span></span>

* <span data-ttu-id="4d3dd-148">Добавлена поддержка DNS-записей типа CAA.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-148">Added support for CAA DNS records</span></span>
* <span data-ttu-id="4d3dd-149">Исправлена проблема, когда конечные точки могли не обновляться с помощью команды `traffic-manager profile update`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-149">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="4d3dd-150">Исправлена проблема, когда команда `vnet update --dns-servers` не работала в зависимости от способа создания виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-150">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="4d3dd-151">Исправлена проблема, когда относительные DNS-имена неправильно импортировались с помощью команды `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-151">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="4d3dd-152">Резервирование</span><span class="sxs-lookup"><span data-stu-id="4d3dd-152">Reservations</span></span>

* <span data-ttu-id="4d3dd-153">Первоначальный выпуск предварительной версии</span><span class="sxs-lookup"><span data-stu-id="4d3dd-153">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="4d3dd-154">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4d3dd-154">Resource</span></span>

* <span data-ttu-id="4d3dd-155">Добавлена поддержка идентификаторов ресурсов для блокировок на уровне ресурсов и параметра `--resource`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-155">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="4d3dd-156">SQL</span><span class="sxs-lookup"><span data-stu-id="4d3dd-156">SQL</span></span>

* <span data-ttu-id="4d3dd-157">Добавлен параметр `--ignore-missing-vnet-service-endpoint` для команды `sql server vnet-rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-157">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="4d3dd-158">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4d3dd-158">Storage</span></span>

* <span data-ttu-id="4d3dd-159">Изменена команда `storage account create` для использования номера SKU `Standard_RAGRS` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-159">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="4d3dd-160">Исправлены ошибки при обработке имени файла или большого двоичного объекта, содержащего символы, отличные от ASCII.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-160">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="4d3dd-161">Исправлена ошибка, препятствующая использованию параметра `--source-uri` с командой `storage [blob|file] copy start-batch`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-161">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="4d3dd-162">Добавлены команды для удаления нескольких объектов с помощью команды `storage [blob|file] delete-batch`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-162">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="4d3dd-163">Исправлена проблема с включением метрик с помощью команды `storage metrics update`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-163">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="4d3dd-164">Исправлена проблема с файлами более 200 ГБ при использовании команды `storage blob upload-batch`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-164">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="4d3dd-165">Исправлена проблема, когда параметры `--bypass` и `--default-action` игнорировались командой `storage account [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-165">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="4d3dd-166">ВМ</span><span class="sxs-lookup"><span data-stu-id="4d3dd-166">VM</span></span>

* <span data-ttu-id="4d3dd-167">Исправлена ошибка с командой `vmss create`, препятствующая использованию уровня `Basic`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-167">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="4d3dd-168">Добавлены аргументы `--plan` для команды `[vm|vmss] create` для пользовательских образов с информацией о выставлении счетов.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-168">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="4d3dd-169">Добавлены команды `vm secret `[add|remove|list]\`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-169">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="4d3dd-170">Команда `vm format-secret` переименована в `vm secret format`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-170">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="4d3dd-171">Добавлен аргумент `--encrypt format` для команды `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="4d3dd-171">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="4d3dd-172">24 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-172">October 24, 2017</span></span>

<span data-ttu-id="4d3dd-173">Версия 2.0.20</span><span class="sxs-lookup"><span data-stu-id="4d3dd-173">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="4d3dd-174">Core</span><span class="sxs-lookup"><span data-stu-id="4d3dd-174">Core</span></span>

* <span data-ttu-id="4d3dd-175">Обновление `2017-03-09-profile` для использования API `MGMT_STORAGE` версии `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="4d3dd-175">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="4d3dd-176">ACR</span><span class="sxs-lookup"><span data-stu-id="4d3dd-176">ACR</span></span>

* <span data-ttu-id="4d3dd-177">Обновление службы управления ресурсами для указания API версии `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="4d3dd-177">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="4d3dd-178">Изменение номера SKU BYOS-хранилища на "Классический"</span><span class="sxs-lookup"><span data-stu-id="4d3dd-178">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="4d3dd-179">Переименование номеров SKU реестра на "Базовый", "Стандартный" и "Премиум"</span><span class="sxs-lookup"><span data-stu-id="4d3dd-179">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="4d3dd-180">ACS</span><span class="sxs-lookup"><span data-stu-id="4d3dd-180">ACS</span></span>

* <span data-ttu-id="4d3dd-181">[ПРЕДВАРИЕТЛЬНАЯ ВЕРСИЯ] Добавление команд `az aks`</span><span class="sxs-lookup"><span data-stu-id="4d3dd-181">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="4d3dd-182">Исправление Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="4d3dd-182">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="4d3dd-183">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4d3dd-183">Appservice</span></span>

* <span data-ttu-id="4d3dd-184">Исправление проблемы с недопустимыми скачанными журналами `webapp`</span><span class="sxs-lookup"><span data-stu-id="4d3dd-184">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="4d3dd-185">Компонент</span><span class="sxs-lookup"><span data-stu-id="4d3dd-185">Component</span></span>

* <span data-ttu-id="4d3dd-186">Добавление более понятного сообщения об устаревании для всех установщиков, а также запроса на подтверждение</span><span class="sxs-lookup"><span data-stu-id="4d3dd-186">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="4d3dd-187">Монитор</span><span class="sxs-lookup"><span data-stu-id="4d3dd-187">Monitor</span></span>

* <span data-ttu-id="4d3dd-188">Добавлены команды `action-group`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-188">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="4d3dd-189">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4d3dd-189">Resource</span></span>

* <span data-ttu-id="4d3dd-190">Исправление несовместимости с самой последней версии зависимости msrest в `group export`</span><span class="sxs-lookup"><span data-stu-id="4d3dd-190">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="4d3dd-191">Исправление `policy assignment create` для работы с определениями встроенных политик и наборов политик</span><span class="sxs-lookup"><span data-stu-id="4d3dd-191">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="4d3dd-192">ВМ</span><span class="sxs-lookup"><span data-stu-id="4d3dd-192">VM</span></span>

* <span data-ttu-id="4d3dd-193">Добавлен аргумент `--accelerated-networking` для команды `vmss create`</span><span class="sxs-lookup"><span data-stu-id="4d3dd-193">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="4d3dd-194">9 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-194">October 9, 2017</span></span>

<span data-ttu-id="4d3dd-195">Версия 2.0.19</span><span class="sxs-lookup"><span data-stu-id="4d3dd-195">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="4d3dd-196">Core</span><span class="sxs-lookup"><span data-stu-id="4d3dd-196">Core</span></span>

* <span data-ttu-id="4d3dd-197">В Azure Stack добавлена обработка URL-адресов центра ADFS с завершающей косой чертой.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-197">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="4d3dd-198">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4d3dd-198">Appservice</span></span>

* <span data-ttu-id="4d3dd-199">Добавлена возможность общего обновления с помощью новой команды `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-199">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="4d3dd-200">Пакетная служба</span><span class="sxs-lookup"><span data-stu-id="4d3dd-200">Batch</span></span>

* <span data-ttu-id="4d3dd-201">Обновление до пакета SDK для пакетной службы версии 4.0.0</span><span class="sxs-lookup"><span data-stu-id="4d3dd-201">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="4d3dd-202">Обновлен параметр `--image` для команды VirtualMachineConfiguration, обеспечивающий поддержку ссылок на образы ARM в дополнение к publish:offer:sku:version.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-202">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="4d3dd-203">Добавлена поддержка новой модели расширений CLI для команд расширений пакетной службы.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-203">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="4d3dd-204">Удалена поддержка пакетной службы для модели компонентов.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-204">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="4d3dd-205">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="4d3dd-205">Batchai</span></span>

* <span data-ttu-id="4d3dd-206">Исходный выпуск модуля искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="4d3dd-206">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="4d3dd-207">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="4d3dd-207">Keyvault</span></span>

* <span data-ttu-id="4d3dd-208">Исправлена проблема с аутентификацией Key Vault при использовании ADFS в Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-208">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="4d3dd-209">(#4448)</span><span class="sxs-lookup"><span data-stu-id="4d3dd-209">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="4d3dd-210">Сеть</span><span class="sxs-lookup"><span data-stu-id="4d3dd-210">Network</span></span>

* <span data-ttu-id="4d3dd-211">Аргумент `--server` для `application-gateway address-pool create` изменен на необязательный (разрешено использование пустых пулов адресов).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-211">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="4d3dd-212">Обновлен элемент `traffic-manager` для поддержки последних функций.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-212">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="4d3dd-213">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4d3dd-213">Resource</span></span>

* <span data-ttu-id="4d3dd-214">Добавлена поддержка параметров `--resource-group/-g` для изменения имени группы ресурсов на `group`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-214">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="4d3dd-215">Добавлены команды для `account lock` для работы с блокировками на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-215">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="4d3dd-216">Добавлены команды для `group lock` для работы с блокировками на уровне группы.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-216">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="4d3dd-217">Добавлены команды для `resource lock` для работы с блокировками на уровне ресурса.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-217">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="4d3dd-218">SQL</span><span class="sxs-lookup"><span data-stu-id="4d3dd-218">Sql</span></span>

* <span data-ttu-id="4d3dd-219">Добавлена поддержка SQL TDE и BYOK TDE.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-219">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="4d3dd-220">Добавлена команда `db list-deleted` и параметр `db restore --deleted-time` для поиска и восстановления удаленных баз данных.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-220">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="4d3dd-221">Добавлено `db op list` и `db op cancel` для отображения и отмены выполняющихся операций в базе данных.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-221">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="4d3dd-222">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4d3dd-222">Storage</span></span>

* <span data-ttu-id="4d3dd-223">Добавлена поддержка моментальных снимков файловых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-223">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="4d3dd-224">Виртуальные машины</span><span class="sxs-lookup"><span data-stu-id="4d3dd-224">Vm</span></span>

* <span data-ttu-id="4d3dd-225">Исправлена ошибка в команде `vm show`, когда использование `-d` вызывало сбой отсутствующих частных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-225">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="4d3dd-226">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка последовательного обновления для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-226">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="4d3dd-227">Добавлена поддержка обновления параметров шифрования с помощью команды `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-227">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="4d3dd-228">Добавлен параметр `--os-disk-size-gb` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-228">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="4d3dd-229">Добавлен параметр `--license-type` для команды `vmss create` (для Windows).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-229">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="4d3dd-230">22 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-230">September 22, 2017</span></span>

<span data-ttu-id="4d3dd-231">Версия 2.0.18</span><span class="sxs-lookup"><span data-stu-id="4d3dd-231">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="4d3dd-232">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4d3dd-232">Resource</span></span>

* <span data-ttu-id="4d3dd-233">Добавлена поддержка отображения определений встроенных политик</span><span class="sxs-lookup"><span data-stu-id="4d3dd-233">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="4d3dd-234">Добавлена поддержка параметра mode для создания определения политик</span><span class="sxs-lookup"><span data-stu-id="4d3dd-234">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="4d3dd-235">Добавлена поддержка шаблонов и определений пользовательского интерфейса для команды `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="4d3dd-235">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="4d3dd-236">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ] Изменен тип ресурса `managedapp` с `appliances` на `applications` и с `applianceDefinitions` на `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="4d3dd-236">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="4d3dd-237">Сеть</span><span class="sxs-lookup"><span data-stu-id="4d3dd-237">Network</span></span>

* <span data-ttu-id="4d3dd-238">Добавлена поддержка зоны доступности для подкоманд `network lb` и `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="4d3dd-238">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="4d3dd-239">Добавлена поддержка IPv6 (пиринг Майкрософт) для `express-route`</span><span class="sxs-lookup"><span data-stu-id="4d3dd-239">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="4d3dd-240">Добавлены команды группы безопасности приложения `asg`</span><span class="sxs-lookup"><span data-stu-id="4d3dd-240">Added `asg` application security group commands</span></span>
* <span data-ttu-id="4d3dd-241">Добавлен аргумент `--application-security-groups` для команды `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="4d3dd-241">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="4d3dd-242">Добавлены аргументы `--source-asgs` и `--destination-asgs` для команды `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4d3dd-242">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="4d3dd-243">Добавлены аргументы `--ddos-protection` и `--vm-protection` для команды `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4d3dd-243">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="4d3dd-244">Добавлены команды `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-244">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="4d3dd-245">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4d3dd-245">Storage</span></span>

* <span data-ttu-id="4d3dd-246">Исправлена проблема, когда команды `storage account network-rule` могут не работать после обновления пакета SDK</span><span class="sxs-lookup"><span data-stu-id="4d3dd-246">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="4d3dd-247">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="4d3dd-247">Eventgrid</span></span>

* <span data-ttu-id="4d3dd-248">Обновлен пакет SDK Python для службы "Сетка событий Azure" для использования новой версии API 2017-09-15-preview</span><span class="sxs-lookup"><span data-stu-id="4d3dd-248">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="4d3dd-249">SQL</span><span class="sxs-lookup"><span data-stu-id="4d3dd-249">SQL</span></span>

* <span data-ttu-id="4d3dd-250">Аргумент `--resource-group` для команды `sql server list` сделан необязательным.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-250">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="4d3dd-251">Если он не указан, возвращаются все серверы SQL Server в подписке</span><span class="sxs-lookup"><span data-stu-id="4d3dd-251">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="4d3dd-252">Добавлен параметр `--no-wait` для команд `db [create|copy|restore|update|replica create|create|update]` и `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4d3dd-252">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="4d3dd-253">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="4d3dd-253">Keyvault</span></span>

* <span data-ttu-id="4d3dd-254">Добавлена поддержка команд хранилища ключей за прокси-сервером</span><span class="sxs-lookup"><span data-stu-id="4d3dd-254">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="4d3dd-255">ВМ</span><span class="sxs-lookup"><span data-stu-id="4d3dd-255">VM</span></span>

* <span data-ttu-id="4d3dd-256">Добавлена поддержка зоны доступности для команды `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="4d3dd-256">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="4d3dd-257">Исправлена проблема, когда использование аргумента `--app-gateway ID` с командой `vmss create` приводило к сбою</span><span class="sxs-lookup"><span data-stu-id="4d3dd-257">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="4d3dd-258">Добавлен аргумент `--asgs` для команды `vm create`</span><span class="sxs-lookup"><span data-stu-id="4d3dd-258">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="4d3dd-259">Добавлена поддержка выполнения команд на виртуальных машинах с помощью команды `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="4d3dd-259">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="4d3dd-260">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка шифрования диска VMSS с помощью команды `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="4d3dd-260">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="4d3dd-261">Добавлена поддержка обслуживания виртуальных машин с помощью команды `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="4d3dd-261">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="4d3dd-262">ACS</span><span class="sxs-lookup"><span data-stu-id="4d3dd-262">ACS</span></span>

* <span data-ttu-id="4d3dd-263">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлен аргумент `--orchestrator-release` для команды `acs create` для регионов служб ACS (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="4d3dd-263">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="4d3dd-264">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4d3dd-264">Appservice</span></span>

* <span data-ttu-id="4d3dd-265">Добавлена возможность обновлять и отображать параметры аутентификации с помощью команды `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="4d3dd-265">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="4d3dd-266">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="4d3dd-266">Backup</span></span>

* <span data-ttu-id="4d3dd-267">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-267">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="4d3dd-268">11 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-268">September 11, 2017</span></span>

<span data-ttu-id="4d3dd-269">Версия 2.0.17</span><span class="sxs-lookup"><span data-stu-id="4d3dd-269">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="4d3dd-270">Core</span><span class="sxs-lookup"><span data-stu-id="4d3dd-270">Core</span></span>

* <span data-ttu-id="4d3dd-271">Включен командный модуль для настройки собственного идентификатора корреляции в телеметрии.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-271">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="4d3dd-272">Исправлена проблема с дампом JSON, когда для телеметрии настроен режим диагностики.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-272">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="4d3dd-273">ACS</span><span class="sxs-lookup"><span data-stu-id="4d3dd-273">Acs</span></span>

* <span data-ttu-id="4d3dd-274">Добавлена команда `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-274">Added `acs list-locations` command</span></span>
* <span data-ttu-id="4d3dd-275">Для `ssh-key-file` предоставляется ожидаемое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-275">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="4d3dd-276">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4d3dd-276">Appservice</span></span>

* <span data-ttu-id="4d3dd-277">Добавлена возможность создавать веб-приложения в группе ресурсов в рамках плана службы, отличной от активной.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-277">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="4d3dd-278">CDN</span><span class="sxs-lookup"><span data-stu-id="4d3dd-278">CDN</span></span>

* <span data-ttu-id="4d3dd-279">Исправлена ошибка "CustomDomain не пригоден к итерации" для `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-279">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`.</span></span>

### <a name="extension"></a><span data-ttu-id="4d3dd-280">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="4d3dd-280">Extension</span></span>

* <span data-ttu-id="4d3dd-281">Первый выпуск.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-281">Initial Release.</span></span>

### <a name="keyvault"></a><span data-ttu-id="4d3dd-282">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="4d3dd-282">Keyvault</span></span>

* <span data-ttu-id="4d3dd-283">Исправлена проблема с зависимостью разрешений от регистра для `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-283">Fixed issue where permissions were case sensitive for `keyvault set-policy`.</span></span>

### <a name="network"></a><span data-ttu-id="4d3dd-284">Сеть</span><span class="sxs-lookup"><span data-stu-id="4d3dd-284">Network</span></span>

* <span data-ttu-id="4d3dd-285">Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-285">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="4d3dd-286">Аргумент `--private-access-services` переименован в `--service-endpoints` для команды `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-286">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="4d3dd-287">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-287">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="4d3dd-288">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-288">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="4d3dd-289">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-289">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="4d3dd-290">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4d3dd-290">Resource</span></span>

* <span data-ttu-id="4d3dd-291">Разрешена передача в определениях параметров политики ресурсов в командах `policy definition create` и `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-291">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="4d3dd-292">Разрешена передача значений параметров для команды `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-292">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="4d3dd-293">Разрешена передача JSON или файла для всех параметров.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-293">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="4d3dd-294">Версия API изменена на более позднюю.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-294">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="4d3dd-295">SQL</span><span class="sxs-lookup"><span data-stu-id="4d3dd-295">SQL</span></span>

* <span data-ttu-id="4d3dd-296">Добавлены команды `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-296">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="4d3dd-297">ВМ</span><span class="sxs-lookup"><span data-stu-id="4d3dd-297">VM</span></span>

* <span data-ttu-id="4d3dd-298">Исправлено: не назначать доступ, если `--scope` не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-298">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="4d3dd-299">Исправлено: использование тех же расширений имен, что и для портала.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-299">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="4d3dd-300">Удалено `subscription` из выходных данных `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-300">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="4d3dd-301">Исправлено: номер SKU хранилища `[vm|vmss] create` неприменим для дисков данных с образом.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-301">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="4d3dd-302">Исправлено: `vm format-secret --secrets` не принимает идентификаторы, разделенные строками.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-302">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="4d3dd-303">31 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-303">August 31, 2017</span></span>

<span data-ttu-id="4d3dd-304">Версия 2.0.16</span><span class="sxs-lookup"><span data-stu-id="4d3dd-304">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="4d3dd-305">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="4d3dd-305">Keyvault</span></span>

* <span data-ttu-id="4d3dd-306">Исправлена ошибка при попытке автоматически разрешить шифрование секрета с помощью `secret download`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-306">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="4d3dd-307">Sf</span><span class="sxs-lookup"><span data-stu-id="4d3dd-307">Sf</span></span>

* <span data-ttu-id="4d3dd-308">Объявлены неподдерживаемыми все команды; вместо них используется Service Fabric CLI (sfctl).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-308">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="4d3dd-309">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4d3dd-309">Storage</span></span>

* <span data-ttu-id="4d3dd-310">Исправлена проблема, когда учетные записи хранения нельзя было создавать в регионах, которые не поддерживают функцию NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-310">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="4d3dd-311">Определение типа и кодировки содержимого во время передачи больших двоичных объектов и файла, если оба свойства не указаны.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-311">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="4d3dd-312">28 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-312">August 28, 2017</span></span>

<span data-ttu-id="4d3dd-313">Версия 2.0.15</span><span class="sxs-lookup"><span data-stu-id="4d3dd-313">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="4d3dd-314">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="4d3dd-314">CLI</span></span>

* <span data-ttu-id="4d3dd-315">К параметру `--version` добавлено юридическое примечание.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-315">Added legal note to `--version`.</span></span>

### <a name="acs"></a><span data-ttu-id="4d3dd-316">ACS</span><span class="sxs-lookup"><span data-stu-id="4d3dd-316">ACS</span></span>

* <span data-ttu-id="4d3dd-317">Исправлены регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-317">Corrected preview regions.</span></span>
* <span data-ttu-id="4d3dd-318">Правильно отформатирован параметр по умолчанию `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-318">Formatted default `dns_name_prefix` properly.</span></span>
* <span data-ttu-id="4d3dd-319">Оптимизированы выходные данные команды ACS.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-319">Optimized acs command output.</span></span>

### <a name="appservice"></a><span data-ttu-id="4d3dd-320">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4d3dd-320">Appservice</span></span>

* <span data-ttu-id="4d3dd-321">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправлены несоответствия в выходных данных `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-321">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="4d3dd-322">Добавлен новый псевдоним `-i` в команду `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-322">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="4d3dd-323">Предоставлена команда `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-323">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="4d3dd-324">Предоставлены новые аргументы команды `az webapp delete`, которые позволяют сохранить план службы приложений, метрики и данные регистрации DNS.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-324">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="4d3dd-325">Исправление. Параметры слота определяются правильно.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-325">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="4d3dd-326">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="4d3dd-326">IoT</span></span>

* <span data-ttu-id="4d3dd-327">Исправление 3934. При создании политики существующие политики больше не удаляются.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-327">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="4d3dd-328">Сеть</span><span class="sxs-lookup"><span data-stu-id="4d3dd-328">Network</span></span>

* <span data-ttu-id="4d3dd-329">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-329">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="4d3dd-330">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--private-access-services` переименован в `--service-endpoints` в командах `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-330">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="4d3dd-331">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-331">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="4d3dd-332">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-332">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="4d3dd-333">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-333">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="4d3dd-334">Профиль</span><span class="sxs-lookup"><span data-stu-id="4d3dd-334">Profile</span></span>

* <span data-ttu-id="4d3dd-335">Предоставлены параметры `--msi` и `--msi-port` для входа с использованием удостоверения виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-335">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="4d3dd-336">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="4d3dd-336">Service Fabric</span></span>

* <span data-ttu-id="4d3dd-337">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-337">Preview release</span></span>
* <span data-ttu-id="4d3dd-338">Упрощены правила реестра для паролей и имен пользователя для команды.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-338">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="4d3dd-339">Исправлена строка для ввода пароля пользователем даже после передачи параметра.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-339">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="4d3dd-340">Добавлена поддержка пустого значения `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-340">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="4d3dd-341">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4d3dd-341">Storage</span></span>

* <span data-ttu-id="4d3dd-342">Появилась возможность задавать уровень большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-342">Enabled setting blob tier</span></span>
* <span data-ttu-id="4d3dd-343">Добавлены аргументы `--bypass` и `--default-action` в командах `storage account [create|update]` для поддержки туннелирования службы.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-343">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="4d3dd-344">Добавлены команды для добавления правил виртуальной сети и правил на основе IP-адресов в `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-344">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>  
* <span data-ttu-id="4d3dd-345">Разрешено шифрование службы с управляемым пользователем ключом.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-345">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="4d3dd-346">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--encryption` переименован в `--encryption-services` в команде `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-346">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="4d3dd-347">Исправление 4220. Несоответствие синтаксиса `az storage account update encryption`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-347">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="4d3dd-348">ВМ</span><span class="sxs-lookup"><span data-stu-id="4d3dd-348">VM</span></span>

* <span data-ttu-id="4d3dd-349">Исправлена проблема, из-за которой для команды `vmss get-instance-view` отображались лишние и неправильные сведения при использовании параметра `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-349">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="4d3dd-350">Добавлена поддержка параметра `--lb-sku` в команде `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-350">Added support for `--lb-sku` to `vmss create`:</span></span> 
* <span data-ttu-id="4d3dd-351">Из черного списка имен администраторов для команд `[vm|vmss] create` удалены имена людей.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-351">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span> 
* <span data-ttu-id="4d3dd-352">Исправлена проблема, из-за которой команда `[vm|vmss] create` выдавала ошибку, если из образа не удавалось извлечь сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-352">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="4d3dd-353">Исправлена проблема, которая приводила к сбою при создании масштабируемого набора виртуальных машин с внутренней подсистемой балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-353">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="4d3dd-354">Исправлена проблема, из-за которой аргумент `--no-wait` не работал с командой `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-354">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="4d3dd-355">15 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-355">August 15, 2017</span></span>

<span data-ttu-id="4d3dd-356">Версия 2.0.14</span><span class="sxs-lookup"><span data-stu-id="4d3dd-356">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="4d3dd-357">ACS</span><span class="sxs-lookup"><span data-stu-id="4d3dd-357">ACS</span></span>

* <span data-ttu-id="4d3dd-358">Исправлен номер порта sshMaster0 для Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-358">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="4d3dd-359">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4d3dd-359">Appservice</span></span>

* <span data-ttu-id="4d3dd-360">Исправлено исключение при создании веб-приложения Linux на основе Git.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-360">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="4d3dd-361">Служба "Сетка событий Azure"</span><span class="sxs-lookup"><span data-stu-id="4d3dd-361">Event Grid</span></span>

* <span data-ttu-id="4d3dd-362">Добавлены зависимости пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-362">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="4d3dd-363">11 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-363">August 11, 2017</span></span>

<span data-ttu-id="4d3dd-364">Версия 2.0.13</span><span class="sxs-lookup"><span data-stu-id="4d3dd-364">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="4d3dd-365">ACS</span><span class="sxs-lookup"><span data-stu-id="4d3dd-365">ACS</span></span>

* <span data-ttu-id="4d3dd-366">Добавлены дополнительные регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-366">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="4d3dd-367">Пакетная служба</span><span class="sxs-lookup"><span data-stu-id="4d3dd-367">Batch</span></span>

* <span data-ttu-id="4d3dd-368">Пакет SDK для пакетной службы обновлен до версии 3.1.0, а пакет SDK для управления пакетной службой — до версии 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-368">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="4d3dd-369">Добавлена новая команда для отображения количества задач в задании.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-369">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="4d3dd-370">Исправлена ошибка при обработке URL-адреса SAS файла ресурсов.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-370">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="4d3dd-371">Для конечной точки учетной записи пакетной службы теперь поддерживается дополнительный префикс https://.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-371">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="4d3dd-372">Поддерживается добавление к заданию списков, содержащих более 100 задач.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-372">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="4d3dd-373">Добавлено ведение журнала отладки при загрузке командного модуля расширений.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-373">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="4d3dd-374">Компонент</span><span class="sxs-lookup"><span data-stu-id="4d3dd-374">Component</span></span>

* <span data-ttu-id="4d3dd-375">Добавлено предупреждение о прекращении поддержки в команды az component.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-375">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="4d3dd-376">Контейнер</span><span class="sxs-lookup"><span data-stu-id="4d3dd-376">Container</span></span>

* <span data-ttu-id="4d3dd-377">`create`. Исправлена проблема, из-за которой запрещалось использовать знак равенства в переменной среды.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-377">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="4d3dd-378">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="4d3dd-378">Data Lake Store</span></span>

* <span data-ttu-id="4d3dd-379">Включен индикатор хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-379">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="4d3dd-380">Служба "Сетка событий Azure"</span><span class="sxs-lookup"><span data-stu-id="4d3dd-380">Event Grid</span></span>

* <span data-ttu-id="4d3dd-381">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="4d3dd-381">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="4d3dd-382">Сеть</span><span class="sxs-lookup"><span data-stu-id="4d3dd-382">Network</span></span>

* <span data-ttu-id="4d3dd-383">`lb`. Исправлена проблема, из-за которой некоторые имена дочерних ресурсов не разрешались правильно, если не были указаны.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-383">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="4d3dd-384">`application-gateway {subresource} delete`. Исправлена проблема, из-за которой не учитывался параметр `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-384">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="4d3dd-385">`application-gateway http-settings update`. Исправлена проблема, из-за которой не удавалось отключить параметр `--connection-draining-timeout`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-385">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="4d3dd-386">Исправлена проблема с непредвиденным аргументом ключевого слова `sa_data_size_kilobyes` при использовании с командой `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-386">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="4d3dd-387">Профиль</span><span class="sxs-lookup"><span data-stu-id="4d3dd-387">Profile</span></span>

* <span data-ttu-id="4d3dd-388">`account list`. Добавлен параметр `--refresh` для синхронизации последних подписок с сервером.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-388">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="4d3dd-389">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4d3dd-389">Storage</span></span>

* <span data-ttu-id="4d3dd-390">Включено обновление учетной записи хранения с помощью удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-390">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="4d3dd-391">ВМ</span><span class="sxs-lookup"><span data-stu-id="4d3dd-391">VM</span></span>

* <span data-ttu-id="4d3dd-392">`availability-set`. Предоставлено число доменов сбоя при преобразовании.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-392">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="4d3dd-393">Предоставлена команда `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-393">Exposed `list-skus` command</span></span>
* <span data-ttu-id="4d3dd-394">Поддерживается назначение удостоверений без создания назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-394">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="4d3dd-395">При подключении дисков данных применяется номер SKU хранилища.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-395">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="4d3dd-396">Удалено используемое по умолчанию имя диска ОС и номер SKU хранилища при использовании управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-396">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="4d3dd-397">28 июля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-397">July 28, 2017</span></span>

<span data-ttu-id="4d3dd-398">Версия 2.0.12</span><span class="sxs-lookup"><span data-stu-id="4d3dd-398">Version 2.0.12</span></span>

* <span data-ttu-id="4d3dd-399">Добавлены команды для контейнеров.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-399">Added container commands</span></span>
* <span data-ttu-id="4d3dd-400">Добавлены модули выставления счетов и потребления ресурсов.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-400">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="4d3dd-401">Core</span><span class="sxs-lookup"><span data-stu-id="4d3dd-401">Core</span></span>

* <span data-ttu-id="4d3dd-402">Вывод сведений о пакетах SDK для проверки подлинности субъектов-служб с помощью сертификатов.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-402">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="4d3dd-403">Исправлены исключения в ходе выполнения развертывания.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-403">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="4d3dd-404">Для создания клиента подписки используется конечная точка ARM текущего облака.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-404">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="4d3dd-405">Улучшена параллельная обработка файла clouds.config (3636).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-405">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="4d3dd-406">Обновление идентификатора клиентского запроса при каждом выполнении команды.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-406">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="4d3dd-407">Создание клиентов подписки с правильным профилем SDK (3635).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-407">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="4d3dd-408">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-408">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="4d3dd-409">Добавлена поддержка выбора полей вывода в таблице с помощью запроса jmespath (3581).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-409">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="4d3dd-410">Улучшено отключение аргументов анализа и добавлено ведение журналов с помощью жестов (3434).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-410">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="4d3dd-411">Создание клиентов подписки с правильным профилем SDK.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-411">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="4d3dd-412">Перемещение всех существующих файлов записи в последнюю папку.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-412">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="4d3dd-413">Исправлена идемпотентность при создании виртуальной машины или масштабируемого набора виртуальных машин (3586).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-413">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="4d3dd-414">В путях команд больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-414">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="4d3dd-415">В определенных параметрах логического типа больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-415">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="4d3dd-416">Поддержка входа на локальный сервер AD FS, например Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-416">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="4d3dd-417">Исправлена параллельная запись в файл clouds.config (3255).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-417">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="4d3dd-418">ACR</span><span class="sxs-lookup"><span data-stu-id="4d3dd-418">ACR</span></span>

* <span data-ttu-id="4d3dd-419">Добавлена команда `show-usage` для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-419">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="4d3dd-420">Поддержка обновления номера SKU для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-420">Support SKU update for managed registries</span></span>
* <span data-ttu-id="4d3dd-421">Добавлены управляемые реестры с управляемыми номерами SKU.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-421">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="4d3dd-422">Добавлены веб-перехватчики для управляемых реестров с использованием модуля для команды acr webhook.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-422">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="4d3dd-423">Добавлена проверка подлинности с помощью AAD с использованием команды acr login.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-423">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="4d3dd-424">Добавлена команда delete для репозиториев, манифестов и тегов Docker.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-424">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="4d3dd-425">ACS</span><span class="sxs-lookup"><span data-stu-id="4d3dd-425">ACS</span></span>

* <span data-ttu-id="4d3dd-426">Поддержка API версии 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-426">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="4d3dd-427">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4d3dd-427">Appservice</span></span>

* <span data-ttu-id="4d3dd-428">Исправлена ошибка, из-за которой команда вывода списка в веб-приложениях Linux не возвращала данные.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-428">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="4d3dd-429">Поддержка извлечения учетных данных из ACR.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-429">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="4d3dd-430">Удаление всех команд группы `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-430">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="4d3dd-431">Создание масок паролей для реестров Docker из выходных данных команды (3656).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-431">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="4d3dd-432">Обеспечено использование браузера по умолчанию в macOS без ошибок (3623).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-432">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="4d3dd-433">Улучшена справка по командам `webapp log tail` и `webapp log download` (3624).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-433">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="4d3dd-434">Предоставлена команда `traffic-routing` для настройки статической маршрутизации (3566).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-434">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="4d3dd-435">Добавлены исправления, связанные с надежностью, при настройке системы управления версиями (3245).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-435">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="4d3dd-436">Удален неподдерживаемый аргумент `--node-version` из функции `webapp config update` для веб-приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-436">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="4d3dd-437">Вместо него используется `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-437">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="4d3dd-438">Пакетная служба</span><span class="sxs-lookup"><span data-stu-id="4d3dd-438">Batch</span></span>

* <span data-ttu-id="4d3dd-439">Пакеты SDK для пакетной службы обновлены до версии 3.0.0 с поддержкой низкоприоритетных виртуальных машин в пулах.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-439">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="4d3dd-440">Параметр команды `pool create` переименован с `--target-dedicated` в `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-440">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="4d3dd-441">Для команды `pool create` добавлены параметры `--target-low-priority-nodes` и `--application-licenses`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-441">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="4d3dd-442">CDN</span><span class="sxs-lookup"><span data-stu-id="4d3dd-442">CDN</span></span>

* <span data-ttu-id="4d3dd-443">Предоставлено улучшенное сообщение об ошибке для команды `cdn endpoint list`, которое отображается, если заданный параметром `--profile-name` профиль не существует.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-443">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist.</span></span>

### <a name="cloud"></a><span data-ttu-id="4d3dd-444">Облако</span><span class="sxs-lookup"><span data-stu-id="4d3dd-444">Cloud</span></span>

* <span data-ttu-id="4d3dd-445">Формат версии API конечной точки метаданных облака изменен на следующий: ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-445">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="4d3dd-446">Конечная точка коллекции не является обязательной.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-446">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="4d3dd-447">Поддерживается регистрация облака только с конечной точкой диспетчера ARM.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-447">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="4d3dd-448">Предоставлен параметр в команде `cloud set` для выбора профиля при выборе текущего облака.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-448">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="4d3dd-449">Предоставлен параметр `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-449">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4d3dd-450">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="4d3dd-450">CosmosDB</span></span>

* <span data-ttu-id="4d3dd-451">Внесены исправления, которые позволяют создавать коллекцию с пользовательским ключом секции.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-451">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="4d3dd-452">Добавлена поддержка срока жизни по умолчанию для коллекции.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-452">Added support for collection default TTL.</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="4d3dd-453">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="4d3dd-453">Data Lake Analytics</span></span>

* <span data-ttu-id="4d3dd-454">Добавлены команды для управления политикой вычислений в разделе `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-454">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="4d3dd-455">Добавлена команда `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-455">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="4d3dd-456">Добавлена команда `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-456">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="4d3dd-457">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="4d3dd-457">Data Lake Store</span></span>

* <span data-ttu-id="4d3dd-458">Добавлена поддержка смены ключей пользовательского хранилища ключей в `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-458">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="4d3dd-459">Обновлена версия пакета SDK для базовой файловой системы Data Lake Store из-за проблем с производительностью.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-459">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="4d3dd-460">Добавлена команда `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-460">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="4d3dd-461">Эта команда пытается активировать пользовательское хранилище ключей, предназначенное для шифрования данных в учетной записи Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-461">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="4d3dd-462">Интерактивный режим</span><span class="sxs-lookup"><span data-stu-id="4d3dd-462">Interactive</span></span>

* <span data-ttu-id="4d3dd-463">Улучшено время запуска с помощью кэшированных команд.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-463">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="4d3dd-464">Увеличено тестовое покрытие.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-464">Increased test coverage</span></span>
* <span data-ttu-id="4d3dd-465">Расширены возможности жеста "?", которые позволяют также вставить его в следующую команду.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-465">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="4d3dd-466">Исправлены ошибки с интерактивными функциями в предварительной версии профиля 2017-03-09 (3587).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-466">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="4d3dd-467">Разрешено использовать `--version` в качестве параметра в интерактивном режиме (3645).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-467">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="4d3dd-468">В интерактивном режиме больше не возникают ошибки при выполнении проверки (3570).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-468">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="4d3dd-469">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-469">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="4d3dd-470">Добавлен флаг `--progress`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-470">Added `--progress` flag</span></span>
* <span data-ttu-id="4d3dd-471">Из вариантов завершения удалены `--debug` и `--verbose`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-471">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="4d3dd-472">Из вариантов завершения удален `interactive` (3324).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-472">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="4d3dd-473">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="4d3dd-473">IoT</span></span>

* <span data-ttu-id="4d3dd-474">Исправлено. При создании политики больше не удаляются существующие политики</span><span class="sxs-lookup"><span data-stu-id="4d3dd-474">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="4d3dd-475">(3934).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-475">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="4d3dd-476">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="4d3dd-476">Key vault</span></span>

* <span data-ttu-id="4d3dd-477">Добавлены команды для функций восстановления хранилища ключей:</span><span class="sxs-lookup"><span data-stu-id="4d3dd-477">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="4d3dd-478">`keyvault`, подкоманды `purge`, `recover` и `keyvault list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="4d3dd-478">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="4d3dd-479">`keyvault secret`, подкоманды `backup`, `restore`, `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="4d3dd-479">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="4d3dd-480">`keyvault certificate`, подкоманды `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="4d3dd-480">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="4d3dd-481">`keyvault key`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-481">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="4d3dd-482">Добавлена интеграция хранилища ключей с субъектом-службой (3133).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-482">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="4d3dd-483">Обновлена плоскость данных хранилища ключей до версии 0.3.2</span><span class="sxs-lookup"><span data-stu-id="4d3dd-483">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="4d3dd-484">(3307).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-484">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="4d3dd-485">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="4d3dd-485">Lab</span></span>

* <span data-ttu-id="4d3dd-486">Добавлена поддержка запросов ко всем виртуальным машинам в лаборатории с помощью `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-486">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="4d3dd-487">Добавлен модуль форматирования табличных выходных данных команд `az lab vm list` и `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-487">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="4d3dd-488">Монитор</span><span class="sxs-lookup"><span data-stu-id="4d3dd-488">Monitor</span></span>

* <span data-ttu-id="4d3dd-489">Исправлены ошибки с файлом шаблона с помощью команды `monitor autoscale-settings get-parameters-template` (3349).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-489">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="4d3dd-490">Команда `monitor alert-rule-incidents list` переименована в `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-490">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="4d3dd-491">Команда `monitor alert-rule-incidents show` переименована в `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-491">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="4d3dd-492">Команда `monitor metric-defintions list` переименована в `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-492">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="4d3dd-493">Команда `monitor alert-rules` переименована в `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-493">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="4d3dd-494">В команду `monitor alert create` внесены следующие изменения:</span><span class="sxs-lookup"><span data-stu-id="4d3dd-494">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="4d3dd-495">подкоманды `condition` и `action` больше не принимают данные JSON;</span><span class="sxs-lookup"><span data-stu-id="4d3dd-495">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="4d3dd-496">добавлены различные параметры, которые упрощают процесс создания правила;</span><span class="sxs-lookup"><span data-stu-id="4d3dd-496">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="4d3dd-497">параметр `location` больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="4d3dd-497">`location` no longer required</span></span>
  * <span data-ttu-id="4d3dd-498">добавлена поддержка имени и идентификатора для целевого объекта;</span><span class="sxs-lookup"><span data-stu-id="4d3dd-498">Add name and ID support for target</span></span>
  * <span data-ttu-id="4d3dd-499">удален параметр `--alert-rule-resource-name`;</span><span class="sxs-lookup"><span data-stu-id="4d3dd-499">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="4d3dd-500">параметр `is-enabled` переименован в `enabled`, он больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="4d3dd-500">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="4d3dd-501">значения по умолчанию для `description` теперь основаны на указанном условии;</span><span class="sxs-lookup"><span data-stu-id="4d3dd-501">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="4d3dd-502">добавлены примеры, в которых подробно представлен новый формат.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-502">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="4d3dd-503">Поддержка имен или идентификаторов для команд `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-503">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="4d3dd-504">Добавлены вспомогательные аргументы и примеры использования команды `monitor alert rule update`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-504">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="4d3dd-505">Сеть</span><span class="sxs-lookup"><span data-stu-id="4d3dd-505">Network</span></span>

* <span data-ttu-id="4d3dd-506">Добавлена команда `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-506">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="4d3dd-507">Добавлен аргумент `--private-access-services` в команды `vnet subnet create` и `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-507">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="4d3dd-508">Исправлена проблема, из-за которой команда `application-gateway redirect-config create` завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-508">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="4d3dd-509">Исправлена проблема, из-за которой команда `application-gateway redirect-config update` не работала с параметром `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-509">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="4d3dd-510">Исправлена ошибка при использовании аргумента `--servers` с командами `application-gateway address-pool create` и `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-510">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="4d3dd-511">Добавлены команды `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-511">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="4d3dd-512">В команду `application-gateway ssl-policy` добавлены подкоманды `list-options`, `predefined list` и `predefined show`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-512">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="4d3dd-513">В команду `application-gateway ssl-policy set` добавлены аргументы `--name`, `--cipher-suites` и `--min-protocol-version`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-513">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="4d3dd-514">В команды `application-gateway http-settings create` и `application-gateway http-settings update` добавлены аргументы `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe` и `--path`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-514">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="4d3dd-515">В команды `application-gateway url-path-map create` и `application-gateway url-path-map update` добавлены аргументы `--default-redirect-config` и `--redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-515">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="4d3dd-516">Добавлен аргумент `--redirect-config` в команду `application-gateway url-path-map rule create`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-516">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="4d3dd-517">Добавлена поддержка параметра `--no-wait` в команде `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-517">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="4d3dd-518">В команды `application-gateway probe create` и `application-gateway probe update` добавлены аргументы `--host-name-from-http-settings`, `--min-servers`, `--match-body` и `--match-status-codes`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-518">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="4d3dd-519">Добавлен аргумент `--redirect-config` в команды `application-gateway rule create` и `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-519">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="4d3dd-520">Добавлена поддержка аргумента `--accelerated-networking` в командах `nic create` и `nic update`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-520">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="4d3dd-521">Удален аргумент `--internal-dns-name-suffix` из команды `nic create`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-521">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="4d3dd-522">Добавлена поддержка параметра `--dns-servers` в командах `nic update` и `nic create`. Добавлена поддержка параметра --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-522">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="4d3dd-523">Исправлена ошибка, из-за которой команда `local-gateway create` игнорировала параметр `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-523">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="4d3dd-524">Добавлена поддержка параметра `--dns-servers` в команде `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-524">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="4d3dd-525">Исправлена ошибка при создании пиринга без фильтрации маршрутов с помощью команды `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-525">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="4d3dd-526">Исправлена ошибка, из-за которой аргументы `--provider` и `--bandwidth` не работали с командой `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-526">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="4d3dd-527">Исправлена ошибка с логикой установки значений по умолчанию в команде `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-527">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="4d3dd-528">Улучшено форматирование выходных данных команды `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-528">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="4d3dd-529">В команде `application-gateway http-listener create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-529">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="4d3dd-530">В команде `application-gateway rule create` используются пул адресов, параметры HTTP и прослушиватель HTTP по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-530">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="4d3dd-531">В команде `lb rule create` используются интерфейсный IP-адрес и серверный пул по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-531">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="4d3dd-532">В команде `lb inbound-nat-rule create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-532">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="4d3dd-533">Профиль</span><span class="sxs-lookup"><span data-stu-id="4d3dd-533">Profile</span></span>

* <span data-ttu-id="4d3dd-534">Поддержка входа на виртуальную машину с использованием управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-534">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="4d3dd-535">Поддержка вывода данных команды `account show` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-535">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="4d3dd-536">При использовании параметра --expanded-view отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-536">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="4d3dd-537">Добавлена команда `get-access-token` для предоставления необработанного токена AAD.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-537">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="4d3dd-538">Поддержка входа с учетной записью пользователя без связанных подписок.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-538">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="4d3dd-539">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="4d3dd-539">RDBMS</span></span>

* <span data-ttu-id="4d3dd-540">Поддержка вывода списка серверов в подписке (3417).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-540">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="4d3dd-541">Исправлена проблема, когда объект `%s` не обрабатывался из-за отсутствия `% server_type` (3393).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-541">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="4d3dd-542">Исправлено сопоставление источника документа и добавлена задача непрерывной интеграции для проверки (3361).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-542">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="4d3dd-543">Исправлена справка по MySQL и PostgreSQL (3369).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-543">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="4d3dd-544">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4d3dd-544">Resource</span></span>

* <span data-ttu-id="4d3dd-545">Улучшены запросы на ввод отсутствующих параметров для команды `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-545">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="4d3dd-546">Улучшен анализ синтаксиса `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-546">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="4d3dd-547">Исправлены проблемы, из-за которых файлы параметров `group deployment create` не распознавались с использованием синтаксиса `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-547">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="4d3dd-548">Поддержка аргумента `--ids` в командах `resource` и `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-548">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="4d3dd-549">Исправлены некоторые сообщения об ошибках и анализе (3584).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-549">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="4d3dd-550">Исправлены ошибки анализа параметра `--resource-type` в команде `lock`. Теперь принимаются `<resource-namespace>` и `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-550">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="4d3dd-551">Добавлена проверка параметров для шаблонов для ссылок на шаблоны (3629).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-551">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="4d3dd-552">Добавлена поддержка указания параметров развертывания с использованием синтаксиса `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-552">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="4d3dd-553">Роль</span><span class="sxs-lookup"><span data-stu-id="4d3dd-553">Role</span></span>

* <span data-ttu-id="4d3dd-554">Поддержка вывода данных команды `create-for-rbac` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-554">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="4d3dd-555">Добавлена очистка назначений ролей и связанного приложения AAD при удалении субъекта-службы (3610).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-555">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="4d3dd-556">В описания аргументов `--start-date` и `--end-date` команды `app create` добавлен формат времени.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-556">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="4d3dd-557">При использовании параметра `--expanded-view` отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-557">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="4d3dd-558">Добавлена интеграция хранилища ключей для команд `create-for-rbac` и `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-558">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="4d3dd-559">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="4d3dd-559">Service Fabric</span></span>
* <span data-ttu-id="4d3dd-560">Исправлена ошибка, из-за которой большие файлы в приложениях усекались при отправке (3666).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-560">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="4d3dd-561">Добавлены тесты для команд Service Fabric (3424).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-561">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="4d3dd-562">Исправлены многие команды Service Fabric (3234).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-562">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="4d3dd-563">SQL</span><span class="sxs-lookup"><span data-stu-id="4d3dd-563">SQL</span></span>

* <span data-ttu-id="4d3dd-564">Удален недействительный параметр `--identity` команды `sql server create`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-564">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="4d3dd-565">Удалены значения паролей из выходных данных команд `sql server create` и `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-565">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="4d3dd-566">Добавлены команды `sql db list-editions` и `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-566">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="4d3dd-567">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4d3dd-567">Storage</span></span>

* <span data-ttu-id="4d3dd-568">Удален параметр `--marker` из команд `storage blob list`, `storage container list` и `storage share list` (3745).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-568">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="4d3dd-569">Включено создание учетных записей хранения с поддержкой только HTTPS.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-569">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="4d3dd-570">Обновлены метрики хранилища, команды входа и CORS (3495).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-570">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="4d3dd-571">Перефразировано сообщение об исключении, которое выводит команда добавления CORS (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="4d3dd-571">Rephrased exception message from CORS add (#3638) (#3362)</span></span>  
* <span data-ttu-id="4d3dd-572">Генератор преобразован в список в режиме пробного выполнения команды пакетной загрузки (3592).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-572">Converted generator to a list in download batch command dry run mode (#3592)</span></span> 
* <span data-ttu-id="4d3dd-573">Исправлена проблема при пробном выполнении команды пакетной загрузки больших двоичных объектов (3640) (3592).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-573">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="4d3dd-574">ВМ</span><span class="sxs-lookup"><span data-stu-id="4d3dd-574">VM</span></span>

* <span data-ttu-id="4d3dd-575">Поддержка настройки NSG.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-575">Support configuring nsg</span></span>
* <span data-ttu-id="4d3dd-576">Исправлена ошибка, из-за которой не удавалось правильно настроить DNS-сервер.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-576">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="4d3dd-577">Поддержка удостоверений управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-577">Support managed service identities</span></span>
* <span data-ttu-id="4d3dd-578">Исправлена проблема, из-за которой для команды `cmss create` с существующей подсистемой балансировки нагрузки требовался параметр `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-578">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`.</span></span>
* <span data-ttu-id="4d3dd-579">Теперь нумерация LUN дисков данных, создаваемых с помощью команды `vm image create`, начинается с 0.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-579">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="4d3dd-580">10 мая 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-580">May 10, 2017</span></span>

<span data-ttu-id="4d3dd-581">Версия 2.0.6</span><span class="sxs-lookup"><span data-stu-id="4d3dd-581">Version 2.0.6</span></span>

* <span data-ttu-id="4d3dd-582">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-582">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="4d3dd-583">Добавлена реляционная СУБД (MySQL, Postgres).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-583">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="4d3dd-584">Добавлены модули Data Lake Store и Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-584">Include Data Lake Analytics and Data Lake Store modules.</span></span>
* <span data-ttu-id="4d3dd-585">Добавлен модуль Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-585">Include Cognitive Services module.</span></span>
* <span data-ttu-id="4d3dd-586">Добавлен модуль Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-586">Include Service Fabric module.</span></span>
* <span data-ttu-id="4d3dd-587">Добавлен модуль Interactive (az-shell переименован).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-587">Include Interactive module (rename of az-shell).</span></span>
* <span data-ttu-id="4d3dd-588">Добавлена поддержка команд CDN.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-588">Add support for CDN commands.</span></span>
* <span data-ttu-id="4d3dd-589">Удален модуль Container.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-589">Remove Container module.</span></span>
* <span data-ttu-id="4d3dd-590">Добавлена команда az -v для az --version ([№ 2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-590">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="4d3dd-591">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-591">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="4d3dd-592">Core</span><span class="sxs-lookup"><span data-stu-id="4d3dd-592">Core</span></span>

* <span data-ttu-id="4d3dd-593">Ядро: запись исключений, порожденных незарегистрированным поставщиком, и его автоматическая регистрация.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-593">core: capture exceptions caused by unregistered provider and auto-register it</span></span>   
* <span data-ttu-id="4d3dd-594">Производительность: сохранение кэша маркеров библиотеки ADAL в памяти до завершения работы процесса ([№ 2603](https://github.com/Azure/azure-cli/issues/2603)).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-594">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="4d3dd-595">Исправление байтов, возвращаемых из шестнадцатеричных отпечатков -o tsv ([№ 3053](https://github.com/Azure/azure-cli/issues/3053)).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-595">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="4d3dd-596">Улучшенное скачивание сертификатов Key Vault и интеграция субъектов-служб AAD ([№ 3003](https://github.com/Azure/azure-cli/issues/3003)).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-596">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="4d3dd-597">Добавление расположения Python в az -version ([№ 2986](https://github.com/Azure/azure-cli/issues/2986)).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-597">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="4d3dd-598">Вход: поддержка входа при отсутствии подписок ([№ 2929](https://github.com/Azure/azure-cli/issues/2929)).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-598">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="4d3dd-599">Ядро: устранен сбой при двукратном входе с помощью субъекта-службы ([№ 2800](https://github.com/Azure/azure-cli/issues/2800)).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-599">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="4d3dd-600">Ядро: возможность настроить путь к файлу accessTokens.json с помощью env var ([№ 2605](https://github.com/Azure/azure-cli/issues/2605)).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-600">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="4d3dd-601">Ядро: возможность применять настроенные параметры по умолчанию к необязательным аргументам ([№ 2703](https://github.com/Azure/azure-cli/issues/2703)).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-601">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="4d3dd-602">Ядро: повышение производительности.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-602">core: Improved performance</span></span>
* <span data-ttu-id="4d3dd-603">Ядро: настаиваемые сертификаты ЦС — поддержка настройки переменной среды REQUESTS_CA_BUNDLE.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-603">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="4d3dd-604">Ядро: облачная конфигурация — использование конечной точки Resource Manager, если не задана конечная точка управления.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-604">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="4d3dd-605">ACS</span><span class="sxs-lookup"><span data-stu-id="4d3dd-605">ACS</span></span>

* <span data-ttu-id="4d3dd-606">Исправление: теперь значение счетчика баз данных master и агентов — целое число, а не строка.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-606">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="4d3dd-607">Предоставлены команды az acs create --no-wait и az acs wait для асинхронного создания.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-607">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="4d3dd-608">Предоставлена команда az acs create --validate для пробного создания.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-608">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="4d3dd-609">Удален профиль Windows перед вызовом метода PUT для команды scale ([№ 2755](https://github.com/Azure/azure-cli/issues/2755)).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-609">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="4d3dd-610">AppService</span><span class="sxs-lookup"><span data-stu-id="4d3dd-610">AppService</span></span>

* <span data-ttu-id="4d3dd-611">Приложение-функция: добавлена полная поддержка приложений-функций, включая создание, отображение, вывод списка, удаление, настройку имени узла, настройку протокола SSL и т. д.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-611">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="4d3dd-612">Добавлены службы Team Services (VSTS) в качестве параметра непрерывной доставки в конфигурации веб-системы управления версиями службы приложений.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-612">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="4d3dd-613">Создана команда az webapp, заменяющая команду az appservice web (для обеспечения обратной совместимости команда az appservice web будет оставлена еще в двух выпусках).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-613">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="4d3dd-614">Предоставлены аргументы для настройки развертывания и стеков времени выполнения при создании веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-614">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="4d3dd-615">Предоставлена команда webapp list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-615">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="4d3dd-616">Поддержка настройки строк подключения ([№ 2647](https://github.com/Azure/azure-cli/issues/2647)).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-616">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="4d3dd-617">Поддержка переключения слотов с предварительным просмотром.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-617">support slot swap with preview</span></span>
* <span data-ttu-id="4d3dd-618">Устранены ошибки из команд службы приложений ([№ 2948](https://github.com/Azure/azure-cli/issues/2948)).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-618">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="4d3dd-619">Использование группы ресурсов в плане служб приложений для операций с сертификатами ([№ 2750](https://github.com/Azure/azure-cli/issues/2750)).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-619">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4d3dd-620">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="4d3dd-620">CosmosDB</span></span>

* <span data-ttu-id="4d3dd-621">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-621">Rename documentdb module to cosmosdb.</span></span>
* <span data-ttu-id="4d3dd-622">Добавлена поддержка интерфейсов API уровня данных DocumentDB: управление базами данных и коллекциями.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-622">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="4d3dd-623">Добавлена поддержка включения автоматической отработки отказа для учетных записей базы данных.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-623">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="4d3dd-624">Добавлена поддержка нового параметра ConsistentPrefix политики согласованности.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-624">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="4d3dd-625">Аналитика озера данных</span><span class="sxs-lookup"><span data-stu-id="4d3dd-625">Data Lake Analytics</span></span>

* <span data-ttu-id="4d3dd-626">Исправлена ошибка, из-за которой фильтрация списков заданий по результату и состоянию вызывала сбой.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-626">Fix a bug where filtering on result and state for job lists would throw an error.</span></span>
* <span data-ttu-id="4d3dd-627">Добавлена поддержка нового типа элемента каталога — пакета.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-627">Add support for new catalog item type: package.</span></span> <span data-ttu-id="4d3dd-628">Для доступа к нему используется `az dla catalog package`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-628">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="4d3dd-629">Появилась возможность вывести список следующих элементов каталога из базы данных (указание схемы не требуется):</span><span class="sxs-lookup"><span data-stu-id="4d3dd-629">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="4d3dd-630">Таблица</span><span class="sxs-lookup"><span data-stu-id="4d3dd-630">Table</span></span>
  * <span data-ttu-id="4d3dd-631">функция с табличным значением;</span><span class="sxs-lookup"><span data-stu-id="4d3dd-631">Table valued function</span></span>
  * <span data-ttu-id="4d3dd-632">Просмотр</span><span class="sxs-lookup"><span data-stu-id="4d3dd-632">View</span></span>
  * <span data-ttu-id="4d3dd-633">статистика таблицы.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-633">Table Statistics.</span></span> <span data-ttu-id="4d3dd-634">Их можно также вывести с помощью схемы, но без указания имени таблицы.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-634">This can also be listed with a schema, but without specifying a table name.</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="4d3dd-635">Хранилище озера данных</span><span class="sxs-lookup"><span data-stu-id="4d3dd-635">Data Lake Store</span></span>

* <span data-ttu-id="4d3dd-636">Обновлена версия пакета SDK базовой файловой системы, что обеспечивает лучшую поддержку сценариев регулирования на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-636">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios.</span></span>
* <span data-ttu-id="4d3dd-637">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-637">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="4d3dd-638">Отсутствовала справка для команды access show.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-638">missed help for access show.</span></span> <span data-ttu-id="4d3dd-639">Теперь она добавлена.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-639">adding it.</span></span> <span data-ttu-id="4d3dd-640">([№ 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="4d3dd-640">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="4d3dd-641">Поиск</span><span class="sxs-lookup"><span data-stu-id="4d3dd-641">Find</span></span>

* <span data-ttu-id="4d3dd-642">Улучшены результаты поиска и разрешено управление версиями индекса поиска.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-642">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="4d3dd-643">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="4d3dd-643">KeyVault</span></span>

* <span data-ttu-id="4d3dd-644">BC: в команде `az keyvault certificate download` параметр -e со строкового или двоичного значения изменен на PEM или DER, чтобы лучше представить параметры.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-644">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="4d3dd-645">BC: из команды `keyvault certificate create` удалены параметры --expires и --not-before, так как они не поддерживаются службой.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-645">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service.</span></span>
* <span data-ttu-id="4d3dd-646">В команду `keyvault certificate create` добавлен параметр --validity для выборочного переопределения значение в параметре --policy.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-646">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="4d3dd-647">Исправлена ошибка в команде `keyvault certificate get-default-policy`, в которой были доступны параметры expires и not_before, а параметр validity_in_months — нет.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-647">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not.</span></span>
* <span data-ttu-id="4d3dd-648">Добавлено исправление для модуля keyvault для импорта PEM- и PFX-файлов ([№ 2754](https://github.com/Azure/azure-cli/issues/2754)).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-648">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="4d3dd-649">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="4d3dd-649">Lab</span></span>

* <span data-ttu-id="4d3dd-650">Добавлены команды создания, отображения, удаления и вывода списка для среды в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-650">Adding create, show, delete & list commands for environment in the lab.</span></span>
* <span data-ttu-id="4d3dd-651">Добавлены команды отображения и вывода списка для просмотра шаблонов ARM в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-651">Adding show & list commands to view ARM templates in the lab.</span></span>
* <span data-ttu-id="4d3dd-652">В команду `az lab vm list` добавлен флаг --environment для фильтрации виртуальных машин по среде в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-652">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab.</span></span>
* <span data-ttu-id="4d3dd-653">Добавлена вспомогательная команда `az lab formula export-artifacts` для экспорта шаблона артефакта в формуле лаборатории.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-653">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula.</span></span>
* <span data-ttu-id="4d3dd-654">Добавлены команды для управления секретами в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-654">Add commands to manage secrets within a Lab.</span></span>

### <a name="monitor"></a><span data-ttu-id="4d3dd-655">Монитор</span><span class="sxs-lookup"><span data-stu-id="4d3dd-655">Monitor</span></span>

* <span data-ttu-id="4d3dd-656">Исправление ошибки: моделирование `--actions` в `az alert-rules create` для использования строки в формате JSON ([№ 3009](https://github.com/Azure/azure-cli/issues/3009)).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-656">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="4d3dd-657">Исправление ошибки: при создании параметров диагностики не принимались журналы и метрики из команды show ([№ 2913](https://github.com/Azure/azure-cli/issues/2913)).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-657">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="4d3dd-658">Сеть</span><span class="sxs-lookup"><span data-stu-id="4d3dd-658">Network</span></span>

* <span data-ttu-id="4d3dd-659">Добавлена команда `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-659">Add `network watcher test-connectivity` command.</span></span>
* <span data-ttu-id="4d3dd-660">Добавлена поддержка параметра `--filters` в команде `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-660">Add support for `--filters` parameter for `network watcher packet-capture create`.</span></span>
* <span data-ttu-id="4d3dd-661">Добавлена поддержка фильтрации подключений шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-661">Add support for Application Gateway connection draining.</span></span>
* <span data-ttu-id="4d3dd-662">Добавлена поддержка конфигурации набора правил WAF шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-662">Add support for Application Gateway WAF rule set configuration.</span></span>
* <span data-ttu-id="4d3dd-663">Добавлена поддержка правил и фильтров маршрутов ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-663">Add support for ExpressRoute route filters and rules.</span></span>
* <span data-ttu-id="4d3dd-664">Добавлена поддержка географической маршрутизации диспетчера трафика.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-664">Add support for TrafficManager geographic routing.</span></span>
* <span data-ttu-id="4d3dd-665">Добавлена поддержка селекторов трафика на основе политик для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-665">Add support for VPN connection policy-based traffic selectors.</span></span>
* <span data-ttu-id="4d3dd-666">Добавлена поддержка политик IPSec для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-666">Add support for VPN connection IPSec policies.</span></span>
* <span data-ttu-id="4d3dd-667">Исправлена ошибка `vpn-connection create`, возникавшая при использовании параметра `--no-wait` или `--validate`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-667">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters.</span></span>
* <span data-ttu-id="4d3dd-668">Добавлена поддержка шлюзов виртуальной сети "активный-активный".</span><span class="sxs-lookup"><span data-stu-id="4d3dd-668">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="4d3dd-669">Удалены значения NULL из выходных данных команды `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-669">Remove nulls values from output of `network vpn-connection list/show` commands.</span></span>
* <span data-ttu-id="4d3dd-670">BC: исправлена ошибка в выходных данных `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-670">BC: Fix bug in the output of `vpn-connection create`</span></span> 
* <span data-ttu-id="4d3dd-671">Исправлена ошибка, приводившая к неправильному анализу аргумента --key-length команды vpn-connection create.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-671">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly.</span></span>
* <span data-ttu-id="4d3dd-672">Исправлена ошибка в `dns zone import`, из-за которой записи не импортировались правильно.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-672">Fix bug in `dns zone import` where records were not imported correctly.</span></span>
* <span data-ttu-id="4d3dd-673">Исправлена ошибка, из-за которой команда `traffic-manager endpoint update` не работала.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-673">Fix bug where `traffic-manager endpoint update` did not work.</span></span>
* <span data-ttu-id="4d3dd-674">Добавлены команды предварительного просмотра для Наблюдателя за сетями.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-674">Add 'network watcher' preview commands.</span></span>

### <a name="profile"></a><span data-ttu-id="4d3dd-675">Профиль</span><span class="sxs-lookup"><span data-stu-id="4d3dd-675">Profile</span></span>

* <span data-ttu-id="4d3dd-676">Поддержка входа при отсутствии подписок ([№ 2560](https://github.com/Azure/azure-cli/issues/2560)).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-676">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="4d3dd-677">Поддержка сокращенных имен параметров в команде az account set --subscription ([№ 2980](https://github.com/Azure/azure-cli/issues/2980)).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-677">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="4d3dd-678">Redis</span><span class="sxs-lookup"><span data-stu-id="4d3dd-678">Redis</span></span>

* <span data-ttu-id="4d3dd-679">Добавлена команда update, которая также добавляет возможность масштабирования для кэша Redis.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-679">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="4d3dd-680">Команда update-settings объявляется нерекомендуемой.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-680">Deprecates the 'update-settings' command.</span></span>

### <a name="resource"></a><span data-ttu-id="4d3dd-681">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4d3dd-681">Resource</span></span>

* <span data-ttu-id="4d3dd-682">Добавлены команды определения managedapp и managedapp ([№ 2985](https://github.com/Azure/azure-cli/issues/2985)).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-682">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="4d3dd-683">Поддержка команд provider operation ([№ 2908](https://github.com/Azure/azure-cli/issues/2908)).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-683">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="4d3dd-684">Поддержка создания универсального ресурса ([№ 2606](https://github.com/Azure/azure-cli/issues/2606)).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-684">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="4d3dd-685">Исправлен анализ ресурсов и поиск версии API.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-685">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="4d3dd-686">([№ 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="4d3dd-686">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="4d3dd-687">Добавлены документы для команды az lock update.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-687">Add docs for az lock update.</span></span> <span data-ttu-id="4d3dd-688">([№ 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="4d3dd-688">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="4d3dd-689">Исправлена ошибка, возникавшая при попытке вывести список ресурсов группы, которая не существует.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-689">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="4d3dd-690">([№ 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="4d3dd-690">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="4d3dd-691">[Вычисления.] Устранены проблемы с масштабируемым набором виртуальных машин и обновлением группы доступности виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-691">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="4d3dd-692">([№ 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="4d3dd-692">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="4d3dd-693">Исправлена блокировка создания и удаления, возникающая, если параметр parent-resource-path не указан ([№ 2742](https://github.com/Azure/azure-cli/issues/2742)).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-693">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="4d3dd-694">Роль</span><span class="sxs-lookup"><span data-stu-id="4d3dd-694">Role</span></span>

* <span data-ttu-id="4d3dd-695">create-for-rbac: гарантируется, что дата завершения работы поставщика служб не может превышать срок действия сертификата ([№ 2989](https://github.com/Azure/azure-cli/issues/2989)).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-695">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="4d3dd-696">RBAC: добавлена полная поддержка команды ad group ([№ 2016](https://github.com/Azure/azure-cli/issues/2016)).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-696">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="4d3dd-697">Роль: устранены проблемы при обновлении определения роли ([№ 2745](https://github.com/Azure/azure-cli/issues/2745)).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-697">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="4d3dd-698">create-for-rbac: обеспечен выбор введенного пользователем пароля.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-698">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="4d3dd-699">SQL</span><span class="sxs-lookup"><span data-stu-id="4d3dd-699">SQL</span></span>

* <span data-ttu-id="4d3dd-700">Добавлены команды az sql server list-usages и az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-700">Added az sql server list-usages and az sql db list-usages commands.</span></span>
* <span data-ttu-id="4d3dd-701">SQL: возможность прямого подключения к поставщику ресурса ([№ 2832](https://github.com/Azure/azure-cli/issues/2832)).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-701">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="4d3dd-702">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4d3dd-702">Storage</span></span>

* <span data-ttu-id="4d3dd-703">Добавлено расположение по умолчанию группы ресурсов для `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-703">Default location to resource group location for `storage account create`.</span></span>
* <span data-ttu-id="4d3dd-704">Добавлена поддержка добавочного копирования больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-704">Add support for incremental blob copy</span></span>
* <span data-ttu-id="4d3dd-705">Добавлена поддержка передачи больших блочных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-705">Add support for large block blob upload</span></span>
* <span data-ttu-id="4d3dd-706">Размер блока изменяется и составляет 100 МБ, если передается файл, чей размер превышает 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-706">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="4d3dd-707">ВМ</span><span class="sxs-lookup"><span data-stu-id="4d3dd-707">VM</span></span>

* <span data-ttu-id="4d3dd-708">avail-set: число доменов обновления и доменов сбоя сделано необязательным.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-708">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="4d3dd-709">Примечание. Команды виртуальной машины в независимых облаках: избегайте использовать функции, связанные с Управляемыми дисками, включая следующие:</span><span class="sxs-lookup"><span data-stu-id="4d3dd-709">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="4d3dd-710">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="4d3dd-710">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="4d3dd-711">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="4d3dd-711">az vm/vmss disk</span></span>
  3. <span data-ttu-id="4d3dd-712">В команде az vm/vmss create используйте параметр --use-unmanaged-disk, чтобы избежать использования Управляемых дисков. Другие команды должны работать.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-712">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="4d3dd-713">vm/vmss: улучшен текст предупреждения при создании пары ключей SSH.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-713">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="4d3dd-714">vm/vmss: поддержка создания из образа Marketplace, для которого требуются сведения о плане ([№ 1209](https://github.com/Azure/azure-cli/issues/1209)).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-714">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="4d3dd-715">3 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-715">April 3, 2017</span></span>

<span data-ttu-id="4d3dd-716">Версия 2.0.2</span><span class="sxs-lookup"><span data-stu-id="4d3dd-716">Version 2.0.2</span></span>

<span data-ttu-id="4d3dd-717">В этом выпуске мы добавили компоненты ACR, Batch, KeyVault и SQL.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-717">We released the ACR, Batch, KeyVault, and SQL components in this release.</span></span>

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

### <a name="core"></a><span data-ttu-id="4d3dd-718">Core</span><span class="sxs-lookup"><span data-stu-id="4d3dd-718">Core</span></span>

* <span data-ttu-id="4d3dd-719">Модули Acr, Lab, Monitor и Find добавлены в список по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-719">Add acr, lab, monitor, and find modules to default list.</span></span>
* <span data-ttu-id="4d3dd-720">Вход: пропуск неправильного клиента ([#2634](https://github.com/Azure/azure-cli/pull/2634)).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-720">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="4d3dd-721">Вход: для подписки по умолчанию задано значение 1 с состоянием "Включено" ([#2575](https://github.com/Azure/azure-cli/pull/2575)).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-721">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="4d3dd-722">Добавлена поддержка команд wait и --no-wait для дополнительных команд ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-722">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="4d3dd-723">Core: поддержка входа при помощи субъекта-службы с использованием сертификата ([#2457](https://github.com/Azure/azure-cli/pull/2457)).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-723">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="4d3dd-724">Добавлен запрос для отсутствующих параметров шаблона</span><span class="sxs-lookup"><span data-stu-id="4d3dd-724">Add prompting for missing template parameters.</span></span> <span data-ttu-id="4d3dd-725">([#2364](https://github.com/Azure/azure-cli/pull/2364)).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-725">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="4d3dd-726">Добавлена поддержка установки параметров по умолчанию для таких распространенных аргументов, как группа ресурсов по умолчанию, веб-страница по умолчанию, виртуальная машина по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-726">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="4d3dd-727">Добавлена поддержка входа на конкретный клиент.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-727">Support login to specific tenant</span></span>
 
### <a name="acs"></a><span data-ttu-id="4d3dd-728">ACS</span><span class="sxs-lookup"><span data-stu-id="4d3dd-728">ACS</span></span>

* <span data-ttu-id="4d3dd-729">[ACS] Добавлена поддержка настройки кластера ACS по умолчанию ([#2554](https://github.com/Azure/azure-cli/pull/2554)).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-729">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="4d3dd-730">Добавлена поддержка запроса пароля для ключа SSH</span><span class="sxs-lookup"><span data-stu-id="4d3dd-730">Add support for ssh key password prompting.</span></span> <span data-ttu-id="4d3dd-731">([#2044](https://github.com/Azure/azure-cli/pull/2044)).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-731">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="4d3dd-732">Добавлена поддержка кластеров Windows</span><span class="sxs-lookup"><span data-stu-id="4d3dd-732">Add support for windows clusters.</span></span> <span data-ttu-id="4d3dd-733">([#2211](https://github.com/Azure/azure-cli/pull/2211)).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-733">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="4d3dd-734">Добавлена возможность изменения роли "Владелец" на роль "Участник"</span><span class="sxs-lookup"><span data-stu-id="4d3dd-734">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="4d3dd-735">([#2321](https://github.com/Azure/azure-cli/pull/2321)).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-735">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>
 
### <a name="appservice"></a><span data-ttu-id="4d3dd-736">AppService</span><span class="sxs-lookup"><span data-stu-id="4d3dd-736">AppService</span></span>

* <span data-ttu-id="4d3dd-737">AppService: добавлена поддержка получения внешнего IP-адреса, используемого для записей DNS типа A ([#2627](https://github.com/Azure/azure-cli/pull/2627)).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-737">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="4d3dd-738">AppService: добавлена поддержка привязки групповых сертификатов ([#2625](https://github.com/Azure/azure-cli/pull/2625)).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-738">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="4d3dd-739">AppService: добавлена поддержка профилей для публикации списком ([#2504](https://github.com/Azure/azure-cli/pull/2504)).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-739">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="4d3dd-740">AppService: добавлен триггер синхронизации с системой управления версиями после настройки ([#2326](https://github.com/Azure/azure-cli/pull/2326)).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-740">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>
 
### <a name="datalake"></a><span data-ttu-id="4d3dd-741">DataLake</span><span class="sxs-lookup"><span data-stu-id="4d3dd-741">DataLake</span></span>

* <span data-ttu-id="4d3dd-742">Первоначальный выпуск модуля Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-742">Initial release of Data Lake Analytics module.</span></span>
* <span data-ttu-id="4d3dd-743">Первоначальный выпуск модуля Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-743">Initial release of Data Lake Store module.</span></span>
 
### <a name="docuemntdb"></a><span data-ttu-id="4d3dd-744">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="4d3dd-744">DocuemntDB</span></span>

* <span data-ttu-id="4d3dd-745">DocumentDB: добавлена поддержка для получения списка строк подключения ([#2580](https://github.com/Azure/azure-cli/pull/2580)).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-745">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="4d3dd-746">ВМ</span><span class="sxs-lookup"><span data-stu-id="4d3dd-746">VM</span></span>

* <span data-ttu-id="4d3dd-747">[Вычисления] Добавлена поддержка AppGateway для создания масштабируемого набора виртуальных машин ([#2570](https://github.com/Azure/azure-cli/pull/2570)).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-747">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="4d3dd-748">[ВМ и VMSS] Улучшена поддержка кэширования диска ([#2522](https://github.com/Azure/azure-cli/pull/2522)).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-748">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="4d3dd-749">ВМ и VMSS: внедрена логика проверки учетных данных, используемая на портале ([#2537](https://github.com/Azure/azure-cli/pull/2537)).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-749">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="4d3dd-750">Добавлена поддержка команд wait и --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-750">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="4d3dd-751">Масштабируемый набор виртуальных машин: добавлена поддержка * для представления экземпляров на виртуальных машинах в виде списка ([#2467](https://github.com/Azure/azure-cli/pull/2467)).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-751">Virtual machine scale set: support * to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="4d3dd-752">Добавлена команда --secrets для виртуальных машин и масштабируемого набора виртуальных машин ([#2212}(https://github.com/Azure/azure-cli/pull/2212)).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-752">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="4d3dd-753">Добавлено разрешение на создание виртуальных машин на основе специализированного образа VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256)).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-753">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="4d3dd-754">27 февраля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-754">February 27, 2017</span></span>

<span data-ttu-id="4d3dd-755">Версия 2.0.0</span><span class="sxs-lookup"><span data-stu-id="4d3dd-755">Version 2.0.0</span></span>

<span data-ttu-id="4d3dd-756">Этот первый общедоступный выпуск Azure CLI 2.0.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-756">This release of Azure CLI 2.0 is the first "Generally Available" release.</span></span>
<span data-ttu-id="4d3dd-757">Общедоступными являются такие командные модули:</span><span class="sxs-lookup"><span data-stu-id="4d3dd-757">General availability applies to these command modules:</span></span>
- <span data-ttu-id="4d3dd-758">служба контейнеров (ACS);</span><span class="sxs-lookup"><span data-stu-id="4d3dd-758">Container Service (acs)</span></span>
- <span data-ttu-id="4d3dd-759">вычисления (в том числе Resource Manager, виртуальная машина, масштабируемые наборы виртуальных машин, управляемые диски);</span><span class="sxs-lookup"><span data-stu-id="4d3dd-759">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="4d3dd-760">Сеть</span><span class="sxs-lookup"><span data-stu-id="4d3dd-760">Networking</span></span>
- <span data-ttu-id="4d3dd-761">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4d3dd-761">Storage</span></span>

<span data-ttu-id="4d3dd-762">Эти командные модули могут использоваться в рабочих средах и поддерживаются стандартными соглашениями Майкрософт об уровне обслуживания.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-762">These command modules can be used in production and are supported by standard Microsoft SLA.</span></span>
<span data-ttu-id="4d3dd-763">Вы можете отправлять запросы непосредственно в службу технической поддержки Майкрософт или добавлять описание проблем в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-763">You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/).</span></span>
<span data-ttu-id="4d3dd-764">Вы можете задавать вопросы на сайте [StackOverflow, используя тег azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), или обращаться к группе разработчиков по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Можно отправлять отзывы из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-764">You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). You can provide feedback from the command line with the `az feedback` command.</span></span>

<span data-ttu-id="4d3dd-765">Команды в этих модулях стабильны, и предполагается, что в следующих выпусках этой версии Azure CLI их синтаксис не будет меняться.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-765">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI.</span></span>

<span data-ttu-id="4d3dd-766">Чтобы проверить версию интерфейса командной строки, используйте `az --version`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-766">To verify the version of the CLI, use `az --version`.</span></span>
<span data-ttu-id="4d3dd-767">В выходных данных указана версия самого интерфейса командной строки (2.0.0 в этом выпуске), версии отдельных командных модулей и используемые вами версии Python и GCC.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-767">The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using.</span></span>

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
> <span data-ttu-id="4d3dd-768">Некоторые командные модули имеют постфикс b*n* или rc*n*.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-768">Some of the command modules have a "b*n*" or "rc*n*" postfix.</span></span>
> <span data-ttu-id="4d3dd-769">Эти командные модули все еще находятся на стадии предварительной версии и станут общедоступными в будущем.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-769">These command modules are still in preview and will become generally available in the future.</span></span>

<span data-ttu-id="4d3dd-770">У нас также есть предварительные ежедневные сборки интерфейса командной строки.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-770">We also have nightly preview builds of the CLI.</span></span>
<span data-ttu-id="4d3dd-771">Дополнительные сведения см. в инструкциях по [получению ежедневных сборок](https://github.com/Azure/azure-cli#nightly-builds), а также в инструкциях по [настройке среды разработки и участии в написании кода](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="4d3dd-771">For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup).</span></span>

<span data-ttu-id="4d3dd-772">О проблемах с предварительными ежедневными сборками можно сообщить несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="4d3dd-772">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="4d3dd-773">добавив информацию о проблемах в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/);</span><span class="sxs-lookup"><span data-stu-id="4d3dd-773">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="4d3dd-774">обратившись к специалистам группы разработчиков продукта по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com);</span><span class="sxs-lookup"><span data-stu-id="4d3dd-774">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
- <span data-ttu-id="4d3dd-775">отправив отзыв из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="4d3dd-775">Provide feedback from the command line with the `az feedback` command.</span></span>

