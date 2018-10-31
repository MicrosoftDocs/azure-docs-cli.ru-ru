---
title: Заметки о выпуске Azure CLI
description: Узнайте о последних обновлениях в Azure CLI
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 10/23/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 65e34ab6014c47ae92a6d4bae8cdc30d4a1413dc
ms.sourcegitcommit: aec89531c938781b4724f43b5bb4b878e106a26a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2018
ms.locfileid: "49952491"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="70ea7-103">Заметки о выпуске Azure CLI</span><span class="sxs-lookup"><span data-stu-id="70ea7-103">Azure CLI release notes</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="70ea7-104">23 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70ea7-104">October 23, 2018</span></span>

<span data-ttu-id="70ea7-105">Версия 2.0.49</span><span class="sxs-lookup"><span data-stu-id="70ea7-105">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="70ea7-106">Core</span><span class="sxs-lookup"><span data-stu-id="70ea7-106">Core</span></span>
* <span data-ttu-id="70ea7-107">Исправлена проблема с аргументом `--ids`, из-за которой аргумент `--subscription` имел приоритет над подпиской, указанной с использованием `--ids`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-107">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="70ea7-108">Добавлены явные предупреждения о том, что параметры будут игнорироваться при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-108">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="70ea7-109">ACR</span><span class="sxs-lookup"><span data-stu-id="70ea7-109">ACR</span></span>
* <span data-ttu-id="70ea7-110">Исправлена ошибка, связанная с шифрованием сборки ACR в Python2.</span><span class="sxs-lookup"><span data-stu-id="70ea7-110">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="70ea7-111">CDN</span><span class="sxs-lookup"><span data-stu-id="70ea7-111">CDN</span></span>
* <span data-ttu-id="70ea7-112">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено стандартное поведение при кешировании строки запроса `cdn endpoint create`. Теперь IgnoreQueryString не является значением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="70ea7-112">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="70ea7-113">Это значение задает служба.</span><span class="sxs-lookup"><span data-stu-id="70ea7-113">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="70ea7-114">Контейнер</span><span class="sxs-lookup"><span data-stu-id="70ea7-114">Container</span></span>
* <span data-ttu-id="70ea7-115">Добавлен тип `Private` в качестве допустимого типа для передачи в --ip-address.</span><span class="sxs-lookup"><span data-stu-id="70ea7-115">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="70ea7-116">При настройке подсети для группы контейнеров разрешено использовать только идентификатор подсети.</span><span class="sxs-lookup"><span data-stu-id="70ea7-116">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="70ea7-117">Разрешено указывать имя виртуальной сети или идентификатор ресурса для использования виртуальных сетей из разных групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="70ea7-117">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="70ea7-118">Добавлен параметр `--assign-identity`, позволяющий добавить удостоверение MSI для группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="70ea7-118">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="70ea7-119">Добавлен параметр `--scope`, позволяющий создать назначение ролей для удостоверения MSI, назначаемого системой.</span><span class="sxs-lookup"><span data-stu-id="70ea7-119">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="70ea7-120">Добавлено предупреждение, которое появляется при создании группы контейнеров с помощью образа без использования длительного процесса.</span><span class="sxs-lookup"><span data-stu-id="70ea7-120">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="70ea7-121">Исправлены ошибки, связанные с табличными выходными данными для команд `list` и `show`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-121">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="70ea7-122">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="70ea7-122">CosmosDB</span></span>
* <span data-ttu-id="70ea7-123">В команду `cosmosdb create` добавлена поддержка параметра `--enable-multiple-write-locations`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-123">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="70ea7-124">Interactive</span><span class="sxs-lookup"><span data-stu-id="70ea7-124">Interactive</span></span>
* <span data-ttu-id="70ea7-125">Внесены изменения, которые обеспечивают отображение параметра глобальных подписок в списке параметров.</span><span class="sxs-lookup"><span data-stu-id="70ea7-125">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="70ea7-126">IoT Central</span><span class="sxs-lookup"><span data-stu-id="70ea7-126">IoT Central</span></span>
* <span data-ttu-id="70ea7-127">Добавлены параметры для шаблона и отображаемого имени, используемые при создании приложения IoT Central.</span><span class="sxs-lookup"><span data-stu-id="70ea7-127">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="70ea7-128">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена поддержка номера SKU F1. Вместо него используйте S1.</span><span class="sxs-lookup"><span data-stu-id="70ea7-128">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="70ea7-129">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="70ea7-129">Monitor</span></span>
* <span data-ttu-id="70ea7-130">Изменения в `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="70ea7-130">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="70ea7-131">Добавлена поддержка для вывода списка всех событий на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="70ea7-131">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="70ea7-132">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="70ea7-132">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="70ea7-133">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="70ea7-133">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="70ea7-134">Добавлен параметр `--namespace` в качестве псевдонима для нерекомендуемого параметра `--resource-provider`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-134">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="70ea7-135">Параметр `--filters` отмечен как нерекомендуемый, так как служба не поддерживает значения, отличные от значений со строгой типизацией.</span><span class="sxs-lookup"><span data-stu-id="70ea7-135">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="70ea7-136">Изменения в `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="70ea7-136">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="70ea7-137">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="70ea7-137">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="70ea7-138">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="70ea7-138">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="70ea7-139">Улучшена проверка аргументов `--event-hub` и `--event-hub-rule` для `monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-139">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="70ea7-140">Сеть</span><span class="sxs-lookup"><span data-stu-id="70ea7-140">Network</span></span>
* <span data-ttu-id="70ea7-141">Для `nic create` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="70ea7-141">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="70ea7-142">Для `nic ip-config create/update` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="70ea7-142">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="70ea7-143">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="70ea7-143">ServiceBus</span></span>
* <span data-ttu-id="70ea7-144">В класс MigrationConfigProperties добавлено свойство `migration_state` с доступом только для чтения. Это свойство позволяет получить сведения о текущем состоянии миграции с ценовой категории Служебной шины "Стандартный" на ценовую категорию "Премиум".</span><span class="sxs-lookup"><span data-stu-id="70ea7-144">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="70ea7-145">SQL</span><span class="sxs-lookup"><span data-stu-id="70ea7-145">SQL</span></span>
* <span data-ttu-id="70ea7-146">Исправлены `sql failover-group create` и `sql failover-group update` для работы с политикой перехода на другой ресурс вручную.</span><span class="sxs-lookup"><span data-stu-id="70ea7-146">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="70ea7-147">Хранилище</span><span class="sxs-lookup"><span data-stu-id="70ea7-147">Storage</span></span>
* <span data-ttu-id="70ea7-148">Исправлен формат выходных данных `az storage cors list`: для всех элементов отображается правильный ключ службы.</span><span class="sxs-lookup"><span data-stu-id="70ea7-148">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="70ea7-149">Добавлен параметр `--bypass-immutability-policy`, который позволяет удалить контейнер, блокируемый политикой неизменяемости.</span><span class="sxs-lookup"><span data-stu-id="70ea7-149">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="70ea7-150">ВМ</span><span class="sxs-lookup"><span data-stu-id="70ea7-150">VM</span></span>
* <span data-ttu-id="70ea7-151">Для режима кэширования диска принудительно применяется значение `None` при использовании команды `[vm|vmss] create` для виртуальных машин серии Lv или Lv2.</span><span class="sxs-lookup"><span data-stu-id="70ea7-151">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="70ea7-152">Для `vm create` обновлен список поддерживаемых размеров для поддерживаемого сетевого ускорителя.</span><span class="sxs-lookup"><span data-stu-id="70ea7-152">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="70ea7-153">Для `disk create` добавлены строго типизированные аргументы, которые позволяют настроить скорость операций ввода-вывода и передачи данных в секунду для дисков SSD ценовой категории "Ультра".</span><span class="sxs-lookup"><span data-stu-id="70ea7-153">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="70ea7-154">16 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70ea7-154">October 16, 2018</span></span>

<span data-ttu-id="70ea7-155">Версия 2.0.48</span><span class="sxs-lookup"><span data-stu-id="70ea7-155">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="70ea7-156">ВМ</span><span class="sxs-lookup"><span data-stu-id="70ea7-156">VM</span></span>
* <span data-ttu-id="70ea7-157">Исправлена проблема с пакетом SDK, из-за которой установка Homebrew завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="70ea7-157">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="70ea7-158">9 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70ea7-158">October 9, 2018</span></span>

<span data-ttu-id="70ea7-159">Версия 2.0.47</span><span class="sxs-lookup"><span data-stu-id="70ea7-159">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="70ea7-160">Core</span><span class="sxs-lookup"><span data-stu-id="70ea7-160">Core</span></span>
* <span data-ttu-id="70ea7-161">Улучшена обработка ошибок типа Bad Request (Недопустимый запрос).</span><span class="sxs-lookup"><span data-stu-id="70ea7-161">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="70ea7-162">ACR</span><span class="sxs-lookup"><span data-stu-id="70ea7-162">ACR</span></span>
* <span data-ttu-id="70ea7-163">Добавлена поддержка табличного формата, как в клиенте Helm.</span><span class="sxs-lookup"><span data-stu-id="70ea7-163">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="70ea7-164">ACS</span><span class="sxs-lookup"><span data-stu-id="70ea7-164">ACS</span></span>
* <span data-ttu-id="70ea7-165">Добавлен параметр `aks [create|scale] --nodepool-name` для настройки имени пула узлов. Длина имени ограничена 12 символами. Имя по умолчанию — nodepool1.</span><span class="sxs-lookup"><span data-stu-id="70ea7-165">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="70ea7-166">Исправлен возврат к scp при сбое Paramiko.</span><span class="sxs-lookup"><span data-stu-id="70ea7-166">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="70ea7-167">Изменена команда `aks create`, которая больше не требует `--aad-tenant-id`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-167">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="70ea7-168">Улучшена функция слияния учетных данных Kubernetes при наличии дублированных записей.</span><span class="sxs-lookup"><span data-stu-id="70ea7-168">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="70ea7-169">Контейнер</span><span class="sxs-lookup"><span data-stu-id="70ea7-169">Container</span></span>
* <span data-ttu-id="70ea7-170">Изменена команда `functionapp create`, которая теперь поддерживает создание типа для плана потребления Linux с конкретной средой выполнения.</span><span class="sxs-lookup"><span data-stu-id="70ea7-170">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="70ea7-171">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для размещения веб-приложений в контейнерах Windows.</span><span class="sxs-lookup"><span data-stu-id="70ea7-171">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="70ea7-172">Концентратор событий</span><span class="sxs-lookup"><span data-stu-id="70ea7-172">Event Hub</span></span>
* <span data-ttu-id="70ea7-173">Исправлена команда `eventhub update`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-173">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="70ea7-174">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="70ea7-174">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="70ea7-175">расширения.</span><span class="sxs-lookup"><span data-stu-id="70ea7-175">Extensions</span></span>
* <span data-ttu-id="70ea7-176">Исправлена проблема при попытке добавить расширение, которое уже установлено.</span><span class="sxs-lookup"><span data-stu-id="70ea7-176">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="70ea7-177">HDInsight</span><span class="sxs-lookup"><span data-stu-id="70ea7-177">HDInsight</span></span>
* <span data-ttu-id="70ea7-178">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="70ea7-178">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="70ea7-179">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="70ea7-179">IoT</span></span>
* <span data-ttu-id="70ea7-180">На баннер, отображаемый при первом запуске, добавлена команда для установки расширений.</span><span class="sxs-lookup"><span data-stu-id="70ea7-180">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="70ea7-181">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="70ea7-181">KeyVault</span></span>
* <span data-ttu-id="70ea7-182">Изменены команды для работы с хранилищем ключей.Теперь они ограничены последним профилем API.</span><span class="sxs-lookup"><span data-stu-id="70ea7-182">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="70ea7-183">Сеть</span><span class="sxs-lookup"><span data-stu-id="70ea7-183">Network</span></span>
* <span data-ttu-id="70ea7-184">Исправлена команда `network dns zone create`. Теперь команда выполняется успешно, даже если пользователь настроил расположение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="70ea7-184">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="70ea7-185">См. № 6052.</span><span class="sxs-lookup"><span data-stu-id="70ea7-185">See #6052</span></span>
* <span data-ttu-id="70ea7-186">`--remote-vnet-id` не рекомендуется к использованию для `network vnet peering create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-186">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="70ea7-187">Добавлена параметр `--remote-vnet` в команду `network vnet peering create`, который принимает имя или идентификатор.</span><span class="sxs-lookup"><span data-stu-id="70ea7-187">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="70ea7-188">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet create` с параметром `--subnet-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-188">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="70ea7-189">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet subnet [create|update]` с параметром `--address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-189">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="70ea7-190">Исправлена ошибка в команде `network application-gateway create`, из-за которой было невозможно создать шлюзы с номером SKU `WAF_v2` или `Standard_v2`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-190">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="70ea7-191">Добавлен вспомогательный аргумент `--service-endpoint-policy` в команду `network vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-191">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="70ea7-192">Роль</span><span class="sxs-lookup"><span data-stu-id="70ea7-192">Role</span></span>
* <span data-ttu-id="70ea7-193">Добавлена поддержка для списка владельцев приложения Azure AD в команду `ad app owner`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-193">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="70ea7-194">Добавлена поддержка для списка владельцев субъекта-службы Azure AD в команду `ad sp owner`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-194">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="70ea7-195">Изменены команды для создания и обновления определений ролей, которые теперь принимают несколько конфигураций разрешений.</span><span class="sxs-lookup"><span data-stu-id="70ea7-195">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="70ea7-196">Изменена команда `ad sp create-for-rbac`, чтобы универсальный код ресурса (URI) для домашней страницы всегда начинался с https.</span><span class="sxs-lookup"><span data-stu-id="70ea7-196">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="70ea7-197">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="70ea7-197">Service Bus</span></span>
* <span data-ttu-id="70ea7-198">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="70ea7-198">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="70ea7-199">ВМ</span><span class="sxs-lookup"><span data-stu-id="70ea7-199">VM</span></span>
* <span data-ttu-id="70ea7-200">Исправлено пустое поле `accessSas` в `disk grant-access`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-200">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="70ea7-201">Изменена команда `vmss create`, которая теперь резервирует достаточно большой диапазон внешних портов для обработки избыточной подготовки.</span><span class="sxs-lookup"><span data-stu-id="70ea7-201">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="70ea7-202">Исправлены команды обновления для `sig`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-202">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="70ea7-203">Добавлена поддержка `--no-wait` для управления версиями образов в `sig`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-203">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="70ea7-204">Изменена команда `vm list-ip-addresses` для отображения зоны доступности общедоступного IP-адреса.</span><span class="sxs-lookup"><span data-stu-id="70ea7-204">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="70ea7-205">Изменена команда `[vm|vmss] disk attach`, которая теперь по умолчанию устанавливает для логического номера диска первое доступно значение.</span><span class="sxs-lookup"><span data-stu-id="70ea7-205">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="70ea7-206">21 сентября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70ea7-206">September 21, 2018</span></span>

<span data-ttu-id="70ea7-207">Версия 2.0.46</span><span class="sxs-lookup"><span data-stu-id="70ea7-207">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="70ea7-208">ACR</span><span class="sxs-lookup"><span data-stu-id="70ea7-208">ACR</span></span>
* <span data-ttu-id="70ea7-209">Добавлены команды задач ACR.</span><span class="sxs-lookup"><span data-stu-id="70ea7-209">Added ACR Task commands</span></span>
* <span data-ttu-id="70ea7-210">Добавлена команда быстрого запуска.</span><span class="sxs-lookup"><span data-stu-id="70ea7-210">Added quick run command</span></span>
* <span data-ttu-id="70ea7-211">Группа команд `build-task` не рекомендуется к использованию.</span><span class="sxs-lookup"><span data-stu-id="70ea7-211">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="70ea7-212">Добавлена группа команд `helm` для поддержки управления чартами Helm в ACR.</span><span class="sxs-lookup"><span data-stu-id="70ea7-212">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="70ea7-213">Добавлена поддержка создания идемпотентных элементов для управляемого реестра.</span><span class="sxs-lookup"><span data-stu-id="70ea7-213">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="70ea7-214">Добавлен флаг отсутствия форматирования для отображения журналов сборки.</span><span class="sxs-lookup"><span data-stu-id="70ea7-214">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="70ea7-215">ACS</span><span class="sxs-lookup"><span data-stu-id="70ea7-215">ACS</span></span>
* <span data-ttu-id="70ea7-216">Изменена команда `install-connector` для указания главного полного доменного имени в AKS.</span><span class="sxs-lookup"><span data-stu-id="70ea7-216">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="70ea7-217">Исправлена ошибка при назначении ролей для идентификатора подсети виртуальной сети, если не указан субъект-служба и пропущен шаг назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="70ea7-217">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="70ea7-218">AppService</span><span class="sxs-lookup"><span data-stu-id="70ea7-218">AppService</span></span>

* <span data-ttu-id="70ea7-219">Добавлена поддержка операций управления веб-заданиями (как непрерывных, так и активируемых).</span><span class="sxs-lookup"><span data-stu-id="70ea7-219">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="70ea7-220">Добавлена поддержка свойства fts-state в az webapp config set. Также добавлена поддержка команд az functionapp config set и az functionapp config show.</span><span class="sxs-lookup"><span data-stu-id="70ea7-220">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="70ea7-221">Добавлена возможность использования собственного хранилища для веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="70ea7-221">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="70ea7-222">Добавлена возможность вывода списка удаленных веб-приложений и их восстановления.</span><span class="sxs-lookup"><span data-stu-id="70ea7-222">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="70ea7-223">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="70ea7-223">Batch</span></span>
* <span data-ttu-id="70ea7-224">Изменена функция добавления задач с помощью `--json-file` для поддержки синтаксиса AddTaskCollectionParameter.</span><span class="sxs-lookup"><span data-stu-id="70ea7-224">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="70ea7-225">Обновлена документация в принятом формате `--json-file`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-225">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="70ea7-226">Добавлен параметр `--max-tasks-per-node-option` для команды `batch pool create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-226">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="70ea7-227">Изменен режим работы `batch account` на отображение учетной записи, в которую выполнен вход, если не заданы другие параметры.</span><span class="sxs-lookup"><span data-stu-id="70ea7-227">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="70ea7-228">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="70ea7-228">Batch AI</span></span> 
* <span data-ttu-id="70ea7-229">Исправлен сбой при автоматическом создании учетной записи хранения при выполнении команды `batchai cluster create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-229">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="70ea7-230">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="70ea7-230">Cognitive Services</span></span>
* <span data-ttu-id="70ea7-231">Добавлено средство заполнения для аргументов `--sku`, `--kind` и `--location`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-231">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="70ea7-232">Добавлена команда `cognitiveservices account list-usage`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-232">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="70ea7-233">Добавлена команда `cognitiveservices account list-kinds`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-233">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="70ea7-234">Добавлена команда `cognitiveservices account list`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-234">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="70ea7-235">Команда `cognitiveservices list` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="70ea7-235">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="70ea7-236">Изменен параметр `--name`, который теперь является необязательным для `cognitiveservices account list-skus`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-236">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="70ea7-237">Контейнер</span><span class="sxs-lookup"><span data-stu-id="70ea7-237">Container</span></span>
* <span data-ttu-id="70ea7-238">Добавлена возможность перезапуска и остановки выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="70ea7-238">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="70ea7-239">Добавлен параметр `--network-profile` для передачи в сетевой профиль.</span><span class="sxs-lookup"><span data-stu-id="70ea7-239">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="70ea7-240">Добавлены параметры `--subnet` и `--vnet_name` для создания групп контейнеров в виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="70ea7-240">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="70ea7-241">Изменены табличные выходные данные для отображения состояния группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="70ea7-241">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="70ea7-242">Data Lake</span><span class="sxs-lookup"><span data-stu-id="70ea7-242">Datalake</span></span>
* <span data-ttu-id="70ea7-243">Добавлены команды для правил виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="70ea7-243">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="70ea7-244">Интерактивная оболочка</span><span class="sxs-lookup"><span data-stu-id="70ea7-244">Interactive Shell</span></span>
* <span data-ttu-id="70ea7-245">Исправлена ошибка в Windows, связанная со сбоем при выполнении команд.</span><span class="sxs-lookup"><span data-stu-id="70ea7-245">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="70ea7-246">Исправлена проблема с загрузкой команд в интерактивной оболочке из-за использования нерекомендуемых объектов.</span><span class="sxs-lookup"><span data-stu-id="70ea7-246">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="70ea7-247">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="70ea7-247">IoT</span></span>
* <span data-ttu-id="70ea7-248">Добавлена поддержка маршрутизации Центров Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="70ea7-248">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="70ea7-249">Key Vault</span><span class="sxs-lookup"><span data-stu-id="70ea7-249">Key Vault</span></span>
* <span data-ttu-id="70ea7-250">Исправлена ошибка импорта ключа в Key Vault для ключей RSA.</span><span class="sxs-lookup"><span data-stu-id="70ea7-250">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="70ea7-251">Сеть</span><span class="sxs-lookup"><span data-stu-id="70ea7-251">Network</span></span>
* <span data-ttu-id="70ea7-252">Добавлены команды `network public-ip prefix` для поддержки операций с префиксами общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="70ea7-252">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="70ea7-253">Добавлены команды `network service-endpoint` для поддержки операций с политиками конечной точки службы.</span><span class="sxs-lookup"><span data-stu-id="70ea7-253">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="70ea7-254">Добавлены команды `network lb outbound-rule` для поддержки создания правил для исходящего трафика в Load Balancer (цен. категория "Стандартный").</span><span class="sxs-lookup"><span data-stu-id="70ea7-254">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="70ea7-255">Добавлен параметр `--public-ip-prefix` для `network lb frontend-ip create/update` для поддержки конфигурации IP внешнего интерфейса с помощью префиксов общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="70ea7-255">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="70ea7-256">Добавлен параметр `--enable-tcp-reset` для `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-256">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="70ea7-257">Добавлен параметр `--disable-outbound-snat` для `network lb rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-257">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="70ea7-258">Добавлена возможность использования `network watcher flow-log show/configure` с классическими группами безопасности сети.</span><span class="sxs-lookup"><span data-stu-id="70ea7-258">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="70ea7-259">Добавлена команда `network watcher run-configuration-diagnostic`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-259">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="70ea7-260">Исправлена команда `network watcher test-connectivity` и добавлены свойства `--method`, `--valid-status-codes` и `--headers`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-260">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="70ea7-261">`network express-route create/update`: добавлен флаг `--allow-global-reach`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-261">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="70ea7-262">`network vnet subnet create/update`: добавлена поддержка `--delegation`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-262">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="70ea7-263">Добавлена команда `network vnet subnet list-available-delegations`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-263">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="70ea7-264">`network traffic-manager profile create/update`: добавлена поддержка `--interval`, `--timeout` и `--max-failures` для конфигурации мониторинга. Не рекомендуются к использованию параметры`--monitor-path`, `--monitor-port` и `--monitor-protocol`, которые следует заменить на `--path`, `--port` и `--protocol`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-264">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="70ea7-265">`network lb frontend-ip create/update`: исправлена логика указания метода распределения частных IP-адресов. Если назначается частный IP-адрес, он назначается статически. Если частный IP-адрес не назначается или строка с данными о частных IP-адресах не заполнена, происходит динамическое распределение.</span><span class="sxs-lookup"><span data-stu-id="70ea7-265">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="70ea7-266">`dns record-set * create/update`: добавлена поддержка `--target-resource`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-266">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="70ea7-267">Добавлены команды `network interface-endpoint` для обращения к объектам конечных точек интерфейса.</span><span class="sxs-lookup"><span data-stu-id="70ea7-267">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="70ea7-268">Добавлено `network profile show/list/delete` для частичного управления сетевыми профилями.</span><span class="sxs-lookup"><span data-stu-id="70ea7-268">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="70ea7-269">Добавлено `network express-route peering connection` для управления пиринговыми подключениями через ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="70ea7-269">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="70ea7-270">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="70ea7-270">RDBMS</span></span>
* <span data-ttu-id="70ea7-271">Добавлена поддержка MariaDB.</span><span class="sxs-lookup"><span data-stu-id="70ea7-271">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="70ea7-272">резервирование.</span><span class="sxs-lookup"><span data-stu-id="70ea7-272">Reservation</span></span>
* <span data-ttu-id="70ea7-273">База данных CosmosDB добавлена в тип перечисления зарезервированных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="70ea7-273">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="70ea7-274">Добавлено свойство имени в модели Patch.</span><span class="sxs-lookup"><span data-stu-id="70ea7-274">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="70ea7-275">Управление приложением</span><span class="sxs-lookup"><span data-stu-id="70ea7-275">Manage App</span></span>
* <span data-ttu-id="70ea7-276">Исправлена ошибка в `managedapp create --kind MarketPlace`, приводившая к аварийному завершению создания экземпляра управляемого приложения Marketplace.</span><span class="sxs-lookup"><span data-stu-id="70ea7-276">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="70ea7-277">Изменены команды`feature`, действие которых теперь ограничено поддерживаемыми профилями.</span><span class="sxs-lookup"><span data-stu-id="70ea7-277">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="70ea7-278">Роль</span><span class="sxs-lookup"><span data-stu-id="70ea7-278">Role</span></span>
* <span data-ttu-id="70ea7-279">Добавлена функция перечисления членства пользователя в группах.</span><span class="sxs-lookup"><span data-stu-id="70ea7-279">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="70ea7-280">SignalR</span><span class="sxs-lookup"><span data-stu-id="70ea7-280">SignalR</span></span>
* <span data-ttu-id="70ea7-281">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="70ea7-281">First release</span></span>

### <a name="storage"></a><span data-ttu-id="70ea7-282">Хранилище</span><span class="sxs-lookup"><span data-stu-id="70ea7-282">Storage</span></span>
* <span data-ttu-id="70ea7-283">Добавлен параметр `--auth-mode login` для использования учетных данных пользователя для авторизации в больших двоичных объектах и очереди.</span><span class="sxs-lookup"><span data-stu-id="70ea7-283">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="70ea7-284">Добавлена команда `storage container immutability-policy/legal-hold` для управления неизменяемым хранилищем.</span><span class="sxs-lookup"><span data-stu-id="70ea7-284">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="70ea7-285">ВМ</span><span class="sxs-lookup"><span data-stu-id="70ea7-285">VM</span></span>
* <span data-ttu-id="70ea7-286">Исправлена ошибка, при которой команда `vm create --generate-ssh-keys` перезаписывала файл закрытого ключа, если отсутствовал файл открытого ключа (#4725, #6780).</span><span class="sxs-lookup"><span data-stu-id="70ea7-286">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="70ea7-287">Добавлена поддержка общей коллекции изображений с помощью команды `az sig`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-287">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="70ea7-288">28 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70ea7-288">August 28, 2018</span></span>

<span data-ttu-id="70ea7-289">Версия 2.0.45</span><span class="sxs-lookup"><span data-stu-id="70ea7-289">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="70ea7-290">Core</span><span class="sxs-lookup"><span data-stu-id="70ea7-290">Core</span></span>

* <span data-ttu-id="70ea7-291">Исправлена проблема с загрузкой пустого файла конфигурации.</span><span class="sxs-lookup"><span data-stu-id="70ea7-291">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="70ea7-292">Добавлена поддержка профиля `2018-03-01-hybrid` для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="70ea7-292">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="70ea7-293">ACR</span><span class="sxs-lookup"><span data-stu-id="70ea7-293">ACR</span></span>

* <span data-ttu-id="70ea7-294">Добавлено решение для операций среды выполнения без запросов ARM.</span><span class="sxs-lookup"><span data-stu-id="70ea7-294">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="70ea7-295">Внесено изменение для исключения файлов управления версиями (например, файлов с расширениями .git, .gitignore) из отправляемого файла с расширением .tar по умолчанию для команды `build`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-295">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="70ea7-296">ACS</span><span class="sxs-lookup"><span data-stu-id="70ea7-296">ACS</span></span>

* <span data-ttu-id="70ea7-297">Внесено изменение в `aks create` с заменой параметрами по умолчанию для виртуальных машин `Standard_DS2_v2`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-297">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="70ea7-298">Внесено изменение в `aks get-credentials` для вызова новых API и получения учетных данных кластера.</span><span class="sxs-lookup"><span data-stu-id="70ea7-298">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="70ea7-299">AppService</span><span class="sxs-lookup"><span data-stu-id="70ea7-299">AppService</span></span>

* <span data-ttu-id="70ea7-300">Добавлена поддержка CORS в приложениях-функциях и веб-приложениях.</span><span class="sxs-lookup"><span data-stu-id="70ea7-300">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="70ea7-301">Добавлена поддержка тегов ARM для команды создания.</span><span class="sxs-lookup"><span data-stu-id="70ea7-301">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="70ea7-302">Внесено изменение в `[webapp|functionapp] identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="70ea7-302">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="70ea7-303">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="70ea7-303">Backup</span></span>

* <span data-ttu-id="70ea7-304">Внесено изменение в `backup vault backup-properties show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="70ea7-304">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="70ea7-305">Служба Bot Service</span><span class="sxs-lookup"><span data-stu-id="70ea7-305">Bot Service</span></span>

* <span data-ttu-id="70ea7-306">Начальный выпуск CLI для службы Azure Bot</span><span class="sxs-lookup"><span data-stu-id="70ea7-306">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="70ea7-307">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="70ea7-307">Cognitive Services</span></span>

* <span data-ttu-id="70ea7-308">Добавлен новый параметр `--api-properties,`, требуемый для создания некоторых служб.</span><span class="sxs-lookup"><span data-stu-id="70ea7-308">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="70ea7-309">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="70ea7-309">IoT</span></span>

* <span data-ttu-id="70ea7-310">Исправлена проблема со связыванием связанных центров.</span><span class="sxs-lookup"><span data-stu-id="70ea7-310">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="70ea7-311">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="70ea7-311">Monitor</span></span>

* <span data-ttu-id="70ea7-312">Добавлены команды `monitor metrics alert` для создания оповещений метрик почти в реальном времени.</span><span class="sxs-lookup"><span data-stu-id="70ea7-312">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="70ea7-313">Команды `monitor alert` не рекомендуются к использованию.</span><span class="sxs-lookup"><span data-stu-id="70ea7-313">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="70ea7-314">Сеть</span><span class="sxs-lookup"><span data-stu-id="70ea7-314">Network</span></span>

* <span data-ttu-id="70ea7-315">Внесено изменение в `network application-gateway ssl-policy predefined show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="70ea7-315">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="70ea7-316">Ресурс</span><span class="sxs-lookup"><span data-stu-id="70ea7-316">Resource</span></span>

* <span data-ttu-id="70ea7-317">Внесено изменение в `provider operation show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="70ea7-317">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="70ea7-318">Хранилище</span><span class="sxs-lookup"><span data-stu-id="70ea7-318">Storage</span></span>

* <span data-ttu-id="70ea7-319">Внесено изменение в `storage share policy show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="70ea7-319">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="70ea7-320">ВМ</span><span class="sxs-lookup"><span data-stu-id="70ea7-320">VM</span></span>

* <span data-ttu-id="70ea7-321">Внесено изменение в `vm/vmss identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="70ea7-321">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="70ea7-322">`--storage-caching` не рекомендуется к использованию для `vm create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-322">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="70ea7-323">14 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70ea7-323">Auguest 14, 2018</span></span>

<span data-ttu-id="70ea7-324">Версия 2.0.44</span><span class="sxs-lookup"><span data-stu-id="70ea7-324">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="70ea7-325">Core</span><span class="sxs-lookup"><span data-stu-id="70ea7-325">Core</span></span>

* <span data-ttu-id="70ea7-326">Исправлено отображение чисел в выходных данных `table`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-326">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="70ea7-327">Добавлен формат выходных данных YAML.</span><span class="sxs-lookup"><span data-stu-id="70ea7-327">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="70ea7-328">Телеметрия</span><span class="sxs-lookup"><span data-stu-id="70ea7-328">Telemetry</span></span>

* <span data-ttu-id="70ea7-329">Улучшены функции отчетности телеметрии.</span><span class="sxs-lookup"><span data-stu-id="70ea7-329">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="70ea7-330">ACR</span><span class="sxs-lookup"><span data-stu-id="70ea7-330">ACR</span></span>

* <span data-ttu-id="70ea7-331">Добавлены команды `content-trust policy`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-331">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="70ea7-332">Исправлена проблема с правильной обработкой `.dockerignore`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-332">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="70ea7-333">ACS</span><span class="sxs-lookup"><span data-stu-id="70ea7-333">ACS</span></span>

* <span data-ttu-id="70ea7-334">Внесено изменение в `az acs/aks install-cli` для установки в разделе `%USERPROFILE%\.azure-kubectl` в Windows.</span><span class="sxs-lookup"><span data-stu-id="70ea7-334">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="70ea7-335">Внесено изменение в `az aks install-connector` для определения RBAC в кластере и правильной настройки соединителя ACI.</span><span class="sxs-lookup"><span data-stu-id="70ea7-335">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="70ea7-336">Внесено изменение в назначение ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="70ea7-336">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="70ea7-337">Внесен новый параметр пропуска назначения ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="70ea7-337">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="70ea7-338">Внесено изменение в параметр пропуска назначения ролей для подсети, если назначение уже существует.</span><span class="sxs-lookup"><span data-stu-id="70ea7-338">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="70ea7-339">AppService</span><span class="sxs-lookup"><span data-stu-id="70ea7-339">AppService</span></span>

* <span data-ttu-id="70ea7-340">Исправлена ошибка с созданием приложения-функции с помощью учетных записей хранения во внешних группах ресурсов.</span><span class="sxs-lookup"><span data-stu-id="70ea7-340">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="70ea7-341">Исправлен сбой при развертывании ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="70ea7-341">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="70ea7-342">Batch AI</span><span class="sxs-lookup"><span data-stu-id="70ea7-342">BatchAI</span></span>

* <span data-ttu-id="70ea7-343">Внесены изменения в выходные данные средства ведения журнала для автоматического создания учетной записи хранения и определения *группы ресурсов*.</span><span class="sxs-lookup"><span data-stu-id="70ea7-343">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="70ea7-344">Контейнер</span><span class="sxs-lookup"><span data-stu-id="70ea7-344">Container</span></span>

* <span data-ttu-id="70ea7-345">Добавлено `--secure-environment-variables` для передачи переменных среды в контейнер.</span><span class="sxs-lookup"><span data-stu-id="70ea7-345">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="70ea7-346">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="70ea7-346">IoT</span></span>

* <span data-ttu-id="70ea7-347">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены устаревшие команды, которые были перемещены в расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="70ea7-347">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="70ea7-348">Обновлены элементы для игнорирования домена `azure-devices.net`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-348">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="70ea7-349">IoT Central</span><span class="sxs-lookup"><span data-stu-id="70ea7-349">Iot Central</span></span>

* <span data-ttu-id="70ea7-350">Начальный выпуск модуля IoT Central</span><span class="sxs-lookup"><span data-stu-id="70ea7-350">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="70ea7-351">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="70ea7-351">KeyVault</span></span>


* <span data-ttu-id="70ea7-352">Добавлены команды для управления учетными записями хранения и определений SAS.</span><span class="sxs-lookup"><span data-stu-id="70ea7-352">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="70ea7-353">Добавлены команды для правил сети.</span><span class="sxs-lookup"><span data-stu-id="70ea7-353">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="70ea7-354">Добавлен параметр `--id` для операций с секретами, ключами и сертификатами.</span><span class="sxs-lookup"><span data-stu-id="70ea7-354">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="70ea7-355">Добавлена поддержка версии с несколькими API управления хранилищем ключей.</span><span class="sxs-lookup"><span data-stu-id="70ea7-355">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="70ea7-356">Добавлена поддержка версии с несколькими API плоскости данных хранилища ключей.</span><span class="sxs-lookup"><span data-stu-id="70ea7-356">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="70ea7-357">Передача</span><span class="sxs-lookup"><span data-stu-id="70ea7-357">Relay</span></span>

* <span data-ttu-id="70ea7-358">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="70ea7-358">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="70ea7-359">SQL</span><span class="sxs-lookup"><span data-stu-id="70ea7-359">Sql</span></span>

* <span data-ttu-id="70ea7-360">Добавлены команды `sql failover-group`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-360">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="70ea7-361">Хранилище</span><span class="sxs-lookup"><span data-stu-id="70ea7-361">Storage</span></span>

* <span data-ttu-id="70ea7-362">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `storage account show-usage` для запроса параметра `--location` и отображения по регионам.</span><span class="sxs-lookup"><span data-stu-id="70ea7-362">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="70ea7-363">Внесено изменение в параметр `--resource-group` для команд `storage account`, который теперь необязателен.</span><span class="sxs-lookup"><span data-stu-id="70ea7-363">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="70ea7-364">Удалены предупреждения о нарушении необходимого условия для отдельных сбоев в командах пакетной службы для одного сообщения.</span><span class="sxs-lookup"><span data-stu-id="70ea7-364">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="70ea7-365">Внесено изменение в команды `[blob|file] delete-batch`, которые больше не выводят выходной массив значений NULL.</span><span class="sxs-lookup"><span data-stu-id="70ea7-365">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="70ea7-366">Внесено изменение в команды `blob [download|upload|delete-batch]`, которые теперь считывают маркер SAS из URL-адреса контейнера.</span><span class="sxs-lookup"><span data-stu-id="70ea7-366">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="70ea7-367">ВМ</span><span class="sxs-lookup"><span data-stu-id="70ea7-367">VM</span></span>

* <span data-ttu-id="70ea7-368">Добавлены общие фильтры для `vm list-skus` для удобства использования.</span><span class="sxs-lookup"><span data-stu-id="70ea7-368">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="70ea7-369">31 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70ea7-369">July 31, 2018</span></span>

<span data-ttu-id="70ea7-370">Версия 2.0.43</span><span class="sxs-lookup"><span data-stu-id="70ea7-370">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="70ea7-371">ACR</span><span class="sxs-lookup"><span data-stu-id="70ea7-371">ACR</span></span>

* <span data-ttu-id="70ea7-372">В команду `acr build-task show` добавлен флаг `--with-secure-properties`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-372">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="70ea7-373">Добавлена команда `acr build-task update-build`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-373">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="70ea7-374">ACS</span><span class="sxs-lookup"><span data-stu-id="70ea7-374">ACS</span></span>

* <span data-ttu-id="70ea7-375">При завершении команды `az aks browse` нажатием клавиш CTRL + C теперь возвращается значение 0 (успешное завершение).</span><span class="sxs-lookup"><span data-stu-id="70ea7-375">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="70ea7-376">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="70ea7-376">Batch</span></span>

* <span data-ttu-id="70ea7-377">Исправлена ошибка при отображении маркера AAD в CloudShell.</span><span class="sxs-lookup"><span data-stu-id="70ea7-377">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="70ea7-378">Контейнер</span><span class="sxs-lookup"><span data-stu-id="70ea7-378">Container</span></span>

* <span data-ttu-id="70ea7-379">Удалено требование указания `--log-analytics-workspace-key` для имени или идентификатора при выборе подписки.</span><span class="sxs-lookup"><span data-stu-id="70ea7-379">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="70ea7-380">Сеть</span><span class="sxs-lookup"><span data-stu-id="70ea7-380">Network</span></span>

* <span data-ttu-id="70ea7-381">В профиль 2017-03-09-profile для Azure Stack добавлена поддержка DNS.</span><span class="sxs-lookup"><span data-stu-id="70ea7-381">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="70ea7-382">Ресурс</span><span class="sxs-lookup"><span data-stu-id="70ea7-382">Resource</span></span>

* <span data-ttu-id="70ea7-383">В `group deployment create` добавлен параметр `--rollback-on-error` для выполнения достоверно корректного развертывания в случае возникновения ошибки.</span><span class="sxs-lookup"><span data-stu-id="70ea7-383">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="70ea7-384">Исправлена проблема, из-за которой использование `--parameters {}` с `group deployment create` приводило к ошибке.</span><span class="sxs-lookup"><span data-stu-id="70ea7-384">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="70ea7-385">Роль</span><span class="sxs-lookup"><span data-stu-id="70ea7-385">Role</span></span>

* <span data-ttu-id="70ea7-386">Добавлена поддержка профиля 2017-03-09-profile для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="70ea7-386">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="70ea7-387">Исправлена проблема, из-за которой универсальные параметры обновления `app update` работали неправильно.</span><span class="sxs-lookup"><span data-stu-id="70ea7-387">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="70ea7-388">поиска</span><span class="sxs-lookup"><span data-stu-id="70ea7-388">Search</span></span>

* <span data-ttu-id="70ea7-389">Добавлены команды для службы "Поиск Azure".</span><span class="sxs-lookup"><span data-stu-id="70ea7-389">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="70ea7-390">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="70ea7-390">Service Bus</span></span>

* <span data-ttu-id="70ea7-391">Добавлена группа команд migration для переноса пространства имен из служебной шины ценовой категории "Стандартный" в служебную шину ценовой категории "Премиум".</span><span class="sxs-lookup"><span data-stu-id="70ea7-391">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="70ea7-392">Добавлены новые необязательные свойства для очереди и подписки служебной шины:</span><span class="sxs-lookup"><span data-stu-id="70ea7-392">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="70ea7-393">`--enable-batched-operations` и `--enable-dead-lettering-on-message-expiration` в `queue`;</span><span class="sxs-lookup"><span data-stu-id="70ea7-393">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="70ea7-394">`--dead-letter-on-filter-exceptions` в `subscriptions`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-394">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="70ea7-395">Хранилище</span><span class="sxs-lookup"><span data-stu-id="70ea7-395">Storage</span></span>

* <span data-ttu-id="70ea7-396">Добавлена поддержка скачивания больших файлов с помощью одного подключения.</span><span class="sxs-lookup"><span data-stu-id="70ea7-396">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="70ea7-397">Преобразованы команды `show`, которые ранее отсутствовали: теперь в случае отсутствия ресурса не возвращается код завершения 3.</span><span class="sxs-lookup"><span data-stu-id="70ea7-397">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="70ea7-398">ВМ</span><span class="sxs-lookup"><span data-stu-id="70ea7-398">VM</span></span>

* <span data-ttu-id="70ea7-399">Добавлена поддержка вывода списка групп доступности по подпискам.</span><span class="sxs-lookup"><span data-stu-id="70ea7-399">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="70ea7-400">Добавлена поддержка параметра `StandardSSD_LRS`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-400">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="70ea7-401">Добавлена поддержка групп безопасности приложений при создании масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="70ea7-401">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="70ea7-402">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены `[vm|vmss] create`, `[vm|vmss] identity assign` и `[vm|vmss] identity remove` для вывода пользовательских удостоверений в формате словаря.</span><span class="sxs-lookup"><span data-stu-id="70ea7-402">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="70ea7-403">18 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70ea7-403">July 18, 2018</span></span>

<span data-ttu-id="70ea7-404">Версия 2.0.42</span><span class="sxs-lookup"><span data-stu-id="70ea7-404">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="70ea7-405">Core</span><span class="sxs-lookup"><span data-stu-id="70ea7-405">Core</span></span>

* <span data-ttu-id="70ea7-406">Добавлена поддержка входа в окно WSL bash из браузера.</span><span class="sxs-lookup"><span data-stu-id="70ea7-406">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="70ea7-407">Добавлен флаг `--force-string` для всех универсальных команд обновления.</span><span class="sxs-lookup"><span data-stu-id="70ea7-407">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="70ea7-408">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды show: сообщения об ошибках записываются в журнал, а команды возвращают код выхода 3, если ресурс отсутствует.</span><span class="sxs-lookup"><span data-stu-id="70ea7-408">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="70ea7-409">ACR</span><span class="sxs-lookup"><span data-stu-id="70ea7-409">ACR</span></span>

* <span data-ttu-id="70ea7-410">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр --no-push в команде acr build сделан обычным флагом.</span><span class="sxs-lookup"><span data-stu-id="70ea7-410">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="70ea7-411">В группу `acr repository` добавлены команды `show` и `update`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-411">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="70ea7-412">Добавлен флаг `--detail` для `show-manifests` и `show-tags`, позволяющий выводить более подробные сведения.</span><span class="sxs-lookup"><span data-stu-id="70ea7-412">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="70ea7-413">Добавлен параметр `--image`, позволяющий получать сведения о сборке или журналы для определенного образа.</span><span class="sxs-lookup"><span data-stu-id="70ea7-413">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="70ea7-414">ACS</span><span class="sxs-lookup"><span data-stu-id="70ea7-414">ACS</span></span>

* <span data-ttu-id="70ea7-415">Поведение `az aks create` изменено так, чтобы выдавалась ошибка, если `--max-pods` меньше 5.</span><span class="sxs-lookup"><span data-stu-id="70ea7-415">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="70ea7-416">AppService</span><span class="sxs-lookup"><span data-stu-id="70ea7-416">AppService</span></span>

* <span data-ttu-id="70ea7-417">Добавлена поддержка номеров SKU для PremiumV2.</span><span class="sxs-lookup"><span data-stu-id="70ea7-417">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="70ea7-418">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="70ea7-418">Batch</span></span>

* <span data-ttu-id="70ea7-419">Исправлена ошибка при использовании учетных данных токена в режиме Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="70ea7-419">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="70ea7-420">Регистр во входных данных JSON теперь не учитывается.</span><span class="sxs-lookup"><span data-stu-id="70ea7-420">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="70ea7-421">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="70ea7-421">Batch AI</span></span>

* <span data-ttu-id="70ea7-422">Исправлена команда `az batchai job exec`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-422">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="70ea7-423">Контейнер</span><span class="sxs-lookup"><span data-stu-id="70ea7-423">Container</span></span>

* <span data-ttu-id="70ea7-424">Удалено требование указывать имя пользователя и пароль для реестров, не связанных с dockerhub.</span><span class="sxs-lookup"><span data-stu-id="70ea7-424">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="70ea7-425">Исправлена ошибка, возникающая при создании групп контейнеров из файла YAML.</span><span class="sxs-lookup"><span data-stu-id="70ea7-425">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="70ea7-426">Сеть</span><span class="sxs-lookup"><span data-stu-id="70ea7-426">Network</span></span>

* <span data-ttu-id="70ea7-427">В команду `network nic [create|update|delete]` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-427">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="70ea7-428">Добавлена команда `network nic wait`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-428">Added `network nic wait`</span></span>
* <span data-ttu-id="70ea7-429">Аргумент `--ids` команды `network vnet [subnet|peering] list` объявлен устаревшим.</span><span class="sxs-lookup"><span data-stu-id="70ea7-429">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="70ea7-430">Добавлен флаг `--include-default`, позволяющий включать в выходные данные команды `network nsg rule list` стандартные правила безопасности.</span><span class="sxs-lookup"><span data-stu-id="70ea7-430">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="70ea7-431">Ресурс</span><span class="sxs-lookup"><span data-stu-id="70ea7-431">Resource</span></span>

* <span data-ttu-id="70ea7-432">В команду `group deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-432">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="70ea7-433">В команду `deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-433">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="70ea7-434">Добавлена команда `deployment wait`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-434">Added `deployment wait` command</span></span>
* <span data-ttu-id="70ea7-435">Исправлена проблема, когда для профиля 2017-03-09-profile по ошибке отображались команды `az deployment` для работы с подписками.</span><span class="sxs-lookup"><span data-stu-id="70ea7-435">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="70ea7-436">SQL</span><span class="sxs-lookup"><span data-stu-id="70ea7-436">SQL</span></span>

* <span data-ttu-id="70ea7-437">Исправлена ошибка "The provided resource group name ... did not match the name in the Url" (Указанное имя группы ресурсов ... не соответствовало имени в URL-адресе), которая возникала при указании имени эластичного пула для команд `sql db copy` и `sql db replica create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-437">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="70ea7-438">Разрешена настройка сервера SQL Server по умолчанию с помощью команды `az configure --defaults sql-server=<name>`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-438">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="70ea7-439">Реализованы модули форматирования таблиц для команд `sql server`, `sql server firewall-rule`, `sql list-usages` и `sql show-usage`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-439">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="70ea7-440">Хранилище</span><span class="sxs-lookup"><span data-stu-id="70ea7-440">Storage</span></span>

* <span data-ttu-id="70ea7-441">В выходные данные команды `storage blob show` добавлено свойство `pageRanges`, которое будет заполняться для страничных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="70ea7-441">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="70ea7-442">ВМ</span><span class="sxs-lookup"><span data-stu-id="70ea7-442">VM</span></span>

* <span data-ttu-id="70ea7-443">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] По умолчанию команда `vmss create` теперь использует `Standard_DS1_v2` как размер экземпляра по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="70ea7-443">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="70ea7-444">Добавлена поддержка параметра `--no-wait` для `vm extension [set|delete]` и `vmss extension [set|delete]`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-444">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="70ea7-445">Добавлена команда `vm extension wait`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-445">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="70ea7-446">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70ea7-446">July 3, 2018</span></span>

<span data-ttu-id="70ea7-447">Версия 2.0.41</span><span class="sxs-lookup"><span data-stu-id="70ea7-447">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="70ea7-448">AKS</span><span class="sxs-lookup"><span data-stu-id="70ea7-448">AKS</span></span>

* <span data-ttu-id="70ea7-449">Теперь для мониторинга используется идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="70ea7-449">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="70ea7-450">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70ea7-450">July 3, 2018</span></span>

<span data-ttu-id="70ea7-451">Версия 2.0.40</span><span class="sxs-lookup"><span data-stu-id="70ea7-451">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="70ea7-452">Core</span><span class="sxs-lookup"><span data-stu-id="70ea7-452">Core</span></span>

* <span data-ttu-id="70ea7-453">Добавлен новый поток кода авторизации для интерактивного входа.</span><span class="sxs-lookup"><span data-stu-id="70ea7-453">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="70ea7-454">ACR</span><span class="sxs-lookup"><span data-stu-id="70ea7-454">ACR</span></span>

* <span data-ttu-id="70ea7-455">Добавлено состояние сборки опроса.</span><span class="sxs-lookup"><span data-stu-id="70ea7-455">Added polling build status</span></span>
* <span data-ttu-id="70ea7-456">Добавлена поддержка значений перечисления без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="70ea7-456">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="70ea7-457">Добавлены параметры `--top` и `--orderby` для `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-457">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="70ea7-458">ACS</span><span class="sxs-lookup"><span data-stu-id="70ea7-458">ACS</span></span>

* <span data-ttu-id="70ea7-459">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Управление доступом на основе ролей Kubernetes включено по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="70ea7-459">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="70ea7-460">Добавлен аргумент `--disable-rbac`. Аргумент `--enable-rbac` не рекомендуется использовать, так как теперь это значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="70ea7-460">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="70ea7-461">Обновлены параметры команды `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-461">Updated options for `aks browse` command.</span></span> <span data-ttu-id="70ea7-462">Добавлена поддержка параметра `--listen-port`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-462">Added `--listen-port` support</span></span>
* <span data-ttu-id="70ea7-463">Обновлен пакет диаграмм Helm по умолчанию для команды `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-463">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="70ea7-464">Используйте файл virtual-kubelet-for-aks-latest.tgz.</span><span class="sxs-lookup"><span data-stu-id="70ea7-464">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="70ea7-465">Для обновления существующего кластера добавлены команды `aks enable-addons` и `aks disable-addons`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-465">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="70ea7-466">AppService</span><span class="sxs-lookup"><span data-stu-id="70ea7-466">AppService</span></span>

* <span data-ttu-id="70ea7-467">Добавлена поддержка отключения удостоверения с помощью команды `webapp identity remove`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-467">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="70ea7-468">Удален тег `preview` для функции идентификации.</span><span class="sxs-lookup"><span data-stu-id="70ea7-468">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="70ea7-469">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="70ea7-469">Backup</span></span>

* <span data-ttu-id="70ea7-470">Обновлено определение модуля.</span><span class="sxs-lookup"><span data-stu-id="70ea7-470">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="70ea7-471">Batch AI</span><span class="sxs-lookup"><span data-stu-id="70ea7-471">BatchAI</span></span>

* <span data-ttu-id="70ea7-472">Исправлены табличные выходные данные для команд `batchai cluster node list` и `batchai job node list`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-472">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="70ea7-473">Облако</span><span class="sxs-lookup"><span data-stu-id="70ea7-473">Cloud</span></span>

* <span data-ttu-id="70ea7-474">В облачную конфигурацию добавлен суффикс сервера `acr login`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-474">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="70ea7-475">Контейнер</span><span class="sxs-lookup"><span data-stu-id="70ea7-475">Container</span></span>

* <span data-ttu-id="70ea7-476">Для команды `container create` действие по умолчанию изменено на длительную операцию.</span><span class="sxs-lookup"><span data-stu-id="70ea7-476">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="70ea7-477">Добавлены параметры Log Analytics `--log-analytics-workspace` и `--log-analytics-workspace-key`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-477">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="70ea7-478">Добавлен параметр `--protocol`, с помощью которого можно указать сетевой протокол для использования.</span><span class="sxs-lookup"><span data-stu-id="70ea7-478">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="70ea7-479">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="70ea7-479">Extension</span></span>

* <span data-ttu-id="70ea7-480">Изменена команда `extension list-available`. Теперь с ее помощью отображаются только расширения, совместимые с текущей версией CLI.</span><span class="sxs-lookup"><span data-stu-id="70ea7-480">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="70ea7-481">Сеть</span><span class="sxs-lookup"><span data-stu-id="70ea7-481">Network</span></span>

* <span data-ttu-id="70ea7-482">Исправлена проблема с зависимостью типов записей от регистра ([#6602](https://github.com/Azure/azure-cli/issues/6602)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-482">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="70ea7-483">Rdbms</span><span class="sxs-lookup"><span data-stu-id="70ea7-483">Rdbms</span></span>

* <span data-ttu-id="70ea7-484">Добавлены команды `[postgres|myql] server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-484">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="70ea7-485">Ресурс</span><span class="sxs-lookup"><span data-stu-id="70ea7-485">Resource</span></span>

* <span data-ttu-id="70ea7-486">Добавлена новая группа операций `deployment`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-486">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="70ea7-487">ВМ</span><span class="sxs-lookup"><span data-stu-id="70ea7-487">VM</span></span>

* <span data-ttu-id="70ea7-488">Добавлена поддержка удаления удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="70ea7-488">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="70ea7-489">25 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70ea7-489">June 25, 2018</span></span>

<span data-ttu-id="70ea7-490">Версия 2.0.39</span><span class="sxs-lookup"><span data-stu-id="70ea7-490">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="70ea7-491">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="70ea7-491">CLI</span></span>

* <span data-ttu-id="70ea7-492">В установщике MSI обновлена обрезка файлов, чтобы устранить проблему с установкой расширений.</span><span class="sxs-lookup"><span data-stu-id="70ea7-492">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="70ea7-493">19 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70ea7-493">June 19, 2018</span></span>

<span data-ttu-id="70ea7-494">Версия 2.0.38</span><span class="sxs-lookup"><span data-stu-id="70ea7-494">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="70ea7-495">Core</span><span class="sxs-lookup"><span data-stu-id="70ea7-495">Core</span></span>

* <span data-ttu-id="70ea7-496">Добавлена глобальная поддержка параметра `--subscription` в большинстве команд.</span><span class="sxs-lookup"><span data-stu-id="70ea7-496">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="70ea7-497">ACR</span><span class="sxs-lookup"><span data-stu-id="70ea7-497">ACR</span></span>

* <span data-ttu-id="70ea7-498">Добавлена зависимость `azure-storage-blob`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-498">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="70ea7-499">Изменена конфигурация ЦП по умолчанию с `acr build-task create`: теперь используется 2 ядра.</span><span class="sxs-lookup"><span data-stu-id="70ea7-499">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="70ea7-500">ACS</span><span class="sxs-lookup"><span data-stu-id="70ea7-500">ACS</span></span>

* <span data-ttu-id="70ea7-501">Обновлены параметры команды `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-501">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="70ea7-502">Добавлена поддержка параметра `--update`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-502">Added `--update` support</span></span>
* <span data-ttu-id="70ea7-503">Изменена команда `aks get-credentials --admin`, чтобы не заменять контекст пользователя в `$HOME/.kube/config`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-503">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="70ea7-504">В управляемых кластерах предоставляется доступное только для чтения свойство `nodeResourceGroup`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-504">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="70ea7-505">Исправлена ошибка в команде `acs browse`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-505">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="70ea7-506">Параметр `--connector-name` стал необязательным для `aks install-connector`, `aks upgrade-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-506">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="70ea7-507">Добавлены новые регионы экземпляров контейнеров Azure для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-507">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="70ea7-508">В имя выпуска и имя узла Helm добавлено нормализованное расположение для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-508">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="70ea7-509">AppService</span><span class="sxs-lookup"><span data-stu-id="70ea7-509">AppService</span></span>

* <span data-ttu-id="70ea7-510">Добавлена поддержка новых версий urllib.</span><span class="sxs-lookup"><span data-stu-id="70ea7-510">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="70ea7-511">Добавлена поддержка `functionapp create`, что позволяет использовать план службы приложений из внешних групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="70ea7-511">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="70ea7-512">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="70ea7-512">Batch</span></span>

* <span data-ttu-id="70ea7-513">Удалена зависимость `azure-batch-extensions`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-513">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="70ea7-514">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="70ea7-514">Batch AI</span></span>

* <span data-ttu-id="70ea7-515">Добавлена поддержка рабочих областей.</span><span class="sxs-lookup"><span data-stu-id="70ea7-515">Added support for workspaces.</span></span> <span data-ttu-id="70ea7-516">Рабочие области позволяют объединять кластеры, файловые серверы и эксперименты в группы без ограничений по количеству созданных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="70ea7-516">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="70ea7-517">Добавлена поддержка экспериментов.</span><span class="sxs-lookup"><span data-stu-id="70ea7-517">Added support for experiments.</span></span> <span data-ttu-id="70ea7-518">Эксперименты позволяют объединять задания в коллекции без ограничений по количеству созданных заданий.</span><span class="sxs-lookup"><span data-stu-id="70ea7-518">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="70ea7-519">Добавлена поддержка настройки `/dev/shm` для заданий, выполняющихся в контейнере Docker.</span><span class="sxs-lookup"><span data-stu-id="70ea7-519">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="70ea7-520">Добавлены команды `batchai cluster node exec` и `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-520">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="70ea7-521">Эти команды позволяют выполнять любые команды непосредственно на узлах и предоставляют функциональные возможности для перенаправления портов.</span><span class="sxs-lookup"><span data-stu-id="70ea7-521">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="70ea7-522">Добавлена поддержка параметра `--ids` в командах `batchai`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-522">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="70ea7-523">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Все кластеры и файловые серверы необходимо создавать в рабочих областях.</span><span class="sxs-lookup"><span data-stu-id="70ea7-523">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="70ea7-524">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Задания необходимо создавать в рамках экспериментов.</span><span class="sxs-lookup"><span data-stu-id="70ea7-524">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="70ea7-525">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--nfs-resource-group` из команд `cluster create` и `job create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-525">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="70ea7-526">Для подключения NFS из другой рабочей области или группы ресурсов следует указать идентификатор ARM файлового сервера с помощью параметра `--nfs`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-526">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="70ea7-527">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--cluster-resource-group` из команды `job create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-527">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="70ea7-528">Для отправки задания в кластере, относящемся к другой рабочей области или группе ресурсов, следует указать идентификатор ARM кластера с помощью параметра `--cluster`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-528">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="70ea7-529">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален атрибут `location` для заданий, кластера и файловых серверов.</span><span class="sxs-lookup"><span data-stu-id="70ea7-529">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="70ea7-530">Расположение теперь указывается как атрибут рабочей области.</span><span class="sxs-lookup"><span data-stu-id="70ea7-530">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="70ea7-531">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--location` из команд `job create`, `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-531">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="70ea7-532">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены имена коротких параметров, чтобы обеспечить согласованность интерфейса:</span><span class="sxs-lookup"><span data-stu-id="70ea7-532">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="70ea7-533">[`--config`, `-c`] переименовано в [`--config-file`, `-f`];</span><span class="sxs-lookup"><span data-stu-id="70ea7-533">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="70ea7-534">[`--cluster`, `-r`] переименовано в [`--cluster`, `-c`];</span><span class="sxs-lookup"><span data-stu-id="70ea7-534">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="70ea7-535">[`--cluster`, `-n`] переименовано в [`--cluster`, `-c`];</span><span class="sxs-lookup"><span data-stu-id="70ea7-535">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="70ea7-536">[`--job`, `-n`] переименовано в [`--job`, `-j`].</span><span class="sxs-lookup"><span data-stu-id="70ea7-536">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="70ea7-537">Карты</span><span class="sxs-lookup"><span data-stu-id="70ea7-537">Maps</span></span>

* <span data-ttu-id="70ea7-538">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесены изменения в `maps account create`. Теперь необходимо принимать условия использования — либо с помощью интерактивной командной строки, либо с помощью флага `--accept-tos`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-538">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="70ea7-539">Сеть</span><span class="sxs-lookup"><span data-stu-id="70ea7-539">Network</span></span>

* <span data-ttu-id="70ea7-540">Добавлена поддержка `https` для `network lb probe create`. [#6571](https://github.com/Azure/azure-cli/issues/6571).</span><span class="sxs-lookup"><span data-stu-id="70ea7-540">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="70ea7-541">Исправлена проблема, из-за которой в параметре `--endpoint-status` учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="70ea7-541">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="70ea7-542">#6502</span><span class="sxs-lookup"><span data-stu-id="70ea7-542">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="70ea7-543">Резервирование</span><span class="sxs-lookup"><span data-stu-id="70ea7-543">Reservations</span></span>

* <span data-ttu-id="70ea7-544">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Добавлен обязательный параметр `ReservedResourceType` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-544">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="70ea7-545">Добавлен параметр `Location` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-545">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="70ea7-546">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `kind` из команды `ReservationProperties`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-546">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="70ea7-547">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `capabilities` в команде `Catalog` переименован в `sku_properties`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-547">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="70ea7-548">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены свойства `size` и `tier` из команды `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-548">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="70ea7-549">Добавлен параметр `InstanceFlexibility` для команды `reservations reservation update`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-549">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="70ea7-550">Роль</span><span class="sxs-lookup"><span data-stu-id="70ea7-550">Role</span></span>

* <span data-ttu-id="70ea7-551">Улучшена обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="70ea7-551">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="70ea7-552">SQL</span><span class="sxs-lookup"><span data-stu-id="70ea7-552">SQL</span></span>

* <span data-ttu-id="70ea7-553">Исправлена вносившая путаницу ошибка, которая возникала при выполнении команды `az sql db list-editions` для расположения, недоступного для указанной подписки.</span><span class="sxs-lookup"><span data-stu-id="70ea7-553">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="70ea7-554">Хранилище</span><span class="sxs-lookup"><span data-stu-id="70ea7-554">Storage</span></span>

* <span data-ttu-id="70ea7-555">Выходные данные таблицы для `storage blob download` изменены на более удобочитаемые.</span><span class="sxs-lookup"><span data-stu-id="70ea7-555">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="70ea7-556">ВМ</span><span class="sxs-lookup"><span data-stu-id="70ea7-556">VM</span></span>

* <span data-ttu-id="70ea7-557">Улучшено уточнение размера виртуальной машины для поддержки ускоренной сети в `vm create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-557">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="70ea7-558">Для `vmss create` добавлено предупреждение о том, что стандартный размер виртуальной машины будет изменен с `Standard_D1_v2` на `Standard_DS1_v2`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-558">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="70ea7-559">Добавлен параметр `--force-update` для команды `[vm|vmss] extension set`, что позволяет обновлять расширение, даже если конфигурация не изменялась.</span><span class="sxs-lookup"><span data-stu-id="70ea7-559">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="70ea7-560">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70ea7-560">June 13, 2018</span></span>

<span data-ttu-id="70ea7-561">Версия 2.0.37</span><span class="sxs-lookup"><span data-stu-id="70ea7-561">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="70ea7-562">Core</span><span class="sxs-lookup"><span data-stu-id="70ea7-562">Core</span></span>

* <span data-ttu-id="70ea7-563">Улучшена интерактивная телеметрия.</span><span class="sxs-lookup"><span data-stu-id="70ea7-563">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="70ea7-564">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70ea7-564">June 13, 2018</span></span>

<span data-ttu-id="70ea7-565">Версия 2.0.36</span><span class="sxs-lookup"><span data-stu-id="70ea7-565">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="70ea7-566">AKS</span><span class="sxs-lookup"><span data-stu-id="70ea7-566">AKS</span></span>

* <span data-ttu-id="70ea7-567">В `aks create` добавлены дополнительные сетевые параметры.</span><span class="sxs-lookup"><span data-stu-id="70ea7-567">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="70ea7-568">В `aks create` добавлены аргументы для наблюдения и маршрутизации HTTP-трафика.</span><span class="sxs-lookup"><span data-stu-id="70ea7-568">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="70ea7-569">Добавлен аргумент `--no-ssh-key` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="70ea7-569">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="70ea7-570">Добавлен аргумент `--enable-rbac` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="70ea7-570">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="70ea7-571">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] В `aks create` добавлена поддержка аутентификации Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="70ea7-571">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="70ea7-572">AppService</span><span class="sxs-lookup"><span data-stu-id="70ea7-572">AppService</span></span>

* <span data-ttu-id="70ea7-573">Устранена проблема с несовместимыми версиями urllib.</span><span class="sxs-lookup"><span data-stu-id="70ea7-573">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="70ea7-574">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70ea7-574">June 5, 2018</span></span>

<span data-ttu-id="70ea7-575">Версия 2.0.35</span><span class="sxs-lookup"><span data-stu-id="70ea7-575">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="70ea7-576">Interactive</span><span class="sxs-lookup"><span data-stu-id="70ea7-576">Interactive</span></span>

* <span data-ttu-id="70ea7-577">Добавлены ограничения в зависимости интерактивного режима.</span><span class="sxs-lookup"><span data-stu-id="70ea7-577">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="70ea7-578">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70ea7-578">June 5, 2018</span></span>

<span data-ttu-id="70ea7-579">Версия 2.0.34</span><span class="sxs-lookup"><span data-stu-id="70ea7-579">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="70ea7-580">Core</span><span class="sxs-lookup"><span data-stu-id="70ea7-580">Core</span></span>

* <span data-ttu-id="70ea7-581">Добавлена поддержка перекрестных ссылок на ресурсы клиента.</span><span class="sxs-lookup"><span data-stu-id="70ea7-581">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="70ea7-582">Улучшена надежность при передаче данных телеметрии.</span><span class="sxs-lookup"><span data-stu-id="70ea7-582">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="70ea7-583">ACR</span><span class="sxs-lookup"><span data-stu-id="70ea7-583">ACR</span></span>

* <span data-ttu-id="70ea7-584">Добавлена поддержка VSTS в качестве расположения удаленного источника.</span><span class="sxs-lookup"><span data-stu-id="70ea7-584">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="70ea7-585">Добавлена команда `acr import`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-585">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="70ea7-586">AKS</span><span class="sxs-lookup"><span data-stu-id="70ea7-586">AKS</span></span>

* <span data-ttu-id="70ea7-587">Изменена команда `aks get-credentials` для создания файла конфигурации kube с более надежными разрешениями файловой системы.</span><span class="sxs-lookup"><span data-stu-id="70ea7-587">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="70ea7-588">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="70ea7-588">Batch</span></span>

* <span data-ttu-id="70ea7-589">Исправлена ошибка, связанная с форматированием таблиц при выполнении команды pool list. [[Ошибка #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="70ea7-589">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="70ea7-590">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="70ea7-590">IOT</span></span>

* <span data-ttu-id="70ea7-591">Добавлена возможность создания Центров Интернета вещей категории "Базовый".</span><span class="sxs-lookup"><span data-stu-id="70ea7-591">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="70ea7-592">Сеть</span><span class="sxs-lookup"><span data-stu-id="70ea7-592">Network</span></span>

* <span data-ttu-id="70ea7-593">Улучшена команда `network vnet peering`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-593">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="70ea7-594">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="70ea7-594">Policy Insights</span></span>

* <span data-ttu-id="70ea7-595">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="70ea7-595">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="70ea7-596">ARM</span><span class="sxs-lookup"><span data-stu-id="70ea7-596">ARM</span></span>

* <span data-ttu-id="70ea7-597">Добавлены команды `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-597">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="70ea7-598">SQL</span><span class="sxs-lookup"><span data-stu-id="70ea7-598">SQL</span></span>

* <span data-ttu-id="70ea7-599">Добавлены новые команды для управляемого экземпляра:</span><span class="sxs-lookup"><span data-stu-id="70ea7-599">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="70ea7-600">Добавлены новые команды для управляемой базы данных:</span><span class="sxs-lookup"><span data-stu-id="70ea7-600">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="70ea7-601">Хранилище</span><span class="sxs-lookup"><span data-stu-id="70ea7-601">Storage</span></span>

* <span data-ttu-id="70ea7-602">Добавлены типы MIME для JSON и JavaScript, выводимые из расширений файлов.</span><span class="sxs-lookup"><span data-stu-id="70ea7-602">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="70ea7-603">ВМ</span><span class="sxs-lookup"><span data-stu-id="70ea7-603">VM</span></span>

* <span data-ttu-id="70ea7-604">Изменена команда `vm list-skus` для использования фиксированных столбцов, а также добавлено предупреждение об удалении `Tier` и `Size`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-604">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="70ea7-605">Добавлен параметр `--accelerated-networking` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-605">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="70ea7-606">Добавлен параметр `--tags` для команды `identity create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-606">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="70ea7-607">22 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70ea7-607">May 22, 2018</span></span>

<span data-ttu-id="70ea7-608">Версия 2.0.33</span><span class="sxs-lookup"><span data-stu-id="70ea7-608">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="70ea7-609">Core</span><span class="sxs-lookup"><span data-stu-id="70ea7-609">Core</span></span>

* <span data-ttu-id="70ea7-610">Добавлена возможность включения символа `@` в имена файлов.</span><span class="sxs-lookup"><span data-stu-id="70ea7-610">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="70ea7-611">ACS</span><span class="sxs-lookup"><span data-stu-id="70ea7-611">ACS</span></span>

* <span data-ttu-id="70ea7-612">Добавлены новые команды для Dev Spaces: `aks use-dev-spaces` и `aks remove-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-612">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="70ea7-613">Исправлена опечатка в справочном сообщении.</span><span class="sxs-lookup"><span data-stu-id="70ea7-613">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="70ea7-614">AppService</span><span class="sxs-lookup"><span data-stu-id="70ea7-614">AppService</span></span>

* <span data-ttu-id="70ea7-615">Улучшены команды общего обновления.</span><span class="sxs-lookup"><span data-stu-id="70ea7-615">Improved generic update commands</span></span>
* <span data-ttu-id="70ea7-616">Добавлена поддержка асинхронного выполнения для `webapp deployment source config-zip`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-616">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="70ea7-617">Контейнер</span><span class="sxs-lookup"><span data-stu-id="70ea7-617">Container</span></span>

* <span data-ttu-id="70ea7-618">Добавлена возможность экспорта группы контейнеров в формате YAML.</span><span class="sxs-lookup"><span data-stu-id="70ea7-618">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="70ea7-619">Добавлена возможность использования файла YAML для создания или обновления группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="70ea7-619">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="70ea7-620">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="70ea7-620">Extension</span></span>

* <span data-ttu-id="70ea7-621">Улучшена операция удаления расширений.</span><span class="sxs-lookup"><span data-stu-id="70ea7-621">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="70ea7-622">Interactive</span><span class="sxs-lookup"><span data-stu-id="70ea7-622">Interactive</span></span>

* <span data-ttu-id="70ea7-623">Изменены параметры ведения журнала для отключения средства синтаксического анализа для завершенных операций.</span><span class="sxs-lookup"><span data-stu-id="70ea7-623">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="70ea7-624">Улучшена обработка поврежденных кэшей справки.</span><span class="sxs-lookup"><span data-stu-id="70ea7-624">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="70ea7-625">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="70ea7-625">KeyVault</span></span>

* <span data-ttu-id="70ea7-626">Исправлены команды хранилища ключей для работы с удостоверениями в Cloud Shell или виртуальных машинах.</span><span class="sxs-lookup"><span data-stu-id="70ea7-626">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="70ea7-627">Сеть</span><span class="sxs-lookup"><span data-stu-id="70ea7-627">Network</span></span>

* <span data-ttu-id="70ea7-628">Исправлена проблема, при которой `network watcher show-topology` не будет выполняться, если виртуальной сети или подсети присвоить имя. [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="70ea7-628">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="70ea7-629">Исправлена проблема, при которой некоторые команды `network watcher` выдают ошибку, что Наблюдатель за сетями не включен в определенных регионах. [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="70ea7-629">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="70ea7-630">SQL</span><span class="sxs-lookup"><span data-stu-id="70ea7-630">SQL</span></span>

* <span data-ttu-id="70ea7-631">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены объекты ответа, возвращаемые в результатах команд `db` и `dw`:</span><span class="sxs-lookup"><span data-stu-id="70ea7-631">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="70ea7-632">Свойство `serviceLevelObjective` переименовано на `currentServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-632">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="70ea7-633">Удалены свойства `currentServiceObjectiveId` и `requestedServiceObjectiveId`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-633">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="70ea7-634">Тип свойства `maxSizeBytes` изменен со строкового на целое число.</span><span class="sxs-lookup"><span data-stu-id="70ea7-634">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="70ea7-635">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `db` и `dw` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="70ea7-635">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="70ea7-636">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-636">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="70ea7-637">Для обновления используйте параметр `--service-objective` или задайте свойство `sku.name`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-637">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="70ea7-638">`edition`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-638">`edition`.</span></span> <span data-ttu-id="70ea7-639">Для обновления используйте параметр `--edition` или задайте свойство `sku.tier`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-639">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="70ea7-640">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-640">`elasticPoolName`.</span></span> <span data-ttu-id="70ea7-641">Для обновления используйте параметр `--elastic-pool` или задайте свойство `elasticPoolId`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-641">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="70ea7-642">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `elastic-pool` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="70ea7-642">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="70ea7-643">`edition`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-643">`edition`.</span></span> <span data-ttu-id="70ea7-644">Для обновления используйте параметр `--edition`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-644">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="70ea7-645">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-645">`dtu`.</span></span> <span data-ttu-id="70ea7-646">Для обновления используйте параметр `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-646">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="70ea7-647">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-647">`databaseDtuMin`.</span></span> <span data-ttu-id="70ea7-648">Для обновления используйте параметр `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-648">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="70ea7-649">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-649">`databaseDtuMax`.</span></span> <span data-ttu-id="70ea7-650">Для обновления используйте параметр `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-650">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="70ea7-651">Добавлены параметры `--family` и `--capacity` для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-651">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="70ea7-652">Добавлены модули форматирования таблиц для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-652">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="70ea7-653">Хранилище</span><span class="sxs-lookup"><span data-stu-id="70ea7-653">Storage</span></span>

* <span data-ttu-id="70ea7-654">Добавлено средство заполнения для аргумента `--account-name`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-654">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="70ea7-655">Устранена проблема, связанная с командой `storage entity query`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-655">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="70ea7-656">ВМ</span><span class="sxs-lookup"><span data-stu-id="70ea7-656">VM</span></span>

* <span data-ttu-id="70ea7-657">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--write-accelerator` из команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-657">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="70ea7-658">Такие же возможности предоставляет команда `vm update` или `vm disk attach`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-658">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="70ea7-659">Устранена проблема с сопоставлением образов расширения в команде `[vm|vmss] extension`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-659">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="70ea7-660">Добавлен параметр `--boot-diagnostics-storage` для команды `vm create` для записи журнала загрузки.</span><span class="sxs-lookup"><span data-stu-id="70ea7-660">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="70ea7-661">Добавлен параметр `--license-type` для команды `[vm|vmss] update`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-661">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="70ea7-662">7 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70ea7-662">May 7, 2018</span></span>

<span data-ttu-id="70ea7-663">Версия 2.0.32</span><span class="sxs-lookup"><span data-stu-id="70ea7-663">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="70ea7-664">Core</span><span class="sxs-lookup"><span data-stu-id="70ea7-664">Core</span></span>

* <span data-ttu-id="70ea7-665">Исправлено необработанное исключение при получении секретов из основной учетной записи службы с сертификатом.</span><span class="sxs-lookup"><span data-stu-id="70ea7-665">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="70ea7-666">Добавлена ограниченная поддержка для позиционных аргументов.</span><span class="sxs-lookup"><span data-stu-id="70ea7-666">Added limited support for positional arguments</span></span>
* <span data-ttu-id="70ea7-667">Исправлена проблема, когда `--query` нельзя использовать с `--ids`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-667">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="70ea7-668">#5591</span><span class="sxs-lookup"><span data-stu-id="70ea7-668">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="70ea7-669">Улучшены сценарии конвейерной передачи от команд при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-669">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="70ea7-670">Добавлена поддержка `-o tsv` с указанием запроса или `-o json` без указания запроса.</span><span class="sxs-lookup"><span data-stu-id="70ea7-670">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="70ea7-671">Добавлена команда предложения в случае ошибки, если пользователи вводят команды с опечаткой.</span><span class="sxs-lookup"><span data-stu-id="70ea7-671">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="70ea7-672">Исправлена ошибка, когда пользователи вводят `az ''`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-672">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="70ea7-673">Добавлена поддержка настраиваемого ресурса для командных модулей и расширений.</span><span class="sxs-lookup"><span data-stu-id="70ea7-673">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="70ea7-674">ACR</span><span class="sxs-lookup"><span data-stu-id="70ea7-674">ACR</span></span>

* <span data-ttu-id="70ea7-675">Добавлены команды сборки ACR.</span><span class="sxs-lookup"><span data-stu-id="70ea7-675">Added ACR Build commands</span></span>
* <span data-ttu-id="70ea7-676">Исправлена ошибка о не найденных сообщениях об ошибках.</span><span class="sxs-lookup"><span data-stu-id="70ea7-676">Improved resource not found error messages</span></span>
* <span data-ttu-id="70ea7-677">Оптимизированы производительность создания ресурсов и обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="70ea7-677">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="70ea7-678">Улучшены возможности входа ACR в нестандартные консоли и WSL.</span><span class="sxs-lookup"><span data-stu-id="70ea7-678">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="70ea7-679">Улучшены сообщения об ошибках команд репозитория.</span><span class="sxs-lookup"><span data-stu-id="70ea7-679">Improved repository commands error messages</span></span>
* <span data-ttu-id="70ea7-680">Обновлены столбцы таблиц и порядок их расположения.</span><span class="sxs-lookup"><span data-stu-id="70ea7-680">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="70ea7-681">ACS</span><span class="sxs-lookup"><span data-stu-id="70ea7-681">ACS</span></span>

* <span data-ttu-id="70ea7-682">Добавлено предупреждение о том, что `az aks` — это предварительная версия службы.</span><span class="sxs-lookup"><span data-stu-id="70ea7-682">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="70ea7-683">Исправлена проблема с разрешением в `aks install-connector`, когда `--aci-resource-group` не указывается.</span><span class="sxs-lookup"><span data-stu-id="70ea7-683">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="70ea7-684">AMS</span><span class="sxs-lookup"><span data-stu-id="70ea7-684">AMS</span></span>

* <span data-ttu-id="70ea7-685">Первоначальный выпуск. Управление ресурсами Служб мультимедиа Azure.</span><span class="sxs-lookup"><span data-stu-id="70ea7-685">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="70ea7-686">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="70ea7-686">Appservice</span></span>

* <span data-ttu-id="70ea7-687">Исправлена ошибка в `webapp delete`, когда `--slot` предоставляется.</span><span class="sxs-lookup"><span data-stu-id="70ea7-687">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="70ea7-688">Удалено `--runtime-version` из `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-688">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="70ea7-689">Добавлена поддержка min\_tls\_version и https2.0.</span><span class="sxs-lookup"><span data-stu-id="70ea7-689">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="70ea7-690">Добавлена поддержка нескольких контейнеров.</span><span class="sxs-lookup"><span data-stu-id="70ea7-690">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="70ea7-691">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="70ea7-691">Batch AI</span></span>

* <span data-ttu-id="70ea7-692">Изменено `batchai create cluster` с учетом приоритета виртуальной машины при настройке в файле конфигурации кластера.</span><span class="sxs-lookup"><span data-stu-id="70ea7-692">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="70ea7-693">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="70ea7-693">Cognitive Services</span></span>

* <span data-ttu-id="70ea7-694">Исправлена опечатка в примере для `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603).</span><span class="sxs-lookup"><span data-stu-id="70ea7-694">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="70ea7-695">Потребление</span><span class="sxs-lookup"><span data-stu-id="70ea7-695">Consumption</span></span>

* <span data-ttu-id="70ea7-696">Добавлены новые команды в API для управления бюджетом.</span><span class="sxs-lookup"><span data-stu-id="70ea7-696">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="70ea7-697">Контейнер</span><span class="sxs-lookup"><span data-stu-id="70ea7-697">Container</span></span>

* <span data-ttu-id="70ea7-698">Удалено требование `--registry-server` для `container create`, когда сервер реестра включен в имя образа.</span><span class="sxs-lookup"><span data-stu-id="70ea7-698">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="70ea7-699">База данных Cosmos</span><span class="sxs-lookup"><span data-stu-id="70ea7-699">Cosmos DB</span></span>

* <span data-ttu-id="70ea7-700">Добавлена поддержка VNET для Azure CLI в Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="70ea7-700">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="70ea7-701">DMS</span><span class="sxs-lookup"><span data-stu-id="70ea7-701">DMS</span></span>

* <span data-ttu-id="70ea7-702">Исходный выпуск. Добавлена поддержка сценария миграции SQL — Azure SQL.</span><span class="sxs-lookup"><span data-stu-id="70ea7-702">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="70ea7-703">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="70ea7-703">Extension</span></span>

* <span data-ttu-id="70ea7-704">Исправлена ошибка, когда метаданные остановленного расширения отображались.</span><span class="sxs-lookup"><span data-stu-id="70ea7-704">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="70ea7-705">Interactive</span><span class="sxs-lookup"><span data-stu-id="70ea7-705">Interactive</span></span>

* <span data-ttu-id="70ea7-706">Разрешена работа интерактивных средств завершения с позиционными аргументами.</span><span class="sxs-lookup"><span data-stu-id="70ea7-706">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="70ea7-707">Добавлены более понятные выходные данные, когда пользователи вводят \'.</span><span class="sxs-lookup"><span data-stu-id="70ea7-707">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="70ea7-708">Исправлены завершения для параметров без справки.</span><span class="sxs-lookup"><span data-stu-id="70ea7-708">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="70ea7-709">Исправлены описания для групп команд.</span><span class="sxs-lookup"><span data-stu-id="70ea7-709">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="70ea7-710">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="70ea7-710">Lab</span></span>

* <span data-ttu-id="70ea7-711">Исправлены регрессии из преобразования Knack.</span><span class="sxs-lookup"><span data-stu-id="70ea7-711">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="70ea7-712">Сеть</span><span class="sxs-lookup"><span data-stu-id="70ea7-712">Network</span></span>

* <span data-ttu-id="70ea7-713">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--ids` для:</span><span class="sxs-lookup"><span data-stu-id="70ea7-713">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="70ea7-714">Профиль</span><span class="sxs-lookup"><span data-stu-id="70ea7-714">Profile</span></span>

* <span data-ttu-id="70ea7-715">Исправлено определение источника `disk create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-715">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="70ea7-716">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--msi-port` и `--identity-port`, так как они больше не используются.</span><span class="sxs-lookup"><span data-stu-id="70ea7-716">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="70ea7-717">Исправлена опечатка в кратком описании `account get-access-token`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-717">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="70ea7-718">Redis</span><span class="sxs-lookup"><span data-stu-id="70ea7-718">Redis</span></span>

* <span data-ttu-id="70ea7-719">Вместо `redis patch-schedule patch-schedule show` теперь используется `redis patch-schedule show`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-719">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="70ea7-720">`redis list-all` теперь не используется.</span><span class="sxs-lookup"><span data-stu-id="70ea7-720">Deprecated `redis list-all`.</span></span> <span data-ttu-id="70ea7-721">Эта функция включена в `redis list`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-721">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="70ea7-722">Вместо `redis import-method` теперь используется `redis import`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-722">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="70ea7-723">Добавлена поддержка `--ids` для разных команд.</span><span class="sxs-lookup"><span data-stu-id="70ea7-723">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="70ea7-724">Роль</span><span class="sxs-lookup"><span data-stu-id="70ea7-724">Role</span></span>

* <span data-ttu-id="70ea7-725">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `ad sp reset-credentials` по причине устаревания.</span><span class="sxs-lookup"><span data-stu-id="70ea7-725">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="70ea7-726">Хранилище</span><span class="sxs-lookup"><span data-stu-id="70ea7-726">Storage</span></span>

* <span data-ttu-id="70ea7-727">Разрешено применение SAS-токенов назначения к источнику для копирования BLOB-объектов, если SAS источника и ключ учетной записи не указаны.</span><span class="sxs-lookup"><span data-stu-id="70ea7-727">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="70ea7-728">Добавлено отображение времени ожидания сокета для отправки и скачивания большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="70ea7-728">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="70ea7-729">Добавлена обработка имен больших двоичных объектов, которые начинаются с разделителей пути, как относительных путей.</span><span class="sxs-lookup"><span data-stu-id="70ea7-729">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="70ea7-730">Разрешено использовать `storage blob copy --source-sas` с начальным символом запроса "?".</span><span class="sxs-lookup"><span data-stu-id="70ea7-730">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="70ea7-731">Исправлено `storage entity query --marker` для принятия списка пар "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="70ea7-731">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="70ea7-732">ВМ</span><span class="sxs-lookup"><span data-stu-id="70ea7-732">VM</span></span>

* <span data-ttu-id="70ea7-733">Исправлена недопустимая логика обнаружения в URI неуправляемого BLOB-объекта.</span><span class="sxs-lookup"><span data-stu-id="70ea7-733">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="70ea7-734">Добавлена поддержка шифрования диска без предоставления пользователем субъектов-служб.</span><span class="sxs-lookup"><span data-stu-id="70ea7-734">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="70ea7-735">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Не используйте ManagedIdentityExtension виртуальной машины для включения поддержки MSI.</span><span class="sxs-lookup"><span data-stu-id="70ea7-735">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="70ea7-736">Добавлена поддержка политики вытеснения для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-736">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="70ea7-737">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--ids` из:</span><span class="sxs-lookup"><span data-stu-id="70ea7-737">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="70ea7-738">Добавлена поддержка ускорителя записи.</span><span class="sxs-lookup"><span data-stu-id="70ea7-738">Added write accelerator support</span></span>
* <span data-ttu-id="70ea7-739">Добавлена команда `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-739">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="70ea7-740">Исправлено `vm diagnostics set` для надежного определения типа ОС виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="70ea7-740">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="70ea7-741">Изменено `vm resize` для проверки того, отличается ли запрошенный размер от установленного (с обновлением только при изменении).</span><span class="sxs-lookup"><span data-stu-id="70ea7-741">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="70ea7-742">10 апреля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70ea7-742">April 10, 2018</span></span>

<span data-ttu-id="70ea7-743">Версия 2.0.31</span><span class="sxs-lookup"><span data-stu-id="70ea7-743">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="70ea7-744">ACR</span><span class="sxs-lookup"><span data-stu-id="70ea7-744">ACR</span></span>

* <span data-ttu-id="70ea7-745">Улучшена обработка ошибок при откате wincred.</span><span class="sxs-lookup"><span data-stu-id="70ea7-745">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="70ea7-746">ACS</span><span class="sxs-lookup"><span data-stu-id="70ea7-746">ACS</span></span>

* <span data-ttu-id="70ea7-747">Срок действия имен субъектов-служб, созданных службой контейнеров Azure, изменен до 5 лет.</span><span class="sxs-lookup"><span data-stu-id="70ea7-747">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="70ea7-748">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="70ea7-748">Appservice</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="70ea7-750">Исправлено неперехватываемое исключение для несуществующих планов веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="70ea7-750">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="70ea7-751">Batch AI</span><span class="sxs-lookup"><span data-stu-id="70ea7-751">BatchAI</span></span>

* <span data-ttu-id="70ea7-752">Добавлена поддержка API 2018-03-01.</span><span class="sxs-lookup"><span data-stu-id="70ea7-752">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="70ea7-753">Подключение на уровне задания.</span><span class="sxs-lookup"><span data-stu-id="70ea7-753">Job level mounting</span></span>
  - <span data-ttu-id="70ea7-754">Переменные среды со значениями секретов.</span><span class="sxs-lookup"><span data-stu-id="70ea7-754">Environment variables with secret values</span></span>
  - <span data-ttu-id="70ea7-755">Параметры счетчиков производительности</span><span class="sxs-lookup"><span data-stu-id="70ea7-755">Performance counters settings</span></span>
  - <span data-ttu-id="70ea7-756">Предоставление информации о сегменте пути конкретного задания.</span><span class="sxs-lookup"><span data-stu-id="70ea7-756">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="70ea7-757">Поддержка вложенных папок в API списка файлов.</span><span class="sxs-lookup"><span data-stu-id="70ea7-757">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="70ea7-758">Предоставление информации об использовании и ограничениях.</span><span class="sxs-lookup"><span data-stu-id="70ea7-758">Usage and limits reporting</span></span>
  - <span data-ttu-id="70ea7-759">Возможность указать тип кэширования для NFS-серверов.</span><span class="sxs-lookup"><span data-stu-id="70ea7-759">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="70ea7-760">Поддержка пользовательских образов.</span><span class="sxs-lookup"><span data-stu-id="70ea7-760">Support for custom images</span></span>
  - <span data-ttu-id="70ea7-761">Добавлена поддержка инструментария pyTorch.</span><span class="sxs-lookup"><span data-stu-id="70ea7-761">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="70ea7-762">Добавлена команда `job wait`, позволяющая дождаться завершения задания и сообщить код выхода задания.</span><span class="sxs-lookup"><span data-stu-id="70ea7-762">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="70ea7-763">Добавлена команда `usage show`, позволяющая получить актуальные сведения об использовании и ограничениях ресурсов Batch AI для различных регионов.</span><span class="sxs-lookup"><span data-stu-id="70ea7-763">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="70ea7-764">Поддержка национальных облаков.</span><span class="sxs-lookup"><span data-stu-id="70ea7-764">National clouds are supported</span></span>
* <span data-ttu-id="70ea7-765">Для заданий добавлены аргументы командной строки, которые позволяют подключать файловые системы на уровне заданий. Эти же действия можно выполнять в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="70ea7-765">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="70ea7-766">Добавлены дополнительные параметры для настройки кластеров: приоритет виртуальной машины, подсеть, исходное число узлов для кластеров с автоматическим масштабированием, выбор пользовательского образа.</span><span class="sxs-lookup"><span data-stu-id="70ea7-766">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="70ea7-767">Добавлен параметр командной строки, который позволяет указать тип кэширования для управляемой файловой системы NFS службы Batch AI.</span><span class="sxs-lookup"><span data-stu-id="70ea7-767">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="70ea7-768">Упрощена процедура выбора подключаемой файловой системы в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="70ea7-768">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="70ea7-769">Теперь учетные данные для общего файлового ресурса Azure и контейнеров BLOB-объектов Azure указывать не нужно: CLI получит отсутствующие учетные данные с помощью ключа учетной записи хранения, указанного в параметрах командной строки, или переменной среды либо запросит ключ из службы хранилища Azure (если учетная запись хранения относится к текущей подписке).</span><span class="sxs-lookup"><span data-stu-id="70ea7-769">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="70ea7-770">Команда задания потоковой передачи файлов теперь автоматически завершается при завершении задания (успешное выполнение, сбой, прерывание или удаление).</span><span class="sxs-lookup"><span data-stu-id="70ea7-770">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="70ea7-771">Улучшены выходные данные `table` для операций `show`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-771">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="70ea7-772">Добавлен параметр `--use-auto-storage` для создания кластера.</span><span class="sxs-lookup"><span data-stu-id="70ea7-772">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="70ea7-773">Этот параметр упрощает управление учетными записями хранения, а также подключение общего файлового ресурса Azure и контейнеров BLOB-объектов Azure к кластеру.</span><span class="sxs-lookup"><span data-stu-id="70ea7-773">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="70ea7-774">Добавлен параметр `--generate-ssh-keys` для команд `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-774">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="70ea7-775">Добавлена возможность запустить задачу настройки узла через командную строку.</span><span class="sxs-lookup"><span data-stu-id="70ea7-775">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="70ea7-776">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `job stream-file` и `job list-files` перемещены в группу `job file`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-776">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="70ea7-777">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В команде `file-server create` параметр `--admin-user-name` переименован в `--user-name` для согласованности с командой `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-777">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="70ea7-778">Выставление счетов</span><span class="sxs-lookup"><span data-stu-id="70ea7-778">Billing</span></span>

* <span data-ttu-id="70ea7-779">Добавлены команды для учетной записи регистрации.</span><span class="sxs-lookup"><span data-stu-id="70ea7-779">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="70ea7-780">Потребление</span><span class="sxs-lookup"><span data-stu-id="70ea7-780">Consumption</span></span>

* <span data-ttu-id="70ea7-781">Добавлены команды `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-781">Added `marketplace` commands</span></span>
* <span data-ttu-id="70ea7-782">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations summaries` переименована в `reservation summary`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-782">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="70ea7-783">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations details` переименована в `reservation detail`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-783">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="70ea7-784">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation` удалены короткие параметры `--reservation-order-id` и `--reservation-id`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-784">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="70ea7-785">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation summary` удалены короткие параметры `--grain`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-785">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="70ea7-786">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `pricesheet` удалены короткие параметры `--include-meter-details`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-786">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="70ea7-787">Контейнер</span><span class="sxs-lookup"><span data-stu-id="70ea7-787">Container</span></span>

* <span data-ttu-id="70ea7-788">Добавлены параметры подключения тома репозитория git: `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` и `--gitrepo-mount-path`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-788">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="70ea7-789">Исправлена ошибка [#5926](https://github.com/Azure/azure-cli/issues/5926): команда `az container exec` возвращает ошибку, когда указан параметр --container-name.</span><span class="sxs-lookup"><span data-stu-id="70ea7-789">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="70ea7-790">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="70ea7-790">Extension</span></span>

* <span data-ttu-id="70ea7-791">Сообщение о проверке распространения перенесено на уровень отладки.</span><span class="sxs-lookup"><span data-stu-id="70ea7-791">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="70ea7-792">Interactive</span><span class="sxs-lookup"><span data-stu-id="70ea7-792">Interactive</span></span>

* <span data-ttu-id="70ea7-793">Если команда не распознана, выполнение прерывается.</span><span class="sxs-lookup"><span data-stu-id="70ea7-793">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="70ea7-794">Добавлены перехватчики событий, которые используются до и после создания поддерева команд.</span><span class="sxs-lookup"><span data-stu-id="70ea7-794">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="70ea7-795">Добавлены сведения о выполнении для параметров `--ids`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-795">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="70ea7-796">Сеть</span><span class="sxs-lookup"><span data-stu-id="70ea7-796">Network</span></span>

* <span data-ttu-id="70ea7-797">Исправлена ошибка [#5936](https://github.com/Azure/azure-cli/issues/5936): не задаются теги `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-797">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="70ea7-798">Добавлен аргумент `--auth-certs`, который позволяет подключать сертификаты аутентификации для `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-798">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> <span data-ttu-id="70ea7-799">[#4910](https://github.com/Azure/azure-cli/issues/4910).</span><span class="sxs-lookup"><span data-stu-id="70ea7-799">[#4910](https://github.com/Azure/azure-cli/issues/4910)</span></span>
* <span data-ttu-id="70ea7-800">Добавлены команды `ddos-protection` для создания планов защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="70ea7-800">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="70ea7-801">В команду `vnet [create|update]` добавлена поддержка `--ddos-protection-plan` для связи виртуальной сети с планом защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="70ea7-801">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="70ea7-802">Исправлена ошибка с флагом `--disable-bgp-route-propagation` в команде `network route-table [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-802">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="70ea7-803">Удалены фиктивные аргументы `--public-ip-address-type` и `--subnet-type` для команды `network lb [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-803">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="70ea7-804">В `network dns zone [import|export]` и `network dns record-set txt add-record` добавлена поддержка записей типа TXT с escape-последовательностями RFC 1035.</span><span class="sxs-lookup"><span data-stu-id="70ea7-804">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="70ea7-805">Профиль</span><span class="sxs-lookup"><span data-stu-id="70ea7-805">Profile</span></span>

* <span data-ttu-id="70ea7-806">Добавлена поддержка классических учетных записей Azure для команды `account list`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-806">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="70ea7-807">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены аргументы `--msi`  &  `--msi-port`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-807">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="70ea7-808">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="70ea7-808">RDBMS</span></span>

* <span data-ttu-id="70ea7-809">Добавлена команда `georestore`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-809">Added `georestore` command</span></span>
* <span data-ttu-id="70ea7-810">Из команды `create` исключено ограничение на размер хранилища.</span><span class="sxs-lookup"><span data-stu-id="70ea7-810">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="70ea7-811">Ресурс</span><span class="sxs-lookup"><span data-stu-id="70ea7-811">Resource</span></span>

* <span data-ttu-id="70ea7-812">Добавлена поддержка параметра `--metadata` в команде `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-812">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="70ea7-813">Добавлена поддержка `--metadata`, `--set`, `--add` и `--remove` для команды `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-813">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="70ea7-814">SQL</span><span class="sxs-lookup"><span data-stu-id="70ea7-814">SQL</span></span>

* <span data-ttu-id="70ea7-815">Добавлены команды `sql elastic-pool op list` и `sql elastic-pool op cancel`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-815">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="70ea7-816">Хранилище</span><span class="sxs-lookup"><span data-stu-id="70ea7-816">Storage</span></span>

* <span data-ttu-id="70ea7-817">Улучшены сообщения об ошибках для строк подключения, имеющих неправильный формат.</span><span class="sxs-lookup"><span data-stu-id="70ea7-817">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="70ea7-818">ВМ</span><span class="sxs-lookup"><span data-stu-id="70ea7-818">VM</span></span>

* <span data-ttu-id="70ea7-819">В команде `vmss create` добавлена возможность настроить для платформы количество доменов сбоя.</span><span class="sxs-lookup"><span data-stu-id="70ea7-819">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="70ea7-820">Команда `vmss create` теперь по умолчанию использует стандартную балансировку нагрузки для зональных и больших масштабируемых наборов, а также масштабируемых наборов, в которых отключена одна группа размещения.</span><span class="sxs-lookup"><span data-stu-id="70ea7-820">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="70ea7-822">Добавлена поддержка SKU общедоступного IP-адреса для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-822">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="70ea7-823">В команду `vm secret format` добавлены аргументы `--keyvault` и `--resource-group` для тех случаев, когда команда не может разрешить идентификатор хранилища.</span><span class="sxs-lookup"><span data-stu-id="70ea7-823">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> <span data-ttu-id="70ea7-824">[#5718](https://github.com/Azure/azure-cli/issues/5718).</span><span class="sxs-lookup"><span data-stu-id="70ea7-824">[#5718](https://github.com/Azure/azure-cli/issues/5718)</span></span>
* <span data-ttu-id="70ea7-825">Улучшены сообщения об ошибках для команды `[vm|vmss create]`, когда расположение группы ресурсов не поддерживает зоны.</span><span class="sxs-lookup"><span data-stu-id="70ea7-825">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="70ea7-826">27 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70ea7-826">March 27, 2018</span></span>

<span data-ttu-id="70ea7-827">Версия 2.0.30</span><span class="sxs-lookup"><span data-stu-id="70ea7-827">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="70ea7-828">Core</span><span class="sxs-lookup"><span data-stu-id="70ea7-828">Core</span></span>

* <span data-ttu-id="70ea7-829">Отображение сообщения для расширений, которые отмечены в справке как предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="70ea7-829">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="70ea7-830">ACS</span><span class="sxs-lookup"><span data-stu-id="70ea7-830">ACS</span></span>

* <span data-ttu-id="70ea7-831">Устранена ошибка с проверкой SSL-сертификата для `aks install-cli` в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="70ea7-831">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="70ea7-832">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="70ea7-832">Appservice</span></span>

* <span data-ttu-id="70ea7-833">Добавлена поддержка только протокола HTTPS для `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-833">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="70ea7-834">Добавлена поддержка слотов для `az webapp identity [assign|show]` и `az functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-834">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="70ea7-835">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="70ea7-835">Backup</span></span>

* <span data-ttu-id="70ea7-836">Добавлена новая команда `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-836">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="70ea7-837">Эта команда используется для проверки резервного копирования виртуальной машины в любое хранилище в подписке.</span><span class="sxs-lookup"><span data-stu-id="70ea7-837">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="70ea7-838">Включены идентификаторы объектов Azure для параметров `--resource-group` и `--vault-name` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="70ea7-838">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="70ea7-839">Изменены параметры `--name` для поддержки формата вывода команд `backup ... show`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-839">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="70ea7-840">Контейнер</span><span class="sxs-lookup"><span data-stu-id="70ea7-840">Container</span></span>

* <span data-ttu-id="70ea7-841">Добавлена команда `container exec`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-841">Added `container exec` command.</span></span> <span data-ttu-id="70ea7-842">Выполнение команды в контейнере для выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="70ea7-842">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="70ea7-843">Разрешение выходной таблице создавать и обновлять группу контейнеров.</span><span class="sxs-lookup"><span data-stu-id="70ea7-843">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="70ea7-844">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="70ea7-844">Extension</span></span>

* <span data-ttu-id="70ea7-845">Добавлено сообщение для `extension add`, если расширение доступно в режиме предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="70ea7-845">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="70ea7-846">Изменен параметр `extension list-available` для отображения всех данных расширения с использованием `--show-details`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-846">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="70ea7-847">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменена команда `extension list-available` для отображения упрощенных данных расширения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="70ea7-847">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="70ea7-848">Interactive</span><span class="sxs-lookup"><span data-stu-id="70ea7-848">Interactive</span></span>

* <span data-ttu-id="70ea7-849">Изменены операции завершения, активируемые сразу после завершения загрузки таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="70ea7-849">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="70ea7-850">Исправлена ошибка с использованием параметра `--style`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-850">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="70ea7-851">Отсутствующий интерактивный лексический анализатор создается после дампа таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="70ea7-851">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="70ea7-852">Улучшена поддержка средства заполнения.</span><span class="sxs-lookup"><span data-stu-id="70ea7-852">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="70ea7-853">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="70ea7-853">Lab</span></span>

* <span data-ttu-id="70ea7-854">Исправлены ошибки с командой `create environment`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-854">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="70ea7-855">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="70ea7-855">Monitor</span></span>

* <span data-ttu-id="70ea7-856">Добавлена поддержка `--top`, `--orderby` и `--namespace` для `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="70ea7-856">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="70ea7-857">Исправлена ошибка [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` принимает разделенный пробелами список метрик для извлечения.</span><span class="sxs-lookup"><span data-stu-id="70ea7-857">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="70ea7-858">Добавлена поддержка `--namespace` для `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="70ea7-858">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="70ea7-859">Сеть</span><span class="sxs-lookup"><span data-stu-id="70ea7-859">Network</span></span>

* <span data-ttu-id="70ea7-860">Добавлена поддержка Частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="70ea7-860">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="70ea7-861">Профиль</span><span class="sxs-lookup"><span data-stu-id="70ea7-861">Profile</span></span>

* <span data-ttu-id="70ea7-862">Добавлено предупреждение для `--identity-port` и `--msi-port` в `login`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-862">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="70ea7-863">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="70ea7-863">RDBMS</span></span>

* <span data-ttu-id="70ea7-864">Добавлена общедоступная версия 2017-12-01 бизнес-модели API.</span><span class="sxs-lookup"><span data-stu-id="70ea7-864">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="70ea7-865">Ресурс</span><span class="sxs-lookup"><span data-stu-id="70ea7-865">Resource</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="70ea7-867">Роль</span><span class="sxs-lookup"><span data-stu-id="70ea7-867">Role</span></span>

* <span data-ttu-id="70ea7-868">Добавлена поддержка конфигурации требуемого уровня доступа и собственных клиентов для `az ad app create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-868">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="70ea7-869">Изменены команды `rbac`, чтобы возвращать не более 1000 идентификаторов в разрешении объекта.</span><span class="sxs-lookup"><span data-stu-id="70ea7-869">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="70ea7-870">Добавлены команды `ad sp credential [reset|list|delete]` для управления учетными данными.</span><span class="sxs-lookup"><span data-stu-id="70ea7-870">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="70ea7-871">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр properties из выходных данных `az role assignment [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-871">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="70ea7-872">Добавлена поддержка разрешений `dataActions` и `notDataActions` для `role definition`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-872">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="70ea7-873">Хранилище</span><span class="sxs-lookup"><span data-stu-id="70ea7-873">Storage</span></span>

* <span data-ttu-id="70ea7-874">Исправлена проблема с отправкой файла размером от 195 до 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="70ea7-874">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="70ea7-875">Исправлена ошибка [#4049](https://github.com/Azure/azure-cli/issues/4049): проблемы, когда при отправке добавочного большого двоичного объекта игнорируются параметры условия.</span><span class="sxs-lookup"><span data-stu-id="70ea7-875">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="70ea7-876">ВМ</span><span class="sxs-lookup"><span data-stu-id="70ea7-876">VM</span></span>

* <span data-ttu-id="70ea7-877">Добавлено предупреждение `vmss create` для предстоящих критически важных изменений для наборов из 100 и более экземпляров.</span><span class="sxs-lookup"><span data-stu-id="70ea7-877">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="70ea7-878">Добавлена поддержка устойчивости зон для `vm [snapshot|image]`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-878">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="70ea7-879">Изменено представление экземпляра диска для улучшения отчета о состоянии шифрования.</span><span class="sxs-lookup"><span data-stu-id="70ea7-879">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="70ea7-880">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] `vm extension delete` Изменена команда, которая больше не возвращает выходные данные.</span><span class="sxs-lookup"><span data-stu-id="70ea7-880">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="70ea7-881">13 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70ea7-881">March 13, 2018</span></span>

<span data-ttu-id="70ea7-882">Версия 2.0.29</span><span class="sxs-lookup"><span data-stu-id="70ea7-882">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="70ea7-883">ACR</span><span class="sxs-lookup"><span data-stu-id="70ea7-883">ACR</span></span>

* <span data-ttu-id="70ea7-884">Добавлена поддержка параметра `--image` для `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-884">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="70ea7-885">Параметры `--manifest` и `--tag` команды `repository delete` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="70ea7-885">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="70ea7-886">Добавлена команда `repository untag` для удаления тега без удаления данных.</span><span class="sxs-lookup"><span data-stu-id="70ea7-886">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="70ea7-887">ACS</span><span class="sxs-lookup"><span data-stu-id="70ea7-887">ACS</span></span>

* <span data-ttu-id="70ea7-888">Добавлена команда `aks upgrade-connector` для обновления существующего соединителя.</span><span class="sxs-lookup"><span data-stu-id="70ea7-888">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="70ea7-889">Изменены файлы конфигурации `kubectl`. Теперь используется более разборчивый стиль YAML с разбивкой на блоки.</span><span class="sxs-lookup"><span data-stu-id="70ea7-889">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="70ea7-890">Помощник</span><span class="sxs-lookup"><span data-stu-id="70ea7-890">Advisor</span></span>

* <span data-ttu-id="70ea7-891">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration get` переименована в `advisor configuration list`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-891">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="70ea7-892">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration set` переименована в `advisor configuration update`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-892">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="70ea7-893">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `advisor recommendation generate`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-893">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="70ea7-894">Добавлен параметр `--refresh` для команды `advisor recommendation list`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-894">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="70ea7-895">Добавлена команда `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-895">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="70ea7-896">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="70ea7-896">Appservice</span></span>

* <span data-ttu-id="70ea7-897">Команда `[webapp|functionapp] assign-identity` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="70ea7-897">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="70ea7-898">Добавлены команды управляемого удостоверения `webapp identity [assign|show]` и `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-898">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="70ea7-899">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="70ea7-899">Eventhubs</span></span>

* <span data-ttu-id="70ea7-900">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="70ea7-900">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="70ea7-901">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="70ea7-901">Extension</span></span>

* <span data-ttu-id="70ea7-902">Добавлена проверка, позволяющая предупредить пользователя, если используемый дистрибутив отличается от хранящегося в исходном файле пакета, так как это может привести к возникновению ошибок.</span><span class="sxs-lookup"><span data-stu-id="70ea7-902">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="70ea7-903">Interactive</span><span class="sxs-lookup"><span data-stu-id="70ea7-903">Interactive</span></span>

* <span data-ttu-id="70ea7-904">Исправлена ошибка [#5625](https://github.com/Azure/azure-cli/issues/5625): теперь записи журнала сохраняются в разных сеансах.</span><span class="sxs-lookup"><span data-stu-id="70ea7-904">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="70ea7-905">Исправлена ошибка [#3016](https://github.com/Azure/azure-cli/issues/3016): при использовании области не создавались записи журнала.</span><span class="sxs-lookup"><span data-stu-id="70ea7-905">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="70ea7-906">Исправлена ошибка [#5688](https://github.com/Azure/azure-cli/issues/5688): если при загрузке таблицы команд возникало исключение, опережающий ввод не выполнялся.</span><span class="sxs-lookup"><span data-stu-id="70ea7-906">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="70ea7-907">Исправлен индикатор хода выполнения для длительных операций.</span><span class="sxs-lookup"><span data-stu-id="70ea7-907">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="70ea7-908">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="70ea7-908">Monitor</span></span>

* <span data-ttu-id="70ea7-909">Команды `monitor autoscale-settings` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="70ea7-909">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="70ea7-910">Добавлены команды `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-910">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="70ea7-911">Добавлены команды `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-911">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="70ea7-912">Добавлены команды `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-912">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="70ea7-913">Сеть</span><span class="sxs-lookup"><span data-stu-id="70ea7-913">Network</span></span>

* <span data-ttu-id="70ea7-914">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--tags` из `route-filter rule create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-914">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="70ea7-915">Удалены некоторые ошибочные значения по умолчанию для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="70ea7-915">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="70ea7-916">Добавлены команды `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-916">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="70ea7-917">Добавлены параметры `--vnet` и `--subnet` для `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-917">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="70ea7-918">Профиль</span><span class="sxs-lookup"><span data-stu-id="70ea7-918">Profile</span></span>

* <span data-ttu-id="70ea7-919">Параметр `--msi` для `az login` отмечен как нерекомендуемый.</span><span class="sxs-lookup"><span data-stu-id="70ea7-919">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="70ea7-920">Добавлен параметр `--identity` для `az login`. Он заменяет `--msi`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-920">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="70ea7-921">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="70ea7-921">RDBMS</span></span>

* <span data-ttu-id="70ea7-922">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Внесены изменения для использования предварительной версии API 2017-12-01.</span><span class="sxs-lookup"><span data-stu-id="70ea7-922">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="70ea7-923">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="70ea7-923">Service Bus</span></span>

* <span data-ttu-id="70ea7-924">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="70ea7-924">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="70ea7-925">Хранилище</span><span class="sxs-lookup"><span data-stu-id="70ea7-925">Storage</span></span>

* <span data-ttu-id="70ea7-926">Исправлена ошибка [#4971](https://github.com/Azure/azure-cli/issues/4971): теперь `storage blob copy` поддерживает другие облака Azure.</span><span class="sxs-lookup"><span data-stu-id="70ea7-926">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="70ea7-927">Исправлена ошибка [#5286](https://github.com/Azure/azure-cli/issues/5286): при пакетном выполнении команд `storage blob [delete-batch|download-batch|upload-batch]` больше не отображается сообщение об ошибке в предусловии.</span><span class="sxs-lookup"><span data-stu-id="70ea7-927">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="70ea7-928">ВМ</span><span class="sxs-lookup"><span data-stu-id="70ea7-928">VM</span></span>

* <span data-ttu-id="70ea7-929">В `[vm|vmss] create` добавлена поддержка присоединения неуправляемых дисков данных и настройки кэширования.</span><span class="sxs-lookup"><span data-stu-id="70ea7-929">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="70ea7-930">`[vm|vmss] assign-identity` и `[vm|vmss] remove-identity` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="70ea7-930">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="70ea7-931">Вместо нерекомендуемых команд добавлены команды `vm identity [assign|remove|show]` и `vmss identity [assign|remove|show]`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-931">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="70ea7-932">Для приоритета `vmss create` по умолчанию установлено значение None.</span><span class="sxs-lookup"><span data-stu-id="70ea7-932">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="70ea7-933">27 февраля 2018 г</span><span class="sxs-lookup"><span data-stu-id="70ea7-933">February 27, 2018</span></span>

<span data-ttu-id="70ea7-934">Версия 2.0.28</span><span class="sxs-lookup"><span data-stu-id="70ea7-934">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="70ea7-935">Core</span><span class="sxs-lookup"><span data-stu-id="70ea7-935">Core</span></span>

* <span data-ttu-id="70ea7-936">Исправлена ошибка с установкой Homebrew [#5184](https://github.com/Azure/azure-cli/issues/5184).</span><span class="sxs-lookup"><span data-stu-id="70ea7-936">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="70ea7-937">Добавлена поддержка телеметрии расширения с применением пользовательских ключей.</span><span class="sxs-lookup"><span data-stu-id="70ea7-937">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="70ea7-938">Добавлена функция ведения журнала HTTP в `--debug`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-938">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="70ea7-939">ACS</span><span class="sxs-lookup"><span data-stu-id="70ea7-939">ACS</span></span>

* <span data-ttu-id="70ea7-940">Изменено для использования диаграмм Helm `virtual-kubelet-for-aks` для `aks install-connector` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="70ea7-940">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="70ea7-941">Исправлена ошибка с недостаточными разрешениями субъектов-служб на создание групп контейнеров ACI.</span><span class="sxs-lookup"><span data-stu-id="70ea7-941">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="70ea7-942">Добавлены параметры `--aci-container-group`, `--location` и `--image-tag` для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-942">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="70ea7-943">Удалено уведомление об устаревании из `aks get-versions`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-943">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="70ea7-944">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="70ea7-944">Appservice</span></span>

* <span data-ttu-id="70ea7-945">Обновления для новой версии пакета SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="70ea7-945">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="70ea7-946">Исправлена ошибка [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` указывалось как недопустимый номер SKU.</span><span class="sxs-lookup"><span data-stu-id="70ea7-946">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="70ea7-947">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="70ea7-947">Cognitive Services</span></span>

* <span data-ttu-id="70ea7-948">Обновлено уведомление при создании новой учетной записи Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="70ea7-948">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="70ea7-949">Потребление</span><span class="sxs-lookup"><span data-stu-id="70ea7-949">Consumption</span></span>

* <span data-ttu-id="70ea7-950">Добавлены новые команды для резервирования API прейскуранта.</span><span class="sxs-lookup"><span data-stu-id="70ea7-950">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="70ea7-951">Обновлены существующие форматы сведений об использовании и резервировании.</span><span class="sxs-lookup"><span data-stu-id="70ea7-951">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="70ea7-952">Контейнер</span><span class="sxs-lookup"><span data-stu-id="70ea7-952">Container</span></span>

* <span data-ttu-id="70ea7-953">Добавлены аргументы `--secrets` и `--secrets-mount-path` в командах `container create` для использования секретов в ACI.</span><span class="sxs-lookup"><span data-stu-id="70ea7-953">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="70ea7-954">Сеть</span><span class="sxs-lookup"><span data-stu-id="70ea7-954">Network</span></span>

* <span data-ttu-id="70ea7-955">Исправлена ошибка [#5559](https://github.com/Azure/azure-cli/issues/5559): отсутствующий клиент в `network vnet-gateway vpn-client generate`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-955">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="70ea7-956">Ресурс</span><span class="sxs-lookup"><span data-stu-id="70ea7-956">Resource</span></span>

* <span data-ttu-id="70ea7-957">Изменено `group deployment export` для отображения частичного шаблона и ошибок при сбое.</span><span class="sxs-lookup"><span data-stu-id="70ea7-957">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="70ea7-958">Роль</span><span class="sxs-lookup"><span data-stu-id="70ea7-958">Role</span></span>

* <span data-ttu-id="70ea7-959">Добавлено `role assignment list-changelogs` для включения аудита ролей субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="70ea7-959">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="70ea7-960">SQL</span><span class="sxs-lookup"><span data-stu-id="70ea7-960">SQL</span></span>

* <span data-ttu-id="70ea7-961">Добавлена поддержка избыточности зон для создания и обновления баз данных и эластичных пулов.</span><span class="sxs-lookup"><span data-stu-id="70ea7-961">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="70ea7-962">Хранилище</span><span class="sxs-lookup"><span data-stu-id="70ea7-962">Storage</span></span>

* <span data-ttu-id="70ea7-963">Включено определение пути назначения и префикса для `storage blob [upload-batch|download-batch]`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-963">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="70ea7-964">ВМ</span><span class="sxs-lookup"><span data-stu-id="70ea7-964">VM</span></span>

* <span data-ttu-id="70ea7-965">Добавлена поддержка присоединения и отсоединения дисков на одном экземпляре VMSS.</span><span class="sxs-lookup"><span data-stu-id="70ea7-965">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="70ea7-966">13 февраля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70ea7-966">February 13, 2018</span></span>

<span data-ttu-id="70ea7-967">Версия 2.0.27</span><span class="sxs-lookup"><span data-stu-id="70ea7-967">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="70ea7-968">Core</span><span class="sxs-lookup"><span data-stu-id="70ea7-968">Core</span></span>

* <span data-ttu-id="70ea7-969">Изменен способ аутентификации при входе с помощью MSI: применяется ключ при использовании идентификатора подписки и имени.</span><span class="sxs-lookup"><span data-stu-id="70ea7-969">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="70ea7-970">ACS</span><span class="sxs-lookup"><span data-stu-id="70ea7-970">ACS</span></span>

* <span data-ttu-id="70ea7-971">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименовано `aks get-versions` на `aks get-upgrades` для точности.</span><span class="sxs-lookup"><span data-stu-id="70ea7-971">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="70ea7-972">Изменено `aks get-versions` для отображения версий Kubernetes, доступных для `aks create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-972">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="70ea7-973">Изменены значения по умолчанию `aks create`, чтобы разрешить серверу выбирать версию Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="70ea7-973">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="70ea7-974">Обновлены справочные сообщения, связанные с субъектом-службой и создаваемые AKS.</span><span class="sxs-lookup"><span data-stu-id="70ea7-974">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="70ea7-975">Изменены стандартные размеры узла для `aks create` с уровня Standard\_D1\_v2 на уровень Standard\_DS1\_v2.</span><span class="sxs-lookup"><span data-stu-id="70ea7-975">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="70ea7-976">Улучшена надежность при поиске панели мониторинга для группы pod для `az aks browse`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-976">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="70ea7-977">Исправлена команда `aks get-credentials` для обработки ошибок Юникода при загрузке файлов конфигурации Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="70ea7-977">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="70ea7-978">Добавлено сообщение в `az aks install-cli`, чтобы помочь получить `kubectl` в `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-978">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="70ea7-979">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="70ea7-979">Appservice</span></span>

* <span data-ttu-id="70ea7-980">Исправлена проблема со сбоем `webapp [backup|restore]` из-за пустой ссылки.</span><span class="sxs-lookup"><span data-stu-id="70ea7-980">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="70ea7-981">Добавлена поддержка стандартных планов службы приложений с помощью `az configure --defaults appserviceplan=my-asp`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-981">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="70ea7-982">CDN</span><span class="sxs-lookup"><span data-stu-id="70ea7-982">CDN</span></span>

* <span data-ttu-id="70ea7-983">Добавлены команды `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-983">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="70ea7-984">Контейнер</span><span class="sxs-lookup"><span data-stu-id="70ea7-984">Container</span></span>

* <span data-ttu-id="70ea7-985">Добавлен параметр `--follow` для `az container logs` для журналов потоковой передачи.</span><span class="sxs-lookup"><span data-stu-id="70ea7-985">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="70ea7-986">Добавлена команда `container attach`, которая добавляет локальный стандартный поток вывода и поток вывода сообщений об ошибках к контейнеру в группе контейнеров.</span><span class="sxs-lookup"><span data-stu-id="70ea7-986">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="70ea7-987">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="70ea7-987">CosmosDB</span></span>

* <span data-ttu-id="70ea7-988">Добавлена поддержка настройки параметров.</span><span class="sxs-lookup"><span data-stu-id="70ea7-988">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="70ea7-989">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="70ea7-989">Extension</span></span>

* <span data-ttu-id="70ea7-990">Добавлена поддержка параметра `--pip-proxy` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-990">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="70ea7-991">Добавлена поддержка аргумента `--pip-extra-index-urls` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-991">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="70ea7-992">Отзыв</span><span class="sxs-lookup"><span data-stu-id="70ea7-992">Feedback</span></span>

* <span data-ttu-id="70ea7-993">Добавлены сведения о расширении к данным телеметрии.</span><span class="sxs-lookup"><span data-stu-id="70ea7-993">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="70ea7-994">Interactive</span><span class="sxs-lookup"><span data-stu-id="70ea7-994">Interactive</span></span>

* <span data-ttu-id="70ea7-995">Исправлена проблема, когда пользователю предлагалось войти в интерактивном режиме в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="70ea7-995">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="70ea7-996">Исправлена регрессия с отсутствующей функцией заполнения параметров.</span><span class="sxs-lookup"><span data-stu-id="70ea7-996">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="70ea7-997">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="70ea7-997">IoT</span></span>

* <span data-ttu-id="70ea7-998">Исправлена проблема, когда `iot dps access policy [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="70ea7-998">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="70ea7-999">Исправлена проблема, когда `iot dps linked-hub [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="70ea7-999">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="70ea7-1000">Добавлена поддержка параметра `--no-wait` для `iot dps access policy [create|update]` и `iot dps linked-hub [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1000">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="70ea7-1001">Изменена команда `iot hub create` для указания числа секций.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1001">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="70ea7-1002">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="70ea7-1002">Monitor</span></span>

* <span data-ttu-id="70ea7-1003">Исправлена команда `az monitor log-profiles create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1003">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="70ea7-1004">Сеть</span><span class="sxs-lookup"><span data-stu-id="70ea7-1004">Network</span></span>

* <span data-ttu-id="70ea7-1005">Исправлен параметр `--tags` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="70ea7-1005">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="70ea7-1006">Профиль</span><span class="sxs-lookup"><span data-stu-id="70ea7-1006">Profile</span></span>

* <span data-ttu-id="70ea7-1007">Включена команда `az login` для использования в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1007">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="70ea7-1008">Ресурс</span><span class="sxs-lookup"><span data-stu-id="70ea7-1008">Resource</span></span>

* <span data-ttu-id="70ea7-1009">Снова добавлена команда `feature show`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1009">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="70ea7-1010">Роль</span><span class="sxs-lookup"><span data-stu-id="70ea7-1010">Role</span></span>

* <span data-ttu-id="70ea7-1011">Добавлен аргумент `--available-to-other-tenants` для команды `ad app update`</span><span class="sxs-lookup"><span data-stu-id="70ea7-1011">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="70ea7-1012">SQL</span><span class="sxs-lookup"><span data-stu-id="70ea7-1012">SQL</span></span>

* <span data-ttu-id="70ea7-1013">Добавлены команды `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1013">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="70ea7-1014">Добавлена команда `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1014">Added `sql db rename`</span></span>
* <span data-ttu-id="70ea7-1015">Добавлена поддержка аргумента `--ids` для команд SQL.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1015">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="70ea7-1016">Хранилище</span><span class="sxs-lookup"><span data-stu-id="70ea7-1016">Storage</span></span>

* <span data-ttu-id="70ea7-1017">Добавлены команды `storage blob service-properties delete-policy` и `storage blob undelete` для включения обратимого удаления.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1017">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="70ea7-1018">ВМ</span><span class="sxs-lookup"><span data-stu-id="70ea7-1018">VM</span></span>

* <span data-ttu-id="70ea7-1019">Исправлена ошибка, когда шифрование виртуальной машины инициализировалось не полностью.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1019">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="70ea7-1020">Добавлены выходные данные идентификатора субъекта для включения MSI.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1020">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="70ea7-1021">Фиксированное значение `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="70ea7-1021">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="70ea7-1022">31 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1022">January 31, 2018</span></span>

<span data-ttu-id="70ea7-1023">Версия 2.0.26</span><span class="sxs-lookup"><span data-stu-id="70ea7-1023">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="70ea7-1024">Core</span><span class="sxs-lookup"><span data-stu-id="70ea7-1024">Core</span></span>

* <span data-ttu-id="70ea7-1025">Добавлена поддержка получения необработанного маркера в контексте MSI.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1025">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="70ea7-1026">Удалена строка индикатора опроса после завершения LRO при выполнении cmd.exe в Windows.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1026">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="70ea7-1027">Добавлено предупреждение, которое появляется при использовании настроенных по умолчанию параметров, измененных на запись уровня INFO.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1027">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="70ea7-1028">Используйте `--verbose` для просмотра.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1028">Use `--verbose` to see</span></span>
* <span data-ttu-id="70ea7-1029">Добавьте индикатор хода выполнения для ожидания команд.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1029">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="70ea7-1030">ACS</span><span class="sxs-lookup"><span data-stu-id="70ea7-1030">ACS</span></span>

* <span data-ttu-id="70ea7-1031">Добавлено описание аргумента `--disable-browser`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1031">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="70ea7-1032">Улучшено заполнение нажатием клавиши TAB для аргументов `--vm-size`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1032">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="70ea7-1033">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="70ea7-1033">Appservice</span></span>

* <span data-ttu-id="70ea7-1034">Фиксированное значение `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="70ea7-1034">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="70ea7-1035">Удалена проверка `kind` в веб-приложениях и функциях.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1035">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="70ea7-1036">CDN</span><span class="sxs-lookup"><span data-stu-id="70ea7-1036">CDN</span></span>

* <span data-ttu-id="70ea7-1037">Устранена проблема с отсутствием клиента для команды `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1037">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="70ea7-1038">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="70ea7-1038">CosmosDB</span></span>

* <span data-ttu-id="70ea7-1039">Исправлено описание параметров для политик отработки отказа.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1039">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="70ea7-1040">Interactive</span><span class="sxs-lookup"><span data-stu-id="70ea7-1040">Interactive</span></span>

* <span data-ttu-id="70ea7-1041">Исправлена проблема, когда заполнение параметров команд больше не выполнялось.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1041">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="70ea7-1042">Сеть</span><span class="sxs-lookup"><span data-stu-id="70ea7-1042">Network</span></span>

* <span data-ttu-id="70ea7-1043">Добавлена защита `--cert-password` для `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1043">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="70ea7-1044">Исправлена проблема с `application-gateway update`, когда команда `--sku` ошибочно применяла значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1044">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="70ea7-1045">Добавлена защита `--shared-key` и `--authorization-key` для `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1045">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="70ea7-1046">Устранена проблема с отсутствием клиента для команды `asg create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1046">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="70ea7-1047">Добавлен параметр `--file-name / -f` для экспортируемых имен в `dns zone export`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1047">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="70ea7-1048">Исправлены следующие ошибки для `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="70ea7-1048">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="70ea7-1049">Исправлена проблема, когда длинные записи ТХТ неправильно экспортировались.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1049">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="70ea7-1050">Исправлена проблема, когда записи ТХТ в кавычках неправильно экспортировались без символов экранирования.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1050">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="70ea7-1051">Исправлена проблема, когда некоторые записи импортировались дважды с помощью `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1051">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="70ea7-1052">Восстановлены команды `vnet-gateway root-cert` и `vnet-gateway revoked-cert`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1052">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="70ea7-1053">Профиль</span><span class="sxs-lookup"><span data-stu-id="70ea7-1053">Profile</span></span>

* <span data-ttu-id="70ea7-1054">Исправлена команда `get-access-token` для работы в виртуальной машине с идентификатором.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1054">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="70ea7-1055">Ресурс</span><span class="sxs-lookup"><span data-stu-id="70ea7-1055">Resource</span></span>

* <span data-ttu-id="70ea7-1056">Исправлена ошибка с `deployment [create|validate]`, когда предупреждение неправильно отображалось, если поле type шаблона содержало значения в верхнем регистре.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1056">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="70ea7-1057">Хранилище</span><span class="sxs-lookup"><span data-stu-id="70ea7-1057">Storage</span></span>

* <span data-ttu-id="70ea7-1058">Исправлена проблема с переносом учетных записей хранения из версии 1 в версию 2.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1058">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="70ea7-1059">Добавлены отчеты о ходе выполнения всех команд отправки или скачивания.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1059">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="70ea7-1060">Исправлена ошибка, которая препятствовала использованию параметра аргумента -n с `storage account check-name`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1060">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="70ea7-1061">Добавлен столбец snapshot в табличные выходные данные для `blob [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1061">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="70ea7-1062">Исправлены ошибки с разными параметрами, которые должны были анализироваться как целые числа.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1062">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="70ea7-1063">ВМ</span><span class="sxs-lookup"><span data-stu-id="70ea7-1063">VM</span></span>

* <span data-ttu-id="70ea7-1064">Добавлена команда `vm image accept-terms` для разрешения создания виртуальных машин из образов с дополнительными расходами.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1064">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="70ea7-1065">Исправлена команда `[vm|vmss create]` для выполнения команд с прокси-сервера с помощью неподписанных сертификатов.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1065">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="70ea7-1066">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка режима низкого приоритета для VMSS.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1066">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="70ea7-1067">Добавлена защита `--admin-password` для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1067">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="70ea7-1068">17 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1068">January 17, 2018</span></span>

<span data-ttu-id="70ea7-1069">Версия 2.0.25</span><span class="sxs-lookup"><span data-stu-id="70ea7-1069">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="70ea7-1070">ACR</span><span class="sxs-lookup"><span data-stu-id="70ea7-1070">ACR</span></span>

* <span data-ttu-id="70ea7-1071">Добавлена возможность отката входа ACR при ошибках учетных данных в Windows.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1071">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="70ea7-1072">Включены журналы реестра.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1072">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="70ea7-1073">ACS</span><span class="sxs-lookup"><span data-stu-id="70ea7-1073">ACS</span></span>

* <span data-ttu-id="70ea7-1074">Исправлена команда `get-credentials`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1074">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="70ea7-1075">Удалено требование роли для имени субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1075">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="70ea7-1076">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="70ea7-1076">Appservice</span></span>

* <span data-ttu-id="70ea7-1077">Исправлена ошибка с `config ssl upload`, при которой значение `hosting_environment_profile` было NULL.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1077">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="70ea7-1078">В `browse` добавлена поддержка для пользовательских URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1078">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="70ea7-1079">Исправлена поддержка слотов для `log tail`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1079">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="70ea7-1080">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="70ea7-1080">Backup</span></span>

* <span data-ttu-id="70ea7-1081">Параметр `--container-name` для `backup item list` теперь не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1081">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="70ea7-1082">В `backup restore restore-disks` добавлены варианты учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1082">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="70ea7-1083">Для проверки расположения в `backup protection enable-for-vm` добавлена чувствительность к регистру.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1083">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="70ea7-1084">Устранена проблема, при которой команды завершались сбоем с указанием недопустимого имени контейнера.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1084">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="70ea7-1085">В `backup item list` теперь по умолчанию включен параметр Health Status.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1085">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="70ea7-1086">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="70ea7-1086">Batch</span></span>

* <span data-ttu-id="70ea7-1087">`batch login` теперь возвращает сведения об аутентификации.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1087">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="70ea7-1088">Облако</span><span class="sxs-lookup"><span data-stu-id="70ea7-1088">Cloud</span></span>

* <span data-ttu-id="70ea7-1089">При установке `--profile` в облаке теперь не требуется указывать конечные точки.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1089">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="70ea7-1090">Потребление</span><span class="sxs-lookup"><span data-stu-id="70ea7-1090">Consumption</span></span>

* <span data-ttu-id="70ea7-1091">Добавлены новые команды для резервирования: `consumption reservations summaries` и `consumption reservations details`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1091">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="70ea7-1092">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="70ea7-1092">Event Grid</span></span>

* <span data-ttu-id="70ea7-1093">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid topic event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1093">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="70ea7-1094">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid resource event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1094">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="70ea7-1095">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1095">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="70ea7-1096">Вместо нее следует использовать `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1096">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="70ea7-1097">Добавлена команда `eventgrid topic update`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1097">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="70ea7-1098">Добавлена команда `eventgrid event-subscription update`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1098">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="70ea7-1099">Добавлен параметр `--ids` для команд `eventgrid topic`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1099">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="70ea7-1100">Добавлена поддержка заполнения нажатием клавиши TAB для имен разделов.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1100">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="70ea7-1101">Interactive</span><span class="sxs-lookup"><span data-stu-id="70ea7-1101">Interactive</span></span>

* <span data-ttu-id="70ea7-1102">Устранена проблема, при которой интерактивный режим не работал с Python 2.x.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1102">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="70ea7-1103">Исправлены ошибки при запуске.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1103">Fixed errors on startup</span></span>
* <span data-ttu-id="70ea7-1104">Устранена проблема, при которой некоторые команды не работали в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1104">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="70ea7-1105">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="70ea7-1105">IoT</span></span>

* <span data-ttu-id="70ea7-1106">Добавлена поддержка службы подготовки устройств.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1106">Added support for device provisioning service</span></span>
* <span data-ttu-id="70ea7-1107">В команды и справочную информацию о них добавлены сообщения о нерекомендуемых версиях.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1107">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="70ea7-1108">Теперь при проверке Интернета вещей указывается расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1108">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="70ea7-1109">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="70ea7-1109">Monitor</span></span>

* <span data-ttu-id="70ea7-1110">Добавлена поддержка параметра нескольких диагностических операций.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1110">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="70ea7-1111">Теперь параметр `--name` является обязательным для `az monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1111">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="70ea7-1112">Добавлена команда `monitor diagnostic-settings categories` для получения категории параметров диагностики.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1112">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="70ea7-1113">Сеть</span><span class="sxs-lookup"><span data-stu-id="70ea7-1113">Network</span></span>

* <span data-ttu-id="70ea7-1114">Устранена проблема с `vnet-gateway update` при попытке входа в активный режим и режим ожидания или выхода из них.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1114">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="70ea7-1115">Для `application-gateway [create|update]` добавлена поддержка HTTP2.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1115">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="70ea7-1116">Профиль</span><span class="sxs-lookup"><span data-stu-id="70ea7-1116">Profile</span></span>

* <span data-ttu-id="70ea7-1117">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1117">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="70ea7-1118">Роль</span><span class="sxs-lookup"><span data-stu-id="70ea7-1118">Role</span></span>

* <span data-ttu-id="70ea7-1119">В `role assignment create` добавлен аргумент `--assignee-object-id`, чтобы обойти запрос графов.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1119">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="70ea7-1120">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="70ea7-1120">Service Fabric</span></span>

* <span data-ttu-id="70ea7-1121">В результат проверки при создании кластера добавлены подробные сведения об ошибках.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1121">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="70ea7-1122">Устранена проблема отсутствия клиента при выполнении некоторых команд.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1122">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="70ea7-1123">ВМ</span><span class="sxs-lookup"><span data-stu-id="70ea7-1123">VM</span></span>

* <span data-ttu-id="70ea7-1124">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Поддержка разных зон для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1124">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="70ea7-1125">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию `vmss` для одной зоны заменено данными подсистемы балансировки нагрузки уровня "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="70ea7-1125">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="70ea7-1126">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для EMSI параметр `externalIdentities` изменен на `userAssignedIdentities`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1126">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="70ea7-1127">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка переключения дисков ОС.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1127">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="70ea7-1128">Добавлена поддержка использования образов виртуальных машин из других подписок.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1128">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="70ea7-1129">В `[vm|vmss] create` добавлены аргументы `--plan-name`, `--plan-product`, `--plan-promotion-code` и `--plan-publisher`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1129">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="70ea7-1130">Устранены проблемы с `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1130">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="70ea7-1131">Устранена проблема чрезмерного использования ресурсов из-за `vm image list --all`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1131">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="70ea7-1132">19 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1132">December 19, 2017</span></span>

<span data-ttu-id="70ea7-1133">Версия 2.0.23</span><span class="sxs-lookup"><span data-stu-id="70ea7-1133">Version 2.0.23</span></span>

* <span data-ttu-id="70ea7-1134">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1134">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="70ea7-1135">Контейнер</span><span class="sxs-lookup"><span data-stu-id="70ea7-1135">Container</span></span>

* <span data-ttu-id="70ea7-1136">Исправлен неправильный порядок параметров для журналов контейнеров.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1136">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="70ea7-1137">Сеть</span><span class="sxs-lookup"><span data-stu-id="70ea7-1137">Network</span></span>

* <span data-ttu-id="70ea7-1138">Добавлен аргумент `--disable-bgp-route-propagation` для команды `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="70ea7-1138">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="70ea7-1139">Добавлен аргумент `--ip-tags` для команды `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="70ea7-1139">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="70ea7-1140">Хранилище</span><span class="sxs-lookup"><span data-stu-id="70ea7-1140">Storage</span></span>

* <span data-ttu-id="70ea7-1141">Добавлена поддержка хранилища версии 2.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1141">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="70ea7-1142">ВМ</span><span class="sxs-lookup"><span data-stu-id="70ea7-1142">VM</span></span>

* <span data-ttu-id="70ea7-1143">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для назначенных пользователям удостоверений для виртуальных машин и VMSS.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1143">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="70ea7-1144">5 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1144">December 5, 2017</span></span>

<span data-ttu-id="70ea7-1145">Версия 2.0.22</span><span class="sxs-lookup"><span data-stu-id="70ea7-1145">Version 2.0.22</span></span>

* <span data-ttu-id="70ea7-1146">Удалена команда `az component`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1146">Removed `az component` commands.</span></span> <span data-ttu-id="70ea7-1147">Вместо нее следует использовать `az extension`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1147">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="70ea7-1148">Core</span><span class="sxs-lookup"><span data-stu-id="70ea7-1148">Core</span></span>
* <span data-ttu-id="70ea7-1149">Конечная точка `AZURE_US_GOV_CLOUD` центра AAD изменена с login.microsoftonline.com на login.microsoftonline.us.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1149">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="70ea7-1150">Исправлена проблема с непрерывной отправкой телеметрии.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1150">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="70ea7-1151">ACS</span><span class="sxs-lookup"><span data-stu-id="70ea7-1151">ACS</span></span>

* <span data-ttu-id="70ea7-1152">Добавлены команды `aks install-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1152">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="70ea7-1153">Улучшены сообщения об ошибках для команды `acs create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1153">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="70ea7-1154">Добавлена возможность использования команды `aks get-credentials -f` без полного пути.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1154">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="70ea7-1155">Помощник</span><span class="sxs-lookup"><span data-stu-id="70ea7-1155">Advisor</span></span>

* <span data-ttu-id="70ea7-1156">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="70ea7-1156">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="70ea7-1157">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="70ea7-1157">Appservice</span></span>

* <span data-ttu-id="70ea7-1158">Добавлена возможность создания имени сертификата с помощью команды `webapp config ssl upload`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1158">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="70ea7-1159">Исправлены команды `webapp [list|show]` и `functionapp [list|show]` для отображения правильных приложений.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1159">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="70ea7-1160">Добавлено стандартное значение для переменной `WEBSITE_NODE_DEFAULT_VERSION`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1160">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="70ea7-1161">Потребление</span><span class="sxs-lookup"><span data-stu-id="70ea7-1161">Consumption</span></span>

* <span data-ttu-id="70ea7-1162">Добавлена поддержка API версии 2017-11-30.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1162">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="70ea7-1163">Контейнер</span><span class="sxs-lookup"><span data-stu-id="70ea7-1163">Container</span></span>

* <span data-ttu-id="70ea7-1164">Исправлены стандартные порты регрессии.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1164">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="70ea7-1165">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="70ea7-1165">Monitor</span></span>

* <span data-ttu-id="70ea7-1166">Добавлена поддержка нескольких измерений для команд метрик.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1166">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="70ea7-1167">Ресурс</span><span class="sxs-lookup"><span data-stu-id="70ea7-1167">Resource</span></span>

* <span data-ttu-id="70ea7-1168">Добавлен аргумент `--include-response-body` для команды `resource show`</span><span class="sxs-lookup"><span data-stu-id="70ea7-1168">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="70ea7-1169">Роль</span><span class="sxs-lookup"><span data-stu-id="70ea7-1169">Role</span></span>

* <span data-ttu-id="70ea7-1170">Добавлено отображение стандартных назначений "классических" администраторов для команды `role assignment list`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1170">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="70ea7-1171">Добавлена поддержка команды `ad sp reset-credentials` для добавления учетных данных вместо перезаписи.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1171">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="70ea7-1172">Улучшены сообщения об ошибках для команды `ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1172">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="70ea7-1173">SQL</span><span class="sxs-lookup"><span data-stu-id="70ea7-1173">SQL</span></span>

* <span data-ttu-id="70ea7-1174">Добавлены команды `sql db list-usages` и `sql db show-usage`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1174">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="70ea7-1175">Добавлены команды `sql server conn-policy show` и `sql server conn-policy update`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1175">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="70ea7-1176">ВМ</span><span class="sxs-lookup"><span data-stu-id="70ea7-1176">VM</span></span>

* <span data-ttu-id="70ea7-1177">Добавлены сведения о зонах для команды `az vm list-skus`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1177">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="70ea7-1178">14 ноября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1178">November 14, 2017</span></span>

<span data-ttu-id="70ea7-1179">Версия 2.0.21</span><span class="sxs-lookup"><span data-stu-id="70ea7-1179">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="70ea7-1180">ACR</span><span class="sxs-lookup"><span data-stu-id="70ea7-1180">ACR</span></span>

* <span data-ttu-id="70ea7-1181">Добавлена поддержка создания веб-перехватчиков в регионах репликации.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1181">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="70ea7-1182">ACS</span><span class="sxs-lookup"><span data-stu-id="70ea7-1182">ACS</span></span>

* <span data-ttu-id="70ea7-1183">В AKS агент теперь называется узлом.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1183">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="70ea7-1184">Параметр `--orchestrator-release` для командлета `acs create` не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1184">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="70ea7-1185">Изменен размер виртуальной машины для AKS по умолчанию на `Standard_D1_v2`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1185">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="70ea7-1186">Исправлена команда `az aks browse` для Windows.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1186">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="70ea7-1187">Исправлена команда `az aks get-credentials` для Windows.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1187">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="70ea7-1188">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="70ea7-1188">Appservice</span></span>

* <span data-ttu-id="70ea7-1189">Добавлен источник развертывания `config-zip` для веб-приложений и приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1189">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="70ea7-1190">Добавлен параметр `--docker-container-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1190">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="70ea7-1191">Удален параметр `storage` из параметра `--web-server-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1191">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="70ea7-1192">Улучшены сообщения об ошибках для команды `deployment user set`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1192">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="70ea7-1193">Добавлена поддержка создания приложений-функций Linux</span><span class="sxs-lookup"><span data-stu-id="70ea7-1193">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="70ea7-1194">Фиксированное значение `list-locations`</span><span class="sxs-lookup"><span data-stu-id="70ea7-1194">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="70ea7-1195">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="70ea7-1195">Batch</span></span>

* <span data-ttu-id="70ea7-1196">Исправлена ошибка в команде создания пула, когда идентификатор ресурса использовался с флагом `--image`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1196">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="70ea7-1197">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="70ea7-1197">Batchai</span></span>

* <span data-ttu-id="70ea7-1198">Добавлен короткий параметр `-s` для параметра `--vm-size` при указании размера виртуальной машины в команде `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1198">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="70ea7-1199">Добавлены аргументы ключа и имени учетной записи хранения в параметры команды `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1199">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="70ea7-1200">Исправлена документация по командам `job list-files` и `job stream-file`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1200">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="70ea7-1201">Добавлен короткий параметр `-r` для параметра `--cluster-name` при указании имени кластера в команде `job create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1201">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="70ea7-1202">Облако</span><span class="sxs-lookup"><span data-stu-id="70ea7-1202">Cloud</span></span>

* <span data-ttu-id="70ea7-1203">Изменена команда `cloud [register|update]` для предотвращения регистрации облаков, для которых отсутствуют необходимые конечные точки.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1203">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="70ea7-1204">Контейнер</span><span class="sxs-lookup"><span data-stu-id="70ea7-1204">Container</span></span>

* <span data-ttu-id="70ea7-1205">Добавлена поддержка открытия нескольких портов.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1205">Added support to open multiple ports</span></span>
* <span data-ttu-id="70ea7-1206">Добавлена политика перезапуска группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1206">Added container group restart policy</span></span>
* <span data-ttu-id="70ea7-1207">Добавлена поддержка подключения файлового ресурса Azure в качестве тома.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1207">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="70ea7-1208">Обновлена вспомогательная документация.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1208">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="70ea7-1209">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="70ea7-1209">Data Lake Analytics</span></span>

* <span data-ttu-id="70ea7-1210">Изменена команда `[job|account] list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1210">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="70ea7-1211">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="70ea7-1211">Data Lake Store</span></span>

* <span data-ttu-id="70ea7-1212">Изменена команда `account list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1212">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="70ea7-1213">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="70ea7-1213">Extension</span></span>

* <span data-ttu-id="70ea7-1214">Добавлена команда `extension list-available` для отображения официальных расширений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1214">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="70ea7-1215">Добавлен параметр `--name` для команды `extension [add|update]` для установки расширений по имени.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1215">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="70ea7-1216">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="70ea7-1216">IoT</span></span>

* <span data-ttu-id="70ea7-1217">Добавлена поддержка центров сертификации (ЦС) и цепочек сертификатов.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1217">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="70ea7-1218">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="70ea7-1218">Monitor</span></span>

* <span data-ttu-id="70ea7-1219">Добавлены команды `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1219">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="70ea7-1220">Сеть</span><span class="sxs-lookup"><span data-stu-id="70ea7-1220">Network</span></span>

* <span data-ttu-id="70ea7-1221">Добавлена поддержка DNS-записей типа CAA.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1221">Added support for CAA DNS records</span></span>
* <span data-ttu-id="70ea7-1222">Исправлена проблема, когда конечные точки могли не обновляться с помощью команды `traffic-manager profile update`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1222">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="70ea7-1223">Исправлена проблема, когда команда `vnet update --dns-servers` не работала в зависимости от способа создания виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1223">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="70ea7-1224">Исправлена проблема, когда относительные DNS-имена неправильно импортировались с помощью команды `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1224">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="70ea7-1225">Резервирование</span><span class="sxs-lookup"><span data-stu-id="70ea7-1225">Reservations</span></span>

* <span data-ttu-id="70ea7-1226">Первоначальный выпуск предварительной версии</span><span class="sxs-lookup"><span data-stu-id="70ea7-1226">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="70ea7-1227">Ресурс</span><span class="sxs-lookup"><span data-stu-id="70ea7-1227">Resource</span></span>

* <span data-ttu-id="70ea7-1228">Добавлена поддержка идентификаторов ресурсов для блокировок на уровне ресурсов и параметра `--resource`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1228">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="70ea7-1229">SQL</span><span class="sxs-lookup"><span data-stu-id="70ea7-1229">SQL</span></span>

* <span data-ttu-id="70ea7-1230">Добавлен параметр `--ignore-missing-vnet-service-endpoint` для команды `sql server vnet-rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1230">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="70ea7-1231">Хранилище</span><span class="sxs-lookup"><span data-stu-id="70ea7-1231">Storage</span></span>

* <span data-ttu-id="70ea7-1232">Изменена команда `storage account create` для использования номера SKU `Standard_RAGRS` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1232">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="70ea7-1233">Исправлены ошибки при обработке имени файла или большого двоичного объекта, содержащего символы, отличные от ASCII.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1233">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="70ea7-1234">Исправлена ошибка, препятствующая использованию параметра `--source-uri` с командой `storage [blob|file] copy start-batch`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1234">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="70ea7-1235">Добавлены команды для удаления нескольких объектов с помощью команды `storage [blob|file] delete-batch`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1235">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="70ea7-1236">Исправлена проблема с включением метрик с помощью команды `storage metrics update`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1236">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="70ea7-1237">Исправлена проблема с файлами более 200 ГБ при использовании команды `storage blob upload-batch`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1237">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="70ea7-1238">Исправлена проблема, когда параметры `--bypass` и `--default-action` игнорировались командой `storage account [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1238">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="70ea7-1239">ВМ</span><span class="sxs-lookup"><span data-stu-id="70ea7-1239">VM</span></span>

* <span data-ttu-id="70ea7-1240">Исправлена ошибка с командой `vmss create`, препятствующая использованию уровня `Basic`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1240">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="70ea7-1241">Добавлены аргументы `--plan` для команды `[vm|vmss] create` для пользовательских образов с информацией о выставлении счетов.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1241">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="70ea7-1242">Добавлены команды `vm secret `[add|remove|list]\`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1242">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="70ea7-1243">Команда `vm format-secret` переименована в `vm secret format`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1243">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="70ea7-1244">Добавлен аргумент `--encrypt format` для команды `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="70ea7-1244">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="70ea7-1245">24 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1245">October 24, 2017</span></span>

<span data-ttu-id="70ea7-1246">Версия 2.0.20</span><span class="sxs-lookup"><span data-stu-id="70ea7-1246">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="70ea7-1247">Core</span><span class="sxs-lookup"><span data-stu-id="70ea7-1247">Core</span></span>

* <span data-ttu-id="70ea7-1248">Обновление `2017-03-09-profile` для использования API `MGMT_STORAGE` версии `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="70ea7-1248">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="70ea7-1249">ACR</span><span class="sxs-lookup"><span data-stu-id="70ea7-1249">ACR</span></span>

* <span data-ttu-id="70ea7-1250">Обновление службы управления ресурсами для указания API версии `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="70ea7-1250">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="70ea7-1251">Изменение номера SKU BYOS-хранилища на "Классический"</span><span class="sxs-lookup"><span data-stu-id="70ea7-1251">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="70ea7-1252">Переименование номеров SKU реестра на "Базовый", "Стандартный" и "Премиум"</span><span class="sxs-lookup"><span data-stu-id="70ea7-1252">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="70ea7-1253">ACS</span><span class="sxs-lookup"><span data-stu-id="70ea7-1253">ACS</span></span>

* <span data-ttu-id="70ea7-1254">[ПРЕДВАРИЕТЛЬНАЯ ВЕРСИЯ] Добавление команд `az aks`</span><span class="sxs-lookup"><span data-stu-id="70ea7-1254">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="70ea7-1255">Исправление Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="70ea7-1255">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="70ea7-1256">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="70ea7-1256">Appservice</span></span>

* <span data-ttu-id="70ea7-1257">Исправление проблемы с недопустимыми скачанными журналами `webapp`</span><span class="sxs-lookup"><span data-stu-id="70ea7-1257">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="70ea7-1258">Компонент</span><span class="sxs-lookup"><span data-stu-id="70ea7-1258">Component</span></span>

* <span data-ttu-id="70ea7-1259">Добавление более понятного сообщения об устаревании для всех установщиков, а также запроса на подтверждение</span><span class="sxs-lookup"><span data-stu-id="70ea7-1259">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="70ea7-1260">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="70ea7-1260">Monitor</span></span>

* <span data-ttu-id="70ea7-1261">Добавлены команды `action-group`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1261">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="70ea7-1262">Ресурс</span><span class="sxs-lookup"><span data-stu-id="70ea7-1262">Resource</span></span>

* <span data-ttu-id="70ea7-1263">Исправление несовместимости с самой последней версии зависимости msrest в `group export`</span><span class="sxs-lookup"><span data-stu-id="70ea7-1263">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="70ea7-1264">Исправление `policy assignment create` для работы с определениями встроенных политик и наборов политик</span><span class="sxs-lookup"><span data-stu-id="70ea7-1264">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="70ea7-1265">ВМ</span><span class="sxs-lookup"><span data-stu-id="70ea7-1265">VM</span></span>

* <span data-ttu-id="70ea7-1266">Добавлен аргумент `--accelerated-networking` для команды `vmss create`</span><span class="sxs-lookup"><span data-stu-id="70ea7-1266">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="70ea7-1267">9 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1267">October 9, 2017</span></span>

<span data-ttu-id="70ea7-1268">Версия 2.0.19</span><span class="sxs-lookup"><span data-stu-id="70ea7-1268">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="70ea7-1269">Core</span><span class="sxs-lookup"><span data-stu-id="70ea7-1269">Core</span></span>

* <span data-ttu-id="70ea7-1270">В Azure Stack добавлена обработка URL-адресов центра ADFS с завершающей косой чертой.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1270">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="70ea7-1271">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="70ea7-1271">Appservice</span></span>

* <span data-ttu-id="70ea7-1272">Добавлена возможность общего обновления с помощью новой команды `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1272">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="70ea7-1273">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="70ea7-1273">Batch</span></span>

* <span data-ttu-id="70ea7-1274">Обновление до пакета SDK для пакетной службы версии 4.0.0</span><span class="sxs-lookup"><span data-stu-id="70ea7-1274">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="70ea7-1275">Обновлен параметр `--image` для команды VirtualMachineConfiguration, обеспечивающий поддержку ссылок на образы ARM в дополнение к publish:offer:sku:version.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1275">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="70ea7-1276">Добавлена поддержка новой модели расширений CLI для команд расширений пакетной службы.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1276">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="70ea7-1277">Удалена поддержка пакетной службы для модели компонентов.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1277">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="70ea7-1278">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="70ea7-1278">Batchai</span></span>

* <span data-ttu-id="70ea7-1279">Исходный выпуск модуля искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="70ea7-1279">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="70ea7-1280">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="70ea7-1280">Keyvault</span></span>

* <span data-ttu-id="70ea7-1281">Исправлена проблема с аутентификацией Key Vault при использовании ADFS в Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1281">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="70ea7-1282">(#4448)</span><span class="sxs-lookup"><span data-stu-id="70ea7-1282">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="70ea7-1283">Сеть</span><span class="sxs-lookup"><span data-stu-id="70ea7-1283">Network</span></span>

* <span data-ttu-id="70ea7-1284">Аргумент `--server` для `application-gateway address-pool create` изменен на необязательный (разрешено использование пустых пулов адресов).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1284">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="70ea7-1285">Обновлен элемент `traffic-manager` для поддержки последних функций.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1285">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="70ea7-1286">Ресурс</span><span class="sxs-lookup"><span data-stu-id="70ea7-1286">Resource</span></span>

* <span data-ttu-id="70ea7-1287">Добавлена поддержка параметров `--resource-group/-g` для изменения имени группы ресурсов на `group`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1287">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="70ea7-1288">Добавлены команды для `account lock` для работы с блокировками на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1288">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="70ea7-1289">Добавлены команды для `group lock` для работы с блокировками на уровне группы.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1289">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="70ea7-1290">Добавлены команды для `resource lock` для работы с блокировками на уровне ресурса.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1290">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="70ea7-1291">SQL</span><span class="sxs-lookup"><span data-stu-id="70ea7-1291">Sql</span></span>

* <span data-ttu-id="70ea7-1292">Добавлена поддержка SQL TDE и BYOK TDE.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1292">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="70ea7-1293">Добавлена команда `db list-deleted` и параметр `db restore --deleted-time` для поиска и восстановления удаленных баз данных.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1293">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="70ea7-1294">Добавлено `db op list` и `db op cancel` для отображения и отмены выполняющихся операций в базе данных.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1294">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="70ea7-1295">Хранилище</span><span class="sxs-lookup"><span data-stu-id="70ea7-1295">Storage</span></span>

* <span data-ttu-id="70ea7-1296">Добавлена поддержка моментальных снимков файловых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1296">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="70ea7-1297">Виртуальные машины</span><span class="sxs-lookup"><span data-stu-id="70ea7-1297">Vm</span></span>

* <span data-ttu-id="70ea7-1298">Исправлена ошибка в команде `vm show`, когда использование `-d` вызывало сбой отсутствующих частных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1298">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="70ea7-1299">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка последовательного обновления для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1299">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="70ea7-1300">Добавлена поддержка обновления параметров шифрования с помощью команды `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1300">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="70ea7-1301">Добавлен параметр `--os-disk-size-gb` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1301">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="70ea7-1302">Добавлен параметр `--license-type` для команды `vmss create` (для Windows).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1302">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="70ea7-1303">22 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1303">September 22, 2017</span></span>

<span data-ttu-id="70ea7-1304">Версия 2.0.18</span><span class="sxs-lookup"><span data-stu-id="70ea7-1304">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="70ea7-1305">Ресурс</span><span class="sxs-lookup"><span data-stu-id="70ea7-1305">Resource</span></span>

* <span data-ttu-id="70ea7-1306">Добавлена поддержка отображения определений встроенных политик</span><span class="sxs-lookup"><span data-stu-id="70ea7-1306">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="70ea7-1307">Добавлена поддержка параметра mode для создания определения политик</span><span class="sxs-lookup"><span data-stu-id="70ea7-1307">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="70ea7-1308">Добавлена поддержка шаблонов и определений пользовательского интерфейса для команды `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="70ea7-1308">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="70ea7-1309">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен тип ресурса `managedapp` с `appliances` на `applications` и с `applianceDefinitions` на `applicationDefinitions`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1309">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="70ea7-1310">Сеть</span><span class="sxs-lookup"><span data-stu-id="70ea7-1310">Network</span></span>

* <span data-ttu-id="70ea7-1311">Добавлена поддержка зоны доступности для подкоманд `network lb` и `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="70ea7-1311">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="70ea7-1312">Добавлена поддержка IPv6 (пиринг Майкрософт) для `express-route`</span><span class="sxs-lookup"><span data-stu-id="70ea7-1312">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="70ea7-1313">Добавлены команды группы безопасности приложения `asg`</span><span class="sxs-lookup"><span data-stu-id="70ea7-1313">Added `asg` application security group commands</span></span>
* <span data-ttu-id="70ea7-1314">Добавлен аргумент `--application-security-groups` для команды `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="70ea7-1314">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="70ea7-1315">Добавлены аргументы `--source-asgs` и `--destination-asgs` для команды `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="70ea7-1315">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="70ea7-1316">Добавлены аргументы `--ddos-protection` и `--vm-protection` для команды `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="70ea7-1316">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="70ea7-1317">Добавлены команды `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1317">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="70ea7-1318">Хранилище</span><span class="sxs-lookup"><span data-stu-id="70ea7-1318">Storage</span></span>

* <span data-ttu-id="70ea7-1319">Исправлена проблема, когда команды `storage account network-rule` могут не работать после обновления пакета SDK</span><span class="sxs-lookup"><span data-stu-id="70ea7-1319">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="70ea7-1320">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="70ea7-1320">Eventgrid</span></span>

* <span data-ttu-id="70ea7-1321">Обновлен пакет SDK Python для службы "Сетка событий Azure" для использования новой версии API 2017-09-15-preview</span><span class="sxs-lookup"><span data-stu-id="70ea7-1321">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="70ea7-1322">SQL</span><span class="sxs-lookup"><span data-stu-id="70ea7-1322">SQL</span></span>

* <span data-ttu-id="70ea7-1323">Аргумент `--resource-group` для команды `sql server list` сделан необязательным.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1323">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="70ea7-1324">Если он не указан, возвращаются все серверы SQL Server в подписке</span><span class="sxs-lookup"><span data-stu-id="70ea7-1324">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="70ea7-1325">Добавлен параметр `--no-wait` для команд `db [create|copy|restore|update|replica create|create|update]` и `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="70ea7-1325">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="70ea7-1326">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="70ea7-1326">Keyvault</span></span>

* <span data-ttu-id="70ea7-1327">Добавлена поддержка команд хранилища ключей за прокси-сервером</span><span class="sxs-lookup"><span data-stu-id="70ea7-1327">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="70ea7-1328">ВМ</span><span class="sxs-lookup"><span data-stu-id="70ea7-1328">VM</span></span>

* <span data-ttu-id="70ea7-1329">Добавлена поддержка зоны доступности для команды `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="70ea7-1329">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="70ea7-1330">Исправлена проблема, когда использование аргумента `--app-gateway ID` с командой `vmss create` приводило к сбою</span><span class="sxs-lookup"><span data-stu-id="70ea7-1330">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="70ea7-1331">Добавлен аргумент `--asgs` для команды `vm create`</span><span class="sxs-lookup"><span data-stu-id="70ea7-1331">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="70ea7-1332">Добавлена поддержка выполнения команд на виртуальных машинах с помощью команды `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="70ea7-1332">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="70ea7-1333">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка шифрования диска VMSS с помощью команды `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="70ea7-1333">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="70ea7-1334">Добавлена поддержка обслуживания виртуальных машин с помощью команды `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="70ea7-1334">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="70ea7-1335">ACS</span><span class="sxs-lookup"><span data-stu-id="70ea7-1335">ACS</span></span>

* <span data-ttu-id="70ea7-1336">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлен аргумент `--orchestrator-release` для команды `acs create` для регионов служб ACS (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="70ea7-1336">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="70ea7-1337">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="70ea7-1337">Appservice</span></span>

* <span data-ttu-id="70ea7-1338">Добавлена возможность обновлять и отображать параметры аутентификации с помощью команды `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="70ea7-1338">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="70ea7-1339">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="70ea7-1339">Backup</span></span>

* <span data-ttu-id="70ea7-1340">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1340">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="70ea7-1341">11 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1341">September 11, 2017</span></span>

<span data-ttu-id="70ea7-1342">Версия 2.0.17</span><span class="sxs-lookup"><span data-stu-id="70ea7-1342">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="70ea7-1343">Core</span><span class="sxs-lookup"><span data-stu-id="70ea7-1343">Core</span></span>

* <span data-ttu-id="70ea7-1344">Включен командный модуль для настройки собственного идентификатора корреляции в телеметрии.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1344">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="70ea7-1345">Исправлена проблема с дампом JSON, когда для телеметрии настроен режим диагностики.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1345">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="70ea7-1346">ACS</span><span class="sxs-lookup"><span data-stu-id="70ea7-1346">Acs</span></span>

* <span data-ttu-id="70ea7-1347">Добавлена команда `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1347">Added `acs list-locations` command</span></span>
* <span data-ttu-id="70ea7-1348">Для `ssh-key-file` предоставляется ожидаемое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1348">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="70ea7-1349">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="70ea7-1349">Appservice</span></span>

* <span data-ttu-id="70ea7-1350">Добавлена возможность создавать веб-приложения в группе ресурсов в рамках плана службы, отличной от активной.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1350">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="70ea7-1351">CDN</span><span class="sxs-lookup"><span data-stu-id="70ea7-1351">CDN</span></span>

* <span data-ttu-id="70ea7-1352">Исправлена ошибка "CustomDomain не пригоден к итерации" для `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1352">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="70ea7-1353">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="70ea7-1353">Extension</span></span>

* <span data-ttu-id="70ea7-1354">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="70ea7-1354">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="70ea7-1355">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="70ea7-1355">Keyvault</span></span>

* <span data-ttu-id="70ea7-1356">Исправлена проблема с зависимостью разрешений от регистра для `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1356">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="70ea7-1357">Сеть</span><span class="sxs-lookup"><span data-stu-id="70ea7-1357">Network</span></span>

* <span data-ttu-id="70ea7-1358">Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1358">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="70ea7-1359">Аргумент `--private-access-services` переименован в `--service-endpoints` для команды `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1359">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="70ea7-1360">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1360">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="70ea7-1361">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1361">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="70ea7-1362">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1362">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="70ea7-1363">Ресурс</span><span class="sxs-lookup"><span data-stu-id="70ea7-1363">Resource</span></span>

* <span data-ttu-id="70ea7-1364">Разрешена передача в определениях параметров политики ресурсов в командах `policy definition create` и `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1364">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="70ea7-1365">Разрешена передача значений параметров для команды `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1365">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="70ea7-1366">Разрешена передача JSON или файла для всех параметров.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1366">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="70ea7-1367">Версия API изменена на более позднюю.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1367">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="70ea7-1368">SQL</span><span class="sxs-lookup"><span data-stu-id="70ea7-1368">SQL</span></span>

* <span data-ttu-id="70ea7-1369">Добавлены команды `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1369">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="70ea7-1370">ВМ</span><span class="sxs-lookup"><span data-stu-id="70ea7-1370">VM</span></span>

* <span data-ttu-id="70ea7-1371">Исправлено: не назначать доступ, если `--scope` не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1371">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="70ea7-1372">Исправлено: использование тех же расширений имен, что и для портала.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1372">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="70ea7-1373">Удалено `subscription` из выходных данных `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1373">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="70ea7-1374">Исправлено: номер SKU хранилища `[vm|vmss] create` неприменим для дисков данных с образом.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1374">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="70ea7-1375">Исправлено: `vm format-secret --secrets` не принимает идентификаторы, разделенные строками.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1375">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="70ea7-1376">31 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1376">August 31, 2017</span></span>

<span data-ttu-id="70ea7-1377">Версия 2.0.16</span><span class="sxs-lookup"><span data-stu-id="70ea7-1377">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="70ea7-1378">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="70ea7-1378">Keyvault</span></span>

* <span data-ttu-id="70ea7-1379">Исправлена ошибка при попытке автоматически разрешить шифрование секрета с помощью `secret download`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1379">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="70ea7-1380">Sf</span><span class="sxs-lookup"><span data-stu-id="70ea7-1380">Sf</span></span>

* <span data-ttu-id="70ea7-1381">Объявлены неподдерживаемыми все команды; вместо них используется Service Fabric CLI (sfctl).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1381">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="70ea7-1382">Хранилище</span><span class="sxs-lookup"><span data-stu-id="70ea7-1382">Storage</span></span>

* <span data-ttu-id="70ea7-1383">Исправлена проблема, когда учетные записи хранения нельзя было создавать в регионах, которые не поддерживают функцию NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1383">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="70ea7-1384">Определение типа и кодировки содержимого во время передачи больших двоичных объектов и файла, если оба свойства не указаны.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1384">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="70ea7-1385">28 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1385">August 28, 2017</span></span>

<span data-ttu-id="70ea7-1386">Версия 2.0.15</span><span class="sxs-lookup"><span data-stu-id="70ea7-1386">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="70ea7-1387">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="70ea7-1387">CLI</span></span>

* <span data-ttu-id="70ea7-1388">Для `--version` добавлено юридическое примечание.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1388">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="70ea7-1389">ACS</span><span class="sxs-lookup"><span data-stu-id="70ea7-1389">ACS</span></span>

* <span data-ttu-id="70ea7-1390">Исправлены регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1390">Corrected preview regions</span></span>
* <span data-ttu-id="70ea7-1391">Правильно отформатирован параметр по умолчанию `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1391">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="70ea7-1392">Оптимизированы выходные данные команды ACS.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1392">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="70ea7-1393">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="70ea7-1393">Appservice</span></span>

* <span data-ttu-id="70ea7-1394">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправлены несоответствия в выходных данных `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1394">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="70ea7-1395">Добавлен новый псевдоним `-i` в команду `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1395">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="70ea7-1396">Предоставлена команда `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1396">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="70ea7-1397">Предоставлены новые аргументы команды `az webapp delete`, которые позволяют сохранить план службы приложений, метрики и данные регистрации DNS.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1397">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="70ea7-1398">Исправление. Параметры слота определяются правильно.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1398">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="70ea7-1399">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="70ea7-1399">IoT</span></span>

* <span data-ttu-id="70ea7-1400">Исправление 3934. При создании политики существующие политики больше не удаляются.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1400">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="70ea7-1401">Сеть</span><span class="sxs-lookup"><span data-stu-id="70ea7-1401">Network</span></span>

* <span data-ttu-id="70ea7-1402">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1402">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="70ea7-1403">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--private-access-services` переименован в `--service-endpoints` в командах `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1403">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="70ea7-1404">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1404">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="70ea7-1405">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1405">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="70ea7-1406">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1406">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="70ea7-1407">Профиль</span><span class="sxs-lookup"><span data-stu-id="70ea7-1407">Profile</span></span>

* <span data-ttu-id="70ea7-1408">Предоставлены параметры `--msi` и `--msi-port` для входа с использованием удостоверения виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1408">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="70ea7-1409">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="70ea7-1409">Service Fabric</span></span>

* <span data-ttu-id="70ea7-1410">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1410">Preview release</span></span>
* <span data-ttu-id="70ea7-1411">Упрощены правила реестра для паролей и имен пользователя для команды.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1411">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="70ea7-1412">Исправлена строка для ввода пароля пользователем даже после передачи параметра.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1412">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="70ea7-1413">Добавлена поддержка пустого значения `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1413">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="70ea7-1414">Хранилище</span><span class="sxs-lookup"><span data-stu-id="70ea7-1414">Storage</span></span>

* <span data-ttu-id="70ea7-1415">Появилась возможность задавать уровень большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1415">Enabled setting blob tier</span></span>
* <span data-ttu-id="70ea7-1416">Добавлены аргументы `--bypass` и `--default-action` в командах `storage account [create|update]` для поддержки туннелирования службы.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1416">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="70ea7-1417">Добавлены команды для добавления правил виртуальной сети и правил на основе IP-адресов в `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1417">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="70ea7-1418">Разрешено шифрование службы с управляемым пользователем ключом.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1418">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="70ea7-1419">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--encryption` переименован в `--encryption-services` в команде `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1419">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="70ea7-1420">Исправление 4220. Несоответствие синтаксиса `az storage account update encryption`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1420">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="70ea7-1421">ВМ</span><span class="sxs-lookup"><span data-stu-id="70ea7-1421">VM</span></span>

* <span data-ttu-id="70ea7-1422">Исправлена проблема, из-за которой для команды `vmss get-instance-view` отображались лишние и неправильные сведения при использовании параметра `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1422">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="70ea7-1423">Добавлена поддержка параметра `--lb-sku` в команде `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1423">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="70ea7-1424">Из черного списка имен администраторов для команд `[vm|vmss] create` удалены имена людей.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1424">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="70ea7-1425">Исправлена проблема, из-за которой команда `[vm|vmss] create` выдавала ошибку, если из образа не удавалось извлечь сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1425">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="70ea7-1426">Исправлена проблема, которая приводила к сбою при создании масштабируемого набора виртуальных машин с внутренней подсистемой балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1426">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="70ea7-1427">Исправлена проблема, из-за которой аргумент `--no-wait` не работал с командой `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1427">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="70ea7-1428">15 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1428">August 15, 2017</span></span>

<span data-ttu-id="70ea7-1429">Версия 2.0.14</span><span class="sxs-lookup"><span data-stu-id="70ea7-1429">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="70ea7-1430">ACS</span><span class="sxs-lookup"><span data-stu-id="70ea7-1430">ACS</span></span>

* <span data-ttu-id="70ea7-1431">Исправлен номер порта sshMaster0 для Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1431">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="70ea7-1432">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="70ea7-1432">Appservice</span></span>

* <span data-ttu-id="70ea7-1433">Исправлено исключение при создании веб-приложения Linux на основе Git.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1433">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="70ea7-1434">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="70ea7-1434">Event Grid</span></span>

* <span data-ttu-id="70ea7-1435">Добавлены зависимости пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1435">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="70ea7-1436">11 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1436">August 11, 2017</span></span>

<span data-ttu-id="70ea7-1437">Версия 2.0.13</span><span class="sxs-lookup"><span data-stu-id="70ea7-1437">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="70ea7-1438">ACS</span><span class="sxs-lookup"><span data-stu-id="70ea7-1438">ACS</span></span>

* <span data-ttu-id="70ea7-1439">Добавлены дополнительные регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1439">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="70ea7-1440">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="70ea7-1440">Batch</span></span>

* <span data-ttu-id="70ea7-1441">Пакет SDK для пакетной службы обновлен до версии 3.1.0, а пакет SDK для управления пакетной службой — до версии 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1441">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="70ea7-1442">Добавлена новая команда для отображения количества задач в задании.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1442">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="70ea7-1443">Исправлена ошибка при обработке URL-адреса SAS файла ресурсов.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1443">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="70ea7-1444">Для конечной точки учетной записи пакетной службы теперь поддерживается дополнительный префикс https://.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1444">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="70ea7-1445">Поддерживается добавление к заданию списков, содержащих более 100 задач.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1445">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="70ea7-1446">Добавлено ведение журнала отладки при загрузке командного модуля расширений.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1446">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="70ea7-1447">Компонент</span><span class="sxs-lookup"><span data-stu-id="70ea7-1447">Component</span></span>

* <span data-ttu-id="70ea7-1448">Добавлено предупреждение о прекращении поддержки в команды az component.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1448">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="70ea7-1449">Контейнер</span><span class="sxs-lookup"><span data-stu-id="70ea7-1449">Container</span></span>

* <span data-ttu-id="70ea7-1450">`create`. Исправлена проблема, из-за которой запрещалось использовать знак равенства в переменной среды.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1450">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="70ea7-1451">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="70ea7-1451">Data Lake Store</span></span>

* <span data-ttu-id="70ea7-1452">Включен индикатор хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1452">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="70ea7-1453">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="70ea7-1453">Event Grid</span></span>

* <span data-ttu-id="70ea7-1454">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="70ea7-1454">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="70ea7-1455">Сеть</span><span class="sxs-lookup"><span data-stu-id="70ea7-1455">Network</span></span>

* <span data-ttu-id="70ea7-1456">`lb`. Исправлена проблема, из-за которой некоторые имена дочерних ресурсов не разрешались правильно, если не были указаны.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1456">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="70ea7-1457">`application-gateway {subresource} delete`. Исправлена проблема, из-за которой не учитывался параметр `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1457">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="70ea7-1458">`application-gateway http-settings update`. Исправлена проблема, из-за которой не удавалось отключить параметр `--connection-draining-timeout`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1458">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="70ea7-1459">Исправлена проблема с непредвиденным аргументом ключевого слова `sa_data_size_kilobyes` при использовании с командой `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1459">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="70ea7-1460">Профиль</span><span class="sxs-lookup"><span data-stu-id="70ea7-1460">Profile</span></span>

* <span data-ttu-id="70ea7-1461">`account list`. Добавлен параметр `--refresh` для синхронизации последних подписок с сервером.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1461">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="70ea7-1462">Хранилище</span><span class="sxs-lookup"><span data-stu-id="70ea7-1462">Storage</span></span>

* <span data-ttu-id="70ea7-1463">Включено обновление учетной записи хранения с помощью удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1463">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="70ea7-1464">ВМ</span><span class="sxs-lookup"><span data-stu-id="70ea7-1464">VM</span></span>

* <span data-ttu-id="70ea7-1465">`availability-set`. Предоставлено число доменов сбоя при преобразовании.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1465">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="70ea7-1466">Предоставлена команда `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1466">Exposed `list-skus` command</span></span>
* <span data-ttu-id="70ea7-1467">Поддерживается назначение удостоверений без создания назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1467">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="70ea7-1468">При подключении дисков данных применяется номер SKU хранилища.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1468">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="70ea7-1469">Удалено используемое по умолчанию имя диска ОС и номер SKU хранилища при использовании управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1469">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="70ea7-1470">28 июля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1470">July 28, 2017</span></span>

<span data-ttu-id="70ea7-1471">Версия 2.0.12</span><span class="sxs-lookup"><span data-stu-id="70ea7-1471">Version 2.0.12</span></span>

* <span data-ttu-id="70ea7-1472">Добавлены команды для контейнеров.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1472">Added container commands</span></span>
* <span data-ttu-id="70ea7-1473">Добавлены модули выставления счетов и потребления ресурсов.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1473">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="70ea7-1474">Core</span><span class="sxs-lookup"><span data-stu-id="70ea7-1474">Core</span></span>

* <span data-ttu-id="70ea7-1475">Вывод сведений о пакетах SDK для проверки подлинности субъектов-служб с помощью сертификатов.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1475">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="70ea7-1476">Исправлены исключения в ходе выполнения развертывания.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1476">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="70ea7-1477">Для создания клиента подписки используется конечная точка ARM текущего облака.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1477">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="70ea7-1478">Улучшена параллельная обработка файла clouds.config (3636).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1478">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="70ea7-1479">Обновление идентификатора клиентского запроса при каждом выполнении команды.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1479">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="70ea7-1480">Создание клиентов подписки с правильным профилем SDK (3635).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1480">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="70ea7-1481">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1481">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="70ea7-1482">Добавлена поддержка выбора полей вывода в таблице с помощью запроса jmespath (3581).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1482">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="70ea7-1483">Улучшено отключение аргументов анализа и добавлено ведение журналов с помощью жестов (3434).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1483">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="70ea7-1484">Создание клиентов подписки с правильным профилем SDK.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1484">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="70ea7-1485">Перемещение всех существующих файлов записи в последнюю папку.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1485">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="70ea7-1486">Исправлена идемпотентность при создании виртуальной машины или масштабируемого набора виртуальных машин (3586).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1486">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="70ea7-1487">В путях команд больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1487">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="70ea7-1488">В определенных параметрах логического типа больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1488">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="70ea7-1489">Поддержка входа на локальный сервер AD FS, например Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1489">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="70ea7-1490">Исправлена параллельная запись в файл clouds.config (3255).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1490">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="70ea7-1491">ACR</span><span class="sxs-lookup"><span data-stu-id="70ea7-1491">ACR</span></span>

* <span data-ttu-id="70ea7-1492">Добавлена команда `show-usage` для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1492">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="70ea7-1493">Поддержка обновления номера SKU для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1493">Support SKU update for managed registries</span></span>
* <span data-ttu-id="70ea7-1494">Добавлены управляемые реестры с управляемыми номерами SKU.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1494">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="70ea7-1495">Добавлены веб-перехватчики для управляемых реестров с использованием модуля для команды acr webhook.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1495">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="70ea7-1496">Добавлена проверка подлинности с помощью AAD с использованием команды acr login.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1496">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="70ea7-1497">Добавлена команда delete для репозиториев, манифестов и тегов Docker.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1497">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="70ea7-1498">ACS</span><span class="sxs-lookup"><span data-stu-id="70ea7-1498">ACS</span></span>

* <span data-ttu-id="70ea7-1499">Поддержка API версии 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1499">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="70ea7-1500">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="70ea7-1500">Appservice</span></span>

* <span data-ttu-id="70ea7-1501">Исправлена ошибка, из-за которой команда вывода списка в веб-приложениях Linux не возвращала данные.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1501">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="70ea7-1502">Поддержка извлечения учетных данных из ACR.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1502">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="70ea7-1503">Удаление всех команд группы `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1503">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="70ea7-1504">Создание масок паролей для реестров Docker из выходных данных команды (3656).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1504">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="70ea7-1505">Обеспечено использование браузера по умолчанию в macOS без ошибок (3623).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1505">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="70ea7-1506">Улучшена справка по командам `webapp log tail` и `webapp log download` (3624).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1506">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="70ea7-1507">Предоставлена команда `traffic-routing` для настройки статической маршрутизации (3566).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1507">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="70ea7-1508">Добавлены исправления, связанные с надежностью, при настройке системы управления версиями (3245).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1508">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="70ea7-1509">Удален неподдерживаемый аргумент `--node-version` из функции `webapp config update` для веб-приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1509">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="70ea7-1510">Вместо него используется `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1510">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="70ea7-1511">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="70ea7-1511">Batch</span></span>

* <span data-ttu-id="70ea7-1512">Пакеты SDK для пакетной службы обновлены до версии 3.0.0 с поддержкой низкоприоритетных виртуальных машин в пулах.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1512">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="70ea7-1513">Параметр команды `pool create` переименован с `--target-dedicated` в `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1513">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="70ea7-1514">Для команды `pool create` добавлены параметры `--target-low-priority-nodes` и `--application-licenses`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1514">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="70ea7-1515">CDN</span><span class="sxs-lookup"><span data-stu-id="70ea7-1515">CDN</span></span>

* <span data-ttu-id="70ea7-1516">Предоставлено улучшенное сообщение об ошибке для команды `cdn endpoint list`, которое отображается, если заданный параметром `--profile-name` профиль не существует.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1516">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="70ea7-1517">Облако</span><span class="sxs-lookup"><span data-stu-id="70ea7-1517">Cloud</span></span>

* <span data-ttu-id="70ea7-1518">Формат версии API конечной точки метаданных облака изменен на следующий: ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1518">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="70ea7-1519">Конечная точка коллекции не является обязательной.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1519">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="70ea7-1520">Поддерживается регистрация облака только с конечной точкой диспетчера ARM.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1520">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="70ea7-1521">Предоставлен параметр в команде `cloud set` для выбора профиля при выборе текущего облака.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1521">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="70ea7-1522">Предоставлен параметр `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1522">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="70ea7-1523">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="70ea7-1523">CosmosDB</span></span>

* <span data-ttu-id="70ea7-1524">Внесены исправления, которые позволяют создавать коллекцию с пользовательским ключом секции.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1524">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="70ea7-1525">Добавлена поддержка срока жизни по умолчанию для коллекции.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1525">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="70ea7-1526">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="70ea7-1526">Data Lake Analytics</span></span>

* <span data-ttu-id="70ea7-1527">Добавлены команды для управления политикой вычислений в разделе `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1527">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="70ea7-1528">Добавлена команда `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1528">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="70ea7-1529">Добавлена команда `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1529">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="70ea7-1530">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="70ea7-1530">Data Lake Store</span></span>

* <span data-ttu-id="70ea7-1531">Добавлена поддержка смены ключей пользовательского хранилища ключей в `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1531">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="70ea7-1532">Обновлена версия пакета SDK для базовой файловой системы Data Lake Store из-за проблем с производительностью.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1532">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="70ea7-1533">Добавлена команда `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1533">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="70ea7-1534">Эта команда пытается активировать пользовательское хранилище ключей, предназначенное для шифрования данных в учетной записи Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1534">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="70ea7-1535">Интерактивный режим</span><span class="sxs-lookup"><span data-stu-id="70ea7-1535">Interactive</span></span>

* <span data-ttu-id="70ea7-1536">Улучшено время запуска с помощью кэшированных команд.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1536">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="70ea7-1537">Увеличено тестовое покрытие.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1537">Increased test coverage</span></span>
* <span data-ttu-id="70ea7-1538">Расширены возможности жеста "?", которые позволяют также вставить его в следующую команду.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1538">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="70ea7-1539">Исправлены ошибки с интерактивными функциями в предварительной версии профиля 2017-03-09 (3587).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1539">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="70ea7-1540">Разрешено использовать `--version` в качестве параметра в интерактивном режиме (3645).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1540">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="70ea7-1541">В интерактивном режиме больше не возникают ошибки при выполнении проверки (3570).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1541">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="70ea7-1542">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1542">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="70ea7-1543">Добавлен флаг `--progress`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1543">Added `--progress` flag</span></span>
* <span data-ttu-id="70ea7-1544">Из вариантов завершения удалены `--debug` и `--verbose`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1544">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="70ea7-1545">Из вариантов завершения удален `interactive` (3324).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1545">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="70ea7-1546">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="70ea7-1546">IoT</span></span>

* <span data-ttu-id="70ea7-1547">Исправлено. При создании политики больше не удаляются существующие политики</span><span class="sxs-lookup"><span data-stu-id="70ea7-1547">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="70ea7-1548">(3934).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1548">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="70ea7-1549">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="70ea7-1549">Key vault</span></span>

* <span data-ttu-id="70ea7-1550">Добавлены команды для функций восстановления хранилища ключей:</span><span class="sxs-lookup"><span data-stu-id="70ea7-1550">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="70ea7-1551">`keyvault`, подкоманды `purge`, `recover` и `keyvault list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1551">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="70ea7-1552">`keyvault secret`, подкоманды `backup`, `restore`, `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="70ea7-1552">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="70ea7-1553">`keyvault certificate`, подкоманды `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="70ea7-1553">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="70ea7-1554">`keyvault key`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1554">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="70ea7-1555">Добавлена интеграция хранилища ключей с субъектом-службой (3133).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1555">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="70ea7-1556">Обновлена плоскость данных хранилища ключей до версии 0.3.2</span><span class="sxs-lookup"><span data-stu-id="70ea7-1556">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="70ea7-1557">(3307).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1557">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="70ea7-1558">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="70ea7-1558">Lab</span></span>

* <span data-ttu-id="70ea7-1559">Добавлена поддержка запросов ко всем виртуальным машинам в лаборатории с помощью `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1559">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="70ea7-1560">Добавлен модуль форматирования табличных выходных данных команд `az lab vm list` и `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1560">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="70ea7-1561">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="70ea7-1561">Monitor</span></span>

* <span data-ttu-id="70ea7-1562">Исправлены ошибки с файлом шаблона с помощью команды `monitor autoscale-settings get-parameters-template` (3349).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1562">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="70ea7-1563">Команда `monitor alert-rule-incidents list` переименована в `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1563">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="70ea7-1564">Команда `monitor alert-rule-incidents show` переименована в `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1564">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="70ea7-1565">Команда `monitor metric-defintions list` переименована в `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1565">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="70ea7-1566">Команда `monitor alert-rules` переименована в `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1566">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="70ea7-1567">В команду `monitor alert create` внесены следующие изменения:</span><span class="sxs-lookup"><span data-stu-id="70ea7-1567">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="70ea7-1568">подкоманды `condition` и `action` больше не принимают данные JSON;</span><span class="sxs-lookup"><span data-stu-id="70ea7-1568">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="70ea7-1569">добавлены различные параметры, которые упрощают процесс создания правила;</span><span class="sxs-lookup"><span data-stu-id="70ea7-1569">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="70ea7-1570">параметр `location` больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="70ea7-1570">`location` no longer required</span></span>
  * <span data-ttu-id="70ea7-1571">добавлена поддержка имени и идентификатора для целевого объекта;</span><span class="sxs-lookup"><span data-stu-id="70ea7-1571">Add name and ID support for target</span></span>
  * <span data-ttu-id="70ea7-1572">удален параметр `--alert-rule-resource-name`;</span><span class="sxs-lookup"><span data-stu-id="70ea7-1572">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="70ea7-1573">параметр `is-enabled` переименован в `enabled`, он больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="70ea7-1573">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="70ea7-1574">значения по умолчанию для `description` теперь основаны на указанном условии;</span><span class="sxs-lookup"><span data-stu-id="70ea7-1574">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="70ea7-1575">добавлены примеры, в которых подробно представлен новый формат.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1575">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="70ea7-1576">Поддержка имен или идентификаторов для команд `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1576">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="70ea7-1577">Добавлены вспомогательные аргументы и примеры использования команды `monitor alert rule update`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1577">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="70ea7-1578">Сеть</span><span class="sxs-lookup"><span data-stu-id="70ea7-1578">Network</span></span>

* <span data-ttu-id="70ea7-1579">Добавлена команда `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1579">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="70ea7-1580">Добавлен аргумент `--private-access-services` в команды `vnet subnet create` и `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1580">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="70ea7-1581">Исправлена проблема, из-за которой команда `application-gateway redirect-config create` завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1581">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="70ea7-1582">Исправлена проблема, из-за которой команда `application-gateway redirect-config update` не работала с параметром `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1582">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="70ea7-1583">Исправлена ошибка при использовании аргумента `--servers` с командами `application-gateway address-pool create` и `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1583">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="70ea7-1584">Добавлены команды `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1584">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="70ea7-1585">В команду `application-gateway ssl-policy` добавлены подкоманды `list-options`, `predefined list` и `predefined show`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1585">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="70ea7-1586">В команду `application-gateway ssl-policy set` добавлены аргументы `--name`, `--cipher-suites` и `--min-protocol-version`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1586">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="70ea7-1587">В команды `application-gateway http-settings create` и `application-gateway http-settings update` добавлены аргументы `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe` и `--path`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1587">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="70ea7-1588">В команды `application-gateway url-path-map create` и `application-gateway url-path-map update` добавлены аргументы `--default-redirect-config` и `--redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1588">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="70ea7-1589">Добавлен аргумент `--redirect-config` в команду `application-gateway url-path-map rule create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1589">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="70ea7-1590">Добавлена поддержка параметра `--no-wait` в команде `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1590">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="70ea7-1591">В команды `application-gateway probe create` и `application-gateway probe update` добавлены аргументы `--host-name-from-http-settings`, `--min-servers`, `--match-body` и `--match-status-codes`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1591">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="70ea7-1592">Добавлен аргумент `--redirect-config` в команды `application-gateway rule create` и `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1592">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="70ea7-1593">Добавлена поддержка аргумента `--accelerated-networking` в командах `nic create` и `nic update`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1593">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="70ea7-1594">Удален аргумент `--internal-dns-name-suffix` из команды `nic create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1594">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="70ea7-1595">Добавлена поддержка параметра `--dns-servers` в командах `nic update` и `nic create`. Добавлена поддержка параметра --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1595">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="70ea7-1596">Исправлена ошибка, из-за которой команда `local-gateway create` игнорировала параметр `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1596">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="70ea7-1597">Добавлена поддержка параметра `--dns-servers` в команде `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1597">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="70ea7-1598">Исправлена ошибка при создании пиринга без фильтрации маршрутов с помощью команды `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1598">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="70ea7-1599">Исправлена ошибка, из-за которой аргументы `--provider` и `--bandwidth` не работали с командой `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1599">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="70ea7-1600">Исправлена ошибка с логикой установки значений по умолчанию в команде `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1600">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="70ea7-1601">Улучшено форматирование выходных данных команды `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1601">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="70ea7-1602">В команде `application-gateway http-listener create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1602">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="70ea7-1603">В команде `application-gateway rule create` используются пул адресов, параметры HTTP и прослушиватель HTTP по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1603">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="70ea7-1604">В команде `lb rule create` используются интерфейсный IP-адрес и серверный пул по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1604">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="70ea7-1605">В команде `lb inbound-nat-rule create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1605">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="70ea7-1606">Профиль</span><span class="sxs-lookup"><span data-stu-id="70ea7-1606">Profile</span></span>

* <span data-ttu-id="70ea7-1607">Поддержка входа на виртуальную машину с использованием управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1607">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="70ea7-1608">Поддержка вывода данных команды `account show` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1608">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="70ea7-1609">При использовании параметра --expanded-view отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1609">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="70ea7-1610">Добавлена команда `get-access-token` для предоставления необработанного токена AAD.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1610">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="70ea7-1611">Поддержка входа с учетной записью пользователя без связанных подписок.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1611">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="70ea7-1612">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="70ea7-1612">RDBMS</span></span>

* <span data-ttu-id="70ea7-1613">Поддержка вывода списка серверов в подписке (3417).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1613">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="70ea7-1614">Исправлена проблема, когда объект `%s` не обрабатывался из-за отсутствия `% server_type` (3393).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1614">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="70ea7-1615">Исправлено сопоставление источника документа и добавлена задача непрерывной интеграции для проверки (3361).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1615">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="70ea7-1616">Исправлена справка по MySQL и PostgreSQL (3369).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1616">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="70ea7-1617">Ресурс</span><span class="sxs-lookup"><span data-stu-id="70ea7-1617">Resource</span></span>

* <span data-ttu-id="70ea7-1618">Улучшены запросы на ввод отсутствующих параметров для команды `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1618">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="70ea7-1619">Улучшен анализ синтаксиса `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1619">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="70ea7-1620">Исправлены проблемы, из-за которых файлы параметров `group deployment create` не распознавались с использованием синтаксиса `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1620">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="70ea7-1621">Поддержка аргумента `--ids` в командах `resource` и `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1621">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="70ea7-1622">Исправлены некоторые сообщения об ошибках и анализе (3584).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1622">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="70ea7-1623">Исправлены ошибки анализа параметра `--resource-type` в команде `lock`. Теперь принимаются `<resource-namespace>` и `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1623">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="70ea7-1624">Добавлена проверка параметров для шаблонов для ссылок на шаблоны (3629).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1624">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="70ea7-1625">Добавлена поддержка указания параметров развертывания с использованием синтаксиса `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1625">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="70ea7-1626">Роль</span><span class="sxs-lookup"><span data-stu-id="70ea7-1626">Role</span></span>

* <span data-ttu-id="70ea7-1627">Поддержка вывода данных команды `create-for-rbac` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1627">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="70ea7-1628">Добавлена очистка назначений ролей и связанного приложения AAD при удалении субъекта-службы (3610).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1628">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="70ea7-1629">В описания аргументов `--start-date` и `--end-date` команды `app create` добавлен формат времени.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1629">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="70ea7-1630">При использовании параметра `--expanded-view` отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1630">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="70ea7-1631">Добавлена интеграция хранилища ключей для команд `create-for-rbac` и `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1631">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="70ea7-1632">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="70ea7-1632">Service Fabric</span></span>
* <span data-ttu-id="70ea7-1633">Исправлена ошибка, из-за которой большие файлы в приложениях усекались при отправке (3666).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1633">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="70ea7-1634">Добавлены тесты для команд Service Fabric (3424).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1634">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="70ea7-1635">Исправлены многие команды Service Fabric (3234).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1635">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="70ea7-1636">SQL</span><span class="sxs-lookup"><span data-stu-id="70ea7-1636">SQL</span></span>

* <span data-ttu-id="70ea7-1637">Удален недействительный параметр `--identity` команды `sql server create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1637">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="70ea7-1638">Удалены значения паролей из выходных данных команд `sql server create` и `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1638">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="70ea7-1639">Добавлены команды `sql db list-editions` и `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1639">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="70ea7-1640">Хранилище</span><span class="sxs-lookup"><span data-stu-id="70ea7-1640">Storage</span></span>

* <span data-ttu-id="70ea7-1641">Удален параметр `--marker` из команд `storage blob list`, `storage container list` и `storage share list` (3745).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1641">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="70ea7-1642">Включено создание учетных записей хранения с поддержкой только HTTPS.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1642">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="70ea7-1643">Обновлены метрики хранилища, команды входа и CORS (3495).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1643">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="70ea7-1644">Перефразировано сообщение об исключении, которое выводит команда добавления CORS (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="70ea7-1644">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="70ea7-1645">Генератор преобразован в список в режиме пробного выполнения команды пакетной загрузки (3592).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1645">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="70ea7-1646">Исправлена проблема при пробном выполнении команды пакетной загрузки больших двоичных объектов (3640) (3592).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1646">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="70ea7-1647">ВМ</span><span class="sxs-lookup"><span data-stu-id="70ea7-1647">VM</span></span>

* <span data-ttu-id="70ea7-1648">Поддержка настройки NSG.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1648">Support configuring nsg</span></span>
* <span data-ttu-id="70ea7-1649">Исправлена ошибка, из-за которой не удавалось правильно настроить DNS-сервер.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1649">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="70ea7-1650">Поддержка удостоверений управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1650">Support managed service identities</span></span>
* <span data-ttu-id="70ea7-1651">Исправлена проблема, из-за которой для команды `cmss create` с существующей подсистемой балансировки нагрузки требовался параметр `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1651">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="70ea7-1652">Теперь нумерация LUN дисков данных, создаваемых с помощью команды `vm image create`, начинается с 0.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1652">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="70ea7-1653">10 мая 2017 г.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1653">May 10, 2017</span></span>

<span data-ttu-id="70ea7-1654">Версия 2.0.6</span><span class="sxs-lookup"><span data-stu-id="70ea7-1654">Version 2.0.6</span></span>

* <span data-ttu-id="70ea7-1655">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1655">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="70ea7-1656">Добавлена реляционная СУБД (MySQL, Postgres).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1656">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="70ea7-1657">Добавлены модули Data Lake Store и Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1657">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="70ea7-1658">Добавлен модуль Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1658">Include Cognitive Services module</span></span>
* <span data-ttu-id="70ea7-1659">Добавлен модуль Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1659">Include Service Fabric module</span></span>
* <span data-ttu-id="70ea7-1660">Добавлен модуль Interactive (az-shell переименован).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1660">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="70ea7-1661">Добавлена поддержка команд CDN.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1661">Add support for CDN commands</span></span>
* <span data-ttu-id="70ea7-1662">Удален модуль Container.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1662">Remove Container module</span></span>
* <span data-ttu-id="70ea7-1663">Добавлена команда az -v для az --version ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1663">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="70ea7-1664">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1664">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="70ea7-1665">Core</span><span class="sxs-lookup"><span data-stu-id="70ea7-1665">Core</span></span>

* <span data-ttu-id="70ea7-1666">Ядро: запись исключений, порожденных незарегистрированным поставщиком, и его автоматическая регистрация.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1666">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="70ea7-1667">Производительность: сохранение кэша маркеров библиотеки ADAL в памяти до завершения работы процесса ([№ 2603](https://github.com/Azure/azure-cli/issues/2603)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1667">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="70ea7-1668">Исправление байтов, возвращаемых из шестнадцатеричных отпечатков -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1668">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="70ea7-1669">Улучшенное скачивание сертификатов Key Vault и интеграция субъектов-служб AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1669">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="70ea7-1670">Добавлено расположение Python в az -version ([#2986](https://github.com/Azure/azure-cli/issues/2986)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1670">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="70ea7-1671">Вход: поддержка входа при отсутствии подписок ([#2929](https://github.com/Azure/azure-cli/issues/2929)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1671">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="70ea7-1672">Ядро: устранен сбой при двукратном входе с помощью субъекта-службы ([#2800](https://github.com/Azure/azure-cli/issues/2800)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1672">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="70ea7-1673">Ядро: возможность настроить путь к файлу accessTokens.json с помощью env var ([#2605](https://github.com/Azure/azure-cli/issues/2605)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1673">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="70ea7-1674">Ядро: возможность применять настроенные параметры по умолчанию к необязательным аргументам ([№ 2703](https://github.com/Azure/azure-cli/issues/2703)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1674">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="70ea7-1675">Ядро: повышение производительности.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1675">core: Improved performance</span></span>
* <span data-ttu-id="70ea7-1676">Ядро: настаиваемые сертификаты ЦС — поддержка настройки переменной среды REQUESTS_CA_BUNDLE.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1676">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="70ea7-1677">Ядро: облачная конфигурация — использование конечной точки Resource Manager, если не задана конечная точка управления.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1677">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="70ea7-1678">ACS</span><span class="sxs-lookup"><span data-stu-id="70ea7-1678">ACS</span></span>

* <span data-ttu-id="70ea7-1679">Исправление: теперь значение счетчика баз данных master и агентов — целое число, а не строка.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1679">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="70ea7-1680">Предоставлены команды az acs create --no-wait и az acs wait для асинхронного создания.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1680">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="70ea7-1681">Предоставлена команда az acs create --validate для пробного создания.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1681">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="70ea7-1682">Удален профиль Windows перед вызовом метода PUT для команды scale ([№ 2755](https://github.com/Azure/azure-cli/issues/2755)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1682">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="70ea7-1683">AppService</span><span class="sxs-lookup"><span data-stu-id="70ea7-1683">AppService</span></span>

* <span data-ttu-id="70ea7-1684">Приложение-функция: добавлена полная поддержка приложений-функций, включая создание, отображение, вывод списка, удаление, настройку имени узла, настройку протокола SSL и т. д.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1684">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="70ea7-1685">Добавлены службы Team Services (VSTS) в качестве параметра непрерывной доставки в конфигурации веб-системы управления версиями службы приложений.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1685">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="70ea7-1686">Создана команда az webapp, заменяющая команду az appservice web (для обеспечения обратной совместимости команда az appservice web будет оставлена еще в двух выпусках).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1686">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="70ea7-1687">Предоставлены аргументы для настройки развертывания и стеков времени выполнения при создании веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1687">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="70ea7-1688">Предоставлена команда webapp list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1688">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="70ea7-1689">Поддержка настройки строк подключения ([№ 2647](https://github.com/Azure/azure-cli/issues/2647)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1689">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="70ea7-1690">Поддержка переключения слотов с предварительным просмотром.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1690">support slot swap with preview</span></span>
* <span data-ttu-id="70ea7-1691">Устранены ошибки из команд службы приложений ([№ 2948](https://github.com/Azure/azure-cli/issues/2948)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1691">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="70ea7-1692">Использование группы ресурсов в плане служб приложений для операций с сертификатами ([№ 2750](https://github.com/Azure/azure-cli/issues/2750)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1692">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="70ea7-1693">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="70ea7-1693">CosmosDB</span></span>

* <span data-ttu-id="70ea7-1694">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1694">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="70ea7-1695">Добавлена поддержка интерфейсов API уровня данных DocumentDB: управление базами данных и коллекциями.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1695">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="70ea7-1696">Добавлена поддержка включения автоматической отработки отказа для учетных записей базы данных.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1696">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="70ea7-1697">Добавлена поддержка нового параметра ConsistentPrefix политики согласованности.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1697">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="70ea7-1698">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="70ea7-1698">Data Lake Analytics</span></span>

* <span data-ttu-id="70ea7-1699">Исправлена ошибка, из-за которой фильтрация списков заданий по результату и состоянию вызывала сбой.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1699">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="70ea7-1700">Добавлена поддержка нового типа элемента каталога — пакета.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1700">Add support for new catalog item type: package.</span></span> <span data-ttu-id="70ea7-1701">Для доступа к нему используется `az dla catalog package`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1701">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="70ea7-1702">Появилась возможность вывести список следующих элементов каталога из базы данных (указание схемы не требуется):</span><span class="sxs-lookup"><span data-stu-id="70ea7-1702">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="70ea7-1703">Таблица</span><span class="sxs-lookup"><span data-stu-id="70ea7-1703">Table</span></span>
  * <span data-ttu-id="70ea7-1704">функция с табличным значением;</span><span class="sxs-lookup"><span data-stu-id="70ea7-1704">Table valued function</span></span>
  * <span data-ttu-id="70ea7-1705">Просмотр</span><span class="sxs-lookup"><span data-stu-id="70ea7-1705">View</span></span>
  * <span data-ttu-id="70ea7-1706">статистика таблицы.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1706">Table Statistics.</span></span> <span data-ttu-id="70ea7-1707">Их можно также вывести с помощью схемы, но без указания имени таблицы.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1707">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="70ea7-1708">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="70ea7-1708">Data Lake Store</span></span>

* <span data-ttu-id="70ea7-1709">Обновлена версия пакета SDK базовой файловой системы, что обеспечивает лучшую поддержку сценариев регулирования на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1709">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="70ea7-1710">Повышена производительность загрузки пакетов и выполнения команд ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1710">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="70ea7-1711">Отсутствовала справка для команды access show.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1711">missed help for access show.</span></span> <span data-ttu-id="70ea7-1712">Теперь она добавлена.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1712">adding it.</span></span> <span data-ttu-id="70ea7-1713">([№ 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="70ea7-1713">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="70ea7-1714">Поиск</span><span class="sxs-lookup"><span data-stu-id="70ea7-1714">Find</span></span>

* <span data-ttu-id="70ea7-1715">Улучшены результаты поиска и разрешено управление версиями индекса поиска.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1715">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="70ea7-1716">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="70ea7-1716">KeyVault</span></span>

* <span data-ttu-id="70ea7-1717">BC: в команде `az keyvault certificate download` параметр -e со строкового или двоичного значения изменен на PEM или DER, чтобы лучше представить параметры.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1717">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="70ea7-1718">BC: из команды `keyvault certificate create` удалены параметры --expires и --not-before, так как они не поддерживаются службой.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1718">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="70ea7-1719">В команду `keyvault certificate create` добавлен параметр --validity для выборочного переопределения значение в параметре --policy.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1719">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="70ea7-1720">Исправлена ошибка в команде `keyvault certificate get-default-policy`, в которой были доступны параметры expires и not_before, а параметр validity_in_months — нет.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1720">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="70ea7-1721">Добавлено исправление для модуля keyvault для импорта PEM- и PFX-файлов ([#2754](https://github.com/Azure/azure-cli/issues/2754)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1721">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="70ea7-1722">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="70ea7-1722">Lab</span></span>

* <span data-ttu-id="70ea7-1723">Добавлены команды создания, отображения, удаления и вывода списка для среды в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1723">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="70ea7-1724">Добавлены команды отображения и вывода списка для просмотра шаблонов ARM в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1724">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="70ea7-1725">В команду `az lab vm list` добавлен флаг --environment для фильтрации виртуальных машин по среде в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1725">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="70ea7-1726">Добавлена вспомогательная команда `az lab formula export-artifacts` для экспорта шаблона артефакта в формуле лаборатории.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1726">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="70ea7-1727">Добавлены команды для управления секретами в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1727">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="70ea7-1728">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="70ea7-1728">Monitor</span></span>

* <span data-ttu-id="70ea7-1729">Исправление ошибки: моделирование `--actions` в `az alert-rules create` для использования строки в формате JSON ([№ 3009](https://github.com/Azure/azure-cli/issues/3009)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1729">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="70ea7-1730">Исправление ошибки: при создании параметров диагностики не принимались журналы и метрики из команды show ([№ 2913](https://github.com/Azure/azure-cli/issues/2913)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1730">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="70ea7-1731">Сеть</span><span class="sxs-lookup"><span data-stu-id="70ea7-1731">Network</span></span>

* <span data-ttu-id="70ea7-1732">Добавлена команда `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1732">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="70ea7-1733">Добавлена поддержка параметра `--filters` в команде `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1733">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="70ea7-1734">Добавлена поддержка фильтрации подключений шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1734">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="70ea7-1735">Добавлена поддержка конфигурации набора правил WAF шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1735">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="70ea7-1736">Добавлена поддержка правил и фильтров маршрутов ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1736">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="70ea7-1737">Добавлена поддержка географической маршрутизации диспетчера трафика.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1737">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="70ea7-1738">Добавлена поддержка селекторов трафика на основе политик для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1738">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="70ea7-1739">Добавлена поддержка политик IPSec для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1739">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="70ea7-1740">Исправлена ошибка `vpn-connection create`, возникавшая при использовании параметра `--no-wait` или `--validate`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1740">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="70ea7-1741">Добавлена поддержка шлюзов виртуальной сети "активный-активный".</span><span class="sxs-lookup"><span data-stu-id="70ea7-1741">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="70ea7-1742">Удалены значения NULL из выходных данных команды `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1742">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="70ea7-1743">BC: исправлена ошибка в выходных данных `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1743">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="70ea7-1744">Исправлена ошибка, приводившая к неправильному анализу аргумента --key-length команды vpn-connection create.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1744">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="70ea7-1745">Исправлена ошибка в `dns zone import`, из-за которой записи не импортировались правильно.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1745">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="70ea7-1746">Исправлена ошибка, из-за которой команда `traffic-manager endpoint update` не работала.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1746">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="70ea7-1747">Добавлены команды предварительного просмотра для Наблюдателя за сетями.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1747">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="70ea7-1748">Профиль</span><span class="sxs-lookup"><span data-stu-id="70ea7-1748">Profile</span></span>

* <span data-ttu-id="70ea7-1749">Поддержка входа при отсутствии подписок ([№ 2560](https://github.com/Azure/azure-cli/issues/2560)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1749">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="70ea7-1750">Поддержка сокращенных имен параметров в команде az account set --subscription ([№ 2980](https://github.com/Azure/azure-cli/issues/2980)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1750">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="70ea7-1751">Redis</span><span class="sxs-lookup"><span data-stu-id="70ea7-1751">Redis</span></span>

* <span data-ttu-id="70ea7-1752">Добавлена команда update, которая также добавляет возможность масштабирования для кэша Redis.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1752">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="70ea7-1753">Команда update-settings объявляется нерекомендуемой.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1753">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="70ea7-1754">Ресурс</span><span class="sxs-lookup"><span data-stu-id="70ea7-1754">Resource</span></span>

* <span data-ttu-id="70ea7-1755">Добавлены команды определения managedapp и managedapp ([№ 2985](https://github.com/Azure/azure-cli/issues/2985)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1755">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="70ea7-1756">Включена поддержка команд provider operation ([#2908](https://github.com/Azure/azure-cli/issues/2908)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1756">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="70ea7-1757">Поддержка создания универсального ресурса ([№ 2606](https://github.com/Azure/azure-cli/issues/2606)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1757">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="70ea7-1758">Исправлен анализ ресурсов и поиск версии API.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1758">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="70ea7-1759">([№ 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="70ea7-1759">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="70ea7-1760">Добавлены документы для команды az lock update.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1760">Add docs for az lock update.</span></span> <span data-ttu-id="70ea7-1761">([№ 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="70ea7-1761">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="70ea7-1762">Исправлена ошибка, возникавшая при попытке вывести список ресурсов группы, которая не существует.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1762">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="70ea7-1763">([№ 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="70ea7-1763">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="70ea7-1764">[Вычисления.] Устранены проблемы с масштабируемым набором виртуальных машин и обновлением группы доступности виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1764">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="70ea7-1765">([№ 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="70ea7-1765">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="70ea7-1766">Исправлена блокировка создания и удаления, возникающая, если параметр parent-resource-path не указан ([№ 2742](https://github.com/Azure/azure-cli/issues/2742)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1766">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="70ea7-1767">Роль</span><span class="sxs-lookup"><span data-stu-id="70ea7-1767">Role</span></span>

* <span data-ttu-id="70ea7-1768">create-for-rbac: гарантируется, что дата завершения работы поставщика служб не может превышать срок действия сертификата ([№ 2989](https://github.com/Azure/azure-cli/issues/2989)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1768">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="70ea7-1769">RBAC: добавлена полная поддержка команды ad group ([#2016](https://github.com/Azure/azure-cli/issues/2016)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1769">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="70ea7-1770">Роль: устранены проблемы при обновлении определения роли ([№ 2745](https://github.com/Azure/azure-cli/issues/2745)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1770">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="70ea7-1771">create-for-rbac: обеспечен выбор введенного пользователем пароля.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1771">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="70ea7-1772">SQL</span><span class="sxs-lookup"><span data-stu-id="70ea7-1772">SQL</span></span>

* <span data-ttu-id="70ea7-1773">Добавлены команды az sql server list-usages и az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1773">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="70ea7-1774">SQL: добавлена возможность прямого подключения к поставщику ресурса ([#2832](https://github.com/Azure/azure-cli/issues/2832)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1774">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="70ea7-1775">Хранилище</span><span class="sxs-lookup"><span data-stu-id="70ea7-1775">Storage</span></span>

* <span data-ttu-id="70ea7-1776">Добавлено расположение по умолчанию группы ресурсов для `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1776">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="70ea7-1777">Добавлена поддержка добавочного копирования больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1777">Add support for incremental blob copy</span></span>
* <span data-ttu-id="70ea7-1778">Добавлена поддержка передачи больших блочных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1778">Add support for large block blob upload</span></span>
* <span data-ttu-id="70ea7-1779">Размер блока изменяется и составляет 100 МБ, если передается файл, чей размер превышает 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1779">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="70ea7-1780">ВМ</span><span class="sxs-lookup"><span data-stu-id="70ea7-1780">VM</span></span>

* <span data-ttu-id="70ea7-1781">avail-set: число доменов обновления и доменов сбоя сделано необязательным.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1781">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="70ea7-1782">Примечание. Команды виртуальной машины в независимых облаках: избегайте использовать функции, связанные с Управляемыми дисками, включая следующие:</span><span class="sxs-lookup"><span data-stu-id="70ea7-1782">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="70ea7-1783">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="70ea7-1783">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="70ea7-1784">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="70ea7-1784">az vm/vmss disk</span></span>
  3. <span data-ttu-id="70ea7-1785">В команде az vm/vmss create используйте параметр --use-unmanaged-disk, чтобы избежать использования Управляемых дисков. Другие команды должны работать.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1785">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="70ea7-1786">vm/vmss: улучшен текст предупреждения при создании пары ключей SSH.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1786">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="70ea7-1787">vm/vmss: поддержка создания из образа Marketplace, для которого требуются сведения о плане ([№ 1209](https://github.com/Azure/azure-cli/issues/1209)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1787">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="70ea7-1788">3 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1788">April 3, 2017</span></span>

<span data-ttu-id="70ea7-1789">Версия 2.0.2</span><span class="sxs-lookup"><span data-stu-id="70ea7-1789">Version 2.0.2</span></span>

<span data-ttu-id="70ea7-1790">В этом выпуске мы добавили компоненты ACR, Batch, KeyVault и SQL.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1790">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="70ea7-1791">Core</span><span class="sxs-lookup"><span data-stu-id="70ea7-1791">Core</span></span>

* <span data-ttu-id="70ea7-1792">Модули Acr, Lab, Monitor и Find добавлены в список по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1792">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="70ea7-1793">Вход: пропуск неправильного клиента ([#2634](https://github.com/Azure/azure-cli/pull/2634)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1793">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="70ea7-1794">Вход: для подписки по умолчанию задано значение 1 с состоянием "Включено" ([#2575](https://github.com/Azure/azure-cli/pull/2575)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1794">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="70ea7-1795">Добавлена поддержка команд wait и --no-wait для дополнительных команд ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1795">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="70ea7-1796">Core: поддержка входа при помощи субъекта-службы с использованием сертификата ([#2457](https://github.com/Azure/azure-cli/pull/2457)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1796">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="70ea7-1797">Добавлен запрос для отсутствующих параметров шаблона</span><span class="sxs-lookup"><span data-stu-id="70ea7-1797">Add prompting for missing template parameters.</span></span> <span data-ttu-id="70ea7-1798">([#2364](https://github.com/Azure/azure-cli/pull/2364)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1798">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="70ea7-1799">Добавлена поддержка установки параметров по умолчанию для таких распространенных аргументов, как группа ресурсов по умолчанию, веб-страница по умолчанию, виртуальная машина по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1799">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="70ea7-1800">Добавлена поддержка входа на конкретный клиент.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1800">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="70ea7-1801">ACS</span><span class="sxs-lookup"><span data-stu-id="70ea7-1801">ACS</span></span>

* <span data-ttu-id="70ea7-1802">[ACS] Добавлена поддержка настройки кластера ACS по умолчанию ([#2554](https://github.com/Azure/azure-cli/pull/2554)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1802">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="70ea7-1803">Добавлена поддержка запроса пароля для ключа SSH</span><span class="sxs-lookup"><span data-stu-id="70ea7-1803">Add support for ssh key password prompting.</span></span> <span data-ttu-id="70ea7-1804">([#2044](https://github.com/Azure/azure-cli/pull/2044)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1804">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="70ea7-1805">Добавлена поддержка кластеров Windows</span><span class="sxs-lookup"><span data-stu-id="70ea7-1805">Add support for windows clusters.</span></span> <span data-ttu-id="70ea7-1806">([#2211](https://github.com/Azure/azure-cli/pull/2211)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1806">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="70ea7-1807">Добавлена возможность изменения роли "Владелец" на роль "Участник"</span><span class="sxs-lookup"><span data-stu-id="70ea7-1807">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="70ea7-1808">([#2321](https://github.com/Azure/azure-cli/pull/2321)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1808">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="70ea7-1809">AppService</span><span class="sxs-lookup"><span data-stu-id="70ea7-1809">AppService</span></span>

* <span data-ttu-id="70ea7-1810">AppService: добавлена поддержка получения внешнего IP-адреса, используемого для записей DNS типа A ([#2627](https://github.com/Azure/azure-cli/pull/2627)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1810">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="70ea7-1811">AppService: добавлена поддержка привязки групповых сертификатов ([#2625](https://github.com/Azure/azure-cli/pull/2625)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1811">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="70ea7-1812">AppService: добавлена поддержка профилей для публикации списком ([#2504](https://github.com/Azure/azure-cli/pull/2504)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1812">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="70ea7-1813">AppService: добавлен триггер синхронизации с системой управления версиями после настройки ([#2326](https://github.com/Azure/azure-cli/pull/2326)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1813">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="70ea7-1814">Data Lake</span><span class="sxs-lookup"><span data-stu-id="70ea7-1814">DataLake</span></span>

* <span data-ttu-id="70ea7-1815">Первый выпуск модуля Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1815">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="70ea7-1816">Первый выпуск модуля Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1816">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="70ea7-1817">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="70ea7-1817">DocuemntDB</span></span>

* <span data-ttu-id="70ea7-1818">DocumentDB: добавлена поддержка для получения списка строк подключения ([#2580](https://github.com/Azure/azure-cli/pull/2580)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1818">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="70ea7-1819">ВМ</span><span class="sxs-lookup"><span data-stu-id="70ea7-1819">VM</span></span>

* <span data-ttu-id="70ea7-1820">[Вычисления] Добавлена поддержка AppGateway для создания масштабируемого набора виртуальных машин ([#2570](https://github.com/Azure/azure-cli/pull/2570)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1820">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="70ea7-1821">[ВМ и VMSS] Улучшена поддержка кэширования диска ([#2522](https://github.com/Azure/azure-cli/pull/2522)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1821">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="70ea7-1822">ВМ и VMSS: внедрена логика проверки учетных данных, используемая на портале ([#2537](https://github.com/Azure/azure-cli/pull/2537)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1822">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="70ea7-1823">Добавлена поддержка команд wait и --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1823">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="70ea7-1824">Масштабируемый набор виртуальных машин: добавлена поддержка \* для представления экземпляров на виртуальных машинах в виде списка ([#2467](https://github.com/Azure/azure-cli/pull/2467)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1824">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="70ea7-1825">Добавлен параметр --secrets для виртуальной машины и масштабируемого набора виртуальных машин ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1825">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="70ea7-1826">Добавлено разрешение на создание виртуальных машин на основе специализированного образа VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256)).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1826">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="70ea7-1827">27 февраля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1827">February 27, 2017</span></span>

<span data-ttu-id="70ea7-1828">Версия 2.0.0</span><span class="sxs-lookup"><span data-stu-id="70ea7-1828">Version 2.0.0</span></span>

<span data-ttu-id="70ea7-1829">Этот первый общедоступный выпуск Azure CLI 2.0. Общедоступными являются такие командные модули:</span><span class="sxs-lookup"><span data-stu-id="70ea7-1829">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="70ea7-1830">служба контейнеров (ACS);</span><span class="sxs-lookup"><span data-stu-id="70ea7-1830">Container Service (acs)</span></span>
- <span data-ttu-id="70ea7-1831">вычисления (в том числе Resource Manager, виртуальная машина, масштабируемые наборы виртуальных машин, управляемые диски);</span><span class="sxs-lookup"><span data-stu-id="70ea7-1831">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="70ea7-1832">Сеть</span><span class="sxs-lookup"><span data-stu-id="70ea7-1832">Networking</span></span>
- <span data-ttu-id="70ea7-1833">Хранилище</span><span class="sxs-lookup"><span data-stu-id="70ea7-1833">Storage</span></span>

<span data-ttu-id="70ea7-1834">Эти командные модули могут использоваться в рабочих средах. Они поддерживаются стандартными соглашениями Майкрософт об уровне обслуживания. Вы можете отправлять запросы непосредственно в службу технической поддержки Майкрософт или добавлять описание проблем в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/). Вы можете задавать вопросы на [сайте StackOverflow, используя тег azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), или обращаться к группе разработчиков по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Можно отправлять отзывы из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1834">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="70ea7-1835">Команды в этих модулях стабильны, и предполагается, что в следующих выпусках этой версии Azure CLI их синтаксис не будет меняться.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1835">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="70ea7-1836">Проверить версию CLI можно с помощью команды `az --version`. В выходных данных указана версия самого интерфейса командной строки (2.0.0 в этом выпуске), версии отдельных командных модулей и используемые вами версии Python и GCC.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1836">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="70ea7-1837">Некоторые командные модули имеют постфикс b*n* или rc*n*. Эти командные модули все еще находятся на стадии предварительной версии и станут общедоступными в будущем.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1837">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="70ea7-1838">У нас также есть предварительные ежедневные сборки CLI. Дополнительные сведения см. в инструкциях по [получению ежедневных сборок](https://github.com/Azure/azure-cli#nightly-builds), а также в инструкциях по [настройке среды разработки и участии в написании кода](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="70ea7-1838">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="70ea7-1839">О проблемах с предварительными ежедневными сборками можно сообщить несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="70ea7-1839">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="70ea7-1840">добавив информацию о проблемах в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/);</span><span class="sxs-lookup"><span data-stu-id="70ea7-1840">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="70ea7-1841">Свяжитесь с командой разработчиков ([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)),</span><span class="sxs-lookup"><span data-stu-id="70ea7-1841">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="70ea7-1842">отправив отзыв из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="70ea7-1842">Provide feedback from the command line with the `az feedback` command</span></span>

